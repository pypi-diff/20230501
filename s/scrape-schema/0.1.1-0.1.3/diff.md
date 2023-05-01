# Comparing `tmp/scrape_schema-0.1.1.tar.gz` & `tmp/scrape_schema-0.1.3.tar.gz`

## Comparing `scrape_schema-0.1.1.tar` & `scrape_schema-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/__init__.py
--rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/LICENSE
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/README.md
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 scrape_schema-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    22015 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/parsel.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/parsel.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/README.md
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7805 2020-02-02 00:00:00.000000 scrape_schema-0.1.3/PKG-INFO
```

### Comparing `scrape_schema-0.1.1/scrape_schema/base.py` & `scrape_schema-0.1.3/scrape_schema/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 logger.setLevel(logging.DEBUG)
 _formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(message)s")
 _stdout_handler = logging.StreamHandler()
 _stdout_handler.setFormatter(_formatter)
 logger.addHandler(_stdout_handler)
 
 T = TypeVar("T")
-MARKUP_TYPE: TypeAlias = Union[str, Any]
+MARKUP_TYPE: TypeAlias = Any
 
 
 def extract_fields(markup: MARKUP_TYPE, **fields: "BaseField") -> Dict[str, Any]:
     return {key: field.extract(markup) for key, field in fields.items()}
 
 
 class ABCField(ABC):
@@ -352,14 +352,20 @@
         :return: typed value
         """
         if instance.Config.type_cast:
             if type_annotation := instance.__schema_annotations__.get(name):
                 value = self._cast_type(type_annotation, value)
         return value
 
+    def __repr__(self):
+        return (
+            f"{self.__class__.__name__}(default={self.default}, callback={self.callback}, "
+            f"filter_={self.filter_}, factory={self.factory})"
+        )
+
 
 class BaseSchemaConfig:
     """Schema configuration for BaseSchema
 
     parsers_config: dict[Type[Any], dict[str, Any]] parser classes for usage backend
 
     type_cast: bool usage type casting feature. default True
```

### Comparing `scrape_schema-0.1.1/scrape_schema/callbacks/slax.py` & `scrape_schema-0.1.3/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/scrape_schema/callbacks/soup.py` & `scrape_schema-0.1.3/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/scrape_schema/fields/nested.py` & `scrape_schema-0.1.3/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/scrape_schema/fields/regex.py` & `scrape_schema-0.1.3/scrape_schema/fields/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 **ReMatchDict, ReMatchListDict**
 
 * https://docs.python.org/3.11/library/re.html#re.Match.groupdict
 """
 
 import re
-from typing import Any, Callable, Dict, List, Optional, Pattern, Union
+from typing import Any, Callable, Dict, List, Optional, Pattern, Type, Union, overload
 
 from ..base import BaseField
 
 __all__ = ["ReMatch", "ReMatchList", "ReMatchDict", "ReMatchListDict"]
 
 
 class ReMatch(BaseField):
```

### Comparing `scrape_schema-0.1.1/scrape_schema/fields/slax.py` & `scrape_schema-0.1.3/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/scrape_schema/fields/soup.py` & `scrape_schema-0.1.3/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/.gitignore` & `scrape_schema-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/LICENSE` & `scrape_schema-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.1.1/README.md` & `scrape_schema-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 ```
 
 add selectolax fields
 ```shell
 pip install scrape-schema[selectolax]
 ```
 
+add parsel fields
+```shell
+pip install scrape-schema[parsel]
+```
+
 add all fields
 ```shell
 pip install scrape-schema[all]
 ```
 ____
 # Code comparison
 Before scrape_schema: harder to maintain, change logic
@@ -109,40 +114,40 @@
     #  'words_lower': ['banana', 'potato', 'foo',
     #                  'bar', 'lorem', 'upsum',
     #                  'dolor'],
     #  'words_upper': ['BANANA', 'POTATO']}
 ```
 After scrape_schema: easy change of logic, support, portability
 ```python
-from typing import Annotated
+from typing import List  # if you usage python3.8 - usage GenericAliases
 import pprint
 
-from scrape_schema import BaseSchema
+from scrape_schema import BaseSchema, ScField
 from scrape_schema.fields.regex import ReMatch, ReMatchList
 
 TEXT = """
 banana potato BANANA POTATO
 -foo:10
 -bar:20
 lorem upsum dolor
 192.168.0.1
 """
 
 
 class Schema(BaseSchema):
-    ipv4: Annotated[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
-    max_digit: Annotated[int, ReMatchList(r"(\d+)",
+    ipv4: ScField[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
+    max_digit: ScField[int, ReMatchList(r"(\d+)",
                                           callback=int,                                      
                                           factory=max)]
-    failed_value: Annotated[bool, ReMatchList(r"(ora)", default=False)]
-    digits: Annotated[list[int], ReMatchList(r"(\d+)")]
-    digits_float: Annotated[list[float], ReMatchList(r"(\d+)", 
+    failed_value: ScField[bool, ReMatchList(r"(ora)", default=False)]
+    digits: ScField[List[int], ReMatchList(r"(\d+)")]
+    digits_float: ScField[List[float], ReMatchList(r"(\d+)", 
                                                      callback=lambda s: f"{s}.5")]
-    words_lower: Annotated[list[str], ReMatchList(r"([a-z]+)")]
-    words_upper: Annotated[list[str], ReMatchList(r"([A-Z]+)")]
+    words_lower: ScField[List[str], ReMatchList(r"([a-z]+)")]
+    words_upper: ScField[List[str], ReMatchList(r"([A-Z]+)")]
     
 if __name__ == '__main__':
     schema = Schema(TEXT)
     pprint.pprint(schema.dict(), width=48, compact=True)
     # {'digits': [10, 20, 192, 168, 0, 1],
     #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5,
     #                   1.5],
```

### Comparing `scrape_schema-0.1.1/pyproject.toml` & `scrape_schema-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -33,16 +33,18 @@
 Source = "https://github.com/vypivshiy/scrape-schema"
 Examples = "https://github.com/vypivshiy/scrape-schema/examples"
 
 
 [project.optional-dependencies]
 selectolax = ["selectolax"]
 bs4 = ["bs4"]
-all = ["selectolax", "bs4"]
-dev = ["bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy"]
+parsel = ["parsel"]
+all = ["selectolax", "bs4", "parsel"]
+dev = ["bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy", "parsel"]
+ci = ["hatch", "bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy", "parsel"]
 docs = ["mkdocs-material"]
 
 [tool.hatch.version]
 path = "scrape_schema/__init__.py"
 
 [tool.hatch.envs.docs]
 dependencies = [
@@ -53,23 +55,24 @@
 build = "mkdocs build --clean --strict"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "selectolax",
-  "bs4"
+  "bs4",
+  "parsel"
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=scrape_schema --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.hatch.build.targets.sdist]
 include = [
   "/README.md",
   "/scrape_schema",
 ]
```

### Comparing `scrape_schema-0.1.1/PKG-INFO` & `scrape_schema-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.1.1
+Version: 0.1.3
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -20,27 +20,41 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: all
 Requires-Dist: bs4; extra == 'all'
+Requires-Dist: parsel; extra == 'all'
 Requires-Dist: selectolax; extra == 'all'
 Provides-Extra: bs4
 Requires-Dist: bs4; extra == 'bs4'
+Provides-Extra: ci
+Requires-Dist: black; extra == 'ci'
+Requires-Dist: bs4; extra == 'ci'
+Requires-Dist: flake8; extra == 'ci'
+Requires-Dist: hatch; extra == 'ci'
+Requires-Dist: isort; extra == 'ci'
+Requires-Dist: mypy; extra == 'ci'
+Requires-Dist: parsel; extra == 'ci'
+Requires-Dist: pytest; extra == 'ci'
+Requires-Dist: selectolax; extra == 'ci'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bs4; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: parsel; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: selectolax; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == 'docs'
+Provides-Extra: parsel
+Requires-Dist: parsel; extra == 'parsel'
 Provides-Extra: selectolax
 Requires-Dist: selectolax; extra == 'selectolax'
 Description-Content-Type: text/markdown
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
 ![CI](https://github.com/vypivshiy/scrape_schema/actions/workflows/ci.yml/badge.svg)
@@ -90,14 +104,19 @@
 ```
 
 add selectolax fields
 ```shell
 pip install scrape-schema[selectolax]
 ```
 
+add parsel fields
+```shell
+pip install scrape-schema[parsel]
+```
+
 add all fields
 ```shell
 pip install scrape-schema[all]
 ```
 ____
 # Code comparison
 Before scrape_schema: harder to maintain, change logic
@@ -152,40 +171,40 @@
     #  'words_lower': ['banana', 'potato', 'foo',
     #                  'bar', 'lorem', 'upsum',
     #                  'dolor'],
     #  'words_upper': ['BANANA', 'POTATO']}
 ```
 After scrape_schema: easy change of logic, support, portability
 ```python
-from typing import Annotated
+from typing import List  # if you usage python3.8 - usage GenericAliases
 import pprint
 
-from scrape_schema import BaseSchema
+from scrape_schema import BaseSchema, ScField
 from scrape_schema.fields.regex import ReMatch, ReMatchList
 
 TEXT = """
 banana potato BANANA POTATO
 -foo:10
 -bar:20
 lorem upsum dolor
 192.168.0.1
 """
 
 
 class Schema(BaseSchema):
-    ipv4: Annotated[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
-    max_digit: Annotated[int, ReMatchList(r"(\d+)",
+    ipv4: ScField[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
+    max_digit: ScField[int, ReMatchList(r"(\d+)",
                                           callback=int,                                      
                                           factory=max)]
-    failed_value: Annotated[bool, ReMatchList(r"(ora)", default=False)]
-    digits: Annotated[list[int], ReMatchList(r"(\d+)")]
-    digits_float: Annotated[list[float], ReMatchList(r"(\d+)", 
+    failed_value: ScField[bool, ReMatchList(r"(ora)", default=False)]
+    digits: ScField[List[int], ReMatchList(r"(\d+)")]
+    digits_float: ScField[List[float], ReMatchList(r"(\d+)", 
                                                      callback=lambda s: f"{s}.5")]
-    words_lower: Annotated[list[str], ReMatchList(r"([a-z]+)")]
-    words_upper: Annotated[list[str], ReMatchList(r"([A-Z]+)")]
+    words_lower: ScField[List[str], ReMatchList(r"([a-z]+)")]
+    words_upper: ScField[List[str], ReMatchList(r"([A-Z]+)")]
     
 if __name__ == '__main__':
     schema = Schema(TEXT)
     pprint.pprint(schema.dict(), width=48, compact=True)
     # {'digits': [10, 20, 192, 168, 0, 1],
     #  'digits_float': [10.5, 20.5, 192.5, 168.5, 0.5,
     #                   1.5],
```

