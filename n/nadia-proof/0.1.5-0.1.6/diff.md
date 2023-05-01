# Comparing `tmp/nadia-proof-0.1.5.tar.gz` & `tmp/nadia-proof-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadia-proof-0.1.5.tar", last modified: Wed Mar  8 00:16:25 2023, max compression
+gzip compressed data, was "nadia-proof-0.1.6.tar", last modified: Mon May  1 15:18:16 2023, max compression
```

## Comparing `nadia-proof-0.1.5.tar` & `nadia-proof-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:25.097348 nadia-proof-0.1.5/
--rw-rw-rw-   0        0        0     4898 2023-03-08 00:16:25.095078 nadia-proof-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4311 2023-03-08 00:14:38.000000 nadia-proof-0.1.5/README.md
--rw-rw-rw-   0        0        0     1094 2022-11-18 21:07:18.000000 nadia-proof-0.1.5/license.txt
--rw-rw-rw-   0        0        0       42 2023-03-08 00:16:25.098080 nadia-proof-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-03-08 00:16:04.000000 nadia-proof-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:25.045079 nadia-proof-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:25.072079 nadia-proof-0.1.5/src/nadia/
--rw-rw-rw-   0        0        0        0 2022-12-10 02:04:46.000000 nadia-proof-0.1.5/src/nadia/__init__.py
--rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 nadia-proof-0.1.5/src/nadia/example_theorems.py
--rw-rw-rw-   0        0        0     1498 2023-01-02 23:26:43.000000 nadia-proof-0.1.5/src/nadia/nadia_pt.py
--rw-rw-rw-   0        0        0      301 2022-12-10 02:00:41.000000 nadia-proof-0.1.5/src/nadia/nadia_pt_basic_usage.py
--rw-rw-rw-   0        0        0   119397 2023-03-08 00:12:28.000000 nadia-proof-0.1.5/src/nadia/nadia_pt_fo.py
--rw-rw-rw-   0        0        0    18420 2023-03-08 00:12:28.000000 nadia-proof-0.1.5/src/nadia/nadia_pt_gui.py
-drwxrwxrwx   0        0        0        0 2023-03-08 00:16:25.093078 nadia-proof-0.1.5/src/nadia_proof.egg-info/
--rw-rw-rw-   0        0        0     4898 2023-03-08 00:16:24.000000 nadia-proof-0.1.5/src/nadia_proof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-03-08 00:16:24.000000 nadia-proof-0.1.5/src/nadia_proof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 00:16:24.000000 nadia-proof-0.1.5/src/nadia_proof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-03-08 00:16:24.000000 nadia-proof-0.1.5/src/nadia_proof.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-08 00:16:24.000000 nadia-proof-0.1.5/src/nadia_proof.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 15:18:16.029686 nadia-proof-0.1.6/
+-rw-rw-rw-   0        0        0     4898 2023-05-01 15:18:16.027686 nadia-proof-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4311 2023-03-08 00:14:38.000000 nadia-proof-0.1.6/README.md
+-rw-rw-rw-   0        0        0     1094 2022-11-18 21:07:18.000000 nadia-proof-0.1.6/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 15:18:16.029686 nadia-proof-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-05-01 14:58:48.000000 nadia-proof-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:18:15.959688 nadia-proof-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 15:18:15.985686 nadia-proof-0.1.6/src/nadia/
+-rw-rw-rw-   0        0        0        0 2023-05-01 15:14:32.000000 nadia-proof-0.1.6/src/nadia/__init__.py
+-rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 nadia-proof-0.1.6/src/nadia/example_theorems.py
+-rw-rw-rw-   0        0        0     1498 2023-05-01 14:59:06.000000 nadia-proof-0.1.6/src/nadia/nadia_pt.py
+-rw-rw-rw-   0        0        0      301 2023-05-01 14:57:00.000000 nadia-proof-0.1.6/src/nadia/nadia_pt_basic_usage.py
+-rw-rw-rw-   0        0        0   121044 2023-05-01 15:01:54.000000 nadia-proof-0.1.6/src/nadia/nadia_pt_fo.py
+-rw-rw-rw-   0        0        0    18420 2023-03-08 00:12:28.000000 nadia-proof-0.1.6/src/nadia/nadia_pt_gui.py
+drwxrwxrwx   0        0        0        0 2023-05-01 15:18:16.025685 nadia-proof-0.1.6/src/nadia_proof.egg-info/
+-rw-rw-rw-   0        0        0     4898 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/top_level.txt
```

### Comparing `nadia-proof-0.1.5/PKG-INFO` & `nadia-proof-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadia-proof
-Version: 0.1.5
+Version: 0.1.6
 Summary: NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/nadia
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Natural Deduction,Teaching Logic,Educational Software
 Platform: UNKNOWN
```

### Comparing `nadia-proof-0.1.5/README.md` & `nadia-proof-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.5/license.txt` & `nadia-proof-0.1.6/license.txt`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.5/setup.py` & `nadia-proof-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='nadia-proof',
-    version='0.1.5',
+    version='0.1.6',
     license='MIT',
     author="Davi Romero de Vasconcelos",
     author_email='daviromero@ufc.br',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/daviromero/nadia',
     description='''NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.''',
```

### Comparing `nadia-proof-0.1.5/src/nadia/example_theorems.py` & `nadia-proof-0.1.6/src/nadia/example_theorems.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.5/src/nadia/nadia_pt.py` & `nadia-proof-0.1.6/src/nadia/nadia_pt.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.5/src/nadia/nadia_pt_fo.py` & `nadia-proof-0.1.6/src/nadia/nadia_pt_fo.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             string = '\\lnot ' + self.formula.toLatex()
         else:
             string = '\\lnot({})'.format(self.formula.toLatex())
         return string   
 
     def toString(self, parentheses= False):
         if parentheses:
-            string = '(~' + self.formula.toString()+')'
+            string = '(~' + self.formula.toString(parentheses=parentheses)+')'
         elif not isinstance(self.formula, BinaryFormula):
             string = '~' + self.formula.toString()
         else:
             string = '~({})'.format(self.formula.toString())
         return string 
 
     def all_variables(self):
@@ -762,14 +762,16 @@
   INVALID_RIGHT_CONJUNCTION = 36
   INVALID_NEGATION = 37
   INVALID_LEFT_OR_RIGHT_DISJUNCTION = 38
   INVALID_LEFT_OR_RIGHT_CONJUNCTION = 39
   IS_NOT_BOTTOM = 40
   INVALID_CONCLUSION_UNIVERSAL_LAST_RULE = 41
   BOX_MUST_HAVE_ONLY_A_VARIABLE = 42
+  INVALID_RULE = 43
+  INVALID_RULE_ONE_REFERENCE = 44
 
 
 ## File ast.py
 hypothesis = {}
 
 def limpaHipotese():
     global hypothesis
@@ -1762,14 +1764,16 @@
             self.symbol_table.insert(hypothesis, p[0])
             if(self.symbol_table.current_scope == "scope_0"):
                 self.has_error = True
                 deduction_result.add_error(self.get_error(constants.HYPOTHESIS_WITHOUT_BOX, formula_result[0], hypothesis))
             return p[0], formula_result[0]
 
 
+
+
         @self.pg.production('step : NUM DOT formula HYPOTHESIS')
         @self.pg.production('step : NUM DOT formula ATOM')
         @self.pg.production('step : NUM DOT OPEN_BRACKET formula ATOM')
         def Wrong_pre_hip(p):
             self.has_error = True
             wrong_rule = WrongDef(p[0].value, p[-2])
             deduction_result.add_error(self.get_error(constants.INVALID_HIP_PRE_WRITE, p[-1], wrong_rule))
@@ -1967,14 +1971,35 @@
             formula_result = p[2]
             formula = formula_result[1]
             allIntrod = ForAllIntroductiontionDef(p[0].value, formula, p[4], p[6])
             self.symbol_table.insert(allIntrod, p[0])
             self.box_latex += "{} & $\\forall i$ {}-{}\\\\\n".format(formula.toLatex(), p[4].value, p[6].value)
             return p[0], formula_result[0]
 
+        @self.pg.production('step : NUM DOT formula IMP_ELIM NUM ')
+        @self.pg.production('step : NUM DOT formula IMP_ELIM NUM DASH NUM')
+        @self.pg.production('step : NUM DOT formula AND_INTROD NUM ')
+        @self.pg.production('step : NUM DOT formula AND_INTROD NUM DASH NUM')
+        @self.pg.production('step : NUM DOT formula NEG_ELIM NUM ')
+        @self.pg.production('step : NUM DOT formula NEG_ELIM NUM DASH NUM')
+        def Wrong_use_conective_references(p):
+            self.has_error = True
+            wrong_rule = WrongDef(p[0].value, p[2])
+            deduction_result.add_error(self.get_error(constants.INVALID_RULE, p[3], wrong_rule))
+            return p[0], p[2]
+
+        @self.pg.production('step : NUM DOT formula AND_ELIM NUM COMMA NUM ')
+        @self.pg.production('step : NUM DOT formula AND_ELIM NUM DASH NUM')
+        def Wrong_use_conective_reference(p):
+            self.has_error = True
+            wrong_rule = WrongDef(p[0].value, p[2])
+            deduction_result.add_error(self.get_error(constants.INVALID_RULE_ONE_REFERENCE, p[3], wrong_rule))
+            return p[0], p[2]
+
+
         @self.pg.production('formula : EXT formula')
         @self.pg.production('formula : ALL formula')
         @self.pg.production('formula : formula OR formula')
         @self.pg.production('formula : formula AND formula')
         @self.pg.production('formula : formula IMPLIE formula')
         @self.pg.production('formula : NOT formula')
         @self.pg.production('formula : ATOM OPEN_PAREN variableslist CLOSE_PAREN')
@@ -2096,15 +2121,19 @@
         elif type_error == constants.INVALID_LEFT_OR_RIGHT_CONJUNCTION:
             erro += "^, A fórmula à direita ou à equerda da fórmula da linha {} deve ser a mesma da fórmula da conclusão da regra.".format(token_error.value)
         elif type_error == constants.NONE_COPY:
             erro += "^, A Fórmula referenciada para cópia não existe."
         elif type_error == constants.COPY_DIFFERENT_FORMULE:
             erro += "^, A Fórmula referenciada para cópia é diferente da definida para essa regra."
         elif type_error == constants.INVALID_HIP_PRE_WRITE:
-            erro += "^, Esperado o termo pre."
+            erro += "^, uma hipótese só pode ser usado no início de uma caixa e é introduzida apenas por uma regra de inferência."
+        elif type_error == constants.INVALID_RULE:
+            erro += "^, a regra {} deve ter duas referências separadas por vírgula.".format(token_error.value)
+        elif type_error == constants.INVALID_RULE_ONE_REFERENCE:
+            erro += "^, a regra {} deve ter uma única referência.".format(token_error.value)
         elif type_error == constants.EXCEDENT_HIP_PRE_WRITE:
             erro += "^, Não é esperado texto depois de pre."
         elif type_error == constants.USING_DESCARTED_RULE:
             erro += "^, a referência a fórmula da linha {} não pode ser utilizada, pois esta fórmula já foi descartada.".format(token_error.value)
         elif type_error == constants.REFERENCED_LINE_NOT_DEFINED:
             erro += "^, a referência a fórmula da linha {} não pode ser utilizada, pois todas as referências devem ocorrer antes desta regra.".format(token_error.value)
         elif type_error == constants.INVALID_SCOPE_DELIMITER:
```

### Comparing `nadia-proof-0.1.5/src/nadia/nadia_pt_gui.py` & `nadia-proof-0.1.6/src/nadia/nadia_pt_gui.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.5/src/nadia_proof.egg-info/PKG-INFO` & `nadia-proof-0.1.6/src/nadia_proof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadia-proof
-Version: 0.1.5
+Version: 0.1.6
 Summary: NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/nadia
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Natural Deduction,Teaching Logic,Educational Software
 Platform: UNKNOWN
```

