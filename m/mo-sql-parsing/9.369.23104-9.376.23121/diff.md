# Comparing `tmp/mo_sql_parsing-9.369.23104-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.376.23121-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38189 bytes, number of entries: 13
+Zip file size: 38165 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2597 b- defN 22-Dec-18 22:41 mo_sql_parsing/__init__.py
 -rw-rw-rw-  2.0 fat    22229 b- defN 23-Mar-26 12:53 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10299 b- defN 23-Apr-14 10:13 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    33510 b- defN 23-Apr-14 10:22 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat    33442 b- defN 23-May-01 12:37 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
 -rw-rw-rw-  2.0 fat    22945 b- defN 23-Apr-14 10:14 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-26 12:53 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Apr-14 10:22 mo_sql_parsing-9.369.23104.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Apr-14 10:22 mo_sql_parsing-9.369.23104.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-14 10:22 mo_sql_parsing-9.369.23104.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-14 10:22 mo_sql_parsing-9.369.23104.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-14 10:22 mo_sql_parsing-9.369.23104.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Apr-14 10:22 mo_sql_parsing-9.369.23104.dist-info/RECORD
-13 files, 128416 bytes uncompressed, 36283 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-May-01 12:37 mo_sql_parsing-9.376.23121.dist-info/RECORD
+13 files, 128348 bytes uncompressed, 36259 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.369.23104.dist-info/LICENSE
+Filename: mo_sql_parsing-9.376.23121.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.369.23104.dist-info/METADATA
+Filename: mo_sql_parsing-9.376.23121.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.369.23104.dist-info/WHEEL
+Filename: mo_sql_parsing-9.376.23121.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.369.23104.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.376.23121.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.369.23104.dist-info/zip-safe
+Filename: mo_sql_parsing-9.376.23121.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.369.23104.dist-info/RECORD
+Filename: mo_sql_parsing-9.376.23121.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -428,25 +428,22 @@
 
         row = (LB + delimited_list(Group(expression)) + RB) / to_row
         values = VALUES + delimited_list(row) / to_values
 
         window_clause = identifier("name") + AS + (identifier | over_clause)("value")
 
         unordered_sql = Group(
-            values
-            | selection
-            + Optional(
-                (FROM + delimited_list(table_source) + ZeroOrMore(join))("from")
-                + Optional(WHERE + expression("where"))
-                + Optional(GROUP_BY + delimited_list(Group(named_column))("groupby"))
-                + (
-                    Optional(HAVING + expression("having"))
-                    & Optional(WINDOW + delimited_list(Group(window_clause))("window"))
-                    & Optional(QUALIFY + expression("qualify"))
-                )
+            (values | selection)
+            + Optional((FROM + delimited_list(table_source) + ZeroOrMore(join))("from"))
+            + Optional(WHERE + expression("where"))
+            + Optional(GROUP_BY + delimited_list(Group(named_column))("groupby"))
+            + (
+                Optional(HAVING + expression("having"))
+                & Optional(WINDOW + delimited_list(Group(window_clause))("window"))
+                & Optional(QUALIFY + expression("qualify"))
             )
         )
 
         with NO_WHITESPACE:
 
             def mult(tokens):
                 amount = tokens["bytes"]
```

## Comparing `mo_sql_parsing-9.369.23104.dist-info/LICENSE` & `mo_sql_parsing-9.376.23121.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.369.23104.dist-info/METADATA` & `mo_sql_parsing-9.376.23121.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.369.23104
+Version: 9.376.23121
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots (==9.368.23092)
+Requires-Dist: mo-dots (==9.376.23121)
 Requires-Dist: mo-future (==7.340.23006)
 Requires-Dist: mo-imports (==7.365.23080)
-Requires-Dist: mo-parsing (==8.369.23104)
+Requires-Dist: mo-parsing (==8.376.23121)
 Provides-Extra: dev
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-files ; extra == 'tests'
 Requires-Dist: mo-streams ; extra == 'tests'
 Requires-Dist: zstandard ; extra == 'tests'
```

## Comparing `mo_sql_parsing-9.369.23104.dist-info/RECORD` & `mo_sql_parsing-9.376.23121.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=qu67hMKaz6Rn_c0idUNZ9e_BvFuxXsDZRuwQmmGYqpI,2597
 mo_sql_parsing/formatting.py,sha256=wsdY3_OZLlGvZ45VPsVoMX2kE8o1HGE9AoeqQ_fZuMc,22229
 mo_sql_parsing/keywords.py,sha256=j1tlNoH--4y-M_tskfNir2mFoM7Es97I2Nz3T5bX3c0,10299
-mo_sql_parsing/sql_parser.py,sha256=TKomW0-LCUa6yYBi_YeWOXQOxGKxL6_52hIwbkGQyBM,33510
+mo_sql_parsing/sql_parser.py,sha256=uGPQzgvbfuEYLSAenKOzjBlcOBmsU2mpWif61NpbonA,33442
 mo_sql_parsing/types.py,sha256=4nnewHeuD_q3W7muesXsSS4JW73TM17YgBjlxQkOfpo,7321
 mo_sql_parsing/utils.py,sha256=GHwUttxhfFQsCBj4o4BUm0Wu-7r_qhzYqcgnbbdtY1U,22945
 mo_sql_parsing/windows.py,sha256=DNYTT34qFS8lfaDEg4oXigmYoSA72_LyHLgIQjBSpWI,2987
-mo_sql_parsing-9.369.23104.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.369.23104.dist-info/METADATA,sha256=OLONRV6Zmu9JzZ3-sC_SHvEwOffLZ5VQ7G_lhCmKUhA,9345
-mo_sql_parsing-9.369.23104.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.369.23104.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.369.23104.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.369.23104.dist-info/RECORD,,
+mo_sql_parsing-9.376.23121.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.376.23121.dist-info/METADATA,sha256=DBPVabE6vF7qbtL9t0eCH3w2HZL0hpLVe0MjrKpXHa8,9345
+mo_sql_parsing-9.376.23121.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.376.23121.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.376.23121.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.376.23121.dist-info/RECORD,,
```

