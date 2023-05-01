# Comparing `tmp/strawberry_django_plus-2.3.2.tar.gz` & `tmp/strawberry_django_plus-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.3.2.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.4.0.tar", max compression
```

## Comparing `strawberry_django_plus-2.3.2.tar` & `strawberry_django_plus-2.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-04-26 14:24:37.742461 strawberry_django_plus-2.3.2/LICENSE
--rw-r--r--   0        0        0     3299 2023-04-26 14:24:37.742461 strawberry_django_plus-2.3.2/README.md
--rw-r--r--   0        0        0     4162 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5554 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1641 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6287 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14819 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    24443 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27509 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.746461 strawberry_django_plus-2.3.2/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47551 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    16988 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6924 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    12426 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13406 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-04-26 14:24:37.750462 strawberry_django_plus-2.3.2/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/LICENSE
+-rw-r--r--   0        0        0     3299 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/README.md
+-rw-r--r--   0        0        0     4162 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5554 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1641 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-05-01 18:11:23.820150 strawberry_django_plus-2.4.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6287 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14819 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    24443 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27509 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47551 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    17876 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10174 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6924 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    12426 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13406 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-05-01 18:11:23.824150 strawberry_django_plus-2.4.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.4.0/PKG-INFO
```

### Comparing `strawberry_django_plus-2.3.2/LICENSE` & `strawberry_django_plus-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/README.md` & `strawberry_django_plus-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/pyproject.toml` & `strawberry_django_plus-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.3.2"
+version = "2.4.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/field.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.4.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/type.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import dataclasses
+import inspect
+import sys
 import types
 from contextlib import suppress
+from functools import cached_property
 from typing import (
     Callable,
     Literal,
     Optional,
     Sequence,
     Type,
     TypeVar,
@@ -17,15 +20,15 @@
 import strawberry
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRel
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models.base import Model
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
-from strawberry.exceptions import PrivateStrawberryFieldError
+from strawberry.exceptions import MissingFieldAnnotationError, PrivateStrawberryFieldError
 from strawberry.field import UNRESOLVED, StrawberryField
 from strawberry.private import is_private
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.unset import UnsetType
 from strawberry.utils.typing import __dataclass_transform__
 from strawberry_django.fields.field import field as _field
 from strawberry_django.fields.types import get_model_field, resolve_model_field_name
@@ -147,26 +150,39 @@
     # resolve the django_name and check if it is relation field. django_name
     # is used to access the field data in resolvers
     try:
         model_field = get_model_field(
             django_type.model,
             getattr(field, "django_name", None) or name,
         )
-    except FieldDoesNotExist:
+    except FieldDoesNotExist as e:
         model_attr = getattr(django_type.model, name, None)
+        namespace = sys.modules[django_type.model.__module__].__dict__
         if model_attr is not None and isinstance(model_attr, ModelProperty):
             if field.is_auto:
                 annotation = model_attr.type_annotation
                 if get_origin(annotation) is Annotated:
                     annotation = get_args(annotation)[0]
-                field.type_annotation = StrawberryAnnotation(annotation)
+                field.type_annotation = StrawberryAnnotation(annotation, namespace=namespace)
                 field.is_auto = is_auto(field.type_annotation)
 
             if field.description is None:
                 field.description = model_attr.description
+        elif model_attr is not None and isinstance(model_attr, (property, cached_property)):
+            func = model_attr.fget if isinstance(model_attr, property) else model_attr.func
+            if field.is_auto:
+                annotations = func.__annotations__
+                if (return_type := annotations.get("return")) is None:
+                    raise MissingFieldAnnotationError(name, origin) from e
+
+                field.type_annotation = StrawberryAnnotation(return_type, namespace=namespace)
+                field.is_auto = is_auto(field.type_annotation)
+
+            if field.description is None and func.__doc__:
+                field.description = inspect.cleandoc(func.__doc__)
         elif field.django_name or field.is_auto:
             raise  # field should exist, reraise caught exception
     else:
         field.is_relation = model_field.is_relation
         if not field.django_name:
             field.django_name = resolve_model_field_name(
                 model_field,
```

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/types.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.4.0/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.3.2/PKG-INFO` & `strawberry_django_plus-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.3.2
+Version: 2.4.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

