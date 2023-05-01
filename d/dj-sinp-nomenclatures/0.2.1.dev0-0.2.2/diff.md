# Comparing `tmp/dj_sinp_nomenclatures-0.2.1.dev0.tar.gz` & `tmp/dj_sinp_nomenclatures-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_sinp_nomenclatures-0.2.1.dev0.tar", max compression
+gzip compressed data, was "dj_sinp_nomenclatures-0.2.2.tar", max compression
```

## Comparing `dj_sinp_nomenclatures-0.2.1.dev0.tar` & `dj_sinp_nomenclatures-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    34523 2021-07-15 19:58:42.401985 dj_sinp_nomenclatures-0.2.1.dev0/LICENSE
--rw-r--r--   0        0        0      125 2021-07-15 22:15:35.386820 dj_sinp_nomenclatures-0.2.1.dev0/README.rst
--rw-r--r--   0        0        0     1567 2022-11-10 22:51:50.403427 dj_sinp_nomenclatures-0.2.1.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/__init__.py
--rw-r--r--   0        0        0      409 2022-11-08 22:39:01.015894 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/admin.py
--rw-r--r--   0        0        0      167 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/apps.py
--rw-r--r--   0        0        0        0 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/fixtures/.gitkeep
--rw-r--r--   0        0        0   113858 2022-11-08 23:11:20.868875 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/fixtures/initdata.xml
--rw-r--r--   0        0        0     4870 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/migrations/0001_initial.py
--rw-r--r--   0        0        0      354 2021-07-18 21:47:17.467822 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/migrations/0002_alter_source_unique_together.py
--rw-r--r--   0        0        0      455 2022-11-08 22:39:01.015894 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/migrations/0003_rename_item_nomenclature.py
--rw-r--r--   0        0        0        0 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/migrations/__init__.py
--rw-r--r--   0        0        0     3538 2022-11-08 22:54:57.443097 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/models.py
--rw-r--r--   0        0        0        1 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/permissions.py
--rw-r--r--   0        0        0      610 2022-11-08 23:12:04.488744 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/serializers.py
--rw-r--r--   0        0        0       60 2021-07-15 22:15:35.394820 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/tests.py
--rw-r--r--   0        0        0      455 2022-11-10 22:51:22.023442 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/urls.py
--rw-r--r--   0        0        0      905 2022-11-08 22:39:01.015894 dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/views.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-0.2.1.dev0/setup.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-0.2.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-01 19:52:05.721376 dj_sinp_nomenclatures-0.2.2/LICENSE
+-rw-r--r--   0        0        0      125 2023-05-01 19:52:05.721376 dj_sinp_nomenclatures-0.2.2/README.rst
+-rw-r--r--   0        0        0     1917 2023-05-01 19:52:05.725376 dj_sinp_nomenclatures-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 19:52:05.725376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/__init__.py
+-rw-r--r--   0        0        0      391 2023-05-01 19:52:05.725376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/admin.py
+-rw-r--r--   0        0        0      259 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/apps.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/fixtures/.gitkeep
+-rw-r--r--   0        0        0   138850 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/fixtures/initdata.xml
+-rw-r--r--   0        0        0     8571 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/migrations/0002_alter_source_unique_together.py
+-rw-r--r--   0        0        0      454 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/migrations/0003_rename_item_nomenclature.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/migrations/__init__.py
+-rw-r--r--   0        0        0     3660 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/models.py
+-rw-r--r--   0        0        0        0 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/permissions.py
+-rw-r--r--   0        0        0      820 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/serializers.py
+-rw-r--r--   0        0        0     3075 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/tests.py
+-rw-r--r--   0        0        0      513 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/urls.py
+-rw-r--r--   0        0        0     1129 2023-05-01 19:52:05.729376 dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/views.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 dj_sinp_nomenclatures-0.2.2/PKG-INFO
```

### Comparing `dj_sinp_nomenclatures-0.2.1.dev0/LICENSE` & `dj_sinp_nomenclatures-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_sinp_nomenclatures-0.2.1.dev0/pyproject.toml` & `dj_sinp_nomenclatures-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 [tool.poetry]
 name = "dj_sinp_nomenclatures"
-version = "0.2.1-dev"
+version = "0.2.2"
 description = "Django app to manage french SINP nomenclatures standards"
 authors = ["dbChiro project <project@dbchiro.org>"]
 license = "AGPLv3"
 keywords = ["SINP", "Nomenclatures", "Django", "France", "dbChiroWeb"]
 readme = "README.rst"
 homepage = "https://github.com/dbchiro/DjangoSinpNomenclature"
 repository = "https://github.com/dbchiro/DjangoSinpNomenclature"
 include = ["LICENSE"]
 packages = [{ include = "sinp_nomenclatures" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-Django = "^4.1.3"
-djangorestframework = "^3.14.0"
+python = ">=3.8.1,<4.0"
+Django = ">=3.2,<5.0"
+djangorestframework = ">=3.0,<4.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
-pytest = "^5.2"
-isort = "^5.9.2"
-flake8 = "^3.9.2"
-flake8-isort = "^4.0.0"
-pre-commit = "^2.13.0"
+black = "^23.1.0"
+isort = "^5.12.0"
+flake8 = "^6.0.0"
+flake8-isort = "^6.0.0"
+pre-commit = "^3.0.4"
 python-decouple = "^3.4"
-psycopg2-binary = "^2.9.1"
-drf-yasg = "^1.20.0"
+psycopg2-binary = "^2.9.5"
+drf-yasg = "^1.21.5"
+django-fixture-magic = "^0.1.5"
+pygraphviz = "^1.10"
+django-extensions = "^3.2.1"
+flake8-pyproject = "^1.2.2"
+pylint = "^2.16.2"
+pylint-django = "^2.5.3"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.1.1"
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
 rstcheck = "^6.1.0"
 
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2.1"
+coverage = "^7.1.0"
+
 [tool.isort]
 include_trailing_comma = true
 line_length = 79
 multi_line_output = 3
 profile = "black"
 
 [tool.black]
@@ -58,10 +68,18 @@
 )
 '''
 include = '\.pyi?$'
 line-length = 79
 target-version = ['py37']
 
 
+[tool.flake8]
+ignore = ['E231', 'E241', 'E501']
+per-file-ignores = [
+    '__init__.py:F401',
+]
+max-line-length = 79
+count = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dj_sinp_nomenclatures-0.2.1.dev0/sinp_nomenclatures/models.py` & `dj_sinp_nomenclatures-0.2.2/sinp_nomenclatures/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""Django SINP Nomenclatures Models"""
 
 
-from django.db import models
 from django.conf import settings
+from django.db import models
 from django.utils.translation import gettext as _
 
 # Create your models here.
 STATUS_CHOICES = (
     ("VALID", _("Valide")),
     ("FREEZE", _("Gelée")),
 )
 
 
-class BaseModel(models.Model):  # base class should subclass 'django.db.models.Model'
-    """Common shared base model with metadata fields
-    """
+class BaseModel(
+    models.Model
+):  # base class should subclass 'django.db.models.Model'
+    """Common shared base model with metadata fields"""
+
     timestamp_create = models.DateTimeField(auto_now_add=True, editable=False)
     timestamp_update = models.DateTimeField(auto_now=True, editable=False)
     created_by = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         null=True,
         blank=True,
         db_index=True,
@@ -37,76 +40,88 @@
         on_delete=models.SET_NULL,
     )
 
     class Meta:
         abstract = True
 
 
-
 class Source(BaseModel):
     """Source model, giving nomenclature source
 
     Args:
         BaseModel ([type]): [description]
 
     Returns:
         [type]: [description]
     """
+
     name = models.CharField(_("Nom"), max_length=50)
     version = models.CharField(_("Version"), max_length=50)
     create_date = models.DateField(
         _("Date de création officielle"), auto_now=False, auto_now_add=False
     )
     update_date = models.DateField(
-        _("Date de modification officielle"), auto_now=False, auto_now_add=False
+        _("Date de modification officielle"),
+        auto_now=False,
+        auto_now_add=False,
     )
 
     class Meta:
         verbose_name = _("Source de nomenclatures")
         verbose_name_plural = _("Sources de nomenclatures")
-        unique_together = ['name','version']
+        unique_together = ["name", "version"]
 
     def __str__(self):
         return f"{self.name} ({self.version})"
 
+
 class Type(BaseModel):
-    code = models.CharField(_("Code"), unique=True, max_length=50, db_index=True)
+    code = models.CharField(
+        _("Code"), unique=True, max_length=50, db_index=True
+    )
     mnemonic = models.CharField(_("Mnémonique"), unique=True, max_length=50)
     label = models.CharField(_("Libellé"), max_length=50)
-    status = models.CharField(_("Statut"),max_length=50, choices=STATUS_CHOICES)
+    status = models.CharField(
+        _("Statut"), max_length=50, choices=STATUS_CHOICES
+    )
     create_date = models.DateField(
         _("Date de création officielle"), auto_now=False, auto_now_add=False
     )
     update_date = models.DateField(
-        _("Date de modification officielle"), auto_now=False, auto_now_add=False
+        _("Date de modification officielle"),
+        auto_now=False,
+        auto_now_add=False,
     )
     source = models.ForeignKey(
         "Source",
         verbose_name=_("Source"),
         on_delete=models.CASCADE,
         related_name="type_nomenclature",
         blank=True,
-        null=True
+        null=True,
     )
 
     class Meta:
         verbose_name = _("Type de nomenclature")
         verbose_name_plural = _("Types de nomenclatures")
 
     def __str__(self):
         return f"{self.code} - {self.mnemonic}"
 
+
 class Nomenclature(BaseModel):
     type = models.ForeignKey(
         "Type",
         verbose_name=_("Type"),
         on_delete=models.CASCADE,
         related_name="item_nomenclature",
     )
-    code = models.CharField(max_length=255, db_index=True, verbose_name=_("Code"))
+    code = models.CharField(
+        max_length=255, db_index=True, verbose_name=_("Code")
+    )
     mnemonic = models.CharField(_("Mnémonique"), max_length=50)
     label = models.CharField(max_length=255, verbose_name=_("Libellé"))
     description = models.TextField(_("Description"), blank=True, null=True)
     active = models.BooleanField(default=True, verbose_name=_("Est utilisé"))
 
     class Meta:
         verbose_name_plural = _("nomenclatures")
```

### Comparing `dj_sinp_nomenclatures-0.2.1.dev0/PKG-INFO` & `dj_sinp_nomenclatures-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dj-sinp-nomenclatures
-Version: 0.2.1.dev0
+Version: 0.2.2
 Summary: Django app to manage french SINP nomenclatures standards
 Home-page: https://github.com/dbchiro/DjangoSinpNomenclature
 License: AGPLv3
 Keywords: SINP,Nomenclatures,Django,France,dbChiroWeb
 Author: dbChiro project
 Author-email: project@dbchiro.org
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=4.1.3,<5.0.0)
-Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
+Requires-Dist: Django (>=3.2,<5.0)
+Requires-Dist: djangorestframework (>=3.0,<4.0)
 Project-URL: Repository, https://github.com/dbchiro/DjangoSinpNomenclature
 Description-Content-Type: text/x-rst
 
 DjangoSinpNomenclature
 ======================
```

