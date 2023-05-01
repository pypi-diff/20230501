# Comparing `tmp/CLAM-3.2.5.tar.gz` & `tmp/CLAM-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CLAM-3.2.5.tar", last modified: Thu Mar  2 09:02:33 2023, max compression
+gzip compressed data, was "CLAM-3.2.6.tar", last modified: Mon May  1 10:51:17 2023, max compression
```

## Comparing `CLAM-3.2.5.tar` & `CLAM-3.2.6.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.120507 CLAM-3.2.5/
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.087174 CLAM-3.2.5/CLAM.egg-info/
--rw-r--r--   0 proycon   (1000) users      (100)     6438 2023-03-02 09:02:32.000000 CLAM-3.2.5/CLAM.egg-info/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)     3638 2023-03-02 09:02:33.000000 CLAM-3.2.5/CLAM.egg-info/SOURCES.txt
--rw-r--r--   0 proycon   (1000) users      (100)        1 2023-03-02 09:02:32.000000 CLAM-3.2.5/CLAM.egg-info/dependency_links.txt
--rw-r--r--   0 proycon   (1000) users      (100)      213 2023-03-02 09:02:32.000000 CLAM-3.2.5/CLAM.egg-info/entry_points.txt
--rw-r--r--   0 proycon   (1000) users      (100)       85 2023-03-02 09:02:32.000000 CLAM-3.2.5/CLAM.egg-info/requires.txt
--rw-r--r--   0 proycon   (1000) users      (100)        5 2023-03-02 09:02:32.000000 CLAM-3.2.5/CLAM.egg-info/top_level.txt
--rw-r--r--   0 proycon   (1000) users      (100)    35147 2018-11-21 13:07:01.000000 CLAM-3.2.5/COPYING
--rw-r--r--   0 proycon   (1000) users      (100)      390 2018-11-21 13:07:01.000000 CLAM-3.2.5/MANIFEST.in
--rw-r--r--   0 proycon   (1000) users      (100)     6438 2023-03-02 09:02:33.120507 CLAM-3.2.5/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)     5500 2022-11-17 14:55:17.000000 CLAM-3.2.5/README.rst
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.087174 CLAM-3.2.5/clam/
--rwxr-xr-x   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/__init__.py
--rwxr-xr-x   0 proycon   (1000) users      (100)    11712 2021-01-07 16:02:30.000000 CLAM-3.2.5/clam/clamclient.py
--rwxr-xr-x   0 proycon   (1000) users      (100)    11350 2023-03-01 13:22:18.000000 CLAM-3.2.5/clam/clamdispatcher.py
--rwxr-xr-x   0 proycon   (1000) users      (100)    16379 2022-11-16 20:18:23.000000 CLAM-3.2.5/clam/clamnewproject.py
--rw-r--r--   0 proycon   (1000) users      (100)      473 2016-04-29 13:30:48.000000 CLAM-3.2.5/clam/clamrunjob.py
--rwxr-xr-x   0 proycon   (1000) users      (100)   175893 2022-11-29 12:59:14.000000 CLAM-3.2.5/clam/clamservice.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.087174 CLAM-3.2.5/clam/clients/
--rw-r--r--   0 proycon   (1000) users      (100)     2434 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/clients/clienttest.py
--rw-r--r--   0 proycon   (1000) users      (100)     4578 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/clients/textstats.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.090507 CLAM-3.2.5/clam/common/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/common/__init__.py
--rw-r--r--   0 proycon   (1000) users      (100)    26603 2022-11-22 17:37:08.000000 CLAM-3.2.5/clam/common/auth.py
--rw-r--r--   0 proycon   (1000) users      (100)    25383 2022-11-22 12:43:49.000000 CLAM-3.2.5/clam/common/client.py
--rw-r--r--   0 proycon   (1000) users      (100)     4572 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/common/converters.py
--rw-r--r--   0 proycon   (1000) users      (100)   136423 2023-03-01 13:22:06.000000 CLAM-3.2.5/clam/common/data.py
--rw-r--r--   0 proycon   (1000) users      (100)      339 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/common/digestauth.py
--rw-r--r--   0 proycon   (1000) users      (100)    12172 2022-11-17 13:48:36.000000 CLAM-3.2.5/clam/common/formats.py
--rw-r--r--   0 proycon   (1000) users      (100)      978 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/common/languages.py
--rw-r--r--   0 proycon   (1000) users      (100)     2403 2022-11-15 14:00:38.000000 CLAM-3.2.5/clam/common/oauth.py
--rw-r--r--   0 proycon   (1000) users      (100)    26953 2019-12-14 12:33:12.000000 CLAM-3.2.5/clam/common/parameters.py
--rw-r--r--   0 proycon   (1000) users      (100)      549 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/common/status.py
--rw-r--r--   0 proycon   (1000) users      (100)     5872 2022-11-17 14:27:35.000000 CLAM-3.2.5/clam/common/util.py
--rw-r--r--   0 proycon   (1000) users      (100)     9864 2021-01-12 12:04:36.000000 CLAM-3.2.5/clam/common/viewers.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.093840 CLAM-3.2.5/clam/config/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/__init__.py
--rw-r--r--   0 proycon   (1000) users      (100)     6507 2019-10-30 11:21:07.000000 CLAM-3.2.5/clam/config/actiontest.py
--rw-r--r--   0 proycon   (1000) users      (100)     6654 2020-02-27 10:24:17.000000 CLAM-3.2.5/clam/config/authactiontest.py
--rw-r--r--   0 proycon   (1000) users      (100)     6964 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/authtest.py
--rw-r--r--   0 proycon   (1000) users      (100)     5994 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/config/constrainttest.py
--rw-r--r--   0 proycon   (1000) users      (100)     6805 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/defaults.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     1457 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/example.wsgi
--rw-r--r--   0 proycon   (1000) users      (100)     6931 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/forwardauthtest.py
--rw-r--r--   0 proycon   (1000) users      (100)     6020 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/freqlist.py
--rw-r--r--   0 proycon   (1000) users      (100)     5921 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/config/multiplier.py
--rw-r--r--   0 proycon   (1000) users      (100)     7913 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/config/oauthtest.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     1719 2022-11-16 15:35:51.000000 CLAM-3.2.5/clam/config/setup_template.py
--rw-r--r--   0 proycon   (1000) users      (100)     3135 2022-11-16 19:57:09.000000 CLAM-3.2.5/clam/config/template.Dockerfile
--rw-r--r--   0 proycon   (1000) users      (100)     3168 2022-11-22 12:11:07.000000 CLAM-3.2.5/clam/config/template.config.yml
--rw-r--r--   0 proycon   (1000) users      (100)    12906 2022-11-16 13:44:37.000000 CLAM-3.2.5/clam/config/template.py
--rw-r--r--   0 proycon   (1000) users      (100)     5672 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/test.py
--rw-r--r--   0 proycon   (1000) users      (100)     5693 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/config/test2.py
--rw-r--r--   0 proycon   (1000) users      (100)     9601 2021-04-28 10:09:47.000000 CLAM-3.2.5/clam/config/textstats.py
--rw-r--r--   0 proycon   (1000) users      (100)     7934 2016-03-23 20:44:08.000000 CLAM-3.2.5/clam/config/textstats1.py
--rw-rw-r--   0 proycon   (1000) users      (100)     7341 2015-12-18 13:06:50.000000 CLAM-3.2.5/clam/config/textstats2.py
--rw-r--r--   0 proycon   (1000) users      (100)     7815 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/config/textstats3.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.113840 CLAM-3.2.5/clam/static/
--rw-r--r--   0 proycon   (1000) users      (100)    25376 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/ajaxupload.js
--rw-r--r--   0 proycon   (1000) users      (100)      440 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/back.png
--rw-r--r--   0 proycon   (1000) users      (100)     5010 2021-01-07 16:02:34.000000 CLAM-3.2.5/clam/static/base.css
--rw-r--r--   0 proycon   (1000) users      (100)   155758 2019-02-13 16:40:50.000000 CLAM-3.2.5/clam/static/bootstrap.min.css
--rw-r--r--   0 proycon   (1000) users      (100)    58072 2019-02-13 16:40:57.000000 CLAM-3.2.5/clam/static/bootstrap.min.js
--rw-r--r--   0 proycon   (1000) users      (100)    32913 2022-11-15 16:39:27.000000 CLAM-3.2.5/clam/static/clam.js
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.113840 CLAM-3.2.5/clam/static/custom/
--rw-r--r--   0 proycon   (1000) users      (100)      684 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/custom/sonardropbox_index.html
--rw-r--r--   0 proycon   (1000) users      (100)      115 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/custom/sonardropbox_projectdone.html
--rw-r--r--   0 proycon   (1000) users      (100)     2899 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/custom/sonardropbox_projectstart.html
--rw-r--r--   0 proycon   (1000) users      (100)      820 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/delete.png
--rw-r--r--   0 proycon   (1000) users      (100)     4001 2020-10-27 09:49:52.000000 CLAM-3.2.5/clam/static/fine-uploader.min.css
--rw-r--r--   0 proycon   (1000) users      (100)     3977 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/fineuploader.css
--rw-r--r--   0 proycon   (1000) users      (100)    34193 2022-11-29 13:02:56.000000 CLAM-3.2.5/clam/static/info.xsl
--rw-r--r--   0 proycon   (1000) users      (100)    44829 2022-11-22 14:26:09.000000 CLAM-3.2.5/clam/static/interface.xsl
--rw-r--r--   0 proycon   (1000) users      (100)    88145 2019-05-01 21:14:27.000000 CLAM-3.2.5/clam/static/jquery-3.4.1.min.js
--rw-r--r--   0 proycon   (1000) users      (100)    13850 2020-07-20 08:55:42.000000 CLAM-3.2.5/clam/static/jquery.dataTables.min.css
--rw-r--r--   0 proycon   (1000) users      (100)    84321 2019-10-02 09:26:54.000000 CLAM-3.2.5/clam/static/jquery.dataTables.min.js
--rw-r--r--   0 proycon   (1000) users      (100)   368238 2020-10-27 09:46:47.000000 CLAM-3.2.5/clam/static/jquery.fine-uploader.js
--rw-r--r--   0 proycon   (1000) users      (100)   148232 2020-10-27 09:46:44.000000 CLAM-3.2.5/clam/static/jquery.fine-uploader.min.js
--rw-r--r--   0 proycon   (1000) users      (100)    83444 2020-10-27 10:32:11.000000 CLAM-3.2.5/clam/static/jquery.fineuploader-3.1.js
--rw-r--r--   0 proycon   (1000) users      (100)    37735 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/jquery.fineuploader-3.1.min.js
--rw-r--r--   0 proycon   (1000) users      (100)     1688 2020-10-27 09:48:30.000000 CLAM-3.2.5/clam/static/loading.gif
--rw-r--r--   0 proycon   (1000) users      (100)      866 2022-11-29 13:15:01.000000 CLAM-3.2.5/clam/static/login.xsl
--rw-r--r--   0 proycon   (1000) users      (100)     9342 2020-07-20 09:07:19.000000 CLAM-3.2.5/clam/static/open-iconic-bootstrap.min.css
--rw-r--r--   0 proycon   (1000) users      (100)    23144 2018-05-17 09:24:43.000000 CLAM-3.2.5/clam/static/open-iconic.eot
--rw-r--r--   0 proycon   (1000) users      (100)    21048 2018-05-17 09:23:22.000000 CLAM-3.2.5/clam/static/open-iconic.otf
--rw-r--r--   0 proycon   (1000) users      (100)    55015 2020-07-14 20:00:45.000000 CLAM-3.2.5/clam/static/open-iconic.svg
--rw-r--r--   0 proycon   (1000) users      (100)    25568 2018-05-17 09:23:22.000000 CLAM-3.2.5/clam/static/open-iconic.ttf
--rw-r--r--   0 proycon   (1000) users      (100)    12404 2018-05-17 09:24:43.000000 CLAM-3.2.5/clam/static/open-iconic.woff
--rw-r--r--   0 proycon   (1000) users      (100)    10293 2019-10-28 20:24:56.000000 CLAM-3.2.5/clam/static/parameters.xsl
--rw-r--r--   0 proycon   (1000) users      (100)    21004 2019-01-29 12:15:56.000000 CLAM-3.2.5/clam/static/popper.min.js
--rw-r--r--   0 proycon   (1000) users      (100)     3209 2020-10-27 09:48:30.000000 CLAM-3.2.5/clam/static/processing.gif
--rw-r--r--   0 proycon   (1000) users      (100)    10819 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/progress.gif
--rw-r--r--   0 proycon   (1000) users      (100)     1476 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/sonar.css
--rw-r--r--   0 proycon   (1000) users      (100)      160 2020-01-13 16:02:02.000000 CLAM-3.2.5/clam/static/sort_asc.png
--rw-r--r--   0 proycon   (1000) users      (100)      148 2019-10-02 09:26:54.000000 CLAM-3.2.5/clam/static/sort_asc_disabled.png
--rw-r--r--   0 proycon   (1000) users      (100)      201 2020-01-13 16:02:02.000000 CLAM-3.2.5/clam/static/sort_both.png
--rw-r--r--   0 proycon   (1000) users      (100)      158 2019-10-01 15:25:43.000000 CLAM-3.2.5/clam/static/sort_desc.png
--rw-r--r--   0 proycon   (1000) users      (100)      146 2019-11-20 10:49:49.000000 CLAM-3.2.5/clam/static/sort_desc_disabled.png
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.117173 CLAM-3.2.5/clam/static/tableimages/
--rw-r--r--   0 proycon   (1000) users      (100)    27490 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/Sorting icons.psd
--rw-r--r--   0 proycon   (1000) users      (100)      612 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/back_disabled.jpg
--rw-r--r--   0 proycon   (1000) users      (100)      807 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/back_enabled.jpg
--rw-r--r--   0 proycon   (1000) users      (100)      635 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/forward_disabled.jpg
--rw-r--r--   0 proycon   (1000) users      (100)      852 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/forward_enabled.jpg
--rw-r--r--   0 proycon   (1000) users      (100)      263 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/sort_asc.png
--rw-r--r--   0 proycon   (1000) users      (100)      252 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/sort_asc_disabled.png
--rw-r--r--   0 proycon   (1000) users      (100)      282 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/sort_both.png
--rw-r--r--   0 proycon   (1000) users      (100)      260 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/sort_desc.png
--rw-r--r--   0 proycon   (1000) users      (100)      251 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/static/tableimages/sort_desc_disabled.png
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.117173 CLAM-3.2.5/clam/style/
--rw-r--r--   0 proycon   (1000) users      (100)     2697 2019-10-30 14:06:55.000000 CLAM-3.2.5/clam/style/classic.css
--rw-r--r--   0 proycon   (1000) users      (100)     3837 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/style/pre2.css
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.117173 CLAM-3.2.5/clam/templates/
--rw-r--r--   0 proycon   (1000) users      (100)     2310 2019-10-26 11:32:29.000000 CLAM-3.2.5/clam/templates/admin.html
--rw-r--r--   0 proycon   (1000) users      (100)     1121 2019-10-26 11:32:20.000000 CLAM-3.2.5/clam/templates/admininspect.html
--rw-r--r--   0 proycon   (1000) users      (100)     1261 2019-10-26 09:30:17.000000 CLAM-3.2.5/clam/templates/crudetableviewer.html
--rw-r--r--   0 proycon   (1000) users      (100)      162 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/templates/inputformats.html
--rw-r--r--   0 proycon   (1000) users      (100)      290 2022-11-29 13:01:14.000000 CLAM-3.2.5/clam/templates/login.xml
--rw-r--r--   0 proycon   (1000) users      (100)     2888 2022-12-12 12:12:39.000000 CLAM-3.2.5/clam/templates/response.json
--rw-r--r--   0 proycon   (1000) users      (100)     8404 2022-11-16 12:41:53.000000 CLAM-3.2.5/clam/templates/response.xml
--rw-r--r--   0 proycon   (1000) users      (100)     1751 2021-01-07 16:02:34.000000 CLAM-3.2.5/clam/templates/share.html
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.120507 CLAM-3.2.5/clam/tests/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/tests/__init__.py
--rw-r--r--   0 proycon   (1000) users      (100)     1968 2021-06-03 16:14:42.000000 CLAM-3.2.5/clam/tests/actiontest.py
--rw-r--r--   0 proycon   (1000) users      (100)     2607 2022-04-04 21:17:04.000000 CLAM-3.2.5/clam/tests/authactiontest.py
--rw-r--r--   0 proycon   (1000) users      (100)    17315 2021-01-07 16:02:34.000000 CLAM-3.2.5/clam/tests/authtest.py
--rw-r--r--   0 proycon   (1000) users      (100)       20 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/tests/config.yml
--rw-r--r--   0 proycon   (1000) users      (100)     5890 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/tests/constrainttest.py
--rw-rw-r--   0 proycon   (1000) users      (100)      308 2015-05-29 19:21:48.000000 CLAM-3.2.5/clam/tests/crypttest.py
--rw-r--r--   0 proycon   (1000) users      (100)    13706 2022-04-07 09:01:39.000000 CLAM-3.2.5/clam/tests/datatest.py
--rw-r--r--   0 proycon   (1000) users      (100)     4557 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/tests/frogclient.py
--rw-r--r--   0 proycon   (1000) users      (100)    18492 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/tests/parametertest.py
--rw-r--r--   0 proycon   (1000) users      (100)    14920 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/tests/servicetest.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 09:02:33.120507 CLAM-3.2.5/clam/wrappers/
--rwxr-xr-x   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/wrappers/__init__.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     3682 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/wrappers/constrainttest.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     2658 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/wrappers/freqlistwrapper.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     6253 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/wrappers/template.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     2444 2022-11-16 14:15:18.000000 CLAM-3.2.5/clam/wrappers/template.sh
--rwxr-xr-x   0 proycon   (1000) users      (100)     3870 2018-11-21 13:07:01.000000 CLAM-3.2.5/clam/wrappers/testwrapper.py
--rwxr-xr-x   0 proycon   (1000) users      (100)     7230 2019-10-28 09:06:31.000000 CLAM-3.2.5/clam/wrappers/textstats.py
--rw-r--r--   0 proycon   (1000) users      (100)     6249 2023-03-01 13:33:12.000000 CLAM-3.2.5/codemeta.json
--rw-r--r--   0 proycon   (1000) users      (100)       85 2022-02-17 19:12:52.000000 CLAM-3.2.5/requirements.txt
--rw-r--r--   0 proycon   (1000) users      (100)      183 2023-03-02 09:02:33.120507 CLAM-3.2.5/setup.cfg
--rwxr-xr-x   0 proycon   (1000) users      (100)     2114 2023-03-01 13:21:59.000000 CLAM-3.2.5/setup.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.054751 CLAM-3.2.6/
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.044751 CLAM-3.2.6/CLAM.egg-info/
+-rw-r--r--   0 proycon   (1000) users      (100)     6458 2023-05-01 10:51:17.000000 CLAM-3.2.6/CLAM.egg-info/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)     3638 2023-05-01 10:51:17.000000 CLAM-3.2.6/CLAM.egg-info/SOURCES.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        1 2023-05-01 10:51:17.000000 CLAM-3.2.6/CLAM.egg-info/dependency_links.txt
+-rw-r--r--   0 proycon   (1000) users      (100)      214 2023-05-01 10:51:17.000000 CLAM-3.2.6/CLAM.egg-info/entry_points.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       85 2023-05-01 10:51:17.000000 CLAM-3.2.6/CLAM.egg-info/requires.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        5 2023-05-01 10:51:17.000000 CLAM-3.2.6/CLAM.egg-info/top_level.txt
+-rw-r--r--   0 proycon   (1000) users      (100)    35147 2018-11-21 13:07:01.000000 CLAM-3.2.6/COPYING
+-rw-r--r--   0 proycon   (1000) users      (100)      390 2018-11-21 13:07:01.000000 CLAM-3.2.6/MANIFEST.in
+-rw-r--r--   0 proycon   (1000) users      (100)     6458 2023-05-01 10:51:17.054751 CLAM-3.2.6/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)     5500 2022-11-17 14:55:17.000000 CLAM-3.2.6/README.rst
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.044751 CLAM-3.2.6/clam/
+-rwxr-xr-x   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/__init__.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)    11702 2023-05-01 10:06:17.000000 CLAM-3.2.6/clam/clamclient.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)    11350 2023-05-01 10:05:29.000000 CLAM-3.2.6/clam/clamdispatcher.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)    16379 2022-11-16 20:18:23.000000 CLAM-3.2.6/clam/clamnewproject.py
+-rw-r--r--   0 proycon   (1000) users      (100)      473 2016-04-29 13:30:48.000000 CLAM-3.2.6/clam/clamrunjob.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)   175893 2022-11-29 12:59:14.000000 CLAM-3.2.6/clam/clamservice.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.044751 CLAM-3.2.6/clam/clients/
+-rw-r--r--   0 proycon   (1000) users      (100)     2434 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/clients/clienttest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     4578 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/clients/textstats.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.044751 CLAM-3.2.6/clam/common/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/common/__init__.py
+-rw-r--r--   0 proycon   (1000) users      (100)    26603 2022-11-22 17:37:08.000000 CLAM-3.2.6/clam/common/auth.py
+-rw-r--r--   0 proycon   (1000) users      (100)    25383 2022-11-22 12:43:49.000000 CLAM-3.2.6/clam/common/client.py
+-rw-r--r--   0 proycon   (1000) users      (100)     4572 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/common/converters.py
+-rw-r--r--   0 proycon   (1000) users      (100)   136423 2023-05-01 10:05:15.000000 CLAM-3.2.6/clam/common/data.py
+-rw-r--r--   0 proycon   (1000) users      (100)      339 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/common/digestauth.py
+-rw-r--r--   0 proycon   (1000) users      (100)    12172 2022-11-17 13:48:36.000000 CLAM-3.2.6/clam/common/formats.py
+-rw-r--r--   0 proycon   (1000) users      (100)      978 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/common/languages.py
+-rw-r--r--   0 proycon   (1000) users      (100)     2403 2022-11-15 14:00:38.000000 CLAM-3.2.6/clam/common/oauth.py
+-rw-r--r--   0 proycon   (1000) users      (100)    26953 2019-12-14 12:33:12.000000 CLAM-3.2.6/clam/common/parameters.py
+-rw-r--r--   0 proycon   (1000) users      (100)      549 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/common/status.py
+-rw-r--r--   0 proycon   (1000) users      (100)     5872 2022-11-17 14:27:35.000000 CLAM-3.2.6/clam/common/util.py
+-rw-r--r--   0 proycon   (1000) users      (100)     9864 2021-01-12 12:04:36.000000 CLAM-3.2.6/clam/common/viewers.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.048085 CLAM-3.2.6/clam/config/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/__init__.py
+-rw-r--r--   0 proycon   (1000) users      (100)     6507 2019-10-30 11:21:07.000000 CLAM-3.2.6/clam/config/actiontest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     6654 2020-02-27 10:24:17.000000 CLAM-3.2.6/clam/config/authactiontest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     6964 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/authtest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     5994 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/config/constrainttest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     6805 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/defaults.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     1457 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/example.wsgi
+-rw-r--r--   0 proycon   (1000) users      (100)     6931 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/forwardauthtest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     6020 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/freqlist.py
+-rw-r--r--   0 proycon   (1000) users      (100)     5921 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/config/multiplier.py
+-rw-r--r--   0 proycon   (1000) users      (100)     7913 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/config/oauthtest.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     1719 2022-11-16 15:35:51.000000 CLAM-3.2.6/clam/config/setup_template.py
+-rw-r--r--   0 proycon   (1000) users      (100)     3135 2022-11-16 19:57:09.000000 CLAM-3.2.6/clam/config/template.Dockerfile
+-rw-r--r--   0 proycon   (1000) users      (100)     3168 2022-11-22 12:11:07.000000 CLAM-3.2.6/clam/config/template.config.yml
+-rw-r--r--   0 proycon   (1000) users      (100)    12906 2022-11-16 13:44:37.000000 CLAM-3.2.6/clam/config/template.py
+-rw-r--r--   0 proycon   (1000) users      (100)     5672 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/test.py
+-rw-r--r--   0 proycon   (1000) users      (100)     5693 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/config/test2.py
+-rw-r--r--   0 proycon   (1000) users      (100)     9601 2021-04-28 10:09:47.000000 CLAM-3.2.6/clam/config/textstats.py
+-rw-r--r--   0 proycon   (1000) users      (100)     7934 2016-03-23 20:44:08.000000 CLAM-3.2.6/clam/config/textstats1.py
+-rw-rw-r--   0 proycon   (1000) users      (100)     7341 2015-12-18 13:06:50.000000 CLAM-3.2.6/clam/config/textstats2.py
+-rw-r--r--   0 proycon   (1000) users      (100)     7815 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/config/textstats3.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.051418 CLAM-3.2.6/clam/static/
+-rw-r--r--   0 proycon   (1000) users      (100)    25376 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/ajaxupload.js
+-rw-r--r--   0 proycon   (1000) users      (100)      440 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/back.png
+-rw-r--r--   0 proycon   (1000) users      (100)     5010 2021-01-07 16:02:34.000000 CLAM-3.2.6/clam/static/base.css
+-rw-r--r--   0 proycon   (1000) users      (100)   155758 2019-02-13 16:40:50.000000 CLAM-3.2.6/clam/static/bootstrap.min.css
+-rw-r--r--   0 proycon   (1000) users      (100)    58072 2019-02-13 16:40:57.000000 CLAM-3.2.6/clam/static/bootstrap.min.js
+-rw-r--r--   0 proycon   (1000) users      (100)    32913 2022-11-15 16:39:27.000000 CLAM-3.2.6/clam/static/clam.js
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.051418 CLAM-3.2.6/clam/static/custom/
+-rw-r--r--   0 proycon   (1000) users      (100)      684 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/custom/sonardropbox_index.html
+-rw-r--r--   0 proycon   (1000) users      (100)      115 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/custom/sonardropbox_projectdone.html
+-rw-r--r--   0 proycon   (1000) users      (100)     2899 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/custom/sonardropbox_projectstart.html
+-rw-r--r--   0 proycon   (1000) users      (100)      820 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/delete.png
+-rw-r--r--   0 proycon   (1000) users      (100)     4001 2020-10-27 09:49:52.000000 CLAM-3.2.6/clam/static/fine-uploader.min.css
+-rw-r--r--   0 proycon   (1000) users      (100)     3977 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/fineuploader.css
+-rw-r--r--   0 proycon   (1000) users      (100)    34140 2023-05-01 10:46:23.000000 CLAM-3.2.6/clam/static/info.xsl
+-rw-r--r--   0 proycon   (1000) users      (100)    44829 2023-05-01 10:22:41.000000 CLAM-3.2.6/clam/static/interface.xsl
+-rw-r--r--   0 proycon   (1000) users      (100)    89493 2023-05-01 10:21:52.000000 CLAM-3.2.6/clam/static/jquery-3.5.0.min.js
+-rw-r--r--   0 proycon   (1000) users      (100)    13850 2020-07-20 08:55:42.000000 CLAM-3.2.6/clam/static/jquery.dataTables.min.css
+-rw-r--r--   0 proycon   (1000) users      (100)    84321 2019-10-02 09:26:54.000000 CLAM-3.2.6/clam/static/jquery.dataTables.min.js
+-rw-r--r--   0 proycon   (1000) users      (100)   368238 2020-10-27 09:46:47.000000 CLAM-3.2.6/clam/static/jquery.fine-uploader.js
+-rw-r--r--   0 proycon   (1000) users      (100)   148232 2020-10-27 09:46:44.000000 CLAM-3.2.6/clam/static/jquery.fine-uploader.min.js
+-rw-r--r--   0 proycon   (1000) users      (100)    83444 2020-10-27 10:32:11.000000 CLAM-3.2.6/clam/static/jquery.fineuploader-3.1.js
+-rw-r--r--   0 proycon   (1000) users      (100)    37735 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/jquery.fineuploader-3.1.min.js
+-rw-r--r--   0 proycon   (1000) users      (100)     1688 2020-10-27 09:48:30.000000 CLAM-3.2.6/clam/static/loading.gif
+-rw-r--r--   0 proycon   (1000) users      (100)      866 2022-11-29 13:15:01.000000 CLAM-3.2.6/clam/static/login.xsl
+-rw-r--r--   0 proycon   (1000) users      (100)     9342 2020-07-20 09:07:19.000000 CLAM-3.2.6/clam/static/open-iconic-bootstrap.min.css
+-rw-r--r--   0 proycon   (1000) users      (100)    23144 2018-05-17 09:24:43.000000 CLAM-3.2.6/clam/static/open-iconic.eot
+-rw-r--r--   0 proycon   (1000) users      (100)    21048 2018-05-17 09:23:22.000000 CLAM-3.2.6/clam/static/open-iconic.otf
+-rw-r--r--   0 proycon   (1000) users      (100)    55015 2020-07-14 20:00:45.000000 CLAM-3.2.6/clam/static/open-iconic.svg
+-rw-r--r--   0 proycon   (1000) users      (100)    25568 2018-05-17 09:23:22.000000 CLAM-3.2.6/clam/static/open-iconic.ttf
+-rw-r--r--   0 proycon   (1000) users      (100)    12404 2018-05-17 09:24:43.000000 CLAM-3.2.6/clam/static/open-iconic.woff
+-rw-r--r--   0 proycon   (1000) users      (100)    10293 2019-10-28 20:24:56.000000 CLAM-3.2.6/clam/static/parameters.xsl
+-rw-r--r--   0 proycon   (1000) users      (100)    21004 2019-01-29 12:15:56.000000 CLAM-3.2.6/clam/static/popper.min.js
+-rw-r--r--   0 proycon   (1000) users      (100)     3209 2020-10-27 09:48:30.000000 CLAM-3.2.6/clam/static/processing.gif
+-rw-r--r--   0 proycon   (1000) users      (100)    10819 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/progress.gif
+-rw-r--r--   0 proycon   (1000) users      (100)     1476 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/sonar.css
+-rw-r--r--   0 proycon   (1000) users      (100)      160 2020-01-13 16:02:02.000000 CLAM-3.2.6/clam/static/sort_asc.png
+-rw-r--r--   0 proycon   (1000) users      (100)      148 2019-10-02 09:26:54.000000 CLAM-3.2.6/clam/static/sort_asc_disabled.png
+-rw-r--r--   0 proycon   (1000) users      (100)      201 2020-01-13 16:02:02.000000 CLAM-3.2.6/clam/static/sort_both.png
+-rw-r--r--   0 proycon   (1000) users      (100)      158 2019-10-01 15:25:43.000000 CLAM-3.2.6/clam/static/sort_desc.png
+-rw-r--r--   0 proycon   (1000) users      (100)      146 2019-11-20 10:49:49.000000 CLAM-3.2.6/clam/static/sort_desc_disabled.png
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.051418 CLAM-3.2.6/clam/static/tableimages/
+-rw-r--r--   0 proycon   (1000) users      (100)    27490 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/Sorting icons.psd
+-rw-r--r--   0 proycon   (1000) users      (100)      612 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/back_disabled.jpg
+-rw-r--r--   0 proycon   (1000) users      (100)      807 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/back_enabled.jpg
+-rw-r--r--   0 proycon   (1000) users      (100)      635 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/forward_disabled.jpg
+-rw-r--r--   0 proycon   (1000) users      (100)      852 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/forward_enabled.jpg
+-rw-r--r--   0 proycon   (1000) users      (100)      263 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/sort_asc.png
+-rw-r--r--   0 proycon   (1000) users      (100)      252 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/sort_asc_disabled.png
+-rw-r--r--   0 proycon   (1000) users      (100)      282 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/sort_both.png
+-rw-r--r--   0 proycon   (1000) users      (100)      260 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/sort_desc.png
+-rw-r--r--   0 proycon   (1000) users      (100)      251 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/static/tableimages/sort_desc_disabled.png
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.051418 CLAM-3.2.6/clam/style/
+-rw-r--r--   0 proycon   (1000) users      (100)     2697 2019-10-30 14:06:55.000000 CLAM-3.2.6/clam/style/classic.css
+-rw-r--r--   0 proycon   (1000) users      (100)     3837 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/style/pre2.css
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.054751 CLAM-3.2.6/clam/templates/
+-rw-r--r--   0 proycon   (1000) users      (100)     2310 2019-10-26 11:32:29.000000 CLAM-3.2.6/clam/templates/admin.html
+-rw-r--r--   0 proycon   (1000) users      (100)     1121 2019-10-26 11:32:20.000000 CLAM-3.2.6/clam/templates/admininspect.html
+-rw-r--r--   0 proycon   (1000) users      (100)     1261 2019-10-26 09:30:17.000000 CLAM-3.2.6/clam/templates/crudetableviewer.html
+-rw-r--r--   0 proycon   (1000) users      (100)      162 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/templates/inputformats.html
+-rw-r--r--   0 proycon   (1000) users      (100)      290 2022-11-29 13:01:14.000000 CLAM-3.2.6/clam/templates/login.xml
+-rw-r--r--   0 proycon   (1000) users      (100)     2888 2022-12-12 12:12:39.000000 CLAM-3.2.6/clam/templates/response.json
+-rw-r--r--   0 proycon   (1000) users      (100)     8404 2022-11-16 12:41:53.000000 CLAM-3.2.6/clam/templates/response.xml
+-rw-r--r--   0 proycon   (1000) users      (100)     1751 2021-01-07 16:02:34.000000 CLAM-3.2.6/clam/templates/share.html
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.054751 CLAM-3.2.6/clam/tests/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/tests/__init__.py
+-rw-r--r--   0 proycon   (1000) users      (100)     1968 2021-06-03 16:14:42.000000 CLAM-3.2.6/clam/tests/actiontest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     2607 2022-04-04 21:17:04.000000 CLAM-3.2.6/clam/tests/authactiontest.py
+-rw-r--r--   0 proycon   (1000) users      (100)    17315 2021-01-07 16:02:34.000000 CLAM-3.2.6/clam/tests/authtest.py
+-rw-r--r--   0 proycon   (1000) users      (100)       20 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/tests/config.yml
+-rw-r--r--   0 proycon   (1000) users      (100)     5890 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/tests/constrainttest.py
+-rw-rw-r--   0 proycon   (1000) users      (100)      308 2015-05-29 19:21:48.000000 CLAM-3.2.6/clam/tests/crypttest.py
+-rw-r--r--   0 proycon   (1000) users      (100)    13706 2022-04-07 09:01:39.000000 CLAM-3.2.6/clam/tests/datatest.py
+-rw-r--r--   0 proycon   (1000) users      (100)     4557 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/tests/frogclient.py
+-rw-r--r--   0 proycon   (1000) users      (100)    18492 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/tests/parametertest.py
+-rw-r--r--   0 proycon   (1000) users      (100)    14920 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/tests/servicetest.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-01 10:51:17.054751 CLAM-3.2.6/clam/wrappers/
+-rwxr-xr-x   0 proycon   (1000) users      (100)        0 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/wrappers/__init__.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     3682 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/wrappers/constrainttest.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     2658 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/wrappers/freqlistwrapper.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     6253 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/wrappers/template.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     2444 2022-11-16 14:15:18.000000 CLAM-3.2.6/clam/wrappers/template.sh
+-rwxr-xr-x   0 proycon   (1000) users      (100)     3870 2018-11-21 13:07:01.000000 CLAM-3.2.6/clam/wrappers/testwrapper.py
+-rwxr-xr-x   0 proycon   (1000) users      (100)     7230 2019-10-28 09:06:31.000000 CLAM-3.2.6/clam/wrappers/textstats.py
+-rw-r--r--   0 proycon   (1000) users      (100)     6249 2023-05-01 10:05:01.000000 CLAM-3.2.6/codemeta.json
+-rw-r--r--   0 proycon   (1000) users      (100)       85 2022-02-17 19:12:52.000000 CLAM-3.2.6/requirements.txt
+-rw-r--r--   0 proycon   (1000) users      (100)      183 2023-05-01 10:51:17.054751 CLAM-3.2.6/setup.cfg
+-rwxr-xr-x   0 proycon   (1000) users      (100)     2114 2023-05-01 10:07:03.000000 CLAM-3.2.6/setup.py
```

### Comparing `CLAM-3.2.5/CLAM.egg-info/PKG-INFO` & `CLAM-3.2.6/CLAM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: CLAM
-Version: 3.2.5
+Version: 3.2.6
 Summary: Turns command-line tools into fully-fledged RESTful webservices with an auto-generated web-interface for human end-users.
 Home-page: https://proycon.github.io/clam
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPL-3.0-only
 Keywords: SaaS,webservice,rest
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -160,7 +161,9 @@
 
 **Note:** It is important to regularly keep CLAM up to date as fixes and
 improvements are implemented on a regular basis. Update CLAM using::
 
   $ pip install -U clam
 
 
+
+
```

### Comparing `CLAM-3.2.5/CLAM.egg-info/SOURCES.txt` & `CLAM-3.2.6/CLAM.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 clam/static/bootstrap.min.js
 clam/static/clam.js
 clam/static/delete.png
 clam/static/fine-uploader.min.css
 clam/static/fineuploader.css
 clam/static/info.xsl
 clam/static/interface.xsl
-clam/static/jquery-3.4.1.min.js
+clam/static/jquery-3.5.0.min.js
 clam/static/jquery.dataTables.min.css
 clam/static/jquery.dataTables.min.js
 clam/static/jquery.fine-uploader.js
 clam/static/jquery.fine-uploader.min.js
 clam/static/jquery.fineuploader-3.1.js
 clam/static/jquery.fineuploader-3.1.min.js
 clam/static/loading.gif
```

### Comparing `CLAM-3.2.5/COPYING` & `CLAM-3.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/PKG-INFO` & `CLAM-3.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: CLAM
-Version: 3.2.5
+Version: 3.2.6
 Summary: Turns command-line tools into fully-fledged RESTful webservices with an auto-generated web-interface for human end-users.
 Home-page: https://proycon.github.io/clam
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPL-3.0-only
 Keywords: SaaS,webservice,rest
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -160,7 +161,9 @@
 
 **Note:** It is important to regularly keep CLAM up to date as fixes and
 improvements are implemented on a regular basis. Update CLAM using::
 
   $ pip install -U clam
 
 
+
+
```

### Comparing `CLAM-3.2.5/README.rst` & `CLAM-3.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/clamclient.py` & `CLAM-3.2.6/clam/clamclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,23 @@
 import sys
 import os
 sys.path.append(sys.path[0] + '/..')
 os.environ['PYTHONPATH'] = sys.path[0] + '/..'
 
 
 from clam.common.client import CLAMClient
-from clam.common.data import ParameterCondition, NotFound, PermissionDenied, ServerError, AuthRequired
-
-VERSION = '3.0.0'
+from clam.common.data import ParameterCondition, NotFound, PermissionDenied, ServerError, AuthRequired, VERSION
 
 def usage():
     print("clamclient.py [[options]] [url] [command] [command-arguments]",file=sys.stderr)
     print("  Low-level command-line interface to any CLAM webservice",file=sys.stderr)
     print("Options:",file=sys.stderr)
     print("\t-u [username]",file=sys.stderr)
     print("\t-p [password]",file=sys.stderr)
-    print("\t-b              - Use HTTP Basic Authentication instead of Digest",file=sys.stderr)
+    print("\t-D              - Use HTTP Digest Authentication instead of Basic",file=sys.stderr)
     print("\t-h              - Help",file=sys.stderr)
     print("\t-v              - Version information",file=sys.stderr)
     print("Commands:",file=sys.stderr)
     print(" info             - Get service specification and project list, this is the default if no command is specified.",file=sys.stderr)
     print(" projects         - Show a list of available projects",file=sys.stderr)
     print(" profiles         - Render an overview of all profiles",file=sys.stderr)
     print(" inputtemplates   - Show a list of all available input templates and their metadata",file=sys.stderr)
@@ -63,30 +61,30 @@
     #prin(" metadata [project] [filename]",file=sys.stderr)
     #prin("\t View the metadata of the specified file",file=sys.stderr)
 
 
 
 def main():
     username = password = None
-    basicauth = False
+    basicauth = True
     parameters = {}
     begin = 0
     rawargs = sys.argv[1:]
     for i,o in enumerate(rawargs):
         if o == '-u':
             username = rawargs[i+1]
             begin = i+2
         elif o == '-p':
             password = rawargs[i+1]
             begin = i+2
         elif o == '-h':
             usage()
             sys.exit(0)
-        elif o == '-h':
-            basicauth = True
+        elif o == '-D':
+            basicauth = False
         elif o == '-v':
             print("CLAM Client version " + str(VERSION),file=sys.stderr)
             sys.exit(0)
         elif o[0] == '-' and len(o) > 1 and o[1] != '-':
             usage()
             print("ERROR: Unknown option: ", o,file=sys.stderr)
             sys.exit(2)
```

### Comparing `CLAM-3.2.5/clam/clamdispatcher.py` & `CLAM-3.2.6/clam/clamdispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import datetime
 import subprocess
 import time
 import signal
 import shutil
 import json
 
-VERSION = '3.2.5'
+VERSION = '3.2.6'
 
 sys.path.append(sys.path[0] + '/..')
 
 import clam.common.data #pylint: disable=wrong-import-position
 import clam.common.status
 from clam.common.util import computediskusage
```

### Comparing `CLAM-3.2.5/clam/clamnewproject.py` & `CLAM-3.2.6/clam/clamnewproject.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/clamservice.py` & `CLAM-3.2.6/clam/clamservice.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/clients/clienttest.py` & `CLAM-3.2.6/clam/clients/clienttest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/clients/textstats.py` & `CLAM-3.2.6/clam/clients/textstats.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/auth.py` & `CLAM-3.2.6/clam/common/auth.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/client.py` & `CLAM-3.2.6/clam/common/client.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/converters.py` & `CLAM-3.2.6/clam/common/converters.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/data.py` & `CLAM-3.2.6/clam/common/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from io import StringIO, BytesIO #pylint: disable=ungrouped-imports
 from urllib.parse import quote
 import clam.common.parameters
 import clam.common.status
 import clam.common.util
 import clam.common.viewers
 
-VERSION = '3.2.5'
+VERSION = '3.2.6'
 
 #dirs for services shipped with CLAM itself
 CONFIGDIR = os.path.abspath(os.path.dirname(__file__) + '/../config/')
 WRAPPERDIR = os.path.abspath(os.path.dirname(__file__) + '/../wrappers/')
 
 #clam.common.formats is deliberately imported _at the end_
```

### Comparing `CLAM-3.2.5/clam/common/formats.py` & `CLAM-3.2.6/clam/common/formats.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/languages.py` & `CLAM-3.2.6/clam/common/languages.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/oauth.py` & `CLAM-3.2.6/clam/common/oauth.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/parameters.py` & `CLAM-3.2.6/clam/common/parameters.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/status.py` & `CLAM-3.2.6/clam/common/status.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/util.py` & `CLAM-3.2.6/clam/common/util.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/common/viewers.py` & `CLAM-3.2.6/clam/common/viewers.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/actiontest.py` & `CLAM-3.2.6/clam/config/actiontest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/authactiontest.py` & `CLAM-3.2.6/clam/config/authactiontest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/authtest.py` & `CLAM-3.2.6/clam/config/authtest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/constrainttest.py` & `CLAM-3.2.6/clam/config/constrainttest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/defaults.py` & `CLAM-3.2.6/clam/config/defaults.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/example.wsgi` & `CLAM-3.2.6/clam/config/example.wsgi`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/forwardauthtest.py` & `CLAM-3.2.6/clam/config/forwardauthtest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/freqlist.py` & `CLAM-3.2.6/clam/config/freqlist.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/multiplier.py` & `CLAM-3.2.6/clam/config/multiplier.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/oauthtest.py` & `CLAM-3.2.6/clam/config/oauthtest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/setup_template.py` & `CLAM-3.2.6/clam/config/setup_template.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/template.Dockerfile` & `CLAM-3.2.6/clam/config/template.Dockerfile`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/template.config.yml` & `CLAM-3.2.6/clam/config/template.config.yml`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/template.py` & `CLAM-3.2.6/clam/config/template.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/test.py` & `CLAM-3.2.6/clam/config/test.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/test2.py` & `CLAM-3.2.6/clam/config/test2.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/textstats.py` & `CLAM-3.2.6/clam/config/textstats.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/textstats1.py` & `CLAM-3.2.6/clam/config/textstats1.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/textstats2.py` & `CLAM-3.2.6/clam/config/textstats2.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/config/textstats3.py` & `CLAM-3.2.6/clam/config/textstats3.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/ajaxupload.js` & `CLAM-3.2.6/clam/static/ajaxupload.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/base.css` & `CLAM-3.2.6/clam/static/base.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/bootstrap.min.css` & `CLAM-3.2.6/clam/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/bootstrap.min.js` & `CLAM-3.2.6/clam/static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/clam.js` & `CLAM-3.2.6/clam/static/clam.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/custom/sonardropbox_index.html` & `CLAM-3.2.6/clam/static/custom/sonardropbox_index.html`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/custom/sonardropbox_projectstart.html` & `CLAM-3.2.6/clam/static/custom/sonardropbox_projectstart.html`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/delete.png` & `CLAM-3.2.6/clam/static/delete.png`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/fine-uploader.min.css` & `CLAM-3.2.6/clam/static/fine-uploader.min.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/fineuploader.css` & `CLAM-3.2.6/clam/static/fineuploader.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/info.xsl` & `CLAM-3.2.6/clam/static/info.xsl`

 * *Files 1% similar despite different names*

#### Comparing `CLAM-3.2.5/clam/static/info.xsl` & `CLAM-3.2.6/clam/static/info.xsl`

```diff
@@ -928,30 +928,26 @@
           </div>
           <xsl:call-template name="footer"/>
         </div>
       </body>
     </html>
   </xsl:template>
   <xsl:template name="curlauth">
-    <xsl:choose>
-      <xsl:when test="contains(/clam/@authentication,'oauth')">
-        --oauth2-bearer
-        <em>$oauth_access_token</em>
-      </xsl:when>
-      <xsl:when test="contains(/clam/@authentication,'basic')">
-        --basic -u
-        <em>$username</em>
-        -p
-      </xsl:when>
-      <xsl:when test="contains(/clam/@authentication,'digest')">
-        --digest -u
-        <em>$username</em>
-        -p
-      </xsl:when>
-    </xsl:choose>
+    <xsl:if test="contains(/clam/@authentication,'oauth')">
+      --oauth2-bearer
+      <em>$oauth_access_token</em>
+    </xsl:if>
+    <xsl:if test="contains(/clam/@authentication,'basic')">
+      --basic --user
+      <em>$username:$password</em>
+    </xsl:if>
+    <xsl:if test="contains(/clam/@authentication,'digest')">
+      --digest --user
+      <em>$username:$password</em>
+    </xsl:if>
   </xsl:template>
   <xsl:template name="authtype">
     <xsl:choose>
       <xsl:when test="/clam/@authentication = 'oauth,basic'">OAuth2 or HTTP Basic Authentication</xsl:when>
       <xsl:when test="/clam/@authentication = 'basic,oauth'">HTTP Basic Authentication or OAuth2</xsl:when>
       <xsl:when test="/clam/@authentication = 'basic'">HTTP Basic Authentication or HTTP Digest Authentication</xsl:when>
       <xsl:when test="/clam/@authentication = 'digest'">HTTP Digest Authentication</xsl:when>
@@ -969,15 +965,15 @@
         ::
         <xsl:value-of select="@project"/>
       </title>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/bootstrap.min.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/open-iconic-bootstrap.min.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/base.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/style.css" type="text/css"/>
-      <script src="{/clam/@baseurl}/static/jquery-3.4.1.min.js"/>
+      <script src="{/clam/@baseurl}/static/jquery-3.5.0.min.js"/>
       <script src="{/clam/@baseurl}/static/popper.min.js"/>
       <script src="{/clam/@baseurl}/static/bootstrap.min.js"/>
     </head>
   </xsl:template>
   <xsl:template name="footer">
     <div id="footer" class="card">
       Powered by
```

### Comparing `CLAM-3.2.5/clam/static/interface.xsl` & `CLAM-3.2.6/clam/static/interface.xsl`

 * *Files 0% similar despite different names*

#### Comparing `CLAM-3.2.5/clam/static/interface.xsl` & `CLAM-3.2.6/clam/static/interface.xsl`

```diff
@@ -102,15 +102,15 @@
       </title>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/bootstrap.min.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/jquery.dataTables.min.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/open-iconic-bootstrap.min.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/base.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/static/fineuploader.css" type="text/css"/>
       <link rel="stylesheet" href="{/clam/@baseurl}/style.css" type="text/css"/>
-      <script src="{/clam/@baseurl}/static/jquery-3.4.1.min.js"/>
+      <script src="{/clam/@baseurl}/static/jquery-3.5.0.min.js"/>
       <script src="{/clam/@baseurl}/static/popper.min.js"/>
       <script src="{/clam/@baseurl}/static/jquery.dataTables.min.js"/>
       <script src="{/clam/@baseurl}/static/bootstrap.min.js"/>
       <script type="text/javascript" src="{/clam/@baseurl}/data.js"/>
       <xsl:choose>
         <xsl:when test="contains(/clam/@interfaceoptions,'simplepolling')">
           <script type="text/javascript" src="{/clam/@baseurl}/static/ajaxupload.js"/>
```

### Comparing `CLAM-3.2.5/clam/static/jquery-3.4.1.min.js` & `CLAM-3.2.6/clam/static/jquery-3.5.0.min.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,38 @@
-/*! jQuery v3.4.1 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
+/*! jQuery v3.5.0 | (c) JS Foundation and other contributors | jquery.org/license */ ! function(e, t) {
     "use strict";
     "object" == typeof module && "object" == typeof module.exports ? module.exports = e.document ? t(e, !0) : function(e) {
         if (!e.document) throw new Error("jQuery requires a window with a document");
         return t(e)
     } : t(e)
 }("undefined" != typeof window ? window : this, function(C, e) {
     "use strict";
     var t = [],
-        E = C.document,
         r = Object.getPrototypeOf,
         s = t.slice,
-        g = t.concat,
+        g = t.flat ? function(e) {
+            return t.flat.call(e)
+        } : function(e) {
+            return t.concat.apply([], e)
+        },
         u = t.push,
         i = t.indexOf,
         n = {},
         o = n.toString,
         v = n.hasOwnProperty,
         a = v.toString,
         l = a.call(Object),
         y = {},
         m = function(e) {
             return "function" == typeof e && "number" != typeof e.nodeType
         },
         x = function(e) {
             return null != e && e === e.window
         },
+        E = C.document,
         c = {
             type: !0,
             src: !0,
             nonce: !0,
             noModule: !0
         };
 
@@ -38,77 +42,86 @@
             for (r in c)(i = t[r] || t.getAttribute && t.getAttribute(r)) && o.setAttribute(r, i);
         n.head.appendChild(o).parentNode.removeChild(o)
     }
 
     function w(e) {
         return null == e ? e + "" : "object" == typeof e || "function" == typeof e ? n[o.call(e)] || "object" : typeof e
     }
-    var f = "3.4.1",
-        k = function(e, t) {
-            return new k.fn.init(e, t)
-        },
-        p = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    var f = "3.5.0",
+        S = function(e, t) {
+            return new S.fn.init(e, t)
+        };
 
-    function d(e) {
+    function p(e) {
         var t = !!e && "length" in e && e.length,
             n = w(e);
         return !m(e) && !x(e) && ("array" === n || 0 === t || "number" == typeof t && 0 < t && t - 1 in e)
     }
-    k.fn = k.prototype = {
+    S.fn = S.prototype = {
         jquery: f,
-        constructor: k,
+        constructor: S,
         length: 0,
         toArray: function() {
             return s.call(this)
         },
         get: function(e) {
             return null == e ? s.call(this) : e < 0 ? this[e + this.length] : this[e]
         },
         pushStack: function(e) {
-            var t = k.merge(this.constructor(), e);
+            var t = S.merge(this.constructor(), e);
             return t.prevObject = this, t
         },
         each: function(e) {
-            return k.each(this, e)
+            return S.each(this, e)
         },
         map: function(n) {
-            return this.pushStack(k.map(this, function(e, t) {
+            return this.pushStack(S.map(this, function(e, t) {
                 return n.call(e, t, e)
             }))
         },
         slice: function() {
             return this.pushStack(s.apply(this, arguments))
         },
         first: function() {
             return this.eq(0)
         },
         last: function() {
             return this.eq(-1)
         },
+        even: function() {
+            return this.pushStack(S.grep(this, function(e, t) {
+                return (t + 1) % 2
+            }))
+        },
+        odd: function() {
+            return this.pushStack(S.grep(this, function(e, t) {
+                return t % 2
+            }))
+        },
         eq: function(e) {
             var t = this.length,
                 n = +e + (e < 0 ? t : 0);
             return this.pushStack(0 <= n && n < t ? [this[n]] : [])
         },
         end: function() {
             return this.prevObject || this.constructor()
         },
         push: u,
         sort: t.sort,
         splice: t.splice
-    }, k.extend = k.fn.extend = function() {
+    }, S.extend = S.fn.extend = function() {
         var e, t, n, r, i, o, a = arguments[0] || {},
             s = 1,
             u = arguments.length,
             l = !1;
         for ("boolean" == typeof a && (l = a, a = arguments[s] || {}, s++), "object" == typeof a || m(a) || (a = {}), s === u && (a = this, s--); s < u; s++)
             if (null != (e = arguments[s]))
-                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (k.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || k.isPlainObject(n) ? n : {}, i = !1, a[t] = k.extend(l, o, r)) : void 0 !== r && (a[t] = r));
+                for (t in e) r = e[t], "__proto__" !== t && a !== r && (l && r && (S.isPlainObject(r) || (i = Array.isArray(r))) ? (n = a[t], o = i && !Array.isArray(n) ? [] : i || S.isPlainObject(n) ? n : {}, i = !1, a[t] = S.extend(l, o, r)) : void 0 !== r && (a[t] = r));
         return a
-    }, k.extend({
+    }, S.extend({
         expando: "jQuery" + (f + Math.random()).replace(/\D/g, ""),
         isReady: !0,
         error: function(e) {
             throw new Error(e)
         },
         noop: function() {},
         isPlainObject: function(e) {
@@ -116,35 +129,32 @@
             return !(!e || "[object Object]" !== o.call(e)) && (!(t = r(e)) || "function" == typeof(n = v.call(t, "constructor") && t.constructor) && a.call(n) === l)
         },
         isEmptyObject: function(e) {
             var t;
             for (t in e) return !1;
             return !0
         },
-        globalEval: function(e, t) {
+        globalEval: function(e, t, n) {
             b(e, {
                 nonce: t && t.nonce
-            })
+            }, n)
         },
         each: function(e, t) {
             var n, r = 0;
-            if (d(e)) {
+            if (p(e)) {
                 for (n = e.length; r < n; r++)
                     if (!1 === t.call(e[r], r, e[r])) break
             } else
                 for (r in e)
                     if (!1 === t.call(e[r], r, e[r])) break;
             return e
         },
-        trim: function(e) {
-            return null == e ? "" : (e + "").replace(p, "")
-        },
         makeArray: function(e, t) {
             var n = t || [];
-            return null != e && (d(Object(e)) ? k.merge(n, "string" == typeof e ? [e] : e) : u.call(n, e)), n
+            return null != e && (p(Object(e)) ? S.merge(n, "string" == typeof e ? [e] : e) : u.call(n, e)), n
         },
         inArray: function(e, t, n) {
             return null == t ? -1 : i.call(t, e, n)
         },
         merge: function(e, t) {
             for (var n = +t.length, r = 0, i = e.length; r < n; r++) e[i++] = t[r];
             return e.length = i, e
@@ -152,34 +162,34 @@
         grep: function(e, t, n) {
             for (var r = [], i = 0, o = e.length, a = !n; i < o; i++) !t(e[i], i) !== a && r.push(e[i]);
             return r
         },
         map: function(e, t, n) {
             var r, i, o = 0,
                 a = [];
-            if (d(e))
+            if (p(e))
                 for (r = e.length; o < r; o++) null != (i = t(e[o], o, n)) && a.push(i);
             else
                 for (o in e) null != (i = t(e[o], o, n)) && a.push(i);
-            return g.apply([], a)
+            return g(a)
         },
         guid: 1,
         support: y
-    }), "function" == typeof Symbol && (k.fn[Symbol.iterator] = t[Symbol.iterator]), k.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
+    }), "function" == typeof Symbol && (S.fn[Symbol.iterator] = t[Symbol.iterator]), S.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(e, t) {
         n["[object " + t + "]"] = t.toLowerCase()
     });
-    var h = function(n) {
-        var e, d, b, o, i, h, f, g, w, u, l, T, C, a, E, v, s, c, y, k = "sizzle" + 1 * new Date,
-            m = n.document,
-            S = 0,
+    var d = function(n) {
+        var e, d, b, o, i, h, f, g, w, u, l, T, C, a, E, v, s, c, y, S = "sizzle" + 1 * new Date,
+            p = n.document,
+            k = 0,
             r = 0,
-            p = ue(),
+            m = ue(),
             x = ue(),
-            N = ue(),
             A = ue(),
+            N = ue(),
             D = function(e, t) {
                 return e === t && (l = !0), 0
             },
             j = {}.hasOwnProperty,
             t = [],
             q = t.pop,
             L = t.push,
@@ -188,44 +198,44 @@
             P = function(e, t) {
                 for (var n = 0, r = e.length; n < r; n++)
                     if (e[n] === t) return n;
                 return -1
             },
             R = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
             M = "[\\x20\\t\\r\\n\\f]",
-            I = "(?:\\\\.|[\\w-]|[^\0-\\xa0])+",
+            I = "(?:\\\\[\\da-fA-F]{1,6}" + M + "?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",
             W = "\\[" + M + "*(" + I + ")(?:" + M + "*([*^$|!~]?=)" + M + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + I + "))|)" + M + "*\\]",
-            $ = ":(" + I + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + W + ")*)|.*)\\)|)",
-            F = new RegExp(M + "+", "g"),
-            B = new RegExp("^" + M + "+|((?:^|[^\\\\])(?:\\\\.)*)" + M + "+$", "g"),
+            F = ":(" + I + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + W + ")*)|.*)\\)|)",
+            B = new RegExp(M + "+", "g"),
+            $ = new RegExp("^" + M + "+|((?:^|[^\\\\])(?:\\\\.)*)" + M + "+$", "g"),
             _ = new RegExp("^" + M + "*," + M + "*"),
             z = new RegExp("^" + M + "*([>+~]|" + M + ")" + M + "*"),
             U = new RegExp(M + "|>"),
-            X = new RegExp($),
+            X = new RegExp(F),
             V = new RegExp("^" + I + "$"),
             G = {
                 ID: new RegExp("^#(" + I + ")"),
                 CLASS: new RegExp("^\\.(" + I + ")"),
                 TAG: new RegExp("^(" + I + "|[*])"),
                 ATTR: new RegExp("^" + W),
-                PSEUDO: new RegExp("^" + $),
+                PSEUDO: new RegExp("^" + F),
                 CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + M + "*(even|odd|(([+-]|)(\\d*)n|)" + M + "*(?:([+-]|)" + M + "*(\\d+)|))" + M + "*\\)|)", "i"),
                 bool: new RegExp("^(?:" + R + ")$", "i"),
                 needsContext: new RegExp("^" + M + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + M + "*((?:-\\d)?\\d*)" + M + "*\\)|)(?=[^-]|$)", "i")
             },
             Y = /HTML$/i,
             Q = /^(?:input|select|textarea|button)$/i,
             J = /^h\d$/i,
             K = /^[^{]+\{\s*\[native \w/,
             Z = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
             ee = /[+~]/,
-            te = new RegExp("\\\\([\\da-f]{1,6}" + M + "?|(" + M + ")|.)", "ig"),
-            ne = function(e, t, n) {
-                var r = "0x" + t - 65536;
-                return r != r || n ? t : r < 0 ? String.fromCharCode(r + 65536) : String.fromCharCode(r >> 10 | 55296, 1023 & r | 56320)
+            te = new RegExp("\\\\[\\da-fA-F]{1,6}" + M + "?|\\\\([^\\r\\n\\f])", "g"),
+            ne = function(e, t) {
+                var n = "0x" + e.slice(1) - 65536;
+                return t || (n < 0 ? String.fromCharCode(n + 65536) : String.fromCharCode(n >> 10 | 55296, 1023 & n | 56320))
             },
             re = /([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,
             ie = function(e, t) {
                 return t ? "\0" === e ? "\ufffd" : e.slice(0, -1) + "\\" + e.charCodeAt(e.length - 1).toString(16) + " " : "\\" + e
             },
             oe = function() {
                 T()
@@ -233,15 +243,15 @@
             ae = be(function(e) {
                 return !0 === e.disabled && "fieldset" === e.nodeName.toLowerCase()
             }, {
                 dir: "parentNode",
                 next: "legend"
             });
         try {
-            H.apply(t = O.call(m.childNodes), m.childNodes), t[m.childNodes.length].nodeType
+            H.apply(t = O.call(p.childNodes), p.childNodes), t[p.childNodes.length].nodeType
         } catch (e) {
             H = {
                 apply: t.length ? function(e, t) {
                     L.apply(e, O.call(t))
                 } : function(e, t) {
                     var n = e.length,
                         r = 0;
@@ -251,51 +261,51 @@
             }
         }
 
         function se(t, e, n, r) {
             var i, o, a, s, u, l, c, f = e && e.ownerDocument,
                 p = e ? e.nodeType : 9;
             if (n = n || [], "string" != typeof t || !t || 1 !== p && 9 !== p && 11 !== p) return n;
-            if (!r && ((e ? e.ownerDocument || e : m) !== C && T(e), e = e || C, E)) {
+            if (!r && (T(e), e = e || C, E)) {
                 if (11 !== p && (u = Z.exec(t)))
                     if (i = u[1]) {
                         if (9 === p) {
                             if (!(a = e.getElementById(i))) return n;
                             if (a.id === i) return n.push(a), n
                         } else if (f && (a = f.getElementById(i)) && y(e, a) && a.id === i) return n.push(a), n
                     } else {
                         if (u[2]) return H.apply(n, e.getElementsByTagName(t)), n;
                         if ((i = u[3]) && d.getElementsByClassName && e.getElementsByClassName) return H.apply(n, e.getElementsByClassName(i)), n
-                    } if (d.qsa && !A[t + " "] && (!v || !v.test(t)) && (1 !== p || "object" !== e.nodeName.toLowerCase())) {
-                    if (c = t, f = e, 1 === p && U.test(t)) {
-                        (s = e.getAttribute("id")) ? s = s.replace(re, ie): e.setAttribute("id", s = k), o = (l = h(t)).length;
-                        while (o--) l[o] = "#" + s + " " + xe(l[o]);
-                        c = l.join(","), f = ee.test(t) && ye(e.parentNode) || e
+                    } if (d.qsa && !N[t + " "] && (!v || !v.test(t)) && (1 !== p || "object" !== e.nodeName.toLowerCase())) {
+                    if (c = t, f = e, 1 === p && (U.test(t) || z.test(t))) {
+                        (f = ee.test(t) && ye(e.parentNode) || e) === e && d.scope || ((s = e.getAttribute("id")) ? s = s.replace(re, ie) : e.setAttribute("id", s = S)), o = (l = h(t)).length;
+                        while (o--) l[o] = (s ? "#" + s : ":scope") + " " + xe(l[o]);
+                        c = l.join(",")
                     }
                     try {
                         return H.apply(n, f.querySelectorAll(c)), n
                     } catch (e) {
-                        A(t, !0)
+                        N(t, !0)
                     } finally {
-                        s === k && e.removeAttribute("id")
+                        s === S && e.removeAttribute("id")
                     }
                 }
             }
-            return g(t.replace(B, "$1"), e, n, r)
+            return g(t.replace($, "$1"), e, n, r)
         }
 
         function ue() {
             var r = [];
             return function e(t, n) {
                 return r.push(t + " ") > b.cacheLength && delete e[r.shift()], e[t + " "] = n
             }
         }
 
         function le(e) {
-            return e[k] = !0, e
+            return e[S] = !0, e
         }
 
         function ce(e) {
             var t = C.createElement("fieldset");
             try {
                 return !!e(t)
             } catch (e) {
@@ -354,21 +364,23 @@
             return e && "undefined" != typeof e.getElementsByTagName && e
         }
         for (e in d = se.support = {}, i = se.isXML = function(e) {
                 var t = e.namespaceURI,
                     n = (e.ownerDocument || e).documentElement;
                 return !Y.test(t || n && n.nodeName || "HTML")
             }, T = se.setDocument = function(e) {
-                var t, n, r = e ? e.ownerDocument || e : m;
-                return r !== C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), m !== C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.attributes = ce(function(e) {
+                var t, n, r = e ? e.ownerDocument || e : p;
+                return r != C && 9 === r.nodeType && r.documentElement && (a = (C = r).documentElement, E = !i(C), p != C && (n = C.defaultView) && n.top !== n && (n.addEventListener ? n.addEventListener("unload", oe, !1) : n.attachEvent && n.attachEvent("onunload", oe)), d.scope = ce(function(e) {
+                    return a.appendChild(e).appendChild(C.createElement("div")), "undefined" != typeof e.querySelectorAll && !e.querySelectorAll(":scope fieldset div").length
+                }), d.attributes = ce(function(e) {
                     return e.className = "i", !e.getAttribute("className")
                 }), d.getElementsByTagName = ce(function(e) {
                     return e.appendChild(C.createComment("")), !e.getElementsByTagName("*").length
                 }), d.getElementsByClassName = K.test(C.getElementsByClassName), d.getById = ce(function(e) {
-                    return a.appendChild(e).id = k, !C.getElementsByName || !C.getElementsByName(k).length
+                    return a.appendChild(e).id = S, !C.getElementsByName || !C.getElementsByName(S).length
                 }), d.getById ? (b.filter.ID = function(e) {
                     var t = e.replace(te, ne);
                     return function(e) {
                         return e.getAttribute("id") === t
                     }
                 }, b.find.ID = function(e, t) {
                     if ("undefined" != typeof t.getElementById && E) {
@@ -402,64 +414,65 @@
                         while (n = o[i++]) 1 === n.nodeType && r.push(n);
                         return r
                     }
                     return o
                 }, b.find.CLASS = d.getElementsByClassName && function(e, t) {
                     if ("undefined" != typeof t.getElementsByClassName && E) return t.getElementsByClassName(e)
                 }, s = [], v = [], (d.qsa = K.test(C.querySelectorAll)) && (ce(function(e) {
-                    a.appendChild(e).innerHTML = "<a id='" + k + "'></a><select id='" + k + "-\r\\' msallowcapture=''><option selected=''></option></select>", e.querySelectorAll("[msallowcapture^='']").length && v.push("[*^$]=" + M + "*(?:''|\"\")"), e.querySelectorAll("[selected]").length || v.push("\\[" + M + "*(?:value|" + R + ")"), e.querySelectorAll("[id~=" + k + "-]").length || v.push("~="), e.querySelectorAll(":checked").length || v.push(":checked"), e.querySelectorAll("a#" + k + "+*").length || v.push(".#.+[+~]")
+                    var t;
+                    a.appendChild(e).innerHTML = "<a id='" + S + "'></a><select id='" + S + "-\r\\' msallowcapture=''><option selected=''></option></select>", e.querySelectorAll("[msallowcapture^='']").length && v.push("[*^$]=" + M + "*(?:''|\"\")"), e.querySelectorAll("[selected]").length || v.push("\\[" + M + "*(?:value|" + R + ")"), e.querySelectorAll("[id~=" + S + "-]").length || v.push("~="), (t = C.createElement("input")).setAttribute("name", ""), e.appendChild(t), e.querySelectorAll("[name='']").length || v.push("\\[" + M + "*name" + M + "*=" + M + "*(?:''|\"\")"), e.querySelectorAll(":checked").length || v.push(":checked"), e.querySelectorAll("a#" + S + "+*").length || v.push(".#.+[+~]"), e.querySelectorAll("\\\f"), v.push("[\\r\\n\\f]")
                 }), ce(function(e) {
                     e.innerHTML = "<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";
                     var t = C.createElement("input");
                     t.setAttribute("type", "hidden"), e.appendChild(t).setAttribute("name", "D"), e.querySelectorAll("[name=d]").length && v.push("name" + M + "*[*^$|!~]?="), 2 !== e.querySelectorAll(":enabled").length && v.push(":enabled", ":disabled"), a.appendChild(e).disabled = !0, 2 !== e.querySelectorAll(":disabled").length && v.push(":enabled", ":disabled"), e.querySelectorAll("*,:x"), v.push(",.*:")
                 })), (d.matchesSelector = K.test(c = a.matches || a.webkitMatchesSelector || a.mozMatchesSelector || a.oMatchesSelector || a.msMatchesSelector)) && ce(function(e) {
-                    d.disconnectedMatch = c.call(e, "*"), c.call(e, "[s!='']:x"), s.push("!=", $)
+                    d.disconnectedMatch = c.call(e, "*"), c.call(e, "[s!='']:x"), s.push("!=", F)
                 }), v = v.length && new RegExp(v.join("|")), s = s.length && new RegExp(s.join("|")), t = K.test(a.compareDocumentPosition), y = t || K.test(a.contains) ? function(e, t) {
                     var n = 9 === e.nodeType ? e.documentElement : e,
                         r = t && t.parentNode;
                     return e === r || !(!r || 1 !== r.nodeType || !(n.contains ? n.contains(r) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(r)))
                 } : function(e, t) {
                     if (t)
                         while (t = t.parentNode)
                             if (t === e) return !0;
                     return !1
                 }, D = t ? function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n = !e.compareDocumentPosition - !t.compareDocumentPosition;
-                    return n || (1 & (n = (e.ownerDocument || e) === (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e === C || e.ownerDocument === m && y(m, e) ? -1 : t === C || t.ownerDocument === m && y(m, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
+                    return n || (1 & (n = (e.ownerDocument || e) == (t.ownerDocument || t) ? e.compareDocumentPosition(t) : 1) || !d.sortDetached && t.compareDocumentPosition(e) === n ? e == C || e.ownerDocument == p && y(p, e) ? -1 : t == C || t.ownerDocument == p && y(p, t) ? 1 : u ? P(u, e) - P(u, t) : 0 : 4 & n ? -1 : 1)
                 } : function(e, t) {
                     if (e === t) return l = !0, 0;
                     var n, r = 0,
                         i = e.parentNode,
                         o = t.parentNode,
                         a = [e],
                         s = [t];
-                    if (!i || !o) return e === C ? -1 : t === C ? 1 : i ? -1 : o ? 1 : u ? P(u, e) - P(u, t) : 0;
+                    if (!i || !o) return e == C ? -1 : t == C ? 1 : i ? -1 : o ? 1 : u ? P(u, e) - P(u, t) : 0;
                     if (i === o) return pe(e, t);
                     n = e;
                     while (n = n.parentNode) a.unshift(n);
                     n = t;
                     while (n = n.parentNode) s.unshift(n);
                     while (a[r] === s[r]) r++;
-                    return r ? pe(a[r], s[r]) : a[r] === m ? -1 : s[r] === m ? 1 : 0
+                    return r ? pe(a[r], s[r]) : a[r] == p ? -1 : s[r] == p ? 1 : 0
                 }), C
             }, se.matches = function(e, t) {
                 return se(e, null, null, t)
             }, se.matchesSelector = function(e, t) {
-                if ((e.ownerDocument || e) !== C && T(e), d.matchesSelector && E && !A[t + " "] && (!s || !s.test(t)) && (!v || !v.test(t))) try {
+                if (T(e), d.matchesSelector && E && !N[t + " "] && (!s || !s.test(t)) && (!v || !v.test(t))) try {
                     var n = c.call(e, t);
                     if (n || d.disconnectedMatch || e.document && 11 !== e.document.nodeType) return n
                 } catch (e) {
-                    A(t, !0)
+                    N(t, !0)
                 }
                 return 0 < se(t, C, null, [e]).length
             }, se.contains = function(e, t) {
-                return (e.ownerDocument || e) !== C && T(e), y(e, t)
+                return (e.ownerDocument || e) != C && T(e), y(e, t)
             }, se.attr = function(e, t) {
-                (e.ownerDocument || e) !== C && T(e);
+                (e.ownerDocument || e) != C && T(e);
                 var n = b.attrHandle[t.toLowerCase()],
                     r = n && j.call(b.attrHandle, t.toLowerCase()) ? n(e, t, !E) : void 0;
                 return void 0 !== r ? r : d.attributes || !E ? e.getAttribute(t) : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
             }, se.escape = function(e) {
                 return (e + "").replace(re, ie)
             }, se.error = function(e) {
                 throw new Error("Syntax error, unrecognized expression: " + e)
@@ -524,23 +537,23 @@
                         return "*" === e ? function() {
                             return !0
                         } : function(e) {
                             return e.nodeName && e.nodeName.toLowerCase() === t
                         }
                     },
                     CLASS: function(e) {
-                        var t = p[e + " "];
-                        return t || (t = new RegExp("(^|" + M + ")" + e + "(" + M + "|$)")) && p(e, function(e) {
+                        var t = m[e + " "];
+                        return t || (t = new RegExp("(^|" + M + ")" + e + "(" + M + "|$)")) && m(e, function(e) {
                             return t.test("string" == typeof e.className && e.className || "undefined" != typeof e.getAttribute && e.getAttribute("class") || "")
                         })
                     },
                     ATTR: function(n, r, i) {
                         return function(e) {
                             var t = se.attr(e, n);
-                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace(F, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
+                            return null == t ? "!=" === r : !r || (t += "", "=" === r ? t === i : "!=" === r ? t !== i : "^=" === r ? i && 0 === t.indexOf(i) : "*=" === r ? i && -1 < t.indexOf(i) : "$=" === r ? i && t.slice(-i.length) === i : "~=" === r ? -1 < (" " + t.replace(B, " ") + " ").indexOf(i) : "|=" === r && (t === i || t.slice(0, i.length + 1) === i + "-"))
                         }
                     },
                     CHILD: function(h, e, t, g, v) {
                         var y = "nth" !== h.slice(0, 3),
                             m = "last" !== h.slice(-4),
                             x = "of-type" === e;
                         return 1 === g && 0 === v ? function(e) {
@@ -558,44 +571,44 @@
                                         while (a = a[l])
                                             if (x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) return !1;
                                         u = l = "only" === h && !u && "nextSibling"
                                     }
                                     return !0
                                 }
                                 if (u = [m ? c.firstChild : c.lastChild], m && p) {
-                                    d = (s = (r = (i = (o = (a = c)[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === S && r[1]) && r[2], a = s && c.childNodes[s];
+                                    d = (s = (r = (i = (o = (a = c)[S] || (a[S] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === k && r[1]) && r[2], a = s && c.childNodes[s];
                                     while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
                                         if (1 === a.nodeType && ++d && a === e) {
-                                            i[h] = [S, s, d];
+                                            i[h] = [k, s, d];
                                             break
                                         }
-                                } else if (p && (d = s = (r = (i = (o = (a = e)[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === S && r[1]), !1 === d)
+                                } else if (p && (d = s = (r = (i = (o = (a = e)[S] || (a[S] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] || [])[0] === k && r[1]), !1 === d)
                                     while (a = ++s && a && a[l] || (d = s = 0) || u.pop())
-                                        if ((x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) && ++d && (p && ((i = (o = a[k] || (a[k] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] = [S, d]), a === e)) break;
+                                        if ((x ? a.nodeName.toLowerCase() === f : 1 === a.nodeType) && ++d && (p && ((i = (o = a[S] || (a[S] = {}))[a.uniqueID] || (o[a.uniqueID] = {}))[h] = [k, d]), a === e)) break;
                                 return (d -= v) === g || d % g == 0 && 0 <= d / g
                             }
                         }
                     },
                     PSEUDO: function(e, o) {
                         var t, a = b.pseudos[e] || b.setFilters[e.toLowerCase()] || se.error("unsupported pseudo: " + e);
-                        return a[k] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? le(function(e, t) {
+                        return a[S] ? a(o) : 1 < a.length ? (t = [e, e, "", o], b.setFilters.hasOwnProperty(e.toLowerCase()) ? le(function(e, t) {
                             var n, r = a(e, o),
                                 i = r.length;
                             while (i--) e[n = P(e, r[i])] = !(t[n] = r[i])
                         }) : function(e) {
                             return a(e, 0, t)
                         }) : a
                     }
                 },
                 pseudos: {
                     not: le(function(e) {
                         var r = [],
                             i = [],
-                            s = f(e.replace(B, "$1"));
-                        return s[k] ? le(function(e, t, n, r) {
+                            s = f(e.replace($, "$1"));
+                        return s[S] ? le(function(e, t, n, r) {
                             var i, o = s(e, null, r, []),
                                 a = e.length;
                             while (a--)(i = o[a]) && (e[a] = !(t[a] = i))
                         }) : function(e, t, n) {
                             return r[0] = e, s(r, null, n, i), r[0] = null, !i.pop()
                         }
                     }),
@@ -713,24 +726,24 @@
                 f = t && "parentNode" === c,
                 p = r++;
             return e.first ? function(e, t, n) {
                 while (e = e[u])
                     if (1 === e.nodeType || f) return s(e, t, n);
                 return !1
             } : function(e, t, n) {
-                var r, i, o, a = [S, p];
+                var r, i, o, a = [k, p];
                 if (n) {
                     while (e = e[u])
                         if ((1 === e.nodeType || f) && s(e, t, n)) return !0
                 } else
                     while (e = e[u])
                         if (1 === e.nodeType || f)
-                            if (i = (o = e[k] || (e[k] = {}))[e.uniqueID] || (o[e.uniqueID] = {}), l && l === e.nodeName.toLowerCase()) e = e[u] || e;
+                            if (i = (o = e[S] || (e[S] = {}))[e.uniqueID] || (o[e.uniqueID] = {}), l && l === e.nodeName.toLowerCase()) e = e[u] || e;
                             else {
-                                if ((r = i[c]) && r[0] === S && r[1] === p) return a[2] = r[2];
+                                if ((r = i[c]) && r[0] === k && r[1] === p) return a[2] = r[2];
                                 if ((i[c] = a)[2] = s(e, t, n)) return !0
                             } return !1
             }
         }
 
         function we(i) {
             return 1 < i.length ? function(e, t, n) {
@@ -743,15 +756,15 @@
 
         function Te(e, t, n, r, i) {
             for (var o, a = [], s = 0, u = e.length, l = null != t; s < u; s++)(o = e[s]) && (n && !n(o, r, i) || (a.push(o), l && t.push(s)));
             return a
         }
 
         function Ce(d, h, g, v, y, e) {
-            return v && !v[k] && (v = Ce(v)), y && !y[k] && (y = Ce(y, e)), le(function(e, t, n, r) {
+            return v && !v[S] && (v = Ce(v)), y && !y[S] && (y = Ce(y, e)), le(function(e, t, n, r) {
                 var i, o, a, s = [],
                     u = [],
                     l = t.length,
                     c = e || function(e, t, n) {
                         for (var r = 0, i = t.length; r < i; r++) se(e, t[r], n);
                         return n
                     }(h || "*", n.nodeType ? [n] : n, []),
@@ -782,78 +795,78 @@
                     return -1 < P(i, e)
                 }, a, !0), c = [function(e, t, n) {
                     var r = !o && (n || t !== w) || ((i = t).nodeType ? u(e, t, n) : l(e, t, n));
                     return i = null, r
                 }]; s < r; s++)
                 if (t = b.relative[e[s].type]) c = [be(we(c), t)];
                 else {
-                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[k]) {
+                    if ((t = b.filter[e[s].type].apply(null, e[s].matches))[S]) {
                         for (n = ++s; n < r; n++)
                             if (b.relative[e[n].type]) break;
                         return Ce(1 < s && we(c), 1 < s && xe(e.slice(0, s - 1).concat({
                             value: " " === e[s - 2].type ? "*" : ""
-                        })).replace(B, "$1"), t, s < n && Ee(e.slice(s, n)), n < r && Ee(e = e.slice(n)), n < r && xe(e))
+                        })).replace($, "$1"), t, s < n && Ee(e.slice(s, n)), n < r && Ee(e = e.slice(n)), n < r && xe(e))
                     }
                     c.push(t)
                 } return we(c)
         }
         return me.prototype = b.filters = b.pseudos, b.setFilters = new me, h = se.tokenize = function(e, t) {
             var n, r, i, o, a, s, u, l = x[e + " "];
             if (l) return t ? 0 : l.slice(0);
             a = e, s = [], u = b.preFilter;
             while (a) {
                 for (o in n && !(r = _.exec(a)) || (r && (a = a.slice(r[0].length) || a), s.push(i = [])), n = !1, (r = z.exec(a)) && (n = r.shift(), i.push({
                         value: n,
-                        type: r[0].replace(B, " ")
+                        type: r[0].replace($, " ")
                     }), a = a.slice(n.length)), b.filter) !(r = G[o].exec(a)) || u[o] && !(r = u[o](r)) || (n = r.shift(), i.push({
                     value: n,
                     type: o,
                     matches: r
                 }), a = a.slice(n.length));
                 if (!n) break
             }
             return t ? a.length : a ? se.error(e) : x(e, s).slice(0)
         }, f = se.compile = function(e, t) {
             var n, v, y, m, x, r, i = [],
                 o = [],
-                a = N[e + " "];
+                a = A[e + " "];
             if (!a) {
                 t || (t = h(e)), n = t.length;
-                while (n--)(a = Ee(t[n]))[k] ? i.push(a) : o.push(a);
-                (a = N(e, (v = o, m = 0 < (y = i).length, x = 0 < v.length, r = function(e, t, n, r, i) {
+                while (n--)(a = Ee(t[n]))[S] ? i.push(a) : o.push(a);
+                (a = A(e, (v = o, m = 0 < (y = i).length, x = 0 < v.length, r = function(e, t, n, r, i) {
                     var o, a, s, u = 0,
                         l = "0",
                         c = e && [],
                         f = [],
                         p = w,
                         d = e || x && b.find.TAG("*", i),
-                        h = S += null == p ? 1 : Math.random() || .1,
+                        h = k += null == p ? 1 : Math.random() || .1,
                         g = d.length;
-                    for (i && (w = t === C || t || i); l !== g && null != (o = d[l]); l++) {
+                    for (i && (w = t == C || t || i); l !== g && null != (o = d[l]); l++) {
                         if (x && o) {
-                            a = 0, t || o.ownerDocument === C || (T(o), n = !E);
+                            a = 0, t || o.ownerDocument == C || (T(o), n = !E);
                             while (s = v[a++])
                                 if (s(o, t || C, n)) {
                                     r.push(o);
                                     break
-                                } i && (S = h)
+                                } i && (k = h)
                         }
                         m && ((o = !s && o) && u--, e && c.push(o))
                     }
                     if (u += l, m && l !== u) {
                         a = 0;
                         while (s = y[a++]) s(c, f, t, n);
                         if (e) {
                             if (0 < u)
                                 while (l--) c[l] || f[l] || (f[l] = q.call(r));
                             f = Te(f)
                         }
                         H.apply(r, f), i && !e && 0 < f.length && 1 < u + y.length && se.uniqueSort(r)
                     }
-                    return i && (S = h, w = p), c
+                    return i && (k = h, w = p), c
                 }, m ? le(r) : r))).selector = e
             }
             return a
         }, g = se.select = function(e, t, n, r) {
             var i, o, a, s, u, l = "function" == typeof e && e,
                 c = !r && h(e = l.selector || e);
             if (n = n || [], 1 === c.length) {
@@ -867,15 +880,15 @@
                     if ((u = b.find[s]) && (r = u(a.matches[0].replace(te, ne), ee.test(o[0].type) && ye(t.parentNode) || t))) {
                         if (o.splice(i, 1), !(e = r.length && xe(o))) return H.apply(n, r), n;
                         break
                     }
                 }
             }
             return (l || f(e, c))(r, t, !E, n, !t || ee.test(e) && ye(t.parentNode) || t), n
-        }, d.sortStable = k.split("").sort(D).join("") === k, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
+        }, d.sortStable = S.split("").sort(D).join("") === S, d.detectDuplicates = !!l, T(), d.sortDetached = ce(function(e) {
             return 1 & e.compareDocumentPosition(C.createElement("fieldset"))
         }), ce(function(e) {
             return e.innerHTML = "<a href='#'></a>", "#" === e.firstChild.getAttribute("href")
         }) || fe("type|href|height|width", function(e, t, n) {
             if (!n) return e.getAttribute(t, "type" === t.toLowerCase() ? 1 : 2)
         }), d.attributes && ce(function(e) {
             return e.innerHTML = "<input/>", e.firstChild.setAttribute("value", ""), "" === e.firstChild.getAttribute("value")
@@ -884,221 +897,221 @@
         }), ce(function(e) {
             return null == e.getAttribute("disabled")
         }) || fe(R, function(e, t, n) {
             var r;
             if (!n) return !0 === e[t] ? t.toLowerCase() : (r = e.getAttributeNode(t)) && r.specified ? r.value : null
         }), se
     }(C);
-    k.find = h, k.expr = h.selectors, k.expr[":"] = k.expr.pseudos, k.uniqueSort = k.unique = h.uniqueSort, k.text = h.getText, k.isXMLDoc = h.isXML, k.contains = h.contains, k.escapeSelector = h.escape;
-    var T = function(e, t, n) {
+    S.find = d, S.expr = d.selectors, S.expr[":"] = S.expr.pseudos, S.uniqueSort = S.unique = d.uniqueSort, S.text = d.getText, S.isXMLDoc = d.isXML, S.contains = d.contains, S.escapeSelector = d.escape;
+    var h = function(e, t, n) {
             var r = [],
                 i = void 0 !== n;
             while ((e = e[t]) && 9 !== e.nodeType)
                 if (1 === e.nodeType) {
-                    if (i && k(e).is(n)) break;
+                    if (i && S(e).is(n)) break;
                     r.push(e)
                 } return r
         },
-        S = function(e, t) {
+        T = function(e, t) {
             for (var n = []; e; e = e.nextSibling) 1 === e.nodeType && e !== t && n.push(e);
             return n
         },
-        N = k.expr.match.needsContext;
+        k = S.expr.match.needsContext;
 
     function A(e, t) {
         return e.nodeName && e.nodeName.toLowerCase() === t.toLowerCase()
     }
-    var D = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
+    var N = /^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;
 
-    function j(e, n, r) {
-        return m(n) ? k.grep(e, function(e, t) {
+    function D(e, n, r) {
+        return m(n) ? S.grep(e, function(e, t) {
             return !!n.call(e, t, e) !== r
-        }) : n.nodeType ? k.grep(e, function(e) {
+        }) : n.nodeType ? S.grep(e, function(e) {
             return e === n !== r
-        }) : "string" != typeof n ? k.grep(e, function(e) {
+        }) : "string" != typeof n ? S.grep(e, function(e) {
             return -1 < i.call(n, e) !== r
-        }) : k.filter(n, e, r)
+        }) : S.filter(n, e, r)
     }
-    k.filter = function(e, t, n) {
+    S.filter = function(e, t, n) {
         var r = t[0];
-        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? k.find.matchesSelector(r, e) ? [r] : [] : k.find.matches(e, k.grep(t, function(e) {
+        return n && (e = ":not(" + e + ")"), 1 === t.length && 1 === r.nodeType ? S.find.matchesSelector(r, e) ? [r] : [] : S.find.matches(e, S.grep(t, function(e) {
             return 1 === e.nodeType
         }))
-    }, k.fn.extend({
+    }, S.fn.extend({
         find: function(e) {
             var t, n, r = this.length,
                 i = this;
-            if ("string" != typeof e) return this.pushStack(k(e).filter(function() {
+            if ("string" != typeof e) return this.pushStack(S(e).filter(function() {
                 for (t = 0; t < r; t++)
-                    if (k.contains(i[t], this)) return !0
+                    if (S.contains(i[t], this)) return !0
             }));
-            for (n = this.pushStack([]), t = 0; t < r; t++) k.find(e, i[t], n);
-            return 1 < r ? k.uniqueSort(n) : n
+            for (n = this.pushStack([]), t = 0; t < r; t++) S.find(e, i[t], n);
+            return 1 < r ? S.uniqueSort(n) : n
         },
         filter: function(e) {
-            return this.pushStack(j(this, e || [], !1))
+            return this.pushStack(D(this, e || [], !1))
         },
         not: function(e) {
-            return this.pushStack(j(this, e || [], !0))
+            return this.pushStack(D(this, e || [], !0))
         },
         is: function(e) {
-            return !!j(this, "string" == typeof e && N.test(e) ? k(e) : e || [], !1).length
+            return !!D(this, "string" == typeof e && k.test(e) ? S(e) : e || [], !1).length
         }
     });
-    var q, L = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
-    (k.fn.init = function(e, t, n) {
+    var j, q = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;
+    (S.fn.init = function(e, t, n) {
         var r, i;
         if (!e) return this;
-        if (n = n || q, "string" == typeof e) {
-            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : L.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
+        if (n = n || j, "string" == typeof e) {
+            if (!(r = "<" === e[0] && ">" === e[e.length - 1] && 3 <= e.length ? [null, e, null] : q.exec(e)) || !r[1] && t) return !t || t.jquery ? (t || n).find(e) : this.constructor(t).find(e);
             if (r[1]) {
-                if (t = t instanceof k ? t[0] : t, k.merge(this, k.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), D.test(r[1]) && k.isPlainObject(t))
+                if (t = t instanceof S ? t[0] : t, S.merge(this, S.parseHTML(r[1], t && t.nodeType ? t.ownerDocument || t : E, !0)), N.test(r[1]) && S.isPlainObject(t))
                     for (r in t) m(this[r]) ? this[r](t[r]) : this.attr(r, t[r]);
                 return this
             }
             return (i = E.getElementById(r[2])) && (this[0] = i, this.length = 1), this
         }
-        return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(k) : k.makeArray(e, this)
-    }).prototype = k.fn, q = k(E);
-    var H = /^(?:parents|prev(?:Until|All))/,
-        O = {
+        return e.nodeType ? (this[0] = e, this.length = 1, this) : m(e) ? void 0 !== n.ready ? n.ready(e) : e(S) : S.makeArray(e, this)
+    }).prototype = S.fn, j = S(E);
+    var L = /^(?:parents|prev(?:Until|All))/,
+        H = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
 
-    function P(e, t) {
+    function O(e, t) {
         while ((e = e[t]) && 1 !== e.nodeType);
         return e
     }
-    k.fn.extend({
+    S.fn.extend({
         has: function(e) {
-            var t = k(e, this),
+            var t = S(e, this),
                 n = t.length;
             return this.filter(function() {
                 for (var e = 0; e < n; e++)
-                    if (k.contains(this, t[e])) return !0
+                    if (S.contains(this, t[e])) return !0
             })
         },
         closest: function(e, t) {
             var n, r = 0,
                 i = this.length,
                 o = [],
-                a = "string" != typeof e && k(e);
-            if (!N.test(e))
+                a = "string" != typeof e && S(e);
+            if (!k.test(e))
                 for (; r < i; r++)
                     for (n = this[r]; n && n !== t; n = n.parentNode)
-                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && k.find.matchesSelector(n, e))) {
+                        if (n.nodeType < 11 && (a ? -1 < a.index(n) : 1 === n.nodeType && S.find.matchesSelector(n, e))) {
                             o.push(n);
                             break
-                        } return this.pushStack(1 < o.length ? k.uniqueSort(o) : o)
+                        } return this.pushStack(1 < o.length ? S.uniqueSort(o) : o)
         },
         index: function(e) {
-            return e ? "string" == typeof e ? i.call(k(e), this[0]) : i.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
+            return e ? "string" == typeof e ? i.call(S(e), this[0]) : i.call(this, e.jquery ? e[0] : e) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
         },
         add: function(e, t) {
-            return this.pushStack(k.uniqueSort(k.merge(this.get(), k(e, t))))
+            return this.pushStack(S.uniqueSort(S.merge(this.get(), S(e, t))))
         },
         addBack: function(e) {
             return this.add(null == e ? this.prevObject : this.prevObject.filter(e))
         }
-    }), k.each({
+    }), S.each({
         parent: function(e) {
             var t = e.parentNode;
             return t && 11 !== t.nodeType ? t : null
         },
         parents: function(e) {
-            return T(e, "parentNode")
+            return h(e, "parentNode")
         },
         parentsUntil: function(e, t, n) {
-            return T(e, "parentNode", n)
+            return h(e, "parentNode", n)
         },
         next: function(e) {
-            return P(e, "nextSibling")
+            return O(e, "nextSibling")
         },
         prev: function(e) {
-            return P(e, "previousSibling")
+            return O(e, "previousSibling")
         },
         nextAll: function(e) {
-            return T(e, "nextSibling")
+            return h(e, "nextSibling")
         },
         prevAll: function(e) {
-            return T(e, "previousSibling")
+            return h(e, "previousSibling")
         },
         nextUntil: function(e, t, n) {
-            return T(e, "nextSibling", n)
+            return h(e, "nextSibling", n)
         },
         prevUntil: function(e, t, n) {
-            return T(e, "previousSibling", n)
+            return h(e, "previousSibling", n)
         },
         siblings: function(e) {
-            return S((e.parentNode || {}).firstChild, e)
+            return T((e.parentNode || {}).firstChild, e)
         },
         children: function(e) {
-            return S(e.firstChild)
+            return T(e.firstChild)
         },
         contents: function(e) {
-            return "undefined" != typeof e.contentDocument ? e.contentDocument : (A(e, "template") && (e = e.content || e), k.merge([], e.childNodes))
+            return null != e.contentDocument && r(e.contentDocument) ? e.contentDocument : (A(e, "template") && (e = e.content || e), S.merge([], e.childNodes))
         }
     }, function(r, i) {
-        k.fn[r] = function(e, t) {
-            var n = k.map(this, i, e);
-            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = k.filter(t, n)), 1 < this.length && (O[r] || k.uniqueSort(n), H.test(r) && n.reverse()), this.pushStack(n)
+        S.fn[r] = function(e, t) {
+            var n = S.map(this, i, e);
+            return "Until" !== r.slice(-5) && (t = e), t && "string" == typeof t && (n = S.filter(t, n)), 1 < this.length && (H[r] || S.uniqueSort(n), L.test(r) && n.reverse()), this.pushStack(n)
         }
     });
-    var R = /[^\x20\t\r\n\f]+/g;
+    var P = /[^\x20\t\r\n\f]+/g;
 
-    function M(e) {
+    function R(e) {
         return e
     }
 
-    function I(e) {
+    function M(e) {
         throw e
     }
 
-    function W(e, t, n, r) {
+    function I(e, t, n, r) {
         var i;
         try {
             e && m(i = e.promise) ? i.call(e).done(t).fail(n) : e && m(i = e.then) ? i.call(e, t, n) : t.apply(void 0, [e].slice(r))
         } catch (e) {
             n.apply(void 0, [e])
         }
     }
-    k.Callbacks = function(r) {
+    S.Callbacks = function(r) {
         var e, n;
-        r = "string" == typeof r ? (e = r, n = {}, k.each(e.match(R) || [], function(e, t) {
+        r = "string" == typeof r ? (e = r, n = {}, S.each(e.match(P) || [], function(e, t) {
             n[t] = !0
-        }), n) : k.extend({}, r);
+        }), n) : S.extend({}, r);
         var i, t, o, a, s = [],
             u = [],
             l = -1,
             c = function() {
                 for (a = a || r.once, o = i = !0; u.length; l = -1) {
                     t = u.shift();
                     while (++l < s.length) !1 === s[l].apply(t[0], t[1]) && r.stopOnFalse && (l = s.length, t = !1)
                 }
                 r.memory || (t = !1), i = !1, a && (s = t ? [] : "")
             },
             f = {
                 add: function() {
                     return s && (t && !i && (l = s.length - 1, u.push(t)), function n(e) {
-                        k.each(e, function(e, t) {
+                        S.each(e, function(e, t) {
                             m(t) ? r.unique && f.has(t) || s.push(t) : t && t.length && "string" !== w(t) && n(t)
                         })
                     }(arguments), t && !i && c()), this
                 },
                 remove: function() {
-                    return k.each(arguments, function(e, t) {
+                    return S.each(arguments, function(e, t) {
                         var n;
-                        while (-1 < (n = k.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
+                        while (-1 < (n = S.inArray(t, s, n))) s.splice(n, 1), n <= l && l--
                     }), this
                 },
                 has: function(e) {
-                    return e ? -1 < k.inArray(e, s) : 0 < s.length
+                    return e ? -1 < S.inArray(e, s) : 0 < s.length
                 },
                 empty: function() {
                     return s && (s = []), this
                 },
                 disable: function() {
                     return a = u = [], s = t = "", this
                 },
@@ -1118,36 +1131,36 @@
                     return f.fireWith(this, arguments), this
                 },
                 fired: function() {
                     return !!o
                 }
             };
         return f
-    }, k.extend({
+    }, S.extend({
         Deferred: function(e) {
             var o = [
-                    ["notify", "progress", k.Callbacks("memory"), k.Callbacks("memory"), 2],
-                    ["resolve", "done", k.Callbacks("once memory"), k.Callbacks("once memory"), 0, "resolved"],
-                    ["reject", "fail", k.Callbacks("once memory"), k.Callbacks("once memory"), 1, "rejected"]
+                    ["notify", "progress", S.Callbacks("memory"), S.Callbacks("memory"), 2],
+                    ["resolve", "done", S.Callbacks("once memory"), S.Callbacks("once memory"), 0, "resolved"],
+                    ["reject", "fail", S.Callbacks("once memory"), S.Callbacks("once memory"), 1, "rejected"]
                 ],
                 i = "pending",
                 a = {
                     state: function() {
                         return i
                     },
                     always: function() {
                         return s.done(arguments).fail(arguments), this
                     },
                     "catch": function(e) {
                         return a.then(null, e)
                     },
                     pipe: function() {
                         var i = arguments;
-                        return k.Deferred(function(r) {
-                            k.each(o, function(e, t) {
+                        return S.Deferred(function(r) {
+                            S.each(o, function(e, t) {
                                 var n = m(i[t[4]]) && i[t[4]];
                                 s[t[1]](function() {
                                     var e = n && n.apply(this, arguments);
                                     e && m(e.promise) ? e.promise().progress(r.notify).done(r.resolve).fail(r.reject) : r[t[0] + "With"](this, n ? [e] : arguments)
                                 })
                             }), i = null
                         }).promise()
@@ -1159,480 +1172,473 @@
                             return function() {
                                 var n = this,
                                     r = arguments,
                                     e = function() {
                                         var e, t;
                                         if (!(i < u)) {
                                             if ((e = a.apply(n, r)) === o.promise()) throw new TypeError("Thenable self-resolution");
-                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, m(t) ? s ? t.call(e, l(u, o, M, s), l(u, o, I, s)) : (u++, t.call(e, l(u, o, M, s), l(u, o, I, s), l(u, o, M, o.notifyWith))) : (a !== M && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
+                                            t = e && ("object" == typeof e || "function" == typeof e) && e.then, m(t) ? s ? t.call(e, l(u, o, R, s), l(u, o, M, s)) : (u++, t.call(e, l(u, o, R, s), l(u, o, M, s), l(u, o, R, o.notifyWith))) : (a !== R && (n = void 0, r = [e]), (s || o.resolveWith)(n, r))
                                         }
                                     },
                                     t = s ? e : function() {
                                         try {
                                             e()
                                         } catch (e) {
-                                            k.Deferred.exceptionHook && k.Deferred.exceptionHook(e, t.stackTrace), u <= i + 1 && (a !== I && (n = void 0, r = [e]), o.rejectWith(n, r))
+                                            S.Deferred.exceptionHook && S.Deferred.exceptionHook(e, t.stackTrace), u <= i + 1 && (a !== M && (n = void 0, r = [e]), o.rejectWith(n, r))
                                         }
                                     };
-                                i ? t() : (k.Deferred.getStackHook && (t.stackTrace = k.Deferred.getStackHook()), C.setTimeout(t))
+                                i ? t() : (S.Deferred.getStackHook && (t.stackTrace = S.Deferred.getStackHook()), C.setTimeout(t))
                             }
                         }
-                        return k.Deferred(function(e) {
-                            o[0][3].add(l(0, e, m(r) ? r : M, e.notifyWith)), o[1][3].add(l(0, e, m(t) ? t : M)), o[2][3].add(l(0, e, m(n) ? n : I))
+                        return S.Deferred(function(e) {
+                            o[0][3].add(l(0, e, m(r) ? r : R, e.notifyWith)), o[1][3].add(l(0, e, m(t) ? t : R)), o[2][3].add(l(0, e, m(n) ? n : M))
                         }).promise()
                     },
                     promise: function(e) {
-                        return null != e ? k.extend(e, a) : a
+                        return null != e ? S.extend(e, a) : a
                     }
                 },
                 s = {};
-            return k.each(o, function(e, t) {
+            return S.each(o, function(e, t) {
                 var n = t[2],
                     r = t[5];
                 a[t[1]] = n.add, r && n.add(function() {
                     i = r
                 }, o[3 - e][2].disable, o[3 - e][3].disable, o[0][2].lock, o[0][3].lock), n.add(t[3].fire), s[t[0]] = function() {
                     return s[t[0] + "With"](this === s ? void 0 : this, arguments), this
                 }, s[t[0] + "With"] = n.fireWith
             }), a.promise(s), e && e.call(s, s), s
         },
         when: function(e) {
             var n = arguments.length,
                 t = n,
                 r = Array(t),
                 i = s.call(arguments),
-                o = k.Deferred(),
+                o = S.Deferred(),
                 a = function(t) {
                     return function(e) {
                         r[t] = this, i[t] = 1 < arguments.length ? s.call(arguments) : e, --n || o.resolveWith(r, i)
                     }
                 };
-            if (n <= 1 && (W(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || m(i[t] && i[t].then))) return o.then();
-            while (t--) W(i[t], a(t), o.reject);
+            if (n <= 1 && (I(e, o.done(a(t)).resolve, o.reject, !n), "pending" === o.state() || m(i[t] && i[t].then))) return o.then();
+            while (t--) I(i[t], a(t), o.reject);
             return o.promise()
         }
     });
-    var $ = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
-    k.Deferred.exceptionHook = function(e, t) {
-        C.console && C.console.warn && e && $.test(e.name) && C.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
-    }, k.readyException = function(e) {
+    var W = /^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;
+    S.Deferred.exceptionHook = function(e, t) {
+        C.console && C.console.warn && e && W.test(e.name) && C.console.warn("jQuery.Deferred exception: " + e.message, e.stack, t)
+    }, S.readyException = function(e) {
         C.setTimeout(function() {
             throw e
         })
     };
-    var F = k.Deferred();
+    var F = S.Deferred();
 
     function B() {
-        E.removeEventListener("DOMContentLoaded", B), C.removeEventListener("load", B), k.ready()
+        E.removeEventListener("DOMContentLoaded", B), C.removeEventListener("load", B), S.ready()
     }
-    k.fn.ready = function(e) {
+    S.fn.ready = function(e) {
         return F.then(e)["catch"](function(e) {
-            k.readyException(e)
+            S.readyException(e)
         }), this
-    }, k.extend({
+    }, S.extend({
         isReady: !1,
         readyWait: 1,
         ready: function(e) {
-            (!0 === e ? --k.readyWait : k.isReady) || (k.isReady = !0) !== e && 0 < --k.readyWait || F.resolveWith(E, [k])
+            (!0 === e ? --S.readyWait : S.isReady) || (S.isReady = !0) !== e && 0 < --S.readyWait || F.resolveWith(E, [S])
         }
-    }), k.ready.then = F.then, "complete" === E.readyState || "loading" !== E.readyState && !E.documentElement.doScroll ? C.setTimeout(k.ready) : (E.addEventListener("DOMContentLoaded", B), C.addEventListener("load", B));
-    var _ = function(e, t, n, r, i, o, a) {
+    }), S.ready.then = F.then, "complete" === E.readyState || "loading" !== E.readyState && !E.documentElement.doScroll ? C.setTimeout(S.ready) : (E.addEventListener("DOMContentLoaded", B), C.addEventListener("load", B));
+    var $ = function(e, t, n, r, i, o, a) {
             var s = 0,
                 u = e.length,
                 l = null == n;
             if ("object" === w(n))
-                for (s in i = !0, n) _(e, t, s, n[s], !0, o, a);
+                for (s in i = !0, n) $(e, t, s, n[s], !0, o, a);
             else if (void 0 !== r && (i = !0, m(r) || (a = !0), l && (a ? (t.call(e, r), t = null) : (l = t, t = function(e, t, n) {
-                    return l.call(k(e), n)
+                    return l.call(S(e), n)
                 })), t))
                 for (; s < u; s++) t(e[s], n, a ? r : r.call(e[s], s, t(e[s], n)));
             return i ? e : l ? t.call(e) : u ? t(e[0], n) : o
         },
-        z = /^-ms-/,
-        U = /-([a-z])/g;
+        _ = /^-ms-/,
+        z = /-([a-z])/g;
 
-    function X(e, t) {
+    function U(e, t) {
         return t.toUpperCase()
     }
 
-    function V(e) {
-        return e.replace(z, "ms-").replace(U, X)
+    function X(e) {
+        return e.replace(_, "ms-").replace(z, U)
     }
-    var G = function(e) {
+    var V = function(e) {
         return 1 === e.nodeType || 9 === e.nodeType || !+e.nodeType
     };
 
-    function Y() {
-        this.expando = k.expando + Y.uid++
+    function G() {
+        this.expando = S.expando + G.uid++
     }
-    Y.uid = 1, Y.prototype = {
+    G.uid = 1, G.prototype = {
         cache: function(e) {
             var t = e[this.expando];
-            return t || (t = {}, G(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
+            return t || (t = Object.create(null), V(e) && (e.nodeType ? e[this.expando] = t : Object.defineProperty(e, this.expando, {
                 value: t,
                 configurable: !0
             }))), t
         },
         set: function(e, t, n) {
             var r, i = this.cache(e);
-            if ("string" == typeof t) i[V(t)] = n;
+            if ("string" == typeof t) i[X(t)] = n;
             else
-                for (r in t) i[V(r)] = t[r];
+                for (r in t) i[X(r)] = t[r];
             return i
         },
         get: function(e, t) {
-            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][V(t)]
+            return void 0 === t ? this.cache(e) : e[this.expando] && e[this.expando][X(t)]
         },
         access: function(e, t, n) {
             return void 0 === t || t && "string" == typeof t && void 0 === n ? this.get(e, t) : (this.set(e, t, n), void 0 !== n ? n : t)
         },
         remove: function(e, t) {
             var n, r = e[this.expando];
             if (void 0 !== r) {
                 if (void 0 !== t) {
-                    n = (t = Array.isArray(t) ? t.map(V) : (t = V(t)) in r ? [t] : t.match(R) || []).length;
+                    n = (t = Array.isArray(t) ? t.map(X) : (t = X(t)) in r ? [t] : t.match(P) || []).length;
                     while (n--) delete r[t[n]]
-                }(void 0 === t || k.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
+                }(void 0 === t || S.isEmptyObject(r)) && (e.nodeType ? e[this.expando] = void 0 : delete e[this.expando])
             }
         },
         hasData: function(e) {
             var t = e[this.expando];
-            return void 0 !== t && !k.isEmptyObject(t)
+            return void 0 !== t && !S.isEmptyObject(t)
         }
     };
-    var Q = new Y,
-        J = new Y,
-        K = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-        Z = /[A-Z]/g;
+    var Y = new G,
+        Q = new G,
+        J = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        K = /[A-Z]/g;
 
-    function ee(e, t, n) {
+    function Z(e, t, n) {
         var r, i;
         if (void 0 === n && 1 === e.nodeType)
-            if (r = "data-" + t.replace(Z, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
+            if (r = "data-" + t.replace(K, "-$&").toLowerCase(), "string" == typeof(n = e.getAttribute(r))) {
                 try {
-                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : K.test(i) ? JSON.parse(i) : i)
+                    n = "true" === (i = n) || "false" !== i && ("null" === i ? null : i === +i + "" ? +i : J.test(i) ? JSON.parse(i) : i)
                 } catch (e) {}
-                J.set(e, t, n)
+                Q.set(e, t, n)
             } else n = void 0;
         return n
     }
-    k.extend({
+    S.extend({
         hasData: function(e) {
-            return J.hasData(e) || Q.hasData(e)
+            return Q.hasData(e) || Y.hasData(e)
         },
         data: function(e, t, n) {
-            return J.access(e, t, n)
+            return Q.access(e, t, n)
         },
         removeData: function(e, t) {
-            J.remove(e, t)
+            Q.remove(e, t)
         },
         _data: function(e, t, n) {
-            return Q.access(e, t, n)
+            return Y.access(e, t, n)
         },
         _removeData: function(e, t) {
-            Q.remove(e, t)
+            Y.remove(e, t)
         }
-    }), k.fn.extend({
+    }), S.fn.extend({
         data: function(n, e) {
             var t, r, i, o = this[0],
                 a = o && o.attributes;
             if (void 0 === n) {
-                if (this.length && (i = J.get(o), 1 === o.nodeType && !Q.get(o, "hasDataAttrs"))) {
+                if (this.length && (i = Q.get(o), 1 === o.nodeType && !Y.get(o, "hasDataAttrs"))) {
                     t = a.length;
-                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = V(r.slice(5)), ee(o, r, i[r]));
-                    Q.set(o, "hasDataAttrs", !0)
+                    while (t--) a[t] && 0 === (r = a[t].name).indexOf("data-") && (r = X(r.slice(5)), Z(o, r, i[r]));
+                    Y.set(o, "hasDataAttrs", !0)
                 }
                 return i
             }
             return "object" == typeof n ? this.each(function() {
-                J.set(this, n)
-            }) : _(this, function(e) {
+                Q.set(this, n)
+            }) : $(this, function(e) {
                 var t;
-                if (o && void 0 === e) return void 0 !== (t = J.get(o, n)) ? t : void 0 !== (t = ee(o, n)) ? t : void 0;
+                if (o && void 0 === e) return void 0 !== (t = Q.get(o, n)) ? t : void 0 !== (t = Z(o, n)) ? t : void 0;
                 this.each(function() {
-                    J.set(this, n, e)
+                    Q.set(this, n, e)
                 })
             }, null, e, 1 < arguments.length, null, !0)
         },
         removeData: function(e) {
             return this.each(function() {
-                J.remove(this, e)
+                Q.remove(this, e)
             })
         }
-    }), k.extend({
+    }), S.extend({
         queue: function(e, t, n) {
             var r;
-            if (e) return t = (t || "fx") + "queue", r = Q.get(e, t), n && (!r || Array.isArray(n) ? r = Q.access(e, t, k.makeArray(n)) : r.push(n)), r || []
+            if (e) return t = (t || "fx") + "queue", r = Y.get(e, t), n && (!r || Array.isArray(n) ? r = Y.access(e, t, S.makeArray(n)) : r.push(n)), r || []
         },
         dequeue: function(e, t) {
             t = t || "fx";
-            var n = k.queue(e, t),
+            var n = S.queue(e, t),
                 r = n.length,
                 i = n.shift(),
-                o = k._queueHooks(e, t);
+                o = S._queueHooks(e, t);
             "inprogress" === i && (i = n.shift(), r--), i && ("fx" === t && n.unshift("inprogress"), delete o.stop, i.call(e, function() {
-                k.dequeue(e, t)
+                S.dequeue(e, t)
             }, o)), !r && o && o.empty.fire()
         },
         _queueHooks: function(e, t) {
             var n = t + "queueHooks";
-            return Q.get(e, n) || Q.access(e, n, {
-                empty: k.Callbacks("once memory").add(function() {
-                    Q.remove(e, [t + "queue", n])
+            return Y.get(e, n) || Y.access(e, n, {
+                empty: S.Callbacks("once memory").add(function() {
+                    Y.remove(e, [t + "queue", n])
                 })
             })
         }
-    }), k.fn.extend({
+    }), S.fn.extend({
         queue: function(t, n) {
             var e = 2;
-            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? k.queue(this[0], t) : void 0 === n ? this : this.each(function() {
-                var e = k.queue(this, t, n);
-                k._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && k.dequeue(this, t)
+            return "string" != typeof t && (n = t, t = "fx", e--), arguments.length < e ? S.queue(this[0], t) : void 0 === n ? this : this.each(function() {
+                var e = S.queue(this, t, n);
+                S._queueHooks(this, t), "fx" === t && "inprogress" !== e[0] && S.dequeue(this, t)
             })
         },
         dequeue: function(e) {
             return this.each(function() {
-                k.dequeue(this, e)
+                S.dequeue(this, e)
             })
         },
         clearQueue: function(e) {
             return this.queue(e || "fx", [])
         },
         promise: function(e, t) {
             var n, r = 1,
-                i = k.Deferred(),
+                i = S.Deferred(),
                 o = this,
                 a = this.length,
                 s = function() {
                     --r || i.resolveWith(o, [o])
                 };
             "string" != typeof e && (t = e, e = void 0), e = e || "fx";
-            while (a--)(n = Q.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
+            while (a--)(n = Y.get(o[a], e + "queueHooks")) && n.empty && (r++, n.empty.add(s));
             return s(), i.promise(t)
         }
     });
-    var te = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-        ne = new RegExp("^(?:([+-])=|)(" + te + ")([a-z%]*)$", "i"),
-        re = ["Top", "Right", "Bottom", "Left"],
-        ie = E.documentElement,
-        oe = function(e) {
-            return k.contains(e.ownerDocument, e)
+    var ee = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+        te = new RegExp("^(?:([+-])=|)(" + ee + ")([a-z%]*)$", "i"),
+        ne = ["Top", "Right", "Bottom", "Left"],
+        re = E.documentElement,
+        ie = function(e) {
+            return S.contains(e.ownerDocument, e)
         },
-        ae = {
+        oe = {
             composed: !0
         };
-    ie.getRootNode && (oe = function(e) {
-        return k.contains(e.ownerDocument, e) || e.getRootNode(ae) === e.ownerDocument
+    re.getRootNode && (ie = function(e) {
+        return S.contains(e.ownerDocument, e) || e.getRootNode(oe) === e.ownerDocument
     });
-    var se = function(e, t) {
-            return "none" === (e = t || e).style.display || "" === e.style.display && oe(e) && "none" === k.css(e, "display")
-        },
-        ue = function(e, t, n, r) {
-            var i, o, a = {};
-            for (o in t) a[o] = e.style[o], e.style[o] = t[o];
-            for (o in i = n.apply(e, r || []), t) e.style[o] = a[o];
-            return i
-        };
+    var ae = function(e, t) {
+        return "none" === (e = t || e).style.display || "" === e.style.display && ie(e) && "none" === S.css(e, "display")
+    };
 
-    function le(e, t, n, r) {
+    function se(e, t, n, r) {
         var i, o, a = 20,
             s = r ? function() {
                 return r.cur()
             } : function() {
-                return k.css(e, t, "")
+                return S.css(e, t, "")
             },
             u = s(),
-            l = n && n[3] || (k.cssNumber[t] ? "" : "px"),
-            c = e.nodeType && (k.cssNumber[t] || "px" !== l && +u) && ne.exec(k.css(e, t));
+            l = n && n[3] || (S.cssNumber[t] ? "" : "px"),
+            c = e.nodeType && (S.cssNumber[t] || "px" !== l && +u) && te.exec(S.css(e, t));
         if (c && c[3] !== l) {
             u /= 2, l = l || c[3], c = +u || 1;
-            while (a--) k.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
-            c *= 2, k.style(e, t, c + l), n = n || []
+            while (a--) S.style(e, t, c + l), (1 - o) * (1 - (o = s() / u || .5)) <= 0 && (a = 0), c /= o;
+            c *= 2, S.style(e, t, c + l), n = n || []
         }
         return n && (c = +c || +u || 0, i = n[1] ? c + (n[1] + 1) * n[2] : +n[2], r && (r.unit = l, r.start = c, r.end = i)), i
     }
-    var ce = {};
+    var ue = {};
 
-    function fe(e, t) {
-        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = Q.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && se(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ce[s]) || (o = a.body.appendChild(a.createElement(s)), u = k.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ce[s] = u)))) : "none" !== n && (l[c] = "none", Q.set(r, "display", n)));
+    function le(e, t) {
+        for (var n, r, i, o, a, s, u, l = [], c = 0, f = e.length; c < f; c++)(r = e[c]).style && (n = r.style.display, t ? ("none" === n && (l[c] = Y.get(r, "display") || null, l[c] || (r.style.display = "")), "" === r.style.display && ae(r) && (l[c] = (u = a = o = void 0, a = (i = r).ownerDocument, s = i.nodeName, (u = ue[s]) || (o = a.body.appendChild(a.createElement(s)), u = S.css(o, "display"), o.parentNode.removeChild(o), "none" === u && (u = "block"), ue[s] = u)))) : "none" !== n && (l[c] = "none", Y.set(r, "display", n)));
         for (c = 0; c < f; c++) null != l[c] && (e[c].style.display = l[c]);
         return e
     }
-    k.fn.extend({
+    S.fn.extend({
         show: function() {
-            return fe(this, !0)
+            return le(this, !0)
         },
         hide: function() {
-            return fe(this)
+            return le(this)
         },
         toggle: function(e) {
             return "boolean" == typeof e ? e ? this.show() : this.hide() : this.each(function() {
-                se(this) ? k(this).show() : k(this).hide()
+                ae(this) ? S(this).show() : S(this).hide()
             })
         }
     });
-    var pe = /^(?:checkbox|radio)$/i,
+    var ce, fe, pe = /^(?:checkbox|radio)$/i,
         de = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
-        he = /^$|^module$|\/(?:java|ecma)script/i,
-        ge = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            thead: [1, "<table>", "</table>"],
-            col: [2, "<table><colgroup>", "</colgroup></table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-            _default: [0, "", ""]
-        };
+        he = /^$|^module$|\/(?:java|ecma)script/i;
+    ce = E.createDocumentFragment().appendChild(E.createElement("div")), (fe = E.createElement("input")).setAttribute("type", "radio"), fe.setAttribute("checked", "checked"), fe.setAttribute("name", "t"), ce.appendChild(fe), y.checkClone = ce.cloneNode(!0).cloneNode(!0).lastChild.checked, ce.innerHTML = "<textarea>x</textarea>", y.noCloneChecked = !!ce.cloneNode(!0).lastChild.defaultValue, ce.innerHTML = "<option></option>", y.option = !!ce.lastChild;
+    var ge = {
+        thead: [1, "<table>", "</table>"],
+        col: [2, "<table><colgroup>", "</colgroup></table>"],
+        tr: [2, "<table><tbody>", "</tbody></table>"],
+        td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+        _default: [0, "", ""]
+    };
 
     function ve(e, t) {
         var n;
-        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && A(e, t) ? k.merge([e], n) : n
+        return n = "undefined" != typeof e.getElementsByTagName ? e.getElementsByTagName(t || "*") : "undefined" != typeof e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && A(e, t) ? S.merge([e], n) : n
     }
 
     function ye(e, t) {
-        for (var n = 0, r = e.length; n < r; n++) Q.set(e[n], "globalEval", !t || Q.get(t[n], "globalEval"))
+        for (var n = 0, r = e.length; n < r; n++) Y.set(e[n], "globalEval", !t || Y.get(t[n], "globalEval"))
     }
-    ge.optgroup = ge.option, ge.tbody = ge.tfoot = ge.colgroup = ge.caption = ge.thead, ge.th = ge.td;
-    var me, xe, be = /<|&#?\w+;/;
+    ge.tbody = ge.tfoot = ge.colgroup = ge.caption = ge.thead, ge.th = ge.td, y.option || (ge.optgroup = ge.option = [1, "<select multiple='multiple'>", "</select>"]);
+    var me = /<|&#?\w+;/;
 
-    function we(e, t, n, r, i) {
+    function xe(e, t, n, r, i) {
         for (var o, a, s, u, l, c, f = t.createDocumentFragment(), p = [], d = 0, h = e.length; d < h; d++)
             if ((o = e[d]) || 0 === o)
-                if ("object" === w(o)) k.merge(p, o.nodeType ? [o] : o);
-                else if (be.test(o)) {
-            a = a || f.appendChild(t.createElement("div")), s = (de.exec(o) || ["", ""])[1].toLowerCase(), u = ge[s] || ge._default, a.innerHTML = u[1] + k.htmlPrefilter(o) + u[2], c = u[0];
+                if ("object" === w(o)) S.merge(p, o.nodeType ? [o] : o);
+                else if (me.test(o)) {
+            a = a || f.appendChild(t.createElement("div")), s = (de.exec(o) || ["", ""])[1].toLowerCase(), u = ge[s] || ge._default, a.innerHTML = u[1] + S.htmlPrefilter(o) + u[2], c = u[0];
             while (c--) a = a.lastChild;
-            k.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
+            S.merge(p, a.childNodes), (a = f.firstChild).textContent = ""
         } else p.push(t.createTextNode(o));
         f.textContent = "", d = 0;
         while (o = p[d++])
-            if (r && -1 < k.inArray(o, r)) i && i.push(o);
-            else if (l = oe(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
+            if (r && -1 < S.inArray(o, r)) i && i.push(o);
+            else if (l = ie(o), a = ve(f.appendChild(o), "script"), l && ye(a), n) {
             c = 0;
             while (o = a[c++]) he.test(o.type || "") && n.push(o)
         }
         return f
     }
-    me = E.createDocumentFragment().appendChild(E.createElement("div")), (xe = E.createElement("input")).setAttribute("type", "radio"), xe.setAttribute("checked", "checked"), xe.setAttribute("name", "t"), me.appendChild(xe), y.checkClone = me.cloneNode(!0).cloneNode(!0).lastChild.checked, me.innerHTML = "<textarea>x</textarea>", y.noCloneChecked = !!me.cloneNode(!0).lastChild.defaultValue;
-    var Te = /^key/,
-        Ce = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
-        Ee = /^([^.]*)(?:\.(.+)|)/;
+    var be = /^key/,
+        we = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
+        Te = /^([^.]*)(?:\.(.+)|)/;
 
-    function ke() {
+    function Ce() {
         return !0
     }
 
-    function Se() {
+    function Ee() {
         return !1
     }
 
-    function Ne(e, t) {
+    function Se(e, t) {
         return e === function() {
             try {
                 return E.activeElement
             } catch (e) {}
         }() == ("focus" === t)
     }
 
-    function Ae(e, t, n, r, i, o) {
+    function ke(e, t, n, r, i, o) {
         var a, s;
         if ("object" == typeof t) {
-            for (s in "string" != typeof n && (r = r || n, n = void 0), t) Ae(e, s, n, r, t[s], o);
+            for (s in "string" != typeof n && (r = r || n, n = void 0), t) ke(e, s, n, r, t[s], o);
             return e
         }
-        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Se;
+        if (null == r && null == i ? (i = n, r = n = void 0) : null == i && ("string" == typeof n ? (i = r, r = void 0) : (i = r, r = n, n = void 0)), !1 === i) i = Ee;
         else if (!i) return e;
         return 1 === o && (a = i, (i = function(e) {
-            return k().off(e), a.apply(this, arguments)
-        }).guid = a.guid || (a.guid = k.guid++)), e.each(function() {
-            k.event.add(this, t, i, r, n)
+            return S().off(e), a.apply(this, arguments)
+        }).guid = a.guid || (a.guid = S.guid++)), e.each(function() {
+            S.event.add(this, t, i, r, n)
         })
     }
 
-    function De(e, i, o) {
-        o ? (Q.set(e, i, !1), k.event.add(e, i, {
+    function Ae(e, i, o) {
+        o ? (Y.set(e, i, !1), S.event.add(e, i, {
             namespace: !1,
             handler: function(e) {
-                var t, n, r = Q.get(this, i);
+                var t, n, r = Y.get(this, i);
                 if (1 & e.isTrigger && this[i]) {
-                    if (r.length)(k.event.special[i] || {}).delegateType && e.stopPropagation();
-                    else if (r = s.call(arguments), Q.set(this, i, r), t = o(this, i), this[i](), r !== (n = Q.get(this, i)) || t ? Q.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
-                } else r.length && (Q.set(this, i, {
-                    value: k.event.trigger(k.extend(r[0], k.Event.prototype), r.slice(1), this)
+                    if (r.length)(S.event.special[i] || {}).delegateType && e.stopPropagation();
+                    else if (r = s.call(arguments), Y.set(this, i, r), t = o(this, i), this[i](), r !== (n = Y.get(this, i)) || t ? Y.set(this, i, !1) : n = {}, r !== n) return e.stopImmediatePropagation(), e.preventDefault(), n.value
+                } else r.length && (Y.set(this, i, {
+                    value: S.event.trigger(S.extend(r[0], S.Event.prototype), r.slice(1), this)
                 }), e.stopImmediatePropagation())
             }
-        })) : void 0 === Q.get(e, i) && k.event.add(e, i, ke)
+        })) : void 0 === Y.get(e, i) && S.event.add(e, i, Ce)
     }
-    k.event = {
+    S.event = {
         global: {},
         add: function(t, e, n, r, i) {
-            var o, a, s, u, l, c, f, p, d, h, g, v = Q.get(t);
-            if (v) {
-                n.handler && (n = (o = n).handler, i = o.selector), i && k.find.matchesSelector(ie, i), n.guid || (n.guid = k.guid++), (u = v.events) || (u = v.events = {}), (a = v.handle) || (a = v.handle = function(e) {
-                    return "undefined" != typeof k && k.event.triggered !== e.type ? k.event.dispatch.apply(t, arguments) : void 0
-                }), l = (e = (e || "").match(R) || [""]).length;
-                while (l--) d = g = (s = Ee.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = k.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = k.event.special[d] || {}, c = k.extend({
+            var o, a, s, u, l, c, f, p, d, h, g, v = Y.get(t);
+            if (V(t)) {
+                n.handler && (n = (o = n).handler, i = o.selector), i && S.find.matchesSelector(re, i), n.guid || (n.guid = S.guid++), (u = v.events) || (u = v.events = Object.create(null)), (a = v.handle) || (a = v.handle = function(e) {
+                    return "undefined" != typeof S && S.event.triggered !== e.type ? S.event.dispatch.apply(t, arguments) : void 0
+                }), l = (e = (e || "").match(P) || [""]).length;
+                while (l--) d = g = (s = Te.exec(e[l]) || [])[1], h = (s[2] || "").split(".").sort(), d && (f = S.event.special[d] || {}, d = (i ? f.delegateType : f.bindType) || d, f = S.event.special[d] || {}, c = S.extend({
                     type: d,
                     origType: g,
                     data: r,
                     handler: n,
                     guid: n.guid,
                     selector: i,
-                    needsContext: i && k.expr.match.needsContext.test(i),
+                    needsContext: i && S.expr.match.needsContext.test(i),
                     namespace: h.join(".")
-                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), k.event.global[d] = !0)
+                }, o), (p = u[d]) || ((p = u[d] = []).delegateCount = 0, f.setup && !1 !== f.setup.call(t, r, h, a) || t.addEventListener && t.addEventListener(d, a)), f.add && (f.add.call(t, c), c.handler.guid || (c.handler.guid = n.guid)), i ? p.splice(p.delegateCount++, 0, c) : p.push(c), S.event.global[d] = !0)
             }
         },
         remove: function(e, t, n, r, i) {
-            var o, a, s, u, l, c, f, p, d, h, g, v = Q.hasData(e) && Q.get(e);
+            var o, a, s, u, l, c, f, p, d, h, g, v = Y.hasData(e) && Y.get(e);
             if (v && (u = v.events)) {
-                l = (t = (t || "").match(R) || [""]).length;
+                l = (t = (t || "").match(P) || [""]).length;
                 while (l--)
-                    if (d = g = (s = Ee.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
-                        f = k.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
+                    if (d = g = (s = Te.exec(t[l]) || [])[1], h = (s[2] || "").split(".").sort(), d) {
+                        f = S.event.special[d] || {}, p = u[d = (r ? f.delegateType : f.bindType) || d] || [], s = s[2] && new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)"), a = o = p.length;
                         while (o--) c = p[o], !i && g !== c.origType || n && n.guid !== c.guid || s && !s.test(c.namespace) || r && r !== c.selector && ("**" !== r || !c.selector) || (p.splice(o, 1), c.selector && p.delegateCount--, f.remove && f.remove.call(e, c));
-                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || k.removeEvent(e, d, v.handle), delete u[d])
+                        a && !p.length && (f.teardown && !1 !== f.teardown.call(e, h, v.handle) || S.removeEvent(e, d, v.handle), delete u[d])
                     } else
-                        for (d in u) k.event.remove(e, d + t[l], n, r, !0);
-                k.isEmptyObject(u) && Q.remove(e, "handle events")
+                        for (d in u) S.event.remove(e, d + t[l], n, r, !0);
+                S.isEmptyObject(u) && Y.remove(e, "handle events")
             }
         },
         dispatch: function(e) {
-            var t, n, r, i, o, a, s = k.event.fix(e),
-                u = new Array(arguments.length),
-                l = (Q.get(this, "events") || {})[s.type] || [],
-                c = k.event.special[s.type] || {};
-            for (u[0] = s, t = 1; t < arguments.length; t++) u[t] = arguments[t];
-            if (s.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, s)) {
-                a = k.event.handlers.call(this, s, l), t = 0;
-                while ((i = a[t++]) && !s.isPropagationStopped()) {
-                    s.currentTarget = i.elem, n = 0;
-                    while ((o = i.handlers[n++]) && !s.isImmediatePropagationStopped()) s.rnamespace && !1 !== o.namespace && !s.rnamespace.test(o.namespace) || (s.handleObj = o, s.data = o.data, void 0 !== (r = ((k.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, u)) && !1 === (s.result = r) && (s.preventDefault(), s.stopPropagation()))
+            var t, n, r, i, o, a, s = new Array(arguments.length),
+                u = S.event.fix(e),
+                l = (Y.get(this, "events") || Object.create(null))[u.type] || [],
+                c = S.event.special[u.type] || {};
+            for (s[0] = u, t = 1; t < arguments.length; t++) s[t] = arguments[t];
+            if (u.delegateTarget = this, !c.preDispatch || !1 !== c.preDispatch.call(this, u)) {
+                a = S.event.handlers.call(this, u, l), t = 0;
+                while ((i = a[t++]) && !u.isPropagationStopped()) {
+                    u.currentTarget = i.elem, n = 0;
+                    while ((o = i.handlers[n++]) && !u.isImmediatePropagationStopped()) u.rnamespace && !1 !== o.namespace && !u.rnamespace.test(o.namespace) || (u.handleObj = o, u.data = o.data, void 0 !== (r = ((S.event.special[o.origType] || {}).handle || o.handler).apply(i.elem, s)) && !1 === (u.result = r) && (u.preventDefault(), u.stopPropagation()))
                 }
-                return c.postDispatch && c.postDispatch.call(this, s), s.result
+                return c.postDispatch && c.postDispatch.call(this, u), u.result
             }
         },
         handlers: function(e, t) {
             var n, r, i, o, a, s = [],
                 u = t.delegateCount,
                 l = e.target;
             if (u && l.nodeType && !("click" === e.type && 1 <= e.button))
                 for (; l !== this; l = l.parentNode || this)
                     if (1 === l.nodeType && ("click" !== e.type || !0 !== l.disabled)) {
-                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < k(i, this).index(l) : k.find(i, this, null, [l]).length), a[i] && o.push(r);
+                        for (o = [], a = {}, n = 0; n < u; n++) void 0 === a[i = (r = t[n]).selector + " "] && (a[i] = r.needsContext ? -1 < S(i, this).index(l) : S.find(i, this, null, [l]).length), a[i] && o.push(r);
                         o.length && s.push({
                             elem: l,
                             handlers: o
                         })
                     } return l = this, u < t.length && s.push({
                 elem: l,
                 handlers: t.slice(u)
             }), s
         },
         addProp: function(t, e) {
-            Object.defineProperty(k.Event.prototype, t, {
+            Object.defineProperty(S.Event.prototype, t, {
                 enumerable: !0,
                 configurable: !0,
                 get: m(e) ? function() {
                     if (this.originalEvent) return e(this.originalEvent)
                 } : function() {
                     if (this.originalEvent) return this.originalEvent[t]
                 },
@@ -1643,64 +1649,64 @@
                         writable: !0,
                         value: e
                     })
                 }
             })
         },
         fix: function(e) {
-            return e[k.expando] ? e : new k.Event(e)
+            return e[S.expando] ? e : new S.Event(e)
         },
         special: {
             load: {
                 noBubble: !0
             },
             click: {
                 setup: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && De(t, "click", ke), !1
+                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click", Ce), !1
                 },
                 trigger: function(e) {
                     var t = this || e;
-                    return pe.test(t.type) && t.click && A(t, "input") && De(t, "click"), !0
+                    return pe.test(t.type) && t.click && A(t, "input") && Ae(t, "click"), !0
                 },
                 _default: function(e) {
                     var t = e.target;
-                    return pe.test(t.type) && t.click && A(t, "input") && Q.get(t, "click") || A(t, "a")
+                    return pe.test(t.type) && t.click && A(t, "input") && Y.get(t, "click") || A(t, "a")
                 }
             },
             beforeunload: {
                 postDispatch: function(e) {
                     void 0 !== e.result && e.originalEvent && (e.originalEvent.returnValue = e.result)
                 }
             }
         }
-    }, k.removeEvent = function(e, t, n) {
+    }, S.removeEvent = function(e, t, n) {
         e.removeEventListener && e.removeEventListener(t, n)
-    }, k.Event = function(e, t) {
-        if (!(this instanceof k.Event)) return new k.Event(e, t);
-        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? ke : Se, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && k.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[k.expando] = !0
-    }, k.Event.prototype = {
-        constructor: k.Event,
-        isDefaultPrevented: Se,
-        isPropagationStopped: Se,
-        isImmediatePropagationStopped: Se,
+    }, S.Event = function(e, t) {
+        if (!(this instanceof S.Event)) return new S.Event(e, t);
+        e && e.type ? (this.originalEvent = e, this.type = e.type, this.isDefaultPrevented = e.defaultPrevented || void 0 === e.defaultPrevented && !1 === e.returnValue ? Ce : Ee, this.target = e.target && 3 === e.target.nodeType ? e.target.parentNode : e.target, this.currentTarget = e.currentTarget, this.relatedTarget = e.relatedTarget) : this.type = e, t && S.extend(this, t), this.timeStamp = e && e.timeStamp || Date.now(), this[S.expando] = !0
+    }, S.Event.prototype = {
+        constructor: S.Event,
+        isDefaultPrevented: Ee,
+        isPropagationStopped: Ee,
+        isImmediatePropagationStopped: Ee,
         isSimulated: !1,
         preventDefault: function() {
             var e = this.originalEvent;
-            this.isDefaultPrevented = ke, e && !this.isSimulated && e.preventDefault()
+            this.isDefaultPrevented = Ce, e && !this.isSimulated && e.preventDefault()
         },
         stopPropagation: function() {
             var e = this.originalEvent;
-            this.isPropagationStopped = ke, e && !this.isSimulated && e.stopPropagation()
+            this.isPropagationStopped = Ce, e && !this.isSimulated && e.stopPropagation()
         },
         stopImmediatePropagation: function() {
             var e = this.originalEvent;
-            this.isImmediatePropagationStopped = ke, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = Ce, e && !this.isSimulated && e.stopImmediatePropagation(), this.stopPropagation()
         }
-    }, k.each({
+    }, S.each({
         altKey: !0,
         bubbles: !0,
         cancelable: !0,
         changedTouches: !0,
         ctrlKey: !0,
         detail: !0,
         eventPhase: !0,
@@ -1725,334 +1731,343 @@
         screenX: !0,
         screenY: !0,
         targetTouches: !0,
         toElement: !0,
         touches: !0,
         which: function(e) {
             var t = e.button;
-            return null == e.which && Te.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && Ce.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
+            return null == e.which && be.test(e.type) ? null != e.charCode ? e.charCode : e.keyCode : !e.which && void 0 !== t && we.test(e.type) ? 1 & t ? 1 : 2 & t ? 3 : 4 & t ? 2 : 0 : e.which
         }
-    }, k.event.addProp), k.each({
+    }, S.event.addProp), S.each({
         focus: "focusin",
         blur: "focusout"
     }, function(e, t) {
-        k.event.special[e] = {
+        S.event.special[e] = {
             setup: function() {
-                return De(this, e, Ne), !1
+                return Ae(this, e, Se), !1
             },
             trigger: function() {
-                return De(this, e), !0
+                return Ae(this, e), !0
             },
             delegateType: t
         }
-    }), k.each({
+    }), S.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
         pointerleave: "pointerout"
     }, function(e, i) {
-        k.event.special[e] = {
+        S.event.special[e] = {
             delegateType: i,
             bindType: i,
             handle: function(e) {
                 var t, n = e.relatedTarget,
                     r = e.handleObj;
-                return n && (n === this || k.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
+                return n && (n === this || S.contains(this, n)) || (e.type = r.origType, t = r.handler.apply(this, arguments), e.type = i), t
             }
         }
-    }), k.fn.extend({
+    }), S.fn.extend({
         on: function(e, t, n, r) {
-            return Ae(this, e, t, n, r)
+            return ke(this, e, t, n, r)
         },
         one: function(e, t, n, r) {
-            return Ae(this, e, t, n, r, 1)
+            return ke(this, e, t, n, r, 1)
         },
         off: function(e, t, n) {
             var r, i;
-            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, k(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
+            if (e && e.preventDefault && e.handleObj) return r = e.handleObj, S(e.delegateTarget).off(r.namespace ? r.origType + "." + r.namespace : r.origType, r.selector, r.handler), this;
             if ("object" == typeof e) {
                 for (i in e) this.off(i, t, e[i]);
                 return this
             }
-            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Se), this.each(function() {
-                k.event.remove(this, e, n, t)
+            return !1 !== t && "function" != typeof t || (n = t, t = void 0), !1 === n && (n = Ee), this.each(function() {
+                S.event.remove(this, e, n, t)
             })
         }
     });
-    var je = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([a-z][^\/\0>\x20\t\r\n\f]*)[^>]*)\/>/gi,
-        qe = /<script|<style|<link/i,
-        Le = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        He = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
+    var Ne = /<script|<style|<link/i,
+        De = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        je = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;
 
-    function Oe(e, t) {
-        return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && k(e).children("tbody")[0] || e
+    function qe(e, t) {
+        return A(e, "table") && A(11 !== t.nodeType ? t : t.firstChild, "tr") && S(e).children("tbody")[0] || e
     }
 
-    function Pe(e) {
+    function Le(e) {
         return e.type = (null !== e.getAttribute("type")) + "/" + e.type, e
     }
 
-    function Re(e) {
+    function He(e) {
         return "true/" === (e.type || "").slice(0, 5) ? e.type = e.type.slice(5) : e.removeAttribute("type"), e
     }
 
-    function Me(e, t) {
-        var n, r, i, o, a, s, u, l;
+    function Oe(e, t) {
+        var n, r, i, o, a, s;
         if (1 === t.nodeType) {
-            if (Q.hasData(e) && (o = Q.access(e), a = Q.set(t, o), l = o.events))
-                for (i in delete a.handle, a.events = {}, l)
-                    for (n = 0, r = l[i].length; n < r; n++) k.event.add(t, i, l[i][n]);
-            J.hasData(e) && (s = J.access(e), u = k.extend({}, s), J.set(t, u))
+            if (Y.hasData(e) && (s = Y.get(e).events))
+                for (i in Y.remove(t, "handle events"), s)
+                    for (n = 0, r = s[i].length; n < r; n++) S.event.add(t, i, s[i][n]);
+            Q.hasData(e) && (o = Q.access(e), a = S.extend({}, o), Q.set(t, a))
         }
     }
 
-    function Ie(n, r, i, o) {
-        r = g.apply([], r);
+    function Pe(n, r, i, o) {
+        r = g(r);
         var e, t, a, s, u, l, c = 0,
             f = n.length,
             p = f - 1,
             d = r[0],
             h = m(d);
-        if (h || 1 < f && "string" == typeof d && !y.checkClone && Le.test(d)) return n.each(function(e) {
+        if (h || 1 < f && "string" == typeof d && !y.checkClone && De.test(d)) return n.each(function(e) {
             var t = n.eq(e);
-            h && (r[0] = d.call(this, e, t.html())), Ie(t, r, i, o)
+            h && (r[0] = d.call(this, e, t.html())), Pe(t, r, i, o)
         });
-        if (f && (t = (e = we(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
-            for (s = (a = k.map(ve(e, "script"), Pe)).length; c < f; c++) u = e, c !== p && (u = k.clone(u, !0, !0), s && k.merge(a, ve(u, "script"))), i.call(n[c], u, c);
+        if (f && (t = (e = xe(r, n[0].ownerDocument, !1, n, o)).firstChild, 1 === e.childNodes.length && (e = t), t || o)) {
+            for (s = (a = S.map(ve(e, "script"), Le)).length; c < f; c++) u = e, c !== p && (u = S.clone(u, !0, !0), s && S.merge(a, ve(u, "script"))), i.call(n[c], u, c);
             if (s)
-                for (l = a[a.length - 1].ownerDocument, k.map(a, Re), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Q.access(u, "globalEval") && k.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? k._evalUrl && !u.noModule && k._evalUrl(u.src, {
+                for (l = a[a.length - 1].ownerDocument, S.map(a, He), c = 0; c < s; c++) u = a[c], he.test(u.type || "") && !Y.access(u, "globalEval") && S.contains(l, u) && (u.src && "module" !== (u.type || "").toLowerCase() ? S._evalUrl && !u.noModule && S._evalUrl(u.src, {
                     nonce: u.nonce || u.getAttribute("nonce")
-                }) : b(u.textContent.replace(He, ""), u, l))
+                }, l) : b(u.textContent.replace(je, ""), u, l))
         }
         return n
     }
 
-    function We(e, t, n) {
-        for (var r, i = t ? k.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || k.cleanData(ve(r)), r.parentNode && (n && oe(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
+    function Re(e, t, n) {
+        for (var r, i = t ? S.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || S.cleanData(ve(r)), r.parentNode && (n && ie(r) && ye(ve(r, "script")), r.parentNode.removeChild(r));
         return e
     }
-    k.extend({
+    S.extend({
         htmlPrefilter: function(e) {
-            return e.replace(je, "<$1></$2>")
+            return e
         },
         clone: function(e, t, n) {
             var r, i, o, a, s, u, l, c = e.cloneNode(!0),
-                f = oe(e);
-            if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || k.isXMLDoc(e)))
+                f = ie(e);
+            if (!(y.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || S.isXMLDoc(e)))
                 for (a = ve(c), r = 0, i = (o = ve(e)).length; r < i; r++) s = o[r], u = a[r], void 0, "input" === (l = u.nodeName.toLowerCase()) && pe.test(s.type) ? u.checked = s.checked : "input" !== l && "textarea" !== l || (u.defaultValue = s.defaultValue);
             if (t)
                 if (n)
-                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Me(o[r], a[r]);
-                else Me(e, c);
+                    for (o = o || ve(e), a = a || ve(c), r = 0, i = o.length; r < i; r++) Oe(o[r], a[r]);
+                else Oe(e, c);
             return 0 < (a = ve(c, "script")).length && ye(a, !f && ve(e, "script")), c
         },
         cleanData: function(e) {
-            for (var t, n, r, i = k.event.special, o = 0; void 0 !== (n = e[o]); o++)
-                if (G(n)) {
-                    if (t = n[Q.expando]) {
+            for (var t, n, r, i = S.event.special, o = 0; void 0 !== (n = e[o]); o++)
+                if (V(n)) {
+                    if (t = n[Y.expando]) {
                         if (t.events)
-                            for (r in t.events) i[r] ? k.event.remove(n, r) : k.removeEvent(n, r, t.handle);
-                        n[Q.expando] = void 0
+                            for (r in t.events) i[r] ? S.event.remove(n, r) : S.removeEvent(n, r, t.handle);
+                        n[Y.expando] = void 0
                     }
-                    n[J.expando] && (n[J.expando] = void 0)
+                    n[Q.expando] && (n[Q.expando] = void 0)
                 }
         }
-    }), k.fn.extend({
+    }), S.fn.extend({
         detach: function(e) {
-            return We(this, e, !0)
+            return Re(this, e, !0)
         },
         remove: function(e) {
-            return We(this, e)
+            return Re(this, e)
         },
         text: function(e) {
-            return _(this, function(e) {
-                return void 0 === e ? k.text(this) : this.empty().each(function() {
+            return $(this, function(e) {
+                return void 0 === e ? S.text(this) : this.empty().each(function() {
                     1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || (this.textContent = e)
                 })
             }, null, e, arguments.length)
         },
         append: function() {
-            return Ie(this, arguments, function(e) {
-                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || Oe(this, e).appendChild(e)
+            return Pe(this, arguments, function(e) {
+                1 !== this.nodeType && 11 !== this.nodeType && 9 !== this.nodeType || qe(this, e).appendChild(e)
             })
         },
         prepend: function() {
-            return Ie(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var t = Oe(this, e);
+                    var t = qe(this, e);
                     t.insertBefore(e, t.firstChild)
                 }
             })
         },
         before: function() {
-            return Ie(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this)
             })
         },
         after: function() {
-            return Ie(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
             })
         },
         empty: function() {
-            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (k.cleanData(ve(e, !1)), e.textContent = "");
+            for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (S.cleanData(ve(e, !1)), e.textContent = "");
             return this
         },
         clone: function(e, t) {
             return e = null != e && e, t = null == t ? e : t, this.map(function() {
-                return k.clone(this, e, t)
+                return S.clone(this, e, t)
             })
         },
         html: function(e) {
-            return _(this, function(e) {
+            return $(this, function(e) {
                 var t = this[0] || {},
                     n = 0,
                     r = this.length;
                 if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                if ("string" == typeof e && !qe.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
-                    e = k.htmlPrefilter(e);
+                if ("string" == typeof e && !Ne.test(e) && !ge[(de.exec(e) || ["", ""])[1].toLowerCase()]) {
+                    e = S.htmlPrefilter(e);
                     try {
-                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (k.cleanData(ve(t, !1)), t.innerHTML = e);
+                        for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (S.cleanData(ve(t, !1)), t.innerHTML = e);
                         t = 0
                     } catch (e) {}
                 }
                 t && this.empty().append(e)
             }, null, e, arguments.length)
         },
         replaceWith: function() {
             var n = [];
-            return Ie(this, arguments, function(e) {
+            return Pe(this, arguments, function(e) {
                 var t = this.parentNode;
-                k.inArray(this, n) < 0 && (k.cleanData(ve(this)), t && t.replaceChild(e, this))
+                S.inArray(this, n) < 0 && (S.cleanData(ve(this)), t && t.replaceChild(e, this))
             }, n)
         }
-    }), k.each({
+    }), S.each({
         appendTo: "append",
         prependTo: "prepend",
         insertBefore: "before",
         insertAfter: "after",
         replaceAll: "replaceWith"
     }, function(e, a) {
-        k.fn[e] = function(e) {
-            for (var t, n = [], r = k(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), k(r[o])[a](t), u.apply(n, t.get());
+        S.fn[e] = function(e) {
+            for (var t, n = [], r = S(e), i = r.length - 1, o = 0; o <= i; o++) t = o === i ? this : this.clone(!0), S(r[o])[a](t), u.apply(n, t.get());
             return this.pushStack(n)
         }
     });
-    var $e = new RegExp("^(" + te + ")(?!px)[a-z%]+$", "i"),
-        Fe = function(e) {
+    var Me = new RegExp("^(" + ee + ")(?!px)[a-z%]+$", "i"),
+        Ie = function(e) {
             var t = e.ownerDocument.defaultView;
             return t && t.opener || (t = C), t.getComputedStyle(e)
         },
-        Be = new RegExp(re.join("|"), "i");
+        We = function(e, t, n) {
+            var r, i, o = {};
+            for (i in t) o[i] = e.style[i], e.style[i] = t[i];
+            for (i in r = n.call(e), t) e.style[i] = o[i];
+            return r
+        },
+        Fe = new RegExp(ne.join("|"), "i");
 
-    function _e(e, t, n) {
+    function Be(e, t, n) {
         var r, i, o, a, s = e.style;
-        return (n = n || Fe(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || oe(e) || (a = k.style(e, t)), !y.pixelBoxStyles() && $e.test(a) && Be.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
+        return (n = n || Ie(e)) && ("" !== (a = n.getPropertyValue(t) || n[t]) || ie(e) || (a = S.style(e, t)), !y.pixelBoxStyles() && Me.test(a) && Fe.test(t) && (r = s.width, i = s.minWidth, o = s.maxWidth, s.minWidth = s.maxWidth = s.width = a, a = n.width, s.width = r, s.minWidth = i, s.maxWidth = o)), void 0 !== a ? a + "" : a
     }
 
-    function ze(e, t) {
+    function $e(e, t) {
         return {
             get: function() {
                 if (!e()) return (this.get = t).apply(this, arguments);
                 delete this.get
             }
         }
     }! function() {
         function e() {
-            if (u) {
-                s.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", u.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", ie.appendChild(s).appendChild(u);
-                var e = C.getComputedStyle(u);
-                n = "1%" !== e.top, a = 12 === t(e.marginLeft), u.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), u.style.position = "absolute", i = 12 === t(u.offsetWidth / 3), ie.removeChild(s), u = null
+            if (l) {
+                u.style.cssText = "position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0", l.style.cssText = "position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%", re.appendChild(u).appendChild(l);
+                var e = C.getComputedStyle(l);
+                n = "1%" !== e.top, s = 12 === t(e.marginLeft), l.style.right = "60%", o = 36 === t(e.right), r = 36 === t(e.width), l.style.position = "absolute", i = 12 === t(l.offsetWidth / 3), re.removeChild(u), l = null
             }
         }
 
         function t(e) {
             return Math.round(parseFloat(e))
         }
-        var n, r, i, o, a, s = E.createElement("div"),
-            u = E.createElement("div");
-        u.style && (u.style.backgroundClip = "content-box", u.cloneNode(!0).style.backgroundClip = "", y.clearCloneStyle = "content-box" === u.style.backgroundClip, k.extend(y, {
+        var n, r, i, o, a, s, u = E.createElement("div"),
+            l = E.createElement("div");
+        l.style && (l.style.backgroundClip = "content-box", l.cloneNode(!0).style.backgroundClip = "", y.clearCloneStyle = "content-box" === l.style.backgroundClip, S.extend(y, {
             boxSizingReliable: function() {
                 return e(), r
             },
             pixelBoxStyles: function() {
                 return e(), o
             },
             pixelPosition: function() {
                 return e(), n
             },
             reliableMarginLeft: function() {
-                return e(), a
+                return e(), s
             },
             scrollboxSize: function() {
                 return e(), i
+            },
+            reliableTrDimensions: function() {
+                var e, t, n, r;
+                return null == a && (e = E.createElement("table"), t = E.createElement("tr"), n = E.createElement("div"), e.style.cssText = "position:absolute;left:-11111px", t.style.height = "1px", n.style.height = "9px", re.appendChild(e).appendChild(t).appendChild(n), r = C.getComputedStyle(t), a = 3 < parseInt(r.height), re.removeChild(e)), a
             }
         }))
     }();
-    var Ue = ["Webkit", "Moz", "ms"],
-        Xe = E.createElement("div").style,
-        Ve = {};
-
-    function Ge(e) {
-        var t = k.cssProps[e] || Ve[e];
-        return t || (e in Xe ? e : Ve[e] = function(e) {
+    var _e = ["Webkit", "Moz", "ms"],
+        ze = E.createElement("div").style,
+        Ue = {};
+
+    function Xe(e) {
+        var t = S.cssProps[e] || Ue[e];
+        return t || (e in ze ? e : Ue[e] = function(e) {
             var t = e[0].toUpperCase() + e.slice(1),
-                n = Ue.length;
+                n = _e.length;
             while (n--)
-                if ((e = Ue[n] + t) in Xe) return e
+                if ((e = _e[n] + t) in ze) return e
         }(e) || e)
     }
-    var Ye = /^(none|table(?!-c[ea]).+)/,
-        Qe = /^--/,
-        Je = {
+    var Ve = /^(none|table(?!-c[ea]).+)/,
+        Ge = /^--/,
+        Ye = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Ke = {
+        Qe = {
             letterSpacing: "0",
             fontWeight: "400"
         };
 
-    function Ze(e, t, n) {
-        var r = ne.exec(t);
+    function Je(e, t, n) {
+        var r = te.exec(t);
         return r ? Math.max(0, r[2] - (n || 0)) + (r[3] || "px") : t
     }
 
-    function et(e, t, n, r, i, o) {
+    function Ke(e, t, n, r, i, o) {
         var a = "width" === t ? 1 : 0,
             s = 0,
             u = 0;
         if (n === (r ? "border" : "content")) return 0;
-        for (; a < 4; a += 2) "margin" === n && (u += k.css(e, n + re[a], !0, i)), r ? ("content" === n && (u -= k.css(e, "padding" + re[a], !0, i)), "margin" !== n && (u -= k.css(e, "border" + re[a] + "Width", !0, i))) : (u += k.css(e, "padding" + re[a], !0, i), "padding" !== n ? u += k.css(e, "border" + re[a] + "Width", !0, i) : s += k.css(e, "border" + re[a] + "Width", !0, i));
+        for (; a < 4; a += 2) "margin" === n && (u += S.css(e, n + ne[a], !0, i)), r ? ("content" === n && (u -= S.css(e, "padding" + ne[a], !0, i)), "margin" !== n && (u -= S.css(e, "border" + ne[a] + "Width", !0, i))) : (u += S.css(e, "padding" + ne[a], !0, i), "padding" !== n ? u += S.css(e, "border" + ne[a] + "Width", !0, i) : s += S.css(e, "border" + ne[a] + "Width", !0, i));
         return !r && 0 <= o && (u += Math.max(0, Math.ceil(e["offset" + t[0].toUpperCase() + t.slice(1)] - o - u - s - .5)) || 0), u
     }
 
-    function tt(e, t, n) {
-        var r = Fe(e),
-            i = (!y.boxSizingReliable() || n) && "border-box" === k.css(e, "boxSizing", !1, r),
+    function Ze(e, t, n) {
+        var r = Ie(e),
+            i = (!y.boxSizingReliable() || n) && "border-box" === S.css(e, "boxSizing", !1, r),
             o = i,
-            a = _e(e, t, r),
+            a = Be(e, t, r),
             s = "offset" + t[0].toUpperCase() + t.slice(1);
-        if ($e.test(a)) {
+        if (Me.test(a)) {
             if (!n) return a;
             a = "auto"
         }
-        return (!y.boxSizingReliable() && i || "auto" === a || !parseFloat(a) && "inline" === k.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === k.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + et(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
+        return (!y.boxSizingReliable() && i || !y.reliableTrDimensions() && A(e, "tr") || "auto" === a || !parseFloat(a) && "inline" === S.css(e, "display", !1, r)) && e.getClientRects().length && (i = "border-box" === S.css(e, "boxSizing", !1, r), (o = s in e) && (a = e[s])), (a = parseFloat(a) || 0) + Ke(e, t, n || (i ? "border" : "content"), o, r, a) + "px"
     }
 
-    function nt(e, t, n, r, i) {
-        return new nt.prototype.init(e, t, n, r, i)
+    function et(e, t, n, r, i) {
+        return new et.prototype.init(e, t, n, r, i)
     }
-    k.extend({
+    S.extend({
         cssHooks: {
             opacity: {
                 get: function(e, t) {
                     if (t) {
-                        var n = _e(e, "opacity");
+                        var n = Be(e, "opacity");
                         return "" === n ? "1" : n
                     }
                 }
             }
         },
         cssNumber: {
             animationIterationCount: !0,
@@ -2075,693 +2090,695 @@
             widows: !0,
             zIndex: !0,
             zoom: !0
         },
         cssProps: {},
         style: function(e, t, n, r) {
             if (e && 3 !== e.nodeType && 8 !== e.nodeType && e.style) {
-                var i, o, a, s = V(t),
-                    u = Qe.test(t),
+                var i, o, a, s = X(t),
+                    u = Ge.test(t),
                     l = e.style;
-                if (u || (t = Ge(s)), a = k.cssHooks[t] || k.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
-                "string" === (o = typeof n) && (i = ne.exec(n)) && i[1] && (n = le(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (k.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
+                if (u || (t = Xe(s)), a = S.cssHooks[t] || S.cssHooks[s], void 0 === n) return a && "get" in a && void 0 !== (i = a.get(e, !1, r)) ? i : l[t];
+                "string" === (o = typeof n) && (i = te.exec(n)) && i[1] && (n = se(e, t, i), o = "number"), null != n && n == n && ("number" !== o || u || (n += i && i[3] || (S.cssNumber[s] ? "" : "px")), y.clearCloneStyle || "" !== n || 0 !== t.indexOf("background") || (l[t] = "inherit"), a && "set" in a && void 0 === (n = a.set(e, n, r)) || (u ? l.setProperty(t, n) : l[t] = n))
             }
         },
         css: function(e, t, n, r) {
-            var i, o, a, s = V(t);
-            return Qe.test(t) || (t = Ge(s)), (a = k.cssHooks[t] || k.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = _e(e, t, r)), "normal" === i && t in Ke && (i = Ke[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
+            var i, o, a, s = X(t);
+            return Ge.test(t) || (t = Xe(s)), (a = S.cssHooks[t] || S.cssHooks[s]) && "get" in a && (i = a.get(e, !0, n)), void 0 === i && (i = Be(e, t, r)), "normal" === i && t in Qe && (i = Qe[t]), "" === n || n ? (o = parseFloat(i), !0 === n || isFinite(o) ? o || 0 : i) : i
         }
-    }), k.each(["height", "width"], function(e, u) {
-        k.cssHooks[u] = {
+    }), S.each(["height", "width"], function(e, u) {
+        S.cssHooks[u] = {
             get: function(e, t, n) {
-                if (t) return !Ye.test(k.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? tt(e, u, n) : ue(e, Je, function() {
-                    return tt(e, u, n)
+                if (t) return !Ve.test(S.css(e, "display")) || e.getClientRects().length && e.getBoundingClientRect().width ? Ze(e, u, n) : We(e, Ye, function() {
+                    return Ze(e, u, n)
                 })
             },
             set: function(e, t, n) {
-                var r, i = Fe(e),
+                var r, i = Ie(e),
                     o = !y.scrollboxSize() && "absolute" === i.position,
-                    a = (o || n) && "border-box" === k.css(e, "boxSizing", !1, i),
-                    s = n ? et(e, u, n, a, i) : 0;
-                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - et(e, u, "border", !1, i) - .5)), s && (r = ne.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = k.css(e, u)), Ze(0, t, s)
+                    a = (o || n) && "border-box" === S.css(e, "boxSizing", !1, i),
+                    s = n ? Ke(e, u, n, a, i) : 0;
+                return a && o && (s -= Math.ceil(e["offset" + u[0].toUpperCase() + u.slice(1)] - parseFloat(i[u]) - Ke(e, u, "border", !1, i) - .5)), s && (r = te.exec(t)) && "px" !== (r[3] || "px") && (e.style[u] = t, t = S.css(e, u)), Je(0, t, s)
             }
         }
-    }), k.cssHooks.marginLeft = ze(y.reliableMarginLeft, function(e, t) {
-        if (t) return (parseFloat(_e(e, "marginLeft")) || e.getBoundingClientRect().left - ue(e, {
+    }), S.cssHooks.marginLeft = $e(y.reliableMarginLeft, function(e, t) {
+        if (t) return (parseFloat(Be(e, "marginLeft")) || e.getBoundingClientRect().left - We(e, {
             marginLeft: 0
         }, function() {
             return e.getBoundingClientRect().left
         })) + "px"
-    }), k.each({
+    }), S.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(i, o) {
-        k.cssHooks[i + o] = {
+        S.cssHooks[i + o] = {
             expand: function(e) {
-                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + re[t] + o] = r[t] || r[t - 2] || r[0];
+                for (var t = 0, n = {}, r = "string" == typeof e ? e.split(" ") : [e]; t < 4; t++) n[i + ne[t] + o] = r[t] || r[t - 2] || r[0];
                 return n
             }
-        }, "margin" !== i && (k.cssHooks[i + o].set = Ze)
-    }), k.fn.extend({
+        }, "margin" !== i && (S.cssHooks[i + o].set = Je)
+    }), S.fn.extend({
         css: function(e, t) {
-            return _(this, function(e, t, n) {
+            return $(this, function(e, t, n) {
                 var r, i, o = {},
                     a = 0;
                 if (Array.isArray(t)) {
-                    for (r = Fe(e), i = t.length; a < i; a++) o[t[a]] = k.css(e, t[a], !1, r);
+                    for (r = Ie(e), i = t.length; a < i; a++) o[t[a]] = S.css(e, t[a], !1, r);
                     return o
                 }
-                return void 0 !== n ? k.style(e, t, n) : k.css(e, t)
+                return void 0 !== n ? S.style(e, t, n) : S.css(e, t)
             }, e, t, 1 < arguments.length)
         }
-    }), ((k.Tween = nt).prototype = {
-        constructor: nt,
+    }), ((S.Tween = et).prototype = {
+        constructor: et,
         init: function(e, t, n, r, i, o) {
-            this.elem = e, this.prop = n, this.easing = i || k.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (k.cssNumber[n] ? "" : "px")
+            this.elem = e, this.prop = n, this.easing = i || S.easing._default, this.options = t, this.start = this.now = this.cur(), this.end = r, this.unit = o || (S.cssNumber[n] ? "" : "px")
         },
         cur: function() {
-            var e = nt.propHooks[this.prop];
-            return e && e.get ? e.get(this) : nt.propHooks._default.get(this)
+            var e = et.propHooks[this.prop];
+            return e && e.get ? e.get(this) : et.propHooks._default.get(this)
         },
         run: function(e) {
-            var t, n = nt.propHooks[this.prop];
-            return this.options.duration ? this.pos = t = k.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : nt.propHooks._default.set(this), this
+            var t, n = et.propHooks[this.prop];
+            return this.options.duration ? this.pos = t = S.easing[this.easing](e, this.options.duration * e, 0, 1, this.options.duration) : this.pos = t = e, this.now = (this.end - this.start) * t + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), n && n.set ? n.set(this) : et.propHooks._default.set(this), this
         }
-    }).init.prototype = nt.prototype, (nt.propHooks = {
+    }).init.prototype = et.prototype, (et.propHooks = {
         _default: {
             get: function(e) {
                 var t;
-                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = k.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
+                return 1 !== e.elem.nodeType || null != e.elem[e.prop] && null == e.elem.style[e.prop] ? e.elem[e.prop] : (t = S.css(e.elem, e.prop, "")) && "auto" !== t ? t : 0
             },
             set: function(e) {
-                k.fx.step[e.prop] ? k.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !k.cssHooks[e.prop] && null == e.elem.style[Ge(e.prop)] ? e.elem[e.prop] = e.now : k.style(e.elem, e.prop, e.now + e.unit)
+                S.fx.step[e.prop] ? S.fx.step[e.prop](e) : 1 !== e.elem.nodeType || !S.cssHooks[e.prop] && null == e.elem.style[Xe(e.prop)] ? e.elem[e.prop] = e.now : S.style(e.elem, e.prop, e.now + e.unit)
             }
         }
-    }).scrollTop = nt.propHooks.scrollLeft = {
+    }).scrollTop = et.propHooks.scrollLeft = {
         set: function(e) {
             e.elem.nodeType && e.elem.parentNode && (e.elem[e.prop] = e.now)
         }
-    }, k.easing = {
+    }, S.easing = {
         linear: function(e) {
             return e
         },
         swing: function(e) {
             return .5 - Math.cos(e * Math.PI) / 2
         },
         _default: "swing"
-    }, k.fx = nt.prototype.init, k.fx.step = {};
-    var rt, it, ot, at, st = /^(?:toggle|show|hide)$/,
-        ut = /queueHooks$/;
+    }, S.fx = et.prototype.init, S.fx.step = {};
+    var tt, nt, rt, it, ot = /^(?:toggle|show|hide)$/,
+        at = /queueHooks$/;
 
-    function lt() {
-        it && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(lt) : C.setTimeout(lt, k.fx.interval), k.fx.tick())
+    function st() {
+        nt && (!1 === E.hidden && C.requestAnimationFrame ? C.requestAnimationFrame(st) : C.setTimeout(st, S.fx.interval), S.fx.tick())
     }
 
-    function ct() {
+    function ut() {
         return C.setTimeout(function() {
-            rt = void 0
-        }), rt = Date.now()
+            tt = void 0
+        }), tt = Date.now()
     }
 
-    function ft(e, t) {
+    function lt(e, t) {
         var n, r = 0,
             i = {
                 height: e
             };
-        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = re[r])] = i["padding" + n] = e;
+        for (t = t ? 1 : 0; r < 4; r += 2 - t) i["margin" + (n = ne[r])] = i["padding" + n] = e;
         return t && (i.opacity = i.width = e), i
     }
 
-    function pt(e, t, n) {
-        for (var r, i = (dt.tweeners[t] || []).concat(dt.tweeners["*"]), o = 0, a = i.length; o < a; o++)
+    function ct(e, t, n) {
+        for (var r, i = (ft.tweeners[t] || []).concat(ft.tweeners["*"]), o = 0, a = i.length; o < a; o++)
             if (r = i[o].call(n, t, e)) return r
     }
 
-    function dt(o, e, t) {
+    function ft(o, e, t) {
         var n, a, r = 0,
-            i = dt.prefilters.length,
-            s = k.Deferred().always(function() {
+            i = ft.prefilters.length,
+            s = S.Deferred().always(function() {
                 delete u.elem
             }),
             u = function() {
                 if (a) return !1;
-                for (var e = rt || ct(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
+                for (var e = tt || ut(), t = Math.max(0, l.startTime + l.duration - e), n = 1 - (t / l.duration || 0), r = 0, i = l.tweens.length; r < i; r++) l.tweens[r].run(n);
                 return s.notifyWith(o, [l, n, t]), n < 1 && i ? t : (i || s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l]), !1)
             },
             l = s.promise({
                 elem: o,
-                props: k.extend({}, e),
-                opts: k.extend(!0, {
+                props: S.extend({}, e),
+                opts: S.extend(!0, {
                     specialEasing: {},
-                    easing: k.easing._default
+                    easing: S.easing._default
                 }, t),
                 originalProperties: e,
                 originalOptions: t,
-                startTime: rt || ct(),
+                startTime: tt || ut(),
                 duration: t.duration,
                 tweens: [],
                 createTween: function(e, t) {
-                    var n = k.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
+                    var n = S.Tween(o, l.opts, e, t, l.opts.specialEasing[e] || l.opts.easing);
                     return l.tweens.push(n), n
                 },
                 stop: function(e) {
                     var t = 0,
                         n = e ? l.tweens.length : 0;
                     if (a) return this;
                     for (a = !0; t < n; t++) l.tweens[t].run(1);
                     return e ? (s.notifyWith(o, [l, 1, 0]), s.resolveWith(o, [l, e])) : s.rejectWith(o, [l, e]), this
                 }
             }),
             c = l.props;
         for (! function(e, t) {
                 var n, r, i, o, a;
                 for (n in e)
-                    if (i = t[r = V(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = k.cssHooks[r]) && "expand" in a)
+                    if (i = t[r = X(n)], o = e[n], Array.isArray(o) && (i = o[1], o = e[n] = o[0]), n !== r && (e[r] = o, delete e[n]), (a = S.cssHooks[r]) && "expand" in a)
                         for (n in o = a.expand(o), delete e[r], o) n in e || (e[n] = o[n], t[n] = i);
                     else t[r] = i
             }(c, l.opts.specialEasing); r < i; r++)
-            if (n = dt.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (k._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
-        return k.map(c, pt, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), k.fx.timer(k.extend(u, {
+            if (n = ft.prefilters[r].call(l, o, c, l.opts)) return m(n.stop) && (S._queueHooks(l.elem, l.opts.queue).stop = n.stop.bind(n)), n;
+        return S.map(c, ct, l), m(l.opts.start) && l.opts.start.call(o, l), l.progress(l.opts.progress).done(l.opts.done, l.opts.complete).fail(l.opts.fail).always(l.opts.always), S.fx.timer(S.extend(u, {
             elem: o,
             anim: l,
             queue: l.opts.queue
         })), l
     }
-    k.Animation = k.extend(dt, {
+    S.Animation = S.extend(ft, {
         tweeners: {
             "*": [function(e, t) {
                 var n = this.createTween(e, t);
-                return le(n.elem, e, ne.exec(t), n), n
+                return se(n.elem, e, te.exec(t), n), n
             }]
         },
         tweener: function(e, t) {
-            m(e) ? (t = e, e = ["*"]) : e = e.match(R);
-            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], dt.tweeners[n] = dt.tweeners[n] || [], dt.tweeners[n].unshift(t)
+            m(e) ? (t = e, e = ["*"]) : e = e.match(P);
+            for (var n, r = 0, i = e.length; r < i; r++) n = e[r], ft.tweeners[n] = ft.tweeners[n] || [], ft.tweeners[n].unshift(t)
         },
         prefilters: [function(e, t, n) {
             var r, i, o, a, s, u, l, c, f = "width" in t || "height" in t,
                 p = this,
                 d = {},
                 h = e.style,
-                g = e.nodeType && se(e),
-                v = Q.get(e, "fxshow");
-            for (r in n.queue || (null == (a = k._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
+                g = e.nodeType && ae(e),
+                v = Y.get(e, "fxshow");
+            for (r in n.queue || (null == (a = S._queueHooks(e, "fx")).unqueued && (a.unqueued = 0, s = a.empty.fire, a.empty.fire = function() {
                     a.unqueued || s()
                 }), a.unqueued++, p.always(function() {
                     p.always(function() {
-                        a.unqueued--, k.queue(e, "fx").length || a.empty.fire()
+                        a.unqueued--, S.queue(e, "fx").length || a.empty.fire()
                     })
                 })), t)
-                if (i = t[r], st.test(i)) {
+                if (i = t[r], ot.test(i)) {
                     if (delete t[r], o = o || "toggle" === i, i === (g ? "hide" : "show")) {
                         if ("show" !== i || !v || void 0 === v[r]) continue;
                         g = !0
                     }
-                    d[r] = v && v[r] || k.style(e, r)
-                } if ((u = !k.isEmptyObject(t)) || !k.isEmptyObject(d))
-                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Q.get(e, "display")), "none" === (c = k.css(e, "display")) && (l ? c = l : (fe([e], !0), l = e.style.display || l, c = k.css(e, "display"), fe([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === k.css(e, "float") && (u || (p.done(function() {
+                    d[r] = v && v[r] || S.style(e, r)
+                } if ((u = !S.isEmptyObject(t)) || !S.isEmptyObject(d))
+                for (r in f && 1 === e.nodeType && (n.overflow = [h.overflow, h.overflowX, h.overflowY], null == (l = v && v.display) && (l = Y.get(e, "display")), "none" === (c = S.css(e, "display")) && (l ? c = l : (le([e], !0), l = e.style.display || l, c = S.css(e, "display"), le([e]))), ("inline" === c || "inline-block" === c && null != l) && "none" === S.css(e, "float") && (u || (p.done(function() {
                         h.display = l
                     }), null == l && (c = h.display, l = "none" === c ? "" : c)), h.display = "inline-block")), n.overflow && (h.overflow = "hidden", p.always(function() {
                         h.overflow = n.overflow[0], h.overflowX = n.overflow[1], h.overflowY = n.overflow[2]
-                    })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Q.access(e, "fxshow", {
+                    })), u = !1, d) u || (v ? "hidden" in v && (g = v.hidden) : v = Y.access(e, "fxshow", {
                     display: l
-                }), o && (v.hidden = !g), g && fe([e], !0), p.done(function() {
-                    for (r in g || fe([e]), Q.remove(e, "fxshow"), d) k.style(e, r, d[r])
-                })), u = pt(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
+                }), o && (v.hidden = !g), g && le([e], !0), p.done(function() {
+                    for (r in g || le([e]), Y.remove(e, "fxshow"), d) S.style(e, r, d[r])
+                })), u = ct(g ? v[r] : 0, r, p), r in v || (v[r] = u.start, g && (u.end = u.start, u.start = 0))
         }],
         prefilter: function(e, t) {
-            t ? dt.prefilters.unshift(e) : dt.prefilters.push(e)
+            t ? ft.prefilters.unshift(e) : ft.prefilters.push(e)
         }
-    }), k.speed = function(e, t, n) {
-        var r = e && "object" == typeof e ? k.extend({}, e) : {
+    }), S.speed = function(e, t, n) {
+        var r = e && "object" == typeof e ? S.extend({}, e) : {
             complete: n || !n && t || m(e) && e,
             duration: e,
             easing: n && t || t && !m(t) && t
         };
-        return k.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in k.fx.speeds ? r.duration = k.fx.speeds[r.duration] : r.duration = k.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
-            m(r.old) && r.old.call(this), r.queue && k.dequeue(this, r.queue)
+        return S.fx.off ? r.duration = 0 : "number" != typeof r.duration && (r.duration in S.fx.speeds ? r.duration = S.fx.speeds[r.duration] : r.duration = S.fx.speeds._default), null != r.queue && !0 !== r.queue || (r.queue = "fx"), r.old = r.complete, r.complete = function() {
+            m(r.old) && r.old.call(this), r.queue && S.dequeue(this, r.queue)
         }, r
-    }, k.fn.extend({
+    }, S.fn.extend({
         fadeTo: function(e, t, n, r) {
-            return this.filter(se).css("opacity", 0).show().end().animate({
+            return this.filter(ae).css("opacity", 0).show().end().animate({
                 opacity: t
             }, e, n, r)
         },
         animate: function(t, e, n, r) {
-            var i = k.isEmptyObject(t),
-                o = k.speed(e, n, r),
+            var i = S.isEmptyObject(t),
+                o = S.speed(e, n, r),
                 a = function() {
-                    var e = dt(this, k.extend({}, t), o);
-                    (i || Q.get(this, "finish")) && e.stop(!0)
+                    var e = ft(this, S.extend({}, t), o);
+                    (i || Y.get(this, "finish")) && e.stop(!0)
                 };
             return a.finish = a, i || !1 === o.queue ? this.each(a) : this.queue(o.queue, a)
         },
         stop: function(i, e, o) {
             var a = function(e) {
                 var t = e.stop;
                 delete e.stop, t(o)
             };
-            return "string" != typeof i && (o = e, e = i, i = void 0), e && !1 !== i && this.queue(i || "fx", []), this.each(function() {
+            return "string" != typeof i && (o = e, e = i, i = void 0), e && this.queue(i || "fx", []), this.each(function() {
                 var e = !0,
                     t = null != i && i + "queueHooks",
-                    n = k.timers,
-                    r = Q.get(this);
+                    n = S.timers,
+                    r = Y.get(this);
                 if (t) r[t] && r[t].stop && a(r[t]);
                 else
-                    for (t in r) r[t] && r[t].stop && ut.test(t) && a(r[t]);
+                    for (t in r) r[t] && r[t].stop && at.test(t) && a(r[t]);
                 for (t = n.length; t--;) n[t].elem !== this || null != i && n[t].queue !== i || (n[t].anim.stop(o), e = !1, n.splice(t, 1));
-                !e && o || k.dequeue(this, i)
+                !e && o || S.dequeue(this, i)
             })
         },
         finish: function(a) {
             return !1 !== a && (a = a || "fx"), this.each(function() {
-                var e, t = Q.get(this),
+                var e, t = Y.get(this),
                     n = t[a + "queue"],
                     r = t[a + "queueHooks"],
-                    i = k.timers,
+                    i = S.timers,
                     o = n ? n.length : 0;
-                for (t.finish = !0, k.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
+                for (t.finish = !0, S.queue(this, a, []), r && r.stop && r.stop.call(this, !0), e = i.length; e--;) i[e].elem === this && i[e].queue === a && (i[e].anim.stop(!0), i.splice(e, 1));
                 for (e = 0; e < o; e++) n[e] && n[e].finish && n[e].finish.call(this);
                 delete t.finish
             })
         }
-    }), k.each(["toggle", "show", "hide"], function(e, r) {
-        var i = k.fn[r];
-        k.fn[r] = function(e, t, n) {
-            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(ft(r, !0), e, t, n)
-        }
-    }), k.each({
-        slideDown: ft("show"),
-        slideUp: ft("hide"),
-        slideToggle: ft("toggle"),
+    }), S.each(["toggle", "show", "hide"], function(e, r) {
+        var i = S.fn[r];
+        S.fn[r] = function(e, t, n) {
+            return null == e || "boolean" == typeof e ? i.apply(this, arguments) : this.animate(lt(r, !0), e, t, n)
+        }
+    }), S.each({
+        slideDown: lt("show"),
+        slideUp: lt("hide"),
+        slideToggle: lt("toggle"),
         fadeIn: {
             opacity: "show"
         },
         fadeOut: {
             opacity: "hide"
         },
         fadeToggle: {
             opacity: "toggle"
         }
     }, function(e, r) {
-        k.fn[e] = function(e, t, n) {
+        S.fn[e] = function(e, t, n) {
             return this.animate(r, e, t, n)
         }
-    }), k.timers = [], k.fx.tick = function() {
+    }), S.timers = [], S.fx.tick = function() {
         var e, t = 0,
-            n = k.timers;
-        for (rt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
-        n.length || k.fx.stop(), rt = void 0
-    }, k.fx.timer = function(e) {
-        k.timers.push(e), k.fx.start()
-    }, k.fx.interval = 13, k.fx.start = function() {
-        it || (it = !0, lt())
-    }, k.fx.stop = function() {
-        it = null
-    }, k.fx.speeds = {
+            n = S.timers;
+        for (tt = Date.now(); t < n.length; t++)(e = n[t])() || n[t] !== e || n.splice(t--, 1);
+        n.length || S.fx.stop(), tt = void 0
+    }, S.fx.timer = function(e) {
+        S.timers.push(e), S.fx.start()
+    }, S.fx.interval = 13, S.fx.start = function() {
+        nt || (nt = !0, st())
+    }, S.fx.stop = function() {
+        nt = null
+    }, S.fx.speeds = {
         slow: 600,
         fast: 200,
         _default: 400
-    }, k.fn.delay = function(r, e) {
-        return r = k.fx && k.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
+    }, S.fn.delay = function(r, e) {
+        return r = S.fx && S.fx.speeds[r] || r, e = e || "fx", this.queue(e, function(e, t) {
             var n = C.setTimeout(e, r);
             t.stop = function() {
                 C.clearTimeout(n)
             }
         })
-    }, ot = E.createElement("input"), at = E.createElement("select").appendChild(E.createElement("option")), ot.type = "checkbox", y.checkOn = "" !== ot.value, y.optSelected = at.selected, (ot = E.createElement("input")).value = "t", ot.type = "radio", y.radioValue = "t" === ot.value;
-    var ht, gt = k.expr.attrHandle;
-    k.fn.extend({
+    }, rt = E.createElement("input"), it = E.createElement("select").appendChild(E.createElement("option")), rt.type = "checkbox", y.checkOn = "" !== rt.value, y.optSelected = it.selected, (rt = E.createElement("input")).value = "t", rt.type = "radio", y.radioValue = "t" === rt.value;
+    var pt, dt = S.expr.attrHandle;
+    S.fn.extend({
         attr: function(e, t) {
-            return _(this, k.attr, e, t, 1 < arguments.length)
+            return $(this, S.attr, e, t, 1 < arguments.length)
         },
         removeAttr: function(e) {
             return this.each(function() {
-                k.removeAttr(this, e)
+                S.removeAttr(this, e)
             })
         }
-    }), k.extend({
+    }), S.extend({
         attr: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? k.prop(e, t, n) : (1 === o && k.isXMLDoc(e) || (i = k.attrHooks[t.toLowerCase()] || (k.expr.match.bool.test(t) ? ht : void 0)), void 0 !== n ? null === n ? void k.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = k.find.attr(e, t)) ? void 0 : r)
+            if (3 !== o && 8 !== o && 2 !== o) return "undefined" == typeof e.getAttribute ? S.prop(e, t, n) : (1 === o && S.isXMLDoc(e) || (i = S.attrHooks[t.toLowerCase()] || (S.expr.match.bool.test(t) ? pt : void 0)), void 0 !== n ? null === n ? void S.removeAttr(e, t) : i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : (e.setAttribute(t, n + ""), n) : i && "get" in i && null !== (r = i.get(e, t)) ? r : null == (r = S.find.attr(e, t)) ? void 0 : r)
         },
         attrHooks: {
             type: {
                 set: function(e, t) {
                     if (!y.radioValue && "radio" === t && A(e, "input")) {
                         var n = e.value;
                         return e.setAttribute("type", t), n && (e.value = n), t
                     }
                 }
             }
         },
         removeAttr: function(e, t) {
             var n, r = 0,
-                i = t && t.match(R);
+                i = t && t.match(P);
             if (i && 1 === e.nodeType)
                 while (n = i[r++]) e.removeAttribute(n)
         }
-    }), ht = {
+    }), pt = {
         set: function(e, t, n) {
-            return !1 === t ? k.removeAttr(e, n) : e.setAttribute(n, n), n
+            return !1 === t ? S.removeAttr(e, n) : e.setAttribute(n, n), n
         }
-    }, k.each(k.expr.match.bool.source.match(/\w+/g), function(e, t) {
-        var a = gt[t] || k.find.attr;
-        gt[t] = function(e, t, n) {
+    }, S.each(S.expr.match.bool.source.match(/\w+/g), function(e, t) {
+        var a = dt[t] || S.find.attr;
+        dt[t] = function(e, t, n) {
             var r, i, o = t.toLowerCase();
-            return n || (i = gt[o], gt[o] = r, r = null != a(e, t, n) ? o : null, gt[o] = i), r
+            return n || (i = dt[o], dt[o] = r, r = null != a(e, t, n) ? o : null, dt[o] = i), r
         }
     });
-    var vt = /^(?:input|select|textarea|button)$/i,
-        yt = /^(?:a|area)$/i;
+    var ht = /^(?:input|select|textarea|button)$/i,
+        gt = /^(?:a|area)$/i;
 
-    function mt(e) {
-        return (e.match(R) || []).join(" ")
+    function vt(e) {
+        return (e.match(P) || []).join(" ")
     }
 
-    function xt(e) {
+    function yt(e) {
         return e.getAttribute && e.getAttribute("class") || ""
     }
 
-    function bt(e) {
-        return Array.isArray(e) ? e : "string" == typeof e && e.match(R) || []
+    function mt(e) {
+        return Array.isArray(e) ? e : "string" == typeof e && e.match(P) || []
     }
-    k.fn.extend({
+    S.fn.extend({
         prop: function(e, t) {
-            return _(this, k.prop, e, t, 1 < arguments.length)
+            return $(this, S.prop, e, t, 1 < arguments.length)
         },
         removeProp: function(e) {
             return this.each(function() {
-                delete this[k.propFix[e] || e]
+                delete this[S.propFix[e] || e]
             })
         }
-    }), k.extend({
+    }), S.extend({
         prop: function(e, t, n) {
             var r, i, o = e.nodeType;
-            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && k.isXMLDoc(e) || (t = k.propFix[t] || t, i = k.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
+            if (3 !== o && 8 !== o && 2 !== o) return 1 === o && S.isXMLDoc(e) || (t = S.propFix[t] || t, i = S.propHooks[t]), void 0 !== n ? i && "set" in i && void 0 !== (r = i.set(e, n, t)) ? r : e[t] = n : i && "get" in i && null !== (r = i.get(e, t)) ? r : e[t]
         },
         propHooks: {
             tabIndex: {
                 get: function(e) {
-                    var t = k.find.attr(e, "tabindex");
-                    return t ? parseInt(t, 10) : vt.test(e.nodeName) || yt.test(e.nodeName) && e.href ? 0 : -1
+                    var t = S.find.attr(e, "tabindex");
+                    return t ? parseInt(t, 10) : ht.test(e.nodeName) || gt.test(e.nodeName) && e.href ? 0 : -1
                 }
             }
         },
         propFix: {
             "for": "htmlFor",
             "class": "className"
         }
-    }), y.optSelected || (k.propHooks.selected = {
+    }), y.optSelected || (S.propHooks.selected = {
         get: function(e) {
             var t = e.parentNode;
             return t && t.parentNode && t.parentNode.selectedIndex, null
         },
         set: function(e) {
             var t = e.parentNode;
             t && (t.selectedIndex, t.parentNode && t.parentNode.selectedIndex)
         }
-    }), k.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
-        k.propFix[this.toLowerCase()] = this
-    }), k.fn.extend({
+    }), S.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
+        S.propFix[this.toLowerCase()] = this
+    }), S.fn.extend({
         addClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                k(this).addClass(t.call(this, e, xt(this)))
+                S(this).addClass(t.call(this, e, yt(this)))
             });
-            if ((e = bt(t)).length)
+            if ((e = mt(t)).length)
                 while (n = this[u++])
-                    if (i = xt(n), r = 1 === n.nodeType && " " + mt(i) + " ") {
+                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
                         a = 0;
                         while (o = e[a++]) r.indexOf(" " + o + " ") < 0 && (r += o + " ");
-                        i !== (s = mt(r)) && n.setAttribute("class", s)
+                        i !== (s = vt(r)) && n.setAttribute("class", s)
                     } return this
         },
         removeClass: function(t) {
             var e, n, r, i, o, a, s, u = 0;
             if (m(t)) return this.each(function(e) {
-                k(this).removeClass(t.call(this, e, xt(this)))
+                S(this).removeClass(t.call(this, e, yt(this)))
             });
             if (!arguments.length) return this.attr("class", "");
-            if ((e = bt(t)).length)
+            if ((e = mt(t)).length)
                 while (n = this[u++])
-                    if (i = xt(n), r = 1 === n.nodeType && " " + mt(i) + " ") {
+                    if (i = yt(n), r = 1 === n.nodeType && " " + vt(i) + " ") {
                         a = 0;
                         while (o = e[a++])
                             while (-1 < r.indexOf(" " + o + " ")) r = r.replace(" " + o + " ", " ");
-                        i !== (s = mt(r)) && n.setAttribute("class", s)
+                        i !== (s = vt(r)) && n.setAttribute("class", s)
                     } return this
         },
         toggleClass: function(i, t) {
             var o = typeof i,
                 a = "string" === o || Array.isArray(i);
             return "boolean" == typeof t && a ? t ? this.addClass(i) : this.removeClass(i) : m(i) ? this.each(function(e) {
-                k(this).toggleClass(i.call(this, e, xt(this), t), t)
+                S(this).toggleClass(i.call(this, e, yt(this), t), t)
             }) : this.each(function() {
                 var e, t, n, r;
                 if (a) {
-                    t = 0, n = k(this), r = bt(i);
+                    t = 0, n = S(this), r = mt(i);
                     while (e = r[t++]) n.hasClass(e) ? n.removeClass(e) : n.addClass(e)
-                } else void 0 !== i && "boolean" !== o || ((e = xt(this)) && Q.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Q.get(this, "__className__") || ""))
+                } else void 0 !== i && "boolean" !== o || ((e = yt(this)) && Y.set(this, "__className__", e), this.setAttribute && this.setAttribute("class", e || !1 === i ? "" : Y.get(this, "__className__") || ""))
             })
         },
         hasClass: function(e) {
             var t, n, r = 0;
             t = " " + e + " ";
             while (n = this[r++])
-                if (1 === n.nodeType && -1 < (" " + mt(xt(n)) + " ").indexOf(t)) return !0;
+                if (1 === n.nodeType && -1 < (" " + vt(yt(n)) + " ").indexOf(t)) return !0;
             return !1
         }
     });
-    var wt = /\r/g;
-    k.fn.extend({
+    var xt = /\r/g;
+    S.fn.extend({
         val: function(n) {
             var r, e, i, t = this[0];
             return arguments.length ? (i = m(n), this.each(function(e) {
                 var t;
-                1 === this.nodeType && (null == (t = i ? n.call(this, e, k(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = k.map(t, function(e) {
+                1 === this.nodeType && (null == (t = i ? n.call(this, e, S(this).val()) : n) ? t = "" : "number" == typeof t ? t += "" : Array.isArray(t) && (t = S.map(t, function(e) {
                     return null == e ? "" : e + ""
-                })), (r = k.valHooks[this.type] || k.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
-            })) : t ? (r = k.valHooks[t.type] || k.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(wt, "") : null == e ? "" : e : void 0
+                })), (r = S.valHooks[this.type] || S.valHooks[this.nodeName.toLowerCase()]) && "set" in r && void 0 !== r.set(this, t, "value") || (this.value = t))
+            })) : t ? (r = S.valHooks[t.type] || S.valHooks[t.nodeName.toLowerCase()]) && "get" in r && void 0 !== (e = r.get(t, "value")) ? e : "string" == typeof(e = t.value) ? e.replace(xt, "") : null == e ? "" : e : void 0
         }
-    }), k.extend({
+    }), S.extend({
         valHooks: {
             option: {
                 get: function(e) {
-                    var t = k.find.attr(e, "value");
-                    return null != t ? t : mt(k.text(e))
+                    var t = S.find.attr(e, "value");
+                    return null != t ? t : vt(S.text(e))
                 }
             },
             select: {
                 get: function(e) {
                     var t, n, r, i = e.options,
                         o = e.selectedIndex,
                         a = "select-one" === e.type,
                         s = a ? null : [],
                         u = a ? o + 1 : i.length;
                     for (r = o < 0 ? u : a ? o : 0; r < u; r++)
                         if (((n = i[r]).selected || r === o) && !n.disabled && (!n.parentNode.disabled || !A(n.parentNode, "optgroup"))) {
-                            if (t = k(n).val(), a) return t;
+                            if (t = S(n).val(), a) return t;
                             s.push(t)
                         } return s
                 },
                 set: function(e, t) {
                     var n, r, i = e.options,
-                        o = k.makeArray(t),
+                        o = S.makeArray(t),
                         a = i.length;
-                    while (a--)((r = i[a]).selected = -1 < k.inArray(k.valHooks.option.get(r), o)) && (n = !0);
+                    while (a--)((r = i[a]).selected = -1 < S.inArray(S.valHooks.option.get(r), o)) && (n = !0);
                     return n || (e.selectedIndex = -1), o
                 }
             }
         }
-    }), k.each(["radio", "checkbox"], function() {
-        k.valHooks[this] = {
+    }), S.each(["radio", "checkbox"], function() {
+        S.valHooks[this] = {
             set: function(e, t) {
-                if (Array.isArray(t)) return e.checked = -1 < k.inArray(k(e).val(), t)
+                if (Array.isArray(t)) return e.checked = -1 < S.inArray(S(e).val(), t)
             }
-        }, y.checkOn || (k.valHooks[this].get = function(e) {
+        }, y.checkOn || (S.valHooks[this].get = function(e) {
             return null === e.getAttribute("value") ? "on" : e.value
         })
     }), y.focusin = "onfocusin" in C;
-    var Tt = /^(?:focusinfocus|focusoutblur)$/,
-        Ct = function(e) {
+    var bt = /^(?:focusinfocus|focusoutblur)$/,
+        wt = function(e) {
             e.stopPropagation()
         };
-    k.extend(k.event, {
+    S.extend(S.event, {
         trigger: function(e, t, n, r) {
             var i, o, a, s, u, l, c, f, p = [n || E],
                 d = v.call(e, "type") ? e.type : e,
                 h = v.call(e, "namespace") ? e.namespace.split(".") : [];
-            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !Tt.test(d + k.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[k.expando] ? e : new k.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : k.makeArray(t, [e]), c = k.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
+            if (o = f = a = n = n || E, 3 !== n.nodeType && 8 !== n.nodeType && !bt.test(d + S.event.triggered) && (-1 < d.indexOf(".") && (d = (h = d.split(".")).shift(), h.sort()), u = d.indexOf(":") < 0 && "on" + d, (e = e[S.expando] ? e : new S.Event(d, "object" == typeof e && e)).isTrigger = r ? 2 : 3, e.namespace = h.join("."), e.rnamespace = e.namespace ? new RegExp("(^|\\.)" + h.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, e.result = void 0, e.target || (e.target = n), t = null == t ? [e] : S.makeArray(t, [e]), c = S.event.special[d] || {}, r || !c.trigger || !1 !== c.trigger.apply(n, t))) {
                 if (!r && !c.noBubble && !x(n)) {
-                    for (s = c.delegateType || d, Tt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
+                    for (s = c.delegateType || d, bt.test(s + d) || (o = o.parentNode); o; o = o.parentNode) p.push(o), a = o;
                     a === (n.ownerDocument || E) && p.push(a.defaultView || a.parentWindow || C)
                 }
                 i = 0;
-                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Q.get(o, "events") || {})[e.type] && Q.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && G(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
-                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !G(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), k.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, Ct), n[d](), e.isPropagationStopped() && f.removeEventListener(d, Ct), k.event.triggered = void 0, a && (n[u] = a)), e.result
+                while ((o = p[i++]) && !e.isPropagationStopped()) f = o, e.type = 1 < i ? s : c.bindType || d, (l = (Y.get(o, "events") || Object.create(null))[e.type] && Y.get(o, "handle")) && l.apply(o, t), (l = u && o[u]) && l.apply && V(o) && (e.result = l.apply(o, t), !1 === e.result && e.preventDefault());
+                return e.type = d, r || e.isDefaultPrevented() || c._default && !1 !== c._default.apply(p.pop(), t) || !V(n) || u && m(n[d]) && !x(n) && ((a = n[u]) && (n[u] = null), S.event.triggered = d, e.isPropagationStopped() && f.addEventListener(d, wt), n[d](), e.isPropagationStopped() && f.removeEventListener(d, wt), S.event.triggered = void 0, a && (n[u] = a)), e.result
             }
         },
         simulate: function(e, t, n) {
-            var r = k.extend(new k.Event, n, {
+            var r = S.extend(new S.Event, n, {
                 type: e,
                 isSimulated: !0
             });
-            k.event.trigger(r, null, t)
+            S.event.trigger(r, null, t)
         }
-    }), k.fn.extend({
+    }), S.fn.extend({
         trigger: function(e, t) {
             return this.each(function() {
-                k.event.trigger(e, t, this)
+                S.event.trigger(e, t, this)
             })
         },
         triggerHandler: function(e, t) {
             var n = this[0];
-            if (n) return k.event.trigger(e, t, n, !0)
+            if (n) return S.event.trigger(e, t, n, !0)
         }
-    }), y.focusin || k.each({
+    }), y.focusin || S.each({
         focus: "focusin",
         blur: "focusout"
     }, function(n, r) {
         var i = function(e) {
-            k.event.simulate(r, e.target, k.event.fix(e))
+            S.event.simulate(r, e.target, S.event.fix(e))
         };
-        k.event.special[r] = {
+        S.event.special[r] = {
             setup: function() {
-                var e = this.ownerDocument || this,
-                    t = Q.access(e, r);
-                t || e.addEventListener(n, i, !0), Q.access(e, r, (t || 0) + 1)
+                var e = this.ownerDocument || this.document || this,
+                    t = Y.access(e, r);
+                t || e.addEventListener(n, i, !0), Y.access(e, r, (t || 0) + 1)
             },
             teardown: function() {
-                var e = this.ownerDocument || this,
-                    t = Q.access(e, r) - 1;
-                t ? Q.access(e, r, t) : (e.removeEventListener(n, i, !0), Q.remove(e, r))
+                var e = this.ownerDocument || this.document || this,
+                    t = Y.access(e, r) - 1;
+                t ? Y.access(e, r, t) : (e.removeEventListener(n, i, !0), Y.remove(e, r))
             }
         }
     });
-    var Et = C.location,
-        kt = Date.now(),
-        St = /\?/;
-    k.parseXML = function(e) {
+    var Tt = C.location,
+        Ct = {
+            guid: Date.now()
+        },
+        Et = /\?/;
+    S.parseXML = function(e) {
         var t;
         if (!e || "string" != typeof e) return null;
         try {
             t = (new C.DOMParser).parseFromString(e, "text/xml")
         } catch (e) {
             t = void 0
         }
-        return t && !t.getElementsByTagName("parsererror").length || k.error("Invalid XML: " + e), t
+        return t && !t.getElementsByTagName("parsererror").length || S.error("Invalid XML: " + e), t
     };
-    var Nt = /\[\]$/,
-        At = /\r?\n/g,
-        Dt = /^(?:submit|button|image|reset|file)$/i,
-        jt = /^(?:input|select|textarea|keygen)/i;
+    var St = /\[\]$/,
+        kt = /\r?\n/g,
+        At = /^(?:submit|button|image|reset|file)$/i,
+        Nt = /^(?:input|select|textarea|keygen)/i;
 
-    function qt(n, e, r, i) {
+    function Dt(n, e, r, i) {
         var t;
-        if (Array.isArray(e)) k.each(e, function(e, t) {
-            r || Nt.test(n) ? i(n, t) : qt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
+        if (Array.isArray(e)) S.each(e, function(e, t) {
+            r || St.test(n) ? i(n, t) : Dt(n + "[" + ("object" == typeof t && null != t ? e : "") + "]", t, r, i)
         });
         else if (r || "object" !== w(e)) i(n, e);
         else
-            for (t in e) qt(n + "[" + t + "]", e[t], r, i)
+            for (t in e) Dt(n + "[" + t + "]", e[t], r, i)
     }
-    k.param = function(e, t) {
+    S.param = function(e, t) {
         var n, r = [],
             i = function(e, t) {
                 var n = m(t) ? t() : t;
                 r[r.length] = encodeURIComponent(e) + "=" + encodeURIComponent(null == n ? "" : n)
             };
         if (null == e) return "";
-        if (Array.isArray(e) || e.jquery && !k.isPlainObject(e)) k.each(e, function() {
+        if (Array.isArray(e) || e.jquery && !S.isPlainObject(e)) S.each(e, function() {
             i(this.name, this.value)
         });
         else
-            for (n in e) qt(n, e[n], t, i);
+            for (n in e) Dt(n, e[n], t, i);
         return r.join("&")
-    }, k.fn.extend({
+    }, S.fn.extend({
         serialize: function() {
-            return k.param(this.serializeArray())
+            return S.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
-                var e = k.prop(this, "elements");
-                return e ? k.makeArray(e) : this
+                var e = S.prop(this, "elements");
+                return e ? S.makeArray(e) : this
             }).filter(function() {
                 var e = this.type;
-                return this.name && !k(this).is(":disabled") && jt.test(this.nodeName) && !Dt.test(e) && (this.checked || !pe.test(e))
+                return this.name && !S(this).is(":disabled") && Nt.test(this.nodeName) && !At.test(e) && (this.checked || !pe.test(e))
             }).map(function(e, t) {
-                var n = k(this).val();
-                return null == n ? null : Array.isArray(n) ? k.map(n, function(e) {
+                var n = S(this).val();
+                return null == n ? null : Array.isArray(n) ? S.map(n, function(e) {
                     return {
                         name: t.name,
-                        value: e.replace(At, "\r\n")
+                        value: e.replace(kt, "\r\n")
                     }
                 }) : {
                     name: t.name,
-                    value: n.replace(At, "\r\n")
+                    value: n.replace(kt, "\r\n")
                 }
             }).get()
         }
     });
-    var Lt = /%20/g,
-        Ht = /#.*$/,
-        Ot = /([?&])_=[^&]*/,
-        Pt = /^(.*?):[ \t]*([^\r\n]*)$/gm,
-        Rt = /^(?:GET|HEAD)$/,
-        Mt = /^\/\//,
-        It = {},
-        Wt = {},
-        $t = "*/".concat("*"),
-        Ft = E.createElement("a");
+    var jt = /%20/g,
+        qt = /#.*$/,
+        Lt = /([?&])_=[^&]*/,
+        Ht = /^(.*?):[ \t]*([^\r\n]*)$/gm,
+        Ot = /^(?:GET|HEAD)$/,
+        Pt = /^\/\//,
+        Rt = {},
+        Mt = {},
+        It = "*/".concat("*"),
+        Wt = E.createElement("a");
 
-    function Bt(o) {
+    function Ft(o) {
         return function(e, t) {
             "string" != typeof e && (t = e, e = "*");
             var n, r = 0,
-                i = e.toLowerCase().match(R) || [];
+                i = e.toLowerCase().match(P) || [];
             if (m(t))
                 while (n = i[r++]) "+" === n[0] ? (n = n.slice(1) || "*", (o[n] = o[n] || []).unshift(t)) : (o[n] = o[n] || []).push(t)
         }
     }
 
-    function _t(t, i, o, a) {
+    function Bt(t, i, o, a) {
         var s = {},
-            u = t === Wt;
+            u = t === Mt;
 
         function l(e) {
             var r;
-            return s[e] = !0, k.each(t[e] || [], function(e, t) {
+            return s[e] = !0, S.each(t[e] || [], function(e, t) {
                 var n = t(i, o, a);
                 return "string" != typeof n || u || s[n] ? u ? !(r = n) : void 0 : (i.dataTypes.unshift(n), l(n), !1)
             }), r
         }
         return l(i.dataTypes[0]) || !s["*"] && l("*")
     }
 
-    function zt(e, t) {
-        var n, r, i = k.ajaxSettings.flatOptions || {};
+    function $t(e, t) {
+        var n, r, i = S.ajaxSettings.flatOptions || {};
         for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
-        return r && k.extend(!0, e, r), e
+        return r && S.extend(!0, e, r), e
     }
-    Ft.href = Et.href, k.extend({
+    Wt.href = Tt.href, S.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: Et.href,
+            url: Tt.href,
             type: "GET",
-            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Et.protocol),
+            isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": $t,
+                "*": It,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
                 xml: /\bxml\b/,
@@ -2773,45 +2790,45 @@
                 text: "responseText",
                 json: "responseJSON"
             },
             converters: {
                 "* text": String,
                 "text html": !0,
                 "text json": JSON.parse,
-                "text xml": k.parseXML
+                "text xml": S.parseXML
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(e, t) {
-            return t ? zt(zt(e, k.ajaxSettings), t) : zt(k.ajaxSettings, e)
+            return t ? $t($t(e, S.ajaxSettings), t) : $t(S.ajaxSettings, e)
         },
-        ajaxPrefilter: Bt(It),
-        ajaxTransport: Bt(Wt),
+        ajaxPrefilter: Ft(Rt),
+        ajaxTransport: Ft(Mt),
         ajax: function(e, t) {
             "object" == typeof e && (t = e, e = void 0), t = t || {};
-            var c, f, p, n, d, r, h, g, i, o, v = k.ajaxSetup({}, t),
+            var c, f, p, n, d, r, h, g, i, o, v = S.ajaxSetup({}, t),
                 y = v.context || v,
-                m = v.context && (y.nodeType || y.jquery) ? k(y) : k.event,
-                x = k.Deferred(),
-                b = k.Callbacks("once memory"),
+                m = v.context && (y.nodeType || y.jquery) ? S(y) : S.event,
+                x = S.Deferred(),
+                b = S.Callbacks("once memory"),
                 w = v.statusCode || {},
                 a = {},
                 s = {},
                 u = "canceled",
                 T = {
                     readyState: 0,
                     getResponseHeader: function(e) {
                         var t;
                         if (h) {
                             if (!n) {
                                 n = {};
-                                while (t = Pt.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
+                                while (t = Ht.exec(p)) n[t[1].toLowerCase() + " "] = (n[t[1].toLowerCase() + " "] || []).concat(t[2])
                             }
                             t = n[e.toLowerCase() + " "]
                         }
                         return null == t ? null : t.join(", ")
                     },
                     getAllResponseHeaders: function() {
                         return h ? p : null
@@ -2831,26 +2848,26 @@
                         return this
                     },
                     abort: function(e) {
                         var t = e || u;
                         return c && c.abort(t), l(0, t), this
                     }
                 };
-            if (x.promise(T), v.url = ((e || v.url || Et.href) + "").replace(Mt, Et.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(R) || [""], null == v.crossDomain) {
+            if (x.promise(T), v.url = ((e || v.url || Tt.href) + "").replace(Pt, Tt.protocol + "//"), v.type = t.method || t.type || v.method || v.type, v.dataTypes = (v.dataType || "*").toLowerCase().match(P) || [""], null == v.crossDomain) {
                 r = E.createElement("a");
                 try {
-                    r.href = v.url, r.href = r.href, v.crossDomain = Ft.protocol + "//" + Ft.host != r.protocol + "//" + r.host
+                    r.href = v.url, r.href = r.href, v.crossDomain = Wt.protocol + "//" + Wt.host != r.protocol + "//" + r.host
                 } catch (e) {
                     v.crossDomain = !0
                 }
             }
-            if (v.data && v.processData && "string" != typeof v.data && (v.data = k.param(v.data, v.traditional)), _t(It, v, t, T), h) return T;
-            for (i in (g = k.event && v.global) && 0 == k.active++ && k.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Rt.test(v.type), f = v.url.replace(Ht, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(Lt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (St.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Ot, "$1"), o = (St.test(f) ? "&" : "?") + "_=" + kt++ + o), v.url = f + o), v.ifModified && (k.lastModified[f] && T.setRequestHeader("If-Modified-Since", k.lastModified[f]), k.etag[f] && T.setRequestHeader("If-None-Match", k.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + $t + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
+            if (v.data && v.processData && "string" != typeof v.data && (v.data = S.param(v.data, v.traditional)), Bt(Rt, v, t, T), h) return T;
+            for (i in (g = S.event && v.global) && 0 == S.active++ && S.event.trigger("ajaxStart"), v.type = v.type.toUpperCase(), v.hasContent = !Ot.test(v.type), f = v.url.replace(qt, ""), v.hasContent ? v.data && v.processData && 0 === (v.contentType || "").indexOf("application/x-www-form-urlencoded") && (v.data = v.data.replace(jt, "+")) : (o = v.url.slice(f.length), v.data && (v.processData || "string" == typeof v.data) && (f += (Et.test(f) ? "&" : "?") + v.data, delete v.data), !1 === v.cache && (f = f.replace(Lt, "$1"), o = (Et.test(f) ? "&" : "?") + "_=" + Ct.guid++ + o), v.url = f + o), v.ifModified && (S.lastModified[f] && T.setRequestHeader("If-Modified-Since", S.lastModified[f]), S.etag[f] && T.setRequestHeader("If-None-Match", S.etag[f])), (v.data && v.hasContent && !1 !== v.contentType || t.contentType) && T.setRequestHeader("Content-Type", v.contentType), T.setRequestHeader("Accept", v.dataTypes[0] && v.accepts[v.dataTypes[0]] ? v.accepts[v.dataTypes[0]] + ("*" !== v.dataTypes[0] ? ", " + It + "; q=0.01" : "") : v.accepts["*"]), v.headers) T.setRequestHeader(i, v.headers[i]);
             if (v.beforeSend && (!1 === v.beforeSend.call(y, T, v) || h)) return T.abort();
-            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = _t(Wt, v, t, T)) {
+            if (u = "abort", b.add(v.complete), T.done(v.success), T.fail(v.error), c = Bt(Mt, v, t, T)) {
                 if (T.readyState = 1, g && m.trigger("ajaxSend", [T, v]), h) return T;
                 v.async && 0 < v.timeout && (d = C.setTimeout(function() {
                     T.abort("timeout")
                 }, v.timeout));
                 try {
                     h = !1, c.send(a, l)
                 } catch (e) {
@@ -2878,15 +2895,15 @@
                                 break
                             }
                             a || (a = i)
                         }
                         o = o || a
                     }
                     if (o) return o !== u[0] && u.unshift(o), n[o]
-                }(v, T, n)), s = function(e, t, n, r) {
+                }(v, T, n)), !i && -1 < S.inArray("script", v.dataTypes) && (v.converters["text script"] = function() {}), s = function(e, t, n, r) {
                     var i, o, a, s, u, l = {},
                         c = e.dataTypes.slice();
                     if (c[1])
                         for (a in e.converters) l[a.toLowerCase()] = e.converters[a];
                     o = c.shift();
                     while (o)
                         if (e.responseFields[o] && (n[e.responseFields[o]] = t), !u && r && e.dataFilter && (t = e.dataFilter(t, e.dataType)), u = o, o = c.shift())
@@ -2908,103 +2925,106 @@
                                 }
                             }
                     }
                     return {
                         state: "success",
                         data: t
                     }
-                }(v, s, T, i), i ? (v.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (k.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (k.etag[f] = u)), 204 === e || "HEAD" === v.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(y, [o, l, T]) : x.rejectWith(y, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, v, i ? o : a]), b.fireWith(y, [T, l]), g && (m.trigger("ajaxComplete", [T, v]), --k.active || k.event.trigger("ajaxStop")))
+                }(v, s, T, i), i ? (v.ifModified && ((u = T.getResponseHeader("Last-Modified")) && (S.lastModified[f] = u), (u = T.getResponseHeader("etag")) && (S.etag[f] = u)), 204 === e || "HEAD" === v.type ? l = "nocontent" : 304 === e ? l = "notmodified" : (l = s.state, o = s.data, i = !(a = s.error))) : (a = l, !e && l || (l = "error", e < 0 && (e = 0))), T.status = e, T.statusText = (t || l) + "", i ? x.resolveWith(y, [o, l, T]) : x.rejectWith(y, [T, l, a]), T.statusCode(w), w = void 0, g && m.trigger(i ? "ajaxSuccess" : "ajaxError", [T, v, i ? o : a]), b.fireWith(y, [T, l]), g && (m.trigger("ajaxComplete", [T, v]), --S.active || S.event.trigger("ajaxStop")))
             }
             return T
         },
         getJSON: function(e, t, n) {
-            return k.get(e, t, n, "json")
+            return S.get(e, t, n, "json")
         },
         getScript: function(e, t) {
-            return k.get(e, void 0, t, "script")
+            return S.get(e, void 0, t, "script")
         }
-    }), k.each(["get", "post"], function(e, i) {
-        k[i] = function(e, t, n, r) {
-            return m(t) && (r = r || n, n = t, t = void 0), k.ajax(k.extend({
+    }), S.each(["get", "post"], function(e, i) {
+        S[i] = function(e, t, n, r) {
+            return m(t) && (r = r || n, n = t, t = void 0), S.ajax(S.extend({
                 url: e,
                 type: i,
                 dataType: r,
                 data: t,
                 success: n
-            }, k.isPlainObject(e) && e))
+            }, S.isPlainObject(e) && e))
         }
-    }), k._evalUrl = function(e, t) {
-        return k.ajax({
+    }), S.ajaxPrefilter(function(e) {
+        var t;
+        for (t in e.headers) "content-type" === t.toLowerCase() && (e.contentType = e.headers[t] || "")
+    }), S._evalUrl = function(e, t, n) {
+        return S.ajax({
             url: e,
             type: "GET",
             dataType: "script",
             cache: !0,
             async: !1,
             global: !1,
             converters: {
                 "text script": function() {}
             },
             dataFilter: function(e) {
-                k.globalEval(e, t)
+                S.globalEval(e, t, n)
             }
         })
-    }, k.fn.extend({
+    }, S.fn.extend({
         wrapAll: function(e) {
             var t;
-            return this[0] && (m(e) && (e = e.call(this[0])), t = k(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
+            return this[0] && (m(e) && (e = e.call(this[0])), t = S(e, this[0].ownerDocument).eq(0).clone(!0), this[0].parentNode && t.insertBefore(this[0]), t.map(function() {
                 var e = this;
                 while (e.firstElementChild) e = e.firstElementChild;
                 return e
             }).append(this)), this
         },
         wrapInner: function(n) {
             return m(n) ? this.each(function(e) {
-                k(this).wrapInner(n.call(this, e))
+                S(this).wrapInner(n.call(this, e))
             }) : this.each(function() {
-                var e = k(this),
+                var e = S(this),
                     t = e.contents();
                 t.length ? t.wrapAll(n) : e.append(n)
             })
         },
         wrap: function(t) {
             var n = m(t);
             return this.each(function(e) {
-                k(this).wrapAll(n ? t.call(this, e) : t)
+                S(this).wrapAll(n ? t.call(this, e) : t)
             })
         },
         unwrap: function(e) {
             return this.parent(e).not("body").each(function() {
-                k(this).replaceWith(this.childNodes)
+                S(this).replaceWith(this.childNodes)
             }), this
         }
-    }), k.expr.pseudos.hidden = function(e) {
-        return !k.expr.pseudos.visible(e)
-    }, k.expr.pseudos.visible = function(e) {
+    }), S.expr.pseudos.hidden = function(e) {
+        return !S.expr.pseudos.visible(e)
+    }, S.expr.pseudos.visible = function(e) {
         return !!(e.offsetWidth || e.offsetHeight || e.getClientRects().length)
-    }, k.ajaxSettings.xhr = function() {
+    }, S.ajaxSettings.xhr = function() {
         try {
             return new C.XMLHttpRequest
         } catch (e) {}
     };
-    var Ut = {
+    var _t = {
             0: 200,
             1223: 204
         },
-        Xt = k.ajaxSettings.xhr();
-    y.cors = !!Xt && "withCredentials" in Xt, y.ajax = Xt = !!Xt, k.ajaxTransport(function(i) {
+        zt = S.ajaxSettings.xhr();
+    y.cors = !!zt && "withCredentials" in zt, y.ajax = zt = !!zt, S.ajaxTransport(function(i) {
         var o, a;
-        if (y.cors || Xt && !i.crossDomain) return {
+        if (y.cors || zt && !i.crossDomain) return {
             send: function(e, t) {
                 var n, r = i.xhr();
                 if (r.open(i.type, i.url, i.async, i.username, i.password), i.xhrFields)
                     for (n in i.xhrFields) r[n] = i.xhrFields[n];
                 for (n in i.mimeType && r.overrideMimeType && r.overrideMimeType(i.mimeType), i.crossDomain || e["X-Requested-With"] || (e["X-Requested-With"] = "XMLHttpRequest"), e) r.setRequestHeader(n, e[n]);
                 o = function(e) {
                     return function() {
-                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(Ut[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
+                        o && (o = a = r.onload = r.onerror = r.onabort = r.ontimeout = r.onreadystatechange = null, "abort" === e ? r.abort() : "error" === e ? "number" != typeof r.status ? t(0, "error") : t(r.status, r.statusText) : t(_t[r.status] || r.status, r.statusText, "text" !== (r.responseType || "text") || "string" != typeof r.responseText ? {
                             binary: r.response
                         } : {
                             text: r.responseText
                         }, r.getAllResponseHeaders()))
                     }
                 }, r.onload = o(), a = r.onerror = r.ontimeout = o("error"), void 0 !== r.onabort ? r.onabort = a : r.onreadystatechange = function() {
                     4 === r.readyState && C.setTimeout(function() {
@@ -3017,100 +3037,96 @@
                     if (o) throw e
                 }
             },
             abort: function() {
                 o && o()
             }
         }
-    }), k.ajaxPrefilter(function(e) {
+    }), S.ajaxPrefilter(function(e) {
         e.crossDomain && (e.contents.script = !1)
-    }), k.ajaxSetup({
+    }), S.ajaxSetup({
         accepts: {
             script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
         },
         contents: {
             script: /\b(?:java|ecma)script\b/
         },
         converters: {
             "text script": function(e) {
-                return k.globalEval(e), e
+                return S.globalEval(e), e
             }
         }
-    }), k.ajaxPrefilter("script", function(e) {
+    }), S.ajaxPrefilter("script", function(e) {
         void 0 === e.cache && (e.cache = !1), e.crossDomain && (e.type = "GET")
-    }), k.ajaxTransport("script", function(n) {
+    }), S.ajaxTransport("script", function(n) {
         var r, i;
         if (n.crossDomain || n.scriptAttrs) return {
             send: function(e, t) {
-                r = k("<script>").attr(n.scriptAttrs || {}).prop({
+                r = S("<script>").attr(n.scriptAttrs || {}).prop({
                     charset: n.scriptCharset,
                     src: n.url
                 }).on("load error", i = function(e) {
                     r.remove(), i = null, e && t("error" === e.type ? 404 : 200, e.type)
                 }), E.head.appendChild(r[0])
             },
             abort: function() {
                 i && i()
             }
         }
     });
-    var Vt, Gt = [],
-        Yt = /(=)\?(?=&|$)|\?\?/;
-    k.ajaxSetup({
+    var Ut, Xt = [],
+        Vt = /(=)\?(?=&|$)|\?\?/;
+    S.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var e = Gt.pop() || k.expando + "_" + kt++;
+            var e = Xt.pop() || S.expando + "_" + Ct.guid++;
             return this[e] = !0, e
         }
-    }), k.ajaxPrefilter("json jsonp", function(e, t, n) {
-        var r, i, o, a = !1 !== e.jsonp && (Yt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Yt.test(e.data) && "data");
-        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Yt, "$1" + r) : !1 !== e.jsonp && (e.url += (St.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
-            return o || k.error(r + " was not called"), o[0]
+    }), S.ajaxPrefilter("json jsonp", function(e, t, n) {
+        var r, i, o, a = !1 !== e.jsonp && (Vt.test(e.url) ? "url" : "string" == typeof e.data && 0 === (e.contentType || "").indexOf("application/x-www-form-urlencoded") && Vt.test(e.data) && "data");
+        if (a || "jsonp" === e.dataTypes[0]) return r = e.jsonpCallback = m(e.jsonpCallback) ? e.jsonpCallback() : e.jsonpCallback, a ? e[a] = e[a].replace(Vt, "$1" + r) : !1 !== e.jsonp && (e.url += (Et.test(e.url) ? "&" : "?") + e.jsonp + "=" + r), e.converters["script json"] = function() {
+            return o || S.error(r + " was not called"), o[0]
         }, e.dataTypes[0] = "json", i = C[r], C[r] = function() {
             o = arguments
         }, n.always(function() {
-            void 0 === i ? k(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Gt.push(r)), o && m(i) && i(o[0]), o = i = void 0
+            void 0 === i ? S(C).removeProp(r) : C[r] = i, e[r] && (e.jsonpCallback = t.jsonpCallback, Xt.push(r)), o && m(i) && i(o[0]), o = i = void 0
         }), "script"
-    }), y.createHTMLDocument = ((Vt = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Vt.childNodes.length), k.parseHTML = function(e, t, n) {
-        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = D.exec(e)) ? [t.createElement(i[1])] : (i = we([e], t, o), o && o.length && k(o).remove(), k.merge([], i.childNodes)));
+    }), y.createHTMLDocument = ((Ut = E.implementation.createHTMLDocument("").body).innerHTML = "<form></form><form></form>", 2 === Ut.childNodes.length), S.parseHTML = function(e, t, n) {
+        return "string" != typeof e ? [] : ("boolean" == typeof t && (n = t, t = !1), t || (y.createHTMLDocument ? ((r = (t = E.implementation.createHTMLDocument("")).createElement("base")).href = E.location.href, t.head.appendChild(r)) : t = E), o = !n && [], (i = N.exec(e)) ? [t.createElement(i[1])] : (i = xe([e], t, o), o && o.length && S(o).remove(), S.merge([], i.childNodes)));
         var r, i, o
-    }, k.fn.load = function(e, t, n) {
+    }, S.fn.load = function(e, t, n) {
         var r, i, o, a = this,
             s = e.indexOf(" ");
-        return -1 < s && (r = mt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && k.ajax({
+        return -1 < s && (r = vt(e.slice(s)), e = e.slice(0, s)), m(t) ? (n = t, t = void 0) : t && "object" == typeof t && (i = "POST"), 0 < a.length && S.ajax({
             url: e,
             type: i || "GET",
             dataType: "html",
             data: t
         }).done(function(e) {
-            o = arguments, a.html(r ? k("<div>").append(k.parseHTML(e)).find(r) : e)
+            o = arguments, a.html(r ? S("<div>").append(S.parseHTML(e)).find(r) : e)
         }).always(n && function(e, t) {
             a.each(function() {
                 n.apply(this, o || [e.responseText, t, e])
             })
         }), this
-    }, k.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
-        k.fn[t] = function(e) {
-            return this.on(t, e)
-        }
-    }), k.expr.pseudos.animated = function(t) {
-        return k.grep(k.timers, function(e) {
+    }, S.expr.pseudos.animated = function(t) {
+        return S.grep(S.timers, function(e) {
             return t === e.elem
         }).length
-    }, k.offset = {
+    }, S.offset = {
         setOffset: function(e, t, n) {
-            var r, i, o, a, s, u, l = k.css(e, "position"),
-                c = k(e),
+            var r, i, o, a, s, u, l = S.css(e, "position"),
+                c = S(e),
                 f = {};
-            "static" === l && (e.style.position = "relative"), s = c.offset(), o = k.css(e, "top"), u = k.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, k.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : c.css(f)
+            "static" === l && (e.style.position = "relative"), s = c.offset(), o = S.css(e, "top"), u = S.css(e, "left"), ("absolute" === l || "fixed" === l) && -1 < (o + u).indexOf("auto") ? (a = (r = c.position()).top, i = r.left) : (a = parseFloat(o) || 0, i = parseFloat(u) || 0), m(t) && (t = t.call(e, n, S.extend({}, s))), null != t.top && (f.top = t.top - s.top + a), null != t.left && (f.left = t.left - s.left + i), "using" in t ? t.using.call(e, f) : ("number" == typeof f.top && (f.top += "px"), "number" == typeof f.left && (f.left += "px"), c.css(f))
         }
-    }, k.fn.extend({
+    }, S.fn.extend({
         offset: function(t) {
             if (arguments.length) return void 0 === t ? this : this.each(function(e) {
-                k.offset.setOffset(this, t, e)
+                S.offset.setOffset(this, t, e)
             });
             var e, n, r = this[0];
             return r ? r.getClientRects().length ? (e = r.getBoundingClientRect(), n = r.ownerDocument.defaultView, {
                 top: e.top + n.pageYOffset,
                 left: e.left + n.pageXOffset
             }) : {
                 top: 0,
@@ -3120,100 +3136,107 @@
         position: function() {
             if (this[0]) {
                 var e, t, n, r = this[0],
                     i = {
                         top: 0,
                         left: 0
                     };
-                if ("fixed" === k.css(r, "position")) t = r.getBoundingClientRect();
+                if ("fixed" === S.css(r, "position")) t = r.getBoundingClientRect();
                 else {
                     t = this.offset(), n = r.ownerDocument, e = r.offsetParent || n.documentElement;
-                    while (e && (e === n.body || e === n.documentElement) && "static" === k.css(e, "position")) e = e.parentNode;
-                    e && e !== r && 1 === e.nodeType && ((i = k(e).offset()).top += k.css(e, "borderTopWidth", !0), i.left += k.css(e, "borderLeftWidth", !0))
+                    while (e && (e === n.body || e === n.documentElement) && "static" === S.css(e, "position")) e = e.parentNode;
+                    e && e !== r && 1 === e.nodeType && ((i = S(e).offset()).top += S.css(e, "borderTopWidth", !0), i.left += S.css(e, "borderLeftWidth", !0))
                 }
                 return {
-                    top: t.top - i.top - k.css(r, "marginTop", !0),
-                    left: t.left - i.left - k.css(r, "marginLeft", !0)
+                    top: t.top - i.top - S.css(r, "marginTop", !0),
+                    left: t.left - i.left - S.css(r, "marginLeft", !0)
                 }
             }
         },
         offsetParent: function() {
             return this.map(function() {
                 var e = this.offsetParent;
-                while (e && "static" === k.css(e, "position")) e = e.offsetParent;
-                return e || ie
+                while (e && "static" === S.css(e, "position")) e = e.offsetParent;
+                return e || re
             })
         }
-    }), k.each({
+    }), S.each({
         scrollLeft: "pageXOffset",
         scrollTop: "pageYOffset"
     }, function(t, i) {
         var o = "pageYOffset" === i;
-        k.fn[t] = function(e) {
-            return _(this, function(e, t, n) {
+        S.fn[t] = function(e) {
+            return $(this, function(e, t, n) {
                 var r;
                 if (x(e) ? r = e : 9 === e.nodeType && (r = e.defaultView), void 0 === n) return r ? r[i] : e[t];
                 r ? r.scrollTo(o ? r.pageXOffset : n, o ? n : r.pageYOffset) : e[t] = n
             }, t, e, arguments.length)
         }
-    }), k.each(["top", "left"], function(e, n) {
-        k.cssHooks[n] = ze(y.pixelPosition, function(e, t) {
-            if (t) return t = _e(e, n), $e.test(t) ? k(e).position()[n] + "px" : t
+    }), S.each(["top", "left"], function(e, n) {
+        S.cssHooks[n] = $e(y.pixelPosition, function(e, t) {
+            if (t) return t = Be(e, n), Me.test(t) ? S(e).position()[n] + "px" : t
         })
-    }), k.each({
+    }), S.each({
         Height: "height",
         Width: "width"
     }, function(a, s) {
-        k.each({
+        S.each({
             padding: "inner" + a,
             content: s,
             "": "outer" + a
         }, function(r, o) {
-            k.fn[o] = function(e, t) {
+            S.fn[o] = function(e, t) {
                 var n = arguments.length && (r || "boolean" != typeof e),
                     i = r || (!0 === e || !0 === t ? "margin" : "border");
-                return _(this, function(e, t, n) {
+                return $(this, function(e, t, n) {
                     var r;
-                    return x(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? k.css(e, t, i) : k.style(e, t, n, i)
+                    return x(e) ? 0 === o.indexOf("outer") ? e["inner" + a] : e.document.documentElement["client" + a] : 9 === e.nodeType ? (r = e.documentElement, Math.max(e.body["scroll" + a], r["scroll" + a], e.body["offset" + a], r["offset" + a], r["client" + a])) : void 0 === n ? S.css(e, t, i) : S.style(e, t, n, i)
                 }, s, n ? e : void 0, n)
             }
         })
-    }), k.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
-        k.fn[n] = function(e, t) {
-            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
-        }
-    }), k.fn.extend({
-        hover: function(e, t) {
-            return this.mouseenter(e).mouseleave(t || e)
+    }), S.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(e, t) {
+        S.fn[t] = function(e) {
+            return this.on(t, e)
         }
-    }), k.fn.extend({
+    }), S.fn.extend({
         bind: function(e, t, n) {
             return this.on(e, null, t, n)
         },
         unbind: function(e, t) {
             return this.off(e, null, t)
         },
         delegate: function(e, t, n, r) {
             return this.on(t, e, n, r)
         },
         undelegate: function(e, t, n) {
             return 1 === arguments.length ? this.off(e, "**") : this.off(t, e || "**", n)
+        },
+        hover: function(e, t) {
+            return this.mouseenter(e).mouseleave(t || e)
         }
-    }), k.proxy = function(e, t) {
+    }), S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "), function(e, n) {
+        S.fn[n] = function(e, t) {
+            return 0 < arguments.length ? this.on(n, null, e, t) : this.trigger(n)
+        }
+    });
+    var Gt = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;
+    S.proxy = function(e, t) {
         var n, r, i;
         if ("string" == typeof t && (n = e[t], t = e, e = n), m(e)) return r = s.call(arguments, 2), (i = function() {
             return e.apply(t || this, r.concat(s.call(arguments)))
-        }).guid = e.guid = e.guid || k.guid++, i
-    }, k.holdReady = function(e) {
-        e ? k.readyWait++ : k.ready(!0)
-    }, k.isArray = Array.isArray, k.parseJSON = JSON.parse, k.nodeName = A, k.isFunction = m, k.isWindow = x, k.camelCase = V, k.type = w, k.now = Date.now, k.isNumeric = function(e) {
-        var t = k.type(e);
+        }).guid = e.guid = e.guid || S.guid++, i
+    }, S.holdReady = function(e) {
+        e ? S.readyWait++ : S.ready(!0)
+    }, S.isArray = Array.isArray, S.parseJSON = JSON.parse, S.nodeName = A, S.isFunction = m, S.isWindow = x, S.camelCase = X, S.type = w, S.now = Date.now, S.isNumeric = function(e) {
+        var t = S.type(e);
         return ("number" === t || "string" === t) && !isNaN(e - parseFloat(e))
+    }, S.trim = function(e) {
+        return null == e ? "" : (e + "").replace(Gt, "")
     }, "function" == typeof define && define.amd && define("jquery", [], function() {
-        return k
+        return S
     });
-    var Qt = C.jQuery,
-        Jt = C.$;
-    return k.noConflict = function(e) {
-        return C.$ === k && (C.$ = Jt), e && C.jQuery === k && (C.jQuery = Qt), k
-    }, e || (C.jQuery = C.$ = k), k
+    var Yt = C.jQuery,
+        Qt = C.$;
+    return S.noConflict = function(e) {
+        return C.$ === S && (C.$ = Qt), e && C.jQuery === S && (C.jQuery = Yt), S
+    }, "undefined" == typeof e && (C.jQuery = C.$ = S), S
 });
```

### Comparing `CLAM-3.2.5/clam/static/jquery.dataTables.min.css` & `CLAM-3.2.6/clam/static/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/jquery.dataTables.min.js` & `CLAM-3.2.6/clam/static/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/jquery.fine-uploader.js` & `CLAM-3.2.6/clam/static/jquery.fine-uploader.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/jquery.fine-uploader.min.js` & `CLAM-3.2.6/clam/static/jquery.fine-uploader.min.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/jquery.fineuploader-3.1.js` & `CLAM-3.2.6/clam/static/jquery.fineuploader-3.1.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/jquery.fineuploader-3.1.min.js` & `CLAM-3.2.6/clam/static/jquery.fineuploader-3.1.min.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/loading.gif` & `CLAM-3.2.6/clam/static/loading.gif`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/login.xsl` & `CLAM-3.2.6/clam/static/login.xsl`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/open-iconic-bootstrap.min.css` & `CLAM-3.2.6/clam/static/open-iconic-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/open-iconic.eot` & `CLAM-3.2.6/clam/static/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/open-iconic.otf` & `CLAM-3.2.6/clam/static/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/open-iconic.svg` & `CLAM-3.2.6/clam/static/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/open-iconic.ttf` & `CLAM-3.2.6/clam/static/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/open-iconic.woff` & `CLAM-3.2.6/clam/static/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/parameters.xsl` & `CLAM-3.2.6/clam/static/parameters.xsl`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/popper.min.js` & `CLAM-3.2.6/clam/static/popper.min.js`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/processing.gif` & `CLAM-3.2.6/clam/static/processing.gif`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/progress.gif` & `CLAM-3.2.6/clam/static/progress.gif`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/sonar.css` & `CLAM-3.2.6/clam/static/sonar.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/tableimages/Sorting icons.psd` & `CLAM-3.2.6/clam/static/tableimages/Sorting icons.psd`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/tableimages/back_disabled.jpg` & `CLAM-3.2.6/clam/static/tableimages/back_disabled.jpg`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/tableimages/back_enabled.jpg` & `CLAM-3.2.6/clam/static/tableimages/back_enabled.jpg`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/tableimages/forward_disabled.jpg` & `CLAM-3.2.6/clam/static/tableimages/forward_disabled.jpg`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/static/tableimages/forward_enabled.jpg` & `CLAM-3.2.6/clam/static/tableimages/forward_enabled.jpg`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/style/classic.css` & `CLAM-3.2.6/clam/style/classic.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/style/pre2.css` & `CLAM-3.2.6/clam/style/pre2.css`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/templates/admin.html` & `CLAM-3.2.6/clam/templates/admin.html`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/templates/admininspect.html` & `CLAM-3.2.6/clam/templates/admininspect.html`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/templates/crudetableviewer.html` & `CLAM-3.2.6/clam/templates/crudetableviewer.html`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/templates/response.json` & `CLAM-3.2.6/clam/templates/response.json`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/templates/response.xml` & `CLAM-3.2.6/clam/templates/response.xml`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/templates/share.html` & `CLAM-3.2.6/clam/templates/share.html`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/actiontest.py` & `CLAM-3.2.6/clam/tests/actiontest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/authactiontest.py` & `CLAM-3.2.6/clam/tests/authactiontest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/authtest.py` & `CLAM-3.2.6/clam/tests/authtest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/constrainttest.py` & `CLAM-3.2.6/clam/tests/constrainttest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/datatest.py` & `CLAM-3.2.6/clam/tests/datatest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/frogclient.py` & `CLAM-3.2.6/clam/tests/frogclient.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/parametertest.py` & `CLAM-3.2.6/clam/tests/parametertest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/tests/servicetest.py` & `CLAM-3.2.6/clam/tests/servicetest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/wrappers/constrainttest.py` & `CLAM-3.2.6/clam/wrappers/constrainttest.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/wrappers/freqlistwrapper.py` & `CLAM-3.2.6/clam/wrappers/freqlistwrapper.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/wrappers/template.py` & `CLAM-3.2.6/clam/wrappers/template.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/wrappers/template.sh` & `CLAM-3.2.6/clam/wrappers/template.sh`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/wrappers/testwrapper.py` & `CLAM-3.2.6/clam/wrappers/testwrapper.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/clam/wrappers/textstats.py` & `CLAM-3.2.6/clam/wrappers/textstats.py`

 * *Files identical despite different names*

### Comparing `CLAM-3.2.5/codemeta.json` & `CLAM-3.2.6/codemeta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'dateModified'": "'2023-05-01'", "'version'": "'3.2.6'"}*

```diff
@@ -16,15 +16,15 @@
             "familyName": "van Gompel",
             "givenName": "Maarten"
         }
     ],
     "codeRepository": "https://github.com/proycon/clam",
     "contIntegration": "https://github.com/proycon/clam/actions/workflows/clam.yml",
     "dateCreated": "2010-03-21",
-    "dateModified": "2023-03-01",
+    "dateModified": "2023-05-01",
     "description": "Quickly turn command-line applications into RESTful webservices with a web-application front-end. You provide a specification of your command line application, its input, output and parameters, and CLAM wraps around your application to form a fully fledged RESTful webservice. ",
     "developmentStatus": [
         "https://www.repostatus.org/#active",
         "https://w3id.org/research-technology-readiness-levels#Level9Proven"
     ],
     "funding": [
         {
@@ -201,9 +201,9 @@
                 "Linux",
                 "BSD",
                 "macOS"
             ]
         }
     ],
     "url": "https://proycon.github.io/clam",
-    "version": "3.2.5"
+    "version": "3.2.6"
 }
```

### Comparing `CLAM-3.2.5/setup.py` & `CLAM-3.2.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def read(fname):
     return io.open(os.path.join(os.path.dirname(__file__), fname),'r',encoding='utf-8').read()
 
 
 setup(
     name = "CLAM",
-    version = "3.2.5", #also change in clam.common.data.VERSION and dispatcher.py and codemeta.json
+    version = "3.2.6", #also change in clam.common.data.VERSION and dispatcher.py and codemeta.json
     author = "Maarten van Gompel",
     author_email = "proycon@anaproy.nl",
     description = ("Turns command-line tools into fully-fledged RESTful webservices with an auto-generated web-interface for human end-users."),
     license = "GPL-3.0-only",
     keywords = ["SaaS", "webservice", "rest"],
     url = "https://proycon.github.io/clam",
     packages=['clam','clam.common','clam.config','clam.wrappers'],
```

