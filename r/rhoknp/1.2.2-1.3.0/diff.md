# Comparing `tmp/rhoknp-1.2.2.tar.gz` & `tmp/rhoknp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhoknp-1.2.2.tar", max compression
+gzip compressed data, was "rhoknp-1.3.0.tar", max compression
```

## Comparing `rhoknp-1.2.2.tar` & `rhoknp-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,63 @@
--rw-r--r--   0        0        0     1073 2022-07-07 05:13:45.612050 rhoknp-1.2.2/LICENSE
--rw-r--r--   0        0        0     6528 2023-02-07 06:49:22.767712 rhoknp-1.2.2/README.md
--rw-r--r--   0        0        0     1554 2023-03-18 08:42:20.749014 rhoknp-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      474 2023-01-23 11:06:01.235960 rhoknp-1.2.2/src/rhoknp/__init__.py
--rw-r--r--   0        0        0      293 2023-01-25 04:22:29.044533 rhoknp-1.2.2/src/rhoknp/cli/__init__.py
--rw-r--r--   0        0        0     2935 2023-01-23 11:06:01.236336 rhoknp-1.2.2/src/rhoknp/cli/cli.py
--rw-r--r--   0        0        0     4143 2023-02-07 06:49:22.771309 rhoknp-1.2.2/src/rhoknp/cli/serve.py
--rw-r--r--   0        0        0     4320 2023-02-07 06:49:22.771622 rhoknp-1.2.2/src/rhoknp/cli/show.py
--rw-r--r--   0        0        0     1779 2023-01-23 11:06:01.236808 rhoknp-1.2.2/src/rhoknp/cli/stats.py
--rw-r--r--   0        0        0      826 2023-01-23 11:06:01.237203 rhoknp-1.2.2/src/rhoknp/cohesion/__init__.py
--rw-r--r--   0        0        0     6744 2023-02-07 06:49:22.772304 rhoknp-1.2.2/src/rhoknp/cohesion/argument.py
--rw-r--r--   0        0        0     9899 2023-02-07 06:49:22.772615 rhoknp-1.2.2/src/rhoknp/cohesion/coreference.py
--rw-r--r--   0        0        0     9566 2023-01-23 11:06:01.238718 rhoknp-1.2.2/src/rhoknp/cohesion/discourse.py
--rw-r--r--   0        0        0     2427 2023-01-23 11:06:01.239467 rhoknp-1.2.2/src/rhoknp/cohesion/exophora.py
--rw-r--r--   0        0        0    10329 2023-02-07 06:49:22.772957 rhoknp-1.2.2/src/rhoknp/cohesion/pas.py
--rw-r--r--   0        0        0     2595 2023-01-23 11:06:01.239969 rhoknp-1.2.2/src/rhoknp/cohesion/predicate.py
--rw-r--r--   0        0        0     4716 2023-01-23 11:06:01.240472 rhoknp-1.2.2/src/rhoknp/cohesion/rel.py
--rw-r--r--   0        0        0      226 2023-01-23 11:06:01.240680 rhoknp-1.2.2/src/rhoknp/processors/__init__.py
--rw-r--r--   0        0        0     4777 2023-03-03 06:23:17.601383 rhoknp-1.2.2/src/rhoknp/processors/jumanpp.py
--rw-r--r--   0        0        0     6551 2023-03-03 06:23:17.601701 rhoknp-1.2.2/src/rhoknp/processors/knp.py
--rw-r--r--   0        0        0     4790 2023-03-03 06:23:17.602217 rhoknp-1.2.2/src/rhoknp/processors/kwja.py
--rw-r--r--   0        0        0     2984 2022-10-29 15:30:49.159597 rhoknp-1.2.2/src/rhoknp/processors/processor.py
--rw-r--r--   0        0        0     4303 2023-02-07 06:49:22.773161 rhoknp-1.2.2/src/rhoknp/processors/senter.py
--rw-r--r--   0        0        0      378 2023-01-23 11:06:01.241792 rhoknp-1.2.2/src/rhoknp/props/__init__.py
--rw-r--r--   0        0        0      210 2022-10-24 08:19:10.843963 rhoknp-1.2.2/src/rhoknp/props/dependency.py
--rw-r--r--   0        0        0     1996 2023-01-23 11:06:01.242202 rhoknp-1.2.2/src/rhoknp/props/feature.py
--rw-r--r--   0        0        0      863 2023-01-23 11:06:01.242583 rhoknp-1.2.2/src/rhoknp/props/memo.py
--rw-r--r--   0        0        0     2917 2023-02-07 06:49:22.773596 rhoknp-1.2.2/src/rhoknp/props/named_entity.py
--rw-r--r--   0        0        0     1633 2023-01-23 11:06:01.243129 rhoknp-1.2.2/src/rhoknp/props/semantics.py
--rw-r--r--   0        0        0        0 2022-07-07 07:10:30.837345 rhoknp-1.2.2/src/rhoknp/py.typed
--rw-r--r--   0        0        0      337 2023-01-23 11:06:01.243840 rhoknp-1.2.2/src/rhoknp/units/__init__.py
--rw-r--r--   0        0        0    14479 2023-03-03 06:23:17.602965 rhoknp-1.2.2/src/rhoknp/units/base_phrase.py
--rw-r--r--   0        0        0     7740 2023-02-07 06:49:22.774401 rhoknp-1.2.2/src/rhoknp/units/clause.py
--rw-r--r--   0        0        0    15809 2023-02-07 06:49:22.774863 rhoknp-1.2.2/src/rhoknp/units/document.py
--rw-r--r--   0        0        0    11875 2023-02-07 06:49:22.775146 rhoknp-1.2.2/src/rhoknp/units/morpheme.py
--rw-r--r--   0        0        0     7202 2023-02-07 06:49:22.775468 rhoknp-1.2.2/src/rhoknp/units/phrase.py
--rw-r--r--   0        0        0    19078 2023-02-07 06:49:22.776073 rhoknp-1.2.2/src/rhoknp/units/sentence.py
--rw-r--r--   0        0        0     1521 2023-01-23 11:06:01.246571 rhoknp-1.2.2/src/rhoknp/units/unit.py
--rw-r--r--   0        0        0        0 2023-01-23 11:06:01.246629 rhoknp-1.2.2/src/rhoknp/utils/__init__.py
--rw-r--r--   0        0        0     3930 2023-01-23 11:06:01.247052 rhoknp-1.2.2/src/rhoknp/utils/reader.py
--rw-r--r--   0        0        0     7729 1970-01-01 00:00:00.000000 rhoknp-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-07-07 05:13:45.612050 rhoknp-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6528 2023-05-01 10:39:22.233408 rhoknp-1.3.0/README.md
+-rw-r--r--   0        0        0     1609 2023-05-01 10:39:22.239539 rhoknp-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-01-23 11:06:01.235960 rhoknp-1.3.0/src/rhoknp/__init__.py
+-rw-r--r--   0        0        0      293 2023-01-25 04:22:29.044533 rhoknp-1.3.0/src/rhoknp/cli/__init__.py
+-rw-r--r--   0        0        0     3334 2023-05-01 10:39:22.239944 rhoknp-1.3.0/src/rhoknp/cli/cli.py
+-rw-r--r--   0        0        0     6802 2023-05-01 10:39:22.240180 rhoknp-1.3.0/src/rhoknp/cli/serve.py
+-rw-r--r--   0        0        0     5782 2023-05-01 10:39:22.240529 rhoknp-1.3.0/src/rhoknp/cli/show.py
+-rw-r--r--   0        0        0      823 2023-05-01 10:39:22.240711 rhoknp-1.3.0/src/rhoknp/cli/static/css/style.css
+-rw-r--r--   0        0        0     9898 2023-05-01 10:39:22.241416 rhoknp-1.3.0/src/rhoknp/cli/static/images/apple-touch-icon.png
+-rw-r--r--   0        0        0    15086 2023-05-01 10:39:22.242054 rhoknp-1.3.0/src/rhoknp/cli/static/images/favicon.ico
+-rw-r--r--   0        0        0     1960 2023-05-01 10:39:22.242198 rhoknp-1.3.0/src/rhoknp/cli/static/js/script.js
+-rw-r--r--   0        0        0     1779 2023-01-23 11:06:01.236808 rhoknp-1.3.0/src/rhoknp/cli/stats.py
+-rw-r--r--   0        0        0     1705 2023-05-01 10:39:22.242748 rhoknp-1.3.0/src/rhoknp/cli/templates/base.jinja2
+-rw-r--r--   0        0        0      724 2023-05-01 10:39:22.242904 rhoknp-1.3.0/src/rhoknp/cli/templates/components/dependency_parsing.jinja2
+-rw-r--r--   0        0        0     1840 2023-05-01 10:39:22.243108 rhoknp-1.3.0/src/rhoknp/cli/templates/components/discourse_parsing.jinja2
+-rw-r--r--   0        0        0      276 2023-05-01 10:39:22.243247 rhoknp-1.3.0/src/rhoknp/cli/templates/components/error.jinja2
+-rw-r--r--   0        0        0      344 2023-05-01 10:39:22.243341 rhoknp-1.3.0/src/rhoknp/cli/templates/components/form.jinja2
+-rw-r--r--   0        0        0      136 2023-05-01 10:39:22.243485 rhoknp-1.3.0/src/rhoknp/cli/templates/components/hide_all_button.jinja2
+-rw-r--r--   0        0        0     1987 2023-05-01 10:39:22.243568 rhoknp-1.3.0/src/rhoknp/cli/templates/components/morphological_analysis.jinja2
+-rw-r--r--   0        0        0     1063 2023-05-01 10:39:22.243719 rhoknp-1.3.0/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2
+-rw-r--r--   0        0        0      163 2023-05-01 10:39:22.243791 rhoknp-1.3.0/src/rhoknp/cli/templates/components/navbar.jinja2
+-rw-r--r--   0        0        0       63 2023-05-01 10:39:22.244032 rhoknp-1.3.0/src/rhoknp/cli/templates/components/raw_input.jinja2
+-rw-r--r--   0        0        0      636 2023-05-01 10:39:22.244218 rhoknp-1.3.0/src/rhoknp/cli/templates/components/raw_output.jinja2
+-rw-r--r--   0        0        0      131 2023-05-01 10:39:22.244412 rhoknp-1.3.0/src/rhoknp/cli/templates/components/show_all_button.jinja2
+-rw-r--r--   0        0        0     1034 2023-05-01 10:39:22.244575 rhoknp-1.3.0/src/rhoknp/cli/templates/components/typo_correction.jinja2
+-rw-r--r--   0        0        0      722 2023-05-01 10:39:22.244665 rhoknp-1.3.0/src/rhoknp/cli/templates/components/word_splitting.jinja2
+-rw-r--r--   0        0        0      333 2023-05-01 10:39:22.244808 rhoknp-1.3.0/src/rhoknp/cli/templates/jumanpp.jinja2
+-rw-r--r--   0        0        0      526 2023-05-01 10:39:22.244946 rhoknp-1.3.0/src/rhoknp/cli/templates/knp.jinja2
+-rw-r--r--   0        0        0      643 2023-05-01 10:39:22.245089 rhoknp-1.3.0/src/rhoknp/cli/templates/kwja.jinja2
+-rw-r--r--   0        0        0      826 2023-01-23 11:06:01.237203 rhoknp-1.3.0/src/rhoknp/cohesion/__init__.py
+-rw-r--r--   0        0        0     6744 2023-02-07 06:49:22.772304 rhoknp-1.3.0/src/rhoknp/cohesion/argument.py
+-rw-r--r--   0        0        0     9899 2023-02-07 06:49:22.772615 rhoknp-1.3.0/src/rhoknp/cohesion/coreference.py
+-rw-r--r--   0        0        0     9566 2023-01-23 11:06:01.238718 rhoknp-1.3.0/src/rhoknp/cohesion/discourse.py
+-rw-r--r--   0        0        0     2427 2023-01-23 11:06:01.239467 rhoknp-1.3.0/src/rhoknp/cohesion/exophora.py
+-rw-r--r--   0        0        0    10329 2023-02-07 06:49:22.772957 rhoknp-1.3.0/src/rhoknp/cohesion/pas.py
+-rw-r--r--   0        0        0     2595 2023-01-23 11:06:01.239969 rhoknp-1.3.0/src/rhoknp/cohesion/predicate.py
+-rw-r--r--   0        0        0     4716 2023-01-23 11:06:01.240472 rhoknp-1.3.0/src/rhoknp/cohesion/rel.py
+-rw-r--r--   0        0        0      226 2023-01-23 11:06:01.240680 rhoknp-1.3.0/src/rhoknp/processors/__init__.py
+-rw-r--r--   0        0        0     5264 2023-05-01 10:39:22.245299 rhoknp-1.3.0/src/rhoknp/processors/jumanpp.py
+-rw-r--r--   0        0        0     7027 2023-05-01 10:39:22.245466 rhoknp-1.3.0/src/rhoknp/processors/knp.py
+-rw-r--r--   0        0        0     5617 2023-05-01 10:39:22.245819 rhoknp-1.3.0/src/rhoknp/processors/kwja.py
+-rw-r--r--   0        0        0     2984 2022-10-29 15:30:49.159597 rhoknp-1.3.0/src/rhoknp/processors/processor.py
+-rw-r--r--   0        0        0     3070 2023-05-01 10:39:22.245994 rhoknp-1.3.0/src/rhoknp/processors/senter.py
+-rw-r--r--   0        0        0      378 2023-01-23 11:06:01.241792 rhoknp-1.3.0/src/rhoknp/props/__init__.py
+-rw-r--r--   0        0        0      210 2022-10-24 08:19:10.843963 rhoknp-1.3.0/src/rhoknp/props/dependency.py
+-rw-r--r--   0        0        0     1996 2023-01-23 11:06:01.242202 rhoknp-1.3.0/src/rhoknp/props/feature.py
+-rw-r--r--   0        0        0      863 2023-01-23 11:06:01.242583 rhoknp-1.3.0/src/rhoknp/props/memo.py
+-rw-r--r--   0        0        0     2917 2023-02-07 06:49:22.773596 rhoknp-1.3.0/src/rhoknp/props/named_entity.py
+-rw-r--r--   0        0        0     1633 2023-01-23 11:06:01.243129 rhoknp-1.3.0/src/rhoknp/props/semantics.py
+-rw-r--r--   0        0        0        0 2022-07-07 07:10:30.837345 rhoknp-1.3.0/src/rhoknp/py.typed
+-rw-r--r--   0        0        0      337 2023-01-23 11:06:01.243840 rhoknp-1.3.0/src/rhoknp/units/__init__.py
+-rw-r--r--   0        0        0    14479 2023-03-03 06:23:17.602965 rhoknp-1.3.0/src/rhoknp/units/base_phrase.py
+-rw-r--r--   0        0        0     7740 2023-02-07 06:49:22.774401 rhoknp-1.3.0/src/rhoknp/units/clause.py
+-rw-r--r--   0        0        0    15809 2023-02-07 06:49:22.774863 rhoknp-1.3.0/src/rhoknp/units/document.py
+-rw-r--r--   0        0        0    11875 2023-02-07 06:49:22.775146 rhoknp-1.3.0/src/rhoknp/units/morpheme.py
+-rw-r--r--   0        0        0     7202 2023-02-07 06:49:22.775468 rhoknp-1.3.0/src/rhoknp/units/phrase.py
+-rw-r--r--   0        0        0    18039 2023-05-01 10:39:22.246566 rhoknp-1.3.0/src/rhoknp/units/sentence.py
+-rw-r--r--   0        0        0     1521 2023-01-23 11:06:01.246571 rhoknp-1.3.0/src/rhoknp/units/unit.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:06:01.246629 rhoknp-1.3.0/src/rhoknp/utils/__init__.py
+-rw-r--r--   0        0        0     3783 2023-05-01 10:39:22.247129 rhoknp-1.3.0/src/rhoknp/utils/reader.py
+-rw-r--r--   0        0        0     1112 2023-05-01 10:39:22.247398 rhoknp-1.3.0/src/rhoknp/utils/util.py
+-rw-r--r--   0        0        0     7785 1970-01-01 00:00:00.000000 rhoknp-1.3.0/PKG-INFO
```

### Comparing `rhoknp-1.2.2/LICENSE` & `rhoknp-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/README.md` & `rhoknp-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 <a href="https://www.codefactor.io/repository/github/ku-nlp/rhoknp"><img alt="CodeFactor" src="https://img.shields.io/codefactor/grade/github/ku-nlp/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rhoknp?style=flat-square">
 <a href="https://rhoknp.readthedocs.io/en/latest/"><img alt="Documentation" src="https://img.shields.io/readthedocs/rhoknp?style=flat-square"></a>
 <a href="https://github.com/psf/black"><img alt="Code style - black" src="https://img.shields.io/badge/code%20style-black-222222?style=flat-square"></a>
 </p>
 
-*rhoknp* is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1]
+_rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1]
 
 [^1]: The logo was originally generated using OpenAI DALL·E 2
 
 ```python
 import rhoknp
 
 # Perform language analysis by Juman++
@@ -60,15 +60,15 @@
 
 ## Documentation
 
 [https://rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/)
 
 ## Quick tour
 
-Let's start with using Juman++ with *rhoknp*.
+Let's start with using Juman++ with _rhoknp_.
 Here is a simple example of using Juman++ to analyze a sentence.
 
 ```python
 # Perform language analysis by Juman++
 jumanpp = rhoknp.Jumanpp()
 sentence = jumanpp.apply_to_sentence("電気抵抗率は電気の通しにくさを表す物性値である。")
 ```
@@ -121,15 +121,15 @@
     f.write(sentence.to_knp())
 
 # Load the sentence
 with open("sentence.knp", "rt") as f:
     sentence = rhoknp.Sentence.from_knp(f.read())
 ```
 
-*rhoknp* also provides APIs for document-level language analysis.
+_rhoknp_ also provides APIs for document-level language analysis.
 
 ```python
 document = rhoknp.Document.from_raw_text(
     "電気抵抗率は電気の通しにくさを表す物性値である。単に抵抗率とも呼ばれる。"
 )
 # If you know sentence boundaries, you can use `Document.from_sentences` instead.
 document = rhoknp.Document.from_sentences(
@@ -161,28 +161,28 @@
     document = rhoknp.Document.from_jumanpp(f.read())
 ```
 
 For more information, explore the [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/latest/).
 
 ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
 
-[*pyknp*](https://pypi.org/project/pyknp/) has been developed as the official Python binding for Juman++ and KNP.
-In *rhoknp*, we redesigned the API from the top-down, taking into account the current use cases of *pyknp*.
+[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official Python binding for Juman++ and KNP.
+In _rhoknp_, we redesigned the API from the top-down, taking into account the current use cases of _pyknp_.
 The main differences are as follows:
 
-- **Support for document-level language analysis**: *rhoknp* can load and instantiate the result of document-level language analysis (i.e., cohesion analysis and discourse relation analysis).
-- **Strictly type-aware**: *rhoknp* is thoroughly annotated with type annotations.
-- **Extensive test suite**: *rhoknp* is tested with an extensive test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
+- **Support for document-level language analysis**: _rhoknp_ can load and instantiate the result of document-level language analysis (i.e., cohesion analysis and discourse relation analysis).
+- **Strictly type-aware**: _rhoknp_ is thoroughly annotated with type annotations.
+- **Extensive test suite**: _rhoknp_ is tested with an extensive test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
 
 ## License
 
 MIT
 
 ## Contributing
 
-We welcome contributions to *rhoknp*.
+We welcome contributions to _rhoknp_.
 You can get started by reading the [contribution guide](https://rhoknp.readthedocs.io/en/latest/contributing/index.html).
 
 ## Reference
 
 - [KNP FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html)
 - [KNP - KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
                                  [rhoknp_logo]
      ****** rhoknp: Yet another Python binding for Juman++/KNP/KWJA ******
  [Test] [Codecov] [CodeFactor] [PyPI] [PyPI_-_Python_Version]_[Documentation]_
                              [Code_style_-_black]
-*rhoknp* is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
+_rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
 [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/
 kwja).[^1] [^1]: The logo was originally generated using OpenAI DALLÂ·E 2
 ```python import rhoknp # Perform language analysis by Juman++ jumanpp =
 rhoknp.Jumanpp() sentence = jumanpp.apply_to_sentence
 ( "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã" )
 # Access to the result for morpheme in sentence.morphemes: # a.k.a. keitai-so
 ... # Save language analysis by Juman++ with open("result.jumanpp", "wt") as f:
 f.write(sentence.to_jumanpp()) # Load language analysis by Juman++ with open
 ("result.jumanpp", "rt") as f: sentence = rhoknp.Sentence.from_jumanpp(f.read
 ()) ``` ## Requirements - Python 3.7+ ## Optional requirements for language
 analysis - [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+ - [KNP]
 (https://github.com/ku-nlp/knp) 5.0+ - [KWJA](https://github.com/ku-nlp/kwja)
 1.0.0+ ## Installation ```shell pip install rhoknp ``` ## Documentation [https:
 //rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/
-) ## Quick tour Let's start with using Juman++ with *rhoknp*. Here is a simple
+) ## Quick tour Let's start with using Juman++ with _rhoknp_. Here is a simple
 example of using Juman++ to analyze a sentence. ```python # Perform language
 analysis by Juman++ jumanpp = rhoknp.Jumanpp() sentence =
 jumanpp.apply_to_sentence
 ("é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã")
 ``` You can easily access the morphemes that make up the sentence. ```python
 for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
 can be saved in the JUMAN format. ```python # Save the sentence in the JUMAN
@@ -34,15 +34,15 @@
 ``` KNP performs language analysis at multiple levels. ```python for clause in
 sentence.clauses: # a.k.a., setsu ... for phrase in sentence.phrases: # a.k.a.
 bunsetsu ... for base_phrase in sentence.base_phrases: # a.k.a. kihon-ku ...
 for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
 can be saved in the KNP format. ```python # Save the sentence in the KNP format
 with open("sentence.knp", "wt") as f: f.write(sentence.to_knp()) # Load the
 sentence with open("sentence.knp", "rt") as f: sentence =
-rhoknp.Sentence.from_knp(f.read()) ``` *rhoknp* also provides APIs for
+rhoknp.Sentence.from_knp(f.read()) ``` _rhoknp_ also provides APIs for
 document-level language analysis. ```python document =
 rhoknp.Document.from_raw_text
 (
 "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ãããåã«æµæçã¨ãå¼ã°ããã"
 ) # If you know sentence boundaries, you can use `Document.from_sentences`
 instead. document = rhoknp.Document.from_sentences(
 [ "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã",
@@ -52,21 +52,21 @@
 language units in the document for sentence in document.sentences: ... for
 morpheme in document.morphemes: ... # Save language analysis by Juman++ with
 open("document.jumanpp", "wt") as f: f.write(document.to_jumanpp()) # Load
 language analysis by Juman++ with open("document.jumanpp", "rt") as f: document
 = rhoknp.Document.from_jumanpp(f.read()) ``` For more information, explore the
 [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/
 latest/). ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
-[*pyknp*](https://pypi.org/project/pyknp/) has been developed as the official
-Python binding for Juman++ and KNP. In *rhoknp*, we redesigned the API from the
-top-down, taking into account the current use cases of *pyknp*. The main
+[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official
+Python binding for Juman++ and KNP. In _rhoknp_, we redesigned the API from the
+top-down, taking into account the current use cases of _pyknp_. The main
 differences are as follows: - **Support for document-level language analysis**:
-*rhoknp* can load and instantiate the result of document-level language
+_rhoknp_ can load and instantiate the result of document-level language
 analysis (i.e., cohesion analysis and discourse relation analysis). -
-**Strictly type-aware**: *rhoknp* is thoroughly annotated with type
-annotations. - **Extensive test suite**: *rhoknp* is tested with an extensive
+**Strictly type-aware**: _rhoknp_ is thoroughly annotated with type
+annotations. - **Extensive test suite**: _rhoknp_ is tested with an extensive
 test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-
 nlp/rhoknp). ## License MIT ## Contributing We welcome contributions to
-*rhoknp*. You can get started by reading the [contribution guide](https://
+_rhoknp_. You can get started by reading the [contribution guide](https://
 rhoknp.readthedocs.io/en/latest/contributing/index.html). ## Reference - [KNP
 FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html) - [KNP -
 KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

### Comparing `rhoknp-1.2.2/pyproject.toml` & `rhoknp-1.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhoknp"
-version = "1.2.2"
+version = "1.3.0"
 description = "Yet another Python binding for Juman++/KNP/KWJA"
 license = "MIT"
 authors = [
     "Hirokazu Kiyomaru <h.kiyomaru@gmail.com>",
     "Nobuhiro Ueda <ueda@nlp.ist.i.kyoto-u.ac.jp>",
 ]
 readme = "README.md"
@@ -17,38 +17,39 @@
 cached-property = { version = "^1.5", python = "<3.8" }
 importlib-metadata = { version = ">=5.2", python = "<3.8" }
 typer = { version = ">=0.6.1,<0.8", optional = true }
 PyYAML = { version = "^6.0", optional = true }
 rich = { version = ">=12.6", optional = true }
 uvicorn = { version = ">=0.21.0,<1", optional = true }
 fastapi = { version = ">=0.92.0,<1", optional = true }
+jinja2 = { version = "^3.1.2", optional = true }
 
 [tool.poetry.group.dev]
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.9"
 
 [tool.poetry.group.test]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
-httpx = "^0.23.1"
+httpx = "^0.24.0"
 
 [tool.poetry.group.docs]
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.3"
 sphinx-prompt = "^1.5"
 sphinx-copybutton = "^0.5.0"
-myst-parser = "^0.19.1"
-furo = "^2022.12"
+myst-parser = "^1.0"
+furo = "^2023.3"
 
 [tool.poetry.extras]
-cli = ["typer", "PyYAML", "rich", "uvicorn", "fastapi"]
+cli = ["typer", "PyYAML", "rich", "uvicorn", "fastapi", "jinja2"]
 
 [tool.poetry.scripts]
 rhoknp = "rhoknp.cli.cli:app"
 
 [tool.black]
 line-length = 120
 target-version = ["py37", "py38", "py39", "py310", "py311"]
```

### Comparing `rhoknp-1.2.2/src/rhoknp/cli/cli.py` & `rhoknp-1.3.0/src/rhoknp/cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from pathlib import Path
+from typing import List, Optional
 
 import typer
 import yaml
 
 from rhoknp import Document, __version__
 from rhoknp.cli.serve import AnalyzerType, serve_analyzer
 from rhoknp.cli.show import draw_tree
@@ -31,27 +32,29 @@
     pass
 
 
 @app.command(help="Print given file content in tree format.")
 def show(
     knp_path: Path = typer.Argument(..., exists=True, dir_okay=False, help="Path to knp file to show"),
     pos: bool = typer.Option(False, "--pos", "-p", help="Show POS characters."),
-    rel: bool = typer.Option(False, "--rel", "-r", help="Show <rel> tags."),
+    rel: bool = typer.Option(False, "--rel", "-r", help="Show contents of <rel> tags."),
+    pas: bool = typer.Option(False, "--pas", help="Show predicate-argument structures."),
 ) -> None:
     """KNP ファイルを読み込み係り受けを可視化．
 
     Args:
         knp_path: KNP ファイルのパス．
         pos: True なら同時に品詞を表示．
-        rel: True なら同時に <rel> タグを表示．
+        rel: True なら同時に <rel> タグの内容を表示．
+        pas: True なら同時に述語項構造を表示．
     """
     doc = Document.from_knp(knp_path.read_text())
     for sent in doc.sentences:
         print(sent.comment)
-        draw_tree(sent.base_phrases, show_pos=pos, show_rel=rel)
+        draw_tree(sent.base_phrases, show_pos=pos, show_rel=rel, show_pas=pas)
 
 
 @app.command(help="Show statistics of given KNP file.")
 def stats(
     knp_path: Path = typer.Argument(
         ..., exists=True, dir_okay=False, help="Path to knp file to calculate statistics on."
     ),
@@ -72,20 +75,22 @@
 
 
 @app.command(help="Serve an analyzer as HTTP server.")
 def serve(
     analyzer: AnalyzerType = typer.Argument(..., help="Analyzer to use. Choose from jumanpp, knp, kwja."),
     host: str = typer.Option("localhost", "--host", "-h", help="Host to listen on."),
     port: int = typer.Option(8000, "--port", "-p", help="Port to listen on."),
+    analyzer_args: Optional[List[str]] = typer.Argument(None, help="Additional arguments for the analyzer."),
 ) -> None:
     """解析器を起動し，HTTP サーバとして提供．
 
     Args:
         analyzer: 解析器の種類．
         host: ホスト．
         port: ポート．
+        analyzer_args: 解析器のオプション．
     """
-    serve_analyzer(analyzer, host, port)  # pragma: no cover
+    serve_analyzer(analyzer, host, port, analyzer_args)  # pragma: no cover
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rhoknp-1.2.2/src/rhoknp/cli/show.py` & `rhoknp-1.3.0/src/rhoknp/cli/show.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 from typing import List, Sequence, TextIO, Union
 
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 
+from rhoknp.cohesion import EndophoraArgument
 from rhoknp.props.dependency import DepType
 from rhoknp.units.base_phrase import BasePhrase
 from rhoknp.units.phrase import Phrase
 
 POS_MARK = {
     "特殊": "*",
     "動詞": "v",
@@ -33,22 +34,24 @@
 
 
 def draw_tree(
     leaves: Union[Sequence[Phrase], Sequence[BasePhrase]],
     fh: TextIO = sys.stdout,
     show_pos: bool = False,
     show_rel: bool = False,
+    show_pas: bool = False,
 ) -> None:
     """構文木を指定された fh に出力．
 
     Args:
         leaves: 構文木の葉となる文節列または基本句列．
         fh: 出力先．
         show_pos: True なら同時に品詞を表示する．
-        show_rel: True なら同時に <rel> タグを表示する．
+        show_rel: True なら同時に <rel> タグの内容を表示する．
+        show_pas: True なら同時に述語項構造を表示する．
     """
     console = Console(file=fh)
     table = Table.grid(padding=(0, 2))
     limit = len(leaves)
     item = [[""] * limit for _ in leaves]
     active_column = [0] * limit
     limit -= 1
@@ -97,16 +100,16 @@
             line += _extend_horizontal(item[i][j]) + item[i][j]
         lines.append(line)
 
     max_length = max(_str_real_length(line) for line in lines)
     for line, leaf in zip(lines, leaves):
         diff = max_length - _str_real_length(line)
         tree_string = " " * diff + line
-        rel_string = _rel_string(leaf) if isinstance(leaf, BasePhrase) and show_rel is True else ""
-        table.add_row(Text(tree_string), Text(rel_string))
+        feat_string = _feat_string(leaf, show_rel, show_pas) if isinstance(leaf, BasePhrase) else ""
+        table.add_row(Text(tree_string), Text(feat_string))
     console.print(table)
 
 
 def _extend_horizontal(token: str) -> str:
     if token in ("╂", "┼", "┤", "┨", "┐", "─", "I", "A"):
         return "─"
     elif token in ("╋", "┿", "━", "P"):
@@ -127,9 +130,42 @@
     return ret
 
 
 def _str_real_length(string: str) -> int:
     return Text(string).cell_len
 
 
-def _rel_string(base_phrase: BasePhrase) -> str:
-    return " ".join(f"{tag.type}:{tag.target}" for tag in base_phrase.rel_tags)
+def _feat_string(base_phrase: BasePhrase, show_rel: bool, show_pas: bool) -> str:
+    tag_strings: List[str] = []
+    if show_rel is True:
+        for tag in base_phrase.rel_tags:
+            tag_strings.append(f"{tag.type}:{tag.target}")
+    if show_pas is True:
+        for case, arguments in base_phrase.pas.get_all_arguments(relax=False).items():
+            for arg in arguments:
+                core_text = _get_core_text(arg.base_phrase) if isinstance(arg, EndophoraArgument) else str(arg)
+                tag_string = f"{case}:{core_text}"
+                if tag_string not in tag_strings:
+                    tag_strings.append(tag_string)
+    return " ".join(tag_strings)
+
+
+def _get_core_text(base_phrase: BasePhrase) -> str:
+    """Get the core text without ancillary words."""
+    morphemes = base_phrase.morphemes
+    start_index = 0
+    for i, morpheme in enumerate(morphemes):
+        if morpheme.pos in ("助詞", "特殊", "判定詞"):
+            start_index += 1
+        else:
+            break
+    end_index = len(morphemes)
+    for i, morpheme in enumerate(reversed(morphemes)):
+        if morpheme.pos in ("助詞", "特殊", "判定詞"):
+            end_index -= 1
+        else:
+            break
+    ret = "".join(m.text for m in morphemes[start_index:end_index])
+    if not ret:
+        start_index = 0
+        end_index = len(morphemes)
+    return "".join(m.text for m in morphemes[start_index:end_index])
```

### Comparing `rhoknp-1.2.2/src/rhoknp/cli/stats.py` & `rhoknp-1.3.0/src/rhoknp/cli/stats.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/__init__.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/argument.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/argument.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/coreference.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/coreference.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/discourse.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/discourse.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/exophora.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/exophora.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/pas.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/pas.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/predicate.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/predicate.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/cohesion/rel.py` & `rhoknp-1.3.0/src/rhoknp/cohesion/rel.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/processors/jumanpp.py` & `rhoknp-1.3.0/src/rhoknp/processors/jumanpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import subprocess
 from subprocess import PIPE, Popen
 from threading import Lock
 from typing import List, Optional, Union
 
 from rhoknp.processors.processor import Processor
 from rhoknp.processors.senter import RegexSenter
 from rhoknp.units import Document, Sentence
@@ -120,11 +121,23 @@
             while self.is_available():
                 line = self._proc.stdout.readline()
                 jumanpp_text += line
                 if line.strip() == Sentence.EOS:
                     break
             return Sentence.from_jumanpp(jumanpp_text)
 
+    def get_version(self) -> str:
+        """Juman++ のバージョンを返す．"""
+        if not self.is_available():
+            raise RuntimeError("Juman++ is not available.")
+        p = subprocess.run(self.version_command, capture_output=True, encoding="utf-8")
+        return p.stdout.strip()
+
     @property
     def run_command(self) -> List[str]:
         """解析時に実行するコマンド．"""
         return [self.executable] + self.options
+
+    @property
+    def version_command(self) -> List[str]:
+        """バージョンを確認するコマンド．"""
+        return [self.executable, "--version"]
```

### Comparing `rhoknp-1.2.2/src/rhoknp/processors/knp.py` & `rhoknp-1.3.0/src/rhoknp/processors/knp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import subprocess
 from subprocess import PIPE, Popen
 from threading import Lock
 from typing import List, Optional, Union
 
 from rhoknp.processors.jumanpp import Jumanpp
 from rhoknp.processors.processor import Processor
 from rhoknp.processors.senter import RegexSenter
@@ -151,11 +152,23 @@
             while self.is_available():
                 line = self._proc.stdout.readline()
                 knp_text += line
                 if line.strip() == Sentence.EOS:
                     break
             return Sentence.from_knp(knp_text)
 
+    def get_version(self) -> str:
+        """Juman++ のバージョンを返す．"""
+        if not self.is_available():
+            raise RuntimeError("KNP is not available.")
+        p = subprocess.run(self.version_command, capture_output=True, encoding="utf-8")
+        return p.stderr.strip()
+
     @property
     def run_command(self) -> List[str]:
         """解析時に実行するコマンド．"""
         return [self.executable] + self.options
+
+    @property
+    def version_command(self) -> List[str]:
+        """バージョンを確認するコマンド．"""
+        return [self.executable, "-v"]
```

### Comparing `rhoknp-1.2.2/src/rhoknp/processors/kwja.py` & `rhoknp-1.3.0/src/rhoknp/processors/kwja.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import subprocess
 from subprocess import PIPE, Popen
 from threading import Lock
 from typing import List, Optional, Union
 
 from rhoknp.processors.processor import Processor
 from rhoknp.units import Document, Sentence
 
@@ -35,15 +36,18 @@
         self._proc: Optional[Popen] = None
         self._output_format = "knp"
         if "--tasks" in self.options:
             tasks: List[str] = self.options[self.options.index("--tasks") + 1].split(",")
             if "word" in tasks:
                 self._output_format = "knp"
             elif "char" in tasks:
+                self._output_format = "words"
                 raise ValueError(f"`--tasks {','.join(tasks)}` option is not supported yet in rhoknp.")
+            elif "seq2seq" in tasks:
+                self._output_format = "seq2seq"
             elif "typo" in tasks:
                 self._output_format = "raw"
             else:
                 raise ValueError(f"invalid task: {tasks}")
         try:
             self._proc = Popen(self.run_command, stdin=PIPE, stdout=PIPE, stderr=PIPE, encoding="utf-8")
         except Exception as e:
@@ -87,14 +91,16 @@
             while self.is_available():
                 line = self._proc.stdout.readline()
                 if line.strip() == Document.EOD:
                     break
                 out_text += line
             if self._output_format == "raw":
                 return Document.from_raw_text(out_text)
+            elif self._output_format == "seq2seq":
+                return Document.from_jumanpp(out_text)
             else:
                 assert self._output_format == "knp"
                 return Document.from_knp(out_text)
 
     def apply_to_sentence(self, sentence: Union[Sentence, str]) -> Sentence:
         """文に KWJA を適用する．
 
@@ -119,15 +125,29 @@
             while self.is_available():
                 line = self._proc.stdout.readline()
                 if line.strip() == Document.EOD:
                     break
                 out_text += line
             if self._output_format == "raw":
                 return Sentence.from_raw_text(out_text)
+            elif self._output_format == "seq2seq":
+                return Sentence.from_jumanpp(out_text)
             else:
                 assert self._output_format == "knp"
                 return Sentence.from_knp(out_text)
 
+    def get_version(self) -> str:
+        """Juman++ のバージョンを返す．"""
+        if not self.is_available():
+            raise RuntimeError("KWJA is not available.")
+        p = subprocess.run(self.version_command, capture_output=True, encoding="utf-8")
+        return p.stdout.strip()
+
     @property
     def run_command(self) -> List[str]:
         """解析時に実行するコマンド．"""
         return [self.executable] + self.options
+
+    @property
+    def version_command(self) -> List[str]:
+        """バージョンを確認するコマンド．"""
+        return [self.executable, "--version"]
```

### Comparing `rhoknp-1.2.2/src/rhoknp/processors/processor.py` & `rhoknp-1.3.0/src/rhoknp/processors/processor.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/props/feature.py` & `rhoknp-1.3.0/src/rhoknp/props/feature.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/props/memo.py` & `rhoknp-1.3.0/src/rhoknp/props/memo.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/props/named_entity.py` & `rhoknp-1.3.0/src/rhoknp/props/named_entity.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/props/semantics.py` & `rhoknp-1.3.0/src/rhoknp/props/semantics.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/units/base_phrase.py` & `rhoknp-1.3.0/src/rhoknp/units/base_phrase.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/units/clause.py` & `rhoknp-1.3.0/src/rhoknp/units/clause.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/units/document.py` & `rhoknp-1.3.0/src/rhoknp/units/document.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/units/morpheme.py` & `rhoknp-1.3.0/src/rhoknp/units/morpheme.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/units/phrase.py` & `rhoknp-1.3.0/src/rhoknp/units/phrase.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/units/sentence.py` & `rhoknp-1.3.0/src/rhoknp/units/sentence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 import re
-from typing import TYPE_CHECKING, Any, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from rhoknp.cohesion import EntityManager, Pas
 from rhoknp.props.named_entity import NamedEntity
 from rhoknp.units.base_phrase import BasePhrase
 from rhoknp.units.clause import Clause
 from rhoknp.units.morpheme import Morpheme
 from rhoknp.units.phrase import Phrase
 from rhoknp.units.unit import Unit
+from rhoknp.utils.util import _extract_did_and_sid
 
 if TYPE_CHECKING:
     from rhoknp.units.document import Document
 
 logger = logging.getLogger(__name__)
 
 
@@ -20,15 +21,15 @@
     """文クラス．
 
     Args:
         text: 文の文字列．
     """
 
     EOS = "EOS"
-    SID_PAT = re.compile(r"^(?P<sid>(?P<did>[a-zA-Z\d\-_]+?)(-(\d+))?)$")
+    SID_PAT = re.compile(r"^(?P<sid>(?P<did>[a-zA-Z\d\-_]*?)-?\d*)$")
     SID_PAT_KWDLC = re.compile(r"^(?P<sid>(?P<did>w\d{6}-\d{10})(-\d+){1,2})$")
     SID_PAT_WAC = re.compile(r"^(?P<sid>(?P<did>wiki\d{8})(-\d{2})(-\d{2})?)$")
     count = 0
 
     def __init__(self, text: Optional[str] = None):
         super().__init__()
         if text is not None:
@@ -247,15 +248,17 @@
     @comment.setter
     def comment(self, comment: str) -> None:
         """コメント行．
 
         Args:
             comment: コメント行．
         """
-        doc_id, sent_id, rest = self._extract_sid(comment)
+        doc_id, sent_id, rest = _extract_did_and_sid(
+            comment, patterns=[self.SID_PAT_KWDLC, self.SID_PAT_WAC, self.SID_PAT]
+        )
         if sent_id is not None:
             self.sent_id = sent_id
         if doc_id is not None:
             self.doc_id = doc_id
         self.misc_comment = rest
 
     @property
@@ -440,45 +443,14 @@
             sentence.clauses = clauses
         else:
             sentence.phrases = phrases
         if post_init is True:
             sentence.__post_init__()
         return sentence
 
-    @staticmethod
-    def _extract_sid(comment: str) -> Tuple[Optional[str], Optional[str], str]:
-        """Extract sentence id and document id from comment line.
-
-        Args:
-            comment: A comment line.
-
-        Returns:
-            Optional[str]: Document id if exists; otherwise, None.
-            Optional[str]: Sentence id if exists; otherwise, None.
-            str: The rest of the comment line.
-        """
-        assert comment.startswith("#")
-        match_sid = re.match(r"# S-ID: ?(\S*)( .+)?$", comment)
-        if match_sid is not None:
-            sid_string = match_sid[1]
-            match = (
-                Sentence.SID_PAT_KWDLC.match(sid_string)
-                or Sentence.SID_PAT_WAC.match(sid_string)
-                or Sentence.SID_PAT.match(sid_string)
-            )
-            if match is not None:
-                return (
-                    match["did"],
-                    match["sid"],
-                    match_sid[2].lstrip() if match_sid[2] else "",
-                )
-            else:
-                logger.warning(f"unsupported S-ID format: {sid_string}")
-        return None, None, comment.lstrip("#").lstrip()
-
     def to_raw_text(self) -> str:
         """生テキストフォーマットに変換．"""
         ret = ""
         if self.comment != "":
             ret += self.comment + "\n"
         ret += self.text.rstrip("\n") + "\n"
         return ret
```

### Comparing `rhoknp-1.2.2/src/rhoknp/units/unit.py` & `rhoknp-1.3.0/src/rhoknp/units/unit.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.2.2/src/rhoknp/utils/reader.py` & `rhoknp-1.3.0/src/rhoknp/utils/reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import re
+from functools import partial
 from typing import Callable, Iterator, List, Optional, TextIO, Union
 
 from rhoknp import Sentence
+from rhoknp.utils.util import _extract_did_and_sid
 
 logger = logging.getLogger(__name__)
 
 
 def chunk_by_sentence(f: TextIO) -> Iterator[str]:
     """解析結果ファイルを文ごとに分割するジェネレータ．
 
@@ -57,21 +59,22 @@
 
         関数が指定された場合，文解析結果の先頭行から文書IDを取り出す関数とみなす．
         例えば default 相当の処理を行うには以下のような関数を渡す．
 
             >>> def default_doc_id_format(line: str) -> str:
             ...     return line.lstrip("# S-ID:").rsplit("-", maxsplit=1)[0]
     """
+    extract_doc_id: Callable[[str], Optional[str]]
     if isinstance(doc_id_format, str):
         if doc_id_format == "default":
-            extract_doc_id = _extract_doc_id(Sentence.SID_PAT)
+            extract_doc_id = partial(_extract_doc_id, pat=Sentence.SID_PAT)
         elif doc_id_format == "kwdlc":
-            extract_doc_id = _extract_doc_id(Sentence.SID_PAT_KWDLC)
+            extract_doc_id = partial(_extract_doc_id, pat=Sentence.SID_PAT_KWDLC)
         elif doc_id_format == "wac":
-            extract_doc_id = _extract_doc_id(Sentence.SID_PAT_WAC)
+            extract_doc_id = partial(_extract_doc_id, pat=Sentence.SID_PAT_WAC)
         else:
             raise ValueError(f"Invalid doc_id_format: {doc_id_format}")
     elif callable(doc_id_format):
         extract_doc_id = doc_id_format
     else:
         raise TypeError(f"Invalid doc_id_format: {doc_id_format}")
 
@@ -84,26 +87,16 @@
             buffer = []
         buffer.append(sentence)
         prev_doc_id = doc_id
     if buffer:
         yield "".join(buffer)
 
 
-def _extract_doc_id(pat: re.Pattern) -> Callable[[str], Optional[str]]:
-    """文書IDを抽出する関数を返す．
+def _extract_doc_id(line: str, pat: re.Pattern) -> Optional[str]:
+    """文書IDを抽出する．
 
     Args:
+        line: 文IDが含まれるコメント行．
         pat: 文書IDを抽出する正規表現．
     """
-
-    def extract_doc_id(line: str) -> Optional[str]:
-        match_sid = re.match(r"# S-ID: ?(\S*)( .+)?$", line)
-        if match_sid:
-            sid_string = match_sid[1]
-            match = pat.match(sid_string)
-            if match is None:
-                logger.warning(f"Invalid S-ID: {sid_string}")
-                return None
-            return match["did"]
-        return None
-
-    return extract_doc_id
+    did, _, _ = _extract_did_and_sid(line, [pat])
+    return did
```

### Comparing `rhoknp-1.2.2/PKG-INFO` & `rhoknp-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhoknp
-Version: 1.2.2
+Version: 1.3.0
 Summary: Yet another Python binding for Juman++/KNP/KWJA
 Home-page: https://github.com/ku-nlp/rhoknp
 License: MIT
 Keywords: NLP
 Author: Hirokazu Kiyomaru
 Author-email: h.kiyomaru@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
 Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "cli"
 Requires-Dist: cached-property (>=1.5,<2.0) ; python_version < "3.8"
 Requires-Dist: fastapi (>=0.92.0,<1) ; extra == "cli"
 Requires-Dist: importlib-metadata (>=5.2) ; python_version < "3.8"
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "cli"
 Requires-Dist: rich (>=12.6) ; extra == "cli"
 Requires-Dist: typer (>=0.6.1,<0.8) ; extra == "cli"
 Requires-Dist: uvicorn (>=0.21.0,<1) ; extra == "cli"
 Project-URL: Documentation, https://rhoknp.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/ku-nlp/rhoknp
 Description-Content-Type: text/markdown
 
@@ -41,15 +42,15 @@
 <a href="https://www.codefactor.io/repository/github/ku-nlp/rhoknp"><img alt="CodeFactor" src="https://img.shields.io/codefactor/grade/github/ku-nlp/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rhoknp?style=flat-square"></a>
 <a href="https://pypi.org/project/rhoknp/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/rhoknp?style=flat-square">
 <a href="https://rhoknp.readthedocs.io/en/latest/"><img alt="Documentation" src="https://img.shields.io/readthedocs/rhoknp?style=flat-square"></a>
 <a href="https://github.com/psf/black"><img alt="Code style - black" src="https://img.shields.io/badge/code%20style-black-222222?style=flat-square"></a>
 </p>
 
-*rhoknp* is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1]
+_rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp), [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/kwja).[^1]
 
 [^1]: The logo was originally generated using OpenAI DALL·E 2
 
 ```python
 import rhoknp
 
 # Perform language analysis by Juman++
@@ -89,15 +90,15 @@
 
 ## Documentation
 
 [https://rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/)
 
 ## Quick tour
 
-Let's start with using Juman++ with *rhoknp*.
+Let's start with using Juman++ with _rhoknp_.
 Here is a simple example of using Juman++ to analyze a sentence.
 
 ```python
 # Perform language analysis by Juman++
 jumanpp = rhoknp.Jumanpp()
 sentence = jumanpp.apply_to_sentence("電気抵抗率は電気の通しにくさを表す物性値である。")
 ```
@@ -150,15 +151,15 @@
     f.write(sentence.to_knp())
 
 # Load the sentence
 with open("sentence.knp", "rt") as f:
     sentence = rhoknp.Sentence.from_knp(f.read())
 ```
 
-*rhoknp* also provides APIs for document-level language analysis.
+_rhoknp_ also provides APIs for document-level language analysis.
 
 ```python
 document = rhoknp.Document.from_raw_text(
     "電気抵抗率は電気の通しにくさを表す物性値である。単に抵抗率とも呼ばれる。"
 )
 # If you know sentence boundaries, you can use `Document.from_sentences` instead.
 document = rhoknp.Document.from_sentences(
@@ -190,29 +191,29 @@
     document = rhoknp.Document.from_jumanpp(f.read())
 ```
 
 For more information, explore the [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/latest/).
 
 ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
 
-[*pyknp*](https://pypi.org/project/pyknp/) has been developed as the official Python binding for Juman++ and KNP.
-In *rhoknp*, we redesigned the API from the top-down, taking into account the current use cases of *pyknp*.
+[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official Python binding for Juman++ and KNP.
+In _rhoknp_, we redesigned the API from the top-down, taking into account the current use cases of _pyknp_.
 The main differences are as follows:
 
-- **Support for document-level language analysis**: *rhoknp* can load and instantiate the result of document-level language analysis (i.e., cohesion analysis and discourse relation analysis).
-- **Strictly type-aware**: *rhoknp* is thoroughly annotated with type annotations.
-- **Extensive test suite**: *rhoknp* is tested with an extensive test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
+- **Support for document-level language analysis**: _rhoknp_ can load and instantiate the result of document-level language analysis (i.e., cohesion analysis and discourse relation analysis).
+- **Strictly type-aware**: _rhoknp_ is thoroughly annotated with type annotations.
+- **Extensive test suite**: _rhoknp_ is tested with an extensive test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-nlp/rhoknp).
 
 ## License
 
 MIT
 
 ## Contributing
 
-We welcome contributions to *rhoknp*.
+We welcome contributions to _rhoknp_.
 You can get started by reading the [contribution guide](https://rhoknp.readthedocs.io/en/latest/contributing/index.html).
 
 ## Reference
 
 - [KNP FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html)
 - [KNP - KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: rhoknp Version: 1.2.2 Summary: Yet another Python
+Metadata-Version: 2.1 Name: rhoknp Version: 1.3.0 Summary: Yet another Python
 binding for Juman++/KNP/KWJA Home-page: https://github.com/ku-nlp/rhoknp
 License: MIT Keywords: NLP Author: Hirokazu Kiyomaru Author-email:
 h.kiyomaru@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: cli Requires-Dist: PyYAML
 (>=6.0,<7.0) ; extra == "cli" Requires-Dist: cached-property (>=1.5,<2.0) ;
 python_version < "3.8" Requires-Dist: fastapi (>=0.92.0,<1) ; extra == "cli"
 Requires-Dist: importlib-metadata (>=5.2) ; python_version < "3.8" Requires-
-Dist: rich (>=12.6) ; extra == "cli" Requires-Dist: typer (>=0.6.1,<0.8) ;
-extra == "cli" Requires-Dist: uvicorn (>=0.21.0,<1) ; extra == "cli" Project-
-URL: Documentation, https://rhoknp.readthedocs.io/en/latest Project-URL:
-Repository, https://github.com/ku-nlp/rhoknp Description-Content-Type: text/
-markdown
+Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "cli" Requires-Dist: rich (>=12.6) ;
+extra == "cli" Requires-Dist: typer (>=0.6.1,<0.8) ; extra == "cli" Requires-
+Dist: uvicorn (>=0.21.0,<1) ; extra == "cli" Project-URL: Documentation, https:
+//rhoknp.readthedocs.io/en/latest Project-URL: Repository, https://github.com/
+ku-nlp/rhoknp Description-Content-Type: text/markdown
                                  [rhoknp_logo]
      ****** rhoknp: Yet another Python binding for Juman++/KNP/KWJA ******
  [Test] [Codecov] [CodeFactor] [PyPI] [PyPI_-_Python_Version]_[Documentation]_
                              [Code_style_-_black]
-*rhoknp* is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
+_rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
 [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/
 kwja).[^1] [^1]: The logo was originally generated using OpenAI DALLÂ·E 2
 ```python import rhoknp # Perform language analysis by Juman++ jumanpp =
 rhoknp.Jumanpp() sentence = jumanpp.apply_to_sentence
 ( "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã" )
 # Access to the result for morpheme in sentence.morphemes: # a.k.a. keitai-so
 ... # Save language analysis by Juman++ with open("result.jumanpp", "wt") as f:
 f.write(sentence.to_jumanpp()) # Load language analysis by Juman++ with open
 ("result.jumanpp", "rt") as f: sentence = rhoknp.Sentence.from_jumanpp(f.read
 ()) ``` ## Requirements - Python 3.7+ ## Optional requirements for language
 analysis - [Juman++](https://github.com/ku-nlp/jumanpp) v2.0.0-rc3+ - [KNP]
 (https://github.com/ku-nlp/knp) 5.0+ - [KWJA](https://github.com/ku-nlp/kwja)
 1.0.0+ ## Installation ```shell pip install rhoknp ``` ## Documentation [https:
 //rhoknp.readthedocs.io/en/latest/](https://rhoknp.readthedocs.io/en/latest/
-) ## Quick tour Let's start with using Juman++ with *rhoknp*. Here is a simple
+) ## Quick tour Let's start with using Juman++ with _rhoknp_. Here is a simple
 example of using Juman++ to analyze a sentence. ```python # Perform language
 analysis by Juman++ jumanpp = rhoknp.Jumanpp() sentence =
 jumanpp.apply_to_sentence
 ("é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã")
 ``` You can easily access the morphemes that make up the sentence. ```python
 for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
 can be saved in the JUMAN format. ```python # Save the sentence in the JUMAN
@@ -51,15 +51,15 @@
 ``` KNP performs language analysis at multiple levels. ```python for clause in
 sentence.clauses: # a.k.a., setsu ... for phrase in sentence.phrases: # a.k.a.
 bunsetsu ... for base_phrase in sentence.base_phrases: # a.k.a. kihon-ku ...
 for morpheme in sentence.morphemes: # a.k.a. keitai-so ... ``` Sentence objects
 can be saved in the KNP format. ```python # Save the sentence in the KNP format
 with open("sentence.knp", "wt") as f: f.write(sentence.to_knp()) # Load the
 sentence with open("sentence.knp", "rt") as f: sentence =
-rhoknp.Sentence.from_knp(f.read()) ``` *rhoknp* also provides APIs for
+rhoknp.Sentence.from_knp(f.read()) ``` _rhoknp_ also provides APIs for
 document-level language analysis. ```python document =
 rhoknp.Document.from_raw_text
 (
 "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ãããåã«æµæçã¨ãå¼ã°ããã"
 ) # If you know sentence boundaries, you can use `Document.from_sentences`
 instead. document = rhoknp.Document.from_sentences(
 [ "é»æ°æµæçã¯é»æ°ã®éãã«ãããè¡¨ãç©æ§å¤ã§ããã",
@@ -69,21 +69,21 @@
 language units in the document for sentence in document.sentences: ... for
 morpheme in document.morphemes: ... # Save language analysis by Juman++ with
 open("document.jumanpp", "wt") as f: f.write(document.to_jumanpp()) # Load
 language analysis by Juman++ with open("document.jumanpp", "rt") as f: document
 = rhoknp.Document.from_jumanpp(f.read()) ``` For more information, explore the
 [examples](./examples) and [documentation](https://rhoknp.readthedocs.io/en/
 latest/). ## Main differences from [pyknp](https://github.com/ku-nlp/pyknp/)
-[*pyknp*](https://pypi.org/project/pyknp/) has been developed as the official
-Python binding for Juman++ and KNP. In *rhoknp*, we redesigned the API from the
-top-down, taking into account the current use cases of *pyknp*. The main
+[_pyknp_](https://pypi.org/project/pyknp/) has been developed as the official
+Python binding for Juman++ and KNP. In _rhoknp_, we redesigned the API from the
+top-down, taking into account the current use cases of _pyknp_. The main
 differences are as follows: - **Support for document-level language analysis**:
-*rhoknp* can load and instantiate the result of document-level language
+_rhoknp_ can load and instantiate the result of document-level language
 analysis (i.e., cohesion analysis and discourse relation analysis). -
-**Strictly type-aware**: *rhoknp* is thoroughly annotated with type
-annotations. - **Extensive test suite**: *rhoknp* is tested with an extensive
+**Strictly type-aware**: _rhoknp_ is thoroughly annotated with type
+annotations. - **Extensive test suite**: _rhoknp_ is tested with an extensive
 test suite. See the code coverage at [Codecov](https://app.codecov.io/gh/ku-
 nlp/rhoknp). ## License MIT ## Contributing We welcome contributions to
-*rhoknp*. You can get started by reading the [contribution guide](https://
+_rhoknp_. You can get started by reading the [contribution guide](https://
 rhoknp.readthedocs.io/en/latest/contributing/index.html). ## Reference - [KNP
 FORMAT](http://cr.fvcrc.i.nagoya-u.ac.jp/~sasano/knp/format.html) - [KNP -
 KUROHASHI-CHU-MURAWAKI LAB](https://nlp.ist.i.kyoto-u.ac.jp/?KNP)
```

