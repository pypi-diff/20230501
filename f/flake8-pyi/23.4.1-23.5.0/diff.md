# Comparing `tmp/flake8_pyi-23.4.1.tar.gz` & `tmp/flake8_pyi-23.5.0.tar.gz`

## Comparing `flake8_pyi-23.4.1.tar` & `flake8_pyi-23.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.editorconfig
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.flake8
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/CHANGELOG.md
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    81855 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/pyi.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/scripts/typeshed_primer_download_errors.js
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/scripts/typeshed_primer_post_comment.js
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/check.yml
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/typeshed_primer.yml
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.github/workflows/typeshed_primer_comment.yml
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/aliases.pyi
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/attribute_annotations.pyi
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/calls.pyi
--rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/classdefs.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/comparisons.pyi
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/defaults.pyi
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/defaults_py38.pyi
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/del.pyi
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/emptyclasses.pyi
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/emptyfunctions.pyi
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/exit_methods.pyi
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/forward_refs.pyi
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/forward_refs_annassign.pyi
--rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/imports.pyi
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/names_requiring_values.pyi
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/never_vs_noreturn.pyi
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/pep604_union_types.pyi
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/quotes.pyi
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/sysplatform.pyi
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/sysversioninfo.pyi
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/test_pyi_files.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/type_comments.pyi
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/typevar.pyi
--rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/union_duplicates.pyi
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/unused_things.pyi
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/tests/vanilla_flake8_not_clean_forward_refs.pyi
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/LICENSE
--rw-r--r--   0        0        0    12042 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/README.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/pyproject.toml
--rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 flake8_pyi-23.4.1/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.editorconfig
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.flake8
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14655 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    80868 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/pyi.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.github/scripts/typeshed_primer_download_errors.js
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.github/scripts/typeshed_primer_post_comment.js
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.github/workflows/check.yml
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.github/workflows/typeshed_primer.yml
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.github/workflows/typeshed_primer_comment.yml
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/aliases.pyi
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/attribute_annotations.pyi
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/calls.pyi
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/classdefs.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/comparisons.pyi
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/defaults.pyi
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/defaults_py38.pyi
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/del.pyi
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/emptyclasses.pyi
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/emptyfunctions.pyi
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/exit_methods.pyi
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/forward_refs.pyi
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/forward_refs_annassign.pyi
+-rw-r--r--   0        0        0    10739 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/imports.pyi
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/names_requiring_values.pyi
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/never_vs_noreturn.pyi
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/pep604_union_types.pyi
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/quotes.pyi
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/sysplatform.pyi
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/sysversioninfo.pyi
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/test_pyi_files.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/type_comments.pyi
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/typevar.pyi
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/union_duplicates.pyi
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/unused_things.pyi
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/tests/vanilla_flake8_not_clean_forward_refs.pyi
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/LICENSE
+-rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/README.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 flake8_pyi-23.5.0/PKG-INFO
```

### Comparing `flake8_pyi-23.4.1/.flake8` & `flake8_pyi-23.5.0/.flake8`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/.pre-commit-config.yaml` & `flake8_pyi-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/CHANGELOG.md` & `flake8_pyi-23.5.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,39 @@
 # Change Log
 
+## 23.5.0
+
+* flake8-pyi no longer supports being run with flake8 <5.0.4.
+* The way in which flake8-pyi modifies pyflakes runs has been improved:
+  * When flake8-pyi is installed, pyflakes now correctly recognises an annotation as
+    being equivalent to a binding assignment in a stub file, reducing false
+    positives from flake8's F821 error code.
+  * When flake8-pyi is installed, there are now fewer pyflakes positives from class
+    definitions that have forward references in the bases tuple for the purpose of
+    creating recursive or circular type definitions. These are invalid in `.py` files,
+    but are supported in stub files.
+  * When flake8-pyi is installed, pyflakes will also *complain* about code which (in
+    combination with flake8-pyi) it previously had no issue with. For example, it will
+    now complain about this code:
+
+    ```py
+    class Foo(Bar): ...
+    class Bar: ...
+    ```
+
+    Although the above code is legal in a stub file, it is considered poor style, and
+    the forward reference serves no purpose (there is no recursive or circular
+    definition). As such, it is now disallowed by pyflakes when flake8-pyi is
+    installed.
+
+  Contributed by [tomasr8](https://github.com/tomasr8).
+* Introduce Y056: Various type checkers have different levels of support for method
+  calls on `__all__`. Use `__all__ += ["foo", "bar"]` instead, as this is known to be
+  supported by all major type checkers.
+
 ## 23.4.1
 
 New error codes:
 * Y055: Unions of the form `type[X] | type[Y]` can be simplified to `type[X | Y]`.
   Similarly, `Union[type[X], type[Y]]` can be simplified to `type[Union[X, Y]]`.
   Contributed by [tomasr8](https://github.com/tomasr8).
```

### Comparing `flake8_pyi-23.4.1/CONTRIBUTING.md` & `flake8_pyi-23.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/pyi.py` & `flake8_pyi-23.5.0/pyi.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 from dataclasses import dataclass
 from functools import partial
 from itertools import chain, zip_longest
 from keyword import iskeyword
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, ClassVar, NamedTuple, Union
 
-import flake8  # type: ignore[import]
-from flake8 import checker
+from flake8 import checker  # type: ignore[import]
 from flake8.options.manager import OptionManager  # type: ignore[import]
 from flake8.plugins.pyflakes import FlakesChecker  # type: ignore[import]
-from pyflakes.checker import ClassDefinition, ClassScope, FunctionScope, ModuleScope
+from pyflakes.checker import ModuleScope
 
 if sys.version_info >= (3, 9):
     from ast import unparse
 else:
     from ast_decompiler import decompile
 
     def unparse(node: ast.AST) -> str:
@@ -35,18 +34,17 @@
 
 if TYPE_CHECKING:
     # We don't have typing_extensions as a runtime dependency,
     # but all our annotations are stringized due to __future__ annotations,
     # and mypy thinks typing_extensions is part of the stdlib.
     from typing_extensions import Literal, TypeAlias, TypeGuard
 
-__version__ = "23.4.1"
+__version__ = "23.5.0"
 
 LOG = logging.getLogger("flake8.pyi")
-FLAKE8_MAJOR_VERSION = flake8.__version_info__[0]
 
 if sys.version_info >= (3, 9):
     _SliceContents: TypeAlias = ast.expr
 else:
     _SliceContents: TypeAlias = Union[ast.expr, ast.slice]
 
 
@@ -157,15 +155,49 @@
         # ClassVar deliberately omitted,
         # as it's the only one in this group that should be parameterised.
         # It is special-cased elsewhere.
     }
 )
 
 
+class PyflakesPreProcessor(ast.NodeTransformer):
+    """Transform AST prior to passing it to pyflakes.
+
+    This reduces false positives on recursive class definitions.
+    """
+
+    def visit_ClassDef(self, node: ast.ClassDef) -> ast.ClassDef:
+        self.generic_visit(node)
+        node.bases = [
+            # Remove the subscript to prevent F821 errors from being emitted
+            # for (valid) recursive definitions: Foo[Bar] --> Foo
+            base.value if isinstance(base, ast.Subscript) else base
+            for base in node.bases
+        ]
+        return node
+
+
 class PyiAwareFlakesChecker(FlakesChecker):
+    def __init__(self, tree: ast.AST, *args: Any, **kwargs: Any) -> None:
+        super().__init__(PyflakesPreProcessor().visit(tree), *args, **kwargs)
+
+    @property
+    def annotationsFutureEnabled(self):
+        """pyflakes can already handle forward refs for annotations, but only via
+        `from __future__ import annotations`.
+
+        We don't want to bother including this in every file, so we just set this to `True`.
+        """
+        return True
+
+    @annotationsFutureEnabled.setter
+    def annotationsFutureEnabled(self, value: bool):
+        """Does nothing, as we always want this property to be `True`."""
+        pass
+
     def deferHandleNode(self, node: ast.AST | None, parent) -> None:
         self.deferFunction(lambda: self.handleNode(node, parent))
 
     def ASSIGN(
         self, tree: ast.Assign, omit: str | tuple[str, ...] | None = None
     ) -> None:
         """This is a custom implementation of ASSIGN derived from
@@ -180,106 +212,47 @@
             return
 
         for target in tree.targets:
             self.handleNode(target, tree)
 
         self.deferHandleNode(tree.value, tree)
 
-    def ANNASSIGN(self, node: ast.AnnAssign) -> None:
-        """
-        Annotated assignments don't have annotations evaluated on function
-        scope, hence the custom implementation. Compared to the pyflakes
-        version, we defer evaluation of the annotations (and values on
-        module level).
-        """
-        if node.value:
-            # Only bind the *target* if the assignment has value.
-            # Otherwise it's not really ast.Store and shouldn't silence
-            # UndefinedLocal warnings.
-            self.handleNode(node.target, node)
-        if not isinstance(self.scope, FunctionScope):
-            self.deferHandleNode(node.annotation, node)
-        if node.value:
-            # If the assignment has value, handle the *value*...
-            if isinstance(self.scope, ModuleScope):
-                # ...later (if module scope).
-                self.deferHandleNode(node.value, node)
-            else:
-                # ...now.
-                self.handleNode(node.value, node)
-
     def LAMBDA(self, node: ast.Lambda) -> None:
         """This is likely very brittle, currently works for pyflakes 1.3.0.
 
         Deferring annotation handling depends on the fact that during calls
         to LAMBDA visiting the function's body is already deferred and the
         only eager calls to `handleNode` are for annotations.
         """
         self.handleNode, self.deferHandleNode = self.deferHandleNode, self.handleNode  # type: ignore[method-assign]
         super().LAMBDA(node)
         self.handleNode, self.deferHandleNode = self.deferHandleNode, self.handleNode  # type: ignore[method-assign]
 
-    def CLASSDEF(self, node: ast.ClassDef) -> None:
-        if not isinstance(self.scope, ModuleScope):
-            # This shouldn't be necessary because .pyi files don't nest
-            # scopes much, but better safe than sorry.
-            super().CLASSDEF(node)
-            return
-
-        # What follows is copied from pyflakes 1.3.0. The only changes are the
-        # deferHandleNode calls.
-        for decorator in node.decorator_list:
-            self.handleNode(decorator, node)
-        for baseNode in node.bases:
-            self.deferHandleNode(baseNode, node)
-        for keywordNode in node.keywords:
-            self.deferHandleNode(keywordNode, node)
-        self.pushScope(ClassScope)
-        # doctest does not process doctest within a doctest
-        # classes within classes are processed.
-        if (
-            self.withDoctest
-            and not self._in_doctest()
-            and not isinstance(self.scope, FunctionScope)
-        ):
-            self.deferFunction(lambda: self.handleDoctests(node))
-        for stmt in node.body:
-            self.handleNode(stmt, node)
-        self.popScope()
-        self.addBinding(node, ClassDefinition(node.name, node))
-
     def handleNodeDelete(self, node: ast.AST) -> None:
         """Null implementation.
 
         Lets users use `del` in stubs to denote private names.
         """
         return
 
 
 class PyiAwareFileChecker(checker.FileChecker):
     def run_check(self, plugin, **kwargs: Any) -> Any:
-        if self.filename == "-":
-            filename = self.options.stdin_display_name
-        else:
-            filename = self.filename
-
-        if filename.endswith(".pyi"):
-            log_msg = (
-                f"Replacing FlakesChecker with PyiAwareFlakesChecker while "
-                f"checking {filename!r}"
-            )
-            if FLAKE8_MAJOR_VERSION < 5:
-                if plugin["plugin"] is FlakesChecker:
-                    LOG.info(log_msg)
-                    plugin = dict(plugin)
-                    plugin["plugin"] = PyiAwareFlakesChecker
+        if plugin.obj is FlakesChecker:
+            if self.filename == "-":
+                filename = self.options.stdin_display_name
             else:
-                if plugin.obj is FlakesChecker:
-                    LOG.info(log_msg)
-                    plugin = plugin._replace(obj=PyiAwareFlakesChecker)
+                filename = self.filename
+
+            if filename.endswith(".pyi"):
+                LOG.info(
+                    f"Replacing FlakesChecker with PyiAwareFlakesChecker while "
+                    f"checking {filename!r}"
+                )
+                plugin = plugin._replace(obj=PyiAwareFlakesChecker)
         return super().run_check(plugin, **kwargs)
 
 
 class LegacyNormalizer(ast.NodeTransformer):
     """Transform AST to be consistent across Python versions."""
 
     if sys.version_info < (3, 9):
@@ -1141,14 +1114,20 @@
 
         if _is_NamedTuple(function):
             return self.error(node, Y028)
         elif _is_TypedDict(function):
             if _is_bad_TypedDict(node):
                 self.error(node, Y031)
             return
+        elif (
+            isinstance(function, ast.Attribute)
+            and isinstance(function.value, ast.Name)
+            and function.value.id == "__all__"
+        ):
+            return self.error(node, Y056.format(method=f".{function.attr}()"))
 
         # String literals can appear in positional arguments for
         # TypeVar definitions.
         with self.string_literals_allowed.enabled():
             for arg in node.args:
                 self.visit(arg)
         # But in keyword arguments they're most likely TypeVar bounds,
@@ -2123,7 +2102,11 @@
 Y052 = 'Y052 Need type annotation for "{variable}"'
 Y053 = "Y053 String and bytes literals >50 characters long are not permitted"
 Y054 = (
     "Y054 Numeric literals with a string representation "
     ">10 characters long are not permitted"
 )
 Y055 = 'Y055 Multiple "type[Foo]" members in a union. {suggestion}'
+Y056 = (
+    'Y056 Calling "{method}" on "__all__" may not be supported by all type checkers '
+    "(use += instead)"
+)
```

### Comparing `flake8_pyi-23.4.1/.github/scripts/typeshed_primer_download_errors.js` & `flake8_pyi-23.5.0/.github/scripts/typeshed_primer_download_errors.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/.github/scripts/typeshed_primer_post_comment.js` & `flake8_pyi-23.5.0/.github/scripts/typeshed_primer_post_comment.js`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/.github/workflows/check.yml` & `flake8_pyi-23.5.0/.github/workflows/check.yml`

 * *Files 17% similar despite different names*

```diff
@@ -68,24 +68,7 @@
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
           cache-dependency-path: pyproject.toml
       - run: pip install -e .[dev]
       - run: python3 -m pytest -vv
-
-  tests-flake8-v4:
-    name: pytest suite with flake8 v4
-    timeout-minutes: 10
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          # Run on Python 3.7, as the importlib_metadata compatibility problems with flake8 v5
-          # are much less on Python 3.8+, where importlib.metadata is available in the stdlib
-          python-version: 3.7
-          cache: pip
-          cache-dependency-path: pyproject.toml
-      - run: pip install "flake8<5"
-      - run: pip install -e .[dev]
-      - run: python3 -m pytest -vv
```

### Comparing `flake8_pyi-23.4.1/.github/workflows/publish.yml` & `flake8_pyi-23.5.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/.github/workflows/typeshed_primer.yml` & `flake8_pyi-23.5.0/.github/workflows/typeshed_primer.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/.github/workflows/typeshed_primer_comment.yml` & `flake8_pyi-23.5.0/.github/workflows/typeshed_primer_comment.yml`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/aliases.pyi` & `flake8_pyi-23.5.0/tests/aliases.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/attribute_annotations.pyi` & `flake8_pyi-23.5.0/tests/attribute_annotations.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/calls.pyi` & `flake8_pyi-23.5.0/tests/calls.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -28,7 +28,12 @@
 D = typing_extensions.TypedDict("C", {'while': bytes, 'for': int})
 E = TypedDict("D", {'[][]': dict[str, int]})
 F = TypedDict("E", {'1': list[str], '2': str})
 
 class ClassBased(TypedDict):
     foo: str
     bar: int
+
+__all__ = ["T", "U", "S"]
+__all__.append("W")  # Y056 Calling ".append()" on "__all__" may not be supported by all type checkers (use += instead)
+__all__.extend(["B", "WithTotal"])  # Y056 Calling ".extend()" on "__all__" may not be supported by all type checkers (use += instead)
+__all__.remove("U")  # Y056 Calling ".remove()" on "__all__" may not be supported by all type checkers (use += instead)
```

### Comparing `flake8_pyi-23.4.1/tests/classdefs.pyi` & `flake8_pyi-23.5.0/tests/classdefs.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/defaults.pyi` & `flake8_pyi-23.5.0/tests/defaults.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/emptyfunctions.pyi` & `flake8_pyi-23.5.0/tests/emptyfunctions.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/exit_methods.pyi` & `flake8_pyi-23.5.0/tests/exit_methods.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/imports.pyi` & `flake8_pyi-23.5.0/tests/imports.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/names_requiring_values.pyi` & `flake8_pyi-23.5.0/tests/names_requiring_values.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/never_vs_noreturn.pyi` & `flake8_pyi-23.5.0/tests/never_vs_noreturn.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/pep604_union_types.pyi` & `flake8_pyi-23.5.0/tests/pep604_union_types.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/quotes.pyi` & `flake8_pyi-23.5.0/tests/quotes.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import typing
 from typing import Annotated, Literal, TypeAlias, TypeVar
 
 import typing_extensions
 
 __all__ = ["f", "g"]
 __all__ += ["h"]
-__all__.extend(["i"])
-__all__.append("j")
-__all__.remove("j")
+__all__.extend(["i"])  # Y056 Calling ".extend()" on "__all__" may not be supported by all type checkers (use += instead)
+__all__.append("j")  # Y056 Calling ".append()" on "__all__" may not be supported by all type checkers (use += instead)
+__all__.remove("j")  # Y056 Calling ".remove()" on "__all__" may not be supported by all type checkers (use += instead)
 __match_args__ = ('foo',)  # Y052 Need type annotation for "__match_args__"
 __slots__ = ('foo',)  # Y052 Need type annotation for "__slots__"
 
 def f(x: "int"): ...  # Y020 Quoted annotations should never be used in stubs
 def g(x: list["int"]): ...  # Y020 Quoted annotations should never be used in stubs
 _T = TypeVar("_T", bound="int")  # Y020 Quoted annotations should never be used in stubs
 def h(w: Literal["a", "b"], x: typing.Literal["c"], y: typing_extensions.Literal["d"], z: _T) -> _T: ...
```

### Comparing `flake8_pyi-23.4.1/tests/sysversioninfo.pyi` & `flake8_pyi-23.5.0/tests/sysversioninfo.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/test_pyi_files.py` & `flake8_pyi-23.5.0/tests/test_pyi_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,22 @@
         error_codes = list(re.finditer(r"# ([A-Z]\d\d\d )", line))
 
         for match, next_match in zip_longest(error_codes, error_codes[1:]):
             end_pos = len(line) if next_match is None else next_match.start()
             message = line[match.end() : end_pos].strip()
             expected_output += f"{path}:{lineno}: {match.group(1)}{message}\n"
 
+    bad_flag_msg = (
+        "--ignore flags in test files override the .flake8 config file. "
+        "Use --extend-ignore instead."
+    )
+    for flag in flags:
+        option = flag.split("=")[0]
+        assert option != "--ignore", bad_flag_msg
+
     run_results = [
         # Passing a file on command line
         subprocess.run(
             ["flake8", "-j0", *flags, path],
             env={**os.environ, "PYTHONPATH": "."},
             stdout=subprocess.PIPE,
         ),
```

### Comparing `flake8_pyi-23.4.1/tests/type_comments.pyi` & `flake8_pyi-23.5.0/tests/type_comments.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/typevar.pyi` & `flake8_pyi-23.5.0/tests/typevar.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/union_duplicates.pyi` & `flake8_pyi-23.5.0/tests/union_duplicates.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/tests/unused_things.pyi` & `flake8_pyi-23.5.0/tests/unused_things.pyi`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/.gitignore` & `flake8_pyi-23.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/LICENSE` & `flake8_pyi-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_pyi-23.4.1/README.md` & `flake8_pyi-23.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 | Y049 | A private `TypedDict` should be used at least once in the file in which it is defined.
 | Y050 | Prefer `typing_extensions.Never` over `typing.NoReturn` for argument annotations. This is a purely stylistic choice in the name of readability.
 | Y051 | Y051 detects redundant unions between `Literal` types and builtin supertypes. For example, `Literal[5]` is redundant in the union `int \| Literal[5]`, and `Literal[True]` is redundant in the union `Literal[True] \| bool`.
 | Y052 | Y052 disallows assignments to constant values where the assignment does not have a type annotation. For example, `x = 0` in the global namespace is ambiguous in a stub, as there are four different types that could be inferred for the variable `x`: `int`, `Final[int]`, `Literal[0]`, or `Final[Literal[0]]`. Enum members are excluded from this check, as are various special assignments such as `__all__` and `__match_args__`.
 | Y053 | Only string and bytes literals <=50 characters long are permitted.
 | Y054 | Only numeric literals with a string representation <=10 characters long are permitted.
 | Y055 | Unions of the form `type[X] \| type[Y]` can be simplified to `type[X \| Y]`. Similarly, `Union[type[X], type[Y]]` can be simplified to `type[Union[X, Y]]`.
+| Y056 | Do not call methods such as `.append()`, `.extend()` or `.remove()` on `__all__`. Different type checkers have varying levels of support for calling these methods on `__all__`. Use `+=` instead, which is known to be supported by all major type checkers.
 
 Note that several error codes recommend using types from `typing_extensions` or
 `_typeshed`. Strictly speaking, these packages are not part of the standard
 library. However, these packages are included in typeshed's `stdlib/`
 directory, meaning that type checkers believe them to be part of the standard
 library even if this does not reflect the reality at runtime. As such, since
 stubs are never executed at runtime, types from `typing_extensions` and
```

### Comparing `flake8_pyi-23.4.1/pyproject.toml` & `flake8_pyi-23.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 dependencies = [
-    "flake8 >= 3.2.1, < 7.0.0",
+    "flake8 >= 5.0.4, < 7.0.0",
     "pyflakes >= 2.1.1",
     "ast-decompiler >= 0.7.0, < 1.0; python_version < '3.9'",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/PyCQA/flake8-pyi"
 "Source" = "https://github.com/PyCQA/flake8-pyi"
```

### Comparing `flake8_pyi-23.4.1/PKG-INFO` & `flake8_pyi-23.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-pyi
-Version: 23.4.1
+Version: 23.5.0
 Summary: A plugin for flake8 to enable linting .pyi stub files.
 Project-URL: Homepage, https://github.com/PyCQA/flake8-pyi
 Project-URL: Source, https://github.com/PyCQA/flake8-pyi
 Project-URL: Bug Tracker, https://github.com/PyCQA/flake8-pyi/issues
 Project-URL: Changelog, https://github.com/PyCQA/flake8-pyi/blob/main/CHANGELOG.md
 Author-email: Łukasz Langa <=lukasz@langa.pl>
 Maintainer: Sebastian Rittau, Akuli, Shantanu
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
 Requires-Dist: ast-decompiler<1.0,>=0.7.0; python_version < '3.9'
-Requires-Dist: flake8<7.0.0,>=3.2.1
+Requires-Dist: flake8<7.0.0,>=5.0.4
 Requires-Dist: pyflakes>=2.1.1
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: flake8-bugbear==23.2.13; extra == 'dev'
 Requires-Dist: flake8-noqa==1.3.0; extra == 'dev'
 Requires-Dist: isort==5.12.0; python_version >= '3.8' and extra == 'dev'
 Requires-Dist: mypy==1.1.1; extra == 'dev'
@@ -128,14 +128,15 @@
 | Y049 | A private `TypedDict` should be used at least once in the file in which it is defined.
 | Y050 | Prefer `typing_extensions.Never` over `typing.NoReturn` for argument annotations. This is a purely stylistic choice in the name of readability.
 | Y051 | Y051 detects redundant unions between `Literal` types and builtin supertypes. For example, `Literal[5]` is redundant in the union `int \| Literal[5]`, and `Literal[True]` is redundant in the union `Literal[True] \| bool`.
 | Y052 | Y052 disallows assignments to constant values where the assignment does not have a type annotation. For example, `x = 0` in the global namespace is ambiguous in a stub, as there are four different types that could be inferred for the variable `x`: `int`, `Final[int]`, `Literal[0]`, or `Final[Literal[0]]`. Enum members are excluded from this check, as are various special assignments such as `__all__` and `__match_args__`.
 | Y053 | Only string and bytes literals <=50 characters long are permitted.
 | Y054 | Only numeric literals with a string representation <=10 characters long are permitted.
 | Y055 | Unions of the form `type[X] \| type[Y]` can be simplified to `type[X \| Y]`. Similarly, `Union[type[X], type[Y]]` can be simplified to `type[Union[X, Y]]`.
+| Y056 | Do not call methods such as `.append()`, `.extend()` or `.remove()` on `__all__`. Different type checkers have varying levels of support for calling these methods on `__all__`. Use `+=` instead, which is known to be supported by all major type checkers.
 
 Note that several error codes recommend using types from `typing_extensions` or
 `_typeshed`. Strictly speaking, these packages are not part of the standard
 library. However, these packages are included in typeshed's `stdlib/`
 directory, meaning that type checkers believe them to be part of the standard
 library even if this does not reflect the reality at runtime. As such, since
 stubs are never executed at runtime, types from `typing_extensions` and
```

