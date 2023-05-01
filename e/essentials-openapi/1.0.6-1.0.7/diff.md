# Comparing `tmp/essentials-openapi-1.0.6.tar.gz` & `tmp/essentials_openapi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "essentials-openapi-1.0.6.tar", last modified: Sun Mar 19 07:01:30 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `essentials-openapi-1.0.6.tar` & `essentials_openapi-1.0.7.tar`

### file list

```diff
@@ -1,99 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.290602 essentials-openapi-1.0.6/essentials_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-19 07:01:30.000000 essentials-openapi-1.0.6/essentials_openapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.290602 essentials-openapi-1.0.6/openapidocs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.290602 essentials-openapi-1.0.6/openapidocs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/commands/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.290602 essentials-openapi-1.0.6/openapidocs/mk/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/texts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.290602 essentials-openapi-1.0.6/openapidocs/mk/v3/
--rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.294602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.294602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/components-parameters.html
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/components-responses.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/components-schemas.html
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/components-security-schemes.html
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/content-examples.html
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/external-docs.html
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/info.html
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/path-items.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/request-auth.html
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/request-body.html
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/request-parameters.html
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/request-responses.html
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/schema-repr.html
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/servers.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/tags.html
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/type.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.294602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.294602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-schemas.html
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/content-examples.html
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/external-docs.html
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/info.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/path-items.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-auth.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-body.html
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/servers.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/tags.html
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/type.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/partial/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/partial/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/openapidocs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/utils/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/utils/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/openapidocs/v3.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 07:01:30.298602 essentials-openapi-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_mk.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_mk_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_mk_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    44872 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-03-19 07:01:00.000000 essentials-openapi-1.0.6/tests/test_v3.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/common.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/logs.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/main.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/v2.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/v3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/commands/__init__.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/commands/docs.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/common.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/contents.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/md.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/utils/__init__.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/utils/source.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/openapidocs/utils/web.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/LICENSE
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/README.md
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 essentials_openapi-1.0.7/PKG-INFO
```

### Comparing `essentials-openapi-1.0.6/LICENSE` & `essentials_openapi-1.0.7/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Neoteroi
+Copyright (c) 2022 roberto.prevato@gmail.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `essentials-openapi-1.0.6/PKG-INFO` & `essentials_openapi-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: essentials-openapi
-Version: 1.0.6
-Summary: Classes to generate OpenAPI Documentation v3 and v2, in JSON and YAML
-Home-page: https://github.com/Neoteroi/essentials-openapi
-Author: RobertoPrevato
-Author-email: roberto.prevato@gmail.com
-License: MIT
-Keywords: openapi docs swagger api documentation v3 v2 json yaml Markdown
+Version: 1.0.7
+Summary: Classes to generate OpenAPI Documentation v3 and v2, in JSON and YAML.
+Project-URL: Homepage, https://github.com/Neoteroi/essentials-openapi
+Project-URL: Bug Tracker, https://github.com/Neoteroi/essentials-openapi/issues
+Author-email: Roberto Prevato <roberto.prevato@gmail.com>
+License-File: LICENSE
+Keywords: Markdown,api,docs,documentation,json,openapi,swagger,v2,v3,yaml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+Requires-Python: >=3.7
+Requires-Dist: essentials>=1.1.5
+Requires-Dist: pyyaml>=6
 Provides-Extra: full
-License-File: LICENSE
+Requires-Dist: click~=8.1.3; extra == 'full'
+Requires-Dist: httpx<1; extra == 'full'
+Requires-Dist: jinja2~=3.1.2; extra == 'full'
+Requires-Dist: markupsafe==2.1.2; extra == 'full'
+Requires-Dist: rich~=12.6.0; extra == 'full'
+Description-Content-Type: text/markdown
 
 ![Build](https://github.com/Neoteroi/essentials-openapi/workflows/Build/badge.svg)
 [![pypi](https://img.shields.io/pypi/v/essentials-openapi.svg)](https://pypi.python.org/pypi/essentials-openapi)
 [![versions](https://img.shields.io/pypi/pyversions/essentials-openapi.svg)](https://github.com/neoteroi/essentials-openapi)
 [![license](https://img.shields.io/github/license/neoteroi/essentials-openapi.svg)](https://github.com/neoteroi/essentials-openapi/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/Neoteroi/essentials-openapi/branch/main/graph/badge.svg?token=WEZ8YECJDF)](https://codecov.io/gh/Neoteroi/essentials-openapi)
```

### Comparing `essentials-openapi-1.0.6/README.md` & `essentials_openapi-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/commands/docs.py` & `essentials_openapi-1.0.7/openapidocs/commands/docs.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/common.py` & `essentials_openapi-1.0.7/openapidocs/common.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/main.py` & `essentials_openapi-1.0.7/openapidocs/main.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/__init__.py` & `essentials_openapi-1.0.7/openapidocs/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/common.py` & `essentials_openapi-1.0.7/openapidocs/mk/common.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/contents.py` & `essentials_openapi-1.0.7/openapidocs/mk/contents.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/generate.py` & `essentials_openapi-1.0.7/openapidocs/mk/generate.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/jinja.py` & `essentials_openapi-1.0.7/openapidocs/mk/jinja.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/md.py` & `essentials_openapi-1.0.7/openapidocs/mk/md.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/texts.py` & `essentials_openapi-1.0.7/openapidocs/mk/texts.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/__init__.py` & `essentials_openapi-1.0.7/openapidocs/mk/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/examples.py` & `essentials_openapi-1.0.7/openapidocs/mk/v3/examples.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/layout.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/layout.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/components-parameters.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/components-responses.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/info.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/info.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/path-items.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/path-items.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% for tag, operations in handler.get_operations().items() %}
 
-## {{tag}}
+## {{tag or "Endpoints"}}
 
 {% for path, definition in operations %}
-{%- for http_method, operation in definition.items() -%}
+{%- for http_method, operation in definition.items() %}
 
 ### {{http_method.upper()}} {{path | safe}}
 {% if "summary" in operation -%}
 {{operation.summary | wordwrap(80)}}
 {%- endif -%}
 
 {%- if operation.description and operation.summary != operation.description %}
```

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/request-responses.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_markdown/partial/schema-repr.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_markdown/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/layout.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/layout.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/components-security-schemes.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/info.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/info.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/path-items.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/path-items.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% for tag, operations in handler.get_operations().items() %}
-## <span class="api-tag">{{tag}}</span>
+## <span class="api-tag">{{tag or "Endpoints"}}</span>
 
 {% for path, definition in operations %}
-{%- for http_method, operation in definition.items() -%}
+{%- for http_method, operation in definition.items() %}
 <hr class="operation-separator" />
 
 ### <span class="http-{{http_method.lower()}}">{{http_method.upper()}}</span> {{path | route | safe}}
 {% if "summary" in operation -%}
 {{operation.summary | wordwrap(80)}}
 {%- endif -%}
```

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-body.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-body.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-parameters.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_mkdocs/partial/type.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_mkdocs/partial/type.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/layout.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/layout.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_api/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/layout.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/layout.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html` & `essentials_openapi-1.0.7/openapidocs/mk/v3/views_plantuml_schemas/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/utils/source.py` & `essentials_openapi-1.0.7/openapidocs/utils/source.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/utils/web.py` & `essentials_openapi-1.0.7/openapidocs/utils/web.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/v2.py` & `essentials_openapi-1.0.7/openapidocs/v2.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/openapidocs/v3.py` & `essentials_openapi-1.0.7/openapidocs/v3.py`

 * *Files identical despite different names*

### Comparing `essentials-openapi-1.0.6/setup.py` & `essentials_openapi-1.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-from setuptools import setup
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
-from openapidocs import VERSION
+[project]
+name = "essentials-openapi"
+dynamic = ["version"]
+authors = [{ name = "Roberto Prevato", email = "roberto.prevato@gmail.com" }]
+description = "Classes to generate OpenAPI Documentation v3 and v2, in JSON and YAML."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Operating System :: OS Independent",
+]
+keywords = ["openapi", "docs", "swagger", "api", "documentation", "v3", "v2", "json", "yaml", "Markdown"]
 
+dependencies = ["PyYAML>=6", "essentials>=1.1.5"]
 
-def readme():
-    with open("README.md") as f:
-        return f.read()
-
-
-setup(
-    name="essentials-openapi",
-    version=VERSION,
-    description="Classes to generate OpenAPI Documentation v3 and v2, in JSON and YAML",
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Operating System :: OS Independent",
-    ],
-    url="https://github.com/Neoteroi/essentials-openapi",
-    author="RobertoPrevato",
-    author_email="roberto.prevato@gmail.com",
-    keywords="openapi docs swagger api documentation v3 v2 json yaml Markdown",
-    license="MIT",
-    packages=[
-        "openapidocs",
-        "openapidocs.commands",
-        "openapidocs.mk",
-        "openapidocs.mk.v3",
-        "openapidocs.utils",
-    ],
-    install_requires=[
-        "PyYAML>=6",
-        "essentials>=1.1.5",
-        "dataclasses==0.7;python_version<'3.7'",
-    ],
-    extras_require={
-        "full": ["click~=8.1.3", "Jinja2~=3.1.2", "rich~=12.6.0", "httpx<1"]
-    },
-    entry_points={
-        "console_scripts": [
-            "openapidocs=openapidocs.main:main",
-            "oad=openapidocs.main:main",
-        ]
-    },
-    include_package_data=True,
-    zip_safe=False,
-)
+[tool.hatch.version]
+path = "openapidocs/__init__.py"
+
+[project.optional-dependencies]
+full = ["click~=8.1.3", "Jinja2~=3.1.2", "MarkupSafe==2.1.2", "rich~=12.6.0", "httpx<1"]
+
+[project.scripts]
+openapidocs = "openapidocs.main:main"
+oad = "openapidocs.main:main"
+
+[tool.hatch.build.targets.wheel]
+packages = ["openapidocs"]
+
+[tool.hatch.build.targets.sdist]
+exclude = ["tests"]
+
+[tool.hatch.build]
+only-packages = false
+include = [
+  "LICENSE",
+  "README.md",
+  "CHANGELOG.md",
+  "openapidocs/**/*.py",
+  "openapidocs/**/*.html",
+  "openapidocs/**/*.md",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Neoteroi/essentials-openapi"
+"Bug Tracker" = "https://github.com/Neoteroi/essentials-openapi/issues"
```

