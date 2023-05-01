# Comparing `tmp/utillc-0.9.8-py2.py3-none-any.whl.zip` & `tmp/utillc-0.9.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17248 bytes, number of entries: 9
+Zip file size: 17796 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      178 b- defN 22-Jun-29 15:03 utillc/__init__.py
 -rw-rw-r--  2.0 unx     3170 b- defN 22-Jun-27 09:29 utillc/expression.py
--rw-rw-r--  2.0 unx     7096 b- defN 22-Jul-01 13:16 utillc/parsetab.py
+-rw-rw-r--  2.0 unx     7974 b- defN 22-Jul-11 12:31 utillc/parsetab.py
 -rw-rw-r--  2.0 unx     5327 b- defN 22-Jun-17 13:27 utillc/qtp.py
--rw-rw-r--  2.0 unx    37715 b- defN 22-Jul-01 14:03 utillc/utillc.py
--rw-rw-r--  2.0 unx     1185 b- defN 22-Jul-01 14:03 utillc-0.9.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 22-Jul-01 14:03 utillc-0.9.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 22-Jul-01 14:03 utillc-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      664 b- defN 22-Jul-01 14:03 utillc-0.9.8.dist-info/RECORD
-9 files, 55446 bytes uncompressed, 16124 bytes compressed:  70.9%
+-rw-rw-r--  2.0 unx    39608 b- defN 22-Jul-11 12:39 utillc/utillc.py
+-rw-rw-r--  2.0 unx     1185 b- defN 22-Jul-11 12:40 utillc-0.9.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 22-Jul-11 12:40 utillc-0.9.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 22-Jul-11 12:40 utillc-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      664 b- defN 22-Jul-11 12:40 utillc-0.9.9.dist-info/RECORD
+9 files, 58217 bytes uncompressed, 16672 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: utillc/qtp.py
 Comment: 
 
 Filename: utillc/utillc.py
 Comment: 
 
-Filename: utillc-0.9.8.dist-info/METADATA
+Filename: utillc-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: utillc-0.9.8.dist-info/WHEEL
+Filename: utillc-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: utillc-0.9.8.dist-info/top_level.txt
+Filename: utillc-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: utillc-0.9.8.dist-info/RECORD
+Filename: utillc-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## utillc/parsetab.py

```diff
@@ -2,58 +2,62 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'leftPLUSMINUSCOLONleftTIMESDIVIDErightUMINUSCOLON COMMA DIVIDE DIVIDE2 DOT EQUALS LBRACKET LPAREN MINUS NAME NUMBER PLUS RBRACKET RPAREN STRING TIMEStop : expressionsexpressions : expressionexpressions : expressions COMMA expressionexpression : expression PLUS expression\n                  | expression MINUS expression\n                  | expression TIMES expression\n                  | expression EQUALS expression\n                  | expression DIVIDE2 expression\n                  | expression DIVIDE expression name : expression DOT dot_namesexpression : MINUS expression %prec UMINUSexpression : LPAREN expressions RPAREN\n                  | name LBRACKET expressionsBE RBRACKET\n                  | name LPAREN expressionsV RPAREN\n    expression : NUMBERexpression : nameexpression : STRINGdot_names : NAMEdot_names : dot_names DOT NAMEexpressionsBE : expressionsBE : expressionsBEE COMMA expressionsBEexpressionsBE : expressionsBEEexpressionsBEE : expressionsBEE : expressionexpressionsBEE : COLONexpressionsBEE : expression COLON expressionsBEEexpressionsV : expressionsV : expressions name : NAME'
+_lr_signature = 'leftPLUSMINUSCOLONleftTIMESDIVIDErightUMINUSCOLON COMMA DIVIDE DIVIDE2 DOT EKON EKOT EKOX EQUALS FLOAT LBRACKET LPAREN MINUS NAME NUMBER PLUS RBRACKET RPAREN STRING TIMEStop : expressionstop : EKON expressionstop : EKOX expressionstop : EKOT expressionsexpressions : expressionexpressions : expressions COMMA expressionexpression : expression PLUS expression\n                  | expression MINUS expression\n                  | expression TIMES expression\n                  | expression EQUALS expression\n                  | expression DIVIDE2 expression\n                  | expression DIVIDE expression name : expression DOT dot_namesexpression : MINUS expression %prec UMINUSexpression : LPAREN expressions RPAREN\n                  | name LBRACKET expressionsBE RBRACKET\n                  | name LPAREN expressionsV RPAREN\n    expression : NUMBERexpression : FLOATexpression : nameexpression : STRINGdot_names : NAMEdot_names : dot_names DOT NAMEexpressionsBE : expressionsBE : expressionsBEE COMMA expressionsBEexpressionsBE : expressionsBEEexpressionsBEE : expressionsBEE : expressionexpressionsBEE : COLONexpressionsBEE : expression COLON expressionsBEEexpressionsV : expressionsV : expressions name : NAME'
     
-_lr_action_items = {'MINUS':([0,3,4,5,6,7,8,9,10,11,12,13,14,15,16,18,20,21,22,23,24,25,26,27,28,29,30,31,34,39,40,41,42,43,],[4,12,4,4,-16,-15,-17,-29,4,4,4,4,4,4,4,-11,4,4,12,-4,-5,-6,12,12,-9,-10,-18,-12,12,-13,4,4,-14,-19,]),'LPAREN':([0,4,5,6,9,10,11,12,13,14,15,16,20,21,29,30,40,41,43,],[5,5,5,21,-29,5,5,5,5,5,5,5,5,5,-10,-18,5,5,-19,]),'NUMBER':([0,4,5,10,11,12,13,14,15,16,20,21,40,41,],[7,7,7,7,7,7,7,7,7,7,7,7,7,7,]),'STRING':([0,4,5,10,11,12,13,14,15,16,20,21,40,41,],[8,8,8,8,8,8,8,8,8,8,8,8,8,8,]),'NAME':([0,4,5,10,11,12,13,14,15,16,17,20,21,38,40,41,],[9,9,9,9,9,9,9,9,9,9,30,9,9,43,9,9,]),'$end':([1,2,3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,39,42,43,],[0,-1,-2,-16,-15,-17,-29,-11,-3,-4,-5,-6,-7,-8,-9,-10,-18,-12,-13,-14,-19,]),'COMMA':([2,3,6,7,8,9,18,19,20,22,23,24,25,26,27,28,29,30,31,33,34,35,37,39,40,41,42,43,45,],[10,-2,-16,-15,-17,-29,-11,10,-23,-3,-4,-5,-6,-7,-8,-9,-10,-18,-12,40,-24,-25,10,-13,-23,-23,-14,-19,-26,]),'RPAREN':([3,6,7,8,9,18,19,21,22,23,24,25,26,27,28,29,30,31,36,37,39,42,43,],[-2,-16,-15,-17,-29,-11,31,-27,-3,-4,-5,-6,-7,-8,-9,-10,-18,-12,42,-28,-13,-14,-19,]),'PLUS':([3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,34,39,42,43,],[11,-16,-15,-17,-29,-11,11,-4,-5,-6,11,11,-9,-10,-18,-12,11,-13,-14,-19,]),'TIMES':([3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,34,39,42,43,],[13,-16,-15,-17,-29,-11,13,13,13,-6,13,13,-9,-10,-18,-12,13,-13,-14,-19,]),'EQUALS':([3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,34,39,42,43,],[14,-16,-15,-17,-29,-11,14,-4,-5,-6,14,14,-9,-10,-18,-12,14,-13,-14,-19,]),'DIVIDE2':([3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,34,39,42,43,],[15,-16,-15,-17,-29,-11,15,-4,-5,-6,15,15,-9,-10,-18,-12,15,-13,-14,-19,]),'DIVIDE':([3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,34,39,42,43,],[16,-16,-15,-17,-29,-11,16,16,16,-6,16,16,-9,-10,-18,-12,16,-13,-14,-19,]),'DOT':([3,6,7,8,9,18,22,23,24,25,26,27,28,29,30,31,34,39,42,43,],[17,-16,-15,-17,-29,-11,17,-4,-5,-6,17,17,-9,38,-18,-12,17,-13,-14,-19,]),'LBRACKET':([6,9,29,30,43,],[20,-29,-10,-18,-19,]),'COLON':([6,7,8,9,18,20,23,24,25,26,27,28,29,30,31,34,39,40,41,42,43,],[-16,-15,-17,-29,-11,35,-4,-5,-6,-7,-8,-9,-10,-18,-12,41,-13,35,35,-14,-19,]),'RBRACKET':([6,7,8,9,18,20,23,24,25,26,27,28,29,30,31,32,33,34,35,39,40,41,42,43,44,45,],[-16,-15,-17,-29,-11,-20,-4,-5,-6,-7,-8,-9,-10,-18,-12,39,-22,-24,-25,-13,-20,-23,-14,-19,-21,-26,]),}
+_lr_action_items = {'EKON':([0,],[3,]),'EKOX':([0,],[4,]),'EKOT':([0,],[5,]),'MINUS':([0,3,4,5,6,7,8,9,10,11,12,13,14,18,19,20,21,22,23,25,27,28,29,30,31,32,33,34,35,36,37,38,41,46,47,48,49,50,],[7,7,7,7,19,7,7,-20,-18,-19,-21,-33,7,7,7,7,7,7,7,-14,7,7,19,-7,-8,-9,19,19,-12,-13,-22,-15,19,-16,7,7,-17,-23,]),'LPAREN':([0,3,4,5,7,8,9,13,14,18,19,20,21,22,23,27,28,36,37,47,48,50,],[8,8,8,8,8,8,28,-33,8,8,8,8,8,8,8,8,8,-13,-22,8,8,-23,]),'NUMBER':([0,3,4,5,7,8,14,18,19,20,21,22,23,27,28,47,48,],[10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,]),'FLOAT':([0,3,4,5,7,8,14,18,19,20,21,22,23,27,28,47,48,],[11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,]),'STRING':([0,3,4,5,7,8,14,18,19,20,21,22,23,27,28,47,48,],[12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,]),'NAME':([0,3,4,5,7,8,14,18,19,20,21,22,23,24,27,28,45,47,48,],[13,13,13,13,13,13,13,13,13,13,13,13,13,37,13,13,50,13,13,]),'$end':([1,2,6,9,10,11,12,13,15,16,17,25,29,30,31,32,33,34,35,36,37,38,46,49,50,],[0,-1,-5,-20,-18,-19,-21,-33,-2,-3,-4,-14,-6,-7,-8,-9,-10,-11,-12,-13,-22,-15,-16,-17,-23,]),'COMMA':([2,6,9,10,11,12,13,15,16,17,25,26,27,29,30,31,32,33,34,35,36,37,38,40,41,42,44,46,47,48,49,50,52,],[14,-5,-20,-18,-19,-21,-33,14,14,14,-14,14,-27,-6,-7,-8,-9,-10,-11,-12,-13,-22,-15,47,-28,-29,14,-16,-27,-27,-17,-23,-30,]),'RPAREN':([6,9,10,11,12,13,25,26,28,29,30,31,32,33,34,35,36,37,38,43,44,46,49,50,],[-5,-20,-18,-19,-21,-33,-14,38,-31,-6,-7,-8,-9,-10,-11,-12,-13,-22,-15,49,-32,-16,-17,-23,]),'PLUS':([6,9,10,11,12,13,25,29,30,31,32,33,34,35,36,37,38,41,46,49,50,],[18,-20,-18,-19,-21,-33,-14,18,-7,-8,-9,18,18,-12,-13,-22,-15,18,-16,-17,-23,]),'TIMES':([6,9,10,11,12,13,25,29,30,31,32,33,34,35,36,37,38,41,46,49,50,],[20,-20,-18,-19,-21,-33,-14,20,20,20,-9,20,20,-12,-13,-22,-15,20,-16,-17,-23,]),'EQUALS':([6,9,10,11,12,13,25,29,30,31,32,33,34,35,36,37,38,41,46,49,50,],[21,-20,-18,-19,-21,-33,-14,21,-7,-8,-9,21,21,-12,-13,-22,-15,21,-16,-17,-23,]),'DIVIDE2':([6,9,10,11,12,13,25,29,30,31,32,33,34,35,36,37,38,41,46,49,50,],[22,-20,-18,-19,-21,-33,-14,22,-7,-8,-9,22,22,-12,-13,-22,-15,22,-16,-17,-23,]),'DIVIDE':([6,9,10,11,12,13,25,29,30,31,32,33,34,35,36,37,38,41,46,49,50,],[23,-20,-18,-19,-21,-33,-14,23,23,23,-9,23,23,-12,-13,-22,-15,23,-16,-17,-23,]),'DOT':([6,9,10,11,12,13,25,29,30,31,32,33,34,35,36,37,38,41,46,49,50,],[24,-20,-18,-19,-21,-33,-14,24,-7,-8,-9,24,24,-12,45,-22,-15,24,-16,-17,-23,]),'LBRACKET':([9,13,36,37,50,],[27,-33,-13,-22,-23,]),'COLON':([9,10,11,12,13,25,27,30,31,32,33,34,35,36,37,38,41,46,47,48,49,50,],[-20,-18,-19,-21,-33,-14,42,-7,-8,-9,-10,-11,-12,-13,-22,-15,48,-16,42,42,-17,-23,]),'RBRACKET':([9,10,11,12,13,25,27,30,31,32,33,34,35,36,37,38,39,40,41,42,46,47,48,49,50,51,52,],[-20,-18,-19,-21,-33,-14,-24,-7,-8,-9,-10,-11,-12,-13,-22,-15,46,-26,-28,-29,-16,-24,-27,-17,-23,-25,-30,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
 
-_lr_goto_items = {'top':([0,],[1,]),'expressions':([0,5,21,],[2,19,37,]),'expression':([0,4,5,10,11,12,13,14,15,16,20,21,40,41,],[3,18,3,22,23,24,25,26,27,28,34,3,34,34,]),'name':([0,4,5,10,11,12,13,14,15,16,20,21,40,41,],[6,6,6,6,6,6,6,6,6,6,6,6,6,6,]),'dot_names':([17,],[29,]),'expressionsBE':([20,40,],[32,44,]),'expressionsBEE':([20,40,41,],[33,33,45,]),'expressionsV':([21,],[36,]),}
+_lr_goto_items = {'top':([0,],[1,]),'expressions':([0,3,4,5,8,28,],[2,15,16,17,26,44,]),'expression':([0,3,4,5,7,8,14,18,19,20,21,22,23,27,28,47,48,],[6,6,6,6,25,6,29,30,31,32,33,34,35,41,6,41,41,]),'name':([0,3,4,5,7,8,14,18,19,20,21,22,23,27,28,47,48,],[9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,]),'dot_names':([24,],[36,]),'expressionsBE':([27,47,],[39,51,]),'expressionsBEE':([27,47,48,],[40,40,52,]),'expressionsV':([28,],[43,]),}
 
 _lr_goto = {}
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> top","S'",1,None,None,None),
-  ('top -> expressions','top',1,'p_top','utillc.py',124),
-  ('expressions -> expression','expressions',1,'p_expressions_1','utillc.py',128),
-  ('expressions -> expressions COMMA expression','expressions',3,'p_expressions_2','utillc.py',132),
-  ('expression -> expression PLUS expression','expression',3,'p_expression_binop','utillc.py',137),
-  ('expression -> expression MINUS expression','expression',3,'p_expression_binop','utillc.py',138),
-  ('expression -> expression TIMES expression','expression',3,'p_expression_binop','utillc.py',139),
-  ('expression -> expression EQUALS expression','expression',3,'p_expression_binop','utillc.py',140),
-  ('expression -> expression DIVIDE2 expression','expression',3,'p_expression_binop','utillc.py',141),
-  ('expression -> expression DIVIDE expression','expression',3,'p_expression_binop','utillc.py',142),
-  ('name -> expression DOT dot_names','name',3,'p_expression_dot','utillc.py',146),
-  ('expression -> MINUS expression','expression',2,'p_expression_uminus','utillc.py',150),
-  ('expression -> LPAREN expressions RPAREN','expression',3,'p_expression_group','utillc.py',156),
-  ('expression -> name LBRACKET expressionsBE RBRACKET','expression',4,'p_expression_group','utillc.py',157),
-  ('expression -> name LPAREN expressionsV RPAREN','expression',4,'p_expression_group','utillc.py',158),
-  ('expression -> NUMBER','expression',1,'p_expression_number','utillc.py',168),
-  ('expression -> name','expression',1,'p_expression_name','utillc.py',172),
-  ('expression -> STRING','expression',1,'p_expression_string','utillc.py',176),
-  ('dot_names -> NAME','dot_names',1,'p_dot_names_1','utillc.py',180),
-  ('dot_names -> dot_names DOT NAME','dot_names',3,'p_dot_names_2','utillc.py',184),
-  ('expressionsBE -> <empty>','expressionsBE',0,'p_expressionsBE_1','utillc.py',189),
-  ('expressionsBE -> expressionsBEE COMMA expressionsBE','expressionsBE',3,'p_expressionsBE_2','utillc.py',193),
-  ('expressionsBE -> expressionsBEE','expressionsBE',1,'p_expressionsBE_3','utillc.py',197),
-  ('expressionsBEE -> <empty>','expressionsBEE',0,'p_expressionsBEE_0','utillc.py',201),
-  ('expressionsBEE -> expression','expressionsBEE',1,'p_expressionsBEE_1','utillc.py',204),
-  ('expressionsBEE -> COLON','expressionsBEE',1,'p_expressionsBEE_2','utillc.py',207),
-  ('expressionsBEE -> expression COLON expressionsBEE','expressionsBEE',3,'p_expressionsBEE_3','utillc.py',210),
-  ('expressionsV -> <empty>','expressionsV',0,'p_expressionsV_1','utillc.py',215),
-  ('expressionsV -> expressions','expressionsV',1,'p_expressionsV_2','utillc.py',219),
-  ('name -> NAME','name',1,'p_name_1','utillc.py',227),
+  ('top -> expressions','top',1,'p_top','utillc.py',134),
+  ('top -> EKON expressions','top',2,'p_top_1','utillc.py',138),
+  ('top -> EKOX expressions','top',2,'p_top_2','utillc.py',141),
+  ('top -> EKOT expressions','top',2,'p_top_3','utillc.py',145),
+  ('expressions -> expression','expressions',1,'p_expressions_1','utillc.py',149),
+  ('expressions -> expressions COMMA expression','expressions',3,'p_expressions_2','utillc.py',153),
+  ('expression -> expression PLUS expression','expression',3,'p_expression_binop','utillc.py',158),
+  ('expression -> expression MINUS expression','expression',3,'p_expression_binop','utillc.py',159),
+  ('expression -> expression TIMES expression','expression',3,'p_expression_binop','utillc.py',160),
+  ('expression -> expression EQUALS expression','expression',3,'p_expression_binop','utillc.py',161),
+  ('expression -> expression DIVIDE2 expression','expression',3,'p_expression_binop','utillc.py',162),
+  ('expression -> expression DIVIDE expression','expression',3,'p_expression_binop','utillc.py',163),
+  ('name -> expression DOT dot_names','name',3,'p_expression_dot','utillc.py',167),
+  ('expression -> MINUS expression','expression',2,'p_expression_uminus','utillc.py',171),
+  ('expression -> LPAREN expressions RPAREN','expression',3,'p_expression_group','utillc.py',177),
+  ('expression -> name LBRACKET expressionsBE RBRACKET','expression',4,'p_expression_group','utillc.py',178),
+  ('expression -> name LPAREN expressionsV RPAREN','expression',4,'p_expression_group','utillc.py',179),
+  ('expression -> NUMBER','expression',1,'p_expression_number','utillc.py',189),
+  ('expression -> FLOAT','expression',1,'p_expression_float','utillc.py',193),
+  ('expression -> name','expression',1,'p_expression_name','utillc.py',197),
+  ('expression -> STRING','expression',1,'p_expression_string','utillc.py',201),
+  ('dot_names -> NAME','dot_names',1,'p_dot_names_1','utillc.py',205),
+  ('dot_names -> dot_names DOT NAME','dot_names',3,'p_dot_names_2','utillc.py',209),
+  ('expressionsBE -> <empty>','expressionsBE',0,'p_expressionsBE_1','utillc.py',214),
+  ('expressionsBE -> expressionsBEE COMMA expressionsBE','expressionsBE',3,'p_expressionsBE_2','utillc.py',218),
+  ('expressionsBE -> expressionsBEE','expressionsBE',1,'p_expressionsBE_3','utillc.py',222),
+  ('expressionsBEE -> <empty>','expressionsBEE',0,'p_expressionsBEE_0','utillc.py',226),
+  ('expressionsBEE -> expression','expressionsBEE',1,'p_expressionsBEE_1','utillc.py',229),
+  ('expressionsBEE -> COLON','expressionsBEE',1,'p_expressionsBEE_2','utillc.py',232),
+  ('expressionsBEE -> expression COLON expressionsBEE','expressionsBEE',3,'p_expressionsBEE_3','utillc.py',235),
+  ('expressionsV -> <empty>','expressionsV',0,'p_expressionsV_1','utillc.py',240),
+  ('expressionsV -> expressions','expressionsV',1,'p_expressionsV_2','utillc.py',244),
+  ('name -> NAME','name',1,'p_name_1','utillc.py',252),
 ]
```

## utillc/utillc.py

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 from __future__ import print_function
 
 #from utillc.__init__ import *
 
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 utillc_version = __version__
 __all__ = ( 'EKOX', 'EKON', 'STACK', 'EKO', 'TYPE', 'EKOI', 'EKOT', 'EKOH', 'EKOF', 'test', 'Bool', 'ntimes', 'LINE', 'resizeImage', 'count_parameters', 'parse_args')
 #__all__ = ('listp', 'dump', 'parse')
 
 #import pymf
 from datetime import datetime
 import platform
@@ -58,21 +58,24 @@
 # -----------------------------------------------------------------------------
 # calc.py
 #
 # A simple calculator with variables -- all in one file.
 # -----------------------------------------------------------------------------
 
 tokens = (
-    'NAME','NUMBER',
+    'FLOAT', 'NAME','NUMBER', 'EKON', 'EKOX',  'EKOT',
     'PLUS','MINUS','TIMES','DIVIDE','EQUALS',
     'LPAREN','RPAREN', 'COMMA', 'STRING', 'RBRACKET', 'LBRACKET', 'DOT', 'DIVIDE2', "COLON"
     )
 
 # Tokens
 t_COMMA    = r'\,'
+t_EKON    = r'EKON'
+t_EKOX    = r'EKOX'
+t_EKOT    = r'EKOT'
 t_PLUS    = r'\+'
 t_MINUS   = r'-'
 t_COLON   = r':'
 t_TIMES   = r'\*'
 t_DIVIDE  = r'/'
 t_DIVIDE2  = r'//'
 t_EQUALS  = r'=='
@@ -81,14 +84,21 @@
 t_RPAREN  = r'\)'
 t_LBRACKET  = r'\['
 t_RBRACKET  = r'\]'
 t_NAME    = r'[a-zA-Z_][a-zA-Z0-9_]*'
 
 t_STRING  = r'\"([^\\\"]|\\.)*\"' + '|' +  r"\'([^\\\']|\\.)*\'" 
 
+def t_FLOAT(t):
+    #r'\d+\.\d+'
+    # a better regex taking exponents into account:
+    r'[-+]?[0-9]+(\.([0-9]+)?([eE][-+]?[0-9]+)?|[eE][-+]?[0-9]+)'        
+    t.value = float(t.value)
+    return t
+
 def t_NUMBER(t):
     r'\d+'
     try:
         t.value = int(t.value)
     except ValueError:
         print("Integer value too large %d", t.value)
         t.value = 0
@@ -120,14 +130,25 @@
 # dictionary of names
 names = { }
 
 def p_top(t) :
     'top : expressions'
     t[0] = t[1]
 
+def p_top_1(t) :
+    'top : EKON expressions'
+    t[0] = t[2]
+def p_top_2(t) :
+    'top : EKOX expressions'
+    t[0] = t[2]
+    
+def p_top_3(t) :
+    'top : EKOT expressions'
+    t[0] = t[2]
+
 def p_expressions_1(t) :
     'expressions : expression'
     t[0] = t[1]
 
 def p_expressions_2(t) :
     'expressions : expressions COMMA expression'
     t[0] =  ( ',', t[1], t[3])
@@ -164,14 +185,18 @@
     else:
         t[0] = (t[1], '(', t[3])
 
 def p_expression_number(t):
     'expression : NUMBER'
     t[0] = str(t[1])
 
+def p_expression_float(t):
+    'expression : FLOAT'
+    t[0] = str(t[1])
+
 def p_expression_name(t):
     'expression : name'
     t[0] = t[1]
 
 def p_expression_string(t):
     'expression : STRING'
     t[0] = t[1]
@@ -551,50 +576,64 @@
     ppat = pattern + "("
     #print("coucou x =", x)
     #print((prt, n, el()))
 
     if prt :
         loc = str(ff[1]) +  ':' + str(ff[2])
         strng = str(x)
-        preamb = loc + ": " if withprint else ""        
+        preamb = loc + ": " if withprint else ""
         if (ff[4] != None) :
             ids =  str(ff[4][0])
             doublecommainid1 = ('EKOX((' in ids and ('))' in ids))
             #t2 = lambda :  ids.index('))') ==  (len(ids) - 2)
             doublecommainid = doublecommainid1
             if (isinstance(x, tuple) and doublecommainid) or istuple:
-                tk11 = str(ff[4][0]).replace(ppat, '').replace(')\n', '').strip('\n ')
+                tkin = str(ff[4][0])
+                #print("=================AA ", tkin)    
+                #tk11 = tkin.replace(ppat, '').replace(')\n', '').strip('\n ')
+                tk11 = tkin
                 tk1 = tk11.split(',')
-                #print("=================", tk11)
+                #print("=================BBB ", tk11)
                 #print("=================", "\n".join(tk1))
                 try :
                     ppp = parseE(tk11)
-
-                    if pattern == "EKOX" and ppp[0] == "" and ppp[1] == "(" :
+                    #print("jjjjjjjjjjjjj", dump(ppp))
+                    #print(pattern)
+                    #print(ppp)
+                    ppp = ppp[2]
+                    
+                    if pattern in ["EKOX", "EKON"] and ppp[0] == "" and ppp[1] == "(" :
                         ppp = ppp[2]
-
-                    #print("jjjjjjjjjjjjj", expression.dump(tk11))
-
+                    #print(ppp)                        
                     tk = list(map(dump, listp(ppp)))
-
                     if len(tk) == len(list(x)) :
                         tkkkk = str(ff[4][0]).replace(ppat, '').replace(')\n', '').strip('\n ')[1:-1].split(',')                    
                         tkk = ', '.join([sx + ' = ' + str(sv) for sx, sv in zip(tk, list(x))])
                     else :
                         tkk = str(ff[4][0]).replace(ppat, '').replace(')\n', '').strip('\n ') + '=' + inl + pref + strng
-                except :
+                except Exception as ee:
+                    print("exception", ee)
+                    #raise ee
                     tkk=inl + pref + strng
                     try :
                         tkk = str(ff[4][0]).replace(ppat, '').replace(')\n', '').strip('\n ') + '=' + inl + pref + strng
                     except :
                         pass                        
             else :
+                #print("zaza", ff[4][0], ppat)
+                tk11 = ff[4][0]
+                ppp = parseE(tk11)
+                #print("llllllllllll", ppp)
+                #print("jjjjjjjjjjjjj", dump(ppp))
+                #print("ggggggggggggggg", dump(ppp[2]))
+                
                 tkk=inl + pref + strng
                 try :
                     tkk = str(ff[4][0]).replace(ppat, '').replace(')\n', '').strip('\n ') + '=' + inl + pref + strng
+                    tkk = dump(ppp[2]) + '=' + inl + pref + strng
                 except :
                     pass
             if '\n' in strng :
                 strng = '\n' + strng
             r = print1(preamb + tt(loc) + tkk + '.', color=color, noeko=not withprint)
         else:
             r = print1(preamb + tt(loc) + str(ff[3]) + '=' + inl + pref + strng + '.', color=color, noeko= not withprint)
@@ -1152,14 +1191,19 @@
         def topk(self,x,y) :
             return namedtuple("T", "values indices")
     torch = X()
     t2n = lambda x : x
     vv  = bcn = np.ones([4,4,4])
     
     EKON(t2n(torch.topk(bcn[0,:,0], 3).values), t2n(torch.topk(vv[0,:,0], 3).values))
+    EKON(t2n(torch.topk(bcn[0,:,0], 3).indices), t2n(torch.topk(vv[0,:,0], 3).indices))
+
+
+    EKOX(parseEE("t2n(torch.topk(bcn[0,:,0], 3).values), t2n(torch.topk(vv[0,:,0], 3).values)"))
+    EKOX(parseEE("t2n(torch.topk(bcn[0,:,0], 3).indices), t2n(torch.topk(vv[0,:,0], 3).indices)"))
 
     
     EKOX(parseEE("p"))
     EKOX(parseEE("p()"))
     EKOX(parseEE("a+b"))
     EKOX(parseEE("a+b+c"))
     EKOX(parseEE("t[a:b]"))
@@ -1271,19 +1315,39 @@
     torchtopk = lambda x,y : zzz
     
     bcn = np.zeros((2,2,2))
     
     EKON(t2n(torchtopk(bcn[0,:,0], 3).indices))
     EKON(t2n(torchtopk(bcn[0,:,0], 3).indices), t2n(torchtopk(vv[0,:,0], 3).indices))                        
 
+    EKOT(1,2,"33")
+    EKOX(1.2e3)
+    
 
+    import time
+    
+    a=1
+    b=[2,3,4]
+    EKON(a, b)
+    EKOT(a, b)
+    EKO()
+    for i in range(5) :
+        time.sleep(1)
+        EKOX(i)
+    ilm, ecart = 1,2
+    EKON(ilm, ecart)
+    
+    EKON(ilm, ecart)   
+    EKON(a, ecart)  
+    EKON(ecart, a)  
+    EKON(ilm, b)  
+    EKOX(ecart)
+    EKON(ecart)  
     EKOT("success", n=LOG, color=True)
 
-    EKOT(1,2,"33")
-    
 
 def count_parameters(model):
     return sum(p.numel() for p in model.parameters() if p.requires_grad)
 
 def parse_args(configin = {}) :
     parser = argparse.ArgumentParser()
     parser.add_argument("--dataroot", default="/mnt/hd2/data")
```

## Comparing `utillc-0.9.8.dist-info/METADATA` & `utillc-0.9.9.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utillc
-Version: 0.9.8
+Version: 0.9.9
 Summary: a utility for smart logging
 Author: Clovis Heaulier
 Author-email: clovis.heaulier@gmail.com
 License: MIT
 Keywords: logging fstring alternative
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```
