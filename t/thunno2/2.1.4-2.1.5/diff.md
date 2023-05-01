# Comparing `tmp/thunno2-2.1.4.tar.gz` & `tmp/thunno2-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.4.tar", last modified: Thu Apr 27 09:10:00 2023, max compression
+gzip compressed data, was "thunno2-2.1.5.tar", last modified: Mon May  1 08:32:38 2023, max compression
```

## Comparing `thunno2-2.1.4.tar` & `thunno2-2.1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-27 09:10:00.904464 thunno2-2.1.4/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-27 09:10:00.904352 thunno2-2.1.4/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-27 09:10:00.904498 thunno2-2.1.4/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.4/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-27 09:10:00.903645 thunno2-2.1.4/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.4/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.4/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    51282 2023-04-27 09:09:12.000000 thunno2-2.1.4/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.4/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.4/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     6508 2023-04-17 19:22:08.000000 thunno2-2.1.4/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    50975 2023-04-27 09:09:12.000000 thunno2-2.1.4/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    26276 2023-04-16 17:25:02.000000 thunno2-2.1.4/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    23076 2023-04-16 17:25:02.000000 thunno2-2.1.4/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-16 17:25:02.000000 thunno2-2.1.4/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    71410 2023-04-27 09:09:12.000000 thunno2-2.1.4/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-27 09:09:12.000000 thunno2-2.1.4/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-27 09:09:46.000000 thunno2-2.1.4/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-27 09:10:00.904204 thunno2-2.1.4/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-27 09:10:00.000000 thunno2-2.1.4/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-27 09:10:00.000000 thunno2-2.1.4/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-27 09:10:00.000000 thunno2-2.1.4/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-27 09:10:00.000000 thunno2-2.1.4/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-27 09:10:00.000000 thunno2-2.1.4/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:32:38.086150 thunno2-2.1.5/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 08:32:38.086034 thunno2-2.1.5/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-01 08:32:38.086188 thunno2-2.1.5/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.5/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:32:38.085365 thunno2-2.1.5/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.5/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.5/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.5/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    51654 2023-04-29 19:16:49.000000 thunno2-2.1.5/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.5/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.5/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.5/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    51729 2023-05-01 08:31:39.000000 thunno2-2.1.5/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    27697 2023-04-30 14:45:33.000000 thunno2-2.1.5/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    23408 2023-04-27 13:07:04.000000 thunno2-2.1.5/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-04-30 09:02:54.000000 thunno2-2.1.5/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    72542 2023-04-30 14:45:33.000000 thunno2-2.1.5/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.5/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-01 08:32:19.000000 thunno2-2.1.5/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 08:32:38.085883 thunno2-2.1.5/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-01 08:32:37.000000 thunno2-2.1.5/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.4/PKG-INFO` & `thunno2-2.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.4
+Version: 2.1.5
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.4.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.5.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.4/setup.py` & `thunno2-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.4/thunno2/codepage.py` & `thunno2-2.1.5/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.4/thunno2/commands.py` & `thunno2-2.1.5/thunno2/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1458,20 +1458,32 @@
     ),
 }
 
 list_digraphs = {
     "C": Overload(
         1, {((int, float, str),): pass_, list: centre_list}, 0, ("center", "centre")
     ),
+    ".": Overload(
+        2, {(list, list): dot_product, (Any[0], Any[0]): pass_}, 0, ("dot_product",)
+    ),
     "\\": Overload(
         1, {((int, float, str),): pass_, list: main_diagonal}, 0, ("main_diagonal",)
     ),
     "/": Overload(
         1, {((int, float, str),): pass_, list: anti_diagonal}, 0, ("anti_diagonal",)
     ),
+    "“": Overload(
+        1, {((int, float, str),): pass_, list: all_diagonals}, 0, ("all_diagonals",)
+    ),
+    "”": Overload(
+        1,
+        {((int, float, str),): pass_, list: all_anti_diagonals},
+        0,
+        ("all_anti_diagonals",),
+    ),
 }
 
 random_digraphs_1 = {
     "C": Overload(1, {Any: cosine}, 1, ("cosine", "cos")),
     "D": Overload(1, {Any: degrees}, 1, ("degrees",)),
     "E": Overload(1, {Any: exponent}, 1, ("exponent",)),
     "F": Overload(1, {Any: nth_fibonacci_number}, 1, ("nth_fibonacci_number",)),
```

### Comparing `thunno2-2.1.4/thunno2/constants.py` & `thunno2-2.1.5/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.4/thunno2/dictionary.py` & `thunno2-2.1.5/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.4/thunno2/flags.py` & `thunno2-2.1.5/thunno2/flags.py`

 * *Files 19% similar despite different names*

```diff
@@ -127,14 +127,35 @@
 
         if "b" == flag:
             commands.ctx.stack.push(commands.commands["ɓ"]()[0])
 
         if "!" == flag:
             commands.ctx.stack.push(commands.commands["¬"]()[0])
 
+        if "Ḷ" == flag:
+            a = next(commands.ctx.stack.rmv(1))
+            if isinstance(a, str):
+                commands.ctx.stack.push(a.upper())
+            else:
+                commands.ctx.stack.push(a)
+
+        if "Ṭ" == flag:
+            a = next(commands.ctx.stack.rmv(1))
+            if isinstance(a, str):
+                commands.ctx.stack.push(a.title())
+            else:
+                commands.ctx.stack.push(a)
+
+        if "Ụ" == flag:
+            a = next(commands.ctx.stack.rmv(1))
+            if isinstance(a, str):
+                commands.ctx.stack.push(a.upper())
+            else:
+                commands.ctx.stack.push(a)
+
     if do_print:
         do_printing(flags)
 
 
 def do_printing(flags):
     if (commands.ctx.implicit_print or ("O" in flags)) and not ("o" in flags):
         print(next(commands.ctx.stack.rmv(1)))
```

### Comparing `thunno2-2.1.4/thunno2/helpers.py` & `thunno2-2.1.5/thunno2/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2740,7 +2740,39 @@
     if not l:
         return []
     r = []
     m = min(len(l), min(map(len, l)))
     for i in range(m):
         r.append(l[i][m - i - 1])
     return r
+
+
+def dot_product(x, y):
+    r = []
+    for i, j in zip(x, y):
+        try:
+            r.append(i * j)
+        except:
+            pass
+    return it_sum(r)
+
+
+def all_diagonals(lst):
+    l = [*map(_digits, lst)]
+    if not l:
+        return []
+    r = [[] for _ in range(len(l) + min(map(len, l)) - 1)]
+    for i, x in enumerate(l):
+        for j in range(min(map(len, l))):
+            r[(j - i) % len(r)].append(x[j])
+    return r
+
+
+def all_anti_diagonals(lst):
+    l = [*map(_digits, lst)]
+    if not l:
+        return []
+    r = [[] for _ in range(len(l) + min(map(len, l)) - 1)]
+    for i, x in enumerate(l):
+        for j in range(min(map(len, l))):
+            r[((-i) - j + min(len(l), min(map(len, l))) - 1) % len(r)].append(x[j])
+    return r
```

### Comparing `thunno2-2.1.4/thunno2/interpreter.py` & `thunno2-2.1.5/thunno2/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,18 +220,27 @@
                 + dictionary.dictionary_decompress_string(info[2:]).title()
             )
         elif desc == "compressed number" or desc == "small compressed number":
             base255_number = decompress(info, "»")
             ctx.stack.push(base255_number)
         elif desc == "compressed list":
             base255_number = decompress(info, "¿")
-            decompressed_string = to_custom_base_string(
-                "][0123456789-.,", base255_number
-            )
+            decompressed_string = to_custom_base_string(",.0123456789-", base255_number)
             try:
+                if decompressed_string[:1] == ",":
+                    decompressed_string = "0" + decompressed_string
+                if decompressed_string[-1:] == ",":
+                    decompressed_string += "0"
+                if decompressed_string[:1] == ".":
+                    decompressed_string = ".5" + decompressed_string[1:]
+                if decompressed_string[-1:] == ".":
+                    decompressed_string += "5"
+                decompressed_string = decompressed_string.replace(",,", ",0,").replace(
+                    ",.,", ",.5,"
+                )
                 e = eval(decompressed_string)
                 if isinstance(e, tuple):
                     ctx.stack.push(list(e))
                 else:
                     ctx.stack.push(e)
             except:
                 ctx.stack.push(decompressed_string)
@@ -443,14 +452,19 @@
             print(next(ctx.stack.rmv(1)))
             ctx.implicit_print = False
         elif desc == "print without newline":
             print(next(ctx.stack.rmv(1)), end="")
             ctx.implicit_print = False
         elif desc == "print without popping":
             print((ctx.stack.copy() + ctx.other_il + [0])[0])
+            ctx.implicit_print = False
+        elif desc == "print each":
+            for i in listify(next(ctx.stack.rmv(1))):
+                print(i)
+            ctx.implicit_print = False
         elif desc == "map":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
@@ -610,14 +624,33 @@
                 ctx.stack.push(i)
                 for j in f1():
                     ctx.stack.push(j)
                 for k in f2():
                     ctx.stack.push(k)
                 r.append(next(ctx.stack.rmv(1)))
             ctx.stack.push(r)
+        elif desc == "recursive environment":
+            a = next(ctx.stack.rmv(1))
+            if isinstance(a, list):
+                x = copy.deepcopy(a)
+            else:
+                x = [a]
+            for i in x:
+                print(i)
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            k = 0
+            while True:
+                ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
+                for j in x:
+                    ctx.stack.push(j)
+                run(info, n=([0] + x)[-1], iteration_index=k)
+                y = next(ctx.stack.rmv(1))
+                print(y)
+                x.append(y)
+                k += 1
         else:
             if ctx.warnings:
                 print("TRACEBACK: [UNRECOGNISED TOKEN]", file=sys.stderr)
                 print(f"Got {chars!r} (tokenised to {desc!r})")
     return 0
```

### Comparing `thunno2-2.1.4/thunno2/lexer.py` & `thunno2-2.1.5/thunno2/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,23 @@
         char = code[index]
         if char in commands:
             ret.append((char, "command", commands[char]))
         elif char in DIGRAPHS:
             index += 1
             try:
                 x = code[index]
-                ret.append((char, "digraph", get_a_function(char + x)))
+                y = char + x
+                if y == "µµ":
+                    i, r = tokenise(code[index + 1 :], expected_end=";")
+                    index += i
+                    ret.append((y, "recursive environment", r))
+                elif y == "µ£":
+                    ret.append((y, "print each", 0))
+                else:
+                    ret.append((y, "digraph", get_a_function(y)))
             except:
                 pass
         elif char in "0123456789.":
             s = char
             index += 1
             try:
                 while code[index] in "0123456789.":
```

### Comparing `thunno2-2.1.4/thunno2/run.py` & `thunno2-2.1.5/thunno2/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thunno2 import lexer, version, flags, tokens
+from thunno2 import lexer, version, flags, tokens, autoexplanation
 import sys
 
 
 def from_terminal():
     print("Thunno", version.THUNNO_VERSION, "interpreter\n")
     print("\nFlags:")
     flags_list = input()
@@ -24,14 +24,16 @@
         inp = input()
     inputs = ""
     print("\nInput:")
     inp = input()
     while inp:
         inputs += inp + "\n"
         inp = input()
+    if "e" in flags_list:
+        print("\nExplanation:\n\n" + autoexplanation.auto_explain(code) + "\n")
     if "v" in flags_list:
         transpiled = tokens.transpile(code)
         print("\nTranspiled:")
         print(transpiled)
         print()
         _, tokenised = lexer.tokenise(transpiled)
     else:
@@ -46,16 +48,21 @@
         from_terminal()
         return None
     filename = args[0]
     flags_list = args[1:]
     sys.stderr.write("Thunno, v" + version.THUNNO_VERSION + "\n")
     try:
         with open(filename) as f:
+            code = f.read()
+            if "e" in "".join(flags_list):
+                sys.stderr.write(
+                    "\nExplanation:\n\n" + autoexplanation.auto_explain(code) + "\n"
+                )
             if "v" in "".join(flags_list):
-                transpiled = tokens.transpile(f.read())
+                transpiled = tokens.transpile(code)
                 print("Transpiled:", transpiled, file=sys.stderr)
                 _, tokenised = lexer.tokenise(transpiled)
             else:
-                _, tokenised = lexer.tokenise(f.read())
+                _, tokenised = lexer.tokenise(code)
             flags.run("".join(flags_list), tokenised, sys.stdin.read())
     except Exception as E:
         sys.stderr.write("An error occurred: " + repr(E))
```

### Comparing `thunno2-2.1.4/thunno2/tests.py` & `thunno2-2.1.5/thunno2/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -2721,14 +2721,25 @@
 
 assert_eq(call("ØC", [123, 4567, 8, 90]), "123 \n4567\n 8  \n 90 ")
 assert_eq(
     call("ØC", ["abc", 1234, "xy", 56789, "z"]), " abc \n 1234\n  xy \n56789\n  z  "
 )
 assert_eq(call("ØC", []), "")
 
+# Ø.
+
+assert_eq(call("Ø.", [1, 2, 3], [4, 5, 6]), 32)
+assert_eq(call("Ø.", [123], [456, 789]), 56088)
+assert_eq(call("Ø.", [], [123, 456, 789]), 0)
+
+assert_eq(
+    call("Ø.", [5, 6, 7], ["abc", "def", "ghi"]),
+    "abcabcabcabcabcdefdefdefdefdefdefghighighighighighighi",
+)
+
 # Ø\
 
 assert_eq(call("Ø\\", [123, 456, 789]), [1, 5, 9])
 assert_eq(call("Ø\\", ["abcd", 12345, "xyz", 67]), ["a", 2])
 assert_eq(call("Ø\\", [[123, 456, 789], ["abc", "def", "ghi"]]), [123, "def"])
 assert_eq(call("Ø\\", []), [])
 
@@ -2741,14 +2752,44 @@
 assert_eq(call("Ø/", ["abcd", 12345, "xyz", 67]), ["b", 1])
 assert_eq(call("Ø/", [[123, 456, 789], ["abc", "def", "ghi"]]), [456, "abc"])
 assert_eq(call("Ø/", []), [])
 
 assert_eq(call("Ø/", 123), 123)
 assert_eq(call("Ø/", "abc"), "abc")
 
+# Ø“
+
+assert_eq(call("Ø“", [123, 456, 789]), [[1, 5, 9], [2, 6], [3], [7], [4, 8]])
+assert_eq(
+    call("Ø“", ["abcd", 12345, "xyz", 67]), [["a", 2], ["b"], [6], ["x", 7], [1, "y"]]
+)
+assert_eq(
+    call("Ø“", [[123, 456, 789], ["abc", "def", "ghi"]]),
+    [[123, "def"], [456, "ghi"], [789], ["abc"]],
+)
+assert_eq(call("Ø“", []), [])
+
+assert_eq(call("Ø“", 123), 123)
+assert_eq(call("Ø“", "abc"), "abc")
+
+# Ø”
+
+assert_eq(call("Ø”", [123, 456, 789]), [[3, 5, 7], [2, 4], [1], [9], [6, 8]])
+assert_eq(
+    call("Ø”", ["abcd", 12345, "xyz", 67]), [["b", 1], ["a"], [7], ["y", 6], [2, "x"]]
+)
+assert_eq(
+    call("Ø”", [[123, 456, 789], ["abc", "def", "ghi"]]),
+    [[456, "abc"], [123], ["ghi"], [789, "def"]],
+)
+assert_eq(call("Ø”", []), [])
+
+assert_eq(call("Ø”", 123), 123)
+assert_eq(call("Ø”", "abc"), "abc")
+
 # # ÆC
 #
 # assert_eq(call("ÆC", 0), 1.0)  # ~ 1
 # assert_eq(call("ÆC", 0.524), 0.8658247218821449)  # ~ sqrt(3) / 2
 # assert_eq(call("ÆC", 0.785), 0.7073882691671998)  # ~ sqrt(2) / 2
 # assert_eq(call("ÆC", 1.047), 0.5001710745970702)  # ~ 1/2
 # assert_eq(call("ÆC", 1.571), -0.00020367320369517789)  # ~ 0
```

### Comparing `thunno2-2.1.4/thunno2/tokens.py` & `thunno2-2.1.5/thunno2/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     random_digraphs_2,
 )
 import sys
 
 
 def get_command(token):
     for tokens, cmd in full_list:
-        if token.lower() in tokens:
+        if token.lower() == tokens:
             return cmd
     print(f"Couldn't find a command for token {token!r}", file=sys.stderr)
     sys.exit(0)
 
 
 def transpile(code):
     r = ""
```

### Comparing `thunno2-2.1.4/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.5/thunno2.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.4
+Version: 2.1.5
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.4.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.5.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

