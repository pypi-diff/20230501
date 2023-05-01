# Comparing `tmp/graphql-server-3.0.0b5.tar.gz` & `tmp/graphql-server-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-server-3.0.0b5.tar", last modified: Mon Jan 17 13:36:33 2022, max compression
+gzip compressed data, was "graphql-server-3.0.0b6.tar", last modified: Mon May  1 12:09:38 2023, max compression
```

## Comparing `graphql-server-3.0.0b5.tar` & `graphql-server-3.0.0b6.tar`

### file list

```diff
@@ -1,83 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.748340 graphql-server-3.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-01-17 13:36:33.748340 graphql-server-3.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.736340 graphql-server-3.0.0b5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.736340 graphql-server-3.0.0b5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    10225 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/docs/_static/graphql-server-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4041 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/docs/aiohttp.md
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/docs/flask.md
--rw-r--r--   0 runner    (1001) docker     (121)     3642 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/docs/sanic.md
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/docs/webob.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.736340 graphql-server-3.0.0b5/graphql_server/
--rw-r--r--   0 runner    (1001) docker     (121)    12167 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/graphql_server/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8749 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/aiohttp/graphqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/graphql_server/flask/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6189 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/flask/graphqlview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/graphql_server/quart/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7314 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/quart/graphqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)    11152 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/render_graphiql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/graphql_server/sanic/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/sanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/sanic/graphqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/graphql_server/webob/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6430 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/graphql_server/webob/graphqlview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/graphql_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4151 2022-01-17 13:36:33.000000 graphql-server-3.0.0b5/graphql_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-01-17 13:36:33.000000 graphql-server-3.0.0b5/graphql_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 13:36:33.000000 graphql-server-3.0.0b5/graphql_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-17 13:36:33.000000 graphql-server-3.0.0b5/graphql_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-01-17 13:36:33.000000 graphql-server-3.0.0b5/graphql_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-17 13:36:33.000000 graphql-server-3.0.0b5/graphql_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-01-17 13:36:33.748340 graphql-server-3.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2647 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.740340 graphql-server-3.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.744340 graphql-server-3.0.0b5/tests/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/aiohttp/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/aiohttp/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4223 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/aiohttp/test_graphiqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)    19927 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/aiohttp/test_graphqlview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.744340 graphql-server-3.0.0b5/tests/flask/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/flask/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/flask/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/flask/test_graphiqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)    16918 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/flask/test_graphqlview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.744340 graphql-server-3.0.0b5/tests/quart/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/quart/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/quart/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/quart/test_graphiqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)    22026 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/quart/test_graphqlview.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.744340 graphql-server-3.0.0b5/tests/sanic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/sanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/sanic/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/sanic/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/sanic/test_graphiqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)    19103 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/sanic/test_graphqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    18562 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:33.748340 graphql-server-3.0.0b5/tests/webob/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/webob/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/webob/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/webob/test_graphiqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)    16592 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tests/webob/test_graphqlview.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-01-17 13:36:31.000000 graphql-server-3.0.0b5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.073648 graphql-server-3.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-01 12:09:38.073648 graphql-server-3.0.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.065647 graphql-server-3.0.0b6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.065647 graphql-server-3.0.0b6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/docs/_static/graphql-server-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/docs/aiohttp.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/docs/flask.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/docs/sanic.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/docs/webob.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.065647 graphql-server-3.0.0b6/graphql_server/
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/graphql_server/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/aiohttp/graphqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/graphql_server/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/flask/graphqlview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/graphql_server/quart/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/quart/graphqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/render_graphiql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/graphql_server/sanic/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/sanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/sanic/graphqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/graphql_server/webob/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/graphql_server/webob/graphqlview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.065647 graphql-server-3.0.0b6/graphql_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-01 12:09:38.000000 graphql-server-3.0.0b6/graphql_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-01 12:09:38.000000 graphql-server-3.0.0b6/graphql_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:09:38.000000 graphql-server-3.0.0b6/graphql_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:09:38.000000 graphql-server-3.0.0b6/graphql_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-01 12:09:38.000000 graphql-server-3.0.0b6/graphql_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 12:09:38.000000 graphql-server-3.0.0b6/graphql_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-01 12:09:38.073648 graphql-server-3.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/tests/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/aiohttp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/aiohttp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/aiohttp/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/aiohttp/test_graphiqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/aiohttp/test_graphqlview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/tests/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/flask/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/flask/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/flask/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/flask/test_graphiqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/flask/test_graphqlview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/tests/quart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/quart/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/quart/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/quart/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/quart/test_graphiqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/quart/test_graphqlview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.069647 graphql-server-3.0.0b6/tests/sanic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/sanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/sanic/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/sanic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/sanic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/sanic/test_graphiqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/sanic/test_graphqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:38.073648 graphql-server-3.0.0b6/tests/webob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/webob/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/webob/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/webob/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/webob/test_graphiqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tests/webob/test_graphqlview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 12:09:35.000000 graphql-server-3.0.0b6/tox.ini
```

### Comparing `graphql-server-3.0.0b5/CONTRIBUTING.md` & `graphql-server-3.0.0b6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/LICENSE` & `graphql-server-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/PKG-INFO` & `graphql-server-3.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: graphql-server
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: GraphQL Server tools for powering your server
 Home-page: https://github.com/graphql-python/graphql-server
+Download-URL: https://github.com/graphql-python/graphql-server/releases
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
-Download-URL: https://github.com/graphql-python/graphql-server/releases
 Keywords: api graphql protocol rest
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -79,9 +79,7 @@
 blueprint to build your own integration or GraphQL server implementations.
 
 Please let us know when you have built something new, so we can list it here.
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/graphql-python/graphql-server/blob/master/CONTRIBUTING.md)
-
-
```

### Comparing `graphql-server-3.0.0b5/README.md` & `graphql-server-3.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/docs/_static/graphql-server-logo.svg` & `graphql-server-3.0.0b6/docs/_static/graphql-server-logo.svg`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/docs/aiohttp.md` & `graphql-server-3.0.0b6/docs/aiohttp.md`

 * *Files 6% similar despite different names*

```diff
@@ -43,27 +43,27 @@
 ```python
 gql_view = GraphQLView(schema=Schema, **kwargs)
 gql_view(request)  # <-- the instance is callable and expects a `aiohttp.web.Request` object.
 ```
 
 ### Supported options for GraphQLView
 
- * `schema`: The `GraphQLSchema` object that you want the view to execute when it gets a valid request.
+ * `schema`: The GraphQL schema object that you want the view to execute when it gets a valid request. Accepts either an object of type `GraphQLSchema` from `graphql-core` or `Schema` from `graphene`. For Graphene v3, passing either `schema: graphene.Schema` or `schema.graphql_schema` is allowed.
  * `context`: A value to pass as the `context_value` to graphql `execute` function. By default is set to `dict` with request object at key `request`.
  * `root_value`: The `root_value` you want to provide to graphql `execute`.
  * `pretty`: Whether or not you want the response to be pretty printed JSON.
  * `graphiql`: If `True`, may present [GraphiQL](https://github.com/graphql/graphiql) when loaded directly from a browser (a useful tool for debugging and exploration).
- * `graphiql_version`: The graphiql version to load. Defaults to **"1.0.3"**.
+ * `graphiql_version`: The graphiql version to load. Defaults to **"2.2.0"**.
  * `graphiql_template`: Inject a Jinja template string to customize GraphiQL.
  * `graphiql_html_title`: The graphiql title to display. Defaults to **"GraphiQL"**.
- * `jinja_env`: Sets jinja environment to be used to process GraphiQL template. If Jinja’s async mode is enabled (by `enable_async=True`), uses 
-`Template.render_async` instead of `Template.render`. If environment is not set, fallbacks to simple regex-based renderer.
+ * `jinja_env`: Sets jinja environment to be used to process GraphiQL template. If Jinja’s async mode is enabled (by `enable_async=True`), uses `Template.render_async` instead of `Template.render`. If environment is not set, fallbacks to simple regex-based renderer.
  * `batch`: Set the GraphQL view as batch (for using in [Apollo-Client](http://dev.apollodata.com/core/network.html#query-batching) or [ReactRelayNetworkLayer](https://github.com/nodkz/react-relay-network-layer))
  * `middleware`: A list of graphql [middlewares](http://docs.graphene-python.org/en/latest/execution/middleware/).
  * `validation_rules`: A list of graphql validation rules.
+ * `execution_context_class`: Specifies a custom execution context class.
  * `max_age`: Sets the response header Access-Control-Max-Age for preflight requests.
  * `encode`: the encoder to use for responses (sensibly defaults to `graphql_server.json_encode`).
  * `format_error`: the error formatter to use for responses (sensibly defaults to `graphql_server.default_format_error`.
  * `enable_async`: whether `async` mode will be enabled.
  * `subscriptions`: The GraphiQL socket endpoint for using subscriptions in graphql-ws.
  * `headers`: An optional GraphQL string to use as the initial displayed request headers, if not provided, the stored headers will be used.
  * `default_query`: An optional GraphQL string to use when no query is provided and no stored query exists from a previous session. If not provided, GraphiQL will use its own default query.
```

### Comparing `graphql-server-3.0.0b5/docs/flask.md` & `graphql-server-3.0.0b6/docs/flask.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,34 +35,29 @@
 
 if __name__ == '__main__':
     app.run()
 ```
 
 This will add `/graphql` endpoint to your app and enable the GraphiQL IDE.
 
-### Special Note for Graphene v3
-
-If you are using the `Schema` type of [Graphene](https://github.com/graphql-python/graphene) library, be sure to use the `graphql_schema` attribute to pass as schema on the `GraphQLView` view. Otherwise, the `GraphQLSchema` from `graphql-core` is the way to go.
-
-More info at [Graphene v3 release notes](https://github.com/graphql-python/graphene/wiki/v3-release-notes#graphene-schema-no-longer-subclasses-graphqlschema-type) and [GraphQL-core 3 usage](https://github.com/graphql-python/graphql-core#usage).
-
-
 ### Supported options for GraphQLView
 
- * `schema`: The `GraphQLSchema` object that you want the view to execute when it gets a valid request.
+ * `schema`: The GraphQL schema object that you want the view to execute when it gets a valid request. Accepts either an object of type `GraphQLSchema` from `graphql-core` or `Schema` from `graphene`. For Graphene v3, passing either `schema: graphene.Schema` or `schema.graphql_schema` is allowed.
  * `context`: A value to pass as the `context_value` to graphql `execute` function. By default is set to `dict` with request object at key `request`.
  * `root_value`: The `root_value` you want to provide to graphql `execute`.
  * `pretty`: Whether or not you want the response to be pretty printed JSON.
  * `graphiql`: If `True`, may present [GraphiQL](https://github.com/graphql/graphiql) when loaded directly from a browser (a useful tool for debugging and exploration).
- * `graphiql_version`: The graphiql version to load. Defaults to **"1.0.3"**.
+ * `graphiql_version`: The graphiql version to load. Defaults to **"2.2.0"**.
  * `graphiql_template`: Inject a Jinja template string to customize GraphiQL.
  * `graphiql_html_title`: The graphiql title to display. Defaults to **"GraphiQL"**.
+ * `jinja_env`: Sets jinja environment to be used to process GraphiQL template. If environment is not set, fallbacks to simple regex-based renderer.
  * `batch`: Set the GraphQL view as batch (for using in [Apollo-Client](http://dev.apollodata.com/core/network.html#query-batching) or [ReactRelayNetworkLayer](https://github.com/nodkz/react-relay-network-layer))
  * `middleware`: A list of graphql [middlewares](http://docs.graphene-python.org/en/latest/execution/middleware/).
- * `validation_rules`: A list of graphql validation rules.   
+ * `validation_rules`: A list of graphql validation rules.
+ * `execution_context_class`: Specifies a custom execution context class.
  * `encode`: the encoder to use for responses (sensibly defaults to `graphql_server.json_encode`).
  * `format_error`: the error formatter to use for responses (sensibly defaults to `graphql_server.default_format_error`.
  * `subscriptions`: The GraphiQL socket endpoint for using subscriptions in graphql-ws.
  * `headers`: An optional GraphQL string to use as the initial displayed request headers, if not provided, the stored headers will be used.
  * `default_query`: An optional GraphQL string to use when no query is provided and no stored query exists from a previous session. If not provided, GraphiQL will use its own default query.
 * `header_editor_enabled`: An optional boolean which enables the header editor when true. Defaults to **false**.
 * `should_persist_headers`:  An optional boolean which enables to persist headers to storage when true. Defaults to **false**.
@@ -75,8 +70,8 @@
 class UserRootValue(GraphQLView):
     def get_root_value(self, request):
         return request.user
 
 ```
 
 ## Contributing
-See [CONTRIBUTING.md](../CONTRIBUTING.md)
+See [CONTRIBUTING.md](../CONTRIBUTING.md)
```

### Comparing `graphql-server-3.0.0b5/docs/sanic.md` & `graphql-server-3.0.0b6/docs/sanic.md`

 * *Files 9% similar despite different names*

```diff
@@ -35,27 +35,27 @@
     app.run(host='0.0.0.0', port=8000)
 ```
 
 This will add `/graphql` endpoint to your app and enable the GraphiQL IDE.
 
 ### Supported options for GraphQLView
 
- * `schema`: The `GraphQLSchema` object that you want the view to execute when it gets a valid request.
+ * `schema`: The GraphQL schema object that you want the view to execute when it gets a valid request. Accepts either an object of type `GraphQLSchema` from `graphql-core` or `Schema` from `graphene`. For Graphene v3, passing either `schema: graphene.Schema` or `schema.graphql_schema` is allowed.
  * `context`: A value to pass as the `context_value` to graphql `execute` function. By default is set to `dict` with request object at key `request`.
  * `root_value`: The `root_value` you want to provide to graphql `execute`.
  * `pretty`: Whether or not you want the response to be pretty printed JSON.
  * `graphiql`: If `True`, may present [GraphiQL](https://github.com/graphql/graphiql) when loaded directly from a browser (a useful tool for debugging and exploration).
- * `graphiql_version`: The graphiql version to load. Defaults to **"1.0.3"**.
+ * `graphiql_version`: The graphiql version to load. Defaults to **"2.2.0"**.
  * `graphiql_template`: Inject a Jinja template string to customize GraphiQL.
  * `graphiql_html_title`: The graphiql title to display. Defaults to **"GraphiQL"**.
- * `jinja_env`: Sets jinja environment to be used to process GraphiQL template. If Jinja’s async mode is enabled (by `enable_async=True`), uses 
-`Template.render_async` instead of `Template.render`. If environment is not set, fallbacks to simple regex-based renderer.
+ * `jinja_env`: Sets jinja environment to be used to process GraphiQL template. If Jinja’s async mode is enabled (by `enable_async=True`), uses `Template.render_async` instead of `Template.render`. If environment is not set, fallbacks to simple regex-based renderer.
  * `batch`: Set the GraphQL view as batch (for using in [Apollo-Client](http://dev.apollodata.com/core/network.html#query-batching) or [ReactRelayNetworkLayer](https://github.com/nodkz/react-relay-network-layer))
  * `middleware`: A list of graphql [middlewares](http://docs.graphene-python.org/en/latest/execution/middleware/).
- * `validation_rules`: A list of graphql validation rules.   
+ * `validation_rules`: A list of graphql validation rules.
+ * `execution_context_class`: Specifies a custom execution context class.
  * `max_age`: Sets the response header Access-Control-Max-Age for preflight requests.
  * `encode`: the encoder to use for responses (sensibly defaults to `graphql_server.json_encode`).
  * `format_error`: the error formatter to use for responses (sensibly defaults to `graphql_server.default_format_error`.
  * `enable_async`: whether `async` mode will be enabled.
  * `subscriptions`: The GraphiQL socket endpoint for using subscriptions in graphql-ws.
  * `headers`: An optional GraphQL string to use as the initial displayed request headers, if not provided, the stored headers will be used.
  * `default_query`: An optional GraphQL string to use when no query is provided and no stored query exists from a previous session. If not provided, GraphiQL will use its own default query.
@@ -68,8 +68,8 @@
 ```python
 class UserRootValue(GraphQLView):
     def get_root_value(self, request):
         return request.user
 ```
 
 ## Contributing
-See [CONTRIBUTING.md](../CONTRIBUTING.md)
+See [CONTRIBUTING.md](../CONTRIBUTING.md)
```

### Comparing `graphql-server-3.0.0b5/docs/webob.md` & `graphql-server-3.0.0b6/docs/webob.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,29 +34,31 @@
     server.serve_forever()
 ```
 
 This will add `/graphql` endpoint to your app and enable the GraphiQL IDE.
 
 ### Supported options for GraphQLView
 
- * `schema`: The `GraphQLSchema` object that you want the view to execute when it gets a valid request.
+ * `schema`: The GraphQL schema object that you want the view to execute when it gets a valid request. Accepts either an object of type `GraphQLSchema` from `graphql-core` or `Schema` from `graphene`. For Graphene v3, passing either `schema: graphene.Schema` or `schema.graphql_schema` is allowed.
  * `context`: A value to pass as the `context_value` to graphql `execute` function. By default is set to `dict` with request object at key `request`.
  * `root_value`: The `root_value` you want to provide to graphql `execute`.
  * `pretty`: Whether or not you want the response to be pretty printed JSON.
  * `graphiql`: If `True`, may present [GraphiQL](https://github.com/graphql/graphiql) when loaded directly from a browser (a useful tool for debugging and exploration).
- * `graphiql_version`: The graphiql version to load. Defaults to **"1.0.3"**.
+ * `graphiql_version`: The graphiql version to load. Defaults to **"2.2.0"**.
  * `graphiql_template`: Inject a Jinja template string to customize GraphiQL.
  * `graphiql_html_title`: The graphiql title to display. Defaults to **"GraphiQL"**.
+ * `jinja_env`: Sets jinja environment to be used to process GraphiQL template. If environment is not set, fallbacks to simple regex-based renderer.
  * `batch`: Set the GraphQL view as batch (for using in [Apollo-Client](http://dev.apollodata.com/core/network.html#query-batching) or [ReactRelayNetworkLayer](https://github.com/nodkz/react-relay-network-layer))
  * `middleware`: A list of graphql [middlewares](http://docs.graphene-python.org/en/latest/execution/middleware/).
- * `validation_rules`: A list of graphql validation rules.   
+ * `validation_rules`: A list of graphql validation rules.
+ * `execution_context_class`: Specifies a custom execution context class.
  * `encode`: the encoder to use for responses (sensibly defaults to `graphql_server.json_encode`).
  * `format_error`: the error formatter to use for responses (sensibly defaults to `graphql_server.default_format_error`.
  * `enable_async`: whether `async` mode will be enabled.
  * `subscriptions`: The GraphiQL socket endpoint for using subscriptions in graphql-ws.
  * `headers`: An optional GraphQL string to use as the initial displayed request headers, if not provided, the stored headers will be used.
  * `default_query`: An optional GraphQL string to use when no query is provided and no stored query exists from a previous session. If not provided, GraphiQL will use its own default query.
 * `header_editor_enabled`: An optional boolean which enables the header editor when true. Defaults to **false**.
 * `should_persist_headers`:  An optional boolean which enables to persist headers to storage when true. Defaults to **false**.
 
 ## Contributing
-See [CONTRIBUTING.md](../CONTRIBUTING.md)
+See [CONTRIBUTING.md](../CONTRIBUTING.md)
```

### Comparing `graphql-server-3.0.0b5/graphql_server/__init__.py` & `graphql-server-3.0.0b6/graphql_server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,15 @@
 GraphQL-Server is a base library that serves as a helper
 for building GraphQL servers or integrations into existing web frameworks using
 [GraphQL-Core](https://github.com/graphql-python/graphql-core).
 """
 import json
 from collections import namedtuple
 from collections.abc import MutableMapping
-from typing import (
-    Any,
-    Callable,
-    Collection,
-    Dict,
-    List,
-    Optional,
-    Type,
-    Union,
-    cast,
-)
+from typing import Any, Callable, Collection, Dict, List, Optional, Type, Union, cast
 
 from graphql.error import GraphQLError
 from graphql.execution import ExecutionResult, execute
 from graphql.language import OperationType, parse
 from graphql.pyutils import AwaitableOrValue
 from graphql.type import GraphQLSchema, validate_schema
 from graphql.utilities import get_operation_ast
@@ -341,7 +331,21 @@
                 status_code = 400
             else:
                 response["data"] = execution_result.data
         else:
             response = {"data": execution_result.data}
 
     return FormattedResult(response, status_code)
+
+
+def _check_jinja(jinja_env: Any) -> None:
+    try:
+        from jinja2 import Environment
+    except ImportError:  # pragma: no cover
+        raise RuntimeError(
+            "Attempt to set 'jinja_env' to a value other than None while Jinja2 is not installed.\n"
+            "Please install Jinja2 to render GraphiQL with Jinja2.\n"
+            "Otherwise set 'jinja_env' to None to use the simple regex renderer."
+        )
+
+    if not isinstance(jinja_env, Environment):  # pragma: no cover
+        raise TypeError("'jinja_env' has to be of type jinja2.Environment.")
```

### Comparing `graphql-server-3.0.0b5/graphql_server/aiohttp/graphqlview.py` & `graphql-server-3.0.0b6/graphql_server/aiohttp/graphqlview.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,49 @@
+import asyncio
 import copy
 from collections.abc import MutableMapping
 from functools import partial
 from typing import List
 
 from aiohttp import web
-from graphql import ExecutionResult, GraphQLError, specified_rules
+from graphql import GraphQLError, specified_rules
+from graphql.pyutils import is_awaitable
 from graphql.type.schema import GraphQLSchema
 
 from graphql_server import (
     GraphQLParams,
     HttpQueryError,
+    _check_jinja,
     encode_execution_results,
     format_error_default,
     json_encode,
     load_json_body,
     run_http_query,
 )
 from graphql_server.render_graphiql import (
     GraphiQLConfig,
     GraphiQLData,
     GraphiQLOptions,
     render_graphiql_async,
 )
+from graphql_server.utils import wrap_in_async
 
 
 class GraphQLView:
     schema = None
     root_value = None
     context = None
     pretty = False
     graphiql = False
     graphiql_version = None
     graphiql_template = None
     graphiql_html_title = None
     middleware = None
     validation_rules = None
+    execution_context_class = None
     batch = False
     jinja_env = None
     max_age = 86400
     enable_async = False
     subscriptions = None
     headers = None
     default_query = None
@@ -58,35 +63,41 @@
 
         if not isinstance(self.schema, GraphQLSchema):
             # maybe the GraphQL schema is wrapped in a Graphene schema
             self.schema = getattr(self.schema, "graphql_schema", None)
             if not isinstance(self.schema, GraphQLSchema):
                 raise TypeError("A Schema is required to be provided to GraphQLView.")
 
+        if self.jinja_env is not None:
+            _check_jinja(self.jinja_env)
+
     def get_root_value(self):
         return self.root_value
 
     def get_context(self, request):
         context = (
             copy.copy(self.context)
-            if self.context and isinstance(self.context, MutableMapping)
+            if self.context is not None and isinstance(self.context, MutableMapping)
             else {}
         )
         if isinstance(context, MutableMapping) and "request" not in context:
             context.update({"request": request})
         return context
 
     def get_middleware(self):
         return self.middleware
 
     def get_validation_rules(self):
         if self.validation_rules is None:
             return specified_rules
         return self.validation_rules
 
+    def get_execution_context_class(self):
+        return self.execution_context_class
+
     @staticmethod
     async def parse_body(request):
         content_type = request.content_type
         # request.text() is the aiohttp equivalent to
         # request.body.decode("utf8")
         if content_type == "application/graphql":
             r_text = await request.text()
@@ -154,21 +165,26 @@
                 catch=is_graphiql,
                 # Execute options
                 run_sync=not self.enable_async,
                 root_value=self.get_root_value(),
                 context_value=self.get_context(request),
                 middleware=self.get_middleware(),
                 validation_rules=self.get_validation_rules(),
+                execution_context_class=self.get_execution_context_class(),
             )
 
             exec_res = (
-                [
-                    ex if ex is None or isinstance(ex, ExecutionResult) else await ex
-                    for ex in execution_results
-                ]
+                await asyncio.gather(
+                    *(
+                        ex
+                        if ex is not None and is_awaitable(ex)
+                        else wrap_in_async(lambda: ex)()
+                        for ex in execution_results
+                    )
+                )
                 if self.enable_async
                 else execution_results
             )
             result, status_code = encode_execution_results(
                 exec_res,
                 is_batch=isinstance(data, list),
                 format_error=self.format_error,
```

### Comparing `graphql-server-3.0.0b5/graphql_server/error.py` & `graphql-server-3.0.0b6/graphql_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/graphql_server/flask/graphqlview.py` & `graphql-server-3.0.0b6/graphql_server/flask/graphqlview.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from graphql import specified_rules
 from graphql.error import GraphQLError
 from graphql.type.schema import GraphQLSchema
 
 from graphql_server import (
     GraphQLParams,
     HttpQueryError,
+    _check_jinja,
     encode_execution_results,
     format_error_default,
     json_encode,
     load_json_body,
     run_http_query,
 )
 from graphql_server.render_graphiql import (
@@ -33,15 +34,17 @@
     pretty = False
     graphiql = False
     graphiql_version = None
     graphiql_template = None
     graphiql_html_title = None
     middleware = None
     validation_rules = None
+    execution_context_class = None
     batch = False
+    jinja_env = None
     subscriptions = None
     headers = None
     default_query = None
     header_editor_enabled = None
     should_persist_headers = None
 
     methods = ["GET", "POST", "PUT", "DELETE"]
@@ -57,35 +60,41 @@
 
         if not isinstance(self.schema, GraphQLSchema):
             # maybe the GraphQL schema is wrapped in a Graphene schema
             self.schema = getattr(self.schema, "graphql_schema", None)
             if not isinstance(self.schema, GraphQLSchema):
                 raise TypeError("A Schema is required to be provided to GraphQLView.")
 
+        if self.jinja_env is not None:
+            _check_jinja(self.jinja_env)
+
     def get_root_value(self):
         return self.root_value
 
     def get_context(self):
         context = (
             copy.copy(self.context)
-            if self.context and isinstance(self.context, MutableMapping)
+            if self.context is not None and isinstance(self.context, MutableMapping)
             else {}
         )
         if isinstance(context, MutableMapping) and "request" not in context:
             context.update({"request": request})
         return context
 
     def get_middleware(self):
         return self.middleware
 
     def get_validation_rules(self):
         if self.validation_rules is None:
             return specified_rules
         return self.validation_rules
 
+    def get_execution_context_class(self):
+        return self.execution_context_class
+
     def dispatch_request(self):
         try:
             request_method = request.method.lower()
             data = self.parse_body()
 
             show_graphiql = request_method == "get" and self.should_display_graphiql()
             catch = show_graphiql
@@ -101,14 +110,15 @@
                 batch_enabled=self.batch,
                 catch=catch,
                 # Execute options
                 root_value=self.get_root_value(),
                 context_value=self.get_context(),
                 middleware=self.get_middleware(),
                 validation_rules=self.get_validation_rules(),
+                execution_context_class=self.get_execution_context_class(),
             )
             result, status_code = encode_execution_results(
                 execution_results,
                 is_batch=isinstance(data, list),
                 format_error=self.format_error,
                 encode=partial(self.encode, pretty=pretty),  # noqa
             )
@@ -122,15 +132,15 @@
                     subscription_url=self.subscriptions,
                     headers=self.headers,
                 )
                 graphiql_config = GraphiQLConfig(
                     graphiql_version=self.graphiql_version,
                     graphiql_template=self.graphiql_template,
                     graphiql_html_title=self.graphiql_html_title,
-                    jinja_env=None,
+                    jinja_env=self.jinja_env,
                 )
                 graphiql_options = GraphiQLOptions(
                     default_query=self.default_query,
                     header_editor_enabled=self.header_editor_enabled,
                     should_persist_headers=self.should_persist_headers,
                 )
                 source = render_graphiql_sync(
```

### Comparing `graphql-server-3.0.0b5/graphql_server/quart/graphqlview.py` & `graphql-server-3.0.0b6/graphql_server/quart/graphqlview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,53 @@
+import asyncio
 import copy
-import sys
 from collections.abc import MutableMapping
 from functools import partial
 from typing import List
 
-from graphql import ExecutionResult, specified_rules
+from graphql import specified_rules
 from graphql.error import GraphQLError
+from graphql.pyutils import is_awaitable
 from graphql.type.schema import GraphQLSchema
 from quart import Response, render_template_string, request
 from quart.views import View
 
 from graphql_server import (
     GraphQLParams,
     HttpQueryError,
+    _check_jinja,
     encode_execution_results,
     format_error_default,
     json_encode,
     load_json_body,
     run_http_query,
 )
 from graphql_server.render_graphiql import (
     GraphiQLConfig,
     GraphiQLData,
     GraphiQLOptions,
     render_graphiql_sync,
 )
+from graphql_server.utils import wrap_in_async
 
 
 class GraphQLView(View):
     schema = None
     root_value = None
     context = None
     pretty = False
     graphiql = False
     graphiql_version = None
     graphiql_template = None
     graphiql_html_title = None
     middleware = None
     validation_rules = None
+    execution_context_class = None
     batch = False
+    jinja_env = None
     enable_async = False
     subscriptions = None
     headers = None
     default_query = None
     header_editor_enabled = None
     should_persist_headers = None
 
@@ -59,35 +64,41 @@
 
         if not isinstance(self.schema, GraphQLSchema):
             # maybe the GraphQL schema is wrapped in a Graphene schema
             self.schema = getattr(self.schema, "graphql_schema", None)
             if not isinstance(self.schema, GraphQLSchema):
                 raise TypeError("A Schema is required to be provided to GraphQLView.")
 
+        if self.jinja_env is not None:
+            _check_jinja(self.jinja_env)
+
     def get_root_value(self):
         return self.root_value
 
     def get_context(self):
         context = (
             copy.copy(self.context)
-            if self.context and isinstance(self.context, MutableMapping)
+            if self.context is not None and isinstance(self.context, MutableMapping)
             else {}
         )
         if isinstance(context, MutableMapping) and "request" not in context:
             context.update({"request": request})
         return context
 
     def get_middleware(self):
         return self.middleware
 
     def get_validation_rules(self):
         if self.validation_rules is None:
             return specified_rules
         return self.validation_rules
 
+    def get_execution_context_class(self):
+        return self.execution_context_class
+
     async def dispatch_request(self):
         try:
             request_method = request.method.lower()
             data = await self.parse_body()
 
             show_graphiql = request_method == "get" and self.should_display_graphiql()
             catch = show_graphiql
@@ -103,20 +114,25 @@
                 catch=catch,
                 # Execute options
                 run_sync=not self.enable_async,
                 root_value=self.get_root_value(),
                 context_value=self.get_context(),
                 middleware=self.get_middleware(),
                 validation_rules=self.get_validation_rules(),
+                execution_context_class=self.get_execution_context_class(),
             )
             exec_res = (
-                [
-                    ex if ex is None or isinstance(ex, ExecutionResult) else await ex
-                    for ex in execution_results
-                ]
+                await asyncio.gather(
+                    *(
+                        ex
+                        if ex is not None and is_awaitable(ex)
+                        else wrap_in_async(lambda: ex)()
+                        for ex in execution_results
+                    )
+                )
                 if self.enable_async
                 else execution_results
             )
             result, status_code = encode_execution_results(
                 exec_res,
                 is_batch=isinstance(data, list),
                 format_error=self.format_error,
@@ -132,15 +148,15 @@
                     subscription_url=self.subscriptions,
                     headers=self.headers,
                 )
                 graphiql_config = GraphiQLConfig(
                     graphiql_version=self.graphiql_version,
                     graphiql_template=self.graphiql_template,
                     graphiql_html_title=self.graphiql_html_title,
-                    jinja_env=None,
+                    jinja_env=self.jinja_env,
                 )
                 graphiql_options = GraphiQLOptions(
                     default_query=self.default_query,
                     header_editor_enabled=self.header_editor_enabled,
                     should_persist_headers=self.should_persist_headers,
                 )
                 source = render_graphiql_sync(
@@ -161,19 +177,19 @@
 
     @staticmethod
     async def parse_body():
         # We use mimetype here since we don't need the other
         # information provided by content_type
         content_type = request.mimetype
         if content_type == "application/graphql":
-            refined_data = await request.get_data(raw=False)
+            refined_data = await request.get_data(as_text=True)
             return {"query": refined_data}
 
         elif content_type == "application/json":
-            refined_data = await request.get_data(raw=False)
+            refined_data = await request.get_data(as_text=True)
             return load_json_body(refined_data)
 
         elif content_type == "application/x-www-form-urlencoded":
             return await request.form
 
         # TODO: Fix this check
         elif content_type == "multipart/form-data":
@@ -187,24 +203,12 @@
 
         return self.request_wants_html()
 
     @staticmethod
     def request_wants_html():
         best = request.accept_mimetypes.best_match(["application/json", "text/html"])
 
-        # Needed as this was introduced at Quart 0.8.0: https://gitlab.com/pgjones/quart/-/issues/189
-        def _quality(accept, key: str) -> float:
-            for option in accept.options:
-                if accept._values_match(key, option.value):
-                    return option.quality
-            return 0.0
-
-        if sys.version_info >= (3, 7):
-            return (
-                best == "text/html"
-                and request.accept_mimetypes[best]
-                > request.accept_mimetypes["application/json"]
-            )
-        else:
-            return best == "text/html" and _quality(
-                request.accept_mimetypes, best
-            ) > _quality(request.accept_mimetypes, "application/json")
+        return (
+            best == "text/html"
+            and request.accept_mimetypes[best]
+            > request.accept_mimetypes["application/json"]
+        )
```

### Comparing `graphql-server-3.0.0b5/graphql_server/render_graphiql.py` & `graphql-server-3.0.0b6/graphql_server/render_graphiql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-"""Based on (express-graphql)[https://github.com/graphql/express-graphql/blob/master/src/renderGraphiQL.js] and
-(subscriptions-transport-ws)[https://github.com/apollographql/subscriptions-transport-ws]"""
+"""Based on (express-graphql)[https://github.com/graphql/express-graphql/blob/main/src/renderGraphiQL.ts] and
+(graphql-ws)[https://github.com/enisdenjo/graphql-ws]"""
 import json
 import re
 from typing import Any, Dict, Optional, Tuple
 
-from jinja2 import Environment
+# This Environment import is only for type checking purpose,
+# and only relevant if rendering GraphiQL with Jinja
+try:
+    from jinja2 import Environment
+except ImportError:  # pragma: no cover
+    pass
+
 from typing_extensions import TypedDict
 
-GRAPHIQL_VERSION = "1.0.3"
+GRAPHIQL_VERSION = "2.2.0"
 
 GRAPHIQL_TEMPLATE = """<!--
 The request to this GraphQL server provided the header "Accept: text/html"
 and as a result has been presented GraphiQL - an in-browser IDE for
 exploring GraphQL.
 If you wish to receive JSON, provide the header "Accept: application/json" or
 add "&raw" to the end of the URL within a browser.
@@ -30,21 +36,20 @@
       overflow: hidden;
     }
     #graphiql {
       height: 100vh;
     }
   </style>
   <link href="//cdn.jsdelivr.net/npm/graphiql@{{graphiql_version}}/graphiql.css" rel="stylesheet" />
-  <script src="//cdn.jsdelivr.net/npm/promise-polyfill@8.1.3/dist/polyfill.min.js"></script>
-  <script src="//cdn.jsdelivr.net/npm/unfetch@4.1.0/dist/unfetch.umd.js"></script>
-  <script src="//cdn.jsdelivr.net/npm/react@16.13.1/umd/react.production.min.js"></script>
-  <script src="//cdn.jsdelivr.net/npm/react-dom@16.13.1/umd/react-dom.production.min.js"></script>
+  <script src="//cdn.jsdelivr.net/npm/promise-polyfill@8.2.3/dist/polyfill.min.js"></script>
+  <script src="//cdn.jsdelivr.net/npm/unfetch@5.0.0/dist/unfetch.umd.js"></script>
+  <script src="//cdn.jsdelivr.net/npm/react@18.2.0/umd/react.production.min.js"></script>
+  <script src="//cdn.jsdelivr.net/npm/react-dom@18.2.0/umd/react-dom.production.min.js"></script>
   <script src="//cdn.jsdelivr.net/npm/graphiql@{{graphiql_version}}/graphiql.min.js"></script>
-  <script src="//cdn.jsdelivr.net/npm/subscriptions-transport-ws@0.9.16/browser/client.js"></script>
-  <script src="//cdn.jsdelivr.net/npm/graphiql-subscriptions-fetcher@0.0.2/browser/client.js"></script>
+  <script src="//cdn.jsdelivr.net/npm/graphql-ws@5.11.2/umd/graphql-ws.min.js"></script>
 </head>
 <body>
   <div id="graphiql">Loading...</div>
   <script>
     // Collect the URL parameters
     var parameters = {};
     window.location.search.substr(1).split('&').forEach(function (entry) {
@@ -71,43 +76,24 @@
     };
     var otherParams = {};
     for (var k in parameters) {
       if (parameters.hasOwnProperty(k) && graphqlParamNames[k] !== true) {
         otherParams[k] = parameters[k];
       }
     }
-    // Configure the subscription client
-    let subscriptionsFetcher = null;
-    if ('{{subscription_url}}') {
-      let subscriptionsClient = new SubscriptionsTransportWs.SubscriptionClient(
-        '{{ subscription_url }}',
-        { reconnect: true }
-      );
-      subscriptionsFetcher = GraphiQLSubscriptionsFetcher.graphQLFetcher(
-        subscriptionsClient,
-        graphQLFetcher
-      );
-    }
     var fetchURL = locationQuery(otherParams);
-    // Defines a GraphQL fetcher using the fetch API.
-    function graphQLFetcher(graphQLParams, opts) {
-      return fetch(fetchURL, {
-        method: 'post',
-        headers: Object.assign(
-          {
-            'Accept': 'application/json',
-            'Content-Type': 'application/json'
-          },
-          opts && opts.headers,
-        ),
-        body: JSON.stringify(graphQLParams),
-        credentials: 'include',
-      }).then(function (response) {
-        return response.json();
+    // Defines a GraphQL fetcher.
+    var graphQLFetcher;
+    if ('{{subscription_url}}') {
+      graphQLFetcher = GraphiQL.createFetcher({
+        url: fetchURL,
+        subscription_url: '{{subscription_url}}'
       });
+    } else {
+      graphQLFetcher = GraphiQL.createFetcher({ url: fetchURL });
     }
     // When the query and variables string is edited, update the URL bar so
     // that it can be easily shared.
     function onEditQuery(newQuery) {
       parameters.query = newQuery;
       updateURL();
     }
@@ -125,26 +111,26 @@
     }
     function updateURL() {
       history.replaceState(null, null, locationQuery(parameters));
     }
     // Render <GraphiQL /> into the body.
     ReactDOM.render(
       React.createElement(GraphiQL, {
-        fetcher: subscriptionsFetcher || graphQLFetcher,
+        fetcher: graphQLFetcher,
         onEditQuery: onEditQuery,
         onEditVariables: onEditVariables,
         onEditHeaders: onEditHeaders,
         onEditOperationName: onEditOperationName,
         query: {{query|tojson}},
         response: {{result|tojson}},
         variables: {{variables|tojson}},
         headers: {{headers|tojson}},
         operationName: {{operation_name|tojson}},
         defaultQuery: {{default_query|tojson}},
-        headerEditorEnabled: {{header_editor_enabled|tojson}},
+        isHeadersEditorEnabled: {{header_editor_enabled|tojson}},
         shouldPersistHeaders: {{should_persist_headers|tojson}}
       }),
       document.getElementById('graphiql')
     );
   </script>
 </body>
 </html>"""
@@ -212,32 +198,20 @@
     """
 
     default_query: Optional[str]
     header_editor_enabled: Optional[bool]
     should_persist_headers: Optional[bool]
 
 
-def escape_js_value(value: Any) -> Any:
-    quotation = False
-    if value.startswith('"') and value.endswith('"'):
-        quotation = True
-        value = value[1 : len(value) - 1]
-
-    value = value.replace("\\\\n", "\\\\\\n").replace("\\n", "\\\\n")
-    if quotation:
-        value = '"' + value.replace('\\\\"', '"').replace('"', '\\"') + '"'
-
-    return value
-
-
 def process_var(template: str, name: str, value: Any, jsonify=False) -> str:
-    pattern = r"{{\s*" + name + r"(\s*|[^}]+)*\s*}}"
+    pattern = r"{{\s*" + name.replace("\\", r"\\") + r"(\s*|[^}]+)*\s*}}"
     if jsonify and value not in ["null", "undefined"]:
         value = json.dumps(value)
-        value = escape_js_value(value)
+
+    value = value.replace("\\", r"\\")
 
     return re.sub(pattern, value, template)
 
 
 def simple_renderer(template: str, **values: Dict[str, Any]) -> str:
     replace = [
         "graphiql_version",
@@ -292,39 +266,46 @@
         and options.get("header_editor_enabled")
         or "true",
         "should_persist_headers": options
         and options.get("should_persist_headers")
         or "false",
     }
 
+    if template_vars["result"] in ("null"):
+        template_vars["result"] = None
+
     return graphiql_template, template_vars
 
 
 async def render_graphiql_async(
     data: GraphiQLData,
     config: GraphiQLConfig,
     options: Optional[GraphiQLOptions] = None,
 ) -> str:
     graphiql_template, template_vars = _render_graphiql(data, config, options)
-    jinja_env: Optional[Environment] = config.get("jinja_env")
+    jinja_env = config.get("jinja_env")
 
     if jinja_env:
-        # This method returns a Template. See https://jinja.palletsprojects.com/en/2.11.x/api/#jinja2.Template
         template = jinja_env.from_string(graphiql_template)
-        if jinja_env.is_async:  # type: ignore
+        if jinja_env.is_async:
             source = await template.render_async(**template_vars)
         else:
             source = template.render(**template_vars)
     else:
         source = simple_renderer(graphiql_template, **template_vars)
     return source
 
 
 def render_graphiql_sync(
     data: GraphiQLData,
     config: GraphiQLConfig,
     options: Optional[GraphiQLOptions] = None,
 ) -> str:
     graphiql_template, template_vars = _render_graphiql(data, config, options)
+    jinja_env = config.get("jinja_env")
 
-    source = simple_renderer(graphiql_template, **template_vars)
+    if jinja_env:
+        template = jinja_env.from_string(graphiql_template)
+        source = template.render(**template_vars)
+    else:
+        source = simple_renderer(graphiql_template, **template_vars)
     return source
```

### Comparing `graphql-server-3.0.0b5/graphql_server/sanic/graphqlview.py` & `graphql-server-3.0.0b6/graphql_server/sanic/graphqlview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,51 @@
+import asyncio
 import copy
 from cgi import parse_header
 from collections.abc import MutableMapping
 from functools import partial
 from typing import List
 
-from graphql import ExecutionResult, GraphQLError, specified_rules
+from graphql import GraphQLError, specified_rules
+from graphql.pyutils import is_awaitable
 from graphql.type.schema import GraphQLSchema
 from sanic.response import HTTPResponse, html
 from sanic.views import HTTPMethodView
 
 from graphql_server import (
     GraphQLParams,
     HttpQueryError,
+    _check_jinja,
     encode_execution_results,
     format_error_default,
     json_encode,
     load_json_body,
     run_http_query,
 )
 from graphql_server.render_graphiql import (
     GraphiQLConfig,
     GraphiQLData,
     GraphiQLOptions,
     render_graphiql_async,
 )
+from graphql_server.utils import wrap_in_async
 
 
 class GraphQLView(HTTPMethodView):
     schema = None
     root_value = None
     context = None
     pretty = False
     graphiql = False
     graphiql_version = None
     graphiql_template = None
     graphiql_html_title = None
     middleware = None
     validation_rules = None
+    execution_context_class = None
     batch = False
     jinja_env = None
     max_age = 86400
     enable_async = False
     subscriptions = None
     headers = None
     default_query = None
@@ -60,36 +65,42 @@
 
         if not isinstance(self.schema, GraphQLSchema):
             # maybe the GraphQL schema is wrapped in a Graphene schema
             self.schema = getattr(self.schema, "graphql_schema", None)
             if not isinstance(self.schema, GraphQLSchema):
                 raise TypeError("A Schema is required to be provided to GraphQLView.")
 
+        if self.jinja_env is not None:
+            _check_jinja(self.jinja_env)
+
     def get_root_value(self):
         return self.root_value
 
     def get_context(self, request):
         context = (
             copy.copy(self.context)
-            if self.context and isinstance(self.context, MutableMapping)
+            if self.context is not None and isinstance(self.context, MutableMapping)
             else {}
         )
         if isinstance(context, MutableMapping) and "request" not in context:
             context.update({"request": request})
         return context
 
     def get_middleware(self):
         return self.middleware
 
     def get_validation_rules(self):
         if self.validation_rules is None:
             return specified_rules
         return self.validation_rules
 
-    async def dispatch_request(self, request, *args, **kwargs):
+    def get_execution_context_class(self):
+        return self.execution_context_class
+
+    async def __handle_request(self, request, *args, **kwargs):
         try:
             request_method = request.method.lower()
             data = self.parse_body(request)
 
             show_graphiql = request_method == "get" and self.should_display_graphiql(
                 request
             )
@@ -108,22 +119,25 @@
                     catch=catch,
                     # Execute options
                     run_sync=not self.enable_async,
                     root_value=self.get_root_value(),
                     context_value=self.get_context(request),
                     middleware=self.get_middleware(),
                     validation_rules=self.get_validation_rules(),
+                    execution_context_class=self.get_execution_context_class(),
                 )
                 exec_res = (
-                    [
-                        ex
-                        if ex is None or isinstance(ex, ExecutionResult)
-                        else await ex
-                        for ex in execution_results
-                    ]
+                    await asyncio.gather(
+                        *(
+                            ex
+                            if ex is not None and is_awaitable(ex)
+                            else wrap_in_async(lambda: ex)()
+                            for ex in execution_results
+                        )
+                    )
                     if self.enable_async
                     else execution_results
                 )
                 result, status_code = encode_execution_results(
                     exec_res,
                     is_batch=isinstance(data, list),
                     format_error=self.format_error,
@@ -169,14 +183,16 @@
             return HTTPResponse(
                 self.encode(dict(errors=[self.format_error(parsed_error)])),
                 status=e.status_code,
                 headers=e.headers,
                 content_type="application/json",
             )
 
+    get = post = put = head = options = patch = delete = __handle_request
+
     # noinspection PyBroadException
     def parse_body(self, request):
         content_type = self.get_mime_type(request)
         if content_type == "application/graphql":
             return {"query": request.body.decode("utf8")}
 
         elif content_type == "application/json":
```

### Comparing `graphql-server-3.0.0b5/graphql_server/version.py` & `graphql-server-3.0.0b6/graphql_server/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import NamedTuple
 
 __all__ = ["version", "version_info"]
 
 
-version = "3.0.0b5"
+version = "3.0.0b6"
 
 _re_version = re.compile(r"(\d+)\.(\d+)\.(\d+)(\D*)(\d*)")
 
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
```

### Comparing `graphql-server-3.0.0b5/graphql_server/webob/graphqlview.py` & `graphql-server-3.0.0b6/graphql_server/webob/graphqlview.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from graphql.error import GraphQLError
 from graphql.type.schema import GraphQLSchema
 from webob import Response
 
 from graphql_server import (
     GraphQLParams,
     HttpQueryError,
+    _check_jinja,
     encode_execution_results,
     format_error_default,
     json_encode,
     load_json_body,
     run_http_query,
 )
 from graphql_server.render_graphiql import (
@@ -23,25 +24,26 @@
     GraphiQLOptions,
     render_graphiql_sync,
 )
 
 
 class GraphQLView:
     schema = None
-    request = None
     root_value = None
     context = None
     pretty = False
     graphiql = False
     graphiql_version = None
     graphiql_template = None
     graphiql_html_title = None
     middleware = None
     validation_rules = None
+    execution_context_class = None
     batch = False
+    jinja_env = None
     enable_async = False
     subscriptions = None
     headers = None
     default_query = None
     header_editor_enabled = None
     should_persist_headers = None
     charset = "UTF-8"
@@ -57,35 +59,41 @@
 
         if not isinstance(self.schema, GraphQLSchema):
             # maybe the GraphQL schema is wrapped in a Graphene schema
             self.schema = getattr(self.schema, "graphql_schema", None)
             if not isinstance(self.schema, GraphQLSchema):
                 raise TypeError("A Schema is required to be provided to GraphQLView.")
 
+        if self.jinja_env is not None:
+            _check_jinja(self.jinja_env)
+
     def get_root_value(self):
         return self.root_value
 
     def get_context(self, request):
         context = (
             copy.copy(self.context)
-            if self.context and isinstance(self.context, MutableMapping)
+            if self.context is not None and isinstance(self.context, MutableMapping)
             else {}
         )
         if isinstance(context, MutableMapping) and "request" not in context:
             context.update({"request": request})
         return context
 
     def get_middleware(self):
         return self.middleware
 
     def get_validation_rules(self):
         if self.validation_rules is None:
             return specified_rules
         return self.validation_rules
 
+    def get_execution_context_class(self):
+        return self.execution_context_class
+
     def dispatch_request(self, request):
         try:
             request_method = request.method.lower()
             data = self.parse_body(request)
 
             show_graphiql = request_method == "get" and self.should_display_graphiql(
                 request
@@ -104,14 +112,15 @@
                 catch=catch,
                 # Execute options
                 run_sync=not self.enable_async,
                 root_value=self.get_root_value(),
                 context_value=self.get_context(request),
                 middleware=self.get_middleware(),
                 validation_rules=self.get_validation_rules(),
+                execution_context_class=self.get_execution_context_class(),
             )
             result, status_code = encode_execution_results(
                 execution_results,
                 is_batch=isinstance(data, list),
                 format_error=self.format_error,
                 encode=partial(self.encode, pretty=pretty),  # noqa
             )
@@ -125,15 +134,15 @@
                     subscription_url=self.subscriptions,
                     headers=self.headers,
                 )
                 graphiql_config = GraphiQLConfig(
                     graphiql_version=self.graphiql_version,
                     graphiql_template=self.graphiql_template,
                     graphiql_html_title=self.graphiql_html_title,
-                    jinja_env=None,
+                    jinja_env=self.jinja_env,
                 )
                 graphiql_options = GraphiQLOptions(
                     default_query=self.default_query,
                     header_editor_enabled=self.header_editor_enabled,
                     should_persist_headers=self.should_persist_headers,
                 )
                 return Response(
@@ -183,12 +192,13 @@
 
         return {}
 
     def should_display_graphiql(self, request):
         if not self.graphiql or "raw" in request.params:
             return False
 
-        return self.request_wants_html()
+        return self.request_wants_html(request)
 
-    def request_wants_html(self):
-        best = self.request.accept.best_match(["application/json", "text/html"])
+    @staticmethod
+    def request_wants_html(request):
+        best = request.accept.best_match(["application/json", "text/html"])
         return best == "text/html"
```

### Comparing `graphql-server-3.0.0b5/graphql_server.egg-info/PKG-INFO` & `graphql-server-3.0.0b6/graphql_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: graphql-server
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: GraphQL Server tools for powering your server
 Home-page: https://github.com/graphql-python/graphql-server
+Download-URL: https://github.com/graphql-python/graphql-server/releases
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
-Download-URL: https://github.com/graphql-python/graphql-server/releases
 Keywords: api graphql protocol rest
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -79,9 +79,7 @@
 blueprint to build your own integration or GraphQL server implementations.
 
 Please let us know when you have built something new, so we can list it here.
 
 ## Contributing
 
 See [CONTRIBUTING.md](https://github.com/graphql-python/graphql-server/blob/master/CONTRIBUTING.md)
-
-
```

### Comparing `graphql-server-3.0.0b5/graphql_server.egg-info/SOURCES.txt` & `graphql-server-3.0.0b6/graphql_server.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs/flask.md
 docs/sanic.md
 docs/webob.md
 docs/_static/graphql-server-logo.svg
 graphql_server/__init__.py
 graphql_server/error.py
 graphql_server/render_graphiql.py
+graphql_server/utils.py
 graphql_server/version.py
 graphql_server.egg-info/PKG-INFO
 graphql_server.egg-info/SOURCES.txt
 graphql_server.egg-info/dependency_links.txt
 graphql_server.egg-info/not-zip-safe
 graphql_server.egg-info/requires.txt
 graphql_server.egg-info/top_level.txt
@@ -37,30 +38,35 @@
 tests/test_error.py
 tests/test_helpers.py
 tests/test_query.py
 tests/test_version.py
 tests/utils.py
 tests/aiohttp/__init__.py
 tests/aiohttp/app.py
+tests/aiohttp/conftest.py
 tests/aiohttp/schema.py
 tests/aiohttp/test_graphiqlview.py
 tests/aiohttp/test_graphqlview.py
 tests/flask/__init__.py
 tests/flask/app.py
+tests/flask/conftest.py
 tests/flask/schema.py
 tests/flask/test_graphiqlview.py
 tests/flask/test_graphqlview.py
 tests/quart/__init__.py
 tests/quart/app.py
+tests/quart/conftest.py
 tests/quart/schema.py
 tests/quart/test_graphiqlview.py
 tests/quart/test_graphqlview.py
 tests/sanic/__init__.py
 tests/sanic/app.py
+tests/sanic/conftest.py
 tests/sanic/schema.py
 tests/sanic/test_graphiqlview.py
 tests/sanic/test_graphqlview.py
 tests/webob/__init__.py
 tests/webob/app.py
+tests/webob/conftest.py
 tests/webob/schema.py
 tests/webob/test_graphiqlview.py
 tests/webob/test_graphqlview.py
```

### Comparing `graphql-server-3.0.0b5/graphql_server.egg-info/requires.txt` & `graphql-server-3.0.0b6/graphql_server.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,57 +3,57 @@
 
 [aiohttp]
 aiohttp<4,>=3.8
 
 [all]
 graphql-core<3.3,>=3.2
 typing-extensions<5,>=4
-flask<2,>=1
-sanic<21,>=20.3
+flask<3,>=1
+sanic<23,>=21.12
 webob<2,>=1.8.7
 aiohttp<4,>=3.8
-quart<0.15,>=0.6.15
+quart<1,>=0.15
 
 [dev]
 graphql-core<3.3,>=3.2
 typing-extensions<5,>=4
-flask<2,>=1
-sanic<21,>=20.3
+flask<3,>=1
+sanic<23,>=21.12
 webob<2,>=1.8.7
 aiohttp<4,>=3.8
-quart<0.15,>=0.6.15
-flake8<5,>=4
+quart<1,>=0.15
+flake8<6,>=5
 isort<6,>=5
-black>=19.10b0
-mypy<1,>=0.931
+black<22.13,>=22.12
+mypy<1,>=0.991
 check-manifest<1,>=0.47
-pytest<6.3,>=6.2
-pytest-asyncio<1,>=0.16
-pytest-cov<4,>=3
-aiohttp<4,>=3.8
-Jinja2<3,>=2.11
+pytest<8,>=7.2
+pytest-asyncio<1,>=0.20
+pytest-cov<5,>=4
+Jinja2<4,>=3.1
+sanic-testing<23,>=22.3
 
 [flask]
-flask<2,>=1
+flask<3,>=1
 
 [quart]
-quart<0.15,>=0.6.15
+quart<1,>=0.15
 
 [sanic]
-sanic<21,>=20.3
+sanic<23,>=21.12
 
 [test]
 graphql-core<3.3,>=3.2
 typing-extensions<5,>=4
-flask<2,>=1
-sanic<21,>=20.3
+flask<3,>=1
+sanic<23,>=21.12
 webob<2,>=1.8.7
 aiohttp<4,>=3.8
-quart<0.15,>=0.6.15
-pytest<6.3,>=6.2
-pytest-asyncio<1,>=0.16
-pytest-cov<4,>=3
-aiohttp<4,>=3.8
-Jinja2<3,>=2.11
+quart<1,>=0.15
+pytest<8,>=7.2
+pytest-asyncio<1,>=0.20
+pytest-cov<5,>=4
+Jinja2<4,>=3.1
+sanic-testing<23,>=22.3
 
 [webob]
 webob<2,>=1.8.7
```

### Comparing `graphql-server-3.0.0b5/setup.py` & `graphql-server-3.0.0b6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from re import search
-from setuptools import setup, find_packages
 
-install_requires = ["graphql-core>=3.2,<3.3", "typing-extensions>=4,<5"]
+from setuptools import find_packages, setup
+
+install_requires = [
+    "graphql-core>=3.2,<3.3",
+    "typing-extensions>=4,<5",
+]
 
 tests_requires = [
-    "pytest>=6.2,<6.3",
-    "pytest-asyncio>=0.16,<1",
-    "pytest-cov>=3,<4",
-    "aiohttp>=3.8,<4",
-    "Jinja2>=2.11,<3",
+    "pytest>=7.2,<8",
+    "pytest-asyncio>=0.20,<1",
+    "pytest-cov>=4,<5",
+    "Jinja2>=3.1,<4",
+    "sanic-testing>=22.3,<23",
 ]
 
 dev_requires = [
-    "flake8>=4,<5",
+    "flake8>=5,<6",
     "isort>=5,<6",
-    "black>=19.10b0",
-    "mypy>=0.931,<1",
+    "black>=22.12,<22.13",
+    "mypy>=0.991,<1",
     "check-manifest>=0.47,<1",
 ] + tests_requires
 
 install_flask_requires = [
-    "flask>=1,<2",
+    "flask>=1,<3",
 ]
 
 install_sanic_requires = [
-    "sanic>=20.3,<21",
+    "sanic>=21.12,<23",
 ]
 
 install_webob_requires = [
     "webob>=1.8.7,<2",
 ]
 
 install_aiohttp_requires = [
     "aiohttp>=3.8,<4",
 ]
 
-install_quart_requires = ["quart>=0.6.15,<0.15"]
+install_quart_requires = ["quart>=0.15,<1"]
 
 install_all_requires = (
     install_requires
     + install_flask_requires
     + install_sanic_requires
     + install_webob_requires
     + install_aiohttp_requires
```

### Comparing `graphql-server-3.0.0b5/tests/aiohttp/schema.py` & `graphql-server-3.0.0b6/tests/aiohttp/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
                 name="context",
                 fields={
                     "session": GraphQLField(GraphQLString),
                     "request": GraphQLField(
                         GraphQLNonNull(GraphQLString),
                         resolve=lambda obj, info: info.context["request"],
                     ),
+                    "property": GraphQLField(
+                        GraphQLString, resolve=lambda obj, info: info.context.property
+                    ),
                 },
             ),
             resolve=lambda obj, info: info.context,
         ),
         "test": GraphQLField(
             type_=GraphQLString,
             args={"who": GraphQLArgument(GraphQLString)},
```

### Comparing `graphql-server-3.0.0b5/tests/aiohttp/test_graphiqlview.py` & `graphql-server-3.0.0b6/tests/aiohttp/test_graphiqlview.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,92 @@
 import pytest
-from aiohttp.test_utils import TestClient, TestServer
 from jinja2 import Environment
 
-from tests.aiohttp.app import create_app, url_string
-from tests.aiohttp.schema import AsyncSchema, Schema, SyncSchema
-
-
-@pytest.fixture
-def app():
-    app = create_app()
-    return app
-
-
-@pytest.fixture
-async def client(app):
-    client = TestClient(TestServer(app))
-    await client.start_server()
-    yield client
-    await client.close()
-
-
-@pytest.fixture
-def view_kwargs():
-    return {
-        "schema": Schema,
-        "graphiql": True,
-    }
-
-
-@pytest.fixture
-def pretty_response():
-    return (
-        "{\n"
-        '  "data": {\n'
-        '    "test": "Hello World"\n'
-        "  }\n"
-        "}".replace('"', '\\"').replace("\n", "\\n")
-    )
+from .app import create_app, url_string
+from .schema import AsyncSchema, SyncSchema
 
 
 @pytest.mark.asyncio
-@pytest.mark.parametrize("app", [create_app(graphiql=True)])
+@pytest.mark.parametrize(
+    "app",
+    [
+        create_app(graphiql=True),
+        create_app(graphiql=True, jinja_env=Environment()),
+        create_app(graphiql=True, jinja_env=Environment(enable_async=True)),
+    ],
+)
 async def test_graphiql_is_enabled(app, client):
     response = await client.get(
-        url_string(query="{test}"), headers={"Accept": "text/html"}
-    )
-    assert response.status == 200
-
-
-@pytest.mark.asyncio
-@pytest.mark.parametrize("app", [create_app(graphiql=True)])
-async def test_graphiql_simple_renderer(app, client, pretty_response):
-    response = await client.get(
         url_string(query="{test}"),
         headers={"Accept": "text/html"},
     )
     assert response.status == 200
-    assert pretty_response in await response.text()
 
+    pretty_response = (
+        "{\n"
+        '  "data": {\n'
+        '    "test": "Hello World"\n'
+        "  }\n"
+        "}".replace('"', '\\"').replace("\n", "\\n")
+    )
 
-class TestJinjaEnv:
-    @pytest.mark.asyncio
-    @pytest.mark.parametrize(
-        "app", [create_app(graphiql=True, jinja_env=Environment(enable_async=True))]
-    )
-    async def test_graphiql_jinja_renderer_async(self, app, client, pretty_response):
-        response = await client.get(
-            url_string(query="{test}"),
-            headers={"Accept": "text/html"},
-        )
-        assert response.status == 200
-        assert pretty_response in await response.text()
+    assert pretty_response in await response.text()
 
 
 @pytest.mark.asyncio
 async def test_graphiql_html_is_not_accepted(client):
     response = await client.get(
         "/graphql",
         headers={"Accept": "application/json"},
     )
     assert response.status == 400
 
 
 @pytest.mark.asyncio
-@pytest.mark.parametrize("app", [create_app(graphiql=True)])
+@pytest.mark.parametrize(
+    "app",
+    [create_app(graphiql=True), create_app(graphiql=True, jinja_env=Environment())],
+)
 async def test_graphiql_get_mutation(app, client):
     response = await client.get(
         url_string(query="mutation TestMutation { writeTest { test } }"),
         headers={"Accept": "text/html"},
     )
     assert response.status == 200
     assert "response: null" in await response.text()
 
 
 @pytest.mark.asyncio
-@pytest.mark.parametrize("app", [create_app(graphiql=True)])
+@pytest.mark.parametrize(
+    "app",
+    [create_app(graphiql=True), create_app(graphiql=True, jinja_env=Environment())],
+)
 async def test_graphiql_get_subscriptions(app, client):
     response = await client.get(
         url_string(
             query="subscription TestSubscriptions { subscriptionsTest { test } }"
         ),
         headers={"Accept": "text/html"},
     )
     assert response.status == 200
     assert "response: null" in await response.text()
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "app", [create_app(schema=AsyncSchema, enable_async=True, graphiql=True)]
+    "app",
+    [
+        create_app(schema=AsyncSchema, enable_async=True, graphiql=True),
+        create_app(
+            schema=AsyncSchema,
+            enable_async=True,
+            graphiql=True,
+            jinja_env=Environment(),
+        ),
+    ],
 )
 async def test_graphiql_enabled_async_schema(app, client):
     response = await client.get(
         url_string(query="{a,b,c}"),
         headers={"Accept": "text/html"},
     )
 
@@ -131,15 +105,21 @@
     )
     assert response.status == 200
     assert expected_response in await response.text()
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "app", [create_app(schema=SyncSchema, enable_async=True, graphiql=True)]
+    "app",
+    [
+        create_app(schema=SyncSchema, enable_async=True, graphiql=True),
+        create_app(
+            schema=SyncSchema, enable_async=True, graphiql=True, jinja_env=Environment()
+        ),
+    ],
 )
 async def test_graphiql_enabled_sync_schema(app, client):
     response = await client.get(
         url_string(query="{a,b}"),
         headers={"Accept": "text/html"},
     )
```

### Comparing `graphql-server-3.0.0b5/tests/aiohttp/test_graphqlview.py` & `graphql-server-3.0.0b6/tests/aiohttp/test_graphqlview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 import json
 from urllib.parse import urlencode
 
 import pytest
 from aiohttp import FormData
-from aiohttp.test_utils import TestClient, TestServer
 
+from ..utils import RepeatExecutionContext
 from .app import create_app, url_string
 from .schema import AsyncSchema
 
 
-@pytest.fixture
-def app():
-    app = create_app()
-    return app
-
-
-@pytest.fixture
-async def client(app):
-    client = TestClient(TestServer(app))
-    await client.start_server()
-    yield client
-    await client.close()
-
-
 @pytest.mark.asyncio
 async def test_allows_get_with_query_param(client):
     response = await client.get(url_string(query="{test}"))
 
     assert response.status == 200
     assert await response.json() == {"data": {"test": "Hello World"}}
 
@@ -549,14 +535,32 @@
     assert "data" in _json
     assert "session" in _json["data"]["context"]
     assert "request" in _json["data"]["context"]
     assert "CUSTOM CONTEXT" not in _json["data"]["context"]["request"]
     assert "Request" in _json["data"]["context"]["request"]
 
 
+class CustomContext(dict):
+    property = "A custom property"
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("app", [create_app(context=CustomContext())])
+async def test_allow_empty_custom_context(app, client):
+    response = await client.get(url_string(query="{context { property request }}"))
+
+    _json = await response.json()
+    assert response.status == 200
+    assert "data" in _json
+    assert "request" in _json["data"]["context"]
+    assert "property" in _json["data"]["context"]
+    assert "A custom property" == _json["data"]["context"]["property"]
+    assert "Request" in _json["data"]["context"]["request"]
+
+
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(context={"request": "test"})])
 async def test_request_not_replaced(app, client):
     response = await client.get(url_string(query="{context { request }}"))
 
     _json = await response.json()
     assert response.status == 200
@@ -677,7 +681,22 @@
 async def test_preflight_incorrect_request(client):
     response = await client.options(
         "/graphql",
         headers={"Access-Control-Request-Method": "OPTIONS"},
     )
 
     assert response.status == 400
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "app", [create_app(execution_context_class=RepeatExecutionContext)]
+)
+async def test_custom_execution_context_class(client):
+    response = await client.post(
+        "/graphql",
+        data=json.dumps(dict(query="{test}")),
+        headers={"content-type": "application/json"},
+    )
+
+    assert response.status == 200
+    assert await response.json() == {"data": {"test": "Hello WorldHello World"}}
```

### Comparing `graphql-server-3.0.0b5/tests/flask/schema.py` & `graphql-server-3.0.0b6/tests/flask/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,17 @@
                 name="context",
                 fields={
                     "session": GraphQLField(GraphQLString),
                     "request": GraphQLField(
                         GraphQLNonNull(GraphQLString),
                         resolve=lambda obj, info: info.context["request"],
                     ),
+                    "property": GraphQLField(
+                        GraphQLString, resolve=lambda obj, info: info.context.property
+                    ),
                 },
             ),
             resolve=lambda obj, info: info.context,
         ),
         "test": GraphQLField(
             type_=GraphQLString,
             args={"who": GraphQLArgument(GraphQLString)},
```

### Comparing `graphql-server-3.0.0b5/tests/flask/test_graphqlview.py` & `graphql-server-3.0.0b6/tests/flask/test_graphqlview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,23 @@
 import json
 from io import StringIO
 from urllib.parse import urlencode
 
 import pytest
 from flask import url_for
 
+from ..utils import RepeatExecutionContext
 from .app import create_app
 
 
-@pytest.fixture
-def app():
-    # import app factory pattern
-    app = create_app()
-
-    # pushes an application context manually
-    ctx = app.app_context()
-    ctx.push()
-    return app
-
-
-@pytest.fixture
-def client(app):
-    return app.test_client()
-
-
 def url_string(app, **url_params):
     with app.test_request_context():
-        string = url_for("graphql")
-
-    if url_params:
-        string += "?" + urlencode(url_params)
+        url = url_for("graphql")
 
-    return string
+    return f"{url}?{urlencode(url_params)}" if url_params else url
 
 
 def response_json(response):
     return json.loads(response.data.decode())
 
 
 def json_dump_kwarg(**kwargs):
@@ -513,14 +495,31 @@
     assert "data" in res
     assert "session" in res["data"]["context"]
     assert "request" in res["data"]["context"]
     assert "CUSTOM CONTEXT" not in res["data"]["context"]["request"]
     assert "Request" in res["data"]["context"]["request"]
 
 
+class CustomContext(dict):
+    property = "A custom property"
+
+
+@pytest.mark.parametrize("app", [create_app(context=CustomContext())])
+def test_allow_empty_custom_context(app, client):
+    response = client.get(url_string(app, query="{context { property request }}"))
+
+    assert response.status_code == 200
+    res = response_json(response)
+    assert "data" in res
+    assert "request" in res["data"]["context"]
+    assert "property" in res["data"]["context"]
+    assert "A custom property" == res["data"]["context"]["property"]
+    assert "Request" in res["data"]["context"]["request"]
+
+
 def test_post_multipart_data(app, client):
     query = "mutation TestMutation { writeTest { test } }"
     response = client.post(
         url_string(app),
         data={"query": query, "file": (StringIO(), "text1.txt")},
         content_type="multipart/form-data",
     )
@@ -574,7 +573,21 @@
         content_type="application/json",
     )
 
     assert response.status_code == 200
     assert response_json(response) == [
         {"data": {"test": "Hello World", "shared": "Hello Everyone"}}
     ]
+
+
+@pytest.mark.parametrize(
+    "app", [create_app(execution_context_class=RepeatExecutionContext)]
+)
+def test_custom_execution_context_class(app, client):
+    response = client.post(
+        url_string(app),
+        data=json_dump_kwarg(query="{test}"),
+        content_type="application/json",
+    )
+
+    assert response.status_code == 200
+    assert response_json(response) == {"data": {"test": "Hello WorldHello World"}}
```

### Comparing `graphql-server-3.0.0b5/tests/quart/schema.py` & `graphql-server-3.0.0b6/tests/webob/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,39 +8,43 @@
 from graphql.type.schema import GraphQLSchema
 
 
 def resolve_raises(*_):
     raise Exception("Throws!")
 
 
+# Sync schema
 QueryRootType = GraphQLObjectType(
     name="QueryRoot",
     fields={
         "thrower": GraphQLField(GraphQLNonNull(GraphQLString), resolve=resolve_raises),
         "request": GraphQLField(
             GraphQLNonNull(GraphQLString),
-            resolve=lambda obj, info: info.context["request"].args.get("q"),
+            resolve=lambda obj, info: info.context["request"].params.get("q"),
         ),
         "context": GraphQLField(
             GraphQLObjectType(
                 name="context",
                 fields={
                     "session": GraphQLField(GraphQLString),
                     "request": GraphQLField(
                         GraphQLNonNull(GraphQLString),
                         resolve=lambda obj, info: info.context["request"],
                     ),
+                    "property": GraphQLField(
+                        GraphQLString, resolve=lambda obj, info: info.context.property
+                    ),
                 },
             ),
             resolve=lambda obj, info: info.context,
         ),
         "test": GraphQLField(
             type_=GraphQLString,
             args={"who": GraphQLArgument(GraphQLString)},
-            resolve=lambda obj, info, who="World": "Hello %s" % who,
+            resolve=lambda obj, info, who=None: "Hello %s" % (who or "World"),
         ),
     },
 )
 
 MutationRootType = GraphQLObjectType(
     name="MutationRoot",
     fields={
```

### Comparing `graphql-server-3.0.0b5/tests/quart/test_graphiqlview.py` & `graphql-server-3.0.0b6/tests/quart/test_graphiqlview.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,87 @@
+from typing import Optional
+
 import pytest
+from jinja2 import Environment
 from quart import Quart, Response, url_for
-from quart.testing import QuartClient
+from quart.typing import TestClientProtocol
 from werkzeug.datastructures import Headers
 
 from .app import create_app
 
 
-@pytest.fixture
-def app() -> Quart:
-    # import app factory pattern
-    app = create_app(graphiql=True)
-
-    # pushes an application context manually
-    # ctx = app.app_context()
-    # await ctx.push()
-    return app
-
-
-@pytest.fixture
-def client(app: Quart) -> QuartClient:
-    return app.test_client()
-
-
 @pytest.mark.asyncio
 async def execute_client(
     app: Quart,
-    client: QuartClient,
+    client: TestClientProtocol,
     method: str = "GET",
-    headers: Headers = None,
+    headers: Optional[Headers] = None,
     **extra_params
 ) -> Response:
     test_request_context = app.test_request_context(path="/", method=method)
     async with test_request_context:
         string = url_for("graphql", **extra_params)
     return await client.get(string, headers=headers)
 
 
 @pytest.mark.asyncio
-async def test_graphiql_is_enabled(app: Quart, client: QuartClient):
+@pytest.mark.parametrize(
+    "app",
+    [create_app(graphiql=True), create_app(graphiql=True, jinja_env=Environment())],
+)
+async def test_graphiql_is_enabled(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app, client, headers=Headers({"Accept": "text/html"}), externals=False
     )
     assert response.status_code == 200
 
 
 @pytest.mark.asyncio
-async def test_graphiql_renders_pretty(app: Quart, client: QuartClient):
+@pytest.mark.parametrize(
+    "app",
+    [create_app(graphiql=True), create_app(graphiql=True, jinja_env=Environment())],
+)
+async def test_graphiql_renders_pretty(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app, client, headers=Headers({"Accept": "text/html"}), query="{test}"
     )
     assert response.status_code == 200
     pretty_response = (
         "{\n"
         '  "data": {\n'
         '    "test": "Hello World"\n'
         "  }\n"
         "}".replace('"', '\\"').replace("\n", "\\n")
     )
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert pretty_response in result
 
 
 @pytest.mark.asyncio
-async def test_graphiql_default_title(app: Quart, client: QuartClient):
+@pytest.mark.parametrize(
+    "app",
+    [create_app(graphiql=True), create_app(graphiql=True, jinja_env=Environment())],
+)
+async def test_graphiql_default_title(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app, client, headers=Headers({"Accept": "text/html"})
     )
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert "<title>GraphiQL</title>" in result
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "app", [create_app(graphiql=True, graphiql_html_title="Awesome")]
+    "app",
+    [
+        create_app(graphiql=True, graphiql_html_title="Awesome"),
+        create_app(
+            graphiql=True, graphiql_html_title="Awesome", jinja_env=Environment()
+        ),
+    ],
 )
-async def test_graphiql_custom_title(app: Quart, client: QuartClient):
+async def test_graphiql_custom_title(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app, client, headers=Headers({"Accept": "text/html"})
     )
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert "<title>Awesome</title>" in result
```

### Comparing `graphql-server-3.0.0b5/tests/quart/test_graphqlview.py` & `graphql-server-3.0.0b6/tests/quart/test_graphqlview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,28 @@
 import json
+from typing import Optional
 from urllib.parse import urlencode
 
 import pytest
 from quart import Quart, Response, url_for
-from quart.testing import QuartClient
+from quart.typing import TestClientProtocol
 from werkzeug.datastructures import Headers
 
+from ..utils import RepeatExecutionContext
 from .app import create_app
-
-
-@pytest.fixture
-def app() -> Quart:
-    # import app factory pattern
-    app = create_app(graphiql=True)
-
-    # pushes an application context manually
-    # ctx = app.app_context()
-    # await ctx.push()
-    return app
-
-
-@pytest.fixture
-def client(app: Quart) -> QuartClient:
-    return app.test_client()
+from .schema import AsyncSchema
 
 
 @pytest.mark.asyncio
 async def execute_client(
     app: Quart,
-    client: QuartClient,
+    client: TestClientProtocol,
     method: str = "GET",
-    data: str = None,
-    headers: Headers = None,
+    data: Optional[str] = None,
+    headers: Optional[Headers] = None,
     **url_params,
 ) -> Response:
     test_request_context = app.test_request_context(path="/", method=method)
     async with test_request_context:
         string = url_for("graphql")
 
     if url_params:
@@ -58,38 +45,38 @@
 
 
 def json_dump_kwarg_list(**kwargs):
     return json.dumps([kwargs])
 
 
 @pytest.mark.asyncio
-async def test_allows_get_with_query_param(app: Quart, client: QuartClient):
+async def test_allows_get_with_query_param(app: Quart, client: TestClientProtocol):
     response = await execute_client(app, client, query="{test}")
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello World"}}
 
 
 @pytest.mark.asyncio
-async def test_allows_get_with_variable_values(app: Quart, client: QuartClient):
+async def test_allows_get_with_variable_values(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         query="query helloWho($who: String){ test(who: $who) }",
         variables=json.dumps({"who": "Dolly"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
-async def test_allows_get_with_operation_name(app: Quart, client: QuartClient):
+async def test_allows_get_with_operation_name(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         query="""
             query helloYou { test(who: "You"), ...shared }
             query helloWorld { test(who: "World"), ...shared }
             query helloDolly { test(who: "Dolly"), ...shared }
@@ -97,28 +84,28 @@
               shared: test(who: "Everyone")
             }
         """,
         operationName="helloWorld",
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "data": {"test": "Hello World", "shared": "Hello Everyone"}
     }
 
 
 @pytest.mark.asyncio
-async def test_reports_validation_errors(app: Quart, client: QuartClient):
+async def test_reports_validation_errors(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app, client, query="{ test, unknownOne, unknownTwo }"
     )
 
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "message": "Cannot query field 'unknownOne' on type 'QueryRoot'.",
                 "locations": [{"line": 1, "column": 9}],
             },
             {
@@ -126,186 +113,194 @@
                 "locations": [{"line": 1, "column": 21}],
             },
         ]
     }
 
 
 @pytest.mark.asyncio
-async def test_errors_when_missing_operation_name(app: Quart, client: QuartClient):
+async def test_errors_when_missing_operation_name(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         query="""
             query TestQuery { test }
             mutation TestMutation { writeTest { test } }
         """,
     )
 
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "message": "Must provide operation name"
                 " if query contains multiple operations.",
             }
         ]
     }
 
 
 @pytest.mark.asyncio
-async def test_errors_when_sending_a_mutation_via_get(app: Quart, client: QuartClient):
+async def test_errors_when_sending_a_mutation_via_get(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         query="""
             mutation TestMutation { writeTest { test } }
         """,
     )
     assert response.status_code == 405
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "message": "Can only perform a mutation operation from a POST request.",
             }
         ]
     }
 
 
 @pytest.mark.asyncio
 async def test_errors_when_selecting_a_mutation_within_a_get(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         query="""
             query TestQuery { test }
             mutation TestMutation { writeTest { test } }
         """,
         operationName="TestMutation",
     )
 
     assert response.status_code == 405
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "message": "Can only perform a mutation operation from a POST request.",
             }
         ]
     }
 
 
 @pytest.mark.asyncio
-async def test_allows_mutation_to_exist_within_a_get(app: Quart, client: QuartClient):
+async def test_allows_mutation_to_exist_within_a_get(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         query="""
             query TestQuery { test }
             mutation TestMutation { writeTest { test } }
         """,
         operationName="TestQuery",
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello World"}}
 
 
 @pytest.mark.asyncio
-async def test_allows_post_with_json_encoding(app: Quart, client: QuartClient):
+async def test_allows_post_with_json_encoding(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg(query="{test}"),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello World"}}
 
 
 @pytest.mark.asyncio
-async def test_allows_sending_a_mutation_via_post(app: Quart, client: QuartClient):
+async def test_allows_sending_a_mutation_via_post(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg(query="mutation TestMutation { writeTest { test } }"),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"writeTest": {"test": "Hello World"}}}
 
 
 @pytest.mark.asyncio
-async def test_allows_post_with_url_encoding(app: Quart, client: QuartClient):
+async def test_allows_post_with_url_encoding(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=urlencode(dict(query="{test}")),
         headers=Headers({"Content-Type": "application/x-www-form-urlencoded"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello World"}}
 
 
 @pytest.mark.asyncio
 async def test_supports_post_json_query_with_string_variables(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg(
             query="query helloWho($who: String){ test(who: $who) }",
             variables=json.dumps({"who": "Dolly"}),
         ),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
 async def test_supports_post_json_query_with_json_variables(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg(
             query="query helloWho($who: String){ test(who: $who) }",
             variables={"who": "Dolly"},
         ),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
 async def test_supports_post_url_encoded_query_with_string_variables(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=urlencode(
             dict(
@@ -313,41 +308,41 @@
                 variables=json.dumps({"who": "Dolly"}),
             )
         ),
         headers=Headers({"Content-Type": "application/x-www-form-urlencoded"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
 async def test_supports_post_json_query_with_get_variable_values(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg(
             query="query helloWho($who: String){ test(who: $who) }",
         ),
         headers=Headers({"Content-Type": "application/json"}),
         variables=json.dumps({"who": "Dolly"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
 async def test_post_url_encoded_query_with_get_variable_values(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=urlencode(
             dict(
@@ -355,38 +350,38 @@
             )
         ),
         headers=Headers({"Content-Type": "application/x-www-form-urlencoded"}),
         variables=json.dumps({"who": "Dolly"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
 async def test_supports_post_raw_text_query_with_get_variable_values(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client=client,
         method="POST",
         data="query helloWho($who: String){ test(who: $who) }",
         headers=Headers({"Content-Type": "application/graphql"}),
         variables=json.dumps({"who": "Dolly"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"test": "Hello Dolly"}}
 
 
 @pytest.mark.asyncio
-async def test_allows_post_with_operation_name(app: Quart, client: QuartClient):
+async def test_allows_post_with_operation_name(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg(
             query="""
                 query helloYou { test(who: "You"), ...shared }
@@ -398,22 +393,24 @@
             """,
             operationName="helloWorld",
         ),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "data": {"test": "Hello World", "shared": "Hello Everyone"}
     }
 
 
 @pytest.mark.asyncio
-async def test_allows_post_with_get_operation_name(app: Quart, client: QuartClient):
+async def test_allows_post_with_get_operation_name(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         method="POST",
         data="""
             query helloYou { test(who: "You"), ...shared }
             query helloWorld { test(who: "World"), ...shared }
@@ -423,213 +420,244 @@
             }
         """,
         headers=Headers({"Content-Type": "application/graphql"}),
         operationName="helloWorld",
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "data": {"test": "Hello World", "shared": "Hello Everyone"}
     }
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(pretty=True)])
-async def test_supports_pretty_printing(app: Quart, client: QuartClient):
+async def test_supports_pretty_printing(app: Quart, client: TestClientProtocol):
     response = await execute_client(app, client, query="{test}")
 
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert result == ("{\n" '  "data": {\n' '    "test": "Hello World"\n' "  }\n" "}")
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(pretty=False)])
-async def test_not_pretty_by_default(app: Quart, client: QuartClient):
+async def test_not_pretty_by_default(app: Quart, client: TestClientProtocol):
     response = await execute_client(app, client, query="{test}")
 
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert result == '{"data":{"test":"Hello World"}}'
 
 
 @pytest.mark.asyncio
-async def test_supports_pretty_printing_by_request(app: Quart, client: QuartClient):
+async def test_supports_pretty_printing_by_request(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(app, client, query="{test}", pretty="1")
 
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert result == "{\n" '  "data": {\n' '    "test": "Hello World"\n' "  }\n" "}"
 
 
 @pytest.mark.asyncio
-async def test_handles_field_errors_caught_by_graphql(app: Quart, client: QuartClient):
+async def test_handles_field_errors_caught_by_graphql(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(app, client, query="{thrower}")
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "locations": [{"column": 2, "line": 1}],
                 "path": ["thrower"],
                 "message": "Throws!",
             }
         ],
         "data": None,
     }
 
 
 @pytest.mark.asyncio
-async def test_handles_syntax_errors_caught_by_graphql(app: Quart, client: QuartClient):
+async def test_handles_syntax_errors_caught_by_graphql(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(app, client, query="syntaxerror")
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "locations": [{"column": 1, "line": 1}],
                 "message": "Syntax Error: Unexpected Name 'syntaxerror'.",
             }
         ]
     }
 
 
 @pytest.mark.asyncio
 async def test_handles_errors_caused_by_a_lack_of_query(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(app, client)
 
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [{"message": "Must provide query string."}]
     }
 
 
 @pytest.mark.asyncio
-async def test_handles_batch_correctly_if_is_disabled(app: Quart, client: QuartClient):
+async def test_handles_batch_correctly_if_is_disabled(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         method="POST",
         data="[]",
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [
             {
                 "message": "Batch GraphQL requests are not enabled.",
             }
         ]
     }
 
 
 @pytest.mark.asyncio
-async def test_handles_incomplete_json_bodies(app: Quart, client: QuartClient):
+async def test_handles_incomplete_json_bodies(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         method="POST",
         data='{"query":',
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [{"message": "POST body sent invalid JSON."}]
     }
 
 
 @pytest.mark.asyncio
-async def test_handles_plain_post_text(app: Quart, client: QuartClient):
+async def test_handles_plain_post_text(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         method="POST",
         data="query helloWho($who: String){ test(who: $who) }",
         headers=Headers({"Content-Type": "text/plain"}),
         variables=json.dumps({"who": "Dolly"}),
     )
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [{"message": "Must provide query string."}]
     }
 
 
 @pytest.mark.asyncio
-async def test_handles_poorly_formed_variables(app: Quart, client: QuartClient):
+async def test_handles_poorly_formed_variables(app: Quart, client: TestClientProtocol):
     response = await execute_client(
         app,
         client,
         query="query helloWho($who: String){ test(who: $who) }",
         variables="who:You",
     )
     assert response.status_code == 400
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {
         "errors": [{"message": "Variables are invalid JSON."}]
     }
 
 
 @pytest.mark.asyncio
-async def test_handles_unsupported_http_methods(app: Quart, client: QuartClient):
+async def test_handles_unsupported_http_methods(app: Quart, client: TestClientProtocol):
     response = await execute_client(app, client, method="PUT", query="{test}")
     assert response.status_code == 405
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response.headers["Allow"] in ["GET, POST", "HEAD, GET, POST, OPTIONS"]
     assert response_json(result) == {
         "errors": [{"message": "GraphQL only supports GET and POST requests."}]
     }
 
 
 @pytest.mark.asyncio
-async def test_passes_request_into_request_context(app: Quart, client: QuartClient):
+async def test_passes_request_into_request_context(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(app, client, query="{request}", q="testing")
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == {"data": {"request": "testing"}}
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(context={"session": "CUSTOM CONTEXT"})])
-async def test_passes_custom_context_into_context(app: Quart, client: QuartClient):
+async def test_passes_custom_context_into_context(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(app, client, query="{context { session request }}")
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     res = response_json(result)
     assert "data" in res
     assert "session" in res["data"]["context"]
     assert "request" in res["data"]["context"]
     assert "CUSTOM CONTEXT" in res["data"]["context"]["session"]
     assert "Request" in res["data"]["context"]["request"]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(context="CUSTOM CONTEXT")])
-async def test_context_remapped_if_not_mapping(app: Quart, client: QuartClient):
+async def test_context_remapped_if_not_mapping(app: Quart, client: TestClientProtocol):
     response = await execute_client(app, client, query="{context { session request }}")
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     res = response_json(result)
     assert "data" in res
     assert "session" in res["data"]["context"]
     assert "request" in res["data"]["context"]
     assert "CUSTOM CONTEXT" not in res["data"]["context"]["request"]
     assert "Request" in res["data"]["context"]["request"]
 
 
+class CustomContext(dict):
+    property = "A custom property"
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("app", [create_app(context=CustomContext())])
+async def test_allow_empty_custom_context(app: Quart, client: TestClientProtocol):
+    response = await execute_client(app, client, query="{context { property request }}")
+
+    assert response.status_code == 200
+    result = await response.get_data(as_text=True)
+    res = response_json(result)
+    assert "data" in res
+    assert "request" in res["data"]["context"]
+    assert "property" in res["data"]["context"]
+    assert "A custom property" == res["data"]["context"]["property"]
+    assert "Request" in res["data"]["context"]["request"]
+
+
 # @pytest.mark.asyncio
-# async def test_post_multipart_data(app: Quart, client: QuartClient):
+# async def test_post_multipart_data(app: Quart, client: TestClientProtocol):
 #     query = "mutation TestMutation { writeTest { test } }"
 #     response = await execute_client(
 #         app,
 #         client,
 #         method='POST',
 #         data={"query": query, "file": (StringIO(), "text1.txt")},
 #         headers=Headers({"Content-Type": "multipart/form-data"})
@@ -640,52 +668,56 @@
 #     assert response_json(result) == {
 #         "data": {u"writeTest": {u"test": u"Hello World"}}
 #     }
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(batch=True)])
-async def test_batch_allows_post_with_json_encoding(app: Quart, client: QuartClient):
+async def test_batch_allows_post_with_json_encoding(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg_list(query="{test}"),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == [{"data": {"test": "Hello World"}}]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(batch=True)])
 async def test_batch_supports_post_json_query_with_json_variables(
-    app: Quart, client: QuartClient
+    app: Quart, client: TestClientProtocol
 ):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg_list(
             query="query helloWho($who: String){ test(who: $who) }",
             variables={"who": "Dolly"},
         ),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == [{"data": {"test": "Hello Dolly"}}]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("app", [create_app(batch=True)])
-async def test_batch_allows_post_with_operation_name(app: Quart, client: QuartClient):
+async def test_batch_allows_post_with_operation_name(
+    app: Quart, client: TestClientProtocol
+):
     response = await execute_client(
         app,
         client,
         method="POST",
         data=json_dump_kwarg_list(
             # id=1,
             query="""
@@ -698,11 +730,43 @@
             """,
             operationName="helloWorld",
         ),
         headers=Headers({"Content-Type": "application/json"}),
     )
 
     assert response.status_code == 200
-    result = await response.get_data(raw=False)
+    result = await response.get_data(as_text=True)
     assert response_json(result) == [
         {"data": {"test": "Hello World", "shared": "Hello Everyone"}}
     ]
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize("app", [create_app(schema=AsyncSchema, enable_async=True)])
+async def test_async_schema(app, client):
+    response = await execute_client(
+        app,
+        client,
+        query="{a,b,c}",
+    )
+
+    assert response.status_code == 200
+    result = await response.get_data(as_text=True)
+    assert response_json(result) == {"data": {"a": "hey", "b": "hey2", "c": "hey3"}}
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "app", [create_app(execution_context_class=RepeatExecutionContext)]
+)
+async def test_custom_execution_context_class(app: Quart, client: TestClientProtocol):
+    response = await execute_client(
+        app,
+        client,
+        method="POST",
+        data=json_dump_kwarg(query="{test}"),
+        headers=Headers({"Content-Type": "application/json"}),
+    )
+
+    assert response.status_code == 200
+    result = await response.get_data(as_text=True)
+    assert response_json(result) == {"data": {"test": "Hello WorldHello World"}}
```

### Comparing `graphql-server-3.0.0b5/tests/sanic/schema.py` & `graphql-server-3.0.0b6/tests/sanic/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,17 @@
                 name="context",
                 fields={
                     "session": GraphQLField(GraphQLString),
                     "request": GraphQLField(
                         GraphQLNonNull(GraphQLString),
                         resolve=lambda obj, info: info.context["request"],
                     ),
+                    "property": GraphQLField(
+                        GraphQLString, resolve=lambda obj, info: info.context.property
+                    ),
                 },
             ),
             resolve=lambda obj, info: info.context,
         ),
         "test": GraphQLField(
             type_=GraphQLString,
             args={"who": GraphQLArgument(GraphQLString)},
```

### Comparing `graphql-server-3.0.0b5/tests/sanic/test_graphqlview.py` & `graphql-server-3.0.0b6/tests/sanic/test_graphqlview.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from urllib.parse import urlencode
 
 import pytest
 
+from ..utils import RepeatExecutionContext
 from .app import create_app, url_string
 from .schema import AsyncSchema
 
 
 def response_json(response):
     return json.loads(response.body.decode())
 
@@ -15,38 +16,35 @@
     return json.dumps(kwargs)
 
 
 def json_dump_kwarg_list(**kwargs):
     return json.dumps([kwargs])
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_get_with_query_param(app):
-    _, response = app.client.get(uri=url_string(query="{test}"))
+    _, response = app.test_client.get(uri=url_string(query="{test}"))
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello World"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_get_with_variable_values(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="query helloWho($who: String){ test(who: $who) }",
             variables=json.dumps({"who": "Dolly"}),
         )
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_get_with_operation_name(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="""
         query helloYou { test(who: "You"), ...shared }
         query helloWorld { test(who: "World"), ...shared }
         query helloDolly { test(who: "Dolly"), ...shared }
         fragment shared on QueryRoot {
           shared: test(who: "Everyone")
@@ -58,17 +56,16 @@
 
     assert response.status == 200
     assert response_json(response) == {
         "data": {"test": "Hello World", "shared": "Hello Everyone"}
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_reports_validation_errors(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(query="{ test, unknownOne, unknownTwo }")
     )
 
     assert response.status == 400
     assert response_json(response) == {
         "errors": [
             {
@@ -79,17 +76,16 @@
                 "message": "Cannot query field 'unknownTwo' on type 'QueryRoot'.",
                 "locations": [{"line": 1, "column": 21}],
             },
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_errors_when_missing_operation_name(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="""
         query TestQuery { test }
         mutation TestMutation { writeTest { test } }
         """
         )
     )
@@ -101,17 +97,16 @@
                 "message": "Must provide operation name"
                 " if query contains multiple operations.",
             }
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_errors_when_sending_a_mutation_via_get(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="""
         mutation TestMutation { writeTest { test } }
         """
         )
     )
     assert response.status == 405
@@ -120,17 +115,16 @@
             {
                 "message": "Can only perform a mutation operation from a POST request.",
             }
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_errors_when_selecting_a_mutation_within_a_get(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="""
         query TestQuery { test }
         mutation TestMutation { writeTest { test } }
         """,
             operationName="TestMutation",
         )
@@ -142,164 +136,153 @@
             {
                 "message": "Can only perform a mutation operation from a POST request.",
             }
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_mutation_to_exist_within_a_get(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="""
         query TestQuery { test }
         mutation TestMutation { writeTest { test } }
         """,
             operationName="TestQuery",
         )
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello World"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_post_with_json_encoding(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg(query="{test}"),
+        content=json_dump_kwarg(query="{test}"),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello World"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_sending_a_mutation_via_post(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg(query="mutation TestMutation { writeTest { test } }"),
+        content=json_dump_kwarg(query="mutation TestMutation { writeTest { test } }"),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"writeTest": {"test": "Hello World"}}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_post_with_url_encoding(app):
     # Example of how sanic does send data using url enconding
     # can be found at their repo.
     # https://github.com/huge-success/sanic/blob/master/tests/test_requests.py#L927
     payload = "query={test}"
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=payload,
+        content=payload,
         headers={"content-type": "application/x-www-form-urlencoded"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello World"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_supports_post_json_query_with_string_variables(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg(
+        content=json_dump_kwarg(
             query="query helloWho($who: String){ test(who: $who) }",
             variables=json.dumps({"who": "Dolly"}),
         ),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_supports_post_json_query_with_json_variables(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg(
+        content=json_dump_kwarg(
             query="query helloWho($who: String){ test(who: $who) }",
             variables={"who": "Dolly"},
         ),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_supports_post_url_encoded_query_with_string_variables(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=urlencode(
+        content=urlencode(
             dict(
                 query="query helloWho($who: String){ test(who: $who) }",
                 variables=json.dumps({"who": "Dolly"}),
             )
         ),
         headers={"content-type": "application/x-www-form-urlencoded"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_supports_post_json_query_with_get_variable_values(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(variables=json.dumps({"who": "Dolly"})),
-        data=json_dump_kwarg(
+        content=json_dump_kwarg(
             query="query helloWho($who: String){ test(who: $who) }",
         ),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_post_url_encoded_query_with_get_variable_values(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(variables=json.dumps({"who": "Dolly"})),
-        data=urlencode(
+        content=urlencode(
             dict(
                 query="query helloWho($who: String){ test(who: $who) }",
             )
         ),
         headers={"content-type": "application/x-www-form-urlencoded"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_supports_post_raw_text_query_with_get_variable_values(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(variables=json.dumps({"who": "Dolly"})),
-        data="query helloWho($who: String){ test(who: $who) }",
+        content="query helloWho($who: String){ test(who: $who) }",
         headers={"content-type": "application/graphql"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"test": "Hello Dolly"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_post_with_operation_name(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg(
+        content=json_dump_kwarg(
             query="""
         query helloYou { test(who: "You"), ...shared }
         query helloWorld { test(who: "World"), ...shared }
         query helloDolly { test(who: "Dolly"), ...shared }
         fragment shared on QueryRoot {
           shared: test(who: "Everyone")
         }
@@ -311,19 +294,18 @@
 
     assert response.status == 200
     assert response_json(response) == {
         "data": {"test": "Hello World", "shared": "Hello Everyone"}
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_allows_post_with_get_operation_name(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(operationName="helloWorld"),
-        data="""
+        content="""
     query helloYou { test(who: "You"), ...shared }
     query helloWorld { test(who: "World"), ...shared }
     query helloDolly { test(who: "Dolly"), ...shared }
     fragment shared on QueryRoot {
       shared: test(who: "Everyone")
     }
     """,
@@ -334,180 +316,197 @@
     assert response_json(response) == {
         "data": {"test": "Hello World", "shared": "Hello Everyone"}
     }
 
 
 @pytest.mark.parametrize("app", [create_app(pretty=True)])
 def test_supports_pretty_printing(app):
-    _, response = app.client.get(uri=url_string(query="{test}"))
+    _, response = app.test_client.get(uri=url_string(query="{test}"))
 
     assert response.body.decode() == (
         "{\n" '  "data": {\n' '    "test": "Hello World"\n' "  }\n" "}"
     )
 
 
 @pytest.mark.parametrize("app", [create_app(pretty=False)])
 def test_not_pretty_by_default(app):
-    _, response = app.client.get(url_string(query="{test}"))
+    _, response = app.test_client.get(url_string(query="{test}"))
 
     assert response.body.decode() == '{"data":{"test":"Hello World"}}'
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_supports_pretty_printing_by_request(app):
-    _, response = app.client.get(uri=url_string(query="{test}", pretty="1"))
+    _, response = app.test_client.get(uri=url_string(query="{test}", pretty="1"))
 
     assert response.body.decode() == (
         "{\n" '  "data": {\n' '    "test": "Hello World"\n' "  }\n" "}"
     )
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_field_errors_caught_by_graphql(app):
-    _, response = app.client.get(uri=url_string(query="{thrower}"))
+    _, response = app.test_client.get(uri=url_string(query="{thrower}"))
     assert response.status == 200
     assert response_json(response) == {
         "data": None,
         "errors": [
             {
                 "locations": [{"column": 2, "line": 1}],
                 "message": "Throws!",
                 "path": ["thrower"],
             }
         ],
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_syntax_errors_caught_by_graphql(app):
-    _, response = app.client.get(uri=url_string(query="syntaxerror"))
+    _, response = app.test_client.get(uri=url_string(query="syntaxerror"))
     assert response.status == 400
     assert response_json(response) == {
         "errors": [
             {
                 "locations": [{"column": 1, "line": 1}],
                 "message": "Syntax Error: Unexpected Name 'syntaxerror'.",
             }
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_errors_caused_by_a_lack_of_query(app):
-    _, response = app.client.get(uri=url_string())
+    _, response = app.test_client.get(uri=url_string())
 
     assert response.status == 400
     assert response_json(response) == {
         "errors": [{"message": "Must provide query string."}]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_batch_correctly_if_is_disabled(app):
-    _, response = app.client.post(
-        uri=url_string(), data="[]", headers={"content-type": "application/json"}
+    _, response = app.test_client.post(
+        uri=url_string(), content="[]", headers={"content-type": "application/json"}
     )
 
     assert response.status == 400
     assert response_json(response) == {
         "errors": [
             {
                 "message": "Batch GraphQL requests are not enabled.",
             }
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_incomplete_json_bodies(app):
-    _, response = app.client.post(
-        uri=url_string(), data='{"query":', headers={"content-type": "application/json"}
+    _, response = app.test_client.post(
+        uri=url_string(),
+        content='{"query":',
+        headers={"content-type": "application/json"},
     )
 
     assert response.status == 400
     assert response_json(response) == {
         "errors": [{"message": "POST body sent invalid JSON."}]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_plain_post_text(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(variables=json.dumps({"who": "Dolly"})),
-        data="query helloWho($who: String){ test(who: $who) }",
+        content="query helloWho($who: String){ test(who: $who) }",
         headers={"content-type": "text/plain"},
     )
     assert response.status == 400
     assert response_json(response) == {
         "errors": [{"message": "Must provide query string."}]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_poorly_formed_variables(app):
-    _, response = app.client.get(
+    _, response = app.test_client.get(
         uri=url_string(
             query="query helloWho($who: String){ test(who: $who) }", variables="who:You"
         )
     )
     assert response.status == 400
     assert response_json(response) == {
         "errors": [{"message": "Variables are invalid JSON."}]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_handles_unsupported_http_methods(app):
-    _, response = app.client.put(uri=url_string(query="{test}"))
+    _, response = app.test_client.put(uri=url_string(query="{test}"))
     assert response.status == 405
-    assert response.headers["Allow"] in ["GET, POST", "HEAD, GET, POST, OPTIONS"]
+    allowed_methods = set(
+        method.strip() for method in response.headers["Allow"].split(",")
+    )
+    assert allowed_methods in [{"GET", "POST"}, {"HEAD", "GET", "POST", "OPTIONS"}]
     assert response_json(response) == {
         "errors": [
             {
                 "message": "GraphQL only supports GET and POST requests.",
             }
         ]
     }
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_passes_request_into_request_context(app):
-    _, response = app.client.get(uri=url_string(query="{request}", q="testing"))
+    _, response = app.test_client.get(uri=url_string(query="{request}", q="testing"))
 
     assert response.status == 200
     assert response_json(response) == {"data": {"request": "testing"}}
 
 
 @pytest.mark.parametrize("app", [create_app(context={"session": "CUSTOM CONTEXT"})])
 def test_passes_custom_context_into_context(app):
-    _, response = app.client.get(uri=url_string(query="{context { session request }}"))
+    _, response = app.test_client.get(
+        uri=url_string(query="{context { session request }}")
+    )
 
     assert response.status_code == 200
     res = response_json(response)
     assert "data" in res
     assert "session" in res["data"]["context"]
     assert "request" in res["data"]["context"]
     assert "CUSTOM CONTEXT" in res["data"]["context"]["session"]
     assert "Request" in res["data"]["context"]["request"]
 
 
+class CustomContext(dict):
+    property = "A custom property"
+
+
+@pytest.mark.parametrize("app", [create_app(context=CustomContext())])
+def test_allow_empty_custom_context(app):
+    _, response = app.test_client.get(
+        uri=url_string(query="{context { property request }}")
+    )
+
+    assert response.status_code == 200
+    res = response_json(response)
+    assert "data" in res
+    assert "request" in res["data"]["context"]
+    assert "property" in res["data"]["context"]
+    assert "A custom property" == res["data"]["context"]["property"]
+    assert "Request" in res["data"]["context"]["request"]
+
+
 @pytest.mark.parametrize("app", [create_app(context="CUSTOM CONTEXT")])
 def test_context_remapped_if_not_mapping(app):
-    _, response = app.client.get(uri=url_string(query="{context { session request }}"))
+    _, response = app.test_client.get(
+        uri=url_string(query="{context { session request }}")
+    )
 
     assert response.status_code == 200
     res = response_json(response)
     assert "data" in res
     assert "session" in res["data"]["context"]
     assert "request" in res["data"]["context"]
     assert "CUSTOM CONTEXT" not in res["data"]["context"]["request"]
     assert "Request" in res["data"]["context"]["request"]
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_post_multipart_data(app):
     query = "mutation TestMutation { writeTest { test } }"
 
     data = (
         "------sanicgraphql\r\n"
         + 'Content-Disposition: form-data; name="query"\r\n'
         + "\r\n"
@@ -517,57 +516,57 @@
         + "Content-Type: text/plain; charset=utf-8\r\n"
         + 'Content-Disposition: form-data; name="file"; filename="text1.txt"; filename*=utf-8\'\'text1.txt\r\n'
         + "\r\n"
         + "\r\n"
         + "------sanicgraphql--\r\n"
     )
 
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=data,
+        content=data,
         headers={"content-type": "multipart/form-data; boundary=----sanicgraphql"},
     )
 
     assert response.status == 200
     assert response_json(response) == {"data": {"writeTest": {"test": "Hello World"}}}
 
 
 @pytest.mark.parametrize("app", [create_app(batch=True)])
 def test_batch_allows_post_with_json_encoding(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg_list(id=1, query="{test}"),
+        content=json_dump_kwarg_list(id=1, query="{test}"),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == [{"data": {"test": "Hello World"}}]
 
 
 @pytest.mark.parametrize("app", [create_app(batch=True)])
 def test_batch_supports_post_json_query_with_json_variables(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg_list(
+        content=json_dump_kwarg_list(
             id=1,
             query="query helloWho($who: String){ test(who: $who) }",
             variables={"who": "Dolly"},
         ),
         headers={"content-type": "application/json"},
     )
 
     assert response.status == 200
     assert response_json(response) == [{"data": {"test": "Hello Dolly"}}]
 
 
 @pytest.mark.parametrize("app", [create_app(batch=True)])
 def test_batch_allows_post_with_operation_name(app):
-    _, response = app.client.post(
+    _, response = app.test_client.post(
         uri=url_string(),
-        data=json_dump_kwarg_list(
+        content=json_dump_kwarg_list(
             id=1,
             query="""
             query helloYou { test(who: "You"), ...shared }
             query helloWorld { test(who: "World"), ...shared }
             query helloDolly { test(who: "Dolly"), ...shared }
             fragment shared on QueryRoot {
               shared: test(who: "Everyone")
@@ -583,29 +582,41 @@
         {"data": {"test": "Hello World", "shared": "Hello Everyone"}}
     ]
 
 
 @pytest.mark.parametrize("app", [create_app(schema=AsyncSchema, enable_async=True)])
 def test_async_schema(app):
     query = "{a,b,c}"
-    _, response = app.client.get(uri=url_string(query=query))
+    _, response = app.test_client.get(uri=url_string(query=query))
 
     assert response.status == 200
     assert response_json(response) == {"data": {"a": "hey", "b": "hey2", "c": "hey3"}}
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_preflight_request(app):
-    _, response = app.client.options(
+    _, response = app.test_client.options(
         uri=url_string(), headers={"Access-Control-Request-Method": "POST"}
     )
 
     assert response.status == 200
 
 
-@pytest.mark.parametrize("app", [create_app()])
 def test_preflight_incorrect_request(app):
-    _, response = app.client.options(
+    _, response = app.test_client.options(
         uri=url_string(), headers={"Access-Control-Request-Method": "OPTIONS"}
     )
 
     assert response.status == 400
+
+
+@pytest.mark.parametrize(
+    "app", [create_app(execution_context_class=RepeatExecutionContext)]
+)
+def test_custom_execution_context_class(app):
+    _, response = app.test_client.post(
+        uri=url_string(),
+        content=json_dump_kwarg(query="{test}"),
+        headers={"content-type": "application/json"},
+    )
+
+    assert response.status == 200
+    assert response_json(response) == {"data": {"test": "Hello WorldHello World"}}
```

### Comparing `graphql-server-3.0.0b5/tests/schema.py` & `graphql-server-3.0.0b6/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/tests/test_asyncio.py` & `graphql-server-3.0.0b6/tests/test_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import asyncio
 
-from graphql.type.definition import (
-    GraphQLField,
-    GraphQLNonNull,
-    GraphQLObjectType,
-)
+from graphql.type.definition import GraphQLField, GraphQLNonNull, GraphQLObjectType
 from graphql.type.scalars import GraphQLString
 from graphql.type.schema import GraphQLSchema
 
 from graphql_server import GraphQLParams, run_http_query
 
 from .utils import as_dicts
 
@@ -45,27 +41,22 @@
 
 schema = GraphQLSchema(QueryRootType)
 
 
 def test_get_responses_using_asyncio_executor():
     query = "{fieldSync fieldAsync}"
 
-    loop = asyncio.get_event_loop()
-
     async def get_results():
         result_promises, params = run_http_query(
             schema, "get", {}, dict(query=query), run_sync=False
         )
         res = [await result for result in result_promises]
         return res, params
 
-    try:
-        results, params = loop.run_until_complete(get_results())
-    finally:
-        loop.close()
+    results, params = asyncio.run(get_results())
 
     expected_results = [
         {"data": {"fieldSync": "sync", "fieldAsync": "async"}, "errors": None}
     ]
 
     assert as_dicts(results) == expected_results
     assert params == [GraphQLParams(query=query, variables=None, operation_name=None)]
```

### Comparing `graphql-server-3.0.0b5/tests/test_error.py` & `graphql-server-3.0.0b6/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/tests/test_helpers.py` & `graphql-server-3.0.0b6/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/tests/test_query.py` & `graphql-server-3.0.0b6/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
     HttpQueryError,
     encode_execution_results,
     format_execution_result,
     json_encode,
     load_json_body,
     run_http_query,
 )
+from graphql_server.render_graphiql import (
+    GraphiQLConfig,
+    GraphiQLData,
+    render_graphiql_sync,
+)
 
 from .schema import invalid_schema, schema
 from .utils import as_dicts
 
 
 def test_request_params():
     assert issubclass(GraphQLParams, tuple)
@@ -649,7 +654,25 @@
             operationName="helloWorld",
         )
     ]
     data = load_json_body(json_encode(data))
     results, params = run_http_query(schema, "post", data, batch_enabled=True)
 
     assert results == [({"test": "Hello World", "shared": "Hello Everyone"}, None)]
+
+
+def test_graphiql_render_umlaut():
+    results, params = run_http_query(
+        schema,
+        "get",
+        data=dict(query="query helloWho($who: String){ test(who: $who) }"),
+        query_data=dict(variables='{"who": "Björn"}'),
+        catch=True,
+    )
+    result, status_code = encode_execution_results(results)
+
+    assert status_code == 200
+
+    graphiql_data = GraphiQLData(result=result, query=params[0].query)
+    source = render_graphiql_sync(data=graphiql_data, config=GraphiQLConfig())
+
+    assert "Hello Bj\\\\u00f6rn" in source
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `graphql-server-3.0.0b5/tests/test_version.py` & `graphql-server-3.0.0b6/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `graphql-server-3.0.0b5/tests/webob/app.py` & `graphql-server-3.0.0b6/tests/webob/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from urllib.parse import urlencode
 
 from webob import Request
 
 from graphql_server.webob import GraphQLView
-from tests.webob.schema import Schema
 
+from .schema import Schema
 
-def url_string(**url_params):
-    string = "/graphql"
 
-    if url_params:
-        string += "?" + urlencode(url_params)
-
-    return string
+def url_string(url="/graphql", **url_params):
+    return f"{url}?{urlencode(url_params)}" if url_params else url
 
 
 class Client(object):
     def __init__(self, **kwargs):
         self.schema = kwargs.pop("schema", None) or Schema
         self.settings = kwargs.pop("settings", None) or {}
```

### Comparing `graphql-server-3.0.0b5/tests/webob/schema.py` & `graphql-server-3.0.0b6/tests/quart/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import asyncio
+
 from graphql.type.definition import (
     GraphQLArgument,
     GraphQLField,
     GraphQLNonNull,
     GraphQLObjectType,
 )
 from graphql.type.scalars import GraphQLString
@@ -15,38 +17,86 @@
 # Sync schema
 QueryRootType = GraphQLObjectType(
     name="QueryRoot",
     fields={
         "thrower": GraphQLField(GraphQLNonNull(GraphQLString), resolve=resolve_raises),
         "request": GraphQLField(
             GraphQLNonNull(GraphQLString),
-            resolve=lambda obj, info: info.context["request"].params.get("q"),
+            resolve=lambda obj, info: info.context["request"].args.get("q"),
         ),
         "context": GraphQLField(
             GraphQLObjectType(
                 name="context",
                 fields={
                     "session": GraphQLField(GraphQLString),
                     "request": GraphQLField(
                         GraphQLNonNull(GraphQLString),
                         resolve=lambda obj, info: info.context["request"],
                     ),
+                    "property": GraphQLField(
+                        GraphQLString, resolve=lambda obj, info: info.context.property
+                    ),
                 },
             ),
             resolve=lambda obj, info: info.context,
         ),
         "test": GraphQLField(
             type_=GraphQLString,
             args={"who": GraphQLArgument(GraphQLString)},
-            resolve=lambda obj, info, who=None: "Hello %s" % (who or "World"),
+            resolve=lambda obj, info, who="World": f"Hello {who}",
         ),
     },
 )
 
 MutationRootType = GraphQLObjectType(
     name="MutationRoot",
     fields={
         "writeTest": GraphQLField(type_=QueryRootType, resolve=lambda *_: QueryRootType)
     },
 )
 
 Schema = GraphQLSchema(QueryRootType, MutationRootType)
+
+
+# Schema with async methods
+async def resolver_field_async_1(_obj, info):
+    await asyncio.sleep(0.001)
+    return "hey"
+
+
+async def resolver_field_async_2(_obj, info):
+    await asyncio.sleep(0.003)
+    return "hey2"
+
+
+def resolver_field_sync(_obj, info):
+    return "hey3"
+
+
+AsyncQueryType = GraphQLObjectType(
+    name="AsyncQueryType",
+    fields={
+        "a": GraphQLField(GraphQLString, resolve=resolver_field_async_1),
+        "b": GraphQLField(GraphQLString, resolve=resolver_field_async_2),
+        "c": GraphQLField(GraphQLString, resolve=resolver_field_sync),
+    },
+)
+
+
+def resolver_field_sync_1(_obj, info):
+    return "synced_one"
+
+
+def resolver_field_sync_2(_obj, info):
+    return "synced_two"
+
+
+SyncQueryType = GraphQLObjectType(
+    "SyncQueryType",
+    {
+        "a": GraphQLField(GraphQLString, resolve=resolver_field_sync_1),
+        "b": GraphQLField(GraphQLString, resolve=resolver_field_sync_2),
+    },
+)
+
+AsyncSchema = GraphQLSchema(AsyncQueryType)
+SyncSchema = GraphQLSchema(SyncQueryType)
```

### Comparing `graphql-server-3.0.0b5/tests/webob/test_graphqlview.py` & `graphql-server-3.0.0b6/tests/webob/test_graphqlview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 import json
 from urllib.parse import urlencode
 
 import pytest
 
-from .app import Client, url_string
-
-
-@pytest.fixture
-def settings():
-    return {}
-
-
-@pytest.fixture
-def client(settings):
-    return Client(settings=settings)
+from ..utils import RepeatExecutionContext
+from .app import url_string
 
 
 def response_json(response):
     return json.loads(response.body.decode())
 
 
 def json_dump_kwarg(**kwargs):
@@ -466,14 +457,31 @@
     assert "data" in res
     assert "session" in res["data"]["context"]
     assert "request" in res["data"]["context"]
     assert "CUSTOM CONTEXT" not in res["data"]["context"]["request"]
     assert "request" in res["data"]["context"]["request"]
 
 
+class CustomContext(dict):
+    property = "A custom property"
+
+
+@pytest.mark.parametrize("settings", [dict(context=CustomContext())])
+def test_allow_empty_custom_context(client, settings):
+    response = client.get(url_string(query="{context { property request }}"))
+
+    assert response.status_code == 200
+    res = response_json(response)
+    assert "data" in res
+    assert "request" in res["data"]["context"]
+    assert "property" in res["data"]["context"]
+    assert "A custom property" == res["data"]["context"]["property"]
+    assert "request" in res["data"]["context"]["request"]
+
+
 def test_post_multipart_data(client):
     query = "mutation TestMutation { writeTest { test } }"
     data = (
         "------webobgraphql\r\n"
         + 'Content-Disposition: form-data; name="query"\r\n'
         + "\r\n"
         + query
@@ -559,7 +567,21 @@
     assert response.status_code == 200
     assert response_json(response) == [
         {
             # 'id': 1,
             "data": {"test": "Hello World", "shared": "Hello Everyone"}
         }
     ]
+
+
+@pytest.mark.parametrize(
+    "settings", [dict(execution_context_class=RepeatExecutionContext)]
+)
+def test_custom_execution_context_class(client):
+    response = client.post(
+        url_string(),
+        data=json_dump_kwarg(query="{test}"),
+        content_type="application/json",
+    )
+
+    assert response.status_code == 200
+    assert response_json(response) == {"data": {"test": "Hello WorldHello World"}}
```

### Comparing `graphql-server-3.0.0b5/tox.ini` & `graphql-server-3.0.0b6/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 [tox]
 envlist =
     black,flake8,import-order,mypy,manifest,
-    py{36,37,38,39,310}
+    py{37,38,39,310,311}
 ; requires = tox-conda
 
 [gh-actions]
 python =
-    3.6: py36
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
+    3.11: py311
 
 [testenv]
 conda_channels = conda-forge
 passenv = *
 setenv =
     PYTHONPATH = {toxinidir}
 install_command = python -m pip install --ignore-installed {opts} {packages}
 deps = -e.[test]
 whitelist_externals =
     python
 commands =
     pip install -U setuptools
-    py{36,37,39}: pytest tests {posargs}
-    py{38}: pytest tests --cov-report=term-missing --cov=graphql_server {posargs}
+    py{37,38,39,311}: pytest tests {posargs}
+    py{310}: pytest tests --cov-report=term-missing --cov=graphql_server {posargs}
 
 [testenv:black]
-basepython = python3.9
+basepython = python3.10
 deps = -e.[dev]
 commands =
     black --check graphql_server tests
 
 [testenv:flake8]
-basepython = python3.9
+basepython = python3.10
 deps = -e.[dev]
 commands =
     flake8 setup.py graphql_server tests
 
 [testenv:import-order]
-basepython = python3.9
+basepython = python3.10
 deps = -e.[dev]
 commands =
     isort graphql_server/ tests/
 
 [testenv:mypy]
-basepython = python3.9
+basepython = python3.10
 deps = -e.[dev]
 commands =
     mypy graphql_server tests --ignore-missing-imports
 
 [testenv:manifest]
-basepython = python3.9
+basepython = python3.10
 deps = -e.[dev]
 commands =
     check-manifest -v
```

