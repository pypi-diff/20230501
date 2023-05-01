# Comparing `tmp/python_minifier-2.8.1.tar.gz` & `tmp/python_minifier-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_minifier-2.8.1.tar", last modified: Wed Mar 15 23:55:04 2023, max compression
+gzip compressed data, was "python_minifier-2.9.0.tar", last modified: Mon May  1 12:18:37 2023, max compression
```

## Comparing `python_minifier-2.8.1.tar` & `python_minifier-2.9.0.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.463412 python_minifier-2.8.1/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-03-15 23:54:57.000000 python_minifier-2.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6086 2023-03-15 23:55:04.463412 python_minifier-2.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4572 2023-03-15 23:54:57.000000 python_minifier-2.8.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-15 23:55:04.463412 python_minifier-2.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2072 2023-03-15 23:54:57.000000 python_minifier-2.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.455412 python_minifier-2.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.459412 python_minifier-2.8.1/src/python_minifier/
--rw-r--r--   0 root         (0) root         (0)     7163 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)     8557 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3134 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/ast_compare.py
--rw-r--r--   0 root         (0) root         (0)    21773 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/expression_printer.py
--rw-r--r--   0 root         (0) root         (0)    11289 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/f_string.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/ministring.py
--rw-r--r--   0 root         (0) root         (0)    22817 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/module_printer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.459412 python_minifier-2.8.1/src/python_minifier/rename/
--rw-r--r--   0 root         (0) root         (0)      375 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6166 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/bind_names.py
--rw-r--r--   0 root         (0) root         (0)    13968 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/binding.py
--rw-r--r--   0 root         (0) root         (0)     5827 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/mapper.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/name_generator.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/rename_literals.py
--rw-r--r--   0 root         (0) root         (0)     6676 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/renamer.py
--rw-r--r--   0 root         (0) root         (0)     3539 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/resolve_names.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/rename/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.459412 python_minifier-2.8.1/src/python_minifier/transforms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/combine_imports.py
--rw-r--r--   0 root         (0) root         (0)     3677 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_annotations.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_asserts.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_debug.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_literal_statements.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_object_base.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_pass.py
--rw-r--r--   0 root         (0) root         (0)      300 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/remove_posargs.py
--rw-r--r--   0 root         (0) root         (0)     6068 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/transforms/suite_transformer.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-15 23:54:57.000000 python_minifier-2.8.1/src/python_minifier/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.459412 python_minifier-2.8.1/src/python_minifier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6086 2023-03-15 23:55:04.000000 python_minifier-2.8.1/src/python_minifier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2155 2023-03-15 23:55:04.000000 python_minifier-2.8.1/src/python_minifier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 23:55:04.000000 python_minifier-2.8.1/src/python_minifier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-15 23:55:04.000000 python_minifier-2.8.1/src/python_minifier.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-15 23:55:04.000000 python_minifier-2.8.1/src/python_minifier.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 23:55:04.000000 python_minifier-2.8.1/src/python_minifier.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 23:55:04.463412 python_minifier-2.8.1/test/
--rw-r--r--   0 root         (0) root         (0)      618 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_assignment_expressions.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_await_fstring.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_combine_imports.py
--rw-r--r--   0 root         (0) root         (0)     2373 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_comprehension_rename.py
--rw-r--r--   0 root         (0) root         (0)     1181 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_decorator_expressions.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_dict_expansion.py
--rw-r--r--   0 root         (0) root         (0)      449 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_empty_fstring.py
--rw-r--r--   0 root         (0) root         (0)     8887 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_hoist_literals.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_iterable_unpacking.py
--rw-r--r--   0 root         (0) root         (0)     8591 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_match.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_match_rename.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_name_generator.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_nonlocal.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_posargs.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_preserve_shebang.py
--rw-r--r--   0 root         (0) root         (0)     4963 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_remove_annotations.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_remove_assert.py
--rw-r--r--   0 root         (0) root         (0)     3309 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_remove_debug.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_remove_literal_statements.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_remove_object.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_remove_pass.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_rename_builtins.py
--rw-r--r--   0 root         (0) root         (0)     7460 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_rename_locals.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-03-15 23:54:57.000000 python_minifier-2.8.1/test/test_slice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.639707 python_minifier-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-01 12:18:35.000000 python_minifier-2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6086 2023-05-01 12:18:37.639707 python_minifier-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-01 12:18:35.000000 python_minifier-2.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 12:18:37.639707 python_minifier-2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-05-01 12:18:35.000000 python_minifier-2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.623707 python_minifier-2.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.627707 python_minifier-2.9.0/src/python_minifier/
+-rw-r--r--   0 root         (0) root         (0)     7501 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)     8867 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/ast_compare.py
+-rw-r--r--   0 root         (0) root         (0)    22267 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/expression_printer.py
+-rw-r--r--   0 root         (0) root         (0)    13251 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/f_string.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/ministring.py
+-rw-r--r--   0 root         (0) root         (0)    23056 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/module_printer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.631707 python_minifier-2.9.0/src/python_minifier/rename/
+-rw-r--r--   0 root         (0) root         (0)      375 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6166 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/bind_names.py
+-rw-r--r--   0 root         (0) root         (0)    13968 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/binding.py
+-rw-r--r--   0 root         (0) root         (0)     5827 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/mapper.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/name_generator.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/rename_literals.py
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/renamer.py
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/resolve_names.py
+-rw-r--r--   0 root         (0) root         (0)     5103 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/rename/util.py
+-rw-r--r--   0 root         (0) root         (0)     9297 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/token_printer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.631707 python_minifier-2.9.0/src/python_minifier/transforms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/combine_imports.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_annotations.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_asserts.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_debug.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_explicit_return_none.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_literal_statements.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_object_base.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_pass.py
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/remove_posargs.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/transforms/suite_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-05-01 12:18:35.000000 python_minifier-2.9.0/src/python_minifier/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.627707 python_minifier-2.9.0/src/python_minifier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6086 2023-05-01 12:18:37.000000 python_minifier-2.9.0/src/python_minifier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-05-01 12:18:37.000000 python_minifier-2.9.0/src/python_minifier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 12:18:37.000000 python_minifier-2.9.0/src/python_minifier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-01 12:18:37.000000 python_minifier-2.9.0/src/python_minifier.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-01 12:18:37.000000 python_minifier-2.9.0/src/python_minifier.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 12:18:37.000000 python_minifier-2.9.0/src/python_minifier.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 12:18:37.635707 python_minifier-2.9.0/test/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_assignment_expressions.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_await_fstring.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_combine_imports.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_comprehension_rename.py
+-rw-r--r--   0 root         (0) root         (0)     1181 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_decorator_expressions.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_dict_expansion.py
+-rw-r--r--   0 root         (0) root         (0)      449 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_empty_fstring.py
+-rw-r--r--   0 root         (0) root         (0)     8887 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_hoist_literals.py
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_import.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_iterable_unpacking.py
+-rw-r--r--   0 root         (0) root         (0)     8591 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_match.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_match_rename.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_name_generator.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_nonlocal.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_posargs.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_preserve_shebang.py
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_annotations.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_assert.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_debug.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_explicit_return_none.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_literal_statements.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_object.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_remove_pass.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_rename_builtins.py
+-rw-r--r--   0 root         (0) root         (0)     7460 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_rename_locals.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-01 12:18:35.000000 python_minifier-2.9.0/test/test_slice.py
```

### Comparing `python_minifier-2.8.1/LICENSE` & `python_minifier-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/PKG-INFO` & `python_minifier-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_minifier
-Version: 2.8.1
+Version: 2.9.0
 Summary: Transform Python source code into it's most compact representation
 Home-page: https://github.com/dflook/python-minifier
 Author: Daniel Flook
 Author-email: daniel@flook.org
 License: MIT
 Project-URL: Issues, https://github.com/dflook/python-minifier/issues
 Project-URL: Documentation, https://dflook.github.io/python-minifier/
```

### Comparing `python_minifier-2.8.1/README.md` & `python_minifier-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/setup.py` & `python_minifier-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     package_dir={'': 'src'},
     packages=find_packages('src'),
     package_data={"python_minifier": ["py.typed", "__init__.pyi"]},
     long_description=long_desc,
     long_description_content_type='text/markdown',
 
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <3.12',
-    version='2.8.1',
+    version='2.9.0',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
```

### Comparing `python_minifier-2.8.1/src/python_minifier/__init__.py` & `python_minifier-2.9.0/src/python_minifier/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     add_namespace,
 )
 
 from python_minifier.transforms.combine_imports import CombineImports
 from python_minifier.transforms.remove_annotations import RemoveAnnotations
 from python_minifier.transforms.remove_asserts import RemoveAsserts
 from python_minifier.transforms.remove_debug import RemoveDebug
+from python_minifier.transforms.remove_explicit_return_none import RemoveExplicitReturnNone
 from python_minifier.transforms.remove_literal_statements import RemoveLiteralStatements
 from python_minifier.transforms.remove_object_base import RemoveObject
 from python_minifier.transforms.remove_pass import RemovePass
 from python_minifier.transforms.remove_posargs import remove_posargs
 
 
 class UnstableMinification(RuntimeError):
@@ -60,15 +61,16 @@
     preserve_locals=None,
     rename_globals=False,
     preserve_globals=None,
     remove_object_base=True,
     convert_posargs_to_args=True,
     preserve_shebang=True,
     remove_asserts=False,
-    remove_debug=False
+    remove_debug=False,
+    remove_explicit_return_none=True,
 ):
     """
     Minify a python module
 
     The module is transformed according the the arguments.
     If all transformation arguments are False, no transformations are made to the AST, the returned string will
     parse into exactly the same module.
@@ -90,14 +92,15 @@
     :param preserve_globals: Global names to leave unchanged when rename_globals is True
     :type preserve_globals: list[str]
     :param bool remove_object_base: If object as a base class may be removed
     :param bool convert_posargs_to_args: If positional-only arguments will be converted to normal arguments
     :param bool preserve_shebang: Keep any shebang interpreter directive from the source in the minified output
     :param bool remove_asserts: If assert statements should be removed
     :param bool remove_debug: If conditional statements that test '__debug__ is True' should be removed
+    :param bool remove_explicit_return_none: If explicit return None statements should be replaced with a bare return
 
     :rtype: str
 
     """
 
     filename = filename or 'python_minifier.minify source'
 
@@ -123,14 +126,17 @@
 
     if remove_asserts:
         module = RemoveAsserts()(module)
 
     if remove_debug:
         module = RemoveDebug()(module)
 
+    if remove_explicit_return_none:
+        module = RemoveExplicitReturnNone()(module)
+
     bind_names(module)
     resolve_names(module)
 
     if module.tainted:
         rename_globals = False
         rename_locals = False
```

### Comparing `python_minifier-2.8.1/src/python_minifier/__init__.pyi` & `python_minifier-2.9.0/src/python_minifier/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     preserve_locals: Optional[List[Text]] = ...,
     rename_globals: bool = ...,
     preserve_globals: Optional[List[Text]] = ...,
     remove_object_base: bool = ...,
     convert_posargs_to_args: bool = ...,
     preserve_shebang: bool = ...,
     remove_asserts: bool = ...,
-    remove_debug: bool = ...
+    remove_debug: bool = ...,
+    remove_explicit_return_none: bool = ...
 ) -> Text: ...
 
 def unparse(module: ast.Module) -> Text: ...
 
 def awslambda(
     source: AnyStr,
     filename: Optional[Text] = ...,
```

### Comparing `python_minifier-2.8.1/src/python_minifier/__main__.py` & `python_minifier-2.9.0/src/python_minifier/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,15 +179,20 @@
     )
     minification_options.add_argument(
         '--remove-debug',
         action='store_true',
         help='Remove conditional statements that test __debug__ is True',
         dest='remove_debug',
     )
-
+    minification_options.add_argument(
+        '--no-remove-explicit-return-none',
+        action='store_false',
+        help='Replace explicit return None with a bare return',
+        dest='remove_explicit_return_none',
+    )
     parser.add_argument('--version', '-v', action='version', version=version)
 
     args = parser.parse_args()
 
     # Handle some invalid argument combinations
     if '-' in args.path and len(args.path) != 1:
         sys.stderr.write('error: multiple path arguments, reading from stdin not allowed\n')
@@ -244,13 +249,14 @@
         preserve_locals=preserve_locals,
         rename_globals=minification_args.rename_globals,
         preserve_globals=preserve_globals,
         remove_object_base=minification_args.remove_object_base,
         convert_posargs_to_args=minification_args.convert_posargs_to_args,
         preserve_shebang=minification_args.preserve_shebang,
         remove_asserts=minification_args.remove_asserts,
-        remove_debug=minification_args.remove_debug
+        remove_debug=minification_args.remove_debug,
+        remove_explicit_return_none=minification_args.remove_explicit_return_none,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `python_minifier-2.8.1/src/python_minifier/ast_compare.py` & `python_minifier-2.9.0/src/python_minifier/ast_compare.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/expression_printer.py` & `python_minifier-2.9.0/src/python_minifier/expression_printer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import ast
 import sys
 
 from python_minifier.util import is_ast_node
 
+from python_minifier.token_printer import TokenPrinter, Delimiter
+
 
 class ExpressionPrinter(object):
     """
     Builds the smallest possible exact representation of an ast
     """
 
     def __init__(self):
 
-        self.code = ''
-        self.indent = 0
-        self.unicode_literals = False
-
         self.precedences = {
             'Lambda': 2,  # Lambda
             'IfExp': 3,  # IfExp
             'comprehension': 3.5,
             'Or': 4,  # BoolOp
             'And': 5,
             'Not': 6,
@@ -29,29 +27,31 @@
             'LShift': 11, 'RShift': 11,
             'Add': 12, 'Sub': 12,
             'Mult': 13, 'Div': 13, 'FloorDiv': 13, 'Mod': 13, 'MatMult': 13,
             'UAdd': 14, 'USub': 14, 'Invert': 14,
             'Pow': 15,
             'Await': 16,
             'Subscript': 17, 'Call': 17, 'Attribute': 17,
-            'Tuple': 18, 'Set': 18, 'List': 18, 'Dict': 18,
+            'Tuple': 18, 'Set': 18, 'List': 18, 'Dict': 18, 'ListComp': 18, 'SetComp': 18, 'DictComp': 18, 'GeneratorExp': 18,  # Container
         }
 
+        self.printer = TokenPrinter()
+
     def __call__(self, module):
         """
         Generate the source code for an AST
 
         :param module: The Module to generate code for
         :type module: ast.Module
         :rtype: str
 
         """
 
         self.visit(module)
-        return self.code
+        return str(self.printer)
 
     def precedence(self, node):
         """
         The precedence of an expression
 
         Node will usually be an operator or literal.
         Nodes with no precedence value return 0.
@@ -94,144 +94,114 @@
 
     def visit_Unknown(self, node):
         raise RuntimeError('Unknown node %r' % node)
 
     # region Literals
 
     def visit_Constant(self, node):
-        if node.value in [None, True, False]:
+        if node.value is None or node.value is True or node.value is False:
             return self.visit_NameConstant(node)
         elif isinstance(node.value, (int, float, complex)):
             return self.visit_Num(node)
         elif isinstance(node.value, str):
             return self.visit_Str(node)
         elif isinstance(node.value, bytes):
             return self.visit_Bytes(node)
         elif node.value == Ellipsis:
             return self.visit_Ellipsis(node)
 
         raise RuntimeError('Unknown Constant value %r' % type(node.value))
 
     def visit_Num(self, node):
-        self.token_break()
-
-        v = repr(node.n)
-
-        if v == 'inf':
-            self.code += '1e999'
-        elif v == '-inf':
-            self.code += '-1e999'
-        elif v in ['infj', 'inf*j']:
-            self.code += '1e999j'
-        elif v in ['-infj', '-inf*j']:
-            self.code += '-1e999j'
-
-        else:
-            if isinstance(node.n, int):
-                # Due to the 0x notation, it's unlikely a base-16 literal will be more compact than base-10
-                # But for those rare cases....
-                h = hex(node.n)
-                if len(h) < len(v):
-                    v = h
-
-            self.code += v
+        if isinstance(node.n, float):
+            self.printer.floatnumber(node.n)
+        elif isinstance(node.n, complex):
+            self.printer.imagnumber(node.n)
+        else:
+            # int or possibly long in python2
+            self.printer.integer(node.n)
 
     def visit_Str(self, node):
-
-        s = repr(node.s)
-
-        if sys.version_info < (3, 0) and self.unicode_literals:
-            if s[0] == 'u':
-                s = s[1:]
-            else:
-                s = 'b' + s
-
-        if len(s) > 0 and s[0].isalpha():
-            self.token_break()
-
-        self.code += s
+        self.printer.stringliteral(node.s)
 
     def visit_Bytes(self, node):
-
-        s = repr(node.s)
-
-        if len(s) > 0 and s[0].isalpha():
-            self.token_break()
-
-        self.code += s
+        self.printer.bytesliteral(node.s)
 
     def visit_List(self, node):
-        self.code += '['
+        self.printer.delimiter('[')
         self._exprlist(node.elts)
-        self.code += ']'
+        self.printer.delimiter(']')
 
     def visit_Tuple(self, node):
 
         if len(node.elts) == 0:
-            self.code += '()'
+            self.printer.delimiter('(')
+            self.printer.delimiter(')')
             return
 
         self._exprlist(node.elts)
 
         if len(node.elts) == 1:
-            self.code += ','
+            self.printer.delimiter(',')
 
     def visit_Set(self, node):
-        self.code += '{'
+        self.printer.delimiter('{')
         self._exprlist(node.elts)
-        self.code += '}'
+        self.printer.delimiter('}')
 
     def visit_Dict(self, node):
-        self.code += '{'
+        assert isinstance(node, ast.Dict)
 
-        first = True
-        for k, v in zip(node.keys, node.values):
-            if not first:
-                self.code += ','
-            else:
-                first = False
+        def key_datum(key, datum):
 
-            if k is None:
-                self.code += '**'
+            if key is None:
+                self.printer.operator('**')
 
-                if 0 < self.precedence(v) <=7:
-                    self.code += '('
-                    self._expression(v)
-                    self.code += ')'
+                if 0 < self.precedence(datum) <=7:
+                    self.printer.delimiter('(')
+                    self._expression(datum)
+                    self.printer.delimiter(')')
                 else:
-                    self._expression(v)
+                    self._expression(datum)
             else:
-                self._expression(k)
-                self.code += ':'
+                self._expression(key)
+                self.printer.delimiter(':')
 
-                self._expression(v)
+                self._expression(datum)
+
+        self.printer.delimiter('{')
+
+        delimiter = Delimiter(self.printer)
+        for key, datum in zip(node.keys, node.values):
+            delimiter.new_item()
+            key_datum(key, datum)
 
-        self.code += '}'
+        self.printer.delimiter('}')
 
     def visit_Ellipsis(self, node):
-        self.code += '...'
+        self.printer.delimiter('.')
+        self.printer.delimiter('.')
+        self.printer.delimiter('.')
 
     def visit_NameConstant(self, node):
-        self.token_break()
-        self.code += repr(node.value)
+        self.printer.keyword(repr(node.value))
 
     # endregion
 
     # region Variables
 
     def visit_Name(self, node):
-        self.token_break()
-        self.code += node.id
+        self.printer.identifier(node.id)
 
     def visit_Starred(self, node):
-        self.code += '*'
-        if self.precedence(node.value) <= 7:
-            self.code += '('
+        self.printer.operator('*')
+        if 0 < self.precedence(node.value) <= 7:
+            self.printer.delimiter('(')
             self._expression(node.value)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self._expression(node.value)
 
     # endregion
 
     # region Expressions
 
@@ -239,77 +209,86 @@
         self.visit(node.op)
 
         if sys.version_info < (3, 0) and isinstance(node.op, ast.USub) and isinstance(node.operand, ast.Num):
             # For: -(1), which is parsed as a UnaryOp(USub, Num(1)).
             # Without this special case it would be printed as -1
             # This is fine, but python 2 will then parse it at Num(-1) so the AST wouldn't round-trip.
 
-            self.code += '('
+            self.printer.delimiter('(')
             self.visit_Num(node.operand)
-            self.code += ')'
+            self.printer.delimiter(')')
             return
 
-        self._rhs(node.operand, node)
+        right_precedence = self.precedence(node.operand)
+        op_precedence = self.precedence(node)
+
+        if right_precedence != 0 and (
+            (op_precedence > right_precedence)
+        ):
+            self.printer.delimiter('(')
+            self._expression(node.operand)
+            self.printer.delimiter(')')
+        else:
+            self._expression(node.operand)
 
     def visit_UAdd(self, node):
-        self.code += '+'
+        self.printer.operator('+')
 
     def visit_USub(self, node):
-        self.code += '-'
+        self.printer.operator('-')
 
     def visit_Not(self, node):
-        self.token_break()
-        self.code += 'not'
+        self.printer.keyword('not')
 
     def visit_Invert(self, node):
-        self.code += '~'
+        self.printer.operator('~')
 
     def visit_BinOp(self, node):
         self._lhs(node.left, node.op)
         self.visit(node.op)
         self._rhs(node.right, node.op)
 
     def visit_Add(self, node):
-        self.code += '+'
+        self.printer.operator('+')
 
     def visit_Sub(self, node):
-        self.code += '-'
+        self.printer.operator('-')
 
     def visit_Mult(self, node):
-        self.code += '*'
+        self.printer.operator('*')
 
     def visit_Div(self, node):
-        self.code += '/'
+        self.printer.operator('/')
 
     def visit_FloorDiv(self, node):
-        self.code += '//'
+        self.printer.operator('//')
 
     def visit_Mod(self, node):
-        self.code += '%'
+        self.printer.operator('%')
 
     def visit_Pow(self, node):
-        self.code += '**'
+        self.printer.operator('**')
 
     def visit_LShift(self, node):
-        self.code += '<<'
+        self.printer.operator('<<')
 
     def visit_RShift(self, node):
-        self.code += '>>'
+        self.printer.operator('>>')
 
     def visit_BitOr(self, node):
-        self.code += '|'
+        self.printer.operator('|')
 
     def visit_BitXor(self, node):
-        self.code += '^'
+        self.printer.operator('^')
 
     def visit_BitAnd(self, node):
-        self.code += '&'
+        self.printer.operator('&')
 
     def visit_MatMult(self, node):
-        self.code += '@'
+        self.printer.operator('@')
 
     def visit_BoolOp(self, node):
         first = True
 
         op_precedence = self.precedence(node.op)
 
         for v in node.values:
@@ -321,175 +300,165 @@
             value_precedence = self.precedence(v)
 
             if value_precedence != 0 and (
                 (op_precedence > value_precedence)
                 or op_precedence == value_precedence
                 and self._is_left_associative(node.op)
             ):
-                self.code += '('
+                self.printer.delimiter('(')
                 self._expression(v)
-                self.code += ')'
+                self.printer.delimiter(')')
             else:
                 self._expression(v)
 
     def visit_And(self, node):
-        self.token_break()
-        self.code += 'and'
+        self.printer.keyword('and')
 
     def visit_Or(self, node):
-        self.token_break()
-        self.code += 'or'
+        self.printer.keyword('or')
 
     def visit_Compare(self, node):
 
         left_precedence = self.precedence(node.left)
         op_precedence = self.precedence(node.ops[0])
 
         if left_precedence != 0 and ((op_precedence > left_precedence) or (op_precedence == left_precedence)):
-            self.code += '('
+            self.printer.delimiter('(')
             self._expression(node.left)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self._expression(node.left)
 
         for op, comparator in zip(node.ops, node.comparators):
             self._expression(op)
             self._rhs(comparator, op)
 
     def visit_Eq(self, node):
-        self.code += '=='
+        self.printer.operator('==')
 
     def visit_NotEq(self, node):
-        self.code += '!='
+        self.printer.operator('!=')
 
     def visit_Lt(self, node):
-        self.code += '<'
+        self.printer.operator('<')
 
     def visit_LtE(self, node):
-        self.code += '<='
+        self.printer.operator('<=')
 
     def visit_Gt(self, node):
-        self.code += '>'
+        self.printer.operator('>')
 
     def visit_GtE(self, node):
-        self.code += '>='
+        self.printer.operator('>=')
 
     def visit_Is(self, node):
-        self.token_break()
-        self.code += 'is'
+        self.printer.keyword('is')
 
     def visit_IsNot(self, node):
-        self.token_break()
-        self.code += 'is not'
+        self.printer.keyword('is')
+        self.printer.keyword('not')
 
     def visit_In(self, node):
-        self.token_break()
-        self.code += 'in'
+        self.printer.keyword('in')
 
     def visit_NotIn(self, node):
-        self.token_break()
-        self.code += 'not in'
+        self.printer.keyword('not')
+        self.printer.keyword('in')
 
     def visit_Call(self, node):
 
         self._lhs(node.func, node)
 
-        self.code += '('
+        self.printer.delimiter('(')
+
+        single_call = len(node.args) == 1 and not node.keywords and not hasattr(node, 'starargs') and not hasattr(node, 'kwargs')
+
+        delimiter = Delimiter(self.printer)
 
-        first = True
         for arg in node.args:
-            if first:
-                first = False
-            else:
-                self.code += ','
+            delimiter.new_item()
 
-            self._expression(arg)
+            if single_call and isinstance(arg, ast.GeneratorExp):
+                self.visit_GeneratorExp(arg, omit_parens=True)
+            else:
+                self._expression(arg)
 
         if node.keywords:
             for kwarg in node.keywords:
-                if first:
-                    first = False
-                else:
-                    self.code += ','
+                delimiter.new_item()
 
                 assert isinstance(kwarg, ast.keyword)
                 self.visit_keyword(kwarg)
 
         if hasattr(node, 'starargs') and node.starargs is not None:
-            if first:
-                first = False
-            else:
-                self.code += ','
+            delimiter.new_item()
 
-            self.code += '*'
+            self.printer.operator('*')
             self._expression(node.starargs)
 
         if hasattr(node, 'kwargs') and node.kwargs is not None:
-            if not first:
-                self.code += ','
+            delimiter.new_item()
 
-            self.code += '**'
+            self.printer.operator('**')
             self.visit(node.kwargs)
 
-        self.code += ')'
+        self.printer.delimiter(')')
 
     def visit_keyword(self, node):
         if node.arg is None:
-            self.code += '**'
+            self.printer.operator('**')
             self._expression(node.value)
         else:
-            self.code += node.arg + '='
+            self.printer.identifier(node.arg)
+            self.printer.delimiter('=')
             self._expression(node.value)
 
     def visit_IfExp(self, node):
 
         self._rhs(node.body, node)
 
-        self.token_break()
-        self.code += 'if'
+        self.printer.keyword('if')
 
         self._rhs(node.test, node)
 
-        self.token_break()
-        self.code += 'else'
+        self.printer.keyword('else')
 
         self._expression(node.orelse)
 
     def visit_Attribute(self, node):
-        self.token_break()
-
         value_precedence = self.precedence(node.value)
         attr_precedence = self.precedence(node)
 
         if (value_precedence != 0 and (attr_precedence > value_precedence)) or isinstance(node.value, ast.Num):
-            self.code += '('
+            self.printer.delimiter('(')
             self._expression(node.value)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self._expression(node.value)
 
-        self.code += '.' + node.attr
+        self.printer.delimiter('.')
+        self.printer.identifier(node.attr)
 
     # endregion
 
     # region Subscripting
 
     def visit_Subscript(self, node):
 
         value_precedence = self.precedence(node.value)
         slice_precedence = 17  # self.precedence(node)
 
         if value_precedence != 0 and (slice_precedence > value_precedence):
-            self.code += '('
+            self.printer.delimiter('(')
             self._expression(node.value)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self._expression(node.value)
 
-        self.code += '['
+        self.printer.delimiter('[')
 
         if isinstance(node.slice, ast.Index):
             self.visit_Index(node.slice)
         elif isinstance(node.slice, ast.Slice):
             self.visit_Slice(node.slice)
         elif isinstance(node.slice, ast.ExtSlice):
             self.visit_ExtSlice(node.slice)
@@ -498,254 +467,230 @@
         elif sys.version_info >= (3, 9) and isinstance(node.slice, ast.Tuple):
             self.visit_Tuple(node.slice)
         elif sys.version_info >= (3, 9):
             self._expression(node.slice)
         else:
             raise AssertionError('Unknown slice type %r' % node.slice)
 
-        self.code += ']'
+        self.printer.delimiter(']')
 
     def visit_Index(self, node):
         self._expression(node.value)
 
     def visit_Slice(self, node):
         if node.lower:
             self._expression(node.lower)
-        self.code += ':'
+        self.printer.delimiter(':')
+
         if node.upper:
             self._expression(node.upper)
         if node.step:
-            self.code += ':'
+            self.printer.delimiter(':')
             self._expression(node.step)
 
     def visit_ExtSlice(self, node):
-        first = True
 
+        delimiter = Delimiter(self.printer)
         for s in node.dims:
-            if not first:
-                self.code += ','
-            else:
-                first = False
-
+            delimiter.new_item()
             self._expression(s)
 
         if len(node.dims) == 1:
-            self.code += ','
+            self.printer.delimiter(',')
 
     # endregion
 
     # region Comprehensions
 
     def visit_ListComp(self, node):
-        self.code += '['
+        self.printer.delimiter('[')
         self._expression(node.elt)
         [self.visit_comprehension(x) for x in node.generators]
-        self.code += ']'
+        self.printer.delimiter(']')
 
     def visit_SetComp(self, node):
-        self.code += '{'
+        self.printer.delimiter('{')
         self._expression(node.elt)
         [self.visit_comprehension(x) for x in node.generators]
-        self.code += '}'
+        self.printer.delimiter('}')
+
+    def visit_GeneratorExp(self, node, omit_parens=False):
+
+        if not omit_parens:
+            self.printer.delimiter('(')
 
-    def visit_GeneratorExp(self, node):
-        self.code += '('
         self._expression(node.elt)
         [self.visit_comprehension(x) for x in node.generators]
-        self.code += ')'
+
+        if not omit_parens:
+            self.printer.delimiter(')')
 
     def visit_DictComp(self, node):
-        self.code += '{'
+        self.printer.delimiter('{')
         self._expression(node.key)
-        self.code += ':'
+        self.printer.delimiter(':')
         self._expression(node.value)
         [self.visit_comprehension(x) for x in node.generators]
-        self.code += '}'
+        self.printer.delimiter('}')
 
     def visit_comprehension(self, node):
         assert isinstance(node, ast.comprehension)
 
-        self.token_break()
-
         if hasattr(node, 'is_async') and node.is_async:
-            self.code += 'async '
+            self.printer.keyword('async')
 
-        self.code += 'for'
+        self.printer.keyword('for')
         self._exprlist([node.target])
-        self.token_break()
-        self.code += 'in'
+        self.printer.keyword('in')
 
         self._rhs(node.iter, node)
 
         if node.ifs:
             for i in node.ifs:
-                self.token_break()
-                self.code += 'if'
+                self.printer.keyword('if')
                 self._rhs(i, node)
 
     # endregion
 
     # region Function and Class definitions
 
     def visit_Lambda(self, node):
 
-        self.token_break()
-        self.code += 'lambda'
+        self.printer.keyword('lambda')
 
         self.visit_arguments(node.args)
 
-        self.code += ':'
+        self.printer.delimiter(':')
 
         self._expression(node.body)
 
     def visit_arguments(self, node):
-        first = True
-
         args = getattr(node, 'posonlyargs', []) + node.args
 
+        delimiter = Delimiter(self.printer)
+
         count_no_defaults = len(args) - len(node.defaults)
         for i, arg in enumerate(args):
-            if not first:
-                self.code += ','
-            else:
-                self.token_break()
-                first = False
+            delimiter.new_item()
 
             self._expression(arg)
 
             if i >= count_no_defaults:
-                self.code += '='
+                self.printer.delimiter('=')
                 self._expression(node.defaults[i - count_no_defaults])
 
             if hasattr(node, 'posonlyargs') and node.posonlyargs and i + 1 == len(node.posonlyargs):
-                self.code += ',/'
+                self.printer.delimiter(',')
+                self.printer.operator('/')
 
         if node.vararg:
-            if not first:
-                self.code += ','
-            else:
-                self.token_break()
-                first = False
+            delimiter.new_item()
 
-            self.code += '*'
+            self.printer.operator('*')
 
             if hasattr(node, 'varargannotation'):
-                self.code += node.vararg
+                self.printer.identifier(node.vararg)
                 if node.varargannotation is not None:
-                    self.code += ':'
+                    self.printer.delimiter(':')
                     self._expression(node.varargannotation)
             elif isinstance(node.vararg, str):
-                self.code += node.vararg
+                self.printer.identifier(node.vararg)
             else:
                 self.visit(node.vararg)
 
         if hasattr(node, 'kwonlyargs') and node.kwonlyargs:
 
             if not node.vararg:
-                if not first:
-                    self.code += ','
-                else:
-                    self.token_break()
-                    first = False
-
-                self.code += '*'
+                delimiter.new_item()
+                self.printer.operator('*')
 
             for i, arg in enumerate(node.kwonlyargs):
-                self.code += ','
+                self.printer.delimiter(',')
                 self.visit_arg(arg)
 
                 if node.kw_defaults[i] is not None:
-                    self.code += '='
+                    self.printer.delimiter('=')
                     self._expression(node.kw_defaults[i])
 
         if node.kwarg:
-            if not first:
-                self.code += ','
-            else:
-                self.token_break()
-                first = False
+            delimiter.new_item()
 
-            self.code += '**'
+            self.printer.operator('**')
 
             if hasattr(node, 'kwargannotation'):
-                self.code += node.kwarg
+                self.printer.identifier(node.kwarg)
                 if node.kwargannotation is not None:
-                    self.code += ':'
+                    self.printer.delimiter(':')
                     self._expression(node.kwargannotation)
             elif isinstance(node.kwarg, str):
-                self.code += node.kwarg
+                self.printer.identifier(node.kwarg)
             else:
                 self.visit(node.kwarg)
 
     def visit_arg(self, node):
         if isinstance(node, ast.Name):
             # Python 2 uses Name nodes
             return self.visit_Name(node)
 
-        self.code += node.arg
+        self.printer.identifier(node.arg)
 
         if node.annotation:
-            self.code += ':'
+            self.printer.delimiter(':')
             self._expression(node.annotation)
 
     def visit_Repr(self, node):
-        self.code += '`'
+        self.printer.delimiter('`')
         self._expression(node.value)
-        self.code += '`'
+        self.printer.delimiter('`')
 
     # endregion
 
     def visit_Expression(self, node):
         self._expression(node.body)
 
     def _expression(self, expression):
         if is_ast_node(expression, (ast.Yield, 'YieldFrom')):
-            self.code += '('
+            self.printer.delimiter('(')
             self._yield_expr(expression)
-            self.code += ')'
+            self.printer.delimiter(')')
         elif isinstance(expression, ast.Tuple) and len(expression.elts) > 0:
-            self.code += '('
+            self.printer.delimiter('(')
             self.visit_Tuple(expression)
-            self.code += ')'
+            self.printer.delimiter(')')
         elif is_ast_node(expression, 'NamedExpr'):
-            self.code += '('
+            self.printer.delimiter('(')
             self.visit_NamedExpr(expression)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self.visit(expression)
 
     def _testlist(self, test):
         if is_ast_node(test, (ast.Yield, 'YieldFrom')):
-            self.code += '('
+            self.printer.delimiter('(')
             self._yield_expr(test)
-            self.code += ')'
+            self.printer.delimiter(')')
         elif is_ast_node(test, 'NamedExpr'):
-            self.code += '('
+            self.printer.delimiter('(')
             self.visit_NamedExpr(test)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self.visit(test)
 
     def _exprlist(self, exprlist):
-        first = True
-
+        delimiter = Delimiter(self.printer)
         for expr in exprlist:
-            if first:
-                first = False
-            else:
-                self.code += ','
+            delimiter.new_item()
             self._expression(expr)
 
     def _yield_expr(self, yield_node):
-        self.token_break()
-
         if isinstance(yield_node, ast.Yield):
-            self.code += 'yield'
+            self.printer.keyword('yield')
         elif isinstance(yield_node, ast.YieldFrom):
-            self.code += 'yield from'
+            self.printer.keyword('yield')
+            self.printer.keyword('from')
 
         if yield_node.value is not None:
             self._expression(yield_node.value)
 
     @staticmethod
     def _is_right_associative(operator):
         return isinstance(operator, ast.Pow)
@@ -758,52 +703,46 @@
         left_precedence = self.precedence(left_node)
         op_precedence = self.precedence(op_node)
 
         if left_precedence != 0 and (
             (op_precedence > left_precedence)
             or (op_precedence == left_precedence and self._is_right_associative(op_node))
         ):
-            self.code += '('
+            self.printer.delimiter('(')
             self._expression(left_node)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self._expression(left_node)
 
     def _rhs(self, right_node, op_node):
         right_precedence = self.precedence(right_node)
         op_precedence = self.precedence(op_node)
 
+        if isinstance(op_node, ast.Pow) and right_precedence == 14:
+            op_precedence = right_precedence
+
         if right_precedence != 0 and (
             (op_precedence > right_precedence)
             or (op_precedence == right_precedence and self._is_left_associative(op_node))
         ):
-            self.code += '('
+            self.printer.delimiter('(')
             self._expression(right_node)
-            self.code += ')'
+            self.printer.delimiter(')')
         else:
             self._expression(right_node)
 
-    def token_break(self):
-        if len(self.code) == 0:
-            return
-
-        if self.code[-1] not in '[]{}() :"\'=\n\t<>|^&+-*@/%;,':
-            self.code += ' '
-
     def visit_JoinedStr(self, node):
         assert isinstance(node, ast.JoinedStr)
 
         import python_minifier.f_string
 
-        self.token_break()
-        self.code += str(python_minifier.f_string.OuterFString(node))
+        self.printer.fstring(str(python_minifier.f_string.OuterFString(node)))
 
     def visit_NamedExpr(self, node):
         self._expression(node.target)
-        self.code += ':='
+        self.printer.operator(':=')
         self._expression(node.value)
 
     def visit_Await(self, node):
         assert isinstance(node, ast.Await)
-        self.token_break()
-        self.code += 'await'
+        self.printer.keyword('await')
         self._rhs(node.value, node)
```

### Comparing `python_minifier-2.8.1/src/python_minifier/f_string.py` & `python_minifier-2.9.0/src/python_minifier/f_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 This whole module feels like a hack.
 Mostly because FStrings feel like a hack.
 
 """
 
 import ast
 import copy
+import re
 
 from python_minifier import UnstableMinification
 from python_minifier.ast_compare import CompareError
 from python_minifier.ast_compare import compare_ast
 from python_minifier.expression_printer import ExpressionPrinter
 from python_minifier.ministring import MiniString
+from python_minifier.token_printer import TokenTypes
 from python_minifier.util import is_ast_node
 
 
 class FString(object):
     """
     An F-string in the expression part of another f-string
     """
@@ -32,32 +34,65 @@
         try:
             c = ast.parse(code, 'FString candidate', mode='eval')
             compare_ast(self.node, c.body)
             return True
         except Exception as e:
             return False
 
+    def complete_debug_specifier(self, partial_specifier_candidates, value_node):
+        assert isinstance(value_node, ast.FormattedValue)
+
+        conversion = ''
+        if value_node.conversion == 115:
+            conversion = '!s'
+        elif value_node.conversion == 114 and value_node.format_spec is not None:
+            # This is the default for debug specifiers, unless there's a format_spec
+            conversion = '!r'
+        elif value_node.conversion == 97:
+            conversion = '!a'
+
+        conversion_candidates = [x + conversion for x in partial_specifier_candidates]
+
+        if value_node.format_spec is not None:
+            conversion_candidates = [c + ':' + fs for c in conversion_candidates for fs in FormatSpec(value_node.format_spec, self.allowed_quotes).candidates()]
+
+        return [x + '}' for x in conversion_candidates]
+
     def candidates(self):
         actual_candidates = []
 
         for quote in self.allowed_quotes:
             candidates = ['']
+            debug_specifier_candidates = []
             nested_allowed = copy.copy(self.allowed_quotes)
             nested_allowed.remove(quote)
             for v in self.node.values:
                 if is_ast_node(v, ast.Str):
+
+                    # Could this be used as a debug specifier?
+                    if len(candidates) < 10:
+                        debug_specifier = re.match(r'.*=\s*$', v.s)
+                        if debug_specifier:
+                            # Maybe!
+                            try:
+                                debug_specifier_candidates = [x + '{' + v.s for x in candidates]
+                            except Exception as e:
+                                continue
+
                     try:
                         candidates = [x + self.str_for(v.s, quote) for x in candidates]
                     except Exception as e:
                         continue
                 elif isinstance(v, ast.FormattedValue):
                     try:
+                        completed = self.complete_debug_specifier(debug_specifier_candidates, v)
                         candidates = [
                             x + y for x in candidates for y in FormattedValue(v, nested_allowed).get_candidates()
-                        ]
+                        ] + completed
+                        debug_specifier_candidates = []
                     except Exception as e:
                         continue
                 else:
                     raise RuntimeError('Unexpected JoinedStr value')
 
                 actual_candidates += ['f' + quote + x + quote for x in candidates]
 
@@ -100,15 +135,15 @@
 
         if not candidates:
             raise ValueError('Unable to create representation for f-string')
 
         return min(candidates, key=len)
 
     def str_for(self, s, quote):
-        mini_s =  str(MiniString(s, quote)).replace('{', '{{').replace('}', '}}')
+        mini_s = str(MiniString(s, quote)).replace('{', '{{').replace('}', '}}')
 
         if mini_s == '':
             return '\\\n'
         return mini_s
 
 
 class FormattedValue(ExpressionPrinter):
@@ -122,33 +157,33 @@
         assert isinstance(node, ast.FormattedValue)
         self.node = node
         self.allowed_quotes = allowed_quotes
         self.candidates = ['']
 
     def get_candidates(self):
 
-        self.code = '{'
+        self.printer.delimiter('{')
 
         if self.is_curly(self.node.value):
-            self.code += ' '
+            self.printer.delimiter(' ')
 
         self._expression(self.node.value)
 
         if self.node.conversion == 115:
-            self.code += '!s'
+            self.printer.append('!s', TokenTypes.Delimiter)
         elif self.node.conversion == 114:
-            self.code += '!r'
+            self.printer.append('!r', TokenTypes.Delimiter)
         elif self.node.conversion == 97:
-            self.code += '!a'
+            self.printer.append('!a', TokenTypes.Delimiter)
 
         if self.node.format_spec is not None:
-            self.code += ':'
+            self.printer.delimiter(':')
             self._append(FormatSpec(self.node.format_spec, self.allowed_quotes).candidates())
 
-        self.code += '}'
+        self.printer.delimiter('}')
 
         self._finalize()
         return self.candidates
 
     def is_curly(self, node):
         if isinstance(node, (ast.SetComp, ast.DictComp, ast.Set, ast.Dict)):
             return True
@@ -167,27 +202,28 @@
 
         if isinstance(node, ast.IfExp):
             return self.is_curly(node.body)
 
         return False
 
     def visit_Str(self, node):
-        self.code += str(Str(node.s, self.allowed_quotes))
+        self.printer.append(str(Str(node.s, self.allowed_quotes)), TokenTypes.NonNumberLiteral)
 
     def visit_Bytes(self, node):
-        self.code += str(Bytes(node.s, self.allowed_quotes))
+        self.printer.append(str(Bytes(node.s, self.allowed_quotes)), TokenTypes.NonNumberLiteral)
 
     def visit_JoinedStr(self, node):
         assert isinstance(node, ast.JoinedStr)
-        self.token_break()
+        if self.printer.previous_token in [TokenTypes.Identifier, TokenTypes.Keyword, TokenTypes.SoftKeyword]:
+            self.printer.delimiter(' ')
         self._append(FString(node, allowed_quotes=self.allowed_quotes).candidates())
 
     def _finalize(self):
-        self.candidates = [x + self.code for x in self.candidates]
-        self.code = ''
+        self.candidates = [x + str(self.printer) for x in self.candidates]
+        self.printer._code = ''
 
     def _append(self, candidates):
         self._finalize()
         self.candidates = [x + y for x in self.candidates for y in candidates]
 
 
 class Str(object):
```

### Comparing `python_minifier-2.8.1/src/python_minifier/ministring.py` & `python_minifier-2.9.0/src/python_minifier/ministring.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/bind_names.py` & `python_minifier-2.9.0/src/python_minifier/rename/bind_names.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/binding.py` & `python_minifier-2.9.0/src/python_minifier/rename/binding.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/mapper.py` & `python_minifier-2.9.0/src/python_minifier/rename/mapper.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/name_generator.py` & `python_minifier-2.9.0/src/python_minifier/rename/name_generator.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/rename_literals.py` & `python_minifier-2.9.0/src/python_minifier/rename/rename_literals.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/renamer.py` & `python_minifier-2.9.0/src/python_minifier/rename/renamer.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/resolve_names.py` & `python_minifier-2.9.0/src/python_minifier/rename/resolve_names.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/rename/util.py` & `python_minifier-2.9.0/src/python_minifier/rename/util.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/combine_imports.py` & `python_minifier-2.9.0/src/python_minifier/transforms/combine_imports.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/remove_annotations.py` & `python_minifier-2.9.0/src/python_minifier/transforms/remove_annotations.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/remove_asserts.py` & `python_minifier-2.9.0/src/python_minifier/transforms/remove_asserts.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/remove_debug.py` & `python_minifier-2.9.0/src/python_minifier/transforms/remove_debug.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/remove_literal_statements.py` & `python_minifier-2.9.0/src/python_minifier/transforms/remove_literal_statements.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/remove_object_base.py` & `python_minifier-2.9.0/src/python_minifier/transforms/remove_object_base.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/remove_pass.py` & `python_minifier-2.9.0/src/python_minifier/transforms/remove_pass.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/transforms/suite_transformer.py` & `python_minifier-2.9.0/src/python_minifier/transforms/suite_transformer.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier/util.py` & `python_minifier-2.9.0/src/python_minifier/util.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/src/python_minifier.egg-info/PKG-INFO` & `python_minifier-2.9.0/src/python_minifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-minifier
-Version: 2.8.1
+Version: 2.9.0
 Summary: Transform Python source code into it's most compact representation
 Home-page: https://github.com/dflook/python-minifier
 Author: Daniel Flook
 Author-email: daniel@flook.org
 License: MIT
 Project-URL: Issues, https://github.com/dflook/python-minifier/issues
 Project-URL: Documentation, https://dflook.github.io/python-minifier/
```

### Comparing `python_minifier-2.8.1/src/python_minifier.egg-info/SOURCES.txt` & `python_minifier-2.9.0/src/python_minifier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/python_minifier/__main__.py
 src/python_minifier/ast_compare.py
 src/python_minifier/expression_printer.py
 src/python_minifier/f_string.py
 src/python_minifier/ministring.py
 src/python_minifier/module_printer.py
 src/python_minifier/py.typed
+src/python_minifier/token_printer.py
 src/python_minifier/util.py
 src/python_minifier.egg-info/PKG-INFO
 src/python_minifier.egg-info/SOURCES.txt
 src/python_minifier.egg-info/dependency_links.txt
 src/python_minifier.egg-info/entry_points.txt
 src/python_minifier.egg-info/top_level.txt
 src/python_minifier.egg-info/zip-safe
@@ -27,36 +28,39 @@
 src/python_minifier/rename/resolve_names.py
 src/python_minifier/rename/util.py
 src/python_minifier/transforms/__init__.py
 src/python_minifier/transforms/combine_imports.py
 src/python_minifier/transforms/remove_annotations.py
 src/python_minifier/transforms/remove_asserts.py
 src/python_minifier/transforms/remove_debug.py
+src/python_minifier/transforms/remove_explicit_return_none.py
 src/python_minifier/transforms/remove_literal_statements.py
 src/python_minifier/transforms/remove_object_base.py
 src/python_minifier/transforms/remove_pass.py
 src/python_minifier/transforms/remove_posargs.py
 src/python_minifier/transforms/suite_transformer.py
 test/test_assignment_expressions.py
 test/test_await_fstring.py
 test/test_combine_imports.py
 test/test_comprehension_rename.py
 test/test_decorator_expressions.py
 test/test_dict_expansion.py
 test/test_empty_fstring.py
 test/test_hoist_literals.py
+test/test_import.py
 test/test_iterable_unpacking.py
 test/test_match.py
 test/test_match_rename.py
 test/test_name_generator.py
 test/test_nonlocal.py
 test/test_posargs.py
 test/test_preserve_shebang.py
 test/test_remove_annotations.py
 test/test_remove_assert.py
 test/test_remove_debug.py
+test/test_remove_explicit_return_none.py
 test/test_remove_literal_statements.py
 test/test_remove_object.py
 test/test_remove_pass.py
 test/test_rename_builtins.py
 test/test_rename_locals.py
 test/test_slice.py
```

### Comparing `python_minifier-2.8.1/test/test_assignment_expressions.py` & `python_minifier-2.9.0/test/test_assignment_expressions.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_combine_imports.py` & `python_minifier-2.9.0/test/test_combine_imports.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_comprehension_rename.py` & `python_minifier-2.9.0/test/test_comprehension_rename.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_decorator_expressions.py` & `python_minifier-2.9.0/test/test_decorator_expressions.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_dict_expansion.py` & `python_minifier-2.9.0/test/test_dict_expansion.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_hoist_literals.py` & `python_minifier-2.9.0/test/test_hoist_literals.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_iterable_unpacking.py` & `python_minifier-2.9.0/test/test_iterable_unpacking.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_match.py` & `python_minifier-2.9.0/test/test_match.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_match_rename.py` & `python_minifier-2.9.0/test/test_match_rename.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_nonlocal.py` & `python_minifier-2.9.0/test/test_nonlocal.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_posargs.py` & `python_minifier-2.9.0/test/test_posargs.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_preserve_shebang.py` & `python_minifier-2.9.0/test/test_preserve_shebang.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_remove_annotations.py` & `python_minifier-2.9.0/test/test_remove_annotations.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_remove_assert.py` & `python_minifier-2.9.0/test/test_remove_assert.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_remove_debug.py` & `python_minifier-2.9.0/test/test_remove_debug.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_remove_literal_statements.py` & `python_minifier-2.9.0/test/test_remove_literal_statements.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_remove_object.py` & `python_minifier-2.9.0/test/test_remove_object.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_remove_pass.py` & `python_minifier-2.9.0/test/test_remove_pass.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_rename_builtins.py` & `python_minifier-2.9.0/test/test_rename_builtins.py`

 * *Files identical despite different names*

### Comparing `python_minifier-2.8.1/test/test_rename_locals.py` & `python_minifier-2.9.0/test/test_rename_locals.py`

 * *Files identical despite different names*

