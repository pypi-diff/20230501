# Comparing `tmp/linkify-it-py-1.0.3.tar.gz` & `tmp/linkify-it-py-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/linkify-it-py-1.0.3.tar", last modified: Sat Dec 18 08:27:17 2021, max compression
+gzip compressed data, was "dist/linkify-it-py-2.0.0.tar", last modified: Sat May  7 07:00:30 2022, max compression
```

## Comparing `linkify-it-py-1.0.3.tar` & `linkify-it-py-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9132 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6467 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/linkify_it/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20360 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/linkify_it/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    20791 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/linkify_it/tlds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7094 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/linkify_it/ucre.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9132 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/linkify_it_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-18 08:27:17.000000 linkify-it-py-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-12-18 08:27:14.000000 linkify-it-py-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9361 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6656 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it/
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21327 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20791 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/linkify_it/ucre.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9361 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/linkify_it_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-07 07:00:30.000000 linkify-it-py-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-05-07 07:00:27.000000 linkify-it-py-2.0.0/setup.py
```

### Comparing `linkify-it-py-1.0.3/LICENSE` & `linkify-it-py-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linkify-it-py-1.0.3/PKG-INFO` & `linkify-it-py-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkify-it-py
-Version: 1.0.3
+Version: 2.0.0
 Summary: Links recognition library with FULL unicode support.
 Home-page: https://github.com/tsutsu3/linkify-it-py
 Author: tsutsu3
 License: MIT
 Description: # linkify-it-py
         
         [![CI](https://github.com/tsutsu3/linkify-it-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/linkify-it-py/actions)
@@ -188,14 +188,19 @@
           protocol-neutral links.
         - __index__ - offset of matched text
         - __last_index__ - index of next char after mathch end
         - __raw__ - matched text
         - __text__ - normalized text
         - __url__ - link, generated from matched text
         
+        ### .matchAtStart(text)
+        
+        Checks if a match exists at the start of the string. Returns `Match`
+        (see docs for `match(text)`) or null if no URL is at the start.
+        Doesn't work with fuzzy links.
         
         ### .tlds(list_tlds, keep_old=False)
         
         Load (or merge) new tlds list. Those are needed for fuzzy links (without schema)
         to avoid false positives. By default:
         
         - 2-letter root zones are ok.
```

### Comparing `linkify-it-py-1.0.3/README.md` & `linkify-it-py-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -181,14 +181,19 @@
   protocol-neutral links.
 - __index__ - offset of matched text
 - __last_index__ - index of next char after mathch end
 - __raw__ - matched text
 - __text__ - normalized text
 - __url__ - link, generated from matched text
 
+### .matchAtStart(text)
+
+Checks if a match exists at the start of the string. Returns `Match`
+(see docs for `match(text)`) or null if no URL is at the start.
+Doesn't work with fuzzy links.
 
 ### .tlds(list_tlds, keep_old=False)
 
 Load (or merge) new tlds list. Those are needed for fuzzy links (without schema)
 to avoid false positives. By default:
 
 - 2-letter root zones are ok.
```

### Comparing `linkify-it-py-1.0.3/linkify_it/main.py` & `linkify-it-py-2.0.0/linkify_it/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,15 @@
         re_schema_test = (
             "(^|(?!_)(?:[><\uff5c]|" + self.re["src_ZPCc"] + "))(" + slist + ")"
         )
 
         # (?!_) cause 1.5x slowdown
         self.re["schema_test"] = re_schema_test
         self.re["schema_search"] = re_schema_test
+        self.re["schema_at_start"] = "^" + self.re["schema_search"]
 
         self.re["pretest"] = (
             "(" + re_schema_test + ")|(" + self.re["host_fuzzy_test"] + ")|@"
         )
 
         # Cleanup
 
@@ -555,14 +556,46 @@
             shift += self._last_index
 
         if len(result):
             return result
 
         return None
 
+    def match_at_start(self, text):
+        """Returns fully-formed (not fuzzy) link if it starts at the beginning
+        of the string, and null otherwise.
+
+        Args:
+            text (str): text to search
+
+        Retuns:
+            ``Match`` or ``None``
+        """
+        # Reset scan cache
+        self._text_cache = text
+        self._index = -1
+
+        if not len(text):
+            return None
+
+        founds = re.search(self.re["schema_at_start"], text, flags=re.IGNORECASE)
+        if not founds:
+            return None
+
+        m = (founds.group(), founds.groups()[0], founds.groups()[1])
+        length = self.test_schema_at(text, m[2], len(m[0]))
+        if not length:
+            return None
+
+        self._schema = m[2]
+        self._index = founds.start(0) + len(m[1])
+        self._last_index = founds.start(0) + len(m[0]) + length
+
+        return self._create_match(0)
+
     def tlds(self, list_tlds, keep_old=False):
         """Load (or merge) new tlds list. (chainable)
 
         Those are user for fuzzy links (without prefix) to avoid false positives.
         By default this algorythm used:
 
         * hostname with any 2-letter root zones are ok.
```

### Comparing `linkify-it-py-1.0.3/linkify_it/tlds.py` & `linkify-it-py-2.0.0/linkify_it/tlds.py`

 * *Files identical despite different names*

### Comparing `linkify-it-py-1.0.3/linkify_it/ucre.py` & `linkify-it-py-2.0.0/linkify_it/ucre.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,25 +34,14 @@
 # Prohibit any of "@/[]()" in user/pass to avoid wrong domain fetch.
 SRC_AUTH = "(?:(?:(?!" + SRC_ZCC + "|[@/\\[\\]()]).)+@)?"
 
 SRC_PORT = (
     "(?::(?:6(?:[0-4]\\d{3}|5(?:[0-4]\\d{2}|5(?:[0-2]\\d|3[0-5])))|[1-5]?\\d{1,4}))?"
 )
 
-SRC_HOST_TERMINATOR = (
-    "(?=$|"
-    + TEXT_SEPARATORS
-    + "|"
-    + SRC_ZPCC
-    + ")(?!-|_|:\\d|\\.-|\\.(?!$|"
-    + SRC_ZPCC
-    + "))"
-)
-
-
 # Allow anything in markdown spec, forbid quote (") at the first position
 # because emails enclosed in quotes are far more common
 SRC_EMAIL_NAME = '[\\-:&=\\+\\$,\\.a-zA-Z0-9_][\\-:&=\\+\\$,\\"\\.a-zA-Z0-9_]*'
 
 SRC_XN = "xn--[a-z0-9\\-]{1,59}"
 
 # More to read about domain names
@@ -95,60 +84,40 @@
 
 TPL_HOST_FUZZY = (
     "(?:" + SRC_IP4 + "|" + "(?:(?:(?:" + SRC_DOMAIN + ")\\.)+(?:%TLDS%))" + ")"
 )
 
 TPL_HOST_NO_IP_FUZZY = "(?:(?:(?:" + SRC_DOMAIN + ")\\.)+(?:%TLDS%))"
 
-SRC_HOST_STRICT = SRC_HOST + SRC_HOST_TERMINATOR
-
-TPL_HOST_FUZZY_STRICT = TPL_HOST_FUZZY + SRC_HOST_TERMINATOR
-
-SRC_HOST_PORT_STRICT = SRC_HOST + SRC_PORT + SRC_HOST_TERMINATOR
-
-TPL_HOST_PORT_FUZZY_STRICT = TPL_HOST_FUZZY + SRC_PORT + SRC_HOST_TERMINATOR
-
-TPL_HOST_PORT_NO_IP_FUZZY_STRICT = TPL_HOST_NO_IP_FUZZY + SRC_PORT + SRC_HOST_TERMINATOR
 
 # =============================================================================
 
 # Rude test fuzzy links by host, for quick deny
 TPL_HOST_FUZZY_TEST = (
     "localhost|www\\.|\\.\\d{1,3}\\.|(?:\\.(?:%TLDS%)(?:" + SRC_ZPCC + "|>|$))"
 )
 
-TPL_EMAIL_FUZZY = (
-    "(^|"
-    + TEXT_SEPARATORS
-    + '|"|\\(|'
-    + SRC_ZCC
-    + ")"
-    + "("
-    + SRC_EMAIL_NAME
-    + "@"
-    + TPL_HOST_FUZZY_STRICT
-    + ")"
-)
 
+def _re_host_terminator(opts):
+    src_host_terminator = (
+        "(?=$|"
+        + TEXT_SEPARATORS
+        + "|"
+        + SRC_ZPCC
+        + ")"
+        + "(?!"
+        + ("-(?!--)|" if opts.get("---") else "-|")
+        + "_|:\\d|\\.-|\\.(?!$|"
+        + SRC_ZPCC
+        + "))"
+    )
+    return src_host_terminator
 
-def _re_src_path(opts):
-    try:
-        _ = opts["---"]
-    # KeyError: Not found key:"---"
-    # TypeError: opts is None
-    except (KeyError, TypeError):
-        long_dash_flag = False
-    else:
-        long_dash_flag = True
-
-    if long_dash_flag:
-        options = "\\-(?!--(?:[^-]|$))(?:-*)|"  # `---` => long dash, terminate
-    else:
-        options = "\\-+|"
 
+def _re_src_path(opts):
     src_path = (
         "(?:"
         + "[/?#]"
         + "(?:"
         + "(?!"
         + SRC_ZCC
         + "|"
@@ -167,40 +136,40 @@
         + SRC_ZCC
         + '|["]).)+\\"|'
         + "\\'(?:(?!"
         + SRC_ZCC
         + "|[']).)+\\'|"
         + "\\'(?="
         + SRC_PSEUDO_LETTER
-        + "|[-]).|"
+        + "|[-])|"
         + "\\.{2,}[a-zA-Z0-9%/&]|"
         # google has many dots in "google search" links (#66, #81).
         # github has ... in commit range links,
         # ReSTRICT to
         # - english
         # - percent-encoded
         # - parts of file path
         # - params separator
         # until more examples found.
         + "\\.(?!"
         + SRC_ZCC
-        + "|[.]).|"
-        + options
+        + "|[.]|$)|"
+        + ("\\-(?!--(?:[^-]|$))(?:-*)|" if opts.get("---") else "\\-+|")
         + ",(?!"
         + SRC_ZCC
-        + ").|"  # allow `,,,` in paths
+        + "|$)|"  # allow `,,,` in paths
         + ";(?!"
         + SRC_ZCC
-        + ").|"  # allow `,,,` in paths
+        + "|$)|"  # allow `,,,` in paths
         + "\\!+(?!"
         + SRC_ZCC
-        + "|[!]).|"  # allow `!!!` in paths, but not at the end
+        + "|[!]|$)|"  # allow `!!!` in paths, but not at the end
         + "\\?(?!"
         + SRC_ZCC
-        + "|[?])."
+        + "|[?]|$)"
         + ")+"
         + "|\\/"
         + ")?"
     )
 
     return src_path
 
@@ -210,27 +179,52 @@
 
     Args:
         opts (dict): options
 
     Return:
         dict: dict of regex string
     """
+    SRC_HOST_STRICT = SRC_HOST + _re_host_terminator(opts)
+
+    TPL_HOST_FUZZY_STRICT = TPL_HOST_FUZZY + _re_host_terminator(opts)
+
+    SRC_HOST_PORT_STRICT = SRC_HOST + SRC_PORT + _re_host_terminator(opts)
+
+    TPL_HOST_PORT_FUZZY_STRICT = TPL_HOST_FUZZY + SRC_PORT + _re_host_terminator(opts)
+
+    TPL_HOST_PORT_NO_IP_FUZZY_STRICT = (
+        TPL_HOST_NO_IP_FUZZY + SRC_PORT + _re_host_terminator(opts)
+    )
+
+    TPL_EMAIL_FUZZY = (
+        "(^|"
+        + TEXT_SEPARATORS
+        + '|"|\\(|'
+        + SRC_ZCC
+        + ")"
+        + "("
+        + SRC_EMAIL_NAME
+        + "@"
+        + TPL_HOST_FUZZY_STRICT
+        + ")"
+    )
+
     regex = {
         "src_Any": SRC_ANY,
         "src_Cc": SRC_CC,
         "src_Cf": SRC_CF,
         "src_Z": SRC_Z,
         "src_P": SRC_P,
         "src_ZPCc": SRC_ZPCC,
         "src_ZCc": SRC_ZCC,
         "src_pseudo_letter": SRC_PSEUDO_LETTER,
         "src_ip4": SRC_IP4,
         "src_auth": SRC_AUTH,
         "src_port": SRC_PORT,
-        "src_host_terminator": SRC_HOST_TERMINATOR,
+        "src_host_terminator": _re_host_terminator(opts),
         "src_path": _re_src_path(opts),
         "src_email_name": SRC_EMAIL_NAME,
         "src_xn": SRC_XN,
         "src_domain_root": SRC_DOMAIN_ROOT,
         "src_domain": SRC_DOMAIN,
         "src_host": SRC_HOST,
         "tpl_host_fuzzy": TPL_HOST_FUZZY,
```

### Comparing `linkify-it-py-1.0.3/linkify_it_py.egg-info/PKG-INFO` & `linkify-it-py-2.0.0/linkify_it_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkify-it-py
-Version: 1.0.3
+Version: 2.0.0
 Summary: Links recognition library with FULL unicode support.
 Home-page: https://github.com/tsutsu3/linkify-it-py
 Author: tsutsu3
 License: MIT
 Description: # linkify-it-py
         
         [![CI](https://github.com/tsutsu3/linkify-it-py/workflows/CI/badge.svg?branch=main)](https://github.com/tsutsu3/linkify-it-py/actions)
@@ -188,14 +188,19 @@
           protocol-neutral links.
         - __index__ - offset of matched text
         - __last_index__ - index of next char after mathch end
         - __raw__ - matched text
         - __text__ - normalized text
         - __url__ - link, generated from matched text
         
+        ### .matchAtStart(text)
+        
+        Checks if a match exists at the start of the string. Returns `Match`
+        (see docs for `match(text)`) or null if no URL is at the start.
+        Doesn't work with fuzzy links.
         
         ### .tlds(list_tlds, keep_old=False)
         
         Load (or merge) new tlds list. Those are needed for fuzzy links (without schema)
         to avoid false positives. By default:
         
         - 2-letter root zones are ok.
```

### Comparing `linkify-it-py-1.0.3/setup.py` & `linkify-it-py-2.0.0/setup.py`

 * *Files identical despite different names*

