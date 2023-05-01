# Comparing `tmp/yaralyzer-0.9.2.tar.gz` & `tmp/yaralyzer-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaralyzer-0.9.2.tar", max compression
+gzip compressed data, was "yaralyzer-0.9.3.tar", max compression
```

## Comparing `yaralyzer-0.9.2.tar` & `yaralyzer-0.9.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     3610 2022-10-21 01:35:20.059045 yaralyzer-0.9.2/.yaralyzer.example
--rw-r--r--   0        0        0     1776 2023-02-27 02:52:01.650510 yaralyzer-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-10-02 19:25:19.605920 yaralyzer-0.9.2/LICENSE
--rw-r--r--   0        0        0     8965 2022-10-21 01:55:20.531023 yaralyzer-0.9.2/README.md
--rw-r--r--   0        0        0     1385 2023-02-27 02:51:23.787288 yaralyzer-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2616 2022-10-20 00:03:30.773182 yaralyzer-0.9.2/yaralyzer/__init__.py
--rw-r--r--   0        0        0     7011 2022-10-21 01:35:20.062620 yaralyzer-0.9.2/yaralyzer/bytes_match.py
--rw-r--r--   0        0        0     3693 2022-10-21 01:35:20.062948 yaralyzer-0.9.2/yaralyzer/config.py
--rw-r--r--   0        0        0     7951 2022-10-21 01:35:20.063313 yaralyzer-0.9.2/yaralyzer/decoding/bytes_decoder.py
--rw-r--r--   0        0        0     7241 2022-10-21 01:35:20.063778 yaralyzer-0.9.2/yaralyzer/decoding/decoding_attempt.py
--rw-r--r--   0        0        0     4395 2022-10-15 06:44:45.668414 yaralyzer-0.9.2/yaralyzer/encoding_detection/character_encodings.py
--rw-r--r--   0        0        0     2307 2022-10-06 03:31:54.327245 yaralyzer-0.9.2/yaralyzer/encoding_detection/encoding_assessment.py
--rw-r--r--   0        0        0     4673 2023-02-19 05:06:24.096213 yaralyzer-0.9.2/yaralyzer/encoding_detection/encoding_detector.py
--rw-r--r--   0        0        0     6922 2022-10-21 01:35:20.064622 yaralyzer-0.9.2/yaralyzer/helpers/bytes_helper.py
--rw-r--r--   0        0        0      211 2022-10-02 22:25:49.936913 yaralyzer-0.9.2/yaralyzer/helpers/dict_helper.py
--rw-r--r--   0        0        0     1196 2022-10-15 06:44:21.001732 yaralyzer-0.9.2/yaralyzer/helpers/file_helper.py
--rw-r--r--   0        0        0     4218 2022-10-15 06:52:45.806981 yaralyzer-0.9.2/yaralyzer/helpers/rich_text_helper.py
--rw-r--r--   0        0        0      834 2022-10-21 01:35:20.064951 yaralyzer-0.9.2/yaralyzer/helpers/string_helper.py
--rw-r--r--   0        0        0     3712 2022-10-15 06:44:45.669573 yaralyzer-0.9.2/yaralyzer/output/decoding_attempts_table.py
--rw-r--r--   0        0        0     2270 2022-10-06 03:31:54.328527 yaralyzer-0.9.2/yaralyzer/output/file_export.py
--rw-r--r--   0        0        0     1608 2022-10-21 01:35:20.065247 yaralyzer-0.9.2/yaralyzer/output/file_hashes_table.py
--rw-r--r--   0        0        0     3003 2022-10-21 01:35:20.065599 yaralyzer-0.9.2/yaralyzer/output/regex_match_metrics.py
--rw-r--r--   0        0        0     3682 2022-10-21 01:35:20.065961 yaralyzer-0.9.2/yaralyzer/output/rich_console.py
--rw-r--r--   0        0        0    12551 2022-10-21 01:35:20.066442 yaralyzer-0.9.2/yaralyzer/util/argument_parser.py
--rw-r--r--   0        0        0     4326 2022-10-21 01:35:20.066834 yaralyzer-0.9.2/yaralyzer/util/logging.py
--rw-r--r--   0        0        0     4453 2022-10-15 06:44:45.670113 yaralyzer-0.9.2/yaralyzer/yara/yara_match.py
--rw-r--r--   0        0        0     3021 2022-10-15 06:44:21.003208 yaralyzer-0.9.2/yaralyzer/yara/yara_rule_builder.py
--rw-r--r--   0        0        0     9180 2023-02-27 02:48:04.259413 yaralyzer-0.9.2/yaralyzer/yaralyzer.py
--rw-r--r--   0        0        0    10377 1970-01-01 00:00:00.000000 yaralyzer-0.9.2/setup.py
--rw-r--r--   0        0        0    10282 1970-01-01 00:00:00.000000 yaralyzer-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3610 2022-10-21 01:35:20.059045 yaralyzer-0.9.3/.yaralyzer.example
+-rw-r--r--   0        0        0     1842 2023-05-01 20:11:40.301939 yaralyzer-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2022-10-02 19:25:19.605920 yaralyzer-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8965 2022-10-21 01:55:20.531023 yaralyzer-0.9.3/README.md
+-rw-r--r--   0        0        0     1385 2023-05-01 20:11:40.308400 yaralyzer-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2616 2022-10-20 00:03:30.773182 yaralyzer-0.9.3/yaralyzer/__init__.py
+-rw-r--r--   0        0        0     7011 2022-10-21 01:35:20.062620 yaralyzer-0.9.3/yaralyzer/bytes_match.py
+-rw-r--r--   0        0        0     3693 2022-10-21 01:35:20.062948 yaralyzer-0.9.3/yaralyzer/config.py
+-rw-r--r--   0        0        0     7951 2022-10-21 01:35:20.063313 yaralyzer-0.9.3/yaralyzer/decoding/bytes_decoder.py
+-rw-r--r--   0        0        0     7241 2022-10-21 01:35:20.063778 yaralyzer-0.9.3/yaralyzer/decoding/decoding_attempt.py
+-rw-r--r--   0        0        0     4395 2022-10-15 06:44:45.668414 yaralyzer-0.9.3/yaralyzer/encoding_detection/character_encodings.py
+-rw-r--r--   0        0        0     2307 2022-10-06 03:31:54.327245 yaralyzer-0.9.3/yaralyzer/encoding_detection/encoding_assessment.py
+-rw-r--r--   0        0        0     4673 2023-02-19 05:06:24.096213 yaralyzer-0.9.3/yaralyzer/encoding_detection/encoding_detector.py
+-rw-r--r--   0        0        0     6922 2022-10-21 01:35:20.064622 yaralyzer-0.9.3/yaralyzer/helpers/bytes_helper.py
+-rw-r--r--   0        0        0      211 2022-10-02 22:25:49.936913 yaralyzer-0.9.3/yaralyzer/helpers/dict_helper.py
+-rw-r--r--   0        0        0     1196 2022-10-15 06:44:21.001732 yaralyzer-0.9.3/yaralyzer/helpers/file_helper.py
+-rw-r--r--   0        0        0     4218 2022-10-15 06:52:45.806981 yaralyzer-0.9.3/yaralyzer/helpers/rich_text_helper.py
+-rw-r--r--   0        0        0      834 2022-10-21 01:35:20.064951 yaralyzer-0.9.3/yaralyzer/helpers/string_helper.py
+-rw-r--r--   0        0        0     3712 2022-10-15 06:44:45.669573 yaralyzer-0.9.3/yaralyzer/output/decoding_attempts_table.py
+-rw-r--r--   0        0        0     2270 2022-10-06 03:31:54.328527 yaralyzer-0.9.3/yaralyzer/output/file_export.py
+-rw-r--r--   0        0        0     1608 2022-10-21 01:35:20.065247 yaralyzer-0.9.3/yaralyzer/output/file_hashes_table.py
+-rw-r--r--   0        0        0     3003 2022-10-21 01:35:20.065599 yaralyzer-0.9.3/yaralyzer/output/regex_match_metrics.py
+-rw-r--r--   0        0        0     3682 2022-10-21 01:35:20.065961 yaralyzer-0.9.3/yaralyzer/output/rich_console.py
+-rw-r--r--   0        0        0    12551 2022-10-21 01:35:20.066442 yaralyzer-0.9.3/yaralyzer/util/argument_parser.py
+-rw-r--r--   0        0        0     4326 2022-10-21 01:35:20.066834 yaralyzer-0.9.3/yaralyzer/util/logging.py
+-rw-r--r--   0        0        0     4453 2022-10-15 06:44:45.670113 yaralyzer-0.9.3/yaralyzer/yara/yara_match.py
+-rw-r--r--   0        0        0     3021 2022-10-15 06:44:21.003208 yaralyzer-0.9.3/yaralyzer/yara/yara_rule_builder.py
+-rw-r--r--   0        0        0     9180 2023-02-27 02:48:04.259413 yaralyzer-0.9.3/yaralyzer/yaralyzer.py
+-rw-r--r--   0        0        0    10282 1970-01-01 00:00:00.000000 yaralyzer-0.9.3/PKG-INFO
```

### Comparing `yaralyzer-0.9.2/.yaralyzer.example` & `yaralyzer-0.9.3/.yaralyzer.example`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/CHANGELOG.md` & `yaralyzer-0.9.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+### 0.9.3
+* Lock `yara-python` at 4.2.3 bc 4.3.x causes problems
+
 ### 0.9.2
 * Fix PyPi screenshots
 * Raise better error message if yara rules file doesn't exist
 
 ### 0.9.1
 * Fix PyPi screenshots
```

### Comparing `yaralyzer-0.9.2/LICENSE` & `yaralyzer-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/README.md` & `yaralyzer-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/pyproject.toml` & `yaralyzer-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yaralyzer"
-version = "0.9.2"
+version = "0.9.3"
 description = "Visualize and force decode YARA and regex matches found in a file or byte stream. With colors. Lots of colors."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/michelcrypt4d4mus/yaralyzer"
 repository = "https://github.com/michelcrypt4d4mus/yaralyzer"
 documentation = "https://github.com/michelcrypt4d4mus/yaralyzer"
@@ -40,15 +40,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 chardet = "^5.0.0"
 #plyara = "^2.1.1"
 python-dotenv = "^0.21.0"
 rich = "^12.5.1"
 rich-argparse-plus = "^0.3.1"
-yara-python = "^4.2.3"
+yara-python = "~4.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 
 
 [tool.poetry.scripts]
 yaralyze = 'yaralyzer:yaralyze'
```

### Comparing `yaralyzer-0.9.2/yaralyzer/__init__.py` & `yaralyzer-0.9.3/yaralyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/bytes_match.py` & `yaralyzer-0.9.3/yaralyzer/bytes_match.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/config.py` & `yaralyzer-0.9.3/yaralyzer/config.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/decoding/bytes_decoder.py` & `yaralyzer-0.9.3/yaralyzer/decoding/bytes_decoder.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/decoding/decoding_attempt.py` & `yaralyzer-0.9.3/yaralyzer/decoding/decoding_attempt.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/encoding_detection/character_encodings.py` & `yaralyzer-0.9.3/yaralyzer/encoding_detection/character_encodings.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/encoding_detection/encoding_assessment.py` & `yaralyzer-0.9.3/yaralyzer/encoding_detection/encoding_assessment.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/encoding_detection/encoding_detector.py` & `yaralyzer-0.9.3/yaralyzer/encoding_detection/encoding_detector.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/helpers/bytes_helper.py` & `yaralyzer-0.9.3/yaralyzer/helpers/bytes_helper.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/helpers/file_helper.py` & `yaralyzer-0.9.3/yaralyzer/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/helpers/rich_text_helper.py` & `yaralyzer-0.9.3/yaralyzer/helpers/rich_text_helper.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/helpers/string_helper.py` & `yaralyzer-0.9.3/yaralyzer/helpers/string_helper.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/output/decoding_attempts_table.py` & `yaralyzer-0.9.3/yaralyzer/output/decoding_attempts_table.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/output/file_export.py` & `yaralyzer-0.9.3/yaralyzer/output/file_export.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/output/file_hashes_table.py` & `yaralyzer-0.9.3/yaralyzer/output/file_hashes_table.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/output/regex_match_metrics.py` & `yaralyzer-0.9.3/yaralyzer/output/regex_match_metrics.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/output/rich_console.py` & `yaralyzer-0.9.3/yaralyzer/output/rich_console.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/util/argument_parser.py` & `yaralyzer-0.9.3/yaralyzer/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/util/logging.py` & `yaralyzer-0.9.3/yaralyzer/util/logging.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/yara/yara_match.py` & `yaralyzer-0.9.3/yaralyzer/yara/yara_match.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/yara/yara_rule_builder.py` & `yaralyzer-0.9.3/yaralyzer/yara/yara_rule_builder.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/yaralyzer/yaralyzer.py` & `yaralyzer-0.9.3/yaralyzer/yaralyzer.py`

 * *Files identical despite different names*

### Comparing `yaralyzer-0.9.2/setup.py` & `yaralyzer-0.9.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: yaralyzer
+Version: 0.9.3
+Summary: Visualize and force decode YARA and regex matches found in a file or byte stream. With colors. Lots of colors.
+Home-page: https://github.com/michelcrypt4d4mus/yaralyzer
+License: GPL-3.0-or-later
+Keywords: ascii art,binary,character encoding,color,decode,encoding,malware,malware analysis,regex,regular expressions,reverse engineering,threat assessment,visualization,yara
+Author: Michel de Cryptadamus
+Author-email: michel@cryptadamus.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Security
+Requires-Dist: chardet (>=5.0.0,<6.0.0)
+Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: rich-argparse-plus (>=0.3.1,<0.4.0)
+Requires-Dist: yara-python (>=4.2.3,<4.3.0)
+Project-URL: Documentation, https://github.com/michelcrypt4d4mus/yaralyzer
+Project-URL: Repository, https://github.com/michelcrypt4d4mus/yaralyzer
+Description-Content-Type: text/markdown
 
-packages = \
-['yaralyzer',
- 'yaralyzer.decoding',
- 'yaralyzer.encoding_detection',
- 'yaralyzer.helpers',
- 'yaralyzer.output',
- 'yaralyzer.util',
- 'yaralyzer.yara']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['chardet>=5.0.0,<6.0.0',
- 'python-dotenv>=0.21.0,<0.22.0',
- 'rich-argparse-plus>=0.3.1,<0.4.0',
- 'rich>=12.5.1,<13.0.0',
- 'yara-python>=4.2.3,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['yaralyze = yaralyzer:yaralyze',
-                     'yaralyzer_show_color_theme = '
-                     'yaralyzer.helpers.rich_text_helper:yaralyzer_show_color_theme']}
-
-setup_kwargs = {
-    'name': 'yaralyzer',
-    'version': '0.9.2',
-    'description': 'Visualize and force decode YARA and regex matches found in a file or byte stream. With colors. Lots of colors.',
-    'long_description': '<!-- ![Tests](https://img.shields.io/github/workflow/status/michelcrypt4d4mus/yaralyzer/tests?label=tests) -->\n![Python Version](https://img.shields.io/pypi/pyversions/yaralyzer)\n![Release](https://img.shields.io/github/v/release/michelcrypt4d4mus/yaralyzer?sort=semver)\n![Downloads](https://img.shields.io/pypi/dm/yaralyzer)\n\n# THE YARALYZER\n\n![YARA match](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/top_of_readme.png)\n\nVisually inspect all of the regex matches (and their sexier, more cloak and dagger cousins, the [YARA](https://github.com/VirusTotal/yara-python) matches) found in binary data and/or text. See what happens when you force various character encodings upon those matched bytes. [With colors](https://github.com/michelcrypt4d4mus/yaralyzer#example-output).\n\n#### Quick Start\n```sh\npipx install yaralyzer\n\n# Scan against YARA definitions in a file:\nyaralyze --yara-rules /secret/vault/sigmunds_malware_rules.yara lacan_buys_the_dip.pdf\n\n# Scan against an arbitrary regular expression:\nyaralyze --regex-pattern \'good and evil.*of\\s+\\w+byte\' the_crypto_archipelago.exe\n\n# Scan against an arbitrary YARA hex pattern\nyaralyze --hex-pattern \'d0 93 d0 a3 d0 [-] 9b d0 90 d0 93\' one_day_in_the_life_of_ivan_cryptosovich.bin\n```\n\n#### What It Do\n1. **See the actual bytes your YARA rules are matching.** No more digging around copy/pasting the start positions reported by YARA into your favorite hex editor. Displays both the bytes matched by YARA as well as a configurable number of bytes before and after each match in hexadecimal and "raw" python string representation.\n1. **Do the same for byte patterns and regular expressions without writing a YARA file.** If you\'re too lazy to write a YARA file but are trying to determine, say, whether there\'s a regular expression hidden somewhere in the file you could scan for the pattern `\'/.+/\'` and immediately get a window into all the bytes in the file that live between front slashes. Same story for quotes, BOMs, etc. Any regex YARA can handle is supported so the sky is the limit.\n1. **Detect the possible encodings of each set of matched bytes.** [The `chardet` library](https://github.com/chardet/chardet) is a sophisticated library for guessing character encodings and it is leveraged here.\n1. **Display the result of forcing various character encodings upon the matched areas.** Several default character encodings will be _forcibly_ attempted in the region around the match. [`chardet`](https://github.com/chardet/chardet) will also be leveraged to see if the bytes fit the pattern of _any_ known encoding. If `chardet` is confident enough (configurable), an attempt at decoding the bytes using that encoding will be displayed.\n1. **Export the matched regions/decodings to SVG, HTML, and colored text files.** Show off your ASCII art.\n\n#### Why It Do\nThe Yaralyzer\'s functionality was extracted from [The Pdfalyzer](https://github.com/michelcrypt4d4mus/pdfalyzer) when it became apparent that visualizing and decoding pattern matches in binaries had more utility than just in a PDF analysis tool.\n\n[YARA](https://github.com/VirusTotal/yara-python), for those who are unaware[^1], is branded as a malware analysis/alerting tool but it\'s actually both a lot more and a lot less than that. One way to think about it is that YARA is a regular expression matching engine on steroids. It can locate regex matches in binaries like any regex engine but it can also do far wilder things like combine regexes in logical groups, compare regexes against all 256 XORed versions of a binary, check for `base64` and other encodings of the pattern, and more.  Maybe most importantly of all YARA provides a standard text based format for\npeople to _share_ their \'roided regexes with the world. All these features are particularly useful when analyzing or reverse engineering malware, whose authors tend to invest a great deal of time into making stuff hard to find.\n\nBut... that\'s also all YARA does. Everything else is up to the user. YARA\'s just a match engine and if you don\'t know what to match (or even what character encoding you might be able to match in) it only gets you so far. I found myself a bit frustrated trying to use YARA to look at all the matches of a few critical patterns:\n\n1. Bytes between escaped quotes (`\\".+\\"` and `\\\'.+\\\'`)\n1. Bytes between front slashes (`/.+/`). Front slashes demarcate a regular expression in many implementations and I was trying to see if any of the bytes matching this pattern were _actually_ regexes.\n\nYARA just tells you the byte position and the matched string but it can\'t tell you whether those bytes are UTF-8, UTF-16, Latin-1, etc. etc. (or none of the above). I also found myself wanting to understand what was going _in the region_ of the matched bytes and not just _in_ the matched bytes. In other words I wanted to scope the bytes immediately before and after whatever got matched.\n\nEnter **The Yaralyzer**, which lets you quickly scan the regions around matches while also showing you what those regions would look like if they were forced into various character encodings.\n\nIt\'s important to note that **The Yaralyzer** isn\'t a full on malware reversing tool. It can\'t do all the things a tool like [CyberChef](https://gchq.github.io/CyberChef/) does and it doesn\'t try to. It\'s more intended to give you a quick visual overview of suspect regions in the binary so you can hone in on the areas you might want to inspect with a more serious tool like [CyberChef](https://gchq.github.io/CyberChef/).\n\n# Installation\nInstall it with [`pipx`](https://pypa.github.io/pipx/) or `pip3`. `pipx` is a marginally better solution as it guarantees any packages installed with it will be isolated from the rest of your local python environment. Of course if you don\'t really have a local python environment this is a moot point and you can feel free to install with `pip`/`pip3`.\n```\npipx install yaralyzer\n```\n\n# Usage\nRun `yaralyze -h` to see the command line options (screenshot below).\n\n![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/yaralyze_help.png)\n\nFor info on exporting SVG images, HTML, etc., see [Example Output](#example-output).\n\n### Configuration\nIf you place a filed called `.yaralyzer` in your home directory or the current working directory then environment variables specified in that `.yaralyzer` file will be added to the environment each time yaralyzer is invoked. This provides a mechanism for permanently configuring various command line options so you can avoid typing them over and over. See the example file [`.yaralyzer.example`](.yaralyzer.example) to see which options can be configured this way.\n\nOnly one `.yaralyzer` file will be loaded and the working directory\'s `.yaralyzer` takes precedence over the home directory\'s `.yaralyzer`.\n\n### As A Library\n[`Yaralyzer`](yaralyzer/yaralyzer.py) is the main class. It has a variety of constructors supporting:\n\n1. Precompiled YARA rules\n1. Creating a YARA rule from a string\n1. Loading YARA rules from files\n1. Loading YARA rules from all `.yara` file in a directory\n1. Scanning `bytes`\n1. Scanning a file\n\nShould you want to iterate over the `BytesMatch` (like a `re.Match` object for a YARA match) and `BytesDecoder` (tracks decoding attempt stats) objects returned by The Yaralyzer, you can do so like this:\n\n```python\nfrom yaralyzer.yaralyzer import Yaralyzer\n\nyaralyzer = Yaralyzer.for_rules_files([\'/secret/rule.yara\'], \'lacan_buys_the_dip.pdf\')\n\nfor bytes_match, bytes_decoder in yaralyzer.match_iterator():\n    do_stuff()\n```\n\n# Example Output\nThe Yaralyzer can export visualizations to HTML, ANSI colored text, and SVG vector images using the file export functionality that comes with [Rich](https://github.com/Textualize/rich). SVGs can be turned into `png` format images with a tool like [Inkscape](https://inkscape.org/) or `cairosvg`. In our experience they both work though we\'ve seen some glitchiness with `cairosvg`.\n\n**PyPi Users:** If you are reading this document [on PyPi](https://pypi.org/project/yaralyzer/) be aware that it renders a lot better [over on GitHub](https://github.com/michelcrypt4d4mus/yaralyzer). Pretty pictures, footnotes that work, etc.\n\n#### Raw YARA match result:\n\n![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/yara_match_result.jpg)\n\n#### Display hex, raw python string, and various attempted decodings of both the match and the bytes before and after the match (configurable):\n\n![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/font_34_frontslash_scan.png)\n\n#### Bonus: see what `chardet.detect()` thinks about the likelihood your bytes are in a given encoding/language:\n\n![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/decoding_and_chardet_table_2.png)\n\n\n# TODO\n* highlight decodes done at `chardet`s behest\n* deal with repetitive matches\n\n[^1]: As I was until recently.\n',
-    'author': 'Michel de Cryptadamus',
-    'author_email': 'michel@cryptadamus.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/michelcrypt4d4mus/yaralyzer',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+<!-- ![Tests](https://img.shields.io/github/workflow/status/michelcrypt4d4mus/yaralyzer/tests?label=tests) -->
+![Python Version](https://img.shields.io/pypi/pyversions/yaralyzer)
+![Release](https://img.shields.io/github/v/release/michelcrypt4d4mus/yaralyzer?sort=semver)
+![Downloads](https://img.shields.io/pypi/dm/yaralyzer)
 
+# THE YARALYZER
+
+![YARA match](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/top_of_readme.png)
+
+Visually inspect all of the regex matches (and their sexier, more cloak and dagger cousins, the [YARA](https://github.com/VirusTotal/yara-python) matches) found in binary data and/or text. See what happens when you force various character encodings upon those matched bytes. [With colors](https://github.com/michelcrypt4d4mus/yaralyzer#example-output).
+
+#### Quick Start
+```sh
+pipx install yaralyzer
+
+# Scan against YARA definitions in a file:
+yaralyze --yara-rules /secret/vault/sigmunds_malware_rules.yara lacan_buys_the_dip.pdf
+
+# Scan against an arbitrary regular expression:
+yaralyze --regex-pattern 'good and evil.*of\s+\w+byte' the_crypto_archipelago.exe
+
+# Scan against an arbitrary YARA hex pattern
+yaralyze --hex-pattern 'd0 93 d0 a3 d0 [-] 9b d0 90 d0 93' one_day_in_the_life_of_ivan_cryptosovich.bin
+```
+
+#### What It Do
+1. **See the actual bytes your YARA rules are matching.** No more digging around copy/pasting the start positions reported by YARA into your favorite hex editor. Displays both the bytes matched by YARA as well as a configurable number of bytes before and after each match in hexadecimal and "raw" python string representation.
+1. **Do the same for byte patterns and regular expressions without writing a YARA file.** If you're too lazy to write a YARA file but are trying to determine, say, whether there's a regular expression hidden somewhere in the file you could scan for the pattern `'/.+/'` and immediately get a window into all the bytes in the file that live between front slashes. Same story for quotes, BOMs, etc. Any regex YARA can handle is supported so the sky is the limit.
+1. **Detect the possible encodings of each set of matched bytes.** [The `chardet` library](https://github.com/chardet/chardet) is a sophisticated library for guessing character encodings and it is leveraged here.
+1. **Display the result of forcing various character encodings upon the matched areas.** Several default character encodings will be _forcibly_ attempted in the region around the match. [`chardet`](https://github.com/chardet/chardet) will also be leveraged to see if the bytes fit the pattern of _any_ known encoding. If `chardet` is confident enough (configurable), an attempt at decoding the bytes using that encoding will be displayed.
+1. **Export the matched regions/decodings to SVG, HTML, and colored text files.** Show off your ASCII art.
+
+#### Why It Do
+The Yaralyzer's functionality was extracted from [The Pdfalyzer](https://github.com/michelcrypt4d4mus/pdfalyzer) when it became apparent that visualizing and decoding pattern matches in binaries had more utility than just in a PDF analysis tool.
+
+[YARA](https://github.com/VirusTotal/yara-python), for those who are unaware[^1], is branded as a malware analysis/alerting tool but it's actually both a lot more and a lot less than that. One way to think about it is that YARA is a regular expression matching engine on steroids. It can locate regex matches in binaries like any regex engine but it can also do far wilder things like combine regexes in logical groups, compare regexes against all 256 XORed versions of a binary, check for `base64` and other encodings of the pattern, and more.  Maybe most importantly of all YARA provides a standard text based format for
+people to _share_ their 'roided regexes with the world. All these features are particularly useful when analyzing or reverse engineering malware, whose authors tend to invest a great deal of time into making stuff hard to find.
+
+But... that's also all YARA does. Everything else is up to the user. YARA's just a match engine and if you don't know what to match (or even what character encoding you might be able to match in) it only gets you so far. I found myself a bit frustrated trying to use YARA to look at all the matches of a few critical patterns:
+
+1. Bytes between escaped quotes (`\".+\"` and `\'.+\'`)
+1. Bytes between front slashes (`/.+/`). Front slashes demarcate a regular expression in many implementations and I was trying to see if any of the bytes matching this pattern were _actually_ regexes.
+
+YARA just tells you the byte position and the matched string but it can't tell you whether those bytes are UTF-8, UTF-16, Latin-1, etc. etc. (or none of the above). I also found myself wanting to understand what was going _in the region_ of the matched bytes and not just _in_ the matched bytes. In other words I wanted to scope the bytes immediately before and after whatever got matched.
+
+Enter **The Yaralyzer**, which lets you quickly scan the regions around matches while also showing you what those regions would look like if they were forced into various character encodings.
+
+It's important to note that **The Yaralyzer** isn't a full on malware reversing tool. It can't do all the things a tool like [CyberChef](https://gchq.github.io/CyberChef/) does and it doesn't try to. It's more intended to give you a quick visual overview of suspect regions in the binary so you can hone in on the areas you might want to inspect with a more serious tool like [CyberChef](https://gchq.github.io/CyberChef/).
+
+# Installation
+Install it with [`pipx`](https://pypa.github.io/pipx/) or `pip3`. `pipx` is a marginally better solution as it guarantees any packages installed with it will be isolated from the rest of your local python environment. Of course if you don't really have a local python environment this is a moot point and you can feel free to install with `pip`/`pip3`.
+```
+pipx install yaralyzer
+```
+
+# Usage
+Run `yaralyze -h` to see the command line options (screenshot below).
+
+![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/yaralyze_help.png)
+
+For info on exporting SVG images, HTML, etc., see [Example Output](#example-output).
+
+### Configuration
+If you place a filed called `.yaralyzer` in your home directory or the current working directory then environment variables specified in that `.yaralyzer` file will be added to the environment each time yaralyzer is invoked. This provides a mechanism for permanently configuring various command line options so you can avoid typing them over and over. See the example file [`.yaralyzer.example`](.yaralyzer.example) to see which options can be configured this way.
+
+Only one `.yaralyzer` file will be loaded and the working directory's `.yaralyzer` takes precedence over the home directory's `.yaralyzer`.
+
+### As A Library
+[`Yaralyzer`](yaralyzer/yaralyzer.py) is the main class. It has a variety of constructors supporting:
+
+1. Precompiled YARA rules
+1. Creating a YARA rule from a string
+1. Loading YARA rules from files
+1. Loading YARA rules from all `.yara` file in a directory
+1. Scanning `bytes`
+1. Scanning a file
+
+Should you want to iterate over the `BytesMatch` (like a `re.Match` object for a YARA match) and `BytesDecoder` (tracks decoding attempt stats) objects returned by The Yaralyzer, you can do so like this:
+
+```python
+from yaralyzer.yaralyzer import Yaralyzer
+
+yaralyzer = Yaralyzer.for_rules_files(['/secret/rule.yara'], 'lacan_buys_the_dip.pdf')
+
+for bytes_match, bytes_decoder in yaralyzer.match_iterator():
+    do_stuff()
+```
+
+# Example Output
+The Yaralyzer can export visualizations to HTML, ANSI colored text, and SVG vector images using the file export functionality that comes with [Rich](https://github.com/Textualize/rich). SVGs can be turned into `png` format images with a tool like [Inkscape](https://inkscape.org/) or `cairosvg`. In our experience they both work though we've seen some glitchiness with `cairosvg`.
+
+**PyPi Users:** If you are reading this document [on PyPi](https://pypi.org/project/yaralyzer/) be aware that it renders a lot better [over on GitHub](https://github.com/michelcrypt4d4mus/yaralyzer). Pretty pictures, footnotes that work, etc.
+
+#### Raw YARA match result:
+
+![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/yara_match_result.jpg)
+
+#### Display hex, raw python string, and various attempted decodings of both the match and the bytes before and after the match (configurable):
+
+![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/font_34_frontslash_scan.png)
+
+#### Bonus: see what `chardet.detect()` thinks about the likelihood your bytes are in a given encoding/language:
+
+![](https://github.com/michelcrypt4d4mus/yaralyzer/raw/master/doc/rendered_images/decoding_and_chardet_table_2.png)
+
+
+# TODO
+* highlight decodes done at `chardet`s behest
+* deal with repetitive matches
+
+[^1]: As I was until recently.
 
-setup(**setup_kwargs)
```

