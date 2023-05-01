# Comparing `tmp/cinemagoer-2022.2.11.tar.gz` & `tmp/cinemagoer-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cinemagoer-2022.2.11.tar", last modified: Fri Feb 11 07:26:45 2022, max compression
+gzip compressed data, was "cinemagoer-2023.5.1.tar", last modified: Mon May  1 13:41:20 2023, max compression
```

## Comparing `cinemagoer-2022.2.11.tar` & `cinemagoer-2023.5.1.tar`

### file list

```diff
@@ -1,165 +1,163 @@
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.412346 cinemagoer-2022.2.11/
--rw-rw-r--   0 da        (1000) da        (1000)    57361 2022-02-11 07:25:19.000000 cinemagoer-2022.2.11/CHANGELOG.txt
--rw-rw-r--   0 da        (1000) da        (1000)     1911 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/CONTRIBUTORS.txt
--rw-rw-r--   0 da        (1000) da        (1000)    13818 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/CREDITS.txt
--rw-rw-r--   0 da        (1000) da        (1000)      482 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/DISCLAIMER.txt
--rw-rw-r--   0 da        (1000) da        (1000)    18092 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/LICENSE.txt
--rw-rw-r--   0 da        (1000) da        (1000)      422 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/MANIFEST.in
--rw-rw-r--   0 da        (1000) da        (1000)     2525 2022-02-11 07:26:45.412346 cinemagoer-2022.2.11/PKG-INFO
--rw-rw-r--   0 da        (1000) da        (1000)     3704 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/README.rst
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.400346 cinemagoer-2022.2.11/bin/
--rwxrwxr-x   0 da        (1000) da        (1000)     1472 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_company.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1114 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_first_company.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1113 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_first_movie.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1103 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_first_person.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1111 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_keyword.py
--rwxrwxr-x   0 da        (1000) da        (1000)     3336 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_movie.py
--rwxrwxr-x   0 da        (1000) da        (1000)      952 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_movie_list.py
--rwxrwxr-x   0 da        (1000) da        (1000)     2782 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_person.py
--rwxrwxr-x   0 da        (1000) da        (1000)      809 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/get_top_bottom_movies.py
--rwxrwxr-x   0 da        (1000) da        (1000)   115020 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/bin/imdbpy2sql.py
--rwxrwxr-x   0 da        (1000) da        (1000)     6627 2022-02-11 06:58:36.000000 cinemagoer-2022.2.11/bin/s32cinemagoer.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1260 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/search_company.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1167 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/search_keyword.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1239 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/search_movie.py
--rwxrwxr-x   0 da        (1000) da        (1000)     1243 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/bin/search_person.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.400346 cinemagoer-2022.2.11/cinemagoer.egg-info/
--rw-rw-r--   0 da        (1000) da        (1000)     2525 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/cinemagoer.egg-info/PKG-INFO
--rw-rw-r--   0 da        (1000) da        (1000)     3750 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/cinemagoer.egg-info/SOURCES.txt
--rw-rw-r--   0 da        (1000) da        (1000)        1 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/cinemagoer.egg-info/dependency_links.txt
--rw-rw-r--   0 da        (1000) da        (1000)       60 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/cinemagoer.egg-info/entry_points.txt
--rw-rw-r--   0 da        (1000) da        (1000)      133 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/cinemagoer.egg-info/requires.txt
--rw-rw-r--   0 da        (1000) da        (1000)        5 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/cinemagoer.egg-info/top_level.txt
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/
--rw-rw-r--   0 da        (1000) da        (1000)     7142 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/Character.py
--rw-rw-r--   0 da        (1000) da        (1000)     7134 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/Company.py
--rw-rw-r--   0 da        (1000) da        (1000)    13820 2021-12-05 19:21:14.000000 cinemagoer-2022.2.11/imdb/Movie.py
--rw-rw-r--   0 da        (1000) da        (1000)    10914 2020-10-18 07:35:06.000000 cinemagoer-2022.2.11/imdb/Person.py
--rw-rw-r--   0 da        (1000) da        (1000)    47575 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/imdb/__init__.py
--rw-rw-r--   0 da        (1000) da        (1000)     1695 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/_exceptions.py
--rw-rw-r--   0 da        (1000) da        (1000)     1733 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/_logging.py
--rw-rw-r--   0 da        (1000) da        (1000)     6488 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/cli.py
--rw-rw-r--   0 da        (1000) da        (1000)    23476 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/helpers.py
--rw-rw-r--   0 da        (1000) da        (1000)     9486 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/linguistics.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/
--rw-rw-r--   0 da        (1000) da        (1000)     1036 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/__init__.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/ar/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/ar/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)     3041 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/ar/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/bg/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)     5671 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/bg/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/de/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/de/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)    13477 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/de/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/en/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/en/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)    13723 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/en/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/es/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/es/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)    15624 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/es/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/fr/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)     3214 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/fr/LC_MESSAGES/imdbpy.mo
--rwxrwxr-x   0 da        (1000) da        (1000)     2355 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/locale/generatepot.py
--rw-rw-r--   0 da        (1000) da        (1000)    19765 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-ar.po
--rw-rw-r--   0 da        (1000) da        (1000)    21161 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-bg.po
--rw-rw-r--   0 da        (1000) da        (1000)    23174 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-de.po
--rw-rw-r--   0 da        (1000) da        (1000)    21974 2020-05-02 21:08:05.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-en.po
--rw-rw-r--   0 da        (1000) da        (1000)    24257 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-es.po
--rw-rw-r--   0 da        (1000) da        (1000)    19684 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-fr.po
--rw-rw-r--   0 da        (1000) da        (1000)    23271 2020-08-29 14:58:26.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-it.po
--rw-rw-r--   0 da        (1000) da        (1000)    19695 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-pt_BR.po
--rw-rw-r--   0 da        (1000) da        (1000)    25808 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-sr.po
--rw-rw-r--   0 da        (1000) da        (1000)    22303 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy-tr.po
--rw-rw-r--   0 da        (1000) da        (1000)    18867 2020-08-29 14:58:26.000000 cinemagoer-2022.2.11/imdb/locale/imdbpy.pot
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/it/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/it/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)    13779 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/it/LC_MESSAGES/imdbpy.mo
--rw-rw-r--   0 da        (1000) da        (1000)     7064 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/imdb/locale/msgfmt.py
--rw-rw-r--   0 da        (1000) da        (1000)     7329 2017-11-05 11:48:25.000000 cinemagoer-2022.2.11/imdb/locale/msgfmt.pyc
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.396345 cinemagoer-2022.2.11/imdb/locale/pt_BR/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)     2441 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/pt_BR/LC_MESSAGES/imdbpy.mo
--rwxrwxr-x   0 da        (1000) da        (1000)     1450 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/locale/rebuildmo.py
--rw-rw-r--   0 da        (1000) da        (1000)      973 2018-06-24 08:32:45.000000 cinemagoer-2022.2.11/imdb/locale/rebuildmo.pyc
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.400346 cinemagoer-2022.2.11/imdb/locale/sr/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/sr/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)    15935 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/sr/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.400346 cinemagoer-2022.2.11/imdb/locale/tr/
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 da        (1000) da        (1000)    11195 2022-02-11 07:26:45.000000 cinemagoer-2022.2.11/imdb/locale/tr/LC_MESSAGES/imdbpy.mo
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/parser/
--rw-rw-r--   0 da        (1000) da        (1000)     1091 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/__init__.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.404346 cinemagoer-2022.2.11/imdb/parser/http/
--rw-rw-r--   0 da        (1000) da        (1000)    32222 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/imdb/parser/http/__init__.py
--rw-rw-r--   0 da        (1000) da        (1000)     4254 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/companyParser.py
--rw-rw-r--   0 da        (1000) da        (1000)     4108 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/listParser.py
--rw-rw-r--   0 da        (1000) da        (1000)       97 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/logging.py
--rw-rw-r--   0 da        (1000) da        (1000)    96340 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/imdb/parser/http/movieParser.py
--rw-rw-r--   0 da        (1000) da        (1000)    21944 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/personParser.py
--rw-rw-r--   0 da        (1000) da        (1000)    33068 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/piculet.py
--rw-rw-r--   0 da        (1000) da        (1000)     2406 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/searchCompanyParser.py
--rw-rw-r--   0 da        (1000) da        (1000)     3595 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/searchKeywordParser.py
--rw-rw-r--   0 da        (1000) da        (1000)     9746 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/searchMovieAdvancedParser.py
--rw-rw-r--   0 da        (1000) da        (1000)     3706 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/searchMovieParser.py
--rw-rw-r--   0 da        (1000) da        (1000)     2882 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/searchPersonParser.py
--rw-rw-r--   0 da        (1000) da        (1000)     6646 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/imdb/parser/http/topBottomParser.py
--rw-rw-r--   0 da        (1000) da        (1000)    22619 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/http/utils.py
--rw-rw-r--   0 da        (1000) da        (1000)       81 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/logging.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.408346 cinemagoer-2022.2.11/imdb/parser/s3/
--rw-rw-r--   0 da        (1000) da        (1000)    11612 2021-03-19 20:37:37.000000 cinemagoer-2022.2.11/imdb/parser/s3/__init__.py
--rw-rw-r--   0 da        (1000) da        (1000)    12177 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/imdb/parser/s3/utils.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.408346 cinemagoer-2022.2.11/imdb/parser/sql/
--rw-rw-r--   0 da        (1000) da        (1000)    63944 2020-10-11 15:24:58.000000 cinemagoer-2022.2.11/imdb/parser/sql/__init__.py
--rw-rw-r--   0 da        (1000) da        (1000)    16586 2020-10-11 15:24:58.000000 cinemagoer-2022.2.11/imdb/parser/sql/alchemyadapter.py
--rw-rw-r--   0 da        (1000) da        (1000)    19323 2020-10-11 15:24:58.000000 cinemagoer-2022.2.11/imdb/parser/sql/dbschema.py
--rw-rw-r--   0 da        (1000) da        (1000)       96 2020-10-11 15:24:58.000000 cinemagoer-2022.2.11/imdb/parser/sql/logging.py
--rw-rw-r--   0 da        (1000) da        (1000)    60397 2022-01-26 19:52:29.000000 cinemagoer-2022.2.11/imdb/utils.py
--rw-rw-r--   0 da        (1000) da        (1000)       27 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/imdb/version.py
--rw-rw-r--   0 da        (1000) da        (1000)      485 2022-02-11 07:26:45.412346 cinemagoer-2022.2.11/setup.cfg
--rwxrwxr-x   0 da        (1000) da        (1000)     5222 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/setup.py
-drwxrwxr-x   0 da        (1000) da        (1000)        0 2022-02-11 07:26:45.408346 cinemagoer-2022.2.11/tests/
--rw-rw-r--   0 da        (1000) da        (1000)     1204 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/tests/conftest.py
--rw-rw-r--   0 da        (1000) da        (1000)     1303 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_chart_bottom.py
--rw-rw-r--   0 da        (1000) da        (1000)      403 2022-02-11 06:56:56.000000 cinemagoer-2022.2.11/tests/test_http_chart_boxoffice.py
--rw-rw-r--   0 da        (1000) da        (1000)      832 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_chart_popular_movies.py
--rw-rw-r--   0 da        (1000) da        (1000)      764 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_chart_popular_tv.py
--rw-rw-r--   0 da        (1000) da        (1000)     1254 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_chart_top.py
--rw-rw-r--   0 da        (1000) da        (1000)     1164 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_chart_top_indian.py
--rw-rw-r--   0 da        (1000) da        (1000)     1200 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_chart_top_tv.py
--rw-rw-r--   0 da        (1000) da        (1000)      163 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_company_main.py
--rw-rw-r--   0 da        (1000) da        (1000)      416 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_gather_refs.py
--rw-rw-r--   0 da        (1000) da        (1000)      146 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_awards.py
--rw-rw-r--   0 da        (1000) da        (1000)    21139 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_movie_combined.py
--rw-rw-r--   0 da        (1000) da        (1000)      384 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/tests/test_http_movie_connections.py
--rw-rw-r--   0 da        (1000) da        (1000)      688 2021-09-14 15:36:38.000000 cinemagoer-2022.2.11/tests/test_http_movie_full_credit.py
--rw-rw-r--   0 da        (1000) da        (1000)      142 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_goofs.py
--rw-rw-r--   0 da        (1000) da        (1000)      744 2021-12-05 19:21:14.000000 cinemagoer-2022.2.11/tests/test_http_movie_keywords.py
--rw-rw-r--   0 da        (1000) da        (1000)      678 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_list.py
--rw-rw-r--   0 da        (1000) da        (1000)      698 2021-09-14 15:35:00.000000 cinemagoer-2022.2.11/tests/test_http_movie_parental_guide.py
--rw-rw-r--   0 da        (1000) da        (1000)     1030 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/tests/test_http_movie_plot.py
--rw-rw-r--   0 da        (1000) da        (1000)      147 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_quotes.py
--rw-rw-r--   0 da        (1000) da        (1000)      305 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_movie_recommendations.py
--rw-rw-r--   0 da        (1000) da        (1000)      526 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_releaseinfo.py
--rw-rw-r--   0 da        (1000) da        (1000)      345 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_reviews.py
--rw-rw-r--   0 da        (1000) da        (1000)     2956 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_movie_season_episodes.py
--rw-rw-r--   0 da        (1000) da        (1000)      442 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/tests/test_http_movie_series.py
--rw-rw-r--   0 da        (1000) da        (1000)      804 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_movie_sites.py
--rw-rw-r--   0 da        (1000) da        (1000)      696 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_taglines.py
--rw-rw-r--   0 da        (1000) da        (1000)      390 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_tech.py
--rw-rw-r--   0 da        (1000) da        (1000)      595 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/tests/test_http_movie_titles.py
--rw-rw-r--   0 da        (1000) da        (1000)     1465 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_movie_votes.py
--rw-rw-r--   0 da        (1000) da        (1000)      150 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_person_awards.py
--rw-rw-r--   0 da        (1000) da        (1000)     4551 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_person_bio.py
--rw-rw-r--   0 da        (1000) da        (1000)     2429 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_person_main.py
--rw-rw-r--   0 da        (1000) da        (1000)      665 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_person_otherworks.py
--rw-rw-r--   0 da        (1000) da        (1000)     1601 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/tests/test_http_search_company.py
--rw-rw-r--   0 da        (1000) da        (1000)     1048 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_search_keyword.py
--rw-rw-r--   0 da        (1000) da        (1000)     3621 2021-09-09 11:17:12.000000 cinemagoer-2022.2.11/tests/test_http_search_movie.py
--rw-rw-r--   0 da        (1000) da        (1000)    18928 2022-01-25 19:33:15.000000 cinemagoer-2022.2.11/tests/test_http_search_movie_advanced.py
--rw-rw-r--   0 da        (1000) da        (1000)      847 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_search_movie_keyword.py
--rw-rw-r--   0 da        (1000) da        (1000)     2440 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_http_search_person.py
--rw-rw-r--   0 da        (1000) da        (1000)      737 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_in_operator.py
--rw-rw-r--   0 da        (1000) da        (1000)      237 2020-10-18 07:21:34.000000 cinemagoer-2022.2.11/tests/test_xml.py
--rw-rw-r--   0 da        (1000) da        (1000)      349 2021-03-19 20:37:37.000000 cinemagoer-2022.2.11/tox.ini
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.706995 cinemagoer-2023.5.1/
+-rw-rw-r--   0 da        (1000) da        (1000)    58462 2023-05-01 13:40:34.000000 cinemagoer-2023.5.1/CHANGELOG.txt
+-rw-rw-r--   0 da        (1000) da        (1000)     1911 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/CONTRIBUTORS.txt
+-rw-rw-r--   0 da        (1000) da        (1000)      972 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/CREDITS.txt
+-rw-rw-r--   0 da        (1000) da        (1000)      482 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/DISCLAIMER.txt
+-rw-rw-r--   0 da        (1000) da        (1000)    18092 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/LICENSE.txt
+-rw-rw-r--   0 da        (1000) da        (1000)      422 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/MANIFEST.in
+-rw-rw-r--   0 da        (1000) da        (1000)     2552 2023-05-01 13:41:20.706995 cinemagoer-2023.5.1/PKG-INFO
+-rw-rw-r--   0 da        (1000) da        (1000)     3959 2022-12-03 12:26:09.000000 cinemagoer-2023.5.1/README.rst
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.690994 cinemagoer-2023.5.1/bin/
+-rwxrwxr-x   0 da        (1000) da        (1000)     1472 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_company.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1114 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_first_company.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1113 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_first_movie.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1103 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_first_person.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1111 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_keyword.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     3336 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_movie.py
+-rwxrwxr-x   0 da        (1000) da        (1000)      952 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_movie_list.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     2782 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_person.py
+-rwxrwxr-x   0 da        (1000) da        (1000)      809 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/get_top_bottom_movies.py
+-rwxrwxr-x   0 da        (1000) da        (1000)   115020 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/bin/imdbpy2sql.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     6879 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/bin/s32cinemagoer.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1260 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/search_company.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1167 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/search_keyword.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1239 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/search_movie.py
+-rwxrwxr-x   0 da        (1000) da        (1000)     1243 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/bin/search_person.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.690994 cinemagoer-2023.5.1/cinemagoer.egg-info/
+-rw-rw-r--   0 da        (1000) da        (1000)     2552 2023-05-01 13:41:20.000000 cinemagoer-2023.5.1/cinemagoer.egg-info/PKG-INFO
+-rw-rw-r--   0 da        (1000) da        (1000)     3713 2023-05-01 13:41:20.000000 cinemagoer-2023.5.1/cinemagoer.egg-info/SOURCES.txt
+-rw-rw-r--   0 da        (1000) da        (1000)        1 2023-05-01 13:41:20.000000 cinemagoer-2023.5.1/cinemagoer.egg-info/dependency_links.txt
+-rw-rw-r--   0 da        (1000) da        (1000)       41 2023-05-01 13:41:20.000000 cinemagoer-2023.5.1/cinemagoer.egg-info/entry_points.txt
+-rw-rw-r--   0 da        (1000) da        (1000)       96 2023-05-01 13:41:20.000000 cinemagoer-2023.5.1/cinemagoer.egg-info/requires.txt
+-rw-rw-r--   0 da        (1000) da        (1000)        5 2023-05-01 13:41:20.000000 cinemagoer-2023.5.1/cinemagoer.egg-info/top_level.txt
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/
+-rw-rw-r--   0 da        (1000) da        (1000)     7142 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/imdb/Character.py
+-rw-rw-r--   0 da        (1000) da        (1000)     7112 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/Company.py
+-rw-rw-r--   0 da        (1000) da        (1000)    13798 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/Movie.py
+-rw-rw-r--   0 da        (1000) da        (1000)    10915 2023-03-19 12:16:29.000000 cinemagoer-2023.5.1/imdb/Person.py
+-rw-rw-r--   0 da        (1000) da        (1000)    48283 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/imdb/__init__.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1695 2021-05-07 17:54:06.000000 cinemagoer-2023.5.1/imdb/_exceptions.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1732 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/_logging.py
+-rw-rw-r--   0 da        (1000) da        (1000)     6487 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/cli.py
+-rw-rw-r--   0 da        (1000) da        (1000)    23655 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/imdb/helpers.py
+-rw-rw-r--   0 da        (1000) da        (1000)     9486 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/imdb/linguistics.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/locale/
+-rw-rw-r--   0 da        (1000) da        (1000)     1071 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/imdb/locale/__init__.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/ar/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)     3041 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/ar/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/bg/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)     5671 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/bg/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/de/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)    13477 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/de/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/en/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)    13723 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/en/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/es/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.694994 cinemagoer-2023.5.1/imdb/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)    15624 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/es/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/fr/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)     3214 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/fr/LC_MESSAGES/imdbpy.mo
+-rw-rw-r--   0 da        (1000) da        (1000)    19765 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-ar.po
+-rw-rw-r--   0 da        (1000) da        (1000)    21161 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-bg.po
+-rw-rw-r--   0 da        (1000) da        (1000)    23174 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-de.po
+-rw-rw-r--   0 da        (1000) da        (1000)    21974 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-en.po
+-rw-rw-r--   0 da        (1000) da        (1000)    24257 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-es.po
+-rw-rw-r--   0 da        (1000) da        (1000)    19684 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-fr.po
+-rw-rw-r--   0 da        (1000) da        (1000)    23271 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-it.po
+-rw-rw-r--   0 da        (1000) da        (1000)    19695 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-pt_BR.po
+-rw-rw-r--   0 da        (1000) da        (1000)    25808 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-sr.po
+-rw-rw-r--   0 da        (1000) da        (1000)    22303 2022-02-06 11:36:19.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy-tr.po
+-rw-rw-r--   0 da        (1000) da        (1000)    18867 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/locale/imdbpy.pot
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/it/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)    13779 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/it/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/pt_BR/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)     2441 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/pt_BR/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/sr/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/locale/sr/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)    15935 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/sr/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.686994 cinemagoer-2023.5.1/imdb/locale/tr/
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/locale/tr/LC_MESSAGES/
+-rw-rw-r--   0 da        (1000) da        (1000)    11195 2022-10-02 16:03:20.000000 cinemagoer-2023.5.1/imdb/locale/tr/LC_MESSAGES/imdbpy.mo
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/parser/
+-rw-rw-r--   0 da        (1000) da        (1000)     1090 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/__init__.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/parser/http/
+-rw-rw-r--   0 da        (1000) da        (1000)    33163 2023-03-19 12:19:31.000000 cinemagoer-2023.5.1/imdb/parser/http/__init__.py
+-rw-rw-r--   0 da        (1000) da        (1000)     4253 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/http/companyParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     4107 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/http/listParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)       97 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/parser/http/logging.py
+-rw-rw-r--   0 da        (1000) da        (1000)    97147 2023-05-01 13:04:20.000000 cinemagoer-2023.5.1/imdb/parser/http/movieParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)    22403 2023-02-05 13:33:15.000000 cinemagoer-2023.5.1/imdb/parser/http/personParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)    26143 2022-12-03 14:26:18.000000 cinemagoer-2023.5.1/imdb/parser/http/piculet.py
+-rw-rw-r--   0 da        (1000) da        (1000)     2653 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/imdb/parser/http/searchCompanyParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     3659 2022-12-03 12:26:09.000000 cinemagoer-2023.5.1/imdb/parser/http/searchKeywordParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     9760 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/http/searchMovieAdvancedParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     4614 2023-03-19 11:55:02.000000 cinemagoer-2023.5.1/imdb/parser/http/searchMovieParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     2686 2022-12-03 12:26:09.000000 cinemagoer-2023.5.1/imdb/parser/http/searchPersonParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     3702 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/http/showtimesParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)     6646 2022-01-16 16:03:22.000000 cinemagoer-2023.5.1/imdb/parser/http/topBottomParser.py
+-rw-rw-r--   0 da        (1000) da        (1000)    22603 2022-12-08 10:02:56.000000 cinemagoer-2023.5.1/imdb/parser/http/utils.py
+-rw-rw-r--   0 da        (1000) da        (1000)       81 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/parser/logging.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.698994 cinemagoer-2023.5.1/imdb/parser/s3/
+-rw-rw-r--   0 da        (1000) da        (1000)    11613 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/s3/__init__.py
+-rw-rw-r--   0 da        (1000) da        (1000)    12180 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/imdb/parser/s3/utils.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.702994 cinemagoer-2023.5.1/imdb/parser/sql/
+-rw-rw-r--   0 da        (1000) da        (1000)    63944 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/imdb/parser/sql/__init__.py
+-rw-rw-r--   0 da        (1000) da        (1000)    16586 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/imdb/parser/sql/alchemyadapter.py
+-rw-rw-r--   0 da        (1000) da        (1000)    19323 2021-04-18 10:45:56.000000 cinemagoer-2023.5.1/imdb/parser/sql/dbschema.py
+-rw-rw-r--   0 da        (1000) da        (1000)       96 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/imdb/parser/sql/logging.py
+-rw-rw-r--   0 da        (1000) da        (1000)    60425 2022-12-03 14:28:15.000000 cinemagoer-2023.5.1/imdb/utils.py
+-rw-rw-r--   0 da        (1000) da        (1000)       27 2023-05-01 13:38:29.000000 cinemagoer-2023.5.1/imdb/version.py
+-rw-rw-r--   0 da        (1000) da        (1000)      497 2023-05-01 13:41:20.706995 cinemagoer-2023.5.1/setup.cfg
+-rw-rw-r--   0 da        (1000) da        (1000)     4791 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/setup.py
+drwxrwxr-x   0 da        (1000) da        (1000)        0 2023-05-01 13:41:20.706995 cinemagoer-2023.5.1/tests/
+-rw-rw-r--   0 da        (1000) da        (1000)     1235 2022-12-03 12:26:09.000000 cinemagoer-2023.5.1/tests/conftest.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1303 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_chart_bottom.py
+-rw-rw-r--   0 da        (1000) da        (1000)      403 2022-02-06 11:37:04.000000 cinemagoer-2023.5.1/tests/test_http_chart_boxoffice.py
+-rw-rw-r--   0 da        (1000) da        (1000)      831 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_chart_popular_movies.py
+-rw-rw-r--   0 da        (1000) da        (1000)      763 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_chart_popular_tv.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1254 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_chart_top.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1163 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_chart_top_indian.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1200 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_chart_top_tv.py
+-rw-rw-r--   0 da        (1000) da        (1000)      163 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_company_main.py
+-rw-rw-r--   0 da        (1000) da        (1000)      416 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_gather_refs.py
+-rw-rw-r--   0 da        (1000) da        (1000)      145 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_awards.py
+-rw-rw-r--   0 da        (1000) da        (1000)    21288 2023-05-01 12:16:00.000000 cinemagoer-2023.5.1/tests/test_http_movie_combined.py
+-rw-rw-r--   0 da        (1000) da        (1000)      385 2023-05-01 12:52:29.000000 cinemagoer-2023.5.1/tests/test_http_movie_connections.py
+-rw-rw-r--   0 da        (1000) da        (1000)      689 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_full_credit.py
+-rw-rw-r--   0 da        (1000) da        (1000)      141 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_goofs.py
+-rw-rw-r--   0 da        (1000) da        (1000)      746 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_keywords.py
+-rw-rw-r--   0 da        (1000) da        (1000)      682 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_list.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1002 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_parental_guide.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1028 2023-02-11 17:00:48.000000 cinemagoer-2023.5.1/tests/test_http_movie_plot.py
+-rw-rw-r--   0 da        (1000) da        (1000)      146 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_quotes.py
+-rw-rw-r--   0 da        (1000) da        (1000)      303 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_recommendations.py
+-rw-rw-r--   0 da        (1000) da        (1000)      525 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_releaseinfo.py
+-rw-rw-r--   0 da        (1000) da        (1000)      345 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_movie_reviews.py
+-rw-rw-r--   0 da        (1000) da        (1000)     2963 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_season_episodes.py
+-rw-rw-r--   0 da        (1000) da        (1000)      444 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_series.py
+-rw-rw-r--   0 da        (1000) da        (1000)      804 2021-12-31 12:40:27.000000 cinemagoer-2023.5.1/tests/test_http_movie_sites.py
+-rw-rw-r--   0 da        (1000) da        (1000)      696 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_movie_taglines.py
+-rw-rw-r--   0 da        (1000) da        (1000)      389 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_tech.py
+-rw-rw-r--   0 da        (1000) da        (1000)      595 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_titles.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1621 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_movie_votes.py
+-rw-rw-r--   0 da        (1000) da        (1000)      149 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_http_person_awards.py
+-rw-rw-r--   0 da        (1000) da        (1000)     4551 2021-12-31 12:40:27.000000 cinemagoer-2023.5.1/tests/test_http_person_bio.py
+-rw-rw-r--   0 da        (1000) da        (1000)     2834 2023-02-05 13:33:15.000000 cinemagoer-2023.5.1/tests/test_http_person_main.py
+-rw-rw-r--   0 da        (1000) da        (1000)      665 2021-01-24 16:04:30.000000 cinemagoer-2023.5.1/tests/test_http_person_otherworks.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1805 2023-05-01 12:36:17.000000 cinemagoer-2023.5.1/tests/test_http_search_company.py
+-rw-rw-r--   0 da        (1000) da        (1000)     1034 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/tests/test_http_search_keyword.py
+-rw-rw-r--   0 da        (1000) da        (1000)     3928 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/tests/test_http_search_movie.py
+-rw-rw-r--   0 da        (1000) da        (1000)    18937 2022-12-03 12:26:09.000000 cinemagoer-2023.5.1/tests/test_http_search_movie_advanced.py
+-rw-rw-r--   0 da        (1000) da        (1000)      853 2022-12-03 12:26:09.000000 cinemagoer-2023.5.1/tests/test_http_search_movie_keyword.py
+-rw-rw-r--   0 da        (1000) da        (1000)     2333 2022-12-03 15:42:09.000000 cinemagoer-2023.5.1/tests/test_http_search_person.py
+-rw-rw-r--   0 da        (1000) da        (1000)      370 2022-10-08 16:39:46.000000 cinemagoer-2023.5.1/tests/test_http_showtimes.py
+-rw-rw-r--   0 da        (1000) da        (1000)      755 2022-12-08 10:02:56.000000 cinemagoer-2023.5.1/tests/test_in_operator.py
+-rw-rw-r--   0 da        (1000) da        (1000)      483 2023-01-15 11:53:39.000000 cinemagoer-2023.5.1/tests/test_locale.py
+-rw-rw-r--   0 da        (1000) da        (1000)      238 2022-10-02 15:54:24.000000 cinemagoer-2023.5.1/tests/test_xml.py
+-rw-rw-r--   0 da        (1000) da        (1000)      347 2022-11-05 13:34:27.000000 cinemagoer-2023.5.1/tox.ini
```

### Comparing `cinemagoer-2022.2.11/CHANGELOG.txt` & `cinemagoer-2023.5.1/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,71 @@
 * What's new in the next release
 
+* What's new in release 2023.05.01 (1922)
+
+  [http]
+
+  - #424: parse the "fullcredits" page for persons (courtesy of DLu)
+  - #443: fix parser for plot summary (courtesy of Saleh Dehqanpour)
+  - #448: always transform ratings to float
+  - various other parsers fixed
+
+
+* What's new in release 2022.12.27 (Turist)
+
+  [http]
+
+  - #419: more fixes for movie searches
+  - #426: support 308 Permanent Redirect HTTP code
+  - better handling of locales
+  - fixes for python2.7
+
+
+* What's new in release 2022.12.04 (John Wick)
+
+  [http]
+
+  - #232: add get_showtimes() method (courtesy of Kostya Farber)
+  - #388: add 'videos' key to extract movie trailer links
+  - #391: add parental guide advisory votes (courtesy of salehdeh76)
+  - #395: fix for some wrongly-formatted titles (courtesy of tsaklidis)
+  - #396: raise exception on resize image (courtesy of tsaklidis)
+  - #398: fix for production status
+  - #415: change User-Agent to a more complete form
+  - #419: fix movie and person searches
+  - #420: introduce a contributor guide (courtesy of Elizabeth Thorne)
+  - #421: fixes for person parsers
+
+
 * What's new in release 2022.02.11 (the Cinemagoer Strikes Back release)
 
   [http]
+
   - #373: include TV shows in get top 50 by genre
   - #378: update documentation
 
   [s3]
+
   - #378: rename s32imdbpy.py to s32cinemagoer.py
 
 
 
 * What's new in release 2022.01.25 (the Cinemagoer release)
 
   [general]
+
   - #238: by default, exceptions are raised
   - #315: include all script in the ./bin directory
   - #318: fix kind of tv mini series in search results
   - #369: do not rebuild locales running setup.py clean
   - #371: support for 8-digit imdbIDs
   - #378: renamed to cinemagoer
 
   [http]
+
   - #308: fix movie connections parser
   - #319: parse review rating
   - #327: do not strip new lines
   - #329: improve localized and original title
   - #330: fix for tv series for seasons not found
   - #331: fix kind of tv mini series in search results
   - #342: parse all information from full credits
@@ -38,14 +78,15 @@
   - #366: fix full-size image links
   - #372: support fox box office charts
 
 
 * What's new in release 2021.04.18 (Black Sails)
 
   [general]
+
   - #289: Serbian translations
   - #290: update Portuguese translations
   - #291: allow direct access to filmography keys
   - #299: add pagination to get_movie_list (courtesy of Stein van Broekhoven)
   - #300: any iterable can be used as season_nums parameter of update_series_seasons
   - #305: fix ability to set logging level
   - #310: fix build of locales .mo files
```

### Comparing `cinemagoer-2022.2.11/CONTRIBUTORS.txt` & `cinemagoer-2023.5.1/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/LICENSE.txt` & `cinemagoer-2023.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/PKG-INFO` & `cinemagoer-2023.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: cinemagoer
-Version: 2022.2.11
+Version: 2023.5.1
 Summary: Python package to access the IMDb's database
 Home-page: https://cinemagoer.github.io/
+Download-URL: https://cinemagoer.github.io/downloads/
 Author: Davide Alberani
 Author-email: da@mimante.net
 Maintainer: Davide Alberani
 Maintainer-email: da@mimante.net
 License: GPL
-Download-URL: https://cinemagoer.github.io/downloads/
-Description: Cinemagoer is a Python package useful to retrieve and
-        manage the data of the IMDb movie database about movies, people,
-        characters and companies.
-        
-        Cinemagoer and its authors are not affiliated in any way to
-        Internet Movie Database Inc.; see the DISCLAIMER.txt file for
-        details about data licenses.
-        
-        Platform-independent and written in Python 3
-        
-        Cinemagoer package can be very easily used by programmers and developers
-        to provide access to the IMDb's data to their programs.
-        
-        Some simple example scripts - useful for the end users - are included
-        in this package; other Cinemagoer-based programs are available at the
-        home page: https://cinemagoer.github.io/
-        
+Project-URL: Source, https://github.com/cinemagoer/cinemagoer
 Keywords: imdb,movie,people,database,cinema,film,person,cast,actor,actress,director,sql,character,company,package,plain text data files,keywords,top250,bottom100,xml
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Italian
 Classifier: Natural Language :: Turkish
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: doc
-Provides-Extra: test
+License-File: LICENSE.txt
+
+Cinemagoer is a Python package useful to retrieve and
+manage the data of the IMDb movie database about movies, people,
+characters and companies.
+
+Cinemagoer and its authors are not affiliated in any way to
+Internet Movie Database Inc.; see the DISCLAIMER.txt file for
+details about data licenses.
+
+Platform-independent and written in Python 3
+
+Cinemagoer package can be very easily used by programmers and developers
+to provide access to the IMDb's data to their programs.
+
+Some simple example scripts - useful for the end users - are included
+in this package; other Cinemagoer-based programs are available at the
+home page: https://cinemagoer.github.io/
```

### Comparing `cinemagoer-2022.2.11/README.rst` & `cinemagoer-2023.5.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 Here's an example that demonstrates how to use Cinemagoer:
 
 .. code-block:: python
 
    from imdb import Cinemagoer
 
-   # create an instance of the IMDb class
+   # create an instance of the Cinemagoer class
    ia = Cinemagoer()
 
    # get a movie
    movie = ia.get_movie('0133093')
 
    # print the names of the directors of the movie
    print('Directors:')
@@ -92,14 +92,19 @@
 ------------
 
 Please refer to the `support`_ page on the `project homepage`_
 and to the the online documentation on `Read The Docs`_.
 
 The sources are available on `GitHub`_.
 
+Contribute
+------------
+
+Visit the `CONTRIBUTOR_GUIDE.rst`_ to learn how you can contribute to the Cinemagoer package.
+
 License
 -------
 
 Copyright (C) 2004-2022 Davide Alberani <da --> mimante.net> et al.
 
 Cinemagoer is released under the GPL license, version 2 or later.
 Read the included `LICENSE.txt`_ file for details.
@@ -111,10 +116,11 @@
 .. _IMDb: https://www.imdb.com/
 .. _please help with it!: http://cinemagoer.readthedocs.io/en/latest/devel/test.html
 .. _Curious about that: https://cinemagoer.github.io/ecosystem/
 .. _project homepage: https://cinemagoer.github.io/
 .. _support: https://cinemagoer.github.io/support/
 .. _Read The Docs: https://cinemagoer.readthedocs.io/
 .. _GitHub: https://github.com/cinemagoer/cinemagoer
+.. _CONTRIBUTOR_GUIDE.rst: https://github.com/ethorne2/cinemagoer/blob/documentation-add-contributor-guide/CONTRIBUTOR_GUIDE.rst
 .. _LICENSE.txt: https://raw.githubusercontent.com/cinemagoer/cinemagoer/master/LICENSE.txt
 .. _CONTRIBUTORS.txt: https://raw.githubusercontent.com/cinemagoer/cinemagoer/master/CONTRIBUTORS.txt
 .. _DISCLAIMER.txt: https://raw.githubusercontent.com/cinemagoer/cinemagoer/master/DISCLAIMER.txt
```

### Comparing `cinemagoer-2022.2.11/bin/get_company.py` & `cinemagoer-2023.5.1/bin/get_company.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_first_company.py` & `cinemagoer-2023.5.1/bin/get_first_company.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_first_movie.py` & `cinemagoer-2023.5.1/bin/get_first_movie.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_first_person.py` & `cinemagoer-2023.5.1/bin/get_first_person.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_keyword.py` & `cinemagoer-2023.5.1/bin/get_keyword.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_movie.py` & `cinemagoer-2023.5.1/bin/get_movie.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_movie_list.py` & `cinemagoer-2023.5.1/bin/get_movie_list.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_person.py` & `cinemagoer-2023.5.1/bin/get_person.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/get_top_bottom_movies.py` & `cinemagoer-2023.5.1/bin/get_top_bottom_movies.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/imdbpy2sql.py` & `cinemagoer-2023.5.1/bin/imdbpy2sql.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/s32cinemagoer.py` & `cinemagoer-2023.5.1/bin/s32cinemagoer.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,36 +160,41 @@
                 count += len(block)
                 percent = count * 100 / nr_of_lines
         except Exception as e:
             logging.error('error processing data on table %s: %s' % (table.name, e))
         logging.info('processed file %s: %d entries' % (fn, count))
 
 
-def import_dir(dir_name, engine):
+def import_dir(dir_name, engine, cleanup=False):
     """Import data from a series of .tsv.gz files.
 
     :param dir_name: directory containing the .tsv.gz files
     :type dir_name: str
     :param engine: SQLAlchemy engine
     :type engine: :class:`sqlalchemy.engine.base.Engine`
     """
     for fn in glob.glob(os.path.join(dir_name, '*%s' % TSV_EXT)):
         if not os.path.isfile(fn):
             logging.debug('skipping file %s' % fn)
             continue
         import_file(fn, engine)
+        if cleanup:
+            logging.debug('Removing file %s' % fn)
+            os.remove(fn)
 
-
+ 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('tsv_files_dir')
     parser.add_argument('db_uri')
     parser.add_argument('--verbose', help='increase verbosity and show progress', action='store_true')
+    parser.add_argument('--cleanup', help='Remove files after they\'re imported', action='store_true')
     args = parser.parse_args()
     dir_name = args.tsv_files_dir
     db_uri = args.db_uri
     if args.verbose:
         logger.setLevel(logging.DEBUG)
+    cleanup = args.cleanup
     engine = sqlalchemy.create_engine(db_uri, encoding='utf-8', echo=False)
     metadata.bind = engine
-    import_dir(dir_name, engine)
+    import_dir(dir_name, engine, cleanup)
```

### Comparing `cinemagoer-2022.2.11/bin/search_company.py` & `cinemagoer-2023.5.1/bin/search_company.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/search_keyword.py` & `cinemagoer-2023.5.1/bin/search_keyword.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/search_movie.py` & `cinemagoer-2023.5.1/bin/search_movie.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/bin/search_person.py` & `cinemagoer-2023.5.1/bin/search_person.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/cinemagoer.egg-info/PKG-INFO` & `cinemagoer-2023.5.1/cinemagoer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: cinemagoer
-Version: 2022.2.11
+Version: 2023.5.1
 Summary: Python package to access the IMDb's database
 Home-page: https://cinemagoer.github.io/
+Download-URL: https://cinemagoer.github.io/downloads/
 Author: Davide Alberani
 Author-email: da@mimante.net
 Maintainer: Davide Alberani
 Maintainer-email: da@mimante.net
 License: GPL
-Download-URL: https://cinemagoer.github.io/downloads/
-Description: Cinemagoer is a Python package useful to retrieve and
-        manage the data of the IMDb movie database about movies, people,
-        characters and companies.
-        
-        Cinemagoer and its authors are not affiliated in any way to
-        Internet Movie Database Inc.; see the DISCLAIMER.txt file for
-        details about data licenses.
-        
-        Platform-independent and written in Python 3
-        
-        Cinemagoer package can be very easily used by programmers and developers
-        to provide access to the IMDb's data to their programs.
-        
-        Some simple example scripts - useful for the end users - are included
-        in this package; other Cinemagoer-based programs are available at the
-        home page: https://cinemagoer.github.io/
-        
+Project-URL: Source, https://github.com/cinemagoer/cinemagoer
 Keywords: imdb,movie,people,database,cinema,film,person,cast,actor,actress,director,sql,character,company,package,plain text data files,keywords,top250,bottom100,xml
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Italian
 Classifier: Natural Language :: Turkish
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: doc
-Provides-Extra: test
+License-File: LICENSE.txt
+
+Cinemagoer is a Python package useful to retrieve and
+manage the data of the IMDb movie database about movies, people,
+characters and companies.
+
+Cinemagoer and its authors are not affiliated in any way to
+Internet Movie Database Inc.; see the DISCLAIMER.txt file for
+details about data licenses.
+
+Platform-independent and written in Python 3
+
+Cinemagoer package can be very easily used by programmers and developers
+to provide access to the IMDb's data to their programs.
+
+Some simple example scripts - useful for the end users - are included
+in this package; other Cinemagoer-based programs are available at the
+home page: https://cinemagoer.github.io/
```

### Comparing `cinemagoer-2022.2.11/cinemagoer.egg-info/SOURCES.txt` & `cinemagoer-2023.5.1/cinemagoer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,30 +38,25 @@
 imdb/_logging.py
 imdb/cli.py
 imdb/helpers.py
 imdb/linguistics.py
 imdb/utils.py
 imdb/version.py
 imdb/locale/__init__.py
-imdb/locale/generatepot.py
 imdb/locale/imdbpy-ar.po
 imdb/locale/imdbpy-bg.po
 imdb/locale/imdbpy-de.po
 imdb/locale/imdbpy-en.po
 imdb/locale/imdbpy-es.po
 imdb/locale/imdbpy-fr.po
 imdb/locale/imdbpy-it.po
 imdb/locale/imdbpy-pt_BR.po
 imdb/locale/imdbpy-sr.po
 imdb/locale/imdbpy-tr.po
 imdb/locale/imdbpy.pot
-imdb/locale/msgfmt.py
-imdb/locale/msgfmt.pyc
-imdb/locale/rebuildmo.py
-imdb/locale/rebuildmo.pyc
 imdb/locale/ar/LC_MESSAGES/imdbpy.mo
 imdb/locale/bg/LC_MESSAGES/imdbpy.mo
 imdb/locale/de/LC_MESSAGES/imdbpy.mo
 imdb/locale/en/LC_MESSAGES/imdbpy.mo
 imdb/locale/es/LC_MESSAGES/imdbpy.mo
 imdb/locale/fr/LC_MESSAGES/imdbpy.mo
 imdb/locale/it/LC_MESSAGES/imdbpy.mo
@@ -78,14 +73,15 @@
 imdb/parser/http/personParser.py
 imdb/parser/http/piculet.py
 imdb/parser/http/searchCompanyParser.py
 imdb/parser/http/searchKeywordParser.py
 imdb/parser/http/searchMovieAdvancedParser.py
 imdb/parser/http/searchMovieParser.py
 imdb/parser/http/searchPersonParser.py
+imdb/parser/http/showtimesParser.py
 imdb/parser/http/topBottomParser.py
 imdb/parser/http/utils.py
 imdb/parser/s3/__init__.py
 imdb/parser/s3/utils.py
 imdb/parser/sql/__init__.py
 imdb/parser/sql/alchemyadapter.py
 imdb/parser/sql/dbschema.py
@@ -126,9 +122,11 @@
 tests/test_http_person_otherworks.py
 tests/test_http_search_company.py
 tests/test_http_search_keyword.py
 tests/test_http_search_movie.py
 tests/test_http_search_movie_advanced.py
 tests/test_http_search_movie_keyword.py
 tests/test_http_search_person.py
+tests/test_http_showtimes.py
 tests/test_in_operator.py
+tests/test_locale.py
 tests/test_xml.py
```

### Comparing `cinemagoer-2022.2.11/imdb/Character.py` & `cinemagoer-2023.5.1/imdb/Character.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/Company.py` & `cinemagoer-2023.5.1/imdb/Company.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 a given company.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from copy import deepcopy
 
-from imdb.utils import _Container
-from imdb.utils import analyze_company_name, build_company_name, cmpCompanies, flatten
+from imdb.utils import _Container, analyze_company_name, build_company_name, cmpCompanies, flatten
 
 
 class Company(_Container):
     """A company.
 
     Every information about a company can be accessed as::
```

### Comparing `cinemagoer-2022.2.11/imdb/Movie.py` & `cinemagoer-2023.5.1/imdb/Movie.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from copy import deepcopy
 
 from imdb import linguistics
-from imdb.utils import _Container
-from imdb.utils import analyze_title, build_title, canonicalTitle, cmpMovies, flatten
+from imdb.utils import _Container, analyze_title, build_title, canonicalTitle, cmpMovies, flatten
 
 
 class Movie(_Container):
     """A Movie.
 
     Every information about a movie can be accessed as::
 
@@ -235,17 +234,17 @@
             return True
         return False
     isSameMovie = isSameTitle   # XXX: just for backward compatiblity.
 
     def __contains__(self, item):
         """Return true if the given Person object is listed in this Movie,
         or if the the given Character is represented in this Movie."""
-        from .Person import Person
         from .Character import Character
         from .Company import Company
+        from .Person import Person
         if isinstance(item, Person):
             for p in flatten(self.data, yieldDictKeys=True, scalar=Person,
                              toDescend=(list, dict, tuple, Movie)):
                 if item.isSame(p):
                     return True
         elif isinstance(item, Character):
             for p in flatten(self.data, yieldDictKeys=True, scalar=Person,
```

### Comparing `cinemagoer-2022.2.11/imdb/Person.py` & `cinemagoer-2023.5.1/imdb/Person.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 a given person.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from copy import deepcopy
 
-from imdb.utils import _Container, analyze_name, build_name, cmpPeople, flatten, normalizeName, canonicalName
+from imdb.utils import _Container, analyze_name, build_name, canonicalName, cmpPeople, flatten, normalizeName
 
 
 class Person(_Container):
     """A Person.
 
     Every information about a person can be accessed as::
 
@@ -180,16 +180,17 @@
         """The Person is "false" if the self.data does not contain a name."""
         # XXX: check the name and the personID?
         return 'name' in self.data
 
     def __contains__(self, item):
         """Return true if this Person has worked in the given Movie,
         or if the fiven Character was played by this Person."""
-        from .Movie import Movie
         from .Character import Character
+        from .Movie import Movie
+
         if isinstance(item, Movie):
             for m in flatten(self.data, yieldDictKeys=True, scalar=Movie):
                 if item.isSame(m):
                     return True
         elif isinstance(item, Character):
             for m in flatten(self.data, yieldDictKeys=True, scalar=Movie):
                 if item.isSame(m.currentRole):
```

### Comparing `cinemagoer-2022.2.11/imdb/__init__.py` & `cinemagoer-2023.5.1/imdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,30 +17,31 @@
 """
 This package can be used to retrieve information about a movie or a person
 from the IMDb database. It can fetch data through different media such as
 the IMDb web pages, or a SQL database.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
+
 from imdb.version import __version__
 
 __all__ = ['Cinemagoer', 'IMDb', 'IMDbError', 'Movie', 'Person', 'Character', 'Company',
            'available_access_systems']
 
 VERSION = __version__
 
 
 import os
 import sys
 from pkgutil import find_loader
-from types import MethodType, FunctionType
+from types import FunctionType, MethodType
 
-from imdb._logging import imdbpyLogger as _imdb_logger
-from imdb._exceptions import IMDbDataAccessError, IMDbError
 from imdb import Character, Company, Movie, Person
+from imdb._exceptions import IMDbDataAccessError, IMDbError
+from imdb._logging import imdbpyLogger as _imdb_logger
 from imdb.utils import build_company_name, build_name, build_title
 
 PY2 = sys.hexversion < 0x3000000
 
 if PY2:
     import ConfigParser as configparser
 else:
@@ -73,16 +74,16 @@
 imdbURL_company_main = imdbURL_company_base + 'co%s/'
 # http://www.imdb.com/keyword/%s/
 imdbURL_keyword_main = imdbURL_base + 'search/keyword/?keywords=%s'
 # http://www.imdb.com/chart/top
 imdbURL_top250 = imdbURL_base + 'chart/top'
 # http://www.imdb.com/chart/bottom
 imdbURL_bottom100 = imdbURL_base + 'chart/bottom'
-# http://www.imdb.com/find?%s
-imdbURL_find = imdbURL_base + 'find?%s'
+# http://www.imdb.com/find/?%s
+imdbURL_find = imdbURL_base + 'find/?%s'
 # http://www.imdb.com/list/
 imdbURL_list_base = imdbURL_base + 'list/'
 
 # Name of the configuration files.
 confFileNames = ['cinemagoer.cfg', 'imdbpy.cfg']
 
 
@@ -201,17 +202,19 @@
             from .parser.sql import IMDbSqlAccessSystem
         except ImportError:
             raise IMDbError('the sql access system is not installed')
         return IMDbSqlAccessSystem(*arguments, **keywords)
     else:
         raise IMDbError('unknown kind of data access system: "%s"' % accessSystem)
 
+
 # Cinemagoer alias
 Cinemagoer = IMDb
 
+
 def available_access_systems():
     """Return the list of available data access systems."""
     asList = []
     if find_loader('imdb.parser.http') is not None:
         asList.append('http')
     if find_loader('imdb.parser.sql') is not None:
         asList.append('sql')
@@ -304,20 +307,22 @@
         imdbURL_tvmeter100 = imdbURL_base + 'chart/tvmeter'
         # http://www.imdb.com/chart/toptv
         imdbURL_toptv250 = imdbURL_base + 'chart/toptv'
         # https://www.imdb.com/india/top-rated-indian-movies
         imdbURL_topindian250 = imdbURL_base + 'india/top-rated-indian-movies'
         # http://www.imdb.com/chart/boxoffice/
         imdbURL_boxoffice = imdbURL_base + 'chart/boxoffice/'
-        # http://www.imdb.com/find?%s
-        imdbURL_find = imdbURL_base + 'find?%s'
+        # http://www.imdb.com/find/?%s
+        imdbURL_find = imdbURL_base + 'find/?%s'
         # http://www.imdb.com/search/title?%s
         imdbURL_search_movie_advanced = imdbURL_base + 'search/title/?%s'
         # http://www.imdb.com/list/
         imdbURL_list_base = imdbURL_base + 'list/'
+        # https://www.imdb.com/showtimes
+        imdbURL_showtimes = imdbURL_base + 'showtimes'
         self.urls = dict(
             movie_base=imdbURL_movie_base,
             movie_main=imdbURL_movie_main,
             person_base=imdbURL_person_base,
             person_main=imdbURL_person_main,
             character_base=imdbURL_character_base,
             character_main=imdbURL_character_main,
@@ -329,15 +334,16 @@
             moviemeter100=imdbURL_moviemeter100,
             tvmeter100=imdbURL_tvmeter100,
             toptv250=imdbURL_toptv250,
             topindian250=imdbURL_topindian250,
             find=imdbURL_find,
             movie_list=imdbURL_list_base,
             search_movie_advanced=imdbURL_search_movie_advanced,
-            boxoffice=imdbURL_boxoffice)
+            boxoffice=imdbURL_boxoffice,
+            showtimes=imdbURL_showtimes)
 
     def _normalize_movieID(self, movieID):
         """Normalize the given movieID."""
         # By default, do nothing.
         return movieID
 
     def _normalize_personID(self, personID):
@@ -442,28 +448,28 @@
             results = 20
         if not _episodes:
             res = self._search_movie(title, results)
         else:
             res = self._search_episode(title, results)
         return [Movie.Movie(movieID=self._get_real_movieID(mi),
                 data=md, modFunct=self._defModFunct,
-                accessSystem=self.accessSystem) for mi, md in res][:results]
+                accessSystem=self.accessSystem) for mi, md in res if mi and md][:results]
 
     def _get_movie_list(self, list_, results):
         """Return a list of tuples (movieID, {movieData})"""
         # XXX: for the real implementation, see the method of the
         #      subclass, somewhere under the imdb.parser package.
         raise NotImplementedError('override this method')
 
     def get_movie_list(self, list_, results=None):
         """Return a list of Movie objects for a list id as input """
         res = self._get_movie_list(list_, results)
         return [Movie.Movie(movieID=self._get_real_movieID(mi),
                 data=md, modFunct=self._defModFunct,
-                accessSystem=self.accessSystem) for mi, md in res][:results]
+                accessSystem=self.accessSystem) for mi, md in res if mi and md][:results]
 
     def _search_movie_advanced(self, title=None, adult=None, results=None, sort=None, sort_dir=None):
         """Return a list of tuples (movieID, {movieData})"""
         # XXX: for the real implementation, see the method of the
         #      subclass, somewhere under the imdb.parser package.
         raise NotImplementedError('override this method')
 
@@ -475,15 +481,15 @@
         try:
             results = int(results)
         except (ValueError, OverflowError):
             results = 20
         res = self._search_movie_advanced(title=title, adult=adult, results=results, sort=sort, sort_dir=sort_dir)
         return [Movie.Movie(movieID=self._get_real_movieID(mi),
                 data=md, modFunct=self._defModFunct,
-                accessSystem=self.accessSystem) for mi, md in res][:results]
+                accessSystem=self.accessSystem) for mi, md in res if mi and md][:results]
 
     def _search_episode(self, title, results):
         """Return a list of tuples (movieID, {movieData})"""
         # XXX: for the real implementation, see the method of the
         #      subclass, somewhere under the imdb.parser package.
         raise NotImplementedError('override this method')
 
@@ -528,15 +534,15 @@
         try:
             results = int(results)
         except (ValueError, OverflowError):
             results = 20
         res = self._search_person(name, results)
         return [Person.Person(personID=self._get_real_personID(pi),
                 data=pd, modFunct=self._defModFunct,
-                accessSystem=self.accessSystem) for pi, pd in res][:results]
+                accessSystem=self.accessSystem) for pi, pd in res if pi and pd][:results]
 
     def get_character(self, characterID, info=Character.Character.default_info,
                       modFunct=None):
         """Return a Character object for the given characterID.
 
         The characterID is something used to univocally identify a character;
         it can be the imdbID used by the IMDb web server, a file
@@ -571,15 +577,15 @@
         try:
             results = int(results)
         except (ValueError, OverflowError):
             results = 20
         res = self._search_character(name, results)
         return [Character.Character(characterID=self._get_real_characterID(pi),
                 data=pd, modFunct=self._defModFunct,
-                accessSystem=self.accessSystem) for pi, pd in res][:results]
+                accessSystem=self.accessSystem) for pi, pd in res if pi and pd][:results]
 
     def get_company(self, companyID, info=Company.Company.default_info,
                     modFunct=None):
         """Return a Company object for the given companyID.
 
         The companyID is something used to univocally identify a company;
         it can be the imdbID used by the IMDb web server, a file
@@ -613,15 +619,15 @@
         try:
             results = int(results)
         except (ValueError, OverflowError):
             results = 20
         res = self._search_company(name, results)
         return [Company.Company(companyID=self._get_real_companyID(pi),
                 data=pd, modFunct=self._defModFunct,
-                accessSystem=self.accessSystem) for pi, pd in res][:results]
+                accessSystem=self.accessSystem) for pi, pd in res if pi and pd][:results]
 
     def _search_keyword(self, keyword, results):
         """Return a list of 'keyword' strings."""
         # XXX: for the real implementation, see the method of the
         #      subclass, somewhere under the imdb.parser package.
         raise NotImplementedError('override this method')
 
@@ -739,14 +745,25 @@
             genres = ','.join(map(str, genres))
         tv_filter = '&title_type=tv_series,mini_series'
         res = self._get_top_movies_or_tv_by_genres(genres, tv_filter)
         return [Movie.Movie(movieID=self._get_real_movieID(mi),
                             data=md, modFunct=self._defModFunct,
                             accessSystem=self.accessSystem) for mi, md in res]
 
+    def _get_showtimes(self):
+        # XXX: for the real implementation, see the method of the
+        #      subclass, somewhere under the imdb.parser package.
+        raise NotImplementedError('override this method')
+
+    def get_showtimes(self):
+        """Return a list of objects like this:
+        [{'cinema': 'Cinema Name', 'address and contacts': '...',
+          'movies': [{'movie': MovieObject, 'showtimes': 'showtimes info'}}, ...]"""
+        return self._get_showtimes()
+
     def new_movie(self, *arguments, **keywords):
         """Return a Movie object."""
         # XXX: not really useful...
         return Movie.Movie(accessSystem=self.accessSystem, *arguments, **keywords)
 
     def new_person(self, *arguments, **keywords):
         """Return a Person object."""
```

### Comparing `cinemagoer-2022.2.11/imdb/_exceptions.py` & `cinemagoer-2023.5.1/imdb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/_logging.py` & `cinemagoer-2023.5.1/imdb/_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 This module provides the logging facilities used by the imdb package.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import logging
 
-
 LEVELS = {
     'debug': logging.DEBUG,
     'info': logging.INFO,
     'warn': logging.WARNING,
     'warning': logging.WARNING,
     'error': logging.ERROR,
     'critical': logging.CRITICAL
```

### Comparing `cinemagoer-2022.2.11/imdb/cli.py` & `cinemagoer-2023.5.1/imdb/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import sys
 from argparse import ArgumentParser
 
 from imdb import VERSION, IMDb
 
-
 DEFAULT_RESULT_SIZE = 20
 
 
 def list_results(items, type_, n=None):
     field = 'title' if type_ == 'movie' else 'name'
     print('  # IMDb id %s' % field)
     print('=== ======= %s' % ('=' * len(field),))
```

### Comparing `cinemagoer-2022.2.11/imdb/helpers.py` & `cinemagoer-2023.5.1/imdb/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 but useful for Cinemagoer-based programs.
 """
 
 # XXX: Find better names for the functions in this module.
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-import sys
 import difflib
 import gettext
 import re
-from gettext import gettext as _
+import sys
+
+from imdb.locale import _
 
 PY2 = sys.hexversion < 0x3000000
 if PY2:
     from cgi import escape
 else:
     from html import escape
 
 # The modClearRefs can be used to strip names and titles references from
 # the strings in Movie and Person objects.
 from imdb import IMDb, imdbURL_character_base, imdbURL_movie_base, imdbURL_person_base
+from imdb._exceptions import IMDbError
 from imdb.Character import Character
 from imdb.Company import Company
 from imdb.linguistics import COUNTRY_LANG
 from imdb.Movie import Movie
 from imdb.Person import Person
-from imdb.utils import _tagAttr, re_characterRef, re_nameRef, re_titleRef
-from imdb.utils import TAGS_TO_MODIFY
-
+from imdb.utils import TAGS_TO_MODIFY, _tagAttr, re_characterRef, re_nameRef, re_titleRef
 
 gettext.textdomain('imdbpy')
 
 
 # An URL, more or less.
 _re_href = re.compile(r'(http://.+?)(?=\s|$)', re.I)
 _re_hrefsub = _re_href.sub
@@ -603,20 +603,24 @@
             scores.append(difflib.SequenceMatcher(None, aka.lower(),
                                                   _searchedTitle.lower()), aka)
         scores.sort(reverse=True)
         akas = [x[1] for x in scores]
     return akas
 
 
-def resizeImage(image, width=None, height=None, crop=None):
+def resizeImage(image, width=None, height=None, crop=None, custom_regex=None):
     """Return resized and cropped image url."""
 
-    regexString = r'https://m.media-amazon.com/images/\w/\w+'
+    regexString = custom_regex if custom_regex else r'https://m.media-amazon.com/images/\w/\w+'
+
+    try:
+        resultImage = re.findall(regexString, image)[0]
+    except IndexError:
+        raise IMDbError('Image url not matched. Original url: "%s"' % (image))
 
-    resultImage = re.findall(regexString, image)[0]
     if "@@" in image:
         resultImage += '@'
 
     if "@" not in image:
         resultImage += '._V1_'
     else:
         resultImage += '@._V1_'
```

### Comparing `cinemagoer-2022.2.11/imdb/linguistics.py` & `cinemagoer-2023.5.1/imdb/linguistics.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/__init__.py` & `cinemagoer-2023.5.1/imdb/locale/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import gettext
 import os
 
 LOCALE_DIR = os.path.dirname(__file__)
 
-gettext.bindtextdomain('imdbpy', LOCALE_DIR)
+translation = gettext.translation('imdbpy', LOCALE_DIR)
+_ = translation.gettext
```

### Comparing `cinemagoer-2022.2.11/imdb/locale/ar/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/ar/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/bg/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/bg/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/de/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/de/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/en/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/en/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/es/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/es/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/fr/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/fr/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-ar.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-ar.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-bg.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-bg.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-de.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-de.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-en.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-en.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-es.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-es.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-fr.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-fr.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-it.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-it.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-pt_BR.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-pt_BR.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-sr.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-sr.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy-tr.po` & `cinemagoer-2023.5.1/imdb/locale/imdbpy-tr.po`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/imdbpy.pot` & `cinemagoer-2023.5.1/imdb/locale/imdbpy.pot`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/it/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/it/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/pt_BR/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/pt_BR/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/sr/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/sr/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/locale/tr/LC_MESSAGES/imdbpy.mo` & `cinemagoer-2023.5.1/imdb/locale/tr/LC_MESSAGES/imdbpy.mo`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/parser/__init__.py` & `cinemagoer-2023.5.1/imdb/parser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 This package provides various parsers to access IMDb data, such as
 a parser for the web/http interface, a parser for the SQL database interface,
 etc. So far, the http, s3 and sql parsers are implemented.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-
 __all__ = ['http', 'sql', 's3']
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/__init__.py` & `cinemagoer-2023.5.1/imdb/parser/http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2020 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2022 Davide Alberani <da@erlug.linux.it>
 #                2008 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -24,42 +24,42 @@
 or "html" (this is the default).
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import socket
 import ssl
-from codecs import lookup
 import warnings
+from codecs import lookup
 
-from imdb import PY2
-from imdb import IMDbBase
-from imdb.utils import analyze_title
-from imdb.parser.http.logging import logger
+from imdb import PY2, IMDbBase
 from imdb._exceptions import IMDbDataAccessError, IMDbParserError
+from imdb.parser.http.logging import logger
+from imdb.utils import analyze_title
 
 from . import (
     companyParser,
+    listParser,
     movieParser,
     personParser,
-    searchMovieParser,
-    searchMovieAdvancedParser,
-    searchPersonParser,
     searchCompanyParser,
     searchKeywordParser,
-    topBottomParser,
-    listParser
+    searchMovieAdvancedParser,
+    searchMovieParser,
+    searchPersonParser,
+    showtimesParser,
+    topBottomParser
 )
 
 if PY2:
     from urllib import quote_plus
-    from urllib2 import HTTPSHandler, ProxyHandler, build_opener
+    from urllib2 import HTTPRedirectHandler, HTTPSHandler, ProxyHandler, build_opener  # noqa: I003
 else:
     from urllib.parse import quote_plus
-    from urllib.request import HTTPSHandler, ProxyHandler, build_opener
+    from urllib.request import HTTPRedirectHandler, HTTPSHandler, ProxyHandler, build_opener
 
 # Logger for miscellaneous functions.
 _aux_logger = logger.getChild('aux')
 
 
 class _ModuleProxy:
     """A proxy to instantiate and access parsers."""
@@ -146,26 +146,37 @@
             {'proxy': str(proxy),
              'fullurl': fullurl,
              'error type': 'open_unknown_proxy',
              'data': str(data)}
         )
 
 
+class IMDbHTTPRedirectHandler(HTTPRedirectHandler):
+    """Custom handler to support redirect 308."""
+    def http_error_308(self, req, fp, code, msg, headers):
+        # force handling of redirect 308
+        req.code = 302
+        code = 302
+        return super(IMDbHTTPRedirectHandler, self).http_error_302(req, fp, code, msg, headers)
+
+
 class IMDbURLopener:
     """Fetch web pages and handle errors."""
     _logger = logger.getChild('urlopener')
 
     def __init__(self, *args, **kwargs):
         self._last_url = ''
         self.https_handler = IMDbHTTPSHandler(logger=self._logger)
+        self.redirect_handler = IMDbHTTPRedirectHandler()
         self.proxies = {}
         self.addheaders = []
         for header in ('User-Agent', 'User-agent', 'user-agent'):
             self.del_header(header)
-        self.set_header('User-Agent', 'Mozilla/5.0')
+        self.set_header('User-Agent',
+                        'Mozilla/5.0 (X11; CrOS armv6l 13597.84.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36 Edg/107.0.1418.56')  # noqa: E501
         lang = kwargs.get('languages', 'en-us,en;q=0.5')
         self.set_header('Accept-Language', lang)
 
     def get_proxy(self):
         """Return the used proxy, or an empty string."""
         return self.proxies.get('http', '')
 
@@ -211,14 +222,15 @@
             handlers = []
             if 'http' in self.proxies:
                 proxy_handler = ProxyHandler({
                     'http': self.proxies['http'],
                     'https': self.proxies['http']
                 })
                 handlers.append(proxy_handler)
+            handlers.append(self.redirect_handler)
             handlers.append(self.https_handler)
             uopener = build_opener(*handlers)
             uopener.addheaders = list(self.addheaders)
             response = uopener.open(url)
             content = response.read()
             self._last_url = response.url
             # Maybe the server is so nice to tell us the charset...
@@ -289,14 +301,15 @@
         self.scompProxy = _ModuleProxy(searchCompanyParser, defaultKeys=_def)
         self.skProxy = _ModuleProxy(searchKeywordParser, defaultKeys=_def)
         self.mProxy = _ModuleProxy(movieParser, defaultKeys=_def)
         self.pProxy = _ModuleProxy(personParser, defaultKeys=_def)
         self.compProxy = _ModuleProxy(companyParser, defaultKeys=_def)
         self.topBottomProxy = _ModuleProxy(topBottomParser, defaultKeys=_def)
         self.listProxy = _ModuleProxy(listParser, defaultKeys=_def)
+        self.stimesProxy = _ModuleProxy(showtimesParser, defaultKeys=_def)
 
     def _normalize_movieID(self, movieID):
         """Normalize the given movieID."""
         try:
             return '%07d' % int(movieID)
         except ValueError as e:
             raise IMDbParserError('invalid movieID "%s": %s' % (movieID, e))
@@ -384,15 +397,15 @@
     def _get_search_content(self, kind, ton, results):
         """Retrieve the web page for a given search.
         kind can be 'tt' (for titles), 'nm' (for names),
         or 'co' (for companies).
         ton is the title or the name to search.
         results is the maximum number of results to be retrieved."""
         if PY2:
-            params = 'q=%s&s=%s' % (quote_plus(ton.encode('utf8'), safe=''.encode('utf8')), kind.encode('utf8'))
+            params = 'q=%s&s=%s' % (quote_plus(ton, safe=''.encode('utf8')), kind.encode('utf8'))
         else:
             params = 'q=%s&s=%s' % (quote_plus(ton, safe=''), kind)
         if kind == 'ep':
             params = params.replace('s=ep&', 's=tt&ttype=ep&', 1)
         cont = self._retrieve(self.urls['find'] % params)
         # print 'URL:', imdbURL_find % params
         if cont.find('Your search returned more than') == -1 or \
@@ -615,15 +628,15 @@
         return data_d
 
     def get_movie_episodes(self, movieID, season_nums='all'):
         cont = self._retrieve(self.urls['movie_main'] % movieID + 'episodes')
         temp_d = self.mProxy.season_episodes_parser.parse(cont)
         if isinstance(season_nums, int):
             season_nums = {season_nums}
-        elif (isinstance(season_nums, (list, tuple)) or 
+        elif (isinstance(season_nums, (list, tuple)) or
               not hasattr(season_nums, '__contains__')):
             season_nums = set(season_nums)
         if not temp_d and 'data' in temp_d:
             return {}
 
         _seasons = temp_d['data'].get('_seasons') or []
 
@@ -679,19 +692,19 @@
     def _search_person(self, name, results):
         cont = self._get_search_content('nm', name, results)
         return self.spProxy.search_person_parser.parse(cont, results=results)['data']
 
     def get_person_main(self, personID):
         cont = self._retrieve(self.urls['person_main'] % personID)
         ret = self.pProxy.maindetails_parser.parse(cont)
-        ret['info sets'] = ('main', 'filmography')
         return ret
 
     def get_person_filmography(self, personID):
-        return self.get_person_main(personID)
+        cont = self._retrieve(self.urls['person_main'] % personID + 'fullcredits')
+        return self.pProxy.filmo_parser.parse(cont, getRefs=self._getRefs)
 
     def get_person_biography(self, personID):
         cont = self._retrieve(self.urls['person_main'] % personID + 'bio')
         return self.pProxy.bio_parser.parse(cont, getRefs=self._getRefs)
 
     def get_person_awards(self, personID):
         cont = self._retrieve(self.urls['person_main'] % personID + 'awards')
@@ -779,7 +792,11 @@
         elif kind == 'boxoffice':
             parser = self.topBottomProxy.boxoffice_parser
             url = self.urls['boxoffice']
         else:
             return []
         cont = self._retrieve(url)
         return parser.parse(cont)['data']
+
+    def _get_showtimes(self):
+        cont = self._retrieve(self.urls['showtimes'])
+        return self.stimesProxy.showtime_parser.parse(cont)['data']
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/companyParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/companyParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import re
 
 from .piculet import Path, Rule, Rules
 from .utils import DOMParserBase, analyze_imdbid, build_movie
 
-
 _re_company_name = re.compile(r'With\s+(.+)\s+\(Sorted by.*', re.I | re.M)
 
 
 def clean_company_title(title):
     """Extract company name"""
     name = _re_company_name.findall(title or '')
     if name and name[0]:
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/listParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/listParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 
 """
 This module provides the classes (and the instances) that are used to parse
 the the contents of a list.
 
-For example, when you want to parse the list "Golden Globes 2020: Trending Titles" 
+For example, when you want to parse the list "Golden Globes 2020: Trending Titles"
 the corresponding url would be:
 
 https://www.imdb.com/list/ls091843609/
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
@@ -32,14 +32,15 @@
 from imdb.utils import analyze_title
 
 from .piculet import Path, Rule, Rules, reducers
 from .utils import DOMParserBase, analyze_imdbid
 
 non_numeric_chars = ''.join(set(string.printable) - set(string.digits))
 
+
 class DOMHTMLListParser(DOMParserBase):
     """A parser for the title search page."""
 
     rules = [
         Rule(
             key='chart',
             extractor=Rules(
@@ -67,16 +68,16 @@
                     ),
                     Rule(
                         key='title',
                         extractor=Path('.//h3[@class="lister-item-header"]/a/text()')
                     ),
                     Rule(
                         key='year',
-                        extractor=Path('.//span[@class="lister-item-year text-muted unbold"]/text()', 
-                                        transform=lambda x: int(''.join(i for i in x if i.isdigit())[:4]) )
+                        extractor=Path('.//span[@class="lister-item-year text-muted unbold"]/text()',
+                                       transform=lambda x: int(''.join(i for i in x if i.isdigit())[:4]))
                     ),
                     Rule(
                         key='votes',
                         extractor=Path('.//span[@name="nv"]/@data-value', reduce=reducers.first,
                                        transform=int)
                     )
                 ]
@@ -90,21 +91,22 @@
 
         movies = []
         for entry in data['chart']:
 
             if ('movieID' not in entry) or ('rank' not in entry) or ('title' not in entry):
                 continue
 
-            movie_id = analyze_imdbid(entry['movieID']) # actually url parser to filter out id
+            movie_id = analyze_imdbid(entry['movieID'])  # actually url parser to filter out id
             if movie_id is None:
                 continue
             del entry['movieID']
 
             title = analyze_title(entry['title'])
             entry.update(title)
 
             movies.append((movie_id, entry))
         return movies
 
+
 _OBJECTS = {
     'list_parser': ((DOMHTMLListParser,), None)
 }
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/movieParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/movieParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2004-2021 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2023 Davide Alberani <da@erlug.linux.it>
 #           2008-2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -34,23 +34,22 @@
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import functools
 import re
 
-from imdb import PY2
-from imdb import imdbURL_base
+from imdb import PY2, imdbURL_base
 from imdb.Company import Company
 from imdb.Movie import Movie
 from imdb.Person import Person
-from imdb.utils import _Container, KIND_MAP
+from imdb.utils import KIND_MAP, _Container
 
-from .piculet import Path, Rule, Rules, preprocessors, transformers, ElementTree
-from .utils import DOMParserBase, analyze_imdbid, build_person, build_movie
+from .piculet import Path, Rule, Rules, preprocessors, transformers
+from .utils import DOMParserBase, analyze_imdbid, build_movie, build_person
 
 if PY2:
     from urllib import unquote
 else:
     from urllib.parse import unquote
 
 # Dictionary used to convert some section's names.
@@ -105,21 +104,23 @@
     'other companies': 'miscellaneous companies',
     'producers': 'producer',
     'special effects by': 'special effects department',
 }
 
 re_space = re.compile(r'\s+')
 
+
 def clean_section_name(section):
     """Clean and replace some section names."""
     section = re_space.sub(' ', section.replace('_', ' ').strip().lower())
     if section.endswith(' by'):
         section = section[:-3]
     return _SECT_CONV.get(section, section)
 
+
 def _manageRoles(mo):
     """Perform some transformation on the html, so that roleIDs can
     be easily retrieved."""
     firstHalf = mo.group(1)
     secondHalf = mo.group(2)
     newRoles = []
     roles = secondHalf.split(' / ')
@@ -176,20 +177,22 @@
 
 
 _re_og_title = re.compile(
     r'(.*) \((?:(?:(.+)(?= ))? ?(\d{4})(?:(–)(\d{4}| ))?|(.+))\)',
     re.UNICODE
 )
 
+
 def special_kind(og_title):
     specialKind = re.compile(r"\n(.*)").findall(og_title)
     if len(specialKind):
         return specialKind[0].strip()
     return None
 
+
 def analyze_og_title(og_title):
     data = {}
     og_kind = special_kind(og_title)
     match = _re_og_title.match(og_title)
     if og_title and not match:
         # assume it's a title in production, missing release date information
         return {'title': og_title}
@@ -269,21 +272,21 @@
         Rule(
             key='title',
             extractor=Path('//meta[@property="og:title"]/@content|//*[@id="main"]/section/div/div/ul[1]/li[5]/text()',
                            transform=analyze_og_title)
         ),
         Rule(
             key='original title',
-            extractor=Path('//div[@class="titlereference-header"]//span[@class="titlereference-original-title-label"]/preceding-sibling::text()',
+            extractor=Path('//div[@class="titlereference-header"]//span[@class="titlereference-original-title-label"]/preceding-sibling::text()',  # noqa: E501
                            transform=lambda x: re_space.sub(' ', x).strip())
 
         ),
         Rule(
             key='original title title-year',
-            extractor=Path('//div[@class="titlereference-header"]//span[@class="titlereference-title-year"]/preceding-sibling::text()',
+            extractor=Path('//div[@class="titlereference-header"]//span[@class="titlereference-title-year"]/preceding-sibling::text()',  # noqa: E501
                            transform=lambda x: re_space.sub(' ', x).strip())
         ),
         Rule(
             key='localized title',
             extractor=Path('//meta[@name="title"]/@content',
                            transform=lambda x: analyze_og_title(x).get('title'))
         ),
@@ -603,50 +606,49 @@
             extractor=Path('//a[starts-with(text(), "All Episodes")]/@href')
         ),
         Rule(
             key='akas',
             extractor=Path(
                 foreach='//i[@class="transl"]',
                 path='./text()',
-                transform=lambda x: x
-                    .replace('  ', ' ')
-                    .rstrip('-')
-                    .replace('" - ', '"::', 1)
-                    .strip('"')
-                    .replace('  ', ' ')
+                transform=lambda x: x.replace('  ', ' ')
+                                     .rstrip('-')
+                                     .replace('" - ', '"::', 1)
+                                     .strip('"')
+                                     .replace('  ', ' ')
             )
         ),
         Rule(
             key='production status',
             extractor=Path(
-                '//td[starts-with(text(), "Status:")]/..//div[@class="info-content"]//text()',
+                '//td[starts-with(text(), "Status:")]/../td[2]/text()',
                 transform=lambda x: x.strip().split('|')[0].strip().lower()
             )
         ),
         Rule(
             key='production status updated',
             extractor=Path(
                 '//td[starts-with(text(), "Status Updated:")]/'
-                '..//div[@class="info-content"]//text()',
+                '..//td[2]/text()',
                 transform=transformers.strip
             )
         ),
         Rule(
             key='production comments',
             extractor=Path(
                 '//td[starts-with(text(), "Comments:")]/'
-                '..//div[@class="info-content"]//text()',
+                '..//td[2]/text()',
                 transform=transformers.strip
             )
         ),
         Rule(
             key='production note',
             extractor=Path(
                 '//td[starts-with(text(), "Note:")]/'
-                '..//div[@class="info-content"]//text()',
+                '..//td[2]/text()',
                 transform=transformers.strip
             )
         ),
         Rule(
             key='companies',
             extractor=Rules(
                 foreach="//ul[@class='simpleList']",
@@ -692,14 +694,19 @@
             key='cover url',
             extractor=Path('//img[@alt="Poster"]/@src')
         ),
         Rule(
             key='imdbID',
             extractor=Path('//meta[@property="pageId"]/@content',
                            transform=lambda x: (x or '').replace('tt', ''))
+        ),
+        Rule(
+            key='videos',
+            extractor=Path(foreach='//div[@class="mediastrip_big"]//a',
+                           path='./@href', transform=lambda x: 'http://www.imdb.com' + x)
         )
     ]
 
     preprocessors = [
         ('/releaseinfo">', '"><span imdbpy="airdate">'),
         (re.compile(r'(<b class="blackcatheader">.+?</b>)', re.I), r'</div><div>\1'),
         ('<small>Full cast and crew for<br>', ''),
@@ -826,15 +833,15 @@
                                            accessSystem=self._as,
                                            modFunct=self._modFunct)
                 data['episode of']['kind'] = 'tv series'
                 del data['tv series title']
             del data['tv series link']
         if 'rating' in data:
             try:
-                data['rating'] = float(data['rating'].replace('/10', ''))
+                data['rating'] = float(data['rating'].replace('/10', '').replace(',', '.'))
             except (TypeError, ValueError):
                 pass
             if data['rating'] == 0:
                 del data['rating']
         if 'votes' in data:
             try:
                 votes = data['votes'].replace('(', '').replace(')', '').replace(',', '').replace('votes', '')
@@ -872,47 +879,36 @@
 
     Example::
 
         pparser = HTMLPlotParser()
         result = pparser.parse(plot_summary_html_string)
     """
     _defGetRefs = True
-    def synopsis_reducer(nodes):
-      ret=[]
-      for n in nodes:
-        if 'ElementUnicodeResult' in n.__class__.__name__:
-          ret.append(n)
-      return '\n\n'.join(ret)
 
     # Notice that recently IMDb started to put the email of the
     # author only in the link, that we're not collecting, here.
     rules = [
         Rule(
             key='plot',
             extractor=Rules(
-                foreach='//ul[@id="plot-summaries-content"]/li',
+                foreach='//div[@data-testid="sub-section-summaries"]//li',
                 rules=[
                     Rule(
                         key='plot',
-                        extractor=Path('./p//text()')
+                        extractor=Path('.//text()')
                     ),
-                    Rule(
-                        key='author',
-                        extractor=Path('.//div[@class="author-container"]//a/text()')
-                    )
                 ],
                 transform=_process_plotsummary
             )
         ),
         Rule(
             key='synopsis',
             extractor=Path(
-                foreach='//ul[@id="plot-synopsis-content"]',
-                path='.//li//node()',
-                reduce=synopsis_reducer
+                foreach='//div[@data-testid="sub-section-synopsis"]//li',
+                path='.//text()'
             )
         )
     ]
 
     def preprocess_dom(self, dom):
         preprocessors.remove(dom, '//li[@id="no-summary-content"]')
         return dom
@@ -999,28 +995,28 @@
                 transform=_process_award
             )
         ),
         Rule(
             key='recipients',
             extractor=Rules(
                 foreach='//*[@id="main"]/div[1]/div/table//tr/td[2]/a',
-                            rules=[
-                                Rule(
-                                    key='name',
-                                    extractor=Path('./text()')
-                                ),
-                                Rule(
-                                    key='link',
-                                    extractor=Path('./@href')
-                                ),
-                                Rule(
-                                    key='anchor',
-                                    extractor=Path('./ancestor::tr//text()')
-                                )
-                            ]
+                rules=[
+                    Rule(
+                        key='name',
+                        extractor=Path('./text()')
+                    ),
+                    Rule(
+                        key='link',
+                        extractor=Path('./@href')
+                    ),
+                    Rule(
+                        key='anchor',
+                        extractor=Path('./ancestor::tr//text()')
+                    )
+                ]
             )
         )
     ]
 
     preprocessors = [
         (re.compile('(<tr><td[^>]*>.*?</td></tr>\n\n</table>)', re.I),
          r'\1</table>'),
@@ -1070,15 +1066,14 @@
                 award['for'] = recipients
             nd.append(award)
             if 'anchor' in award:
                 del award['anchor']
         return {'awards': nd}
 
 
-
 class DOMHTMLTaglinesParser(DOMParserBase):
     """Parser for the "taglines" page of a given movie.
     The page should be provided as a string, as taken from
     the www.imdb.com server.  The final result will be a
     dictionary, with a key for every relevant section.
 
     Example::
@@ -1086,25 +1081,20 @@
         tparser = DOMHTMLTaglinesParser()
         result = tparser.parse(taglines_html_string)
     """
     rules = [
         Rule(
             key='taglines',
             extractor=Path(
-                foreach='//div[@id="taglines_content"]/div',
+                foreach='//div[@class="ipc-html-content-inner-div"]',
                 path='.//text()'
             )
         )
     ]
 
-    def preprocess_dom(self, dom):
-        preprocessors.remove(dom, '//div[@id="taglines_content"]/div[@class="header"]')
-        preprocessors.remove(dom, '//div[@id="taglines_content"]/div[@id="no_content"]')
-        return dom
-
     def postprocess_data(self, data):
         if 'taglines' in data:
             data['taglines'] = [tagline.strip() for tagline in data['taglines']]
         return data
 
 
 class DOMHTMLKeywordsParser(DOMParserBase):
@@ -1127,37 +1117,36 @@
                 transform=lambda x: x.lower().replace(' ', '-')
             )
         ),
         Rule(
             key='relevant keywords',
             extractor=Rules(
                 foreach='//td[@data-item-keyword]',
-                            rules=[
-                                Rule(
-                                    key='keyword',
-                                    extractor=Path('./@data-item-keyword')
-                                ),
-                                Rule(
-                                    key='ordering',
-                                    extractor=Path('./@data-item-votes')
-                                ),
-                                Rule(
-                                    key='vote_str',
-                                    extractor=Path('./div[2]/div//text()')
-                                )
-                            ],
-                            transform=lambda x: {
-                                'keyword': x.get('keyword').lower(),
-                                'keyword_dash': x.get('keyword').lower().replace(' ', '-'),
-                                'ordering': x.get('ordering'),
-                                'votes_str': x.get('vote_str').strip().lower()
-                            }
+                rules=[
+                    Rule(
+                        key='keyword',
+                        extractor=Path('./@data-item-keyword')
+                    ),
+                    Rule(
+                        key='ordering',
+                        extractor=Path('./@data-item-votes')
+                    ),
+                    Rule(
+                        key='vote_str',
+                        extractor=Path('./div[2]/div//text()')
+                    )
+                ],
+                transform=lambda x: {
+                    'keyword': x.get('keyword').lower(),
+                    'keyword_dash': x.get('keyword').lower().replace(' ', '-'),
+                    'ordering': x.get('ordering'),
+                    'votes_str': x.get('vote_str').strip().lower()
+                }
             )
         )
-
     ]
 
     def postprocess_data(self, data):
         if 'relevant keywords' in data:
             rk = []
             for x in data['relevant keywords']:
                 if 'votes_str' in x:
@@ -1376,19 +1365,18 @@
 
     rules = [
         Rule(
             key='quotes',
             extractor=Path(
                 foreach='//div[@class="sodatext"]',
                 path='.//text()',
-                transform=lambda x: x
-                    .strip()
-                    .replace(' \n', '::')
-                    .replace('::\n', '::')
-                    .replace('\n', ' ')
+                transform=lambda x: x.strip()
+                                     .replace(' \n', '::')
+                                     .replace('::\n', '::')
+                                     .replace('\n', ' ')
             )
         )
     ]
 
     def preprocess_dom(self, dom):
         preprocessors.remove(dom, '//div[@class="did-you-know-actions"]')
         return dom
@@ -1860,34 +1848,34 @@
     Example::
 
         osparser = DOMHTMLOfficialsitesParser()
         result = osparser.parse(officialsites_html_string)
     """
     rules = [
         Rule(
-            foreach='//h4[@class="li_group"]',
+            foreach='//div[contains(@class, "ipc-page-grid__item")]/section[contains(@class, "ipc-page-section--base")]',
             key=Path(
-                './text()',
+                './/h3//text()',
                 transform=lambda x: x.strip().lower()
             ),
             extractor=Rules(
-                foreach='./following::ul[1]/li/a',
+                foreach='.//ul[1]//li//a[1]',
                 rules=[
                     Rule(
                         key='link',
                         extractor=Path('./@href')
                     ),
                     Rule(
                         key='info',
-                        extractor=Path('./text()')
+                        extractor=Path('.//text()')
                     )
                 ],
                 transform=lambda x: (
-                    x.get('info').strip(),
-                    unquote(_normalize_href(x.get('link')))
+                    x.get('info', '').strip(),
+                    unquote(x.get('link'))
                 )
             )
         )
     ]
 
 
 class DOMHTMLConnectionsParser(DOMParserBase):
@@ -1897,40 +1885,36 @@
     dictionary, with a key for every relevant section.
 
     Example::
 
         osparser = DOMHTMLOfficialsitesParser()
         result = osparser.parse(officialsites_html_string)
     """
-    preprocessors = [
-        (re.compile('(<h4 class="li_group">)', re.I), r'</div><div class="_imdbpy">\1'),
-        (re.compile('(^<br />.*$)', re.I | re.M), r''),
-    ]
     rules = [
         Rule(
-            foreach='//div[@class="_imdbpy"]',
+            foreach='//div[contains(@class, "ipc-page-grid__item")]/section[contains(@class, "ipc-page-section--base")]',
             key=Path(
-                './h4/text()',
-                transform=lambda x: x.strip().lower()
+                './div[1]//h3//text()',
+                transform=lambda x: (x or '').strip().lower()
             ),
             extractor=Rules(
-                foreach='./div[contains(@class, "soda")]',
+                foreach='./div[2]//ul[1]//li',
                 rules=[
                     Rule(
                         key='link',
-                        extractor=Path('./a/@href')
+                        extractor=Path('./div[1]//p//a/@href')
                     ),
                     Rule(
                         key='info',
-                        extractor=Path('.//text()')
+                        extractor=Path('./div[1]//p//text()')
                     )
                 ],
                 transform=lambda x: (
-                    x.get('info').strip(),
-                    unquote(_normalize_href(x.get('link')))
+                    x.get('info', '').strip(),
+                    unquote(_normalize_href(x.get('link', '')))
                 )
             )
         )
     ]
 
     def postprocess_data(self, data):
         connections = {}
@@ -1941,20 +1925,21 @@
             movies = []
             for title, link in v:
                 title = title.strip().replace('\n', '')
                 movieID = analyze_imdbid(link)
                 if not (title and movieID):
                     continue
                 movie = Movie(title=title, movieID=movieID,
-                       accessSystem=self._as, modFunct=self._modFunct)
+                              accessSystem=self._as, modFunct=self._modFunct)
                 movies.append(movie)
             if movies:
                 connections[k] = movies
         return {'connections': connections}
 
+
 class DOMHTMLLocationsParser(DOMParserBase):
     """Parser for the "locations" page of a given movie.
     The page should be provided as a string, as taken from
     the www.imdb.com server.  The final result will be a
     dictionary, with a key for every relevant section.
 
     Example::
@@ -2648,42 +2633,82 @@
             )
         ),
         Rule(
             key='advisories',
             extractor=Rules(
                 foreach='//section[starts-with(@id, "advisory-")]',
                 rules=[
+                    Rule(
+                        key='section',
+                        extractor=Path('./@id')
+                    ),
+                    Rule(
+                        key='items',
+                        extractor=Rules(
+                            foreach='.//li',
+                            rules=[
+                                Rule(
+                                    key='item',
+                                    extractor=Path('./text()')
+                                )
+                            ],
+                            transform=lambda x: x.get('item').strip()
+                        )
+                    )
+                ]
+            )
+        ),
+        Rule(
+            key='advisory votes',
+            extractor=Rules(
+                foreach='//section[starts-with(@id, "advisory-")][not(contains(@id, "advisory-spoiler"))]',
+                rules=[
                     Rule(key='section',
-                         extractor=Path('./@id')
+                         extractor=Path('./@id'),
+                         ),
+                    Rule(key='status',
+                         extractor=Path('.//li[1]//div[contains(@class, "ipl-swapper__content-primary")]//span/text()')
                          ),
-                    Rule(key='items',
-                         extractor=Rules(
-                             foreach='.//li',
-                             rules=[
-                                 Rule(
-                                     key='item',
-                                     extractor=Path('./text()')
-                                 )
-                             ],
-                             transform=lambda x: x.get('item').strip()
+                    Rule(key='votes',
+                         extractor=Path(
+                             foreach='.//li[1]//span[contains(@class, "ipl-vote-button__details")]',
+                             path='./text()',
+                             transform=lambda x: int(x.replace(',', ''))
+                         )
                          )
-                    )
                 ]
             )
         )
     ]
 
     def postprocess_data(self, data):
         if 'advisories' in data:
             for advisory in data['advisories']:
                 sect = advisory.get('section', '').replace('-', ' ')
                 items = [x for x in advisory.get('items', []) if x]
                 if sect and items:
                     data[sect] = items
             del data['advisories']
+
+        if 'advisory votes' in data:
+            advisory_votes = {}
+            for vote in data['advisory votes']:
+                if 'status' not in vote or 'votes' not in vote:
+                    continue
+                advisory_votes[vote['section'][9:]] = {
+                    'votes': {
+                        'None': vote['votes'][0],
+                        'Mild': vote['votes'][1],
+                        'Moderate': vote['votes'][2],
+                        'Severe': vote['votes'][3],
+                    },
+                    'status': vote['status'],
+                }
+            data['advisory votes'] = advisory_votes
+
         return data
 
 
 _OBJECTS = {
     'movie_parser': ((DOMHTMLMovieParser,), None),
     'full_credits_parser': ((DOMHTMLFullCreditsParser,), None),
     'plot_parser': ((DOMHTMLPlotParser,), None),
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/personParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/personParser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2020 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2022 Davide Alberani <da@erlug.linux.it>
 #           2008-2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -32,30 +32,24 @@
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import re
 
 from imdb.utils import analyze_name
 
-from .movieParser import (
-    DOMHTMLAwardsParser,
-    DOMHTMLNewsParser,
-    DOMHTMLOfficialsitesParser,
-    DOMHTMLTechParser
-)
+from .movieParser import DOMHTMLNewsParser, DOMHTMLOfficialsitesParser, DOMHTMLTechParser
 from .piculet import Path, Rule, Rules, transformers
 from .utils import DOMParserBase, analyze_imdbid, build_movie, build_person
 
-
 _re_spaces = re.compile(r'\s+')
 _reRoles = re.compile(r'(<li>.*? \.\.\.\. )(.*?)(</li>|<br>)', re.I | re.M | re.S)
 
 
 class DOMHTMLMaindetailsParser(DOMParserBase):
-    """Parser for the "categorized" (maindetails) page of a given person.
+    """Parser for the "maindetails" page of a given person.
     The page should be provided as a string, as taken from
     the www.imdb.com server.  The final result will be a
     dictionary, with a key for every relevant section.
 
     Example::
 
         cparser = DOMHTMLMaindetailsParser()
@@ -82,58 +76,23 @@
         ),
         Rule(
             key='death place',
             extractor=Path('.//a[starts-with(@href, "/search/name?death_place=")]/text()')
         )
     ]
 
-    _film_rules = [
-        Rule(
-            key='link',
-            extractor=Path('./b/a[1]/@href')
-        ),
-        Rule(
-            key='title',
-            extractor=Path('./b/a[1]/text()')
-        ),
-        Rule(
-            key='notes',
-            extractor=Path('./b/following-sibling::text()')
-        ),
-        Rule(
-            key='year',
-            extractor=Path('./span[@class="year_column"]/text()')
-        ),
-        Rule(
-            key='status',
-            extractor=Path('./a[@class="in_production"]/text()')
-        ),
-        Rule(
-            key='rolesNoChar',
-            extractor=Path('.//br/following-sibling::text()')
-        ),
-        Rule(
-            key='chrRoles',
-            extractor=Path('./a[@imdbpyname]/@imdbpyname')
-        )
-    ]
-
     rules = [
         Rule(
             key='name',
             extractor=Path(
-                '//h1[@class="header"]//text()',
+                '//h1[@data-testid="hero__pageTitle"]//text()',
                 transform=lambda x: analyze_name(x)
             )
         ),
         Rule(
-            key='name_index',
-            extractor=Path('//h1[@class="header"]/span[1]/text()')
-        ),
-        Rule(
             key='birth info',
             extractor=Rules(
                 section='//div[h4="Born:"]',
                 rules=_birth_rules
             )
         ),
         Rule(
@@ -141,51 +100,24 @@
             extractor=Rules(
                 section='//div[h4="Died:"]',
                 rules=_death_rules,
             )
         ),
         Rule(
             key='headshot',
-            extractor=Path('//td[@id="img_primary"]//div[@class="image"]/a/img/@src')
+            extractor=Path('(//section[contains(@class, "ipc-page-section")])[1]//div[contains(@class, "ipc-poster")]/img[@class="ipc-image"]/@src')  # noqa: E501
         ),
         Rule(
             key='akas',
             extractor=Path(
                 '//div[h4="Alternate Names:"]/text()',
                 transform=lambda x: x.strip().split('  ')
             )
         ),
         Rule(
-            key='filmography',
-            extractor=Rules(
-                foreach='//div[starts-with(@id, "filmo-head-")]',
-                rules=[
-                    Rule(
-                        key=Path(
-                            './a[@name]/text()',
-                            transform=lambda x: x.lower().replace(': ', ' ')
-                        ),
-                        extractor=Rules(
-                            foreach='./following-sibling::div[1]/div[starts-with(@class, "filmo-row")]',
-                            rules=_film_rules,
-                            transform=lambda x: build_movie(
-                                x.get('title') or '',
-                                year=x.get('year'),
-                                movieID=analyze_imdbid(x.get('link') or ''),
-                                rolesNoChar=(x.get('rolesNoChar') or '').strip(),
-                                chrRoles=(x.get('chrRoles') or '').strip(),
-                                additionalNotes=x.get('notes'),
-                                status=x.get('status') or None
-                            )
-                        )
-                    )
-                ]
-            )
-        ),
-        Rule(
             key='in development',
             extractor=Rules(
                 foreach='//div[starts-with(@class,"devitem")]',
                 rules=[
                     Rule(
                         key='link',
                         extractor=Path('./a/@href')
@@ -201,56 +133,130 @@
                     roleID=(x.get('roleID') or '').split('/'),
                     status=x.get('status') or None
                 )
             )
         ),
         Rule(
             key='imdbID',
-            extractor=Path('//meta[@property="pageId"]/@content',
-                           transform=lambda x: (x or '').replace('nm', ''))
+            extractor=Path('//meta[@property="og:url"]/@content',
+                           transform=analyze_imdbid)
         )
     ]
 
     preprocessors = [
         ('<div class="clear"/> </div>', ''), ('<br/>', '<br />')
     ]
 
     def postprocess_data(self, data):
-        filmo = {}
-        for job in (data.get('filmography') or []):
-            if not isinstance(job, dict) or not job:
-                continue
-            filmo.update(job)
-        if filmo:
-            data['filmography'] = filmo
         for key in ['name']:
             if (key in data) and isinstance(data[key], dict):
                 subdata = data[key]
                 del data[key]
                 data.update(subdata)
         for what in 'birth date', 'death date':
             if what in data and not data[what]:
                 del data[what]
-        name_index = (data.get('name_index') or '').strip()
-        if name_index:
-            if self._name_imdb_index.match(name_index):
-                data['imdbIndex'] = name_index[1:-1]
-            del data['name_index']
         # XXX: the code below is for backwards compatibility
         # probably could be removed
         for key in list(data.keys()):
             if key == 'birth place':
                 data['birth notes'] = data[key]
                 del data[key]
             if key == 'death place':
                 data['death notes'] = data[key]
                 del data[key]
         return data
 
 
+class DOMHTMLFilmographyParser(DOMParserBase):
+    """Parser for the "full credits" page of a given person.
+    The page should be provided as a string, as taken from
+    the www.imdb.com server.
+
+    Example::
+
+        filmo_parser = DOMHTMLFilmographyParser()
+        result = filmo_parser.parse(fullcredits_html_string)
+    """
+    _defGetRefs = True
+
+    _film_rules = [
+        Rule(
+            key='link',
+            extractor=Path('.//b/a/@href')
+        ),
+        Rule(
+            key='title',
+            extractor=Path('.//b/a/text()')
+        ),
+        # TODO: Notes not migrated yet
+        Rule(
+            key='notes',
+            extractor=Path('.//div[@class="ipc-metadata-list-summary-item__c"]//ul[contains(@class, "ipc-metadata-list-summary-item__stl")]//label/text()')  # noqa: E501
+        ),
+        Rule(
+            key='year',
+            extractor=Path(
+                './/span[@class="year_column"]//text()',
+                transform=lambda x: x.strip(),
+            ),
+        ),
+        Rule(
+            key='status',
+            extractor=Path('./a[@class="in_production"]/text()')
+        ),
+        Rule(
+            key='rolesNoChar',
+            extractor=Path(
+                './/br/following-sibling::text()',
+                transform=lambda x: x.strip(),
+            ),
+        )
+    ]
+
+    rules = [
+        Rule(
+            key='filmography',
+            extractor=Rules(
+                foreach='//div[contains(@id, "filmo-head-")]',
+                rules=[
+                    Rule(
+                        key=Path(
+                            './/a/text()',
+                            transform=lambda x: x.lower()
+                        ),
+                        extractor=Rules(
+                            foreach='./following-sibling::div[1]/div[contains(@class, "filmo-row")]',
+                            rules=_film_rules,
+                            transform=lambda x: build_movie(
+                                x.get('title') or '',
+                                year=x.get('year'),
+                                movieID=analyze_imdbid(x.get('link') or ''),
+                                rolesNoChar=(x.get('rolesNoChar') or '').strip(),
+                                additionalNotes=x.get('notes'),
+                                status=x.get('status') or None
+                            )
+                        )
+                    )
+                ]
+            )
+        )
+    ]
+
+    def postprocess_data(self, data):
+        filmo = {}
+        for job in (data.get('filmography') or []):
+            if not isinstance(job, dict) or not job:
+                continue
+            filmo.update(job)
+        if filmo:
+            data['filmography'] = filmo
+        return data
+
+
 class DOMHTMLBioParser(DOMParserBase):
     """Parser for the "biography" page of a given person.
     The page should be provided as a string, as taken from
     the www.imdb.com server.  The final result will be a
     dictionary, with a key for every relevant section.
 
     Example::
@@ -528,14 +534,15 @@
     ]
 
     def postprocess_data(self, data):
         if len(data) == 0:
             return {}
         return {self.kind: data}
 
+
 def _process_person_award(x):
     awards = {}
     movies = x.get('movies')
     year = x.get('year')
     result = x.get('result')
     prize = x.get('prize')
     category = x.get('category')
@@ -579,46 +586,50 @@
                     Rule(
                         key='prize',
                         extractor=Path('.//span[@class="award_category"]/text()')
                     ),
                     Rule(
                         key='movies',
                         foreach='./td[@class="award_description"]/a',
-                        extractor=Rules([
-                            Rule(
-                                key='title',
-                                extractor=Path('./text()')
-                            ),
-                            Rule(
-                                key='link',
-                                extractor=Path('./@href')
-                            ),
-                            Rule(
-                                key='year',
-                                extractor=Path('./following-sibling::span[@class="title_year"][1]/text()')
+                        extractor=Rules(
+                            [
+                                Rule(
+                                    key='title',
+                                    extractor=Path('./text()')
+                                ),
+                                Rule(
+                                    key='link',
+                                    extractor=Path('./@href')
+                                ),
+                                Rule(
+                                    key='year',
+                                    extractor=Path('./following-sibling::span[@class="title_year"][1]/text()')
+                                )
+                            ],
+                            transform=lambda x: build_movie(
+                                x.get('title') or '',
+                                movieID=analyze_imdbid(x.get('link')),
+                                year=x.get('year')
                             )
-                        ],
-                        transform=lambda x: build_movie(
-                            x.get('title') or '',
-                            movieID=analyze_imdbid(x.get('link')),
-                            year=x.get('year')
                         )
-                    )),
+                    ),
                     Rule(
                         key='shared with',
                         foreach='./td[@class="award_description"]/div[@class="shared_with"]/following-sibling::ul//a',
-                        extractor=Rules([
-                            Rule(
-                                key='name',
-                                extractor=Path('./text()')
-                            ),
-                            Rule(
-                                key='link',
-                                extractor=Path('./@href')
-                            )],
+                        extractor=Rules(
+                            [
+                                Rule(
+                                    key='name',
+                                    extractor=Path('./text()')
+                                ),
+                                Rule(
+                                    key='link',
+                                    extractor=Path('./@href')
+                                )
+                            ],
                             transform=lambda x: build_person(
                                 x.get('name') or '',
                                 personID=analyze_imdbid(x.get('link'))
                             )
                         )
                     ),
                     Rule(
@@ -635,14 +646,15 @@
         )
     ]
 
 
 _OBJECTS = {
     'maindetails_parser': ((DOMHTMLMaindetailsParser,), None),
     'bio_parser': ((DOMHTMLBioParser,), None),
+    'filmo_parser': ((DOMHTMLFilmographyParser,), None),
     'otherworks_parser': ((DOMHTMLOtherWorksParser,), None),
     'person_officialsites_parser': ((DOMHTMLOfficialsitesParser,), None),
     'person_awards_parser': ((DOMHTMLPersonAwardsParser,), None),
     'publicity_parser': ((DOMHTMLTechParser,), {'kind': 'publicity'}),
     'person_contacts_parser': ((DOMHTMLTechParser,), {'kind': 'contacts'}),
     'person_genres_parser': ((DOMHTMLPersonGenresParser,), None),
     'person_keywords_parser': ((DOMHTMLPersonGenresParser,), {'kind': 'keywords'}),
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/piculet.py` & `cinemagoer-2023.5.1/imdb/parser/http/piculet.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2018 H. Turgut Uyar <uyar@tekir.org>
+# Copyright (C) 2014-2022 H. Turgut Uyar <uyar@tekir.org>
 #
 # Piculet is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Piculet is distributed in the hope that it will be useful,
@@ -22,42 +22,39 @@
 For more information, please refer to the documentation:
 https://piculet.readthedocs.io/
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import json
-import os
 import re
 import sys
 from argparse import ArgumentParser
 from collections import deque
 from functools import partial
 from operator import itemgetter
 from pkgutil import find_loader
 
+__version__ = '1.2b1'
 
 PY2 = sys.version_info < (3, 0)
 
-
 if PY2:
     str, bytes = unicode, str
 
-
 if PY2:
     from cgi import escape as html_escape
+    from htmlentitydefs import name2codepoint  # noqa: I003
     from HTMLParser import HTMLParser
     from StringIO import StringIO
-    from htmlentitydefs import name2codepoint
-    from urllib2 import urlopen
 else:
     from html import escape as html_escape
     from html.parser import HTMLParser
     from io import StringIO
-    from urllib.request import urlopen
+    from types import MappingProxyType
 
 
 if PY2:
     from contextlib import contextmanager
 
     @contextmanager
     def redirect_stdout(new_stdout):
@@ -66,59 +63,20 @@
         try:
             yield new_stdout
         finally:
             sys.stdout = old_stdout
 else:
     from contextlib import redirect_stdout
 
-from imdb.parser.http.logging import logger
-
-_logger = logger.getChild('piculet')
-
 
 ###########################################################
 # HTML OPERATIONS
 ###########################################################
 
 
-# TODO: this is too fragile
-_CHARSET_TAGS = [
-    b'<meta http-equiv="content-type" content="text/html; charset=',
-    b'<meta charset="'
-]
-
-
-def decode_html(content, charset=None, fallback_charset='utf-8'):
-    """Decode an HTML document according to a character set.
-
-    If no character set is given, this will try to figure it out
-    from the corresponding ``meta`` tags.
-
-    :sig: (bytes, Optional[str], Optional[str]) -> str
-    :param content: Content of HTML document to decode.
-    :param charset: Character set of the page.
-    :param fallback_charset: Character set to use if it can't be figured out.
-    :return: Decoded content of the document.
-    """
-    if charset is None:
-        for tag in _CHARSET_TAGS:
-            start = content.find(tag)
-            if start >= 0:
-                charset_start = start + len(tag)
-                charset_end = content.find(b'"', charset_start)
-                charset = content[charset_start:charset_end].decode('ascii')
-                _logger.debug('charset found in "meta": "%s"', charset)
-                break
-        else:
-            _logger.debug('charset not found, using fallback: "%s"', fallback_charset)
-            charset = fallback_charset
-    _logger.debug('decoding for charset: "%s"', charset)
-    return content.decode(charset)
-
-
 class HTMLNormalizer(HTMLParser):
     """HTML cleaner and XHTML convertor.
 
     DOCTYPE declarations and comments are removed.
     """
 
     SELF_CLOSING_TAGS = {'br', 'hr', 'img', 'input', 'link', 'meta'}
@@ -140,35 +98,29 @@
         self.omit_attrs = set(omit_attrs) if omit_attrs is not None else set()  # sig: Set[str]
 
         # stacks used during normalization
         self._open_tags = deque()
         self._open_omitted_tags = deque()
 
     def handle_starttag(self, tag, attrs):
-        """Process the starting of a new element."""
         if tag in self.omit_tags:
-            _logger.debug('omitting: "%s"', tag)
             self._open_omitted_tags.append(tag)
         if not self._open_omitted_tags:
             # stack empty -> not in omit mode
             if '@' in tag:
                 # email address in angular brackets
                 print('&lt;%s&gt;' % tag, end='')
                 return
             if (tag == 'li') and (self._open_tags[-1] == 'li'):
-                _logger.debug('opened "li" without closing previous "li", adding closing tag')
                 self.handle_endtag('li')
             attributes = []
             for attr_name, attr_value in attrs:
                 if attr_name in self.omit_attrs:
-                    _logger.debug('omitting "%s" attribute of "%s"', attr_name, tag)
                     continue
                 if attr_value is None:
-                    _logger.debug('no value for "%s" attribute of "%s", adding empty value',
-                                  attr_name, tag)
                     attr_value = ''
                 markup = '%(name)s="%(value)s"' % {
                     'name': attr_name,
                     'value': html_escape(attr_value, quote=True)
                 }
                 attributes.append(markup)
             line = '<%(tag)s%(attrs)s%(slash)s>' % {
@@ -177,56 +129,49 @@
                 'slash': ' /' if tag in self.SELF_CLOSING_TAGS else ''
             }
             print(line, end='')
             if tag not in self.SELF_CLOSING_TAGS:
                 self._open_tags.append(tag)
 
     def handle_endtag(self, tag):
-        """Process the ending of an element."""
         if not self._open_omitted_tags:
             # stack empty -> not in omit mode
             if tag not in self.SELF_CLOSING_TAGS:
                 last = self._open_tags[-1]
                 if (tag == 'ul') and (last == 'li'):
-                    _logger.debug('closing "ul" without closing last "li", adding closing tag')
                     self.handle_endtag('li')
                 if tag == last:
                     # expected end tag
                     print('</%(tag)s>' % {'tag': tag}, end='')
                     self._open_tags.pop()
                 elif tag not in self._open_tags:
-                    _logger.debug('closing tag "%s" without opening tag', tag)
                     # XXX: for <a><b></a></b>, this case gets invoked after the case below
+                    pass
                 elif tag == self._open_tags[-2]:
-                    _logger.debug('unexpected closing tag "%s" instead of "%s", closing both',
-                                  tag, last)
                     print('</%(tag)s>' % {'tag': last}, end='')
                     print('</%(tag)s>' % {'tag': tag}, end='')
                     self._open_tags.pop()
                     self._open_tags.pop()
         elif (tag in self.omit_tags) and (tag == self._open_omitted_tags[-1]):
             # end of expected omitted tag
             self._open_omitted_tags.pop()
 
     def handle_data(self, data):
-        """Process collected character data."""
         if not self._open_omitted_tags:
             # stack empty -> not in omit mode
             line = html_escape(data)
             print(line.decode('utf-8') if PY2 and isinstance(line, bytes) else line, end='')
 
     def handle_entityref(self, name):
-        """Process an entity reference."""
         # XXX: doesn't get called if convert_charrefs=True
         num = name2codepoint.get(name)  # we are sure we're on PY2 here
         if num is not None:
             print('&#%(ref)d;' % {'ref': num}, end='')
 
     def handle_charref(self, name):
-        """Process a character reference."""
         # XXX: doesn't get called if convert_charrefs=True
         print('&#%(ref)s;' % {'ref': name}, end='')
 
     # def feed(self, data):
         # super().feed(data)
         # # close all remaining open tags
         # for tag in reversed(self._open_tags):
@@ -255,15 +200,14 @@
 
 
 # sigalias: XPathResult = Union[Sequence[str], Sequence[Element]]
 
 
 _USE_LXML = find_loader('lxml') is not None
 if _USE_LXML:
-    _logger.info('using lxml')
     from lxml import etree as ElementTree
     from lxml.etree import Element
 
     XPath = ElementTree.XPath
     xpath = ElementTree._Element.xpath
 else:
     from xml.etree import ElementTree
@@ -323,15 +267,15 @@
             :return: Elements or strings resulting from the query.
             """
             return self._apply(element)
 
     xpath = lambda e, p: XPath(p)(e)
 
 
-_EMPTY = {}     # empty result singleton
+_EMPTY = {} if PY2 else MappingProxyType({})  # empty result singleton
 
 
 # sigalias: Reducer = Callable[[Sequence[str]], str]
 # sigalias: PathTransformer = Callable[[str], Any]
 # sigalias: MapTransformer = Callable[[Mapping[str, Any]], Any]
 # sigalias: Transformer = Union[PathTransformer, MapTransformer]
 # sigalias: ExtractedItem = Union[str, Mapping[str, Any]]
@@ -448,23 +392,19 @@
     def apply(self, element):
         """Apply this extractor to an element.
 
         :sig: (Element) -> str
         :param element: Element to apply this extractor to.
         :return: Extracted text.
         """
-        # _logger.debug('applying path "%s" on "%s" element', self.path, element.tag)
         selected = self.path(element)
         if len(selected) == 0:
-            # _logger.debug('no match')
             value = None
         else:
-            # _logger.debug('selected elements: "%s"', selected)
             value = self.reduce(selected)
-            # _logger.debug('reduced using "%s": "%s"', self.reduce, value)
         return value
 
 
 class Rules(Extractor):
     """An extractor for getting data items out of an XML element."""
 
     def __init__(self, rules, section=None, transform=None, foreach=None):
@@ -501,20 +441,18 @@
         :return: Extracted mapping.
         """
         if self.section is None:
             subroot = element
         else:
             subroots = self.section(element)
             if len(subroots) == 0:
-                _logger.debug('No section root found')
                 return _EMPTY
             if len(subroots) > 1:
                 raise ValueError('Section path should select exactly one element')
             subroot = subroots[0]
-            _logger.debug('Moving root to %s element', subroot.tag)
 
         data = {}
         for rule in self.rules:
             extracted = rule.extract(subroot)
             data.update(extracted)
         return data if len(data) > 0 else _EMPTY
 
@@ -558,40 +496,31 @@
         :sig: (Element) -> Mapping[str, Any]
         :param element: Element to extract the data from.
         :return: Extracted data.
         """
         data = {}
         subroots = [element] if self.foreach is None else self.foreach(element)
         for subroot in subroots:
-            # _logger.debug('setting section element to: "%s"', section.tag)
-
             key = self.key if isinstance(self.key, str) else self.key.extract(subroot)
             if key is None:
-                # _logger.debug('no value generated for key name')
                 continue
-            # _logger.debug('extracting key: "%s"', key)
-
             if self.extractor.foreach is None:
                 value = self.extractor.extract(subroot)
                 if (value is None) or (value is _EMPTY):
-                    # _logger.debug('no value generated for key')
                     continue
                 data[key] = value
-                # _logger.debug('extracted value for "%s": "%s"', key, data[key])
             else:
                 # don't try to transform list items by default, it might waste a lot of time
                 raw_values = [self.extractor.extract(r, transform=False)
                               for r in self.extractor.foreach(subroot)]
                 values = [v for v in raw_values if (v is not None) and (v is not _EMPTY)]
                 if len(values) == 0:
-                    # _logger.debug('no items found in list')
                     continue
                 data[key] = values if self.extractor.transform is None else \
                     list(map(self.extractor.transform, values))
-                # _logger.debug('extracted value for "%s": "%s"', key, data[key])
         return data
 
 
 def remove_elements(root, path):
     """Remove selected elements from the tree.
 
     :sig: (Element, str) -> None
@@ -603,18 +532,16 @@
     else:
         # ElementTree doesn't support parent queries, so we'll build a map for it
         get_parent = root.attrib.get('_get_parent')
         if get_parent is None:
             get_parent = {e: p for p in root.iter() for e in p}.get
             root.attrib['_get_parent'] = get_parent
     elements = XPath(path)(root)
-    _logger.debug('removing %s elements using path: "%s"', len(elements), path)
     if len(elements) > 0:
         for element in elements:
-            _logger.debug('removing element: "%s"', element.tag)
             # XXX: could this be hazardous? parent removed in earlier iteration?
             get_parent(element).remove(element)
 
 
 def set_element_attr(root, path, name, value):
     """Set an attribute for selected elements.
 
@@ -627,62 +554,54 @@
         ) -> None
     :param root: Root element of the tree.
     :param path: XPath to select the elements to set attributes for.
     :param name: Description for name generation.
     :param value: Description for value generation.
     """
     elements = XPath(path)(root)
-    _logger.debug('updating %s elements using path: "%s"', len(elements), path)
     for element in elements:
         attr_name = name if isinstance(name, str) else \
             Extractor.from_map(name).extract(element)
         if attr_name is None:
-            _logger.debug('no attribute name generated for "%s" element', element.tag)
             continue
 
         attr_value = value if isinstance(value, str) else \
             Extractor.from_map(value).extract(element)
         if attr_value is None:
-            _logger.debug('no attribute value generated for "%s" element', element.tag)
             continue
 
-        _logger.debug('setting "%s" attribute to "%s" on "%s" element',
-                      attr_name, attr_value, element.tag)
         element.attrib[attr_name] = attr_value
 
 
 def set_element_text(root, path, text):
     """Set the text for selected elements.
 
     :sig: (Element, str, Union[str, Mapping[str, Any]]) -> None
     :param root: Root element of the tree.
     :param path: XPath to select the elements to set attributes for.
     :param text: Description for text generation.
     """
     elements = XPath(path)(root)
-    _logger.debug('updating %s elements using path: "%s"', len(elements), path)
     for element in elements:
         element_text = text if isinstance(text, str) else \
             Extractor.from_map(text).extract(element)
         # note that the text can be None in which case the existing text will be cleared
-        _logger.debug('setting text to "%s" on "%s" element', element_text, element.tag)
         element.text = element_text
 
 
 def build_tree(document, force_html=False):
     """Build a tree from an XML document.
 
     :sig: (str, Optional[bool]) -> Element
     :param document: XML document to build the tree from.
     :param force_html: Force to parse from HTML without converting.
     :return: Root element of the XML tree.
     """
     content = document.encode('utf-8') if PY2 else document
     if _USE_LXML and force_html:
-        _logger.info('using lxml html builder')
         import lxml.html
         return lxml.html.fromstring(content)
     return ElementTree.fromstring(content)
 
 
 class Registry:
     """A simple, attribute-based namespace."""
@@ -806,116 +725,28 @@
 
 
 ###########################################################
 # COMMAND-LINE INTERFACE
 ###########################################################
 
 
-def h2x(source):
-    """Convert an HTML file into XHTML and print.
-
-    :sig: (str) -> None
-    :param source: Path of HTML file to convert.
-    """
-    if source == '-':
-        _logger.debug('reading from stdin')
-        content = sys.stdin.read()
-    else:
-        _logger.debug('reading from file: "%s"', os.path.abspath(source))
-        with open(source, 'rb') as f:
-            content = decode_html(f.read())
-    print(html_to_xhtml(content), end='')
-
-
-def scrape_document(address, spec, content_format='xml'):
-    """Scrape data from a file path or a URL and print.
-
-    :sig: (str, str, Optional[str]) -> None
-    :param address: File path or URL of document to scrape.
-    :param spec: Path of spec file.
-    :param content_format: Whether the content is XML or HTML.
-    """
-    _logger.debug('loading spec from file: "%s"', os.path.abspath(spec))
-    if os.path.splitext(spec)[-1] == '.yaml':
-        if find_loader('yaml') is None:
-            raise RuntimeError('YAML support not available')
-        import yaml
-        spec_loader = yaml.load
-    else:
-        spec_loader = json.loads
-
-    with open(spec) as f:
-        spec_map = spec_loader(f.read())
-
-    if address.startswith(('http://', 'https://')):
-        _logger.debug('loading url: "%s"', address)
-        with urlopen(address) as f:
-            content = f.read()
-    else:
-        _logger.debug('loading file: "%s"', os.path.abspath(address))
-        with open(address, 'rb') as f:
-            content = f.read()
-    document = decode_html(content)
-
-    if content_format == 'html':
-        _logger.debug('converting html document to xhtml')
-        document = html_to_xhtml(document)
-        # _logger.debug('=== CONTENT START ===\n%s\n=== CONTENT END===', document)
+def main():
+    parser = ArgumentParser(description="extract data from XML/HTML")
+    parser.add_argument('--version', action='version', version=__version__)
+    parser.add_argument('--html', action='store_true', help='document is in HTML format')
+    parser.add_argument('-s', '--spec', required=True, help='spec file')
+    arguments = parser.parse_args()
+
+    content = sys.stdin.read()
+    if arguments.html:
+        content = html_to_xhtml(content)
+
+    with open(arguments.spec) as f:
+        spec_content = f.read()
+    spec = json.loads(spec_content)
 
-    data = scrape(document, spec_map)
+    data = scrape(content, spec)
     print(json.dumps(data, indent=2, sort_keys=True))
 
 
-def make_parser(prog):
-    """Build a parser for command line arguments.
-
-    :sig: (str) -> ArgumentParser
-    :param prog: Name of program.
-    :return: Parser for arguments.
-    """
-    parser = ArgumentParser(prog=prog)
-    parser.add_argument('--version', action='version', version='%(prog)s 1.0b7')
-    parser.add_argument('--debug', action='store_true', help='enable debug messages')
-
-    commands = parser.add_subparsers(metavar='command', dest='command')
-    commands.required = True
-
-    h2x_parser = commands.add_parser('h2x', help='convert HTML to XHTML')
-    h2x_parser.add_argument('file', help='file to convert')
-    h2x_parser.set_defaults(func=lambda a: h2x(a.file))
-
-    scrape_parser = commands.add_parser('scrape', help='scrape a document')
-    scrape_parser.add_argument('document', help='file path or URL of document to scrape')
-    scrape_parser.add_argument('-s', '--spec', required=True, help='spec file')
-    scrape_parser.add_argument('--html', action='store_true', help='document is in HTML format')
-    scrape_parser.set_defaults(func=lambda a: scrape_document(
-        a.document, a.spec, content_format='html' if a.html else 'xml'
-    ))
-
-    return parser
-
-
-def main(argv=None):
-    """Entry point of the command line utility.
-
-    :sig: (Optional[List[str]]) -> None
-    :param argv: Command line arguments.
-    """
-    argv = argv if argv is not None else sys.argv
-    parser = make_parser(prog='piculet')
-    arguments = parser.parse_args(argv[1:])
-
-    # set debug mode
-    if arguments.debug:
-        logging.basicConfig(level=logging.DEBUG)
-        _logger.debug('running in debug mode')
-
-    # run the handler for the selected command
-    try:
-        arguments.func(arguments)
-    except Exception as e:
-        print(e, file=sys.stderr)
-        sys.exit(1)
-
-
 if __name__ == '__main__':
     main()
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/searchCompanyParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/searchPersonParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2008-2018 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2022 Davide Alberani <da@erlug.linux.it>
 #           2008-2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -13,58 +13,64 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 
 """
 This module provides the classes (and the instances) that are used to parse
-the results of a search for a given company.
+the results of a search for a given person.
 
-For example, when searching for the name "Columbia Pictures", the parsed page
+For example, when searching for the name "Mel Gibson", the parsed page
 would be:
 
-http://www.imdb.com/find?q=Columbia+Pictures&s=co
+http://www.imdb.com/find?q=Mel+Gibson&s=nm
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from imdb.utils import analyze_company_name
+from imdb.utils import analyze_name
 
 from .piculet import Path, Rule, Rules, reducers
 from .searchMovieParser import DOMHTMLSearchMovieParser
 from .utils import analyze_imdbid
 
 
-class DOMHTMLSearchCompanyParser(DOMHTMLSearchMovieParser):
-    """A parser for the company search page."""
+class DOMHTMLSearchPersonParser(DOMHTMLSearchMovieParser):
+    """A parser for the name search page."""
 
     rules = [
         Rule(
             key='data',
             extractor=Rules(
-                foreach='//td[@class="result_text"]',
+                foreach='//li[contains(@class, "find-name-result")]',
                 rules=[
                     Rule(
                         key='link',
-                        extractor=Path('./a/@href', reduce=reducers.first)
+                        extractor=Path('.//a[@class="ipc-metadata-list-summary-item__t"]/@href', reduce=reducers.first)
                     ),
                     Rule(
                         key='name',
-                        extractor=Path('./a/text()')
+                        extractor=Path('.//a[@class="ipc-metadata-list-summary-item__t"]/text()')
                     ),
                     Rule(
-                        key='notes',
-                        extractor=Path('./text()')
+                        key='headshot',
+                        extractor=Path('.//img[@class="ipc-image"]/@src')
                     )
                 ],
                 transform=lambda x: (
                     analyze_imdbid(x.get('link')),
-                    analyze_company_name(x.get('name') + x.get('notes', ''), stripNotes=True)
+                    analyze_name(x.get('name', '') + x.get('index', ''), canonical=1),
+                    x.get('akas'),
+                    x.get('headshot')
                 )
             )
         )
     ]
 
+    def _init(self):
+        super(DOMHTMLSearchPersonParser, self)._init()
+        self.img_type = 'headshot'
+
 
 _OBJECTS = {
-    'search_company_parser': ((DOMHTMLSearchCompanyParser,), {'kind': 'company'})
+    'search_person_parser': ((DOMHTMLSearchPersonParser,), {'kind': 'person'})
 }
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/searchKeywordParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/searchKeywordParser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2009-2018 Davide Alberani <da@erlug.linux.it>
+# Copyright 2009-2022 Davide Alberani <da@erlug.linux.it>
 #                2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -37,16 +37,16 @@
 class DOMHTMLSearchKeywordParser(DOMHTMLSearchMovieParser):
     """A parser for the keyword search page."""
 
     rules = [
         Rule(
             key='data',
             extractor=Path(
-                foreach='//td[@class="result_text"]',
-                path='./a/text()'
+                foreach='//li[contains(@class, "find-keyword-result")]',
+                path='.//a[@class="ipc-metadata-list-summary-item__t"]/text()'
             )
         )
     ]
 
 
 def custom_analyze_title4kwd(title, yearNote, outline):
     """Return a dictionary with the needed info."""
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/searchMovieAdvancedParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/searchMovieAdvancedParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import re
 
 from .piculet import Path, Rule, Rules, preprocessors, reducers
 from .utils import DOMParserBase, analyze_imdbid, build_movie, build_person
 
-
 _re_secondary_info = re.compile(
     r'''(\(([IVXLCM]+)\)\s+)?\((\d{4})(–(\s|(\d{4})))?(\s+(.*))?\)|(\(([IVXLCM]+)\))'''
 )
 
 
 _KIND_MAP = {
     'tv short': 'tv short movie',
@@ -55,15 +54,15 @@
         parsed['year'] = int(match.group(3))
     if match.group(4):
         kind = 'tv series'
     if match.group(6):
         parsed['series years'] = match.group(3) + "-" + match.group(6)
     if match.group(8):
         kind = match.group(8).lower()
-    if match.group(10): # Added to support case of imdbIndex but no year
+    if match.group(10):  # Added to support case of imdbIndex but no year
         parsed['imdbIndex'] = match.group(10)
     if kind is None:
         kind = 'movie'
     parsed['kind'] = _KIND_MAP.get(kind, kind)
     return parsed
 
 
@@ -171,15 +170,15 @@
                         extractor=Rules(
                             rules=[
                                 Rule(key='link',
                                      extractor=Path('./h3/small/a/@href', reduce=reducers.first)),
                                 Rule(key='title',
                                      extractor=Path('./h3/small/a/text()', reduce=reducers.first)),
                                 Rule(key='secondary_info',
-                                     extractor=Path('./h3/small/span[@class="lister-item-year text-muted unbold"]/text()',
+                                     extractor=Path('./h3/small/span[@class="lister-item-year text-muted unbold"]/text()',  # noqa: E501
                                                     reduce=reducers.first)),
                             ]
                         )
                     )
                 ]
             )
         )
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/searchMovieParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/searchMovieParser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2018 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2022 Davide Alberani <da@erlug.linux.it>
 #           2008-2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -23,66 +23,89 @@
 would be:
 
 http://www.imdb.com/find?q=the+passion&s=tt
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from imdb.utils import analyze_title
+from imdb.utils import analyze_title, re_m_kind
 
 from .piculet import Path, Rule, Rules, reducers
 from .utils import DOMParserBase, analyze_imdbid
 
 
+def process_title(tdict):
+    """Process parsed data and build a tuple that
+    can be used to create a list of results."""
+    imdbid = analyze_imdbid(tdict.get('link'))
+    title = tdict.get('title', '').strip()
+    kind = (tdict.get('kind') or '').strip()
+    if not re_m_kind.match('(%s)' % kind):
+        kind = ''
+    year = (tdict.get('year') or '').strip()
+    if year:
+        title += ' (%s)' % year
+    if kind:
+        title += ' (%s)' % kind
+    if title:
+        analized_title = analyze_title(title)
+    else:
+        analized_title = {}
+    akas = tdict.get('akas')
+    cover = tdict.get('cover url')
+    return imdbid, analized_title, akas, cover
+
+
 class DOMHTMLSearchMovieParser(DOMParserBase):
     """A parser for the title search page."""
 
     rules = [
         Rule(
             key='data',
             extractor=Rules(
-                foreach='//td[@class="result_text"]',
+                foreach='//li[contains(@class, "find-title-result")]',
                 rules=[
                     Rule(
                         key='link',
-                        extractor=Path('./a/@href', reduce=reducers.first)
+                        extractor=Path('.//a[@class="ipc-metadata-list-summary-item__t"]/@href',
+                                       reduce=reducers.first)
+                    ),
+                    Rule(
+                        key='title',
+                        extractor=Path('.//a[@class="ipc-metadata-list-summary-item__t"]/text()')
                     ),
                     Rule(
-                        key='info',
-                        extractor=Path('.//text()')
+                        key='year',
+                        extractor=Path('.//span[@class="ipc-metadata-list-summary-item__li"]/text()',
+                                       reduce=reducers.first)
                     ),
                     Rule(
-                        key='akas',
-                        extractor=Path(foreach='./i', path='./text()')
+                        key='kind',
+                        extractor=Path('(.//span[@class="ipc-metadata-list-summary-item__li"])[2]/text()')
                     ),
                     Rule(
                         key='cover url',
-                        extractor=Path('../td[@class="primary_photo"]/a/img/@src')
+                        extractor=Path('.//img[@class="ipc-image"]/@src')
                     )
                 ],
-                transform=lambda x: (
-                    analyze_imdbid(x.get('link')),
-                    analyze_title(x.get('info', '')),
-                    x.get('akas'),
-                    x.get('cover url')
-                )
+                transform=process_title
             )
         )
     ]
 
     def _init(self):
         self.url = ''
         self.img_type = 'cover url'
 
     def _reset(self):
         self.url = ''
 
     def postprocess_data(self, data):
         if 'data' not in data:
-            data['data'] = []
+            return {'data': []}
         results = getattr(self, 'results', None)
         if results is not None:
             data['data'][:] = data['data'][:results]
         # Horrible hack to support AKAs.
             data['data'] = [x for x in data['data'] if x[0] and x[1]]
         if data and data['data'] and len(data['data'][0]) == 4 and isinstance(data['data'][0], tuple):
             for idx, datum in enumerate(data['data']):
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/searchPersonParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/searchCompanyParser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2019 Davide Alberani <da@erlug.linux.it>
+# Copyright 2008-2022 Davide Alberani <da@erlug.linux.it>
 #           2008-2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -13,72 +13,59 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 
 """
 This module provides the classes (and the instances) that are used to parse
-the results of a search for a given person.
+the results of a search for a given company.
 
-For example, when searching for the name "Mel Gibson", the parsed page
+For example, when searching for the name "Columbia Pictures", the parsed page
 would be:
 
-http://www.imdb.com/find?q=Mel+Gibson&s=nm
+http://www.imdb.com/find?q=Columbia+Pictures&s=co
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from imdb.utils import analyze_name
+from imdb.utils import analyze_company_name
 
 from .piculet import Path, Rule, Rules, reducers
 from .searchMovieParser import DOMHTMLSearchMovieParser
 from .utils import analyze_imdbid
 
 
-class DOMHTMLSearchPersonParser(DOMHTMLSearchMovieParser):
-    """A parser for the name search page."""
+class DOMHTMLSearchCompanyParser(DOMHTMLSearchMovieParser):
+    """A parser for the company search page."""
 
     rules = [
         Rule(
             key='data',
             extractor=Rules(
-                foreach='//td[@class="result_text"]',
+                foreach='//li[contains(@class, "find-company-result")]',
                 rules=[
                     Rule(
                         key='link',
-                        extractor=Path('./a/@href', reduce=reducers.first)
+                        extractor=Path('.//a[@class="ipc-metadata-list-summary-item__t"]/@href', reduce=reducers.first)
                     ),
                     Rule(
                         key='name',
-                        extractor=Path('./a/text()')
+                        extractor=Path('.//a[@class="ipc-metadata-list-summary-item__t"]/text()')
                     ),
                     Rule(
-                        key='index',
-                        extractor=Path('./text()')
+                        key='country',
+                        extractor=Path('.//label[@class="ipc-metadata-list-summary-item__li"]/text()',
+                                       reduce=reducers.first)
                     ),
-                    Rule(
-                        key='akas',
-                        extractor=Path(foreach='./i', path='./text()')
-                    ),
-                    Rule(
-                        key='headshot',
-                        extractor=Path('../td[@class="primary_photo"]/a/img/@src')
-                    )
                 ],
                 transform=lambda x: (
                     analyze_imdbid(x.get('link')),
-                    analyze_name(x.get('name', '') + x.get('index', ''), canonical=1),
-                    x.get('akas'),
-                    x.get('headshot')
+                    analyze_company_name(x.get('name') + (' [%s]' % x.get('country') if x.get('country') else ''))
                 )
             )
         )
     ]
 
-    def _init(self):
-        super(DOMHTMLSearchPersonParser, self)._init()
-        self.img_type = 'headshot'
-
 
 _OBJECTS = {
-    'search_person_parser': ((DOMHTMLSearchPersonParser,), {'kind': 'person'})
+    'search_company_parser': ((DOMHTMLSearchCompanyParser,), {'kind': 'company'})
 }
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/topBottomParser.py` & `cinemagoer-2023.5.1/imdb/parser/http/topBottomParser.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/parser/http/utils.py` & `cinemagoer-2023.5.1/imdb/parser/http/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2019 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2022 Davide Alberani <da@erlug.linux.it>
 #           2008-2018 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -23,36 +23,34 @@
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import re
 
 from imdb import PY2
 from imdb.Character import Character
 from imdb.Movie import Movie
+from imdb.parser.http.logging import logger
 from imdb.Person import Person
 from imdb.utils import _Container, flatten
-from imdb.parser.http.logging import logger
 
-from .piculet import _USE_LXML, ElementTree, Rules, build_tree, html_to_xhtml
+from .piculet import _USE_LXML, ElementTree, Path, Rule, Rules, build_tree, html_to_xhtml
 from .piculet import xpath as piculet_xpath
-from .piculet import Rule, Path
-
 
 if PY2:
     from collections import Callable
 else:
     from collections.abc import Callable
 
 
 # Year, imdbIndex and kind.
 re_yearKind_index = re.compile(
     r'(\([0-9\?]{4}(?:/[IVXLCDM]+)?\)(?: \(mini\)| \(TV\)| \(V\)| \(VG\))?)'
 )
 
 # Match imdb ids in href tags
-re_imdbid = re.compile(r'(title/tt|name/nm|company/co|user/ur)([0-9]+)')
+re_imdbid = re.compile(r'(title/tt|name/nm|company/co|companies=co|user/ur)([0-9]+)')
 
 
 def analyze_imdbid(href):
     """Return an imdbID from an URL."""
     if not href:
         return None
     match = re_imdbid.search(href)
@@ -346,21 +344,21 @@
         if notes:
             notes += ' '
         notes += additionalNotes
     m = Movie(title=title, movieID=movieID, notes=notes, currentRole=role,
               roleID=roleID, roleIsPerson=_parsingCharacter,
               modFunct=modFunct, accessSystem=accessSystem)
     if additionalNotes:
-        if '(TV Series)' in additionalNotes:
+        if 'TV Series' in additionalNotes:
             m['kind'] = 'tv series'
-        elif '(Video Game)' in additionalNotes:
+        elif 'Video Game' in additionalNotes:
             m['kind'] = 'video game'
-        elif '(TV Movie)' in additionalNotes:
+        elif 'TV Movie' in additionalNotes:
             m['kind'] = 'tv movie'
-        elif '(TV Short)' in additionalNotes:
+        elif 'TV Short' in additionalNotes:
             m['kind'] = 'tv short'
     if roleNotes and len(roleNotes) == len(roleID):
         for idx, role in enumerate(m.currentRole):
             try:
                 if roleNotes[idx]:
                     role.notes = roleNotes[idx]
             except IndexError:
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/s3/__init__.py` & `cinemagoer-2023.5.1/imdb/parser/s3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 The :func:`imdb.IMDb` function will return an instance of this class when
 called with the ``accessSystem`` parameter is set to "s3" or "s3dataset".
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import logging
-import sqlalchemy
 from operator import itemgetter
-from imdb import IMDbBase
-from .utils import DB_TRANSFORM, title_soundex, name_soundexes, scan_titles, scan_names
 
+import sqlalchemy
+
+from imdb import IMDbBase
 from imdb.Movie import Movie
 from imdb.Person import Person
 
+from .utils import DB_TRANSFORM, name_soundexes, scan_names, scan_titles, title_soundex
+
 
 def split_array(text):
     """Split a string assuming it's an array.
 
     :param text: the text to split
     :type text: str
     :returns: list of splitted strings
@@ -279,8 +281,7 @@
         results = nb.select(sqlalchemy.or_(*conditions)).execute()
         results = [(x['nconst'], self._clean(self._rename('name_basics', dict(x)),
                                              ('ns_soundex', 'sn_soundex', 's_soundex')))
                    for x in results]
         results = scan_names(results, name)
         results = [x[1] for x in results]
         return results
-
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/s3/utils.py` & `cinemagoer-2023.5.1/imdb/parser/s3/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 """
 This package provides utilities for the s3 dataset.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import re
-import sqlalchemy
 from difflib import SequenceMatcher
-from imdb.utils import canonicalName, canonicalTitle, _unicodeArticles
+
+import sqlalchemy
+
+from imdb.utils import _unicodeArticles, canonicalName, canonicalTitle
 
 SOUNDEX_LENGTH = 5
 RO_THRESHOLD = 0.6
 STRING_MAXLENDIFFER = 0.7
 re_imdbids = re.compile(r'(nm|tt)')
 re_characters = re.compile(r'"(.+?)"')
 
@@ -74,14 +76,15 @@
     'tvMiniSeries': 'tv mini series',
     'tvSeries': 'tv series',
     'tvShort': 'tv short',
     'tvSpecial': 'tv special',
     'videoGame': 'video game'
 }
 
+
 def transf_kind(x):
     return KIND.get(x, x)
 
 
 # Database mapping.
 # 'type' force a conversion to a specific SQL type
 # 'transform' applies a conversion to the content (changes the data in the database)
@@ -115,15 +118,15 @@
         'knownForTitles': {'transform': transf_multi_imdbid, 'rename': 'known for'},
         'ns_soundex': {'type': sqlalchemy.String, 'length': 5, 'index': True},
         'sn_soundex': {'type': sqlalchemy.String, 'length': 5, 'index': True},
         's_soundex': {'type': sqlalchemy.String, 'length': 5, 'index': True},
     },
     'title_akas': {
         'titleId': {'type': sqlalchemy.Integer, 'transform': transf_imdbid,
-                   'rename': 'movieID', 'index': True},
+                    'rename': 'movieID', 'index': True},
         'ordering': {'type': sqlalchemy.Integer, 'transform': transf_int},
         'title': {},
         'region': {'type': sqlalchemy.String, 'length': 5, 'index': True},
         'language': {'type': sqlalchemy.String, 'length': 5, 'index': True},
         'types': {'type': sqlalchemy.String, 'length': 31, 'index': True},
         'attributes': {'type': sqlalchemy.String, 'length': 127},
         'isOriginalTitle': {'type': sqlalchemy.Boolean, 'transform': transf_bool,
@@ -340,8 +343,7 @@
                 resd[i] = (ratio, (i, t_data))
     res = list(resd.values())
     res.sort()
     res.reverse()
     if results > 0:
         res[:] = res[:results]
     return res
-
```

### Comparing `cinemagoer-2022.2.11/imdb/parser/sql/__init__.py` & `cinemagoer-2023.5.1/imdb/parser/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/parser/sql/alchemyadapter.py` & `cinemagoer-2023.5.1/imdb/parser/sql/alchemyadapter.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/parser/sql/dbschema.py` & `cinemagoer-2023.5.1/imdb/parser/sql/dbschema.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/imdb/utils.py` & `cinemagoer-2023.5.1/imdb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2021 Davide Alberani <da@erlug.linux.it>
+# Copyright 2004-2022 Davide Alberani <da@erlug.linux.it>
 #                2009 H. Turgut Uyar <uyar@tekir.org>
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
@@ -24,32 +24,29 @@
 import re
 import string
 import sys
 from copy import copy, deepcopy
 from functools import total_ordering
 from time import strftime, strptime
 
-from imdb import VERSION
 from imdb import linguistics
 from imdb._exceptions import IMDbParserError
 from imdb._logging import imdbpyLogger
 
-
 PY2 = sys.hexversion < 0x3000000
 
-
 # Logger for imdb.utils module.
 _utils_logger = imdbpyLogger.getChild('utils')
 
 # The regular expression for the "long" year format of IMDb, like
 # "(1998)" and "(1986/II)", where the optional roman number (that I call
 # "imdbIndex" after the slash is used for movies with the same title
 # and year of release.
 # XXX: probably L, C, D and M are far too much! ;-)
-re_year_index = re.compile(r'\(([0-9\?]{4}(/[IVXLCDM]+)?)\)')
+re_year_index = re.compile(r'\(([0-9\?]{4}([–-]([0-9\?]{4})?\s?)?(/[IVXLCDM]+)?)\)')
 re_m_episode = re.compile(r'\(TV Episode\)\s+-\s+', re.I)
 re_m_series = re.compile(r'Season\s+(\d+)\s+\|\s+Episode\s+(\d+)\s+-', re.I)
 re_m_imdbIndex = re.compile(r'\(([IVXLCDM]+)\)')
 re_m_kind = re.compile(
     r'\((TV episode|TV Series|TV mini[ -]series|mini|TV|Video|Video Game|VG|Short|TV Movie|TV Short|TV Special|V)\)',
     re.I
 )
@@ -313,15 +310,15 @@
     raise an IMDbParserError exception if the title is not valid.
     """
     # XXX: introduce the 'lang' argument?
     if canonical is not None:
         canonicalSeries = canonicalEpisode = canonical
     original_t = title
     result = {}
-    title = title.split(' aka ')[0].strip()
+    title = title.split(' aka ')[0].strip().replace('""', '"')
     year = ''
     kind = ''
     imdbIndex = ''
     series_title, episode_or_year = _split_series_episode(title)
     if series_title:
         # It's an episode of a series.
         series_d = analyze_title(series_title, canonical=canonicalSeries)
@@ -441,15 +438,15 @@
             result['series years'] = year
             year = year[:4]
         try:
             result['year'] = int(year)
         except (TypeError, ValueError):
             pass
     if imdbIndex:
-        result['imdbIndex'] = imdbIndex
+        result['imdbIndex'] = imdbIndex.strip()
     result['kind'] = kind or 'movie'
     return result
 
 
 _web_format = '%d %B %Y'
 _ptdf_format = '(%Y-%m-%d)'
 
@@ -1215,15 +1212,15 @@
         if not self.__role:
             # XXX: needed?  Just ignore it?  It's probably safer to
             #      ignore it, to prevent some bugs in the parsers.
             # raise IMDbError,"Can't set ID of an empty Character/Person object."
             pass
         if not self._roleIsPerson:
             if not isinstance(roleID, (list, tuple)):
-                if not(PY2 and isinstance(self.currentRole, unicode)):
+                if not (PY2 and isinstance(self.currentRole, unicode)):
                     self.currentRole.characterID = roleID
             else:
                 for index, item in enumerate(roleID):
                     r = self.__role[index]
                     if PY2 and isinstance(r, unicode):
                         continue
                     r.characterID = item
@@ -1280,15 +1277,15 @@
         if not (self._image_key and self._image_key in self.data):
             return None
         url = self.data[self._image_key] or ''
         ext_idx = url.rfind('.')
         if ext_idx == -1:
             return url
         if '@' in url:
-            return url[:url.rindex('@')+1] + url[ext_idx:]
+            return url[:url.rindex('@') + 1] + url[ext_idx:]
         else:
             prev_dot = url[:ext_idx].rfind('.')
             if prev_dot == -1:
                 return url
             return url[:prev_dot] + url[ext_idx:]
 
     def reset(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cinemagoer-2022.2.11/setup.py` & `cinemagoer-2023.5.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
-import sys
 import glob
+import sys
+from subprocess import CalledProcessError, check_call
 
 import setuptools
 
-
 # version of the software from imdb/version.py
 exec(compile(open('imdb/version.py').read(), 'imdb/version.py', 'exec'))
 
 home_page = 'https://cinemagoer.github.io/'
 
 long_desc = """Cinemagoer is a Python package useful to retrieve and
 manage the data of the IMDb movie database about movies, people,
@@ -37,14 +36,16 @@
 Intended Audience :: Developers
 Intended Audience :: End Users/Desktop
 License :: OSI Approved :: GNU General Public License (GPL)
 Natural Language :: English
 Natural Language :: Italian
 Natural Language :: Turkish
 Programming Language :: Python
+Programming Language :: Python :: 3.11
+Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.5
 Programming Language :: Python :: 2.7
 Programming Language :: Python :: Implementation :: CPython
@@ -73,14 +74,17 @@
     'maintainer': 'Davide Alberani',
     'maintainer_email': 'da@mimante.net',
     'license': 'GPL',
     'platforms': 'any',
     'keywords': keywords,
     'classifiers': [_f for _f in classifiers.split("\n") if _f],
     'url': home_page,
+    'project_urls': {
+        'Source': 'https://github.com/cinemagoer/cinemagoer',
+    },
     'download_url': dwnl_url,
     'scripts': scripts,
     'package_data': {
         # Here, the "*" represents any possible language ID.
         'imdb.locale': [
             'imdbpy.pot',
             'imdbpy-*.po',
@@ -88,24 +92,21 @@
         ],
     },
     'install_requires': ['SQLAlchemy', 'lxml'],
     'extras_require': {
         'dev': [
             'flake8',
             'flake8-isort',
-            'readme_renderer'
+            'pytest',
+            'pytest-cov',
+            'tox',
         ],
         'doc': [
             'sphinx',
             'sphinx_rtd_theme'
-        ],
-        'test': [
-            'pytest',
-            'pytest-cov',
-            'pytest-profiling'
         ]
     },
     'packages': setuptools.find_packages(),
     'entry_points': """
         [console_scripts]
         imdbpy=imdb.cli:main
     """
@@ -126,37 +127,20 @@
   The best solution is to resolve these dependencies (maybe you're
   not connected to Internet?)
 
   The caught exception, is re-raise below:
 """
 
 
-REBUILDMO_DIR = os.path.join('imdb', 'locale')
-REBUILDMO_NAME = 'rebuildmo'
-
-
 def runRebuildmo():
     """Call the function to rebuild the locales."""
-    cwd = os.getcwd()
-    path = list(sys.path)
-    languages = []
     try:
-        import importlib
-        scriptPath = os.path.dirname(__file__)
-        modulePath = os.path.join(cwd, scriptPath, REBUILDMO_DIR)
-        sys.path += [modulePath, '.', cwd]
-        rebuildmo = importlib.import_module(os.path.join(REBUILDMO_DIR, REBUILDMO_NAME).replace(os.path.sep, '.'))
-        os.chdir(modulePath)
-        languages = rebuildmo.rebuildmo()
-        print('Created locale for: %s.' % ' '.join(languages))
-    except Exception as e:
+        check_call([sys.executable, "rebuildmo.py"])
+    except CalledProcessError as e:
         print('ERROR: unable to rebuild .mo files; caught exception %s' % e)
-    sys.path = path
-    os.chdir(cwd)
-    return languages
 
 
 def hasCommand():
     """Return true if at least one command is found on the command line."""
     args = sys.argv[1:]
     if '--help' in args:
         return False
```

### Comparing `cinemagoer-2022.2.11/tests/conftest.py` & `cinemagoer-2023.5.1/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from pytest import fixture
 
 import logging
 import os
-from hashlib import md5
+import time
 
 from imdb import Cinemagoer
 from imdb.parser.http import IMDbURLopener
 
-
 logging.raiseExceptions = False
 
+DELAY = 0
+
 
 cache_dir = os.path.join(os.path.dirname(__file__), '.cache')
 if not os.path.exists(cache_dir):
     os.makedirs(cache_dir)
 
 
 retrieve_unicode_orig = IMDbURLopener.retrieve_unicode
 
 
 def retrieve_unicode_cached(self, url, size=-1):
-    key = md5(url.encode('utf-8')).hexdigest()
+    print(url)
+    key = "_".join(url.split("/")[3:])
     cache_file = os.path.join(cache_dir, key)
     if os.path.exists(cache_file):
         with open(cache_file, 'r') as f:
             content = f.read()
     else:
+        time.sleep(DELAY)
         content = retrieve_unicode_orig(self, url, size=size)
         with open(cache_file, 'w') as f:
             f.write(content)
     return content
 
 
 s3_uri = os.getenv('CINEMAGOER_S3_URI')
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_chart_bottom.py` & `cinemagoer-2023.5.1/tests/test_http_chart_bottom.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_chart_popular_movies.py` & `cinemagoer-2023.5.1/tests/test_http_chart_popular_movies.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
         assert 'title' in movie
 
 
 def test_popular_movies_chart_entries_should_be_movies(ia):
     movies = ia.get_popular100_movies()
     for movie in movies:
         assert movie['kind'] == 'movie'
-
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_chart_popular_tv.py` & `cinemagoer-2023.5.1/tests/test_http_chart_popular_tv.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
         assert 'title' in movie
 
 
 def test_popular_tv_entries_should_have_year(ia):
     movies = ia.get_popular100_tv()
     for movie in movies:
         assert isinstance(movie['year'], int)
-
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_chart_top.py` & `cinemagoer-2023.5.1/tests/test_http_chart_top.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_chart_top_indian.py` & `cinemagoer-2023.5.1/tests/test_http_chart_top_indian.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,7 @@
         assert isinstance(movie['year'], int)
 
 
 def test_top_indian_chart_entries_should_have_high_ratings(ia):
     movies = ia.get_top250_indian_movies()
     for movie in movies:
         assert movie['rating'] > 7
-
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_chart_top_tv.py` & `cinemagoer-2023.5.1/tests/test_http_chart_top_tv.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_combined.py` & `cinemagoer-2023.5.1/tests/test_http_movie_combined.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from pytest import mark
 
 import re
 
 from imdb.Movie import Movie
 from imdb.Person import Person
 
-
 months = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
 re_date = re.compile(r'[0-9]{1,2} (%s) [0-9]{4}' % '|'.join(months), re.I)
 
 
 def test_movie_cover_url_should_be_an_image_link(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert re.match(r'^https?://.*\.jpg$', movie.get('cover url'))
 
 
 def test_cover_url_if_none_should_be_excluded(ia):
     movie = ia.get_movie('3629794', info=['main'])      # Aslan
     assert 'cover url' not in movie
 
 
+def test_videos_if_none_should_be_excluded(ia):
+    movie = ia.get_movie('7967312', info=['main'])      # Simple Worker Needed
+    assert 'videos' not in movie
+
+
 def test_movie_directors_should_be_a_list_of_persons(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     directors = [p for p in movie.get('directors', [])]
     assert len(directors) == 2
     for p in directors:
         assert isinstance(p, Person)
 
@@ -127,14 +131,15 @@
     assert movie.get('kind') == 'movie'
 
 
 def test_movie_kind_tv_movie_should_be_tv_movie(ia):
     movie = ia.get_movie('0389150', info=['main'])      # Matrix (TV)
     assert movie.get('kind') == 'tv movie'
 
+
 def test_movie_kind_tv_special_should_be_tv_special(ia):
     movie = ia.get_movie('14544192', info=['main'])      # Bo Burnham: Inside
     assert movie.get('kind') == 'tv special'
 
 
 def test_movie_kind_video_movie_should_be_video_movie(ia):
     movie = ia.get_movie('0109151', info=['main'])      # Matrix (V)
@@ -265,25 +270,25 @@
 
 def test_movie_rating_should_be_between_1_and_10(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert 1.0 <= movie.get('rating') <= 10.0
 
 
 def test_movie_rating_if_none_should_be_excluded(ia):
-    movie = ia.get_movie('1863157', info=['main'])      # Ates Parcasi
+    movie = ia.get_movie('3629794', info=['main'])      # Aslan
     assert 'rating' not in movie
 
 
 def test_movie_votes_should_be_an_integer(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert movie.get('votes') > 1000000
 
 
 def test_movie_votes_if_none_should_be_excluded(ia):
-    movie = ia.get_movie('1863157', info=['main'])      # Ates Parcasi
+    movie = ia.get_movie('3629794', info=['main'])      # Aslan
     assert 'votes' not in movie
 
 
 def test_movie_top250_rank_should_be_between_1_and_250(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert 1 <= movie.get('top 250 rank') <= 250
 
@@ -519,14 +524,15 @@
     assert expected.issubset(set(movie.get('sound mix', [])))
 
 
 def test_movie_sound_mix_if_none_should_be_excluded(ia):
     movie = ia.get_movie('1863157', info=['main'])      # Ates Parcasi
     assert 'sound mix' not in movie
 
+
 def test_movie_certificates_should_be_a_list_of_certificates(ia):
     movie = ia.get_movie('1000252', info=['main'])      # Doctor Who - Blink
     assert movie.get('certificates', []) == [
         'Australia:PG::(most episodes)',
         'Brazil:12',
         'Netherlands:9::(some episodes)',
         'New Zealand:PG',
@@ -551,24 +557,24 @@
 def test_movie_cast_must_be_in_plain_format(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert movie['cast'][0].data.get('name') == 'Keanu Reeves'
 
 
 def test_movie_misc_sections_must_contain_items(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
-    assert len(movie.get('casting department', [])) == 2
+    assert len(movie.get('casting department', [])) == 3
 
 
 def test_movie_misc_sections_must_be_in_plain_format(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert movie['casting department'][0].data.get('name') == 'Tim Littleton'
 
 
 def test_movie_companies_sections_must_contain_items(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
-    assert len(movie.get('special effects companies', [])) == 7
+    assert len(movie.get('special effects companies', [])) == 6
 
 
 def test_movie_box_office_should_be_a_dict(ia):
     movie = ia.get_movie('0133093', info=['main'])      # Matrix
     assert isinstance(movie.get('box office'), dict)
     assert len(movie.get('box office', {})) == 3
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_full_credit.py` & `cinemagoer-2023.5.1/tests/test_http_movie_full_credit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-
 def test_movie_full_credits(ia):
-    movie = ia.get_movie('0133093', info=['full credits']) # Matrix
+    movie = ia.get_movie('0133093', info=['full credits'])  # Matrix
     assert 'cast' in movie
     lcast = len(movie['cast'])
     assert lcast > 38 and lcast < 42
 
+
 def test_movie_full_credits_for_tv_show(ia):
-    movie = ia.get_movie('0098904', info=['full credits']) # Seinfeld
+    movie = ia.get_movie('0098904', info=['full credits'])  # Seinfeld
     assert 'cast' in movie
     assert len(movie['cast']) > 1300 and len(movie['cast']) < 1350
 
+
 def test_movie_full_credits_contains_headshot(ia):
-    movie = ia.get_movie('0133093', info=['main', 'full credits'])      # Matrix
-    assert 'headshot' in movie['cast'][0] # Keanu Reeves
-    assert 'nopicture' not in movie['cast'][0]['headshot'] # is real headshot, not default
+    movie = ia.get_movie('0133093', info=['main', 'full credits'])  # Matrix
+    assert 'headshot' in movie['cast'][0]  # Keanu Reeves
+    assert 'nopicture' not in movie['cast'][0]['headshot']  # is real headshot, not default
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_keywords.py` & `cinemagoer-2023.5.1/tests/test_http_movie_keywords.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 def test_movie_keywords_should_be_a_list_of_keywords(ia):
     movie = ia.get_movie('0133093', info=['keywords'])  # Matrix
     keywords = movie.get('keywords', [])
     assert 250 <= len(keywords) <= 400
     assert {'computer-hacker', 'messiah', 'artificial-reality'}.issubset(set(keywords))
 
+
 def test_movie_relevant_keywords_should_be_a_list_of_keywords(ia):
     movie = ia.get_movie('0133093', info=['keywords'])  # Matrix
     keywords = movie.get('relevant keywords', [])
     assert 250 <= len(keywords) <= 400
     assert 'artificial reality' in [x['keyword'] for x in keywords]
 
+
 def test_movie_keywords_if_none_should_be_excluded(ia):
     movie = ia.get_movie('1863157', info=['keywords'])  # Ates Parcasi
     assert 'keywords' not in movie
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_parental_guide.py` & `cinemagoer-2023.5.1/tests/test_http_movie_parental_guide.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 def test_movie_parental_guide_contains_mpaa_rating(ia):
     movie = ia.get_movie('0133093', info=['parents guide'])  # Matrix
     assert movie.get('mpaa') == "Rated R for sci-fi violence and brief language"
 
+
 def test_movie_certificates_from_parental_guide(ia):
     movie = ia.get_movie('0133093', info=['parents guide'])      # Matrix
     arCert = {'country_code': 'AR', 'country': 'Argentina', 'certificate': '13', 'note': '', 'full': 'Argentina:13'}
     assert arCert in movie.get('certificates', [])
 
+
 def test_movie_advisories(ia):
     movie = ia.get_movie('0133093', info=['parents guide'])      # Matrix
     assert any(['Mouse gets shot' in x for x in movie.get('advisory spoiler violence')])
+
+
+def test_movie_advisory_votes(ia):
+    movie = ia.get_movie('0133093', info=['parents guide'])      # Matrix
+    votes = movie.get('advisory votes')
+    assert votes['nudity']['votes']['Mild'] > 300
+    assert votes['nudity']['status'] == 'Mild'
+    assert votes['profanity']['status'] == 'Moderate'
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_plot.py` & `cinemagoer-2023.5.1/tests/test_http_movie_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     plots = movie.get('plot', [])
     assert 3 <= len(plots) <= 10
     sel_plot = ''
     for plot in plots:
         if plot.endswith('redcommander27'):
             sel_plot = plot
             break
-    assert re.match(r'^Thomas A. Anderson is a man.*As a rebel.*::redcommander27$', sel_plot)
+    assert re.match(r'^Thomas A. Anderson is a man.*As a rebel.*redcommander27$', sel_plot)
 
 
 def test_movie_summary_if_none_should_be_excluded(ia):
     movie = ia.get_movie('1863157', info=['plot'])  # Ates Parcasi
     assert 'plot' not in movie
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_releaseinfo.py` & `cinemagoer-2023.5.1/tests/test_http_movie_releaseinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,7 @@
 
 
 def test_movie_release_info_raw_release_dates_must_be_a_list(ia):
     movie = ia.get_movie('0133093', info=['release info'])    # Matrix
     akas = movie.get('raw release dates', [])
     assert len(akas) >= 56
     assert len(akas) == len(movie.get('release dates'))
-
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_season_episodes.py` & `cinemagoer-2023.5.1/tests/test_http_movie_season_episodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,49 +21,56 @@
     movie = ia.get_movie('0185906', info=['episodes'])      # Band of Brothers
     episodes = movie.get('episodes')
     rating = episodes[1][1]['rating']
     votes = episodes[1][1]['votes']
     assert 8.3 <= rating <= 9.0
     assert votes > 4400
 
+
 def test_update_series_seasons_single_int(ia):
     movie = ia.get_movie('0264235')                         # Curb Your Enthusiasm
     ia.update_series_seasons(movie, season_nums=10)
     assert 'episodes' in movie
     assert list(movie['episodes']) == [10]
 
+
 def test_update_series_seasons_range(ia):
     movie = ia.get_movie('0264235')                         # Curb Your Enthusiasm
     ia.update_series_seasons(movie, season_nums=range(3, 10))
     assert 'episodes' in movie
     assert list(sorted(movie['episodes'])) == list(range(3, 10))
 
+
 def test_update_series_seasons_list(ia):
     movie = ia.get_movie('0264235')                         # Curb Your Enthusiasm
     ia.update_series_seasons(movie, season_nums=[1, 3, 5])
     assert 'episodes' in movie
     assert list(sorted(movie['episodes'])) == [1, 3, 5]
 
+
 def test_update_series_seasons_tuple(ia):
     movie = ia.get_movie('0264235')                         # Curb Your Enthusiasm
     ia.update_series_seasons(movie, season_nums=(1, 3, 5))
     assert 'episodes' in movie
     assert list(sorted(movie['episodes'])) == [1, 3, 5]
 
+
 def test_update_series_seasons_set(ia):
     movie = ia.get_movie('0264235')                         # Curb Your Enthusiasm
     ia.update_series_seasons(movie, season_nums={1, 3, 5})
     assert 'episodes' in movie
     assert list(sorted(movie['episodes'])) == [1, 3, 5]
 
+
 def test_update_series_seasons_iterable(ia):
     movie = ia.get_movie('0264235')                         # Curb Your Enthusiasm
     ia.update_series_seasons(movie, season_nums=(i for i in range(6) if i % 2))
     assert 'episodes' in movie
     assert list(sorted(movie['episodes'])) == [1, 3, 5]
 
+
 def test_update_series_seasons_less_season_available(ia):
     movie = ia.get_movie('0185906')                         # Band of Brothers
     # Only 1 season but request 9
     ia.update_series_seasons(movie, season_nums=range(1, 10))
     assert 'episodes' in movie
     assert list(movie['episodes']) == [1]
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_sites.py` & `cinemagoer-2023.5.1/tests/test_http_movie_sites.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_taglines.py` & `cinemagoer-2023.5.1/tests/test_http_movie_taglines.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_titles.py` & `cinemagoer-2023.5.1/tests/test_http_movie_titles.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pytest import mark
 
+
 @mark.skip('obviously this depends on your country of origin')
 def test_movie_localized_title(ia):
     movie = ia.get_movie('2991224', info=['main'])
     title = movie.get('localized title', '')
     assert title in ('Tangerines - Mandarini', 'Tangerines')
 
 
@@ -13,8 +14,7 @@
     assert title == 'Mandariinid'
 
 
 def test_movie_title(ia):
     movie = ia.get_movie('2991224', info=['main'])
     title = movie.get('title', '')
     assert title == 'Tangerines'
-
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_movie_votes.py` & `cinemagoer-2023.5.1/tests/test_http_movie_votes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from pytest import mark
+
+
 def test_movie_votes_should_be_divided_into_10_slots(ia):
     movie = ia.get_movie('0133093', info=['vote details'])  # Matrix
     votes = movie.get('number of votes', [])
     assert len(votes) == 10
 
 
 def test_movie_votes_should_be_integers(ia):
@@ -25,17 +28,19 @@
 
 def test_movie_demographics_should_be_divided_into_multiple_categories(ia):
     movie = ia.get_movie('0133093', info=['vote details'])  # Matrix
     demographics = movie['demographics']
     assert len(demographics) >= 18
 
 
+@mark.skip(reason="top 1000 voters parser doesn't seem to work")
 def test_movie_demographics_votes_should_be_integers(ia):
     movie = ia.get_movie('0133093', info=['vote details'])  # Matrix
     top1000 = movie['demographics']['top 1000 voters']
     assert 890 <= top1000['votes'] <= 1000
 
 
+@mark.skip(reason="top 1000 voters parser doesn't seem to work")
 def test_movie_demographics_rating_should_be_numeric(ia):
     movie = ia.get_movie('0133093', info=['vote details'])  # Matrix
     top1000 = movie['demographics']['top 1000 voters']
     assert 8 <= top1000['rating'] <= 8.5
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_person_bio.py` & `cinemagoer-2023.5.1/tests/test_http_person_bio.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_person_main.py` & `cinemagoer-2023.5.1/tests/test_http_person_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import re
 
 
 def test_person_headshot_should_be_an_image_link(ia):
     person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
     assert re.match(r'^https?://.*\.jpg$', person['headshot'])
 
-def test_person_director_is_in_filmography(ia):
-    person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
-    assert 'director' in person.get('filmography', {})
+
+def test_person_producer_is_in_filmography(ia):
+    person = ia.get_person('0000206', info=['filmography'])    # Keanu Reeves
+    assert 'producer' in person.get('filmography', {})
+
 
 def test_person_filmography_includes_role(ia):
-    person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
+    person = ia.get_person('0000206', info=['filmography'])    # Keanu Reeves
     movies = person.get('filmography', {}).get('actor', {})
     assert 'John Wick' in [str(movie.currentRole) for movie in movies]
 
+
 def test_person_with_id_redirect(ia):
     person = ia.get_person('1890852', info=['main'])    # Aleksandr Karpov
     assert '0440022' == person.get('imdbID')
 
+
 def test_person_name_in_data_should_be_plain(ia):
     person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
     assert person.data.get('name') == 'Keanu Reeves'
 
+
 def test_person_canonical_name(ia):
     person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
     assert person.get('canonical name') == 'Reeves, Keanu'
 
+
 def test_person_headshot_if_none_should_be_excluded(ia):
     person = ia.get_person('0330139', info=['main'])    # Deni Gordon
     assert 'headshot' not in person
 
+
 def test_person_name_should_not_be_canonicalized(ia):
     person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
     assert person.get('name') == 'Keanu Reeves'
 
 
 def test_person_name_should_not_have_birth_and_death_years(ia):
     person = ia.get_person('0000001', info=['main'])    # Fred Astaire
@@ -42,20 +49,29 @@
 
 def test_person_imdb_index_should_be_a_roman_number(ia):
     person = ia.get_person('0000210', info=['main'])    # Julia Roberts
     assert person.get('imdbIndex') == 'I'
 
 
 def test_person_should_have_filmography(ia):
-    person = ia.get_person('0000210', info=['main'])    # Julia Roberts
-    filmoset = set(['actress', 'producer', 'self'])
+    person = ia.get_person('0000210', info=['filmography'])    # Julia Roberts
+    filmoset = set(['actress', 'producer', 'soundtrack'])
     assert filmoset.issubset(set(person.get('filmography', {}).keys()))
 
 
 def test_person_filmography_should_contain_movies(ia):
-    person = ia.get_person('0000210', info=['main'])    # Julia Roberts
-    assert len(person.get('filmography', {}).get('actress')) > 60
+    person = ia.get_person('0000210', info=['filmography'])    # Julia Roberts
+    assert len(person.get('filmography', {}).get('actress')) >= 20
+
+
+def test_person_filmography_should_contain_many_roles(ia):
+    person = ia.get_person('0000110', info=['filmography'])    # Kenneth Branagh
+    filmography = person.get('filmography', {})
+    assert len(filmography) > 9
+    assert len(filmography.get('actor')) >= 70
+    assert len(filmography.get('writer')) >= 9
+    assert len(filmography.get('self')) >= 150
 
 
 def test_person_imdb_index_if_none_should_be_excluded(ia):
     person = ia.get_person('0000206', info=['main'])    # Keanu Reeves
     assert 'imdbIndex' not in person
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_person_otherworks.py` & `cinemagoer-2023.5.1/tests/test_http_person_otherworks.py`

 * *Files identical despite different names*

### Comparing `cinemagoer-2022.2.11/tests/test_http_search_keyword.py` & `cinemagoer-2023.5.1/tests/test_http_search_keyword.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 def test_search_keyword_check_list_of_keywords(ia):
     keywords = ia.search_keyword('zoolander')
-    assert 'reference-to-zoolander' in keywords
+    assert 'reference to zoolander' in keywords
 
 
 def test_search_keyword_if_multiple_should_list_correct_number_of_keywords(ia):
     keywords = ia.search_keyword('messiah')
-    assert 60 <= len(keywords) <= 120
+    assert len(keywords) == 25
 
 
 def test_search_keyword_if_too_many_should_list_upper_limit_of_keywords(ia):
     keywords = ia.search_keyword('computer')
-    assert len(keywords) == 200
+    assert len(keywords) == 25
 
 
 def test_search_keyword_if_none_result_should_be_empty(ia):
     keywords = ia.search_keyword('%e3%82%a2')
     assert keywords == []
 
 
 def test_get_keyword_pagination(ia):
     superheroes_without_page_param = ia.get_keyword('superhero')
     superheroes_page_one = ia.get_keyword('superhero', page=1)
     superheroes_page_two = ia.get_keyword('superhero', page=2)
     for i in range(50):
         assert superheroes_without_page_param[i]['title'] == superheroes_page_one[i]['title']
         assert superheroes_without_page_param[i]['title'] != superheroes_page_two[i]['title']
-
-
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_search_movie.py` & `cinemagoer-2023.5.1/tests/test_http_search_movie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+# -*- coding: utf-8 -*-
+from pytest import mark
+
+
 def test_search_movie_if_single_should_list_one_movie(ia):
     movies = ia.search_movie('od instituta do proizvodnje')
     assert len(movies) == 1
     assert movies[0].movieID == '0483758'
     assert movies[0]['kind'] == 'short'
     assert movies[0]['title'] == 'Od instituta do proizvodnje'
     assert movies[0]['year'] == 1971
 
 
 def test_search_movie_should_list_default_number_of_movies(ia):
     movies = ia.search_movie('movie')
     assert len(movies) == 20
 
 
+@mark.skip(reason="number of results limit is not honored anymore")
 def test_search_movie_limited_should_list_requested_number_of_movies(ia):
     movies = ia.search_movie('ace in the hole', results=98)
     assert len(movies) == 98
 
 
 def test_search_movie_unlimited_should_list_correct_number_of_movies(ia):
     movies = ia.search_movie('ace in the hole', results=500)
-    assert 185 <= len(movies) <= 200
+    assert len(movies) == 25
 
 
 def test_search_movie_if_too_many_result_should_list_upper_limit_of_movies(ia):
     movies = ia.search_movie('matrix', results=500)
-    assert len(movies) == 200
+    assert len(movies) == 25
 
 
 def test_search_movie_if_none_should_be_empty(ia):
-    movies = ia.search_movie('%e4%82%a2', results=500)
+    movies = ia.search_movie('ᚣ', results=500)
     assert movies == []
 
 
 def test_search_movie_entries_should_include_movie_id(ia):
     movies = ia.search_movie('matrix')
     assert movies[0].movieID == '0133093'
 
@@ -60,44 +65,47 @@
 
 
 def test_search_movie_entries_should_include_movie_year(ia):
     movies = ia.search_movie('matrix')
     assert movies[0]['year'] == 1999
 
 
+@mark.skip(reason="index is no longer shown on search results")
 def test_search_movie_entries_should_include_imdb_index(ia):
     movies = ia.search_movie('blink')
     movie_with_index = [m for m in movies if m.movieID == '6544524']
     assert len(movie_with_index) == 1
-    assert movie_with_index[0]['imdbIndex'] == 'IV'
+    assert movie_with_index[0]['imdbIndex'] == 'XXIV'
 
 
 def test_search_movie_entries_missing_imdb_index_should_be_excluded(ia):
     movies = ia.search_movie('matrix')
     assert 'imdbIndex' not in movies[0]
 
 
+@mark.skip(reason="AKAs are no longer shown on search results")
 def test_search_movie_entries_should_include_akas(ia):
     movies = ia.search_movie('Una calibro 20 per lo specialista')
     movie_with_aka = [m for m in movies if m.movieID == '0072288']
     assert len(movie_with_aka) == 1
     assert movie_with_aka[0]['akas'] == ['Una calibro 20 per lo specialista']
 
 
 def test_search_movie_entries_missing_akas_should_be_excluded(ia):
     movies = ia.search_movie('matrix')
     assert 'akas' not in movies[0]
 
 
+@mark.skip(reason="episode title are no longer shown on search results")
 def test_search_movie_episodes_should_include_season_and_number(ia):
     movies = ia.search_movie('swarley')  # How I Met Your Mother S02E07
     movie_with_season_and_episode = [m for m in movies if m.movieID == '0875360']
     assert len(movie_with_season_and_episode) == 1
     assert movie_with_season_and_episode[0]['season'] == 2
     assert movie_with_season_and_episode[0]['episode'] == 7
 
 
 def test_search_movie_entries_tv_mini_series_should_have_correct_kind(ia):
-    movies = ia.search_movie('capture 2019') # The Capture (2019)
+    movies = ia.search_movie('capture 2019')  # The Capture (2019)
     miniseries = [m for m in movies if m.movieID == '8201186']
     assert len(miniseries) == 1
     miniseries[0]['kind'] == 'tv mini series'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_search_movie_advanced.py` & `cinemagoer-2023.5.1/tests/test_http_search_movie_advanced.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import sys
 from pytest import mark
 
+import sys
+
 
 def test_search_results_should_include_correct_number_of_works_by_default(ia):
     movies = ia.search_movie_advanced('matrix')
     assert len(movies) == 20
 
 
 def test_search_results_should_include_correct_number_of_works(ia):
@@ -147,22 +148,22 @@
     movies = ia.search_movie_advanced('matrix', results=50)
     selected = [m for m in movies if m.movieID == '0133093'][0]
     assert selected['plot'].startswith('When a beautiful stranger')
 
 
 def test_selected_movie_should_have_correct_director_imdb_ids(ia):
     movies = ia.search_movie_advanced('matrix', results=50)
-    selected = [m for m in movies if m.movieID == '1830851'][0]
-    assert [p.personID for p in selected['directors']] == ['0649609']
+    selected = [m for m in movies if m.movieID == '10838180'][0]
+    assert [p.personID for p in selected['directors']] == ['0905154']
 
 
 def test_selected_work_should_have_correct_director_name(ia):
     movies = ia.search_movie_advanced('matrix', results=50)
-    selected = [m for m in movies if m.movieID == '1830851'][0]
-    assert [p['name'] for p in selected['directors']] == ['Josh Oreck']
+    selected = [m for m in movies if m.movieID == '10838180'][0]
+    assert [p['name'] for p in selected['directors']] == ['Lana Wachowski']
 
 
 def test_selected_work_should_have_correct_director_imdb_ids_if_multiple(ia):
     movies = ia.search_movie_advanced('matrix', results=50)
     selected = [m for m in movies if m.movieID == '0133093'][0]
     assert [p.personID for p in selected['directors']] == ['0905154', '0905152']
 
@@ -171,22 +172,22 @@
     movies = ia.search_movie_advanced('matrix', results=50)
     selected = [m for m in movies if m.movieID == '0133093'][0]
     assert [p['name'] for p in selected['directors']] == ['Lana Wachowski', 'Lilly Wachowski']
 
 
 def test_selected_work_should_have_correct_cast_imdb_id(ia):
     movies = ia.search_movie_advanced('matrix', results=50)
-    selected = [m for m in movies if m.movieID == '1830851'][0]
-    assert [p.personID for p in selected['cast']] == ['1047143']
+    selected = [m for m in movies if m.movieID == '11749868'][0]
+    assert [p.personID for p in selected['cast']] == ['4216365']
 
 
 def test_selected_work_should_have_correct_cast_name(ia):
     movies = ia.search_movie_advanced('matrix', results=50)
-    selected = [m for m in movies if m.movieID == '1830851'][0]
-    assert [p['name'] for p in selected['cast']] == ['Clayton Watson']
+    selected = [m for m in movies if m.movieID == '11749868'][0]
+    assert [p['name'] for p in selected['cast']] == ['Chris Harvey']
 
 
 def test_selected_work_should_have_correct_cast_imdb_ids_if_multiple(ia):
     movies = ia.search_movie_advanced('matrix', results=50)
     selected = [m for m in movies if m.movieID == '0133093'][0]
     assert [p.personID for p in selected['cast']] == ['0000206', '0000401', '0005251', '0915989']
 
@@ -334,21 +335,23 @@
 
 
 def test_selected_adult_movie_should_have_adult_in_genres(ia):
     movies = ia.search_movie_advanced('matrix', adult=True, results=250)
     selected = [m for m in movies if m.movieID == '0273126'][0]
     assert 'Adult' in selected['genres']
 
+
 @mark.skip('IMDb sorting works in misterious ways')
 def test_search_results_should_be_sortable_in_alphabetical_order_default_ascending(ia):
     movies = ia.search_movie_advanced(title='matrix', sort='alpha')
     titles = [m['title'] for m in movies]
     # assert all(a <= b for a, b in zip(titles, titles[1:]))  # fails due to IMDb
     assert sum(1 if a > b else 0 for a, b in zip(titles, titles[1:])) <= 1
 
+
 @mark.skip('IMDb sorting works in misterious ways')
 def test_search_results_should_be_sortable_in_alphabetical_order_ascending(ia):
     movies = ia.search_movie_advanced(title='matrix', sort='alpha', sort_dir='asc')
     titles = [m['title'] for m in movies]
     # assert all(a <= b for a, b in zip(titles, titles[1:]))  # fails due to IMDb
     assert sum(1 if a > b else 0 for a, b in zip(titles, titles[1:])) <= 1
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_search_movie_keyword.py` & `cinemagoer-2023.5.1/tests/test_http_search_movie_keyword.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 def test_get_keyword_should_list_correct_number_of_movies(ia):
     movies = ia.get_keyword('colander')
-    assert len(movies) == 6
+    assert 5 <= len(movies) <= 10
 
 
 def test_get_keyword_if_too_many_should_list_upper_limit_of_movies(ia):
     movies = ia.get_keyword('computer')
     assert len(movies) == 50
```

### Comparing `cinemagoer-2022.2.11/tests/test_http_search_person.py` & `cinemagoer-2023.5.1/tests/test_http_search_person.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from pytest import mark
 
+
 def test_search_person_should_list_default_number_of_people(ia):
     people = ia.search_person('julia')
     assert len(people) == 20
 
 
 def test_search_person_limited_should_list_requested_number_of_people(ia):
     people = ia.search_person('julia', results=11)
     assert len(people) == 11
 
 
-def test_search_person_unlimited_should_list_correct_number_of_people(ia):
-    people = ia.search_person('engelbart', results=500)
-    assert 120 <= len(people) <= 150
-
-
 def test_search_person_if_too_many_should_list_upper_limit_of_people(ia):
     people = ia.search_person('john', results=500)
-    assert len(people) == 200
+    assert len(people) == 25
 
 
 def test_search_person_if_none_result_should_be_empty(ia):
     people = ia.search_person('%e3%82%a2')
     assert people == []
 
 
@@ -30,29 +26,32 @@
     assert people[0].personID == '0000210'
 
 
 def test_search_person_entries_should_include_person_name(ia):
     people = ia.search_person('julia roberts')
     assert people[0]['name'] == 'Julia Roberts'
 
+
 def test_search_person_entries_should_include_headshot_if_available(ia):
     people = ia.search_person('julia roberts')
     assert 'headshot' in people[0]
 
+
 def test_search_person_entries_with_aka_should_exclude_name_in_aka(ia):
     people = ia.search_person('julia roberts')
     robertson = None
     for person in people:
         if person['name'] == 'Julia Robertson':
             robertson = person
             break
     assert robertson
     assert robertson['name'] == 'Julia Robertson'
 
 
+@mark.skip(reason="imdbIndex no longer included in results")
 def test_search_person_entries_should_include_person_index(ia):
     people = ia.search_person('julia roberts')
     assert people[0]['imdbIndex'] == 'I'
 
 
 @mark.skip(reason="no persons without imdbIndex in the first 20 results")
 def test_search_person_entries_missing_index_should_be_excluded(ia):
```

### Comparing `cinemagoer-2022.2.11/tests/test_in_operator.py` & `cinemagoer-2023.5.1/tests/test_in_operator.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 
 def test_key_in_movie(ia):
     movie = ia.get_movie('0133093', info=['main'])  # Matrix
     assert 'cast' in movie
 
 
 def test_movie_in_person(ia):
-    movie = ia.get_movie('0133093', info=['main'])  # Matrix
+    movie = ia.get_movie('10838180', info=['main'])  # The Matrix Resurrections
     person = ia.get_person('0000206', info=['main'])  # Keanu Reeves
     assert movie in person
 
 
 def test_key_in_person(ia):
     person = ia.get_person('0000206')  # Keanu Reeves
     assert 'filmography' in person
 
 
 def test_key_in_company(ia):
     company = ia.get_company('0017902', info=['main'])  # Pixar
     assert 'name' in company
-
```

