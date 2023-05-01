# Comparing `tmp/spaczz-0.5.4.tar.gz` & `tmp/spaczz-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaczz-0.5.4.tar", max compression
+gzip compressed data, was "spaczz-0.6.0a0.tar", max compression
```

## Comparing `spaczz-0.5.4.tar` & `spaczz-0.6.0a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1086 2021-12-23 19:29:52.719191 spaczz-0.5.4/LICENSE
--rw-r--r--   0        0        0    36223 2021-12-23 19:29:52.719191 spaczz-0.5.4/README.md
--rw-r--r--   0        0        0     1549 2021-12-23 19:29:52.723191 spaczz-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      481 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/__init__.py
--rw-r--r--   0        0        0     5676 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/customattrs.py
--rw-r--r--   0        0        0      982 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/exceptions.py
--rw-r--r--   0        0        0      358 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/matcher/__init__.py
--rw-r--r--   0        0        0    13095 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/matcher/_phrasematcher.py
--rw-r--r--   0        0        0     1942 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/matcher/fuzzymatcher.py
--rw-r--r--   0        0        0    13535 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/matcher/regexmatcher.py
--rw-r--r--   0        0        0     1997 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/matcher/similaritymatcher.py
--rw-r--r--   0        0        0    12815 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/matcher/tokenmatcher.py
--rw-r--r--   0        0        0      102 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/pipeline/__init__.py
--rw-r--r--   0        0        0    36072 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/pipeline/_spaczzruler.py
--rw-r--r--   0        0        0    28837 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/pipeline/_spaczzruler_legacy.py
--rw-r--r--   0        0        0      664 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/pipeline/spaczzruler.py
--rw-r--r--   0        0        0     3939 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/process.py
--rw-r--r--   0        0        0      100 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/regex/__init__.py
--rw-r--r--   0        0        0     6686 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/regex/_commonregex.py
--rw-r--r--   0        0        0     3517 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/regex/regexconfig.py
--rw-r--r--   0        0        0      382 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/search/__init__.py
--rw-r--r--   0        0        0    15263 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/search/_phrasesearcher.py
--rw-r--r--   0        0        0     4366 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/search/fuzzysearcher.py
--rw-r--r--   0        0        0     5517 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/search/regexsearcher.py
--rw-r--r--   0        0        0     3478 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/search/similaritysearcher.py
--rw-r--r--   0        0        0     9058 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/search/tokensearcher.py
--rw-r--r--   0        0        0     1854 2021-12-23 19:29:52.723191 spaczz-0.5.4/src/spaczz/util.py
--rw-r--r--   0        0        0    38425 2021-12-23 19:37:28.684405 spaczz-0.5.4/setup.py
--rw-r--r--   0        0        0    37177 2021-12-23 19:37:28.686713 spaczz-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-01 12:42:21.748603 spaczz-0.6.0a0/LICENSE
+-rw-r--r--   0        0        0    35958 2023-05-01 12:42:21.748603 spaczz-0.6.0a0/README.md
+-rw-r--r--   0        0        0     2717 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0      531 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/__init__.py
+-rw-r--r--   0        0        0      379 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/__init__.py
+-rw-r--r--   0        0        0     2292 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/fuzzysearcher.py
+-rw-r--r--   0        0        0    11289 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/phrasesearcher.py
+-rw-r--r--   0        0        0     5090 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/regexsearcher.py
+-rw-r--r--   0        0        0     3098 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/searchutil.py
+-rw-r--r--   0        0        0     1814 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/similaritysearcher.py
+-rw-r--r--   0        0        0     8592 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/_search/tokensearcher.py
+-rw-r--r--   0        0        0     4681 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/customattrs.py
+-rw-r--r--   0        0        0      813 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/customtypes.py
+-rw-r--r--   0        0        0      783 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/exceptions.py
+-rw-r--r--   0        0        0      293 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/matcher/__init__.py
+-rw-r--r--   0        0        0     6721 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/matcher/_phrasematcher.py
+-rw-r--r--   0        0        0     9666 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/matcher/fuzzymatcher.py
+-rw-r--r--   0        0        0    12699 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/matcher/regexmatcher.py
+-rw-r--r--   0        0        0     9537 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/matcher/similaritymatcher.py
+-rw-r--r--   0        0        0    13716 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/matcher/tokenmatcher.py
+-rw-r--r--   0        0        0      102 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/pipeline/__init__.py
+-rw-r--r--   0        0        0    37739 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/pipeline/spaczzruler.py
+-rw-r--r--   0        0        0        0 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/py.typed
+-rw-r--r--   0        0        0      397 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/registry/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/registry/fuzzyfuncs.py
+-rw-r--r--   0        0        0     7125 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/registry/repatterns.py
+-rw-r--r--   0        0        0      330 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/registry/reweights.py
+-rw-r--r--   0        0        0     1690 2023-05-01 12:42:21.752603 spaczz-0.6.0a0/src/spaczz/util.py
+-rw-r--r--   0        0        0    37403 1970-01-01 00:00:00.000000 spaczz-0.6.0a0/PKG-INFO
```

### Comparing `spaczz-0.5.4/LICENSE` & `spaczz-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `spaczz-0.5.4/README.md` & `spaczz-0.6.0a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,110 @@
-[![Tests](https://github.com/gandersen101/spaczz/workflows/Tests/badge.svg)](https://github.com/gandersen101/spaczz/actions?workflow=Tests)
+[![Tests](https://github.com/gandersen101/spaczz/workflows/Lint,%20Typecheck%20and%20Test/badge.svg)](https://github.com/gandersen101/spaczz/actions?workflow=Lint,%20Typecheck%20and%20Test)
 [![Codecov](https://codecov.io/gh/gandersen101/spaczz/branch/master/graph/badge.svg)](https://codecov.io/gh/gandersen101/spaczz)
 [![PyPI](https://img.shields.io/pypi/v/spaczz.svg)](https://pypi.org/project/spaczz/)
 [![Read the Docs](https://readthedocs.org/projects/spaczz/badge/)](https://spaczz.readthedocs.io/)
 
 # spaczz: Fuzzy matching and more for spaCy
 
-Spaczz provides fuzzy matching and additional regex matching functionality for [spaCy](https://spacy.io/).
-Spaczz's components have similar APIs to their spaCy counterparts and spaczz pipeline components can integrate into spaCy pipelines where they can be saved/loaded as models.
+spaczz provides fuzzy matching and additional regex matching functionality for [spaCy](https://spacy.io/).
+spaczz's components have similar APIs to their spaCy counterparts and spaczz pipeline components can integrate into spaCy pipelines where they can be saved/loaded as models.
 
-Fuzzy matching is currently performed with matchers from [RapidFuzz](https://github.com/maxbachmann/rapidfuzz)'s fuzz module and regex matching currently relies on the [regex](https://pypi.org/project/regex/) library. Spaczz certainly takes additional influence from other libraries and resources. For additional details see the references section.
+Fuzzy matching is currently performed with matchers from [RapidFuzz](https://github.com/maxbachmann/rapidfuzz)'s fuzz module and regex matching currently relies on the [regex](https://pypi.org/project/regex/) library. spaczz certainly takes additional influence from other libraries and resources. For additional details see the references section.
 
-**Supports spaCy v3 and v2 (>= 2.2)!**
+**Supports spaCy >= 3.0**
 
-Spaczz has been tested on Ubuntu 20.04, MacOS 10.15, and Windows Server 2019.
+spaczz has been tested on Ubuntu, MacOS, and Windows Server.
 
-*v0.5.4 Release Notes:*
-- BugFix for german Combination words for RegexSearcher.
-- Other minor docs/tooling updates.
-
-*v0.5.3 Release Notes:*
-- *Fixed a "bug" in the `TokenMatcher`. Spaczz expects token matches returned in order of ascending match start, then descending match length. However, spaCy's `Matcher` does not return matches in this order by default. Added a sort in the `TokenMatcher` to ensure this.*
+*v0.6.0 Release Notes:*
+- *Returning the matching pattern for all matchers, this is a breaking change as matches are now tuples of length 5 instead of 4.*
+- *Regex and token matches now return match ratios.*
+- *Support for `python<=3.11,>=3.7`, along with `rapidfuzz>=1.0.0`.
+- *Dropped support for spaCy v2. Sorry to do this without a deprecation cycle, but I stepped away from this project for a long time.*
+- *Removed support of `"spaczz_"` preprended optional `SpaczzRuler` init arguments. Also, sorry to do this without a deprecation cycle.*
+- *`Matcher.pipe` methods, which were deprecated, are now removed.
+- *`spaczz_span` custom attribute, which was deprecated, is now removed.
 
 Please see the [changelog](https://github.com/gandersen101/spaczz/blob/master/CHANGELOG.md) for previous release notes. This will eventually be moved to the [Read the Docs](https://spaczz.readthedocs.io/en/latest/) page.
 
 <h1>Table of Contents<span class="tocSkip"></span></h1>
-<div class="toc"><ul class="toc-item"><li><span><a href="#Installation" data-toc-modified-id="Installation-1">Installation</a></span></li><li><span><a href="#Basic-Usage" data-toc-modified-id="Basic-Usage-2">Basic Usage</a></span><ul class="toc-item"><li><span><a href="#FuzzyMatcher" data-toc-modified-id="FuzzyMatcher-2.1">FuzzyMatcher</a></span></li><li><span><a href="#RegexMatcher" data-toc-modified-id="RegexMatcher-2.2">RegexMatcher</a></span></li><li><span><a href="#SimilarityMatcher" data-toc-modified-id="SimilarityMatcher-2.3">SimilarityMatcher</a></span></li><li><span><a href="#TokenMatcher" data-toc-modified-id="TokenMatcher-2.4">TokenMatcher</a></span></li><li><span><a href="#SpaczzRuler" data-toc-modified-id="SpaczzRuler-2.5">SpaczzRuler</a></span></li><li><span><a href="#Custom-Attributes" data-toc-modified-id="Custom-Attributes-2.6">Custom Attributes</a></span></li><li><span><a href="#Saving/Loading" data-toc-modified-id="Saving/Loading-2.7">Saving/Loading</a></span></li></ul></li><li><span><a href="#Known-Issues" data-toc-modified-id="Known-Issues-3">Known Issues</a></span><ul class="toc-item"><li><span><a href="#Performance" data-toc-modified-id="Performance-3.1">Performance</a></span></li><li><span><a href="#SpaczzRuler-Inconsistencies" data-toc-modified-id="SpaczzRuler-Inconsistencies-3.2">SpaczzRuler Inconsistencies</a></span></li></ul></li><li><span><a href="#Roadmap" data-toc-modified-id="Roadmap-4">Roadmap</a></span></li><li><span><a href="#Development" data-toc-modified-id="Development-5">Development</a></span></li><li><span><a href="#References" data-toc-modified-id="References-6">References</a></span></li></ul></div>
+<div class="toc"><ul class="toc-item"><li><span><a href="#Installation" data-toc-modified-id="Installation-1">Installation</a></span></li><li><span><a href="#Basic-Usage" data-toc-modified-id="Basic-Usage-2">Basic Usage</a></span><ul class="toc-item"><li><span><a href="#FuzzyMatcher" data-toc-modified-id="FuzzyMatcher-2.1">FuzzyMatcher</a></span></li><li><span><a href="#RegexMatcher" data-toc-modified-id="RegexMatcher-2.2">RegexMatcher</a></span></li><li><span><a href="#SimilarityMatcher" data-toc-modified-id="SimilarityMatcher-2.3">SimilarityMatcher</a></span></li><li><span><a href="#TokenMatcher" data-toc-modified-id="TokenMatcher-2.4">TokenMatcher</a></span></li><li><span><a href="#SpaczzRuler" data-toc-modified-id="SpaczzRuler-2.5">SpaczzRuler</a></span></li><li><span><a href="#Custom-Attributes" data-toc-modified-id="Custom-Attributes-2.6">Custom Attributes</a></span></li><li><span><a href="#Saving/Loading" data-toc-modified-id="Saving/Loading-2.7">Saving/Loading</a></span></li></ul></li><li><span><a href="#Known-Issues" data-toc-modified-id="Known-Issues-3">Known Issues</a></span><ul class="toc-item"><li><span><a href="#Performance" data-toc-modified-id="Performance-3.1">Performance</a></span></li></ul></li><li><span><a href="#Roadmap" data-toc-modified-id="Roadmap-4">Roadmap</a></span></li><li><span><a href="#Development" data-toc-modified-id="Development-5">Development</a></span></li><li><span><a href="#References" data-toc-modified-id="References-6">References</a></span></li></ul></div>
 
 ## Installation
 
 Spaczz can be installed using pip.
 
-
 ```python
 pip install spaczz
 ```
 
 ## Basic Usage
 
 Spaczz's primary features are the `FuzzyMatcher`, `RegexMatcher`, and "fuzzy" `TokenMatcher` that function similarly to spaCy's `Matcher` and `PhraseMatcher`, and the `SpaczzRuler` which integrates the spaczz matchers into a spaCy pipeline component similar to spaCy's `EntityRuler`.
 
 ### FuzzyMatcher
 
-The basic usage of the fuzzy matcher is similar to spaCy's `PhraseMatcher` except it returns the fuzzy ratio along with match id, start and end information, so make sure to include a variable for the ratio when unpacking results.
+The basic usage of the fuzzy matcher is similar to spaCy's `PhraseMatcher` except it returns the fuzzy ratio and matched pattern, along with match id, start and end information, so make sure to include variables for the ratio and pattern when unpacking results.
 
 
 ```python
 import spacy
 from spaczz.matcher import FuzzyMatcher
 
 nlp = spacy.blank("en")
-text = """Grint Anderson created spaczz in his home at 555 Fake St,
+text = """Grint M Anderson created spaczz in his home at 555 Fake St,
 Apt 5 in Nashv1le, TN 55555-1234 in the US."""  # Spelling errors intentional.
 doc = nlp(text)
 
 matcher = FuzzyMatcher(nlp.vocab)
 matcher.add("NAME", [nlp("Grant Andersen")])
 matcher.add("GPE", [nlp("Nashville")])
 matches = matcher(doc)
 
-for match_id, start, end, ratio in matches:
-    print(match_id, doc[start:end], ratio)
+for match_id, start, end, ratio, pattern in matches:
+    print(match_id, doc[start:end], ratio, pattern)
 ```
 
-    NAME Grint Anderson 86
-    GPE Nashv1le 82
+    NAME Grint M Anderson 80 Grant Andersen
+    GPE Nashv1le 82 Nashville
 
 
 Unlike spaCy matchers, spaczz matchers are written in pure Python. While they are required to have a spaCy vocab passed to them during initialization, this is purely for consistency as the spaczz matchers do not use currently use the spaCy vocab. This is why the `match_id` above is simply a string instead of an integer value like in spaCy matchers.
 
 Spaczz matchers can also make use of on-match rules via callback functions. These on-match callbacks need to accept the matcher itself, the doc the matcher was called on, the match index and the matches produced by the matcher.
 
 
 ```python
 import spacy
 from spacy.tokens import Span
 from spaczz.matcher import FuzzyMatcher
 
 nlp = spacy.blank("en")
-text = """Grint Anderson created spaczz in his home at 555 Fake St,
+text = """Grint M Anderson created spaczz in his home at 555 Fake St,
 Apt 5 in Nashv1le, TN 55555-1234 in the US."""  # Spelling errors intentional.
 doc = nlp(text)
 
 
 def add_name_ent(matcher, doc, i, matches):
     """Callback on match function. Adds "NAME" entities to doc."""
     # Get the current match and create tuple of entity label, start and end.
     # Append entity to the doc's entity. (Don't overwrite doc.ents!)
-    _match_id, start, end, _ratio = matches[i]
+    _match_id, start, end, _ratio, _pattern = matches[i]
     entity = Span(doc, start, end, label="NAME")
     doc.ents += (entity,)
 
 
 matcher = FuzzyMatcher(nlp.vocab)
 matcher.add("NAME", [nlp("Grant Andersen")], on_match=add_name_ent)
 matches = matcher(doc)
 
 for ent in doc.ents:
     print((ent.text, ent.start, ent.end, ent.label_))
 ```
 
-    ('Grint Anderson', 0, 2, 'NAME')
+    ('Grint M Anderson', 0, 3, 'NAME')
 
 
 Like spaCy's `EntityRuler`, a very similar entity updating logic has been implemented in the `SpaczzRuler`. The `SpaczzRuler` also takes care of handling overlapping matches. It is discussed in a later section.
 
 Unlike spaCy's matchers, rules added to spaczz matchers have optional keyword arguments that can modify the matching behavior. Take the below fuzzy matching examples:
 
 
@@ -118,19 +119,19 @@
 doc = nlp(text)
 
 matcher = FuzzyMatcher(nlp.vocab)
 matcher.add("NAME", [nlp("Grant Andersen")])
 matches = matcher(doc)
 
 # The default fuzzy matching settings will not find a match.
-for match_id, start, end, ratio in matches:
-    print(match_id, doc[start:end], ratio)
+for match_id, start, end, ratio, pattern in matches:
+    print(match_id, doc[start:end], ratio, pattern)
 ```
 
-Next we change the fuzzy matching behavior for the "NAME" rule.
+Next we change the fuzzy matching behavior for the pattern in the "NAME" rule.
 
 
 ```python
 import spacy
 from spaczz.matcher import FuzzyMatcher
 
 nlp = spacy.blank("en")
@@ -140,73 +141,70 @@
 doc = nlp(text)
 
 matcher = FuzzyMatcher(nlp.vocab)
 matcher.add("NAME", [nlp("Grant Andersen")], kwargs=[{"fuzzy_func": "token_sort"}])
 matches = matcher(doc)
 
 # The default fuzzy matching settings will not find a match.
-for match_id, start, end, ratio in matches:
-    print(match_id, doc[start:end], ratio)
+for match_id, start, end, ratio, pattern in matches:
+    print(match_id, doc[start:end], ratio, pattern)
 ```
 
-    NAME Anderson, Grint 86
+    NAME Anderson, Grint 83 Grant Andersen
 
 
-The full list of keyword arguments available for fuzzy matching rules includes:
+The full list of keyword arguments available for fuzzy matching settings includes:
 
-- `fuzzy_func`: Key name of fuzzy matching function to use. All rapidfuzz matching functions with default settings are available. Default is `"simple"`:
-    - "simple" = `ratio`
-    - "partial" = `partial_ratio`
-    - "token_set" = `token_set_ratio`
-    - "token_sort" = `token_sort_ratio`
-    - "partial_token_set" = `partial_token_set_ratio`
-    - "partial_token_sort" = `partial_token_sort_ratio`
-    - "quick" = `QRatio`
-    - "weighted" = `WRatio`
-    - "token" = `token_ratio`,
-    - "partial_token" = `partial_token_ratio`
-    - Default is `"simple"`.
-- `ignore_case`: If strings should be lower-cased before comparison or not. Default is `True`.
-- `flex`: Number of tokens to move match match boundaries left and right during optimization. Can be an integer value with a max of `len(query)` and a min of `0` (will warn and change if higher or lower),or the strings "max", "min", or "default". Default is `"default"`: `len(query) // 2`.
-- `min_r1`: Minimum match ratio required forselection during the intial search over doc. If `flex == 0`, `min_r1` will be overwritten by `min_r2`. If `flex > 0`, `min_r1` must be lower than `min_r2` and "low" in general because match boundaries are not flexed initially. Default is `50`.
-- `min_r2`: Minimum match ratio required for selection during match optimization. Needs to be higher than `min_r1` and "high" in general to ensure only quality matches are returned. Default is `75`.
-- `thresh`: If this ratio is exceeded in initial scan, and `flex > 0`, no optimization will be attempted. If `flex == 0`, `thresh` has no effect. Default is `100`.
+- `ignore_case` (bool): Whether to lower-case text before matching. Default is `True`.
+- `min_r` (int): Minimum match ratio required.
+- `thresh` (int): If this ratio is exceeded in initial scan, and `flex > 0`, no optimization will be attempted. If `flex == 0`, `thresh` has no effect. Default is `100`.
+- `fuzzy_func` (str): Key name of fuzzy matching function to use. All rapidfuzz matching functions with default settings are available. Additional fuzzy matching functions can be registered by users. Default is `"simple"`:
+    * `"simple"` = `ratio`
+    * `"partial"` = `partial_ratio`
+    * `"token"` = `token_ratio`
+    * `"token_set"` = `token_set_ratio`
+    * `"token_sort"` = `token_sort_ratio`
+    * `"partial_token"` = `partial_token_ratio`
+    * `"partial_token_set"` = `partial_token_set_ratio`
+    * `"partial_token_sort"` = `partial_token_sort_ratio`
+    * `"weighted"` = `WRatio`
+    * `"quick"` = `QRatio`
+    * `"partial_alignment"` = `partial_ratio_alignment` (Requires `rapidfuzz>=2.0.3`)
+- `flex` (int|Literal['default', 'min', 'max']): Number of tokens to move match boundaries left and right during optimization. Can be an `int` with a max of `len(pattern)` and a min of `0`, (will warn and change if higher or lower). `"max"`, `"min"`, or `"default"` are also valid. Default is `"default"`: `len(pattern) // 2`.
+- `min_r1` (int|None): Optional granular control over the minimum match ratio required for selection during the initial scan. If `flex == 0`, `min_r1` will be overwritten by `min_r2`. If `flex > 0`, `min_r1` must be lower than `min_r2` and "low" in general because match boundaries are not flexed initially. Default is `None`, which will result in `min_r1` being set to `round(min_r / 1.5)`.
 
 ### RegexMatcher
 
-The basic usage of the regex matcher is also fairly similar to spaCy's `PhraseMatcher`. It accepts regex patterns as strings so flags must be inline. Regexes are compiled with the [regex](https://pypi.org/project/regex/) package so approximate "fuzzy" matching is supported. To provide access to these "fuzzy" match results the matcher returns the fuzzy count values along with match id, start and end information, so make sure to include a variable for the counts when unpacking results.
+The basic usage of the regex matcher is also fairly similar to spaCy's `PhraseMatcher`. It accepts regex patterns as strings so flags must be inline. Regexes are compiled with the [regex](https://pypi.org/project/regex/) package so approximate "fuzzy" matching is supported. To provide access to these "fuzzy" match results the matcher returns a calculated fuzzy ratio and matched pattern, along with match id, start and end information, so make sure to include variables for the ratio and pattern when unpacking results.
 
 
 ```python
 import spacy
 from spaczz.matcher import RegexMatcher
 
 nlp = spacy.blank("en")
 text = """Anderson, Grint created spaczz in his home at 555 Fake St,
 Apt 5 in Nashv1le, TN 55555-1234 in the US."""  # Spelling errors intentional.
 doc = nlp(text)
 
 matcher = RegexMatcher(nlp.vocab)
 # Use inline flags for regex strings as needed
 matcher.add(
-    "APT",
-    [
-        r"""(?ix)((?:apartment|apt|building|bldg|floor|fl|suite|ste|unit
-|room|rm|department|dept|row|rw)\.?\s?)#?\d{1,4}[a-z]?"""
-    ],
-)  # Not the most robust regex.
-matcher.add("GPE", [r"(USA){d<=1}"])  # Fuzzy regex.
+    "ZIP",
+    [r"\b\d{5}(?:[-\s]\d{4})?\b"],
+)
+matcher.add("GPE", [r"(usa){d<=1}"])  # Fuzzy regex.
 matches = matcher(doc)
 
-for match_id, start, end, counts in matches:
-    print(match_id, doc[start:end], counts)
+for match_id, start, end, ratio, pattern in matches:
+    print(match_id, doc[start:end], ratio, pattern)
 ```
 
-    APT Apt 5 (0, 0, 0)
-    GPE US (0, 0, 1)
+    ZIP 55555-1234 100 \b\d{5}(?:[-\s]\d{4})?\b
+    GPE US 80 (usa){d<=1}
 
 
 Spaczz matchers can also make use of on-match rules via callback functions. These on-match callbacks need to accept the matcher itself, the doc the matcher was called on, the match index and the matches produced by the matcher. See the fuzzy matcher usage example above for details.
 
 Like the fuzzy matcher, the regex matcher has optional keyword arguments that can modify matching behavior. Take the below regex matching example.
 
 
@@ -224,49 +222,52 @@
 matcher.add(
     "STREET", ["street_addresses"], kwargs=[{"predef": True}]
 )  # Use predefined regex by key name.
 # Below will not expand partial matches to span boundaries.
 matcher.add("GPE", [r"(?i)[U](nited|\.?) ?[S](tates|\.?)"], kwargs=[{"partial": False}])
 matches = matcher(doc)
 
-for match_id, start, end, counts in matches:
+for match_id, start, end, ratio, pattern in matches:
     print(
-        match_id, doc[start:end], counts
+        match_id, doc[start:end], ratio, pattern
     )  # comma in result isn't ideal - see "Roadmap"
 ```
 
-    STREET 555 Fake St, (0, 0, 0)
+    STREET 555 Fake St, 100 street_addresses
 
 
-The full list of keyword arguments available for regex matching rules includes:
+The full list of keyword arguments available for regex matching settings includes:
 
-- `partial`: Whether partial matches should be extended to existing span boundaries in doc or not, i.e. the regex only matches part of a token or span. Default is True.
-- `predef`: Whether the regex string should be interpreted as a key to a predefined regex pattern or not. Default is False. The included regexes are:
-    - `"dates"`
-    - `"times"`
-    - `"phones"`
-    - `"phones_with_exts"`
-    - `"links"`
-    - `"emails"`
-    - `"ips"`
-    - `"ipv6s"`
-    - `"prices"`
-    - `"hex_colors"`
-    - `"credit_cards"`
-    - `"btc_addresses"`
-    - `"street_addresses"`
-    - `"zip_codes"`
-    - `"po_boxes"`
-    - `"ssn_number"`
-
-The above patterns are the same that the [commonregex](https://github.com/madisonmay/CommonRegex) package provides.
+- `ignore_case` (bool): Whether to lower-case text before matching. Default is `True`.
+- `min_r` (int): Minimum match ratio required.
+- `fuzzy_weights` (str): Name of weighting method for regex insertion, deletion, and substituion counts. Additional weighting methods can be registered by users. Default is `"indel"`.
+    * `"indel"` = `(1, 1, 2)`
+    * `"lev"` = `(1, 1, 1)`
+- `partial`: (bool): Whether partial matches should be extended to `Token` or `Span` boundaries in `doc` or not. For example, the regex only matches part of a `Token` or `Span` in `doc`. Default is `True`.
+- `predef` (string): Whether the regex string should be interpreted as a key to a predefined regex pattern or not. Additional predefined regex patterns can be registered by users. Default is `False.`
+    * `"dates"`
+    * `"times"`
+    * `"phones"`
+    * `"phones_with_exts"`
+    * `"links"`
+    * `"emails"`
+    * `"ips"`
+    * `"ipv6s"`
+    * `"prices"`
+    * `"hex_colors"`
+    * `"credit_cards"`
+    * `"btc_addresses"`
+    * `"street_addresses"`
+    * `"zip_codes"`
+    * `"po_boxes"`
+    * `"ssn_numbers"`
 
 ### SimilarityMatcher
 
-The basic usage of the similarity matcher is similar to spaCy's `PhraseMatcher` except it returns the vector similarity ratio along with match id, start and end information, so make sure to include a variable for the ratio when unpacking results.
+The basic usage of the similarity matcher is similar to spaCy's `PhraseMatcher` except it returns the vector similarity ratio and matched pattern, along with match id, start and end information, so make sure to include variables for the ratio and pattern when unpacking results.
 
 In order to produce meaningful results from the similarity matcher, a spaCy model with word vectors (ex. medium or large English models) must be used to initialize the matcher, process the target document, and process any patterns added.
 
 
 ```python
 import spacy
 from spaczz.matcher import SimilarityMatcher
@@ -276,48 +277,71 @@
 doc = nlp(text)
 
 # lowering min_r2 from default of 75 to produce matches in this example
 matcher = SimilarityMatcher(nlp.vocab, min_r2=65)
 matcher.add("FRUIT", [nlp("fruit")])
 matches = matcher(doc)
 
-for match_id, start, end, ratio in matches:
-    print(match_id, doc[start:end], ratio)
+for match_id, start, end, ratio, pattern in matches:
+    print(match_id, doc[start:end], ratio, pattern)
 ```
 
-    FRUIT apples 72
-    FRUIT grapes 72
-    FRUIT bananas 68
+    FRUIT apples 70 fruit
+    FRUIT grapes 73 fruit
+    FRUIT bananas 70 fruit
 
 
 Please note that even for the mostly pure-Python spaczz, this process is currently extremely slow so be mindful of the scope in which it is applied. Enabling GPU support in spaCy ([see here](https://spacy.io/usage#gpu)) should improve the speed somewhat, but I believe the process will still be bottlenecked in the pure-Python search algorithm until I develop a better search algorithm and/or drop the search to lower-level code (ex C).
 
-Also as a somewhat experimental feature, the similarity matcher is not currently part of the `SpaczzRuler` nor does it have a separate ruler. If you need to add similarity matches to a doc's entities you will need to use an on-match callback for the time being. Please see the fuzzy matcher on-match callback example above for ideas. If there is enough interest in integrating/creating a ruler for the similarity matcher this can be done.
+Also as a somewhat experimental feature, the similarity matcher is not currently part of the `SpaczzRuler` nor does it have a separate ruler. If you need to add similarity matches to a `Doc`'s entities you will need to use an on-match callback for the time being. Please see the fuzzy matcher on-match callback example above for ideas. If there is enough interest in integrating/creating a ruler for the similarity matcher this can be done.
 
-The full list of keyword arguments available for similarity matching rules includes:
+The full list of keyword arguments available for similarity matching settings includes:
 
-- `flex`: Number of tokens to move match span boundaries left and right during match optimization. Can be an integer value with a max of `len(query)` and a min of `0` (will warn and change if higher or lower), `"max"`, `"min"`, or `"default"`. Default is `"default"`: `len(query) // 2`.
-- `min_r1`: Minimum similarity match ratio required for selection during the intial search over doc. This should be lower than `min_r2` and "low" in general because match span boundaries are not flexed initially. `0` means all spans of query length in doc will have their boundaries flexed and will be re-compared during match optimization. Lower `min_r1` will result in more fine-grained matching but will run slower. Default is `50`.
-- `min_r2`: Minimum similarity match ratio required for selection during match optimization. Should be higher than `min_r1` and "high" in general to ensure only quality matches are returned. Default is `75`.
-- `thresh`: If this ratio is exceeded in initial scan no optimization will be attempted. Default is `100`.
+- `ignore_case` (bool): Whether to lower-case text before fuzzy matching. Default is `True`.
+- `min_r` (int): Minimum match ratio required.
+- `thresh` (int): If this ratio is exceeded in initial scan, and `flex > 0`, no optimization will be attempted. If `flex == 0`, `thresh` has no effect. Default is `100`.
+- `flex` (int|Literal['default', 'min', 'max']): Number of tokens to move match boundaries left and right during optimization. Can be an `int` with a max of `len(pattern)` and a min of `0`, (will warn and change if higher or lower). `"max"`, `"min"`, or `"default"` are also valid. Default is `"default"`: `len(pattern) // 2`.
+- `min_r1` (int|None): Optional granular control over the minimum match ratio required for selection during the initial scan. If `flex == 0`, `min_r1` will be overwritten by `min_r2`. If `flex > 0`, `min_r1` must be lower than `min_r2` and "low" in general because match boundaries are not flexed initially. Default is `None`, which will result in `min_r1` being set to `round(min_r / 1.5)`.
+- `min_r2` (int|None): Optional granular control over the minimum match ratio required for selection during match optimization. Needs to be higher than `min_r1` and "high" in general to ensure only quality matches are returned. Default is `None`, which will result in `min_r2` being set to `min_r`.
 
 ### TokenMatcher
 
+*Note: spaCy's `Matcher` now supports [fuzzy matching](https://spacy.io/usage/v3-5#fuzzy), so unless you need a specific feature from spaczz's `TokenMatcher`, it is highly recommended to use spaCy's much faster `Matcher`.*
+
 The basic usage of the token matcher is similar to spaCy's `Matcher`. It accepts labeled patterns in the form of lists of dictionaries where each list describes an individual pattern and each dictionary describes an individual token.
 
 The token matcher accepts all the same token attributes and pattern syntax as it's spaCy counterpart but adds fuzzy and fuzzy-regex support.
 
 `"FUZZY"` and `"FREGEX"` are the two additional spaCy token pattern options.
 
 For example:
-    `{"TEXT": {"FREGEX": "(database){e<=1}"}},`
-    `{"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "quick_lev"}}`
+
+```python
+[
+    {"TEXT": {"FREGEX": "(database){e<=1}"}},
+    {"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "quick_lev"}},
+]
+```
 
 **Make sure to use uppercase dictionary keys in patterns.**
 
+The full list of keyword arguments available for token matching settings includes:
+
+- `ignore_case` (bool): Whether to lower-case text before matching. Can only be set at the pattern level. For "FUZZY" and "FREGEX" patterns. Default is `True`.
+- `min_r` (int): Minimum match ratio required. For "FUZZY" and "FREGEX" patterns.
+- `fuzzy_func` (str): Key name of fuzzy matching function to use. Can only be set at the pattern level. For "FUZZY" patterns only. All rapidfuzz matching functions with default settings are available, however any token-based functions provide no utility at the individual token level. Additional fuzzy matching functions can be registered by users. Included, and useful, functions are (the default is `simple`):
+    * `"simple"` = `ratio`
+    * `"partial"` = `partial_ratio`
+    * `"quick"` = `QRatio`
+    * `"partial_alignment"` = `partial_ratio_alignment` (Requires `rapidfuzz>=2.0.3`)
+- `fuzzy_weights` (str): Name of weighting method for regex insertion, deletion, and substituion counts. Additional weighting methods can be registered by users. Default is `"indel"`.
+    * `"indel"` = `(1, 1, 2)`
+    * `"lev"` = `(1, 1, 1)`
+- `predef`: Whether regex should be interpreted as a key to a predefined regex pattern or not. Can only be set at the pattern level. For "FREGEX" patterns only. Default is `False`.
+
 
 ```python
 import spacy
 from spaczz.matcher import TokenMatcher
 
 # Using model results like POS tagging in token patterns requires model that provides these.
 nlp = spacy.load("en_core_web_md")
@@ -336,36 +360,36 @@
         ],
         [{"TEXT": {"FUZZY": "Sequel"}, "POS": "PROPN"}, {"LOWER": "db"}],
     ],
 )
 matcher.add("NAME", [[{"TEXT": {"FUZZY": "Garfield"}}]])
 matches = matcher(doc)
 
-for match_id, start, end, _ in matches:  # Note the _ here. Explained below.
-    print(match_id, doc[start:end])
+for match_id, start, end, ratio, pattern in matches:
+    print(match_id, doc[start:end], ratio, pattern)
 ```
 
-    DATA SQL databesE acess
-    DATA Sequal DB
-    NAME Grfield
+    DATA SQL databesE acess 91 [{"TEXT":"SQL"},{"LOWER":{"FREGEX":"(database){s<=1}"}},{"LOWER":{"FUZZY":"access"}}]
+    DATA Sequal DB 87 [{"TEXT":{"FUZZY":"Sequel"},"POS":"PROPN"},{"LOWER":"db"}]
+    NAME Grfield 93 [{"TEXT":{"FUZZY":"Garfield"}}]
 
 
-Please note that the way the token matcher is implemented does not currently have a way to return fuzzy ratio or fuzzy-regex counts like the fuzzy matcher and regex matcher provide. To keep the API consistent, the token matcher returns a placeholder of `None` as the fourth element of the tuples it returns, so be sure to account for this like we did with `_` in unpacking above.
+Even though the token matcher can be a drop-in replacement for spaCy's `Matcher`, it is still recommended to use spaCy's `Matcher` if you do not need the spaczz token matcher's fuzzy capabilities - it will slow processing down unnecessarily.
 
-Also, even though the token matcher can be a drop-in replacement for spaCy's `Matcher`, it is still recommended to use spaCy's `Matcher` if you do not need the spaczz token matcher's fuzzy capabilities - it will slow processing down unnecessarily.
+*Reminder: spaCy's `Matcher` now supports [fuzzy matching](https://spacy.io/usage/v3-5#fuzzy), so unless you need a specific feature from spaczz's `TokenMatcher`, it is highly recommended to use spaCy's much faster `Matcher`.*
 
 ### SpaczzRuler
 
-The spaczz ruler combines the fuzzy and regex phrase matchers, and the "fuzzy" token matcher, into one pipeline component that can update a doc entities similar to spaCy's `EntityRuler`.
+The spaczz ruler combines the fuzzy and regex phrase matchers, and the "fuzzy" token matcher, into one pipeline component that can update a `Doc.ents` similar to spaCy's `EntityRuler`.
 
 Patterns must be added as an iterable of dictionaries in the format of *{label (str), pattern(str or list), type(str), optional kwargs (dict), and optional id (str)}*.
 
 For example, a fuzzy phrase pattern:
 
-`{'label': 'ORG', 'pattern': 'Apple', 'type': 'fuzzy', 'kwargs': {'min_r2': 90}}`
+`{'label': 'ORG', 'pattern': 'Apple' 'kwargs': {'min_r2': 90}, 'type': 'fuzzy'}`
 
 Or, a token pattern:
 
 `{'label': 'ORG', 'pattern': [{'TEXT': {'FUZZY': 'Apple'}}], 'type': 'token'}`
 
 
 ```python
@@ -414,104 +438,95 @@
     },
 ]
 
 ruler = SpaczzRuler(nlp)
 ruler.add_patterns(patterns)
 doc = ruler(doc)
 
-print("Fuzzy Matches:")
-for ent in doc.ents:
-    if ent._.spaczz_type == "fuzzy":
-        print((ent.text, ent.start, ent.end, ent.label_, ent._.spaczz_ratio))
 
-print("\n", "Regex Matches:", sep="")
 for ent in doc.ents:
-    if ent._.spaczz_type == "regex":
-        print((ent.text, ent.start, ent.end, ent.label_, ent._.spaczz_counts))
-
-print("\n", "Token Matches:", sep="")
-for ent in doc.ents:
-    if ent._.spaczz_type == "token":
-        # ._.spaczz_details is currently just placeholder value of 1
-        print((ent.text, ent.start, ent.end, ent.label_, ent._.spaczz_details))
-```
-
-    Fuzzy Matches:
-    ('Anderson, Grint', 0, 3, 'NAME', 86)
-    ('Nashv1le', 17, 18, 'GPE', 82)
-
-    Regex Matches:
-    ('555 Fake St,', 9, 13, 'STREET', (0, 0, 0))
-    ('55555-1234', 20, 23, 'ZIP', (1, 0, 0))
-    ('USA', 25, 26, 'GPE', (0, 0, 0))
-
-    Token Matches:
-    ('Converg', 34, 35, 'BAND', 1)
-    ('Protet the Zero', 36, 39, 'BAND', 1)
+    print(
+        (
+            ent.text,
+            ent.start,
+            ent.end,
+            ent.label_,
+            ent._.spaczz_ratio,
+            ent._.spaczz_type,
+            ent._.spaczz_pattern,
+        )
+    )
+```
+
+    ('Anderson, Grint', 0, 3, 'NAME', 83, 'fuzzy', 'Grant Andersen')
+    ('555 Fake St,', 9, 13, 'STREET', 100, 'regex', 'street_addresses')
+    ('Nashv1le', 17, 18, 'GPE', 82, 'fuzzy', 'Nashville')
+    ('55555-1234', 20, 23, 'ZIP', 90, 'regex', '\\b(?:55554){s<=1}(?:(?:[-\\s])?\\d{4}\\b)')
+    ('USA', 25, 26, 'GPE', 100, 'regex', '(?i)[U](nited|\\.?) ?[S](tates|\\.?)')
+    ('Converg', 34, 35, 'BAND', 93, 'token', '[{"LOWER":{"FREGEX":"(converge){e<=1}"}}]')
+    ('Protet the Zero', 36, 39, 'BAND', 89, 'token', '[{"TEXT":{"FUZZY":"Protest"}},{"IS_STOP":true},{"TEXT":{"FUZZY":"Hero"}}]')
 
 
 We see in the example above that we are referencing some custom attributes, which are explained below.
 
-For more `SpaczzRuler` examples see [here](https://github.com/gandersen101/spaczz/blob/master/examples/fuzzy_matching_tweaks.md). In particular this provides details about the ruler's sorting process and fuzzy matching parameters.
+For more `SpaczzRuler` examples see [here](https://github.com/gandersen101/spaczz/blob/master/examples/fuzzy_matching_tweaks.ipynb). In particular this provides details about the ruler's sorting process and fuzzy matching parameters.
 
 ### Custom Attributes
 
 Spaczz initializes some custom attributes upon importing. These are under spaCy's `._.` attribute and are further prepended with `spaczz_` so there should be not conflicts with your own custom attributes. If there are spaczz will force overwrite them.
 
 These custom attributes are only set via the spaczz ruler at the token level. Span and doc versions of these attributes are getters that reference the token level attributes.
 
 The following `Token` attributes are available. All are mutable:
 
-- `spaczz_token`: default = `False`. Boolean that denotes if the token is part of an ent set by the spaczz ruler.
-- `spaczz_type`: default = `None`. String that shows which matcher produced an ent using the token.
-- `spaczz_ratio`: default = `None`. If the token is part of fuzzy-phrase-matched ent, will return fuzzy ratio.
-- `spaczz_counts`: default = `None`. If the token is part of regex-phrase-matched ent, will return fuzzy counts.
-- `spaczz_details`: default = `None`. Placeholder for token matcher fuzzy ratio/counts. To be developed. Will return 1 if the token is part of a "fuzzy"-token-matched ent.
+- `spaczz_token`: default = `False`. Boolean that denotes if the token is part of an entity set by the spaczz ruler.
+- `spaczz_type`: default = `None`. String that shows which matcher produced an entity using the token.
+- `spaczz_ratio`: default = `None`. If the token is part of a matched entity, it will return fuzzy ratio.
+- `spaczz_pattern`: default = `None`. If the token is part of a matched entity, it will return the pattern as a string (JSON-formatted for token patterns) that produced the match.
 
 The following `Span` attributes reference the token attributes included in the span. All are immutable:
 
-- `spaczz_ent`: default = `False`. Boolean that denotes if all tokens in span are part of an ent set by the spaczz ruler.
-- `spaczz_type`: default = `None`. String that denotes which matcher produced an ent using the included tokens.
-- `spaczz_types`: default = `set()`. Set that shows which matchers produced ents using the included tokens. An entity span should only have one type, but this allows you to see the types included in any arbitrary span.
-- `spaczz_ratio`: default = `None`. If all the tokens in span are part of fuzzy-phrase-matched ent, will return fuzzy ratio.
-- `spaczz_counts`: default = `None`. If all the tokens in span are part of regex-phrase-matched ent, will return fuzzy counts.
-- `spaczz_details`: default = `None`. Placeholder for token matcher fuzzy ratio/counts. To be developed. Will return 1 if all the tokens in span are part of a "fuzzy"-token-matched ent.
+- `spaczz_ent`: default = `False`. Boolean that denotes if all tokens in the span are part of an entity set by the spaczz ruler.
+- `spaczz_type`: default = `None`. String that denotes which matcher produced an entity using the included tokens.
+- `spaczz_types`: default = `set()`. Set that shows which matchers produced entities using the included tokens. An entity span should only have one type, but this allows you to see the types included in any arbitrary span.
+- `spaczz_ratio`: default = `None`. If all the tokens in span are part of a matched entity, it will return the fuzzy ratio.
+- `spaczz_pattern`: default = `None`. If all the tokens in a span are part of a matched entity, it will return the pattern as a string (JSON-formatted for token patterns) that produced the match.
 
 The following `Doc` attributes reference the token attributes included in the doc. All are immutable:
 
-- `spaczz_doc`: default = `False`. Boolean that denotes if any tokens in the doc are part of an ent set by the spaczz ruler.
-- `spaczz_types`: default = `set()`. Set that shows which matchers produced ents in the doc.
+- `spaczz_doc`: default = `False`. Boolean that denotes if any tokens in the doc are part of an entity set by the spaczz ruler.
+- `spaczz_types`: default = `set()`. Set that shows which matchers produced entities in the doc.
 
 ### Saving/Loading
 
 The `SpaczzRuler` has it's own to/from disk/bytes methods and will accept `config` parameters passed to `spacy.load()`. It also has it's own spaCy factory entry point so spaCy is aware of the `SpaczzRuler`. Below is an example of saving and loading a spacy pipeline with the small English model, the `EntityRuler`, and the `SpaczzRuler`.
 
 
 ```python
 import spacy
 from spaczz.pipeline import SpaczzRuler
 
-nlp = spacy.load("en_core_web_sm")
+nlp = spacy.load("en_core_web_md")
 text = """Anderson, Grint created spaczz in his home at 555 Fake St,
 Apt 5 in Nashv1le, TN 55555-1234 in the USA.
 Some of his favorite bands are Converg and Protet the Zero."""  # Spelling errors intentional.
 doc = nlp(text)
 
 for ent in doc.ents:
     print((ent.text, ent.start, ent.end, ent.label_))
 ```
 
-    ('Anderson', 0, 1, 'PERSON')
-    ('Grint', 2, 3, 'PERSON')
+    ('Anderson, Grint', 0, 3, 'ORG')
     ('555', 9, 10, 'CARDINAL')
-    ('5', 15, 16, 'CARDINAL')
-    ('TN 55555-1234', 19, 23, 'DATE')
+    ('Apt 5', 14, 16, 'PRODUCT')
+    ('Nashv1le', 17, 18, 'GPE')
+    ('TN 55555-1234', 19, 23, 'ORG')
     ('USA', 25, 26, 'GPE')
     ('Converg', 34, 35, 'PERSON')
-    ('Protet', 36, 37, 'PERSON')
+    ('Zero', 38, 39, 'CARDINAL')
 
 
 While spaCy does a decent job of identifying that named entities are present in this example, we can definitely improve the matches - particularly with the types of labels applied.
 
 Let's add an entity ruler for some rules-based matches.
 
 
@@ -525,22 +540,22 @@
 
 doc = nlp(text)
 
 for ent in doc.ents:
     print((ent.text, ent.start, ent.end, ent.label_))
 ```
 
-    ('Anderson', 0, 1, 'PERSON')
-    ('Grint', 2, 3, 'PERSON')
+    ('Anderson, Grint', 0, 3, 'ORG')
     ('555', 9, 10, 'CARDINAL')
-    ('5', 15, 16, 'CARDINAL')
+    ('Apt 5', 14, 16, 'PRODUCT')
+    ('Nashv1le', 17, 18, 'GPE')
     ('TN', 19, 20, 'GPE')
     ('USA', 25, 26, 'GPE')
     ('Converg', 34, 35, 'PERSON')
-    ('Protet', 36, 37, 'PERSON')
+    ('Zero', 38, 39, 'CARDINAL')
 
 
 We're making progress, but Nashville is spelled wrong in the text so the entity ruler does not find it, and we still have other entities to fix/find.
 
 Let's add a spaczz ruler to round this pipeline out. We will also include the `spaczz_span` custom attribute in the results to denote which entities were set via spaczz.
 
 
@@ -587,45 +602,49 @@
 
 for ent in doc.ents:
     print((ent.text, ent.start, ent.end, ent.label_, ent._.spaczz_ent))
 ```
 
     ('Anderson, Grint', 0, 3, 'NAME', True)
     ('555 Fake St,', 9, 13, 'STREET', True)
-    ('5', 15, 16, 'CARDINAL', False)
+    ('Apt 5', 14, 16, 'PRODUCT', False)
     ('Nashv1le', 17, 18, 'GPE', True)
     ('TN', 19, 20, 'GPE', False)
     ('55555-1234', 20, 23, 'ZIP', True)
     ('USA', 25, 26, 'GPE', False)
     ('Converg', 34, 35, 'BAND', True)
     ('Protet the Zero', 36, 39, 'BAND', True)
 
 
 Awesome! The small English model still makes a named entity recognition mistake ("5" in "Apt 5" as `CARDINAL`), but we're satisfied overall.
 
 Let's save this pipeline to disk and make sure we can load it back correctly.
 
 
 ```python
-nlp.to_disk("./example")
-nlp = spacy.load("./example")
+import tempfile
+
+with tempfile.TemporaryDirectory() as tmp_dir:
+    nlp.to_disk(f"{tmp_dir}/example_pipeline")
+    nlp = spacy.load(f"{tmp_dir}/example_pipeline")
+
 nlp.pipe_names
 ```
 
 
 
 
     ['tok2vec',
      'tagger',
      'parser',
+     'attribute_ruler',
+     'lemmatizer',
      'entity_ruler',
      'spaczz_ruler',
-     'ner',
-     'attribute_ruler',
-     'lemmatizer']
+     'ner']
 
 
 
 We can even ensure all the spaczz ruler patterns are still present.
 
 
 ```python
@@ -662,92 +681,65 @@
 ## Known Issues
 
 ### Performance
 
 The main reason for spaczz's slower speed is that the *c* in it's name is not capitalized like it is in spa*C*y.
 Spaczz is written in pure Python and it's matchers do not currently utilize spaCy language vocabularies, which means following it's logic should be easy to those familiar with Python. However this means spaczz components will run slower and likely consume more memory than their spaCy counterparts, especially as more patterns are added and documents get longer. It is therefore recommended to use spaCy components like the EntityRuler for entities with little uncertainty, like consistent spelling errors. Use spaczz components when there are not viable spaCy alternatives.
 
-I am actively working on performance optimizations to spaczz but it is a gradual process. Algorithmic and optimization suggestions are welcome. I am working on learning C but currently C-based work is outside of my skill set.
-
-The `FuzzyMatcher`, and even more so, the `SimilarityMatcher` are the slowest spaczz components (although allowing for enough "fuzzy" matches in the `RegexMatcher` can get really slow as well). The primary methods for speeding these components up are by decreasing the `flex` parameter towards `0`, or if `flex > 0`, increasing the `min_r1` parameter towards the value of `min_r2` and/or lowering the `thresh` parameter towards `min_r2`. Be aware that all of these "speed-ups" come at the opportunity cost of potentially improved matches.
-
-As mentioned in the `SimilarityMatcher` description, utilizing a GPU will also help speed up it's matching process.
-
-I will likely try to develop some automated and/or heuristic-based API options (while retaining all the current options) in the future to simplify this "tuning" process.
-
-### SpaczzRuler Inconsistencies
-
-This one is particularly annoying for me because I built myself into this hole trying to support too much too fast. That being said I have addressed much of this as of spaczz 0.4.2 and will continue to improve these issues.
-
-Spaczz, like spaCy, has undefined behavior for multiple labels (or label/ent_id combos) sharing the same pattern. For example, if you add the pattern `"Ireland"` as both `"GPE"` and `"NAME"` the resulting label is unpredictable. For the most part this isn't an issue but spaczz also has to deal with the additional wrinkle of fuzzy matches.
+I am *not* currently working on performance optimizations to spaczz, but algorithmic and optimization suggestions are welcome.
 
-For example if we are looking for the string `"Ireland"` and have the patterns `["Ireland", "Iceland"]`. Even with a required match ratio of `85` these will both match at `100` and `86` respectively. When just dealing with fuzzy matches this isn't an issue as we can sort by descending match ratio. However what if the `"Iceland"` pattern was a regex pattern and it returned a tuple of fuzzy regex counts? Or what if the `"Iceland"` pattern was a token pattern and the `TokenMatcher` does not even currently provide match details?!
+The primary methods for speeding up the `FuzzyMatcher` and `SimilarityMatcher` are by decreasing the `flex` parameter towards `0`, or if `flex > 0`, increasing the `min_r1` parameter towards the value of `min_r2` and/or lowering the `thresh` parameter towards `min_r2`. Be aware that all of these "speed-ups" come at the opportunity cost of potentially improved matches.
 
-The above problem is twofold. First and foremost, I need to develop a way or ways to compare apples to oranges - fuzzy ratios and fuzzy regex counts. Then I need to figure out how to include match details from the `TokenMatcher` which supports both fuzzy and "fuzzy" regex matches.
-
-For a short-term solution I am having the entity ruler first go through sorted fuzzy matches, then sorted regex matches, and lastly token matches. Token matches will only be sorted by length of match, not quality, so they may provide inconsistent results. Try to be mindful of your token patterns.
-
-There is additional logic in place to filter overlapping matches preserving earlier matches over later ones. This order of priority (fuzzy, regex, token) may not be ideal for everyone but adding a way to change the order (say regex patterns first) would a temporary solution to a temporary problem.
-
-Please bear with me through these growing pains.
+As mentioned in the `SimilarityMatcher` description, utilizing a GPU may also help speed up it's matching process.
 
 ## Roadmap
 
 I am always open and receptive to feature requests but just be aware, as a solo-dev with a lot left to learn, development can move pretty slow. The following is my roadmap for spaczz so you can see where issues raised might fit into my current priorities.
 
+*Note: while I want to keep `spaczz` functional, I am **not** actively developing it. I try to be responsive to issues and requests but this project is not currently a focus of mine.*
+
 **High Priority**
 
 1. Bug fixes - both breaking and behavioral. Hopefully these will be minimal.
 1. Ease of use and error/warning handling and messaging enhancements.
 1. Building out Read the Docs.
-1. A method for comparing fuzzy ratios and fuzzy regex counts.
-1. A way to return match details from the `TokenMatcher`.
 1. Option to prioritize match quality over length and/or weighing options.
 1. Profiling - hopefully to find "easy" performance optimizations.
 
 **Enhancements**
 
-1. API support for adding user-defined regexes to the predefined regex.
-    1. Saving these additional predefined regexes as part of the SpaczzRuler will also be supported.
-1. Entity start/end trimming on the token level to prevent fuzzy and regex phrase matches from starting/ending with unwanted tokens, i.e. spaces/punctuation.
-
-**Long-Horizon Performance Enhancements**
-
 1. Having spaczz matchers utilize spaCy vocabularies.
 1. Rewrite the phrase and token searching algorithms in Cython to utilize C speed.
-    1. Try to integrate closely with spaCy.
+    1. Try to integrate closer with spaCy.
 
 ## Development
 
 Pull requests and contributors are welcome.
 
 spaczz is linted with [Flake8](https://flake8.pycqa.org/en/latest/), formatted with [Black](https://black.readthedocs.io/en/stable/), type-checked with [MyPy](http://mypy-lang.org/) (although this could benefit from improved specificity), tested with [Pytest](https://docs.pytest.org/en/stable/), automated with [Nox](https://nox.thea.codes/en/stable/), and built/packaged with [Poetry](https://python-poetry.org/). There are a few other development tools detailed in the noxfile.py, along with Git pre-commit hooks.
 
 To contribute to spaczz's development, fork the repository then install spaczz and it's dev dependencies with Poetry. If you're interested in being a regular contributor please contact me directly.
 
-
 ```python
 poetry install # Within spaczz's root directory.
 ```
 
 I keep Nox and pre-commit outside of my poetry environment as part of my Python toolchain environments. With pre-commit installed you may also need to run the below to commit changes.
 
-
 ```python
 pre-commit install
 ```
 
 The only other package that will not be installed via Poetry but is used for testing and in-documentation examples is the spaCy medium English model (`en-core-web-md`). This will need to be installed separately. The command below should do the trick:
 
-
 ```python
 poetry run python -m spacy download "en_core_web_md"
 ```
 
 ## References
 
-- Spaczz tries to stay as close to [spaCy](https://spacy.io/)'s API as possible. Whenever it made sense to use existing spaCy code within spaczz this was done.
+- spaczz tries to stay as close to [spaCy](https://spacy.io/)'s API as possible. Whenever it made sense to use existing spaCy code within spaczz this was done.
 - Fuzzy matching is performed using [RapidFuzz](https://github.com/maxbachmann/rapidfuzz).
 - Regexes are performed using the [regex](https://pypi.org/project/regex/) library.
 - The search algorithm for phrased-based fuzzy and similarity matching was heavily influnced by Stack Overflow user Ulf Aslak's answer in this [thread](https://stackoverflow.com/questions/36013295/find-best-substring-match).
-- Spaczz's predefined regex patterns were borrowed from the [commonregex](https://github.com/madisonmay/CommonRegex) package.
-- Spaczz's development and CI/CD patterns were inspired by Claudio Jolowicz's [*Hypermodern Python*](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/) article series.
+- spaczz's predefined regex patterns were borrowed from the [commonregex](https://github.com/madisonmay/CommonRegex) package.
+- spaczz's development and CI/CD patterns were inspired by Claudio Jolowicz's [*Hypermodern Python*](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/) article series.
```

### Comparing `spaczz-0.5.4/src/spaczz/customattrs.py` & `spaczz-0.6.0a0/src/spaczz/customattrs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,116 @@
 """Custom spaCy attributes for spaczz."""
-from __future__ import annotations
-
-from typing import Iterable, Optional, Set, Tuple, Type
+import typing as ty
 import warnings
 
-from spacy.tokens import Doc, Span, Token
+from spacy.tokens import Doc
+from spacy.tokens import Span
+from spacy.tokens import Token
 
-from .exceptions import AttrOverwriteWarning, SpaczzSpanDeprecation
+from .customtypes import SpaczzType
+from .exceptions import AttrOverwriteWarning
 
 
 class SpaczzAttrs:
-    """Adds spaczz custom attributes to spacy."""
+    """Adds spaczz custom attributes to spaCy."""
 
     _initialized = False
 
     @classmethod
-    def initialize(cls: Type[SpaczzAttrs]) -> None:
+    def initialize(cls: ty.Type["SpaczzAttrs"]) -> None:
         """Initializes and registers custom attributes."""
         if not cls._initialized:
             try:
                 Token.set_extension("spaczz_token", default=False)
                 Token.set_extension("spaczz_type", default=None)
                 Token.set_extension("spaczz_ratio", default=None)
-                Token.set_extension("spaczz_counts", default=None)
-                Token.set_extension("spaczz_details", default=None)
+                Token.set_extension("spaczz_pattern", default=None)
 
-                Span.set_extension("spaczz_span", getter=cls.get_spaczz_span)
                 Span.set_extension("spaczz_ent", getter=cls.get_spaczz_ent)
                 Span.set_extension("spaczz_type", getter=cls.get_span_type)
                 Span.set_extension("spaczz_types", getter=cls.get_span_types)
                 Span.set_extension("spaczz_ratio", getter=cls.get_ratio)
-                Span.set_extension("spaczz_counts", getter=cls.get_counts)
-                Span.set_extension("spaczz_details", getter=cls.get_details)
+                Span.set_extension("spaczz_pattern", getter=cls.get_pattern)
 
                 Doc.set_extension("spaczz_doc", getter=cls.get_spaczz_doc)
                 Doc.set_extension("spaczz_types", getter=cls.get_doc_types)
                 cls._initialized = True
             except ValueError:
                 warnings.warn(
                     """One or more spaczz custom extensions has already been registered.
                     These are being force overwritten. Please avoid defining personal,
-                    custom extensions prepended with "spaczz_".
+                    custom extensions prepended with `"spaczz_"`.
                 """,
                     AttrOverwriteWarning,
+                    stacklevel=2,
                 )
                 Token.set_extension("spaczz_token", default=False, force=True)
                 Token.set_extension("spaczz_type", default=None, force=True)
                 Token.set_extension("spaczz_ratio", default=None, force=True)
-                Token.set_extension("spaczz_counts", default=None, force=True)
 
-                Span.set_extension(
-                    "spaczz_span", getter=cls.get_spaczz_span, force=True
-                )
                 Span.set_extension("spaczz_type", getter=cls.get_span_type, force=True)
                 Span.set_extension(
                     "spaczz_types", getter=cls.get_span_types, force=True
                 )
                 Span.set_extension("spaczz_ratio", getter=cls.get_ratio, force=True)
-                Span.set_extension("spaczz_counts", getter=cls.get_counts, force=True)
+                Span.set_extension("spaczz_pattern", getter=cls.get_pattern, force=True)
 
                 Doc.set_extension("spaczz_doc", getter=cls.get_spaczz_doc, force=True)
                 Doc.set_extension("spaczz_types", getter=cls.get_doc_types, force=True)
 
     @staticmethod
-    def get_spaczz_span(span: Span) -> bool:
-        """Getter for spaczz_span `Span` attribute."""
-        warnings.warn(
-            """spaczz_span is deprecated.
-        Use spaczz_ent instead.""",
-            SpaczzSpanDeprecation,
-        )
-        return all([token._.spaczz_token for token in span])
-
-    @staticmethod
     def get_spaczz_ent(span: Span) -> bool:
         """Getter for spaczz_ent `Span` attribute."""
         return all([token._.spaczz_token for token in span])
 
     @classmethod
-    def get_span_type(cls: Type[SpaczzAttrs], span: Span) -> Optional[str]:
+    def get_span_type(
+        cls: ty.Type["SpaczzAttrs"], span: Span
+    ) -> ty.Optional[SpaczzType]:
         """Getter for spaczz_type `Span` attribute."""
         if cls._all_equal([token._.spaczz_type for token in span]):
             return span[0]._.spaczz_type
         else:
             return None
 
     @staticmethod
-    def get_span_types(span: Span) -> Set[str]:
+    def get_span_types(span: Span) -> ty.Set[SpaczzType]:
         """Getter for spaczz_types `Span` attribute."""
         types = [token._.spaczz_type for token in span if token._.spaczz_type]
         return set(types)
 
     @classmethod
-    def get_ratio(cls: Type[SpaczzAttrs], span: Span) -> Optional[int]:
+    def get_ratio(cls: ty.Type["SpaczzAttrs"], span: Span) -> ty.Optional[int]:
         """Getter for spaczz_ratio `Span` attribute."""
         if cls._all_equal([token._.spaczz_ratio for token in span]):
             return span[0]._.spaczz_ratio
         else:
             return None
 
     @classmethod
-    def get_counts(
-        cls: Type[SpaczzAttrs], span: Span
-    ) -> Optional[Tuple[int, int, int]]:
-        """Getter for spaczz_counts `Span` attribute."""
-        if cls._all_equal([token._.spaczz_counts for token in span]):
-            return span[0]._.spaczz_counts
-        else:
-            return None
-
-    @classmethod
-    def get_details(cls: Type[SpaczzAttrs], span: Span) -> Optional[int]:
-        """Getter for current placeholder spaczz_details `Span` attribute."""
-        if cls._all_equal([token._.spaczz_details for token in span]):
-            return span[0]._.spaczz_details
+    def get_pattern(cls: ty.Type["SpaczzAttrs"], span: Span) -> ty.Optional[str]:
+        """Getter for spaczz_pattern `Span` attribute."""
+        if cls._all_equal([token._.spaczz_pattern for token in span]):
+            return span[0]._.spaczz_pattern
         else:
             return None
 
     @staticmethod
     def get_spaczz_doc(doc: Doc) -> bool:
         """Getter for spaczz_doc `Doc` attribute."""
         return any([token._.spaczz_token for token in doc])
 
     @staticmethod
-    def get_doc_types(doc: Doc) -> Set[str]:
+    def get_doc_types(doc: Doc) -> ty.Set[SpaczzType]:
         """Getter for spaczz_types `Doc` attribute."""
         types = [token._.spaczz_type for token in doc if token._.spaczz_type]
         return set(types)
 
     @staticmethod
-    def _all_equal(iterable: Iterable) -> bool:
+    def _all_equal(iterable: ty.Iterable[ty.Any]) -> bool:
         """Tests if all elements of iterable are equal."""
         iterator = iter(iterable)
         try:
             first = next(iterator)
         except StopIteration:
             return True
         return all(first == rest for rest in iterator)
```

### Comparing `spaczz-0.5.4/src/spaczz/exceptions.py` & `spaczz-0.6.0a0/src/spaczz/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,21 +17,13 @@
     """It warns if there are more kwargs than patterns or vice versa."""
 
 
 class PatternTypeWarning(Warning):
     """It warns if the spaczz pattern does not have a valid pattern type."""
 
 
-class PipeDeprecation(Warning):
-    """Warns that `matcher.pipe` methods are now deprecated."""
-
-
 class MissingVectorsWarning(Warning):
     """It warns if the spaCy Vocab does not have word vectors."""
 
 
 class RatioWarning(Warning):
     """It warns if match ratio values are incompatible with each other."""
-
-
-class SpaczzSpanDeprecation(Warning):
-    """It warns if the spaczz_span attribute is accessed."""
```

### Comparing `spaczz-0.5.4/src/spaczz/matcher/_phrasematcher.py` & `spaczz-0.6.0a0/src/spaczz/matcher/tokenmatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,358 +1,368 @@
-"""Module for _PhraseMatcher: base class for other phrase based spaczz matchers."""
-from __future__ import annotations
-
-from typing import (
-    Any,
-    Callable,
-    DefaultDict,
-    Dict,
-    Generator,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-)
-import warnings
+"""Module for TokenMatcher with an API semi-analogous to spaCy's Matcher."""
+from copy import deepcopy
+import typing as ty
 
+from spacy.matcher import Matcher
 from spacy.tokens import Doc
 from spacy.vocab import Vocab
+import srsly
+
+from .._search import TokenSearcher
+from ..customtypes import SpaczzType
+
+
+class TokenMatcher:
+    """spaCy-like matcher for finding fuzzy token matches in `Doc` objects.
 
-from ..exceptions import KwargsWarning, PipeDeprecation
-from ..search import _PhraseSearcher
-from ..util import nest_defaultdict
+    Fuzzy matches added patterns against the `Doc` object it is called on.
+    Accepts labeled patterns in the form of lists of dictionaries
+    where each list describes an individual pattern and each
+    dictionary describes an individual token.
 
+    Uses extended spaCy token matching patterns.
+    "FUZZY" and "FREGEX" are the two additional spaCy token pattern options.
 
-class _PhraseMatcher:
-    """spaCy-like matcher for finding flexible matches in `Doc` objects.
+    For example::
 
-    Matches added patterns against the `Doc` object it is called on.
-    Accepts labeled patterns in the form of `Doc` objects.
+        [
+            {"TEXT": {"FREGEX": "(database){e<=1}"}},
+            {"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "partial"}},
+        ]
+
+    Make sure to use uppercase dictionary keys in patterns.
 
     Attributes:
-        defaults (dict[str, Any]): Keyword arguments to be used as
-            default matching settings.
-            See `_PhraseSearcher` documentation for details.
         name (str): Class attribute - the name of the matcher.
-        type (str): The kind of matcher object.
-        _callbacks (dict[str, PhraseCallback]):
-            On match functions to modify `Doc` objects passed to the matcher.
-            Can make use of the matches identified.
-        _patterns (DefaultDict[str, DefaultDict[str, Any]]):
-            Patterns added to the matcher. Contains patterns
-            and kwargs that should be used during matching
-            for each labels added.
+        defaults (dict[str, bool|int|str]):
+            Keyword arguments to be used as default match settings.
+            Per-pattern match settings take precedence over defaults.
+
+    Match Settings:
+        ignore_case (bool): Whether to lower-case text before matching.
+            Can only be set at the pattern level. For "FUZZY" and "FREGEX" patterns.
+            Default is `True`.
+        min_r (int): Minimum match ratio required. For "FUZZY" and "FREGEX" patterns.
+        fuzzy_func (str): Key name of fuzzy matching function to use.
+            Can only be set at the pattern level. For "FUZZY" patterns only.
+            All rapidfuzz matching functions with default settings are available,
+            however any token-based functions provide no utility at the individual
+            token level. Additional fuzzy matching functions can be registered by users.
+            Included, and useful, functions are:
+
+            * `"simple"` = `ratio`
+            * `"partial"` = `partial_ratio`
+            * `"quick"` = `QRatio`
+            * `"partial_alignment"` = `partial_ratio_alignment`
+                (Requires `rapidfuzz>=2.0.3`)
+
+            Default is `"simple`".
+        fuzzy_weights: Name of weighting method for regex insertion, deletion, and
+            substituion counts. Can only be set at the pattern level. For "FREGEX"
+            patterns only. Included weighting methods are:
+
+            * `"indel"` = `(1, 1, 2)`
+            * `"lev"` = `(1, 1, 1)`
+
+            Default is `"indel"`.
+        predef: Whether regex should be interpreted as a key to
+            a predefined regex pattern or not. Can only be set at the pattern level.
+            For "FREGEX" patterns only. Default is `False`.
     """
 
-    name = "_phrase_matcher"
+    name = "token_matcher"
 
-    def __init__(self: _PhraseMatcher, vocab: Vocab, **defaults: Any) -> None:
-        """Initializes the base phrase matcher with the given defaults.
+    def __init__(self: "TokenMatcher", vocab: Vocab, **defaults: ty.Any) -> None:
+        """Initializes the matcher with the given defaults.
 
         Args:
-            vocab: A spacy `Vocab` object.
-                Purely for consistency between spaCy
-                and spaczz matcher APIs for now.
-                spaczz matchers are currently pure
-                Python and do not share vocabulary
-                with spaCy pipelines.
+            vocab: A spacy `Vocab` object. Purely for consistency between spaCy
+                and spaczz matcher APIs for now. spaczz matchers are currently pure
+                Python and do not share vocabulary with spacy pipelines.
             **defaults: Keyword arguments that will
-                be used as default matching settings.
-                These arguments will become the new defaults for matching.
-                See `_PhraseSearcher` documentation for details.
+                be used as default matching settings for the class instance.
         """
         self.defaults = defaults
-        self.type = "_phrase"
-        self._callbacks: Dict[str, PhraseCallback] = {}
-        self._patterns: DefaultDict[str, DefaultDict[str, Any]] = nest_defaultdict(
-            list, 2
-        )
-        self._searcher = _PhraseSearcher(vocab=vocab)
-
-    def __call__(self: _PhraseMatcher, doc: Doc) -> List[Tuple[str, int, int, int]]:
-        """Find all sequences matching the supplied patterns in `doc`.
+        self._type: SpaczzType = "token"
+        self._callbacks: ty.Dict[str, TokenCallback] = {}
+        self._patterns: ty.DefaultDict[
+            str, ty.List[ty.List[ty.Dict[str, ty.Any]]]
+        ] = ty.DefaultDict(list)
+        self._searcher = TokenSearcher(vocab=vocab)
+
+    def __call__(
+        self: "TokenMatcher", doc: Doc
+    ) -> ty.List[ty.Tuple[str, int, int, int, str]]:
+        """Finds matches in `doc` given the matchers patterns.
 
         Args:
             doc: The `Doc` object to match over.
 
         Returns:
-            A `list` of (key, start, end, ratio) tuples, describing the matches.
+            A list of `MatchResult` tuples,
+            (label, start index, end index, match ratio, pattern).
 
         Example:
             >>> import spacy
-            >>> from spaczz.matcher import _PhraseMatcher
+            >>> from spaczz.matcher import TokenMatcher
             >>> nlp = spacy.blank("en")
-            >>> matcher = _PhraseMatcher(nlp.vocab)
-            >>> doc = nlp("Ridley Scott was the director of Alien.")
-            >>> matcher.add("NAME", [nlp("Ridley Scott")])
-            >>> matcher(doc)
-            [('NAME', 0, 2, 100)]
+            >>> matcher = TokenMatcher(nlp.vocab)
+            >>> doc = nlp("Rdley Scot was the director of Alien.")
+            >>> matcher.add("NAME", [
+                [{"TEXT": {"FUZZY": "Ridley"}},
+                {"TEXT": {"FUZZY": "Scott"}}]
+                ])
+            >>> matcher(doc)[0][:4]
+            ('NAME', 0, 2, 90)
         """
-        matches = set()
+        matches: ty.Set[ty.Tuple[str, int, int, int, str]] = set()
         for label, patterns in self._patterns.items():
-            for pattern, kwargs in zip(patterns["patterns"], patterns["kwargs"]):
-                if not kwargs:
-                    kwargs = self.defaults
-                matches_wo_label = self._searcher.match(doc, pattern, **kwargs)
-                if matches_wo_label:
-                    matches_w_label = [
-                        (label,) + match_wo_label for match_wo_label in matches_wo_label
-                    ]
-                    for match in matches_w_label:
-                        matches.add(match)
-        if matches:
-            sorted_matches = sorted(matches, key=lambda x: (x[1], -x[2] - x[1], -x[3]))
-            for i, (label, _start, _end, _ratio) in enumerate(sorted_matches):
-                on_match = self._callbacks.get(label)
-                if on_match:
-                    on_match(self, doc, i, sorted_matches)
-            return sorted_matches
-        else:
-            return []
+            for pattern in patterns:
+                spaczz_matches = self._searcher.match(doc, pattern, **self.defaults)
+                if spaczz_matches:
+                    for spaczz_match in spaczz_matches:
+                        matcher = Matcher(self.vocab)
+                        matcher.add(label, [self._spacyfy(spaczz_match, pattern)])
+                        spacy_matches = matcher(doc)
+                        for spacy_match in spacy_matches:
+                            matches.add(
+                                self._calc_ratio(
+                                    doc,
+                                    pattern=pattern,
+                                    spaczz_match=spaczz_match,
+                                    spacy_match=ty.cast(
+                                        ty.Tuple[int, int, int], spacy_match
+                                    ),
+                                )
+                            )
+        sorted_matches = sorted(
+            matches, key=lambda x: (-x[1], x[2] - x[1], x[3]), reverse=True
+        )
+        for i, (label, _start, _end, _ratio, _pattern) in enumerate(sorted_matches):
+            on_match = self._callbacks.get(label)
+            if on_match:
+                on_match(self, doc, i, sorted_matches)
+        return sorted_matches
 
-    def __contains__(self: _PhraseMatcher, label: str) -> bool:
+    def __contains__(self: "TokenMatcher", label: str) -> bool:
         """Whether the matcher contains patterns for a label."""
         return label in self._patterns
 
-    def __len__(self: _PhraseMatcher) -> int:
+    def __len__(self: "TokenMatcher") -> int:
         """The number of labels added to the matcher."""
         return len(self._patterns)
 
     def __reduce__(
-        self: _PhraseMatcher,
-    ) -> Tuple[Any, Any]:  # Precisely typing this would be really long.
+        self: "TokenMatcher",
+    ) -> ty.Tuple[ty.Any, ty.Any]:  # Precisely typing this would be really long.
         """Interface for pickling the matcher."""
         data = (
             self.__class__,
             self.vocab,
             self._patterns,
             self._callbacks,
             self.defaults,
         )
         return (unpickle_matcher, data)
 
     @property
-    def labels(self: _PhraseMatcher) -> Tuple[str, ...]:
+    def labels(self: "TokenMatcher") -> ty.Tuple[str, ...]:
         """All labels present in the matcher.
 
         Returns:
-            The unique labels as a `tuple` of strings.
+            The unique labels as a tuple of strings.
 
         Example:
             >>> import spacy
-            >>> from spaczz.matcher import _PhraseMatcher
+            >>> from spaczz.matcher import TokenMatcher
             >>> nlp = spacy.blank("en")
-            >>> matcher = _PhraseMatcher(nlp.vocab)
-            >>> matcher.add("AUTHOR", [nlp("Kerouac")])
+            >>> matcher = TokenMatcher(nlp.vocab)
+            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
             >>> matcher.labels
             ('AUTHOR',)
         """
         return tuple(self._patterns.keys())
 
     @property
-    def patterns(self: _PhraseMatcher) -> List[Dict[str, Any]]:
-        """Get all patterns and kwargs that were added to the matcher.
+    def patterns(self: "TokenMatcher") -> ty.List[ty.Dict[str, ty.Any]]:
+        """Get all patterns and match settings that were added to the matcher.
 
         Returns:
-            The patterns and their kwargs as a `list` of dicts.
+            The patterns and their respective match settings as a list of dicts.
 
         Example:
             >>> import spacy
-            >>> from spaczz.matcher import _PhraseMatcher
+            >>> from spaczz.matcher import TokenMatcher
             >>> nlp = spacy.blank("en")
-            >>> matcher = _PhraseMatcher(nlp.vocab)
-            >>> matcher.add("AUTHOR", [nlp("Kerouac")],
-                [{"ignore_case": False}])
+            >>> matcher = TokenMatcher(nlp.vocab)
+            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
             >>> matcher.patterns == [
                 {
                     "label": "AUTHOR",
-                    "pattern": "Kerouac",
-                    "type": "_phrase",
-                    "kwargs": {"ignore_case": False}
+                    "pattern": [{"TEXT": {"FUZZY": "Kerouac"}}],
+                    "type": "token",
                     },
                     ]
             True
         """
         all_patterns = []
         for label, patterns in self._patterns.items():
-            for pattern, kwargs in zip(patterns["patterns"], patterns["kwargs"]):
-                p = {"label": label, "pattern": pattern.text, "type": self.type}
-                if kwargs:
-                    p["kwargs"] = kwargs
+            for pattern in patterns:
+                p = {"label": label, "pattern": pattern, "type": self.type}
                 all_patterns.append(p)
         return all_patterns
 
     @property
-    def vocab(self: _PhraseMatcher) -> Vocab:
-        """Returns the spaCy `Vocab` object utilized."""
+    def type(self: "TokenMatcher") -> SpaczzType:
+        """Getter for the matchers `SpaczzType`."""
+        return self._type
+
+    @property
+    def vocab(self: "TokenMatcher") -> Vocab:
+        """Getter for the matchers `Vocab`."""
         return self._searcher.vocab
 
     def add(
-        self: _PhraseMatcher,
+        self: "TokenMatcher",
         label: str,
-        patterns: List[Doc],
-        kwargs: Optional[List[Dict[str, Any]]] = None,
-        on_match: PhraseCallback = None,
+        patterns: ty.List[ty.List[ty.Dict[str, ty.Any]]],
+        on_match: "TokenCallback" = None,
     ) -> None:
         """Add a rule to the matcher, consisting of a label and one or more patterns.
 
-        Patterns must be a `list` of `Doc` objects and if kwargs is not `None`,
-        kwargs must be a `list` of dicts.
+        Patterns must be a list of lists of dicts where each list of dicts represent an
+        individual pattern and each dictionary represents an individual token.
+
+        Uses extended spaCy token matching patterns.
+        "FUZZY" and "FREGEX" are the two additional spaCy token pattern options.
+
+        For example::
+
+            [
+                {"TEXT": {"FREGEX": "(database){e<=1}"}},
+                {"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "partial"}},
+            ]
+
+        Make sure to use uppercase dictionary keys in patterns.
 
         Args:
             label: Name of the rule added to the matcher.
-            patterns: `Doc` objects that will be matched
+            patterns: List of lists of dicts that will be matched
                 against the `Doc` object the matcher is called on.
-            kwargs: Optional arguments to modify the behavior of the matching.
-                Apply to inherited multi_match method.
-                See `_PhraseSearcher` documentation for kwarg details.
-                Default is `None`.
             on_match: Optional callback function to modify the
                 `Doc` object the matcher is called on after matching.
                 Default is `None`.
 
         Raises:
-            TypeError: Patterns must be a `list` of `Doc` objects.
-            TypeError: If kwargs is not an `list` of dicts.
-
-        Warnings:
-            KwargsWarning:
-                If there are more patterns than kwargs
-                default matching settings will be used
-                for extra patterns.
-            KwargsWarning:
-                If there are more kwargs dicts than patterns,
-                the extra kwargs will be ignored.
+            TypeError: If patterns is not a list of `Doc` objects.
+            ValueError: Patterns cannot have zero tokens.
 
         Example:
             >>> import spacy
-            >>> from spaczz.matcher import _PhraseMatcher
+            >>> from spaczz.matcher import TokenMatcher
             >>> nlp = spacy.blank("en")
-            >>> matcher = _PhraseMatcher(nlp.vocab)
-            >>> matcher.add("SOUND", [nlp("mooo")])
-            >>> "SOUND" in matcher
+            >>> matcher = TokenMatcher(nlp.vocab)
+            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
+            >>> "AUTHOR" in matcher
             True
         """
-        if not isinstance(patterns, list):
-            raise TypeError("Patterns must be a list of Doc objects.")
-        if kwargs is None:
-            kwargs = [{} for _ in patterns]
-        elif len(kwargs) < len(patterns):
-            warnings.warn(
-                """There are more patterns then there are kwargs.
-                Patterns not matched to a kwarg dict will have default settings.""",
-                KwargsWarning,
-            )
-            kwargs.extend([{} for _ in range(len(patterns) - len(kwargs))])
-        elif len(kwargs) > len(patterns):
-            warnings.warn(
-                """There are more kwargs dicts than patterns.
-                The extra kwargs will be ignored.""",
-                KwargsWarning,
-            )
-        for pattern, kwarg in zip(patterns, kwargs):
-            if isinstance(pattern, Doc):
-                self._patterns[label]["patterns"].append(pattern)
-            else:
-                raise TypeError("Patterns must be a list of Doc objects.")
-            if isinstance(kwarg, dict):
-                self._patterns[label]["kwargs"].append(kwarg)
+        for pattern in patterns:
+            if len(pattern) == 0:
+                raise ValueError("Pattern cannot have zero tokens.")
+            if isinstance(pattern, list):
+                self._patterns[label].append(list(pattern))
             else:
-                raise TypeError("Kwargs must be a list of dicts.")
+                raise TypeError("Patterns must be lists of dictionaries.")
         self._callbacks[label] = on_match
 
-    def remove(self: _PhraseMatcher, label: str) -> None:
+    def remove(self: "TokenMatcher", label: str) -> None:
         """Remove a label and its respective patterns from the matcher.
 
         Args:
             label: Name of the rule added to the matcher.
 
         Raises:
             ValueError: If label does not exist in the matcher.
 
         Example:
             >>> import spacy
-            >>> from spaczz.matcher import _PhraseMatcher
+            >>> from spaczz.matcher import TokenMatcher
             >>> nlp = spacy.blank("en")
-            >>> matcher = _PhraseMatcher(nlp.vocab)
-            >>> matcher.add("SOUND", [nlp("mooo")])
-            >>> matcher.remove("SOUND")
-            >>> "SOUND" in matcher
+            >>> matcher = TokenMatcher(nlp.vocab)
+            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
+            >>> matcher.remove("AUTHOR")
+            >>> "AUTHOR" in matcher
             False
         """
         try:
             del self._patterns[label]
             del self._callbacks[label]
         except KeyError:
             raise ValueError(
                 f"The label: {label} does not exist within the matcher rules."
             )
 
-    def pipe(
-        self: _PhraseMatcher,
-        stream: Iterable[Doc],
-        batch_size: int = 1000,
-        return_matches: bool = False,
-        as_tuples: bool = False,
-    ) -> Generator[Any, None, None]:
-        """Match a stream of `Doc` objects, yielding them in turn.
-
-        Deprecated as of spaCy v3.0 and spaczz v0.5.
-
-        Args:
-            stream: A stream of `Doc` objects.
-            batch_size: Number of documents to accumulate into a working set.
-                Default is `1000`.
-            return_matches: Yield the match lists along with the docs,
-                making results (doc, matches) tuples. Default is `False`.
-            as_tuples: Interpret the input stream as (doc, context) tuples,
-                and yield (result, context) tuples out.
-                If both return_matches and as_tuples are `True`,
-                the output will be a sequence of ((doc, matches), context) tuples.
-                Default is `False`.
+    def _calc_ratio(
+        self: "TokenMatcher",
+        doc: Doc,
+        pattern: ty.List[ty.Dict[str, ty.Any]],
+        spaczz_match: ty.List[ty.Tuple[str, str, int]],
+        spacy_match: ty.Tuple[int, int, int],
+    ) -> ty.Tuple[str, int, int, int, str]:
+        """Calculates the fuzzy ratio for the entire token match."""
+        ratio = round(
+            sum(
+                [
+                    token_match[2]
+                    / sum(
+                        [len(token) for token in doc[spacy_match[1] : spacy_match[2]]]
+                    )
+                    * len(token)
+                    for token, token_match in zip(  # noqa: B905
+                        doc[spacy_match[1] : spacy_match[2]], spaczz_match
+                    )
+                ]
+            )
+        )
 
-        Yields:
-            `Doc` objects, in order.
-        """
-        warnings.warn(
-            """As of spaczz v0.5 and spaCy v3.0, the matcher.pipe method
-        is deprecated. If you need to match on a stream of documents,
-        you can use nlp.pipe and call the matcher on each Doc object.""",
-            PipeDeprecation,
+        return (
+            ty.cast(str, self.vocab.strings[spacy_match[0]]),
+            spacy_match[1],
+            spacy_match[2],
+            ratio,
+            ty.cast(str, srsly.json_dumps(pattern)),
         )
-        if as_tuples:
-            for doc, context in stream:
-                matches = self(doc)
-                if return_matches:
-                    yield ((doc, matches), context)
-                else:
-                    yield (doc, context)
-        else:
-            for doc in stream:
-                matches = self(doc)
-                if return_matches:
-                    yield (doc, matches)
-                else:
-                    yield doc
-
-
-PMT = TypeVar("PMT", bound=_PhraseMatcher)
-PhraseCallback = Optional[
-    Callable[[PMT, Doc, int, List[Tuple[str, int, int, int]]], None]
+
+    @staticmethod
+    def _spacyfy(
+        match: ty.List[ty.Tuple[str, str, int]],
+        pattern: ty.List[ty.Dict[str, ty.Any]],
+    ) -> ty.List[ty.Dict[str, ty.Any]]:
+        """Turns token searcher matches into spaCy `Matcher` compatible patterns."""
+        new_pattern = deepcopy(pattern)
+        for i, token in enumerate(match):
+            if token[0]:
+                del new_pattern[i][token[0]]
+                new_pattern[i]["TEXT"] = token[1]
+        return new_pattern
+
+
+TokenCallback = ty.Optional[
+    ty.Callable[
+        [TokenMatcher, Doc, int, ty.List[ty.Tuple[str, int, int, int, str]]], None
+    ]
 ]
 
 
 def unpickle_matcher(
-    matcher: Type[_PhraseMatcher],
+    matcher: ty.Type[TokenMatcher],
     vocab: Vocab,
-    patterns: DefaultDict[str, DefaultDict[str, Any]],
-    callbacks: Dict[str, PhraseCallback],
-    defaults: Any,
-) -> Any:
+    patterns: ty.DefaultDict[str, ty.List[ty.List[ty.Dict[str, ty.Any]]]],
+    callbacks: ty.Dict[str, TokenCallback],
+    defaults: ty.Any,
+) -> TokenMatcher:
     """Will return a matcher from pickle protocol."""
     matcher_instance = matcher(vocab, **defaults)
     for key, specs in patterns.items():
         callback = callbacks.get(key)
-        matcher_instance.add(key, specs["patterns"], specs["kwargs"], on_match=callback)
+        matcher_instance.add(key, specs, on_match=callback)
     return matcher_instance
```

### Comparing `spaczz-0.5.4/src/spaczz/matcher/regexmatcher.py` & `spaczz-0.6.0a0/src/spaczz/matcher/regexmatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,180 +1,189 @@
-"""Module for RegexMatcher with an API semi-analogous to spaCy's PhraseMatcher."""
-from __future__ import annotations
-
-from typing import (
-    Any,
-    Callable,
-    DefaultDict,
-    Dict,
-    Generator,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-)
+"""Module for RegexMatcher with an API semi-analogous to spaCy's `PhraseMatcher`."""
+import typing as ty
 import warnings
 
 from spacy.tokens import Doc
 from spacy.vocab import Vocab
 
-from ..exceptions import KwargsWarning, PipeDeprecation
-from ..regex import RegexConfig
-from ..search import RegexSearcher
+from .._search import RegexSearcher
+from ..customtypes import MatchResult
+from ..customtypes import SpaczzType
+from ..exceptions import KwargsWarning
 from ..util import nest_defaultdict
 
 
 class RegexMatcher:
-    """spaCy-like matcher for finding multi-token regex matches in `Doc` objects.
+    """spaCy-like matcher for finding regex phrase matches in `Doc` objects.
+
+    Regex matches patterns against the `Doc` it is called on.
+    Accepts labeled patterns in the form of strings with optional,
+    per-pattern match settings.
 
-    Matches added patterns against the `Doc` object it is called on.
-    Accepts labeled regex patterns in the form of strings.
+    To utilize regex flags, use inline flags.
 
     Attributes:
-        defaults: Keyword arguments to be used as default matching settings.
-            See `RegexSearcher` documentation for details.
-        name: Class attribute - the name of the matcher.
-        type: The kind of matcher object.
-        _callbacks:
-            On match functions to modify `Doc` objects passed to the matcher.
-            Can make use of the matches identified.
-        _patterns:
-            Patterns added to the matcher. Contains patterns
-            and kwargs that should be used during matching
-            for each labels added.
+        name (str): Class attribute - the name of the matcher.
+        defaults (dict[str, bool|int|str]):
+            Keyword arguments to be used as default match settings.
+            Per-pattern match settings take precedence over defaults.
+
+    Match Settings:
+        ignore_case (bool): Whether to lower-case text before matching.
+            Default is `True`.
+        min_r (int): Minimum match ratio required.
+        fuzzy_weights (str): Name of weighting method for regex insertion, deletion, and
+            substituion counts. Additional weighting methods can be registered
+            by users. Included weighting methods are:
+
+            * `"indel"` = `(1, 1, 2)`
+            * `"lev"` = `(1, 1, 1)`
+
+            Default is `"indel"`.
+        partial: (bool): Whether partial matches should be extended
+                to `Token` or `Span` boundaries in `doc` or not.
+                For example, the regex only matches part of a `Token` or `Span` in
+                `doc`. Default is `True`.
+        predef (string): Whether the regex string should be interpreted as a key to
+                a predefined regex pattern or not. Additional predefined regex patterns
+                can be registered by users. The included predefined regex patterns are:
+
+                * `"dates"`
+                * `"times"`
+                * `"phones"`
+                * `"phones_with_exts"`
+                * `"links"`
+                * `"emails"`
+                * `"ips"`
+                * `"ipv6s"`
+                * `"prices"`
+                * `"hex_colors"`
+                * `"credit_cards"`
+                * `"btc_addresses"`
+                * `"street_addresses"`
+                * `"zip_codes"`
+                * `"po_boxes"`
+                * `"ssn_numbers"`
+
+                Default is `False`.
     """
 
     name = "regex_matcher"
 
     def __init__(
-        self: RegexMatcher,
+        self: "RegexMatcher",
         vocab: Vocab,
-        config: Union[str, RegexConfig] = "default",
-        **defaults: Any,
+        **defaults: ty.Any,
     ) -> None:
-        """Initializes the regex matcher with the given config and defaults.
+        """Initializes the matcher with the given defaults.
 
         Args:
-            vocab: A spacy `Vocab` object.
-                Purely for consistency between spaCy
-                and spaczz matcher APIs for now.
-                spaczz matchers are currently pure
-                Python and do not share vocabulary
-                with spacy pipelines.
-            config: Provides predefind regex patterns and flags.
-                Uses the default config if "default", an empty config if "empty",
-                or a custom config by passing a `RegexConfig` object.
-                Default is "default".
+            vocab: A spacy `Vocab` object. Purely for consistency between spaCy
+                and spaczz matcher APIs for now. spaczz matchers are currently pure
+                Python and do not share vocabulary with spacy pipelines.
             **defaults: Keyword arguments that will
-                be used as default matching settings.
-                These arguments will become the new defaults for matching.
-                See `RegexSearcher` documentation for details.
+                be used as default matching settings for the class instance.
         """
         self.defaults = defaults
-        self.type = "regex"
-        self._callbacks: Dict[str, RegexCallback] = {}
-        self._patterns: DefaultDict[str, DefaultDict[str, Any]] = nest_defaultdict(
-            list, 2
-        )
-        self._searcher = RegexSearcher(vocab=vocab, config=config)
+        self._type: SpaczzType = "regex"
+        self._callbacks: ty.Dict[str, RegexCallback] = {}
+        self._patterns: ty.DefaultDict[
+            str, ty.DefaultDict[str, ty.Any]
+        ] = nest_defaultdict(list)
+        self._searcher = RegexSearcher(vocab=vocab)
 
-    def __call__(
-        self: RegexMatcher, doc: Doc
-    ) -> List[Tuple[str, int, int, Tuple[int, int, int]]]:
-        r"""Find all sequences matching the supplied patterns in the doc.
+    def __call__(self: "RegexMatcher", doc: Doc) -> ty.List[MatchResult]:
+        r"""Finds matches in `doc` given the matchers patterns.
 
         Args:
             doc: The `Doc` object to match over.
 
         Returns:
-            A list of (key, start, end, fuzzy change count) tuples,
-            describing the matches.
+            A list of `MatchResult` tuples,
+            (label, start index, end index, match ratio, pattern).
 
         Example:
             >>> import spacy
             >>> from spaczz.matcher import RegexMatcher
             >>> nlp = spacy.blank("en")
             >>> matcher = RegexMatcher(nlp.vocab)
             >>> doc = nlp.make_doc("I live in the united states, or the US")
             >>> matcher.add("GPE", ["[Uu](nited|\.?) ?[Ss](tates|\.?)"])
-            >>> matcher(doc)
-            [('GPE', 4, 6, (0, 0, 0)), ('GPE', 9, 10, (0, 0, 0))]
+            >>> matcher(doc)[0]
+            ('GPE', 4, 6, 100, '[Uu](nited|\\.?) ?[Ss](tates|\\.?)')
         """
         matches = set()
         for label, patterns in self._patterns.items():
-            for pattern, kwargs in zip(patterns["patterns"], patterns["kwargs"]):
+            for pattern, kwargs in zip(  # noqa B905
+                patterns["patterns"], patterns["kwargs"]
+            ):
                 if not kwargs:
                     kwargs = self.defaults
                 matches_wo_label = self._searcher.match(doc, pattern, **kwargs)
                 if matches_wo_label:
                     matches_w_label = [
-                        (label,) + match_wo_label for match_wo_label in matches_wo_label
+                        (label, *match_wo_label, str(pattern))
+                        for match_wo_label in matches_wo_label
                     ]
                     for match in matches_w_label:
                         matches.add(match)
-        if matches:
-            sorted_matches = sorted(
-                matches, key=lambda x: (x[1], -x[2] - x[1], sum(x[3]))
-            )
-            for i, (label, _start, _end, _subs) in enumerate(sorted_matches):
-                on_match = self._callbacks.get(label)
-                if on_match:
-                    on_match(self, doc, i, sorted_matches)
-            return sorted_matches
-        else:
-            return []
+        sorted_matches = sorted(
+            matches, key=lambda x: (-x[1], x[2] - x[1], x[3]), reverse=True
+        )
+        for i, (label, _start, _end, _ratio, _pattern) in enumerate(sorted_matches):
+            on_match = self._callbacks.get(label)
+            if on_match:
+                on_match(self, doc, i, sorted_matches)
+        return sorted_matches
 
-    def __contains__(self: RegexMatcher, label: str) -> bool:
+    def __contains__(self: "RegexMatcher", label: str) -> bool:
         """Whether the matcher contains patterns for a label."""
         return label in self._patterns
 
-    def __len__(self: RegexMatcher) -> int:
+    def __len__(self: "RegexMatcher") -> int:
         """The number of labels added to the matcher."""
         return len(self._patterns)
 
     def __reduce__(
-        self: RegexMatcher,
-    ) -> Tuple[Any, Any]:  # Precisely typing this would be really long.
+        self: "RegexMatcher",
+    ) -> ty.Tuple[ty.Any, ty.Any]:  # Precisely typing this would be really long.
         """Interface for pickling the matcher."""
         data = (
             self.__class__,
             self.vocab,
             self._patterns,
             self._callbacks,
             self.defaults,
         )
         return (unpickle_matcher, data)
 
     @property
-    def labels(self: RegexMatcher) -> Tuple[str, ...]:
+    def labels(self: "RegexMatcher") -> ty.Tuple[str, ...]:
         """All labels present in the matcher.
 
         Returns:
-            The unique string labels as a tuple.
+            The unique labels as a tuple of strings.
 
         Example:
             >>> import spacy
             >>> from spaczz.matcher import RegexMatcher
             >>> nlp = spacy.blank("en")
             >>> matcher = RegexMatcher(nlp.vocab)
             >>> matcher.add("ZIP", ["zip_codes"], [{"predef": True}])
             >>> matcher.labels
             ('ZIP',)
         """
         return tuple(self._patterns.keys())
 
     @property
-    def patterns(self: RegexMatcher) -> List[Dict[str, Any]]:
-        """Get all patterns and kwargs that were added to the matcher.
+    def patterns(self: "RegexMatcher") -> ty.List[ty.Dict[str, ty.Any]]:
+        """Get all patterns and match settings that were added to the matcher.
 
         Returns:
-            The original patterns and kwargs,
-            one dictionary for each combination.
+            The patterns and their respective match settings as a list of dicts.
 
         Example:
             >>> import spacy
             >>> from spaczz.matcher import RegexMatcher
             >>> nlp = spacy.blank("en")
             >>> matcher = RegexMatcher(nlp.vocab)
             >>> matcher.add("ZIP", ["zip_codes"], [{"predef": True}])
@@ -186,63 +195,68 @@
                     "kwargs": {"predef": True},
                     }
                     ]
             True
         """
         all_patterns = []
         for label, patterns in self._patterns.items():
-            for pattern, kwargs in zip(patterns["patterns"], patterns["kwargs"]):
+            for pattern, kwargs in zip(  # noqa: B905
+                patterns["patterns"], patterns["kwargs"]
+            ):
                 p = {"label": label, "pattern": pattern, "type": "regex"}
                 if kwargs:
                     p["kwargs"] = kwargs
                 all_patterns.append(p)
         return all_patterns
 
     @property
-    def vocab(self: RegexMatcher) -> Vocab:
-        """Returns the spaCy `Vocab` object utilized."""
+    def type(self: "RegexMatcher") -> SpaczzType:
+        """Getter for the matchers `SpaczzType`."""
+        return self._type
+
+    @property
+    def vocab(self: "RegexMatcher") -> Vocab:
+        """Getter for the matchers `Vocab`."""
         return self._searcher.vocab
 
     def add(
-        self: RegexMatcher,
+        self: "RegexMatcher",
         label: str,
-        patterns: List[str],
-        kwargs: Optional[List[Dict[str, Any]]] = None,
-        on_match: RegexCallback = None,
+        patterns: ty.List[str],
+        kwargs: ty.Optional[ty.List[ty.Dict[str, ty.Any]]] = None,
+        on_match: "RegexCallback" = None,
     ) -> None:
         r"""Add a rule to the matcher, consisting of a label and one or more patterns.
 
-        Patterns must be a list of strings and if kwargs is not `None`,
-        kwargs must be a list of dictionaries.
-
-        To utilize regex flags, use inline flags.
+        Patterns must be a list of `Doc` objects and if `kwargs` is not `None`,
+        `kwargs` must be a list of dicts.
 
         Args:
             label: Name of the rule added to the matcher.
-            patterns: Strings that will be matched against
-                the Doc object the matcher is called on.
-            kwargs: Optional arguments to modify the behavior of the regex matching.
-                Apply to inherited multi_match method.
+            patterns: `Doc` objects that will be matched
+                against the `Doc` object the matcher is called on.
+            kwargs: Optional settings to modify the matching behavior.
+                If supplying `kwargs`, one per pattern should be included.
+                Empty dicts will use the matcher instances default settings.
                 Default is `None`.
             on_match: Optional callback function to modify the
                 `Doc` object the matcher is called on after matching.
                 Default is `None`.
 
         Raises:
-            TypeError: If patterns is not a non-string iterable of strings.
-            TypeError: If kwargs is not a iterable of dictionaries.
+            TypeError: If `patterns` is not a list of strings.
+            TypeError: If `kwargs` is not a list of dictionaries.
 
         Warnings:
             KwargsWarning:
-                If there are more patterns than kwargs
-                default regex matching settings will be used
-                for extra patterns.
-            KwargsWarning:
-                If there are more kwargs dictionaries than patterns,
-                the extra kwargs will be ignored.
+                * If there are more patterns than kwargs
+                  default matching settings will be used
+                  for extra patterns.
+                * If there are more kwargs dicts than patterns,
+                  the extra kwargs will be ignored.
 
         Example:
             >>> import spacy
             >>> from spaczz.matcher import RegexMatcher
             >>> nlp = spacy.blank("en")
             >>> matcher = RegexMatcher(nlp.vocab)
             >>> matcher.add("GPE", ["[Uu](nited|\.?) ?[Ss](tates|\.?)"])
@@ -252,43 +266,45 @@
         if kwargs is None:
             kwargs = [{} for _ in patterns]
         elif len(kwargs) < len(patterns):
             warnings.warn(
                 """There are more patterns then there are kwargs.\n
                     Patterns not matched to a kwarg dict will have default settings.""",
                 KwargsWarning,
+                stacklevel=2,
             )
             kwargs.extend([{} for _ in range(len(patterns) - len(kwargs))])
         elif len(kwargs) > len(patterns):
             warnings.warn(
                 """There are more kwargs dicts than patterns.\n
                     The extra kwargs will be ignored.""",
                 KwargsWarning,
+                stacklevel=2,
             )
-        if isinstance(patterns, str):
-            raise TypeError("Patterns must be a non-string iterable of strings.")
-        for pattern, kwarg in zip(patterns, kwargs):
+        if not isinstance(patterns, list):
+            raise TypeError("Patterns must be a list strings.")
+        for pattern, kwarg in zip(patterns, kwargs):  # noqa: B905
             if isinstance(pattern, str):
                 self._patterns[label]["patterns"].append(pattern)
             else:
-                raise TypeError("Patterns must be a non-string iterable of strings.")
+                raise TypeError("Patterns must be a list of strings.")
             if isinstance(kwarg, dict):
                 self._patterns[label]["kwargs"].append(kwarg)
             else:
-                raise TypeError("Kwargs must be an iterable of dictionaries.")
+                raise TypeError("Kwargs must be a list of dicts.")
         self._callbacks[label] = on_match
 
-    def remove(self: RegexMatcher, label: str) -> None:
+    def remove(self: "RegexMatcher", label: str) -> None:
         r"""Remove a label and its respective patterns from the matcher.
 
         Args:
             label: Name of the rule added to the matcher.
 
         Raises:
-            ValueError: If label does not exist in the matcher.
+            ValueError: If `label` does not exist in the matcher.
 
         Example:
             >>> import spacy
             >>> from spaczz.matcher import RegexMatcher
             >>> nlp = spacy.blank("en")
             >>> matcher = RegexMatcher(nlp.vocab)
             >>> matcher.add("GPE", ["[Uu](nited|\.?) ?[Ss](tates|\.?)"])
@@ -300,75 +316,26 @@
             del self._patterns[label]
             del self._callbacks[label]
         except KeyError:
             raise ValueError(
                 f"The label: {label} does not exist within the matcher rules."
             )
 
-    def pipe(
-        self: RegexMatcher,
-        stream: Iterable[Doc],
-        batch_size: int = 1000,
-        return_matches: bool = False,
-        as_tuples: bool = False,
-    ) -> Generator[Any, None, None]:
-        r"""Match a stream of `Doc` objects, yielding them in turn.
-
-        Deprecated as of spaCy v3.0 and spaczz v0.5.
-
-        Args:
-            stream: A stream of `Doc` objects.
-            batch_size: Number of documents to accumulate into a working set.
-                Default is `1000`.
-            return_matches: Yield the match lists along with the docs,
-                making results (doc, matches) tuples. Default is `False`.
-            as_tuples: Interpret the input stream as (doc, context) tuples,
-                and yield (result, context) tuples out.
-                If both return_matches and as_tuples are `True`,
-                the output will be a sequence of ((doc, matches), context) tuples.
-                Default is `False`.
 
-        Yields:
-            Doc objects, in order.
-        """
-        warnings.warn(
-            """As of spaczz v0.5 and spaCy v3.0, the matcher.pipe method
-        is deprecated. If you need to match on a stream of documents,
-        you can use nlp.pipe and call the matcher on each Doc object.""",
-            PipeDeprecation,
-        )
-        if as_tuples:
-            for doc, context in stream:
-                matches = self(doc)
-                if return_matches:
-                    yield ((doc, matches), context)
-                else:
-                    yield (doc, context)
-        else:
-            for doc in stream:
-                matches = self(doc)
-                if return_matches:
-                    yield (doc, matches)
-                else:
-                    yield doc
-
-
-RegexCallback = Optional[
-    Callable[
-        [RegexMatcher, Doc, int, List[Tuple[str, int, int, Tuple[int, int, int]]]], None
-    ]
+RegexCallback = ty.Optional[
+    ty.Callable[[RegexMatcher, Doc, int, ty.List[MatchResult]], None]
 ]
 
 
 def unpickle_matcher(
-    matcher: Type[RegexMatcher],
+    matcher: ty.Type[RegexMatcher],
     vocab: Vocab,
-    patterns: DefaultDict[str, DefaultDict[str, Any]],
-    callbacks: Dict[str, RegexCallback],
-    defaults: Any,
-) -> Any:
+    patterns: ty.DefaultDict[str, ty.DefaultDict[str, ty.Any]],
+    callbacks: ty.Dict[str, RegexCallback],
+    defaults: ty.Any,
+) -> RegexMatcher:
     """Will return a matcher from pickle protocol."""
     matcher_instance = matcher(vocab, **defaults)
     for key, specs in patterns.items():
         callback = callbacks.get(key)
         matcher_instance.add(key, specs["patterns"], specs["kwargs"], on_match=callback)
     return matcher_instance
```

### Comparing `spaczz-0.5.4/src/spaczz/matcher/tokenmatcher.py` & `spaczz-0.6.0a0/src/spaczz/_search/phrasesearcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,360 +1,321 @@
-"""Module for TokenMatcher with an API semi-analogous to spaCy's Matcher."""
-from __future__ import annotations
-
-from collections import defaultdict
-from copy import deepcopy
-from typing import (
-    Any,
-    Callable,
-    DefaultDict,
-    Dict,
-    Generator,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-)
+"""`PhraseSearcher` ABC for other phrase-based spaczz searchers."""
+import abc
+import typing as ty
 import warnings
 
-from spacy.matcher import Matcher
 from spacy.tokens import Doc
 from spacy.vocab import Vocab
 
-from ..exceptions import PipeDeprecation
-from ..search import TokenSearcher
-
-
-class TokenMatcher:
-    """spaCy-like token matcher for finding flexible matches in `Doc` objects.
-
-    Matches added patterns against the `Doc` object it is called on.
-    Accepts labeled patterns in the form of lists of dictionaries
-    where each list describes an individual pattern and each
-    dictionary describes an individual token.
-
-    Uses extended spaCy token matching patterns.
-    "FUZZY" and "FREGEX" are the two additional spaCy token pattern options.
-
-    For example:
-        {"TEXT": {"FREGEX": "(database){e<=1}"}},
-        {"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "quick_lev"}}
-
-    Make sure to use uppercase dictionary keys in patterns.
-
-    Attributes:
-        defaults: Keyword arguments to be used as default matching settings.
-            See `TokenSearcher.match()` documentation for details.
-        name: Class attribute - the name of the matcher.
-        type: The kind of matcher object.
-        _callbacks:
-            On match functions to modify `Doc` objects passed to the matcher.
-            Can make use of the matches identified.
-        _patterns:
-            Patterns added to the matcher.
-    """
-
-    name = "token_matcher"
+from .searchutil import filter_overlapping_matches
+from ..customtypes import DocLike
+from ..customtypes import FlexType
+from ..customtypes import SearchResult
+from ..customtypes import TextContainer
+from ..exceptions import FlexWarning
+from ..exceptions import RatioWarning
+
+
+class PhraseSearcher(abc.ABC):
+    """Abstract base class for phrase-based match searching in spaCy `Doc` objects."""
+
+    def __init__(self: "PhraseSearcher", vocab: Vocab) -> None:
+        """Initializes the searcher."""
+        self.vocab = vocab
+
+    @abc.abstractmethod
+    def compare(
+        self: "PhraseSearcher", s1: TextContainer, s2: TextContainer, **kwargs: ty.Any
+    ) -> int:
+        """Abstract method."""
+        pass  # pragma: no cover
+
+    def match(
+        self: "PhraseSearcher",
+        doc: Doc,
+        query: DocLike,
+        *,
+        min_r: int = 75,
+        thresh: int = 100,
+        min_r1: ty.Optional[int] = None,
+        min_r2: ty.Optional[int] = None,
+        flex: FlexType = "default",
+        **kwargs: ty.Any,
+    ) -> ty.List[SearchResult]:
+        """Returns phrase matches in a `Doc` object."""
+        flex = self._calc_flex(query, flex)
+        min_r1_, min_r2_ = self._set_ratios(min_r, min_r1, min_r2)
+        min_r1_, min_r2_, thresh = self._check_ratios(min_r1_, min_r2_, thresh, flex)
+        match_map = self._scan(doc, query, min_r1=min_r1_, **kwargs)
+
+        if match_map:
+            positions = list(match_map.keys())
+            matches_w_nones = [
+                self._optimize(
+                    doc,
+                    query,
+                    match_values=match_map,
+                    pos=pos,
+                    flex=flex,
+                    min_r2=min_r2_,
+                    thresh=thresh,
+                    **kwargs,
+                )
+                for pos in positions
+            ]
 
-    def __init__(self: TokenMatcher, vocab: Vocab, **defaults: Any) -> None:
-        """Initializes the base phrase matcher with the given defaults.
+            matches = [match for match in matches_w_nones if match]
+            if matches:
+                return filter_overlapping_matches(
+                    sorted(
+                        [match for match in matches_w_nones if match],
+                        key=lambda x: (-x[2], x[0]),
+                    ),
+                )
+            else:
+                return []
 
-        Args:
-            vocab: A spacy `Vocab` object.
-                Purely for consistency between spaCy
-                and spaczz matcher APIs for now.
-                spaczz matchers are currently pure
-                Python and do not share vocabulary
-                with spaCy pipelines.
-            **defaults: Keyword arguments that will
-                be used as default matching settings.
-                These arguments will become the new defaults for matching.
-                See `TokenSearcher.match()` documentation for details.
-        """
-        self.defaults = defaults
-        self.type = "token"
-        self._callbacks: Dict[str, TokenCallback] = {}
-        self._patterns: DefaultDict[str, List[List[Dict[str, Any]]]] = DefaultDict(list)
-        self._searcher = TokenSearcher(vocab=vocab)
+        return []
 
-    def __call__(self: TokenMatcher, doc: Doc) -> List[Tuple[str, int, int, None]]:
-        """Find all sequences matching the supplied patterns in the doc.
+    def _optimize(
+        self: "PhraseSearcher",
+        doc: Doc,
+        query: DocLike,
+        match_values: ty.Mapping[int, int],
+        pos: int,
+        flex: int,
+        min_r2: int,
+        thresh: int,
+        **kwargs: ty.Any,
+    ) -> ty.Optional[ty.Tuple[int, int, int]]:
+        """Optimizes a potential match by flexing match boundaries.
+
+        For a match from `._scan` that has match ratio >= `min_r1`, the match boundaries
+        will be extended both left and right by `flex` number of tokens and matched
+        back to the original `query`.
+        The optimal start index, end index, and match ratio are returned
+        if the match ratio >= `min_r2`.
 
         Args:
-            doc: The `Doc` object to match over.
+            doc: `Doc` to optimize initial matches over.
+            query: `Doc` or `Span` to match against `doc`.
+            match_values: Dict of initial match start indices keys to match ratios
+                values.
+            pos: Start index of the match being optimized.
+            flex: Number of tokens to move match boundaries
+                left and right during match optimization.
+            min_r2: Minimum match ratio required
+                to pass optimization. This should be high enough
+                to only return quality matches.
+            thresh: If this ratio <= match ratio from the initial scan,
+                no optimization will be attempted.
+            **kwargs: Overflow for child keyword arguments.
 
         Returns:
-            A list of (key, start, end, None) tuples, describing the matches.
-            The final None is a placeholder for future match details.
-
-        Example:
-            >>> import spacy
-            >>> from spaczz.matcher import TokenMatcher
-            >>> nlp = spacy.blank("en")
-            >>> matcher = TokenMatcher(nlp.vocab)
-            >>> doc = nlp("Rdley Scot was the director of Alien.")
-            >>> matcher.add("NAME", [
-                [{"TEXT": {"FUZZY": "Ridley"}},
-                {"TEXT": {"FUZZY": "Scott"}}]
-                ])
-            >>> matcher(doc)
-            [('NAME', 0, 2, None)]
+            Start index, end index, match ratio tuple, or `None`.
         """
-        mapped_patterns = defaultdict(list)
-        matcher = Matcher(self.vocab)
-        for label, patterns in self._patterns.items():
-            for pattern in patterns:
-                mapped_patterns[label].extend(
-                    _spacyfy(
-                        self._searcher.match(doc, pattern, **self.defaults),
-                        pattern,
+        doc_len = len(doc)
+        p_l, bp_l = [pos] * 2
+        p_r, bp_r = [pos + len(query)] * 2
+        r = match_values[pos]
+        if flex and not r >= thresh:
+            optim_r = r
+            for f in range(1, flex + 1):
+                if p_l - f >= 0:
+                    new_r = self.compare(
+                        query, doc[p_l - f : p_r], min_r=optim_r, **kwargs
                     )
-                )
-        for label in mapped_patterns.keys():
-            matcher.add(label, mapped_patterns[label])
-        matches = matcher(doc)
-        if matches:
-            extended_matches = [
-                (self.vocab.strings[match_id], start, end, None)
-                for match_id, start, end in matches
-            ]
-            extended_matches.sort(key=lambda x: (x[1], -x[2] - x[1]))
-            for i, (label, _start, _end, _details) in enumerate(extended_matches):
-                on_match = self._callbacks.get(label)
-                if on_match:
-                    on_match(self, doc, i, extended_matches)
-            return extended_matches
-        else:
-            return []
-
-    def __contains__(self: TokenMatcher, label: str) -> bool:
-        """Whether the matcher contains patterns for a label."""
-        return label in self._patterns
-
-    def __len__(self: TokenMatcher) -> int:
-        """The number of labels added to the matcher."""
-        return len(self._patterns)
-
-    def __reduce__(
-        self: TokenMatcher,
-    ) -> Tuple[Any, Any]:  # Precisely typing this would be really long.
-        """Interface for pickling the matcher."""
-        data = (
-            self.__class__,
-            self.vocab,
-            self._patterns,
-            self._callbacks,
-            self.defaults,
-        )
-        return (unpickle_matcher, data)
-
-    @property
-    def labels(self: TokenMatcher) -> Tuple[str, ...]:
-        """All labels present in the matcher.
-
-        Returns:
-            The unique string labels as a tuple.
-
-        Example:
-            >>> import spacy
-            >>> from spaczz.matcher import TokenMatcher
-            >>> nlp = spacy.blank("en")
-            >>> matcher = TokenMatcher(nlp.vocab)
-            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
-            >>> matcher.labels
-            ('AUTHOR',)
-        """
-        return tuple(self._patterns.keys())
+                    if new_r:
+                        optim_r = new_r
+                        bp_l = p_l - f
+                        bp_r = p_r
+                if p_l + f < p_r:
+                    new_r = self.compare(
+                        query, doc[p_l + f : p_r], min_r=optim_r, **kwargs
+                    )
+                    if new_r:
+                        optim_r = new_r
+                        bp_l = p_l + f
+                        bp_r = p_r
+                if p_r - f > p_l:
+                    new_r = self.compare(
+                        query, doc[p_l : p_r - f], min_r=optim_r, **kwargs
+                    )
+                    if new_r:
+                        optim_r = new_r
+                        bp_l = p_l
+                        bp_r = p_r - f
+                if p_r + f <= doc_len:
+                    new_r = self.compare(
+                        query, doc[p_l : p_r + f], min_r=optim_r, **kwargs
+                    )
+                    if new_r:
+                        optim_r = new_r
+                        bp_l = p_l
+                        bp_r = p_r + f
+                if p_l - f >= 0 and p_r + f <= doc_len:
+                    new_r = self.compare(
+                        query, doc[p_l - f : p_r + f], min_r=optim_r, **kwargs
+                    )
+                    if new_r:
+                        optim_r = new_r
+                        bp_l = p_l - f
+                        bp_r = p_r + f
+                if p_l + f < p_r and p_r - f > p_l:
+                    new_r = self.compare(
+                        query, doc[p_l + f : p_r - f], min_r=optim_r, **kwargs
+                    )
+                    if new_r:
+                        optim_r = new_r
+                        bp_l = p_l + f
+                        bp_r = p_r - f
+                if optim_r == r:
+                    break
+                else:
+                    r = optim_r
+        if r >= min_r2:
+            return (bp_l, bp_r, r)
+        return None
+
+    def _scan(
+        self: "PhraseSearcher",
+        doc: Doc,
+        query: DocLike,
+        min_r1: int,
+        **kwargs: ty.Any,
+    ) -> ty.Optional[ty.Dict[int, int]]:
+        """Finds potential match start indices.
+
+        Iterates through `doc` by chunks of `len(query)`
+        and comapares each resulting chunk against the `query` looking for
+        match ratios >= `min_r1`.
 
-    @property
-    def patterns(self: TokenMatcher) -> List[Dict[str, Any]]:
-        """Get all patterns that were added to the matcher.
+        Args:
+            doc: `Doc` object to search over.
+            query: `Doc` or `Span` to match against `doc`.
+            min_r1: Minimum match ratio required for
+                selection during the initial search over `doc`.
+                This should be "low" in general because match boundaries
+                are not flexed here. A value of `0` here means all chunks of
+                `len(query)` in `doc` will have their boundaries flexed and recompared
+                during match optimization. Lower `min_r1` will result in more
+                fine-grained matching but will run slower.
+            **kwargs: Overflow for child keyword arguments.
 
         Returns:
-            The original patterns, one dictionary for each combination.
-
-        Example:
-            >>> import spacy
-            >>> from spaczz.matcher import TokenMatcher
-            >>> nlp = spacy.blank("en")
-            >>> matcher = TokenMatcher(nlp.vocab)
-            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
-            >>> matcher.patterns == [
-                {
-                    "label": "AUTHOR",
-                    "pattern": [{"TEXT": {"FUZZY": "Kerouac"}}],
-                    "type": "token",
-                    },
-                    ]
-            True
+            Dict of match start index keys to match ratio values or `None`.
         """
-        all_patterns = []
-        for label, patterns in self._patterns.items():
-            for pattern in patterns:
-                p = {"label": label, "pattern": pattern, "type": self.type}
-                all_patterns.append(p)
-        return all_patterns
-
-    @property
-    def vocab(self: TokenMatcher) -> Vocab:
-        """Returns the spaCy `Vocab` object utilized."""
-        return self._searcher.vocab
-
-    def add(
-        self: TokenMatcher,
-        label: str,
-        patterns: List[List[Dict[str, Any]]],
-        on_match: TokenCallback = None,
-    ) -> None:
-        """Add a rule to the matcher, consisting of a label and one or more patterns.
-
-        Patterns must be a list of dictionary lists where each dictionary
-        list represent an individual pattern and each dictionary represents
-        an individual token.
-
-        Uses extended spaCy token matching patterns.
-        "FUZZY" and "FREGEX" are the two additional spaCy token pattern options.
-
-        For example:
-            {"TEXT": {"FREGEX": "(database){e<=1}"}},
-            {"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "quick_lev"}}
+        doc_len = len(doc)
+        query_len = len(query)
+        if not query_len:
+            return None
+        match_values: ty.Dict[int, int] = dict()
+        i = 0
+        while i + query_len <= doc_len:
+            match = self.compare(
+                query,
+                doc[i : i + query_len],
+                min_r=min_r1 if min_r1 else 1,
+                **kwargs,
+            )
+            if match:
+                match_values[i] = match
+            i += 1
+        if match_values:
+            return match_values
+        else:
+            return None
 
-        Args:
-            label: Name of the rule added to the matcher.
-            patterns: List of dictionary lists that will be matched
-                against the `Doc` object the matcher is called on.
-            on_match: Optional callback function to modify the
-                `Doc` object the matcher is called on after matching.
-                Default is `None`.
+    @staticmethod
+    def _calc_flex(query: DocLike, flex: FlexType) -> int:
+        """Returns a valid `flex` value given `query`.
 
-        Raises:
-            TypeError: If patterns is not an iterable of `Doc` objects.
-            ValueError: pattern cannot have zero tokens.
+        By default `flex` is set to `len(query) // 2`.
 
-        Example:
-            >>> import spacy
-            >>> from spaczz.matcher import TokenMatcher
-            >>> nlp = spacy.blank("en")
-            >>> matcher = TokenMatcher(nlp.vocab)
-            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
-            >>> "AUTHOR" in matcher
-            True
-        """
-        for pattern in patterns:
-            if len(pattern) == 0:
-                raise ValueError("pattern cannot have zero tokens.")
-            if isinstance(pattern, list):
-                self._patterns[label].append(list(pattern))
-            else:
-                raise TypeError("Patterns must be lists of dictionaries.")
-        self._callbacks[label] = on_match
+        If `flex` is `'max'`, or an `int` > `len(query)`,
+        `flex` will be set to `len(query)` value instead.
 
-    def remove(self: TokenMatcher, label: str) -> None:
-        """Remove a label and its respective patterns from the matcher.
+        If `flex` is `'min`', or an `int` < `0`,
+        `flex` will be set to `0` instead.
 
         Args:
-            label: Name of the rule added to the matcher.
+            query: The `Doc`, `Span`, or `Token` to match with.
+            flex: Either `"default"`: `len(query) // 2`,
+                `"max"`: `len(query)`,
+                `"min"`: `0`,
+                or an `int`.
+
+        Returns:
+            The new `flex` value.
 
         Raises:
-            ValueError: If label does not exist in the matcher.
+            TypeError: If `flex` is not `"default"`, `"max"`, `"min"`, or an `int`.
 
-        Example:
-            >>> import spacy
-            >>> from spaczz.matcher import TokenMatcher
-            >>> nlp = spacy.blank("en")
-            >>> matcher = TokenMatcher(nlp.vocab)
-            >>> matcher.add("AUTHOR", [[{"TEXT": {"FUZZY": "Kerouac"}}]])
-            >>> matcher.remove("AUTHOR")
-            >>> "AUTHOR" in matcher
-            False
+        Warnings:
+            FlexWarning:
+                If `flex` > `len(query)` or `flex` < `0`.
         """
-        try:
-            del self._patterns[label]
-            del self._callbacks[label]
-        except KeyError:
-            raise ValueError(
-                f"The label: {label} does not exist within the matcher rules."
+        if flex == "default":
+            flex = len(query) // 2
+        elif flex == "max":
+            flex = len(query)
+        elif flex == "min":
+            flex = 0
+        elif isinstance(flex, int):
+            query_len = len(query)
+            if flex > query_len:
+                warnings.warn(
+                    f"""`flex` of size `{flex}` is > `len(query)`, `{query_len}`.
+                        Setting `flex` to `{query_len}` instead.""",
+                    FlexWarning,
+                    stacklevel=2,
+                )
+                flex = query_len
+            elif flex < 0:
+                warnings.warn(
+                    """`flex` values < `0` are not allowed.
+                    Setting to the min, `0`, instead.""",
+                    FlexWarning,
+                    stacklevel=2,
+                )
+                flex = 0
+        else:
+            raise TypeError(
+                (
+                    "`flex` must be a `FlexLiteral` (`'default'`,",
+                    "`'max'` or `'min'`), or an `int`.",
+                )
             )
+        return flex
 
-    def pipe(
-        self: TokenMatcher,
-        stream: Iterable[Doc],
-        batch_size: int = 1000,
-        return_matches: bool = False,
-        as_tuples: bool = False,
-    ) -> Generator[Any, None, None]:
-        """Match a stream of `Doc` objects, yielding them in turn.
-
-        Deprecated as of spaCy v3.0 and spaczz v0.5.
-
-        Args:
-            stream: A stream of `Doc` objects.
-            batch_size: Number of documents to accumulate into a working set.
-                Default is `1000`.
-            return_matches: Yield the match lists along with the docs,
-                making results (doc, matches) tuples. Default is `False`.
-            as_tuples: Interpret the input stream as (doc, context) tuples,
-                and yield (result, context) tuples out.
-                If both return_matches and as_tuples are `True`,
-                the output will be a sequence of ((doc, matches), context) tuples.
-                Default is `False`.
-
-        Yields:
-            `Doc` objects, in order.
-        """
-        warnings.warn(
-            """As of spaczz v0.5 and spaCy v3.0, the matcher.pipe method
-        is deprecated. If you need to match on a stream of documents,
-        you can use nlp.pipe and call the matcher on each Doc object.""",
-            PipeDeprecation,
-        )
-        if as_tuples:
-            for doc, context in stream:
-                matches = self(doc)
-                if return_matches:
-                    yield ((doc, matches), context)
-                else:
-                    yield (doc, context)
+    @staticmethod
+    def _set_ratios(
+        min_r: int, min_r1: ty.Optional[int], min_r2: ty.Optional[int]
+    ) -> ty.Tuple[int, int]:
+        """Sets `min_r1` and `min_r2` based on `min_r` heuristic or provided values."""
+        min_r1_ = min_r1 if min_r1 is not None else round(min_r / 1.5)
+        min_r2_ = min_r2 if min_r2 is not None else min_r
+        return min_r1_, min_r2_
+
+    @staticmethod
+    def _check_ratios(
+        min_r1: int, min_r2: int, thresh: int, flex: int
+    ) -> ty.Tuple[int, int, int]:
+        """Ensures match ratio requirements are not set to illegal values."""
+        if flex:
+            if min_r1 > min_r2:
+                warnings.warn(
+                    "`min_r1` > `min_r2`, setting `min_r1` = `min_r2`",
+                    RatioWarning,
+                    stacklevel=2,
+                )
+                min_r1 = min_r2
+            if thresh < min_r2:
+                warnings.warn(
+                    "`thresh` < `min_r2`, setting `thresh` = `min_r2`",
+                    RatioWarning,
+                    stacklevel=2,
+                )
+                thresh = min_r2
         else:
-            for doc in stream:
-                matches = self(doc)
-                if return_matches:
-                    yield (doc, matches)
-                else:
-                    yield doc
-
-
-def _spacyfy(
-    matches: List[List[Optional[Tuple[str, str]]]], pattern: List[Dict[str, Any]]
-) -> List[List[Dict[str, Any]]]:
-    """Turns token searcher matches into spaCy `Matcher` compatible patterns."""
-    new_patterns = []
-    if matches:
-        for match in matches:
-            new_pattern = deepcopy(pattern)
-            for i, token in enumerate(match):
-                if token:
-                    del new_pattern[i][token[0]]
-                    new_pattern[i]["TEXT"] = token[1]
-            new_patterns.append(new_pattern)
-    return new_patterns
-
-
-TokenCallback = Optional[
-    Callable[[TokenMatcher, Doc, int, List[Tuple[str, int, int, None]]], None]
-]
-
-
-def unpickle_matcher(
-    matcher: Type[TokenMatcher],
-    vocab: Vocab,
-    patterns: DefaultDict[str, List[List[Dict[str, Any]]]],
-    callbacks: Dict[str, TokenCallback],
-    defaults: Any,
-) -> Any:
-    """Will return a matcher from pickle protocol."""
-    matcher_instance = matcher(vocab, **defaults)
-    for key, specs in patterns.items():
-        callback = callbacks.get(key)
-        matcher_instance.add(key, specs, on_match=callback)
-    return matcher_instance
+            min_r1 = min_r2
+        return min_r1, min_r2, thresh
```

### Comparing `spaczz-0.5.4/src/spaczz/pipeline/_spaczzruler.py` & `spaczz-0.6.0a0/src/spaczz/pipeline/spaczzruler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,234 +1,246 @@
-"""Module for spaCy v3 compatible SpaczzRuler."""
-from __future__ import annotations
-
+"""Module for the SpaczzRuler."""
 from collections import defaultdict
-from itertools import chain
-from logging import exception
 from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    DefaultDict,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    Union,
-)
+import typing as ty
 import warnings
 
-try:
-    from spacy.language import Language
-    from spacy.pipeline import Pipe
-    from spacy.scorer import get_ner_prf
-    from spacy.tokens import Doc, Span
-    from spacy.training import Example, validate_examples
-    from spacy.util import SimpleFrozenDict, SimpleFrozenList
-except ImportError:  # pragma: no cover
-    raise ImportError(
-        (
-            "Trying to import spaCy v3 compatible SpaczzRuler from spaCy v2.",
-            "Please upgrade or use the SpaczzRuler in _spaczzruler-legacy",
-        )
-    )
+from spacy.language import Language
+from spacy.pipeline import Pipe
+from spacy.scorer import get_ner_prf
+from spacy.tokens import Doc
+from spacy.tokens import Span
+from spacy.training import Example
+from spacy.training import validate_examples
+from spacy.util import registry
+from spacy.util import SimpleFrozenDict
+from spacy.util import SimpleFrozenList
 import srsly
 
+from ..customtypes import RulerPattern
+from ..customtypes import RulerResult
+from ..customtypes import SpaczzType
 from ..exceptions import PatternTypeWarning
-from ..matcher import FuzzyMatcher, RegexMatcher, TokenMatcher
-from ..regex import RegexConfig
-from ..util import ensure_path, nest_defaultdict, read_from_disk, write_to_disk
-
+from ..matcher import FuzzyMatcher
+from ..matcher import RegexMatcher
+from ..matcher import TokenMatcher
+from ..util import ensure_path
+from ..util import nest_defaultdict
+from ..util import read_from_disk
+from ..util import write_to_disk
 
 DEFAULT_ENT_ID_SEP = "||"
-simple_frozen_dict = SimpleFrozenDict()
-simple_frozen_list = SimpleFrozenList()
+SIMPLE_FROZEN_DICT = SimpleFrozenDict()
+SIMPLE_FROZEN_LIST = SimpleFrozenList()
+
+REQUIRE_PATTERNS_WARNING = (
+    "The component 'spaczz_ruler' does not have any patterns defined."
+)
+warnings.filterwarnings("once", message=REQUIRE_PATTERNS_WARNING)
+
+DEFAULT_CONFIG = {
+    "overwrite_ents": False,
+    "ent_id_sep": DEFAULT_ENT_ID_SEP,
+    "fuzzy_defaults": SIMPLE_FROZEN_DICT,
+    "regex_defaults": SIMPLE_FROZEN_DICT,
+    "token_defaults": SIMPLE_FROZEN_DICT,
+    "scorer": {"@scorers": "spaczz.spaczz_ruler_scorer.v1"},
+}
+
+
+def spaczz_ruler_scorer(
+    examples: ty.Iterable[Example], **kwargs: ty.Any
+) -> ty.Dict[str, ty.Any]:
+    """Default spaczz scorer."""
+    return get_ner_prf(examples)
+
+
+if getattr(registry, "scorers", None):  # pragma: no cover
+
+    @registry.scorers("spaczz.spaczz_ruler_scorer.v1")  # type: ignore[attr-defined]
+    def make_spaczz_ruler_scorer() -> (
+        ty.Callable[[ty.Iterable[Example]], ty.Dict[str, ty.Any]]
+    ):
+        """Wrapping `spaczz_ruler_scorer` in a callable."""
+        return spaczz_ruler_scorer
+
+else:
+    del DEFAULT_CONFIG["scorer"]
 
 
 @Language.factory(
     "spaczz_ruler",
     assigns=["doc.ents", "token.ent_type", "token.ent_iob"],
-    default_config={
-        "overwrite_ents": False,
-        "ent_id_sep": DEFAULT_ENT_ID_SEP,
-        "fuzzy_defaults": simple_frozen_dict,
-        "regex_defaults": simple_frozen_dict,
-        "token_defaults": simple_frozen_dict,
-    },
+    default_config=DEFAULT_CONFIG,
     default_score_weights={
         "ents_f": 1.0,
         "ents_p": 0.0,
         "ents_r": 0.0,
         "ents_per_type": None,
     },
 )
 def make_spaczz_ruler(
-    # typing nlp with Language causes issue with Pydantic in spaCy integration
-    nlp: Any,
+    nlp: Language,
     name: str,
     overwrite_ents: bool,
     ent_id_sep: str,
-    fuzzy_defaults: Dict[str, Any],
-    regex_defaults: Dict[str, Any],
-    token_defaults: Dict[str, Any],
-) -> SpaczzRuler:
+    fuzzy_defaults: ty.Dict[str, ty.Any],
+    regex_defaults: ty.Dict[str, ty.Any],
+    token_defaults: ty.Dict[str, ty.Any],
+    scorer: ty.Optional[ty.Callable] = None,
+) -> "SpaczzRuler":
     """Factory method for creating a `SpaczzRuler`."""
     return SpaczzRuler(
         nlp,
         name,
         overwrite_ents=overwrite_ents,
         ent_id_sep=ent_id_sep,
         fuzzy_defaults=fuzzy_defaults,
         regex_defaults=regex_defaults,
         token_defaults=token_defaults,
+        scorer=scorer,
     )
 
 
 class SpaczzRuler(Pipe):
-    """The `SpaczzRuler` adds fuzzy and multi-token regex matches to spaCy `Doc.ents`.
+    """The `SpaczzRuler` adds fuzzy matches to spaCy `Doc.ents`.
 
     It can be combined with other spaCy NER components like the statistical
-    `EntityRecognizer` and/or the `EntityRuler` to boost accuracy.
+    `EntityRecognizer`, and/or the `EntityRuler` it is inspired by, to boost accuracy.
     After initialization, the component is typically added to the pipeline
     using `nlp.add_pipe`.
 
     Attributes:
-        nlp: The shared nlp object to pass the vocab to the matchers
-            (not currently used by spaczz matchers) and process fuzzy patterns.
-        fuzzy_patterns:
-            Patterns added to the fuzzy matcher.
-        regex_patterns:
-            Patterns added to the regex matcher.
-        token_patterns:
-            Patterns added to the token matcher
-        fuzzy_matcher: The `FuzzyMatcher` instance
+        nlp (Language): The shared `Language` object that passes its `Vocab` to the
+            matchers (not currently used by spaczz matchers) and processes fuzzy
+            patterns.
+        name (str): Instance name of the current pipeline component. Typically
+            passed in automatically from the factory when the component is
+            added. Used to disable the current entity ruler while creating
+            phrase patterns with the nlp object.
+        overwrite_ents (bool): If existing entities are present, e.g. entities
+            added by the model, overwrite them by matches if necessary.
+        ent_id_sep (str): Separator used internally for entity IDs.
+        scorer (Optional[Callable]): The scoring method for the ruler.
+        fuzzy_matcher (FuzzyMatcher): The `FuzzyMatcher` instance
             the spaczz ruler will use for fuzzy phrase matching.
-        regex_matcher: The `RegexMatcher` instance
+        regex_matcher (RegexMatcher): The `RegexMatcher` instance
             the spaczz ruler will use for regex phrase matching.
-        token_matcher: The `TokenMatcher` instance
-            the spaczz ruler will use for token matching.
-        defaults: Default matching settings for their respective matchers.
+        token_matcher (TokenMatcher): The `TokenMatcher` instance
+            the spaczz ruler will use for fuzzy token matching.
+        defaults (Dict[str, Any]): Default match settings for their respective matchers.
     """
 
     name = "spaczz_ruler"
 
     def __init__(
-        self: SpaczzRuler,
+        self: "SpaczzRuler",
         nlp: Language,
         name: str = "spaczz_ruler",
         *,
         overwrite_ents: bool = False,
         ent_id_sep: str = DEFAULT_ENT_ID_SEP,
-        fuzzy_defaults: Dict[str, Any] = simple_frozen_dict,
-        regex_defaults: Dict[str, Any] = simple_frozen_dict,
-        token_defaults: Dict[str, Any] = simple_frozen_dict,
-        regex_config: Union[str, RegexConfig] = "default",
-        patterns: Optional[Iterable[Dict[str, Any]]] = None,
-        **kwargs: Any,
+        fuzzy_defaults: ty.Dict[str, ty.Any] = SIMPLE_FROZEN_DICT,
+        regex_defaults: ty.Dict[str, ty.Any] = SIMPLE_FROZEN_DICT,
+        token_defaults: ty.Dict[str, ty.Any] = SIMPLE_FROZEN_DICT,
+        patterns: ty.Optional[ty.List[RulerPattern]] = None,
+        scorer: ty.Optional[ty.Callable] = spaczz_ruler_scorer,
     ) -> None:
         """Initialize the spaczz ruler.
 
         If `patterns` is supplied here, it needs to be an iterable of spaczz patterns:
         dictionaries with `"label"`, `"pattern"`, and `"type"` keys.
         If the patterns are fuzzy or regex phrase patterns
         they can include the optional `"kwargs"` keys.
 
-        For example, a fuzzy phrase pattern:
-        `{'label': 'ORG', 'pattern': 'Apple',
-        'type': 'fuzzy', 'kwargs': {'min_r2': 90}}`
-
-        Or, a token pattern:
-        `{'label': 'ORG', 'pattern': [{'TEXT': {'FUZZY': 'Apple'}}], 'type': 'token'}`
-
-        Prior to spaczz v0.5, optional parameters had to be prepended with "spaczz_"
-        to prevent potential conflicts with other spaCy components.
-        As of spaCy v3 this is no longer an issue so prepending optional parameters
-        with "spaczz_" is no longer necessary.
+        For example, a fuzzy phrase pattern::
 
+            {
+                'label': 'ORG',
+                'pattern': 'Apple',
+                'kwargs': {'min_r2': 90},
+                'type': 'fuzzy',
+            }
+
+        Or, a token pattern::
+
+            {
+                'label': 'ORG',
+                'pattern': [{'TEXT': {'FUZZY': 'Apple'}}],
+                'type': 'token',
+            }
 
         Args:
-            nlp: The shared `Language` object to pass the vocab to the matchers
-                and process fuzzy patterns.
-            name: Instance name of the current pipeline component. Typically
+            nlp (Language): The shared `Language` object that passes its `Vocab` to the
+                matchers (not currently used by spaczz matchers) and processes fuzzy
+                patterns.
+            name (str): Instance name of the current pipeline component. Typically
                 passed in automatically from the factory when the component is
                 added. Used to disable the current entity ruler while creating
                 phrase patterns with the nlp object.
-            overwrite_ents: If existing entities are present, e.g. entities
+            overwrite_ents (bool): If existing entities are present, e.g. entities
                 added by the model, overwrite them by matches if necessary.
-                Default is `False`.
-            ent_id_sep: Separator used internally for entity IDs.
-            fuzzy_defaults: Modified default parameters to use with the `FuzzyMatcher`.
-                Default is `None`.
-            regex_defaults: Modified default parameters to use with the `RegexMatcher`.
-                Default is `None`.
-            token_defaults: Modified default parameters to use with the `TokenMatcher`.
-                Default is `None`.
-            regex_config: Should largely be ignored as an artifact of an old spaczz
-                design pattern. Will likely be updated in the future.
-                Default is `"default"`.
-            patterns: Optional patterns to load in. Default is `None`.
-            kwargs: For backwards compatibility with "spaczz_" prepended parameters.
+            ent_id_sep (str): Separator used internally for entity IDs.
+            fuzzy_defaults (Dict[str, Any]): Modified default parameters to use with
+                the `FuzzyMatcher`. Default is `None`.
+            regex_defaults (Dict[str, Any]): Modified default parameters to use with
+                the `RegexMatcher`. Default is `None`.
+            token_defaults (Dict[str, Any]): Modified default parameters to use with
+                the `TokenMatcher`. Default is `None`.
+            patterns (Optional[Dict[str, str | Dict[str, Any] | List[Dict[str, Any]]]):
+                Optional patterns to load in.
+            scorer (Optional[Callable]): The scoring method. Defaults to
+                `spacy.scorer.get_ner_prf`.
 
         Raises:
             TypeError: If matcher defaults passed are not dictionaries.
         """
         self.nlp = nlp
         self.name = name
-        self.overwrite = kwargs.get("spaczz_overwrite_ents", overwrite_ents)
-        self.fuzzy_patterns: DefaultDict[str, DefaultDict[str, Any]] = nest_defaultdict(
-            list, 2
-        )
-        self.regex_patterns: DefaultDict[str, DefaultDict[str, Any]] = nest_defaultdict(
-            list, 2
-        )
-        self.token_patterns: DefaultDict[str, List[List[Dict[str, Any]]]] = defaultdict(
-            list
-        )
-        self.ent_id_sep = kwargs.get("spaczz_ent_id_sep", ent_id_sep)
-        self._ent_ids: DefaultDict[Any, Any] = defaultdict(dict)
+        self.overwrite = overwrite_ents
+        self._fuzzy_patterns: ty.DefaultDict[
+            str, ty.DefaultDict[str, ty.Any]
+        ] = nest_defaultdict(list)
+        self._regex_patterns: ty.DefaultDict[
+            str, ty.DefaultDict[str, ty.Any]
+        ] = nest_defaultdict(list)
+        self._token_patterns: ty.DefaultDict[
+            str, ty.List[ty.List[ty.Dict[str, ty.Any]]]
+        ] = defaultdict(list)
+        self.ent_id_sep = ent_id_sep
+        self._ent_ids: ty.DefaultDict[ty.Any, ty.Any] = defaultdict(dict)
         self.defaults = {}
-        default_names = (
-            "fuzzy_defaults",
-            "regex_defaults",
-            "token_defaults",
-        )
-        fuzzy_defaults = kwargs.get("spaczz_fuzzy_defaults", fuzzy_defaults)
-        regex_defaults = kwargs.get("spaczz_regex_defaults", regex_defaults)
-        token_defaults = kwargs.get("spaczz_token_defaults", token_defaults)
-        for default, name in zip(
+        default_names = ("fuzzy_defaults", "regex_defaults", "token_defaults")
+        for default, name in zip(  # noqa: B905
             (fuzzy_defaults, regex_defaults, token_defaults), default_names
         ):
             if isinstance(default, dict):
                 self.defaults[name] = default
             else:
                 raise TypeError(
                     (
-                        "Defaults must be a dictionary of keyword arguments,",
-                        f"not {type(default)}.",
+                        "`{name}` must be a dictionary of keyword arguments,",
+                        f"not `{type(default)}`.",
                     )
                 )
         self.fuzzy_matcher = FuzzyMatcher(nlp.vocab, **self.defaults["fuzzy_defaults"])
-        self.regex_matcher = RegexMatcher(
-            nlp.vocab, regex_config, **self.defaults["regex_defaults"]
-        )
+        self.regex_matcher = RegexMatcher(nlp.vocab, **self.defaults["regex_defaults"])
         self.token_matcher = TokenMatcher(nlp.vocab, **self.defaults["token_defaults"])
-        patterns = kwargs.get("spaczz_patterns", patterns)
         if patterns is not None:
             self.add_patterns(patterns)
+        self.scorer = scorer
 
-    def __call__(self: SpaczzRuler, doc: Doc) -> Doc:
+    def __call__(self: "SpaczzRuler", doc: Doc) -> Doc:
         """Find matches in document and add them as entities.
 
         Args:
-            doc: The Doc object in the pipeline.
+            doc: The `Doc` object in the pipeline.
 
         Returns:
-            The Doc with added entities, if available.
+            The `Doc` with added entities, if available.
 
         Example:
             >>> import spacy
             >>> from spaczz.pipeline import SpaczzRuler
             >>> nlp = spacy.blank("en")
             >>> ruler = SpaczzRuler(nlp)
             >>> doc = nlp.make_doc("My name is Anderson, Grunt")
@@ -236,37 +248,41 @@
                 "type": "fuzzy", "kwargs": {"fuzzy_func": "token_sort"}}])
             >>> doc = ruler(doc)
             >>> "Anderson, Grunt" in [ent.text for ent in doc.ents]
             True
         """
         error_handler = self.get_error_handler()
         try:
-            matches, lookup = self.match(doc)
-            self.set_annotations(doc, matches, lookup)
+            matches = self.match(doc)
+            self.set_annotations(doc, matches)
             return doc
-        except exception as e:  # type: ignore
+        except Exception as e:
             error_handler(self.name, self, [doc], e)
 
-    def __contains__(self: SpaczzRuler, label: str) -> bool:
+    def __contains__(self: "SpaczzRuler", label: str) -> bool:
         """Whether a label is present in the patterns."""
         return (
-            label in self.fuzzy_patterns
-            or label in self.regex_patterns
-            or label in self.token_patterns
+            label in self._fuzzy_patterns
+            or label in self._regex_patterns
+            or label in self._token_patterns
         )
 
-    def __len__(self: SpaczzRuler) -> int:
+    def __len__(self: "SpaczzRuler") -> int:
         """The number of all patterns added to the ruler."""
-        n_fuzzy_patterns = sum(len(p["patterns"]) for p in self.fuzzy_patterns.values())
-        n_regex_patterns = sum(len(p["patterns"]) for p in self.regex_patterns.values())
-        n_token_patterns = sum(len(p) for p in self.token_patterns.values())
+        n_fuzzy_patterns = sum(
+            len(p["patterns"]) for p in self._fuzzy_patterns.values()
+        )
+        n_regex_patterns = sum(
+            len(p["patterns"]) for p in self._regex_patterns.values()
+        )
+        n_token_patterns = sum(len(p) for p in self._token_patterns.values())
         return n_fuzzy_patterns + n_regex_patterns + n_token_patterns
 
     @property
-    def ent_ids(self: SpaczzRuler) -> Tuple[Optional[str], ...]:
+    def ent_ids(self: "SpaczzRuler") -> ty.Tuple[ty.Optional[str], ...]:
         """All entity ids present in the match patterns id properties.
 
         Returns:
             The unique string entity ids as a tuple.
 
         Example:
             >>> import spacy
@@ -274,28 +290,27 @@
             >>> nlp = spacy.blank("en")
             >>> ruler = SpaczzRuler(nlp)
             >>> ruler.add_patterns([{"label": "AUTHOR", "pattern": "Kerouac",
                 "type": "fuzzy", "id": "BEAT"}])
             >>> ruler.ent_ids
             ('BEAT',)
         """
-        keys = set(self.fuzzy_patterns.keys())
-        keys.update(self.regex_patterns.keys())
-        keys.update(self.token_patterns.keys())
+        keys = set(self._fuzzy_patterns.keys())
+        keys.update(self._regex_patterns.keys())
+        keys.update(self._token_patterns.keys())
         all_ent_ids = set()
 
         for k in keys:
             if self.ent_id_sep in k:
                 _, ent_id = self._split_label(k)
                 all_ent_ids.add(ent_id)
-        all_ent_ids_tuple = tuple(all_ent_ids)
-        return all_ent_ids_tuple
+        return tuple(all_ent_ids)
 
     @property
-    def labels(self: SpaczzRuler) -> Tuple[str, ...]:
+    def labels(self: "SpaczzRuler") -> ty.Tuple[str, ...]:
         """All labels present in the ruler.
 
         Returns:
             The unique string labels as a tuple.
 
         Example:
             >>> import spacy
@@ -303,28 +318,28 @@
             >>> nlp = spacy.blank("en")
             >>> ruler = SpaczzRuler(nlp)
             >>> ruler.add_patterns([{"label": "AUTHOR", "pattern": "Kerouac",
                 "type": "fuzzy"}])
             >>> ruler.labels
             ('AUTHOR',)
         """
-        keys = set(self.fuzzy_patterns.keys())
-        keys.update(self.regex_patterns.keys())
-        keys.update(self.token_patterns.keys())
+        keys = set(self._fuzzy_patterns.keys())
+        keys.update(self._regex_patterns.keys())
+        keys.update(self._token_patterns.keys())
         all_labels = set()
         for k in keys:
             if self.ent_id_sep in k:
                 label, _ = self._split_label(k)
                 all_labels.add(label)
             else:
                 all_labels.add(k)
-        return tuple(all_labels)
+        return tuple(sorted(all_labels))
 
     @property
-    def patterns(self: SpaczzRuler) -> List[Dict[str, Any]]:
+    def patterns(self: "SpaczzRuler") -> ty.List[RulerPattern]:
         """Get all patterns and kwargs that were added to the ruler.
 
         Returns:
             The original patterns and kwargs, one dictionary for each combination.
 
         Example:
             >>> import spacy
@@ -340,71 +355,79 @@
                     "type": "regex",
                     "kwargs": {"predef": True},
                     },
                     ]
             True
         """
         all_patterns = []
-        for label, fuzzy_patterns in self.fuzzy_patterns.items():
-            for fuzzy_pattern, fuzzy_kwargs in zip(
+        for label, fuzzy_patterns in self._fuzzy_patterns.items():
+            for fuzzy_pattern, fuzzy_kwargs in zip(  # noqa: B905
                 fuzzy_patterns["patterns"], fuzzy_patterns["kwargs"]
             ):
                 ent_label, ent_id = self._split_label(label)
                 p = {"label": ent_label, "pattern": fuzzy_pattern.text, "type": "fuzzy"}
                 if fuzzy_kwargs:
                     p["kwargs"] = fuzzy_kwargs
                 if ent_id:
                     p["id"] = ent_id
                 all_patterns.append(p)
-        for label, regex_patterns in self.regex_patterns.items():
-            for regex_pattern, regex_kwargs in zip(
+        for label, regex_patterns in self._regex_patterns.items():
+            for regex_pattern, regex_kwargs in zip(  # noqa: B905
                 regex_patterns["patterns"], regex_patterns["kwargs"]
             ):
                 ent_label, ent_id = self._split_label(label)
                 p = {"label": ent_label, "pattern": regex_pattern, "type": "regex"}
                 if regex_kwargs:
                     p["kwargs"] = regex_kwargs
                 if ent_id:
                     p["id"] = ent_id
                 all_patterns.append(p)
-        for label, token_patterns in self.token_patterns.items():
+        for label, token_patterns in self._token_patterns.items():
             for token_pattern in token_patterns:
                 ent_label, ent_id = self._split_label(label)
                 p = {"label": ent_label, "pattern": token_pattern, "type": "token"}
                 if ent_id:
                     p["id"] = ent_id
                 all_patterns.append(p)
         return all_patterns
 
     def add_patterns(
-        self: SpaczzRuler,
-        patterns: Iterable[Dict[str, Any]],
+        self: "SpaczzRuler",
+        patterns: ty.List[RulerPattern],
     ) -> None:
         """Add patterns to the ruler.
 
         A pattern must be a spaczz pattern:
         `{label (str), pattern (str or list), type (str),
         optional kwargs (dict[str, Any]), and optional id (str)}`.
 
-        For example, a fuzzy phrase pattern:
-        `{'label': 'ORG', 'pattern': 'Apple',
-        'type': 'fuzzy', 'kwargs': {'min_r2': 90}}`
+        For example, a fuzzy phrase pattern::
 
-        Or, a token pattern:
-        `{'label': 'ORG', 'pattern': [{'TEXT': {'FUZZY': 'Apple'}}], 'type': 'token'}`
+            {
+                'label': 'ORG',
+                'pattern': 'Apple',
+                'kwargs': {'min_r2': 90},
+                'type': 'fuzzy',
+            }
 
-        To utilize regex flags, use inline flags.
+        Or, a token pattern::
 
-        Kwarg details to be updated.
+            {
+                'label': 'ORG',
+                'pattern': [{'TEXT': {'FUZZY': 'Apple'}}],
+                'type': 'token',
+            }
+
+        To utilize regex flags, use inline flags.
 
         Args:
             patterns: The spaczz patterns to add.
 
         Raises:
-            TypeError: If patterns is not an iterable of dictionaries.
+            TypeError: If `patterns` is not a list of dicts.
             ValueError: If one or more patterns do not conform
                 the spaczz pattern structure.
 
         Example:
             >>> import spacy
             >>> from spaczz.pipeline import SpaczzRuler
             >>> nlp = spacy.blank("en")
@@ -455,170 +478,215 @@
                             token_patterns.append(entry)
                         else:
                             warnings.warn(
                                 f"""Spaczz pattern "type" must be "fuzzy", "regex",
                                 or "token", not {entry["type"]}. Skipping this pattern.
                                 """,
                                 PatternTypeWarning,
+                                stacklevel=2,
                             )
                     else:
-                        raise TypeError(
-                            ("Patterns must either be an iterable of dicts.")
-                        )
+                        raise TypeError(("Patterns must be a list of dicts."))
                 except KeyError:
                     raise ValueError(
                         (
                             "One or more patterns do not conform",
                             "to spaczz pattern structure: ",
                             "{label (str), pattern (str or list), type (str),",
                             "optional kwargs (dict[str, Any]),",
                             "and optional id (str)}.",
                         )
                     )
 
             fuzzy_patterns = []
-            for label, pattern, kwargs, ent_id in zip(
+            for flabel, fpattern, fkwargs, fent_id in zip(  # noqa: B905
                 fuzzy_pattern_labels,
-                self.nlp.pipe(fuzzy_pattern_texts),
+                self.nlp.pipe(ty.cast(str, fuzzy_pattern_texts)),
                 fuzzy_pattern_kwargs,
                 fuzzy_pattern_ids,
             ):
                 fuzzy_pattern = {
-                    "label": label,
-                    "pattern": pattern,
-                    "kwargs": kwargs,
+                    "label": flabel,
+                    "pattern": fpattern,
+                    "kwargs": fkwargs,
                     "type": "fuzzy",
                 }
-                if ent_id:
-                    fuzzy_pattern["id"] = ent_id
+                if fent_id:
+                    fuzzy_pattern["id"] = fent_id
                 fuzzy_patterns.append(fuzzy_pattern)
 
             regex_patterns = []
-            for label, pattern, kwargs, ent_id in zip(
+            for rlabel, rpattern, rkwargs, rent_id in zip(  # noqa: B905
                 regex_pattern_labels,
                 regex_pattern_texts,
                 regex_pattern_kwargs,
                 regex_pattern_ids,
             ):
                 regex_pattern = {
-                    "label": label,
-                    "pattern": pattern,
-                    "kwargs": kwargs,
+                    "label": rlabel,
+                    "pattern": rpattern,
+                    "kwargs": rkwargs,
                     "type": "regex",
                 }
-                if ent_id:
-                    regex_pattern["id"] = ent_id
+                if rent_id:
+                    regex_pattern["id"] = rent_id
                 regex_patterns.append(regex_pattern)
 
             self._add_patterns(fuzzy_patterns, regex_patterns, token_patterns)
 
-    def clear(self: SpaczzRuler) -> None:
+    def clear(self: "SpaczzRuler") -> None:
         """Reset all patterns."""
-        self.fuzzy_patterns = nest_defaultdict(list, 2)
-        self.regex_patterns = nest_defaultdict(list, 2)
-        self.token_patterns = defaultdict(list)
+        self._fuzzy_patterns = nest_defaultdict(list)
+        self._regex_patterns = nest_defaultdict(list)
+        self._token_patterns = defaultdict(list)
         self._ent_ids = defaultdict(dict)
+        self.fuzzy_matcher = FuzzyMatcher(
+            self.nlp.vocab, **self.defaults["fuzzy_defaults"]
+        )
+        self.regex_matcher = RegexMatcher(
+            self.nlp.vocab, **self.defaults["regex_defaults"]
+        )
+        self.token_matcher = TokenMatcher(
+            self.nlp.vocab, **self.defaults["token_defaults"]
+        )
 
     def initialize(
-        self: SpaczzRuler,
-        get_examples: Callable[[], Iterable[Example]],
+        self: "SpaczzRuler",
+        get_examples: ty.Callable[[], ty.Iterable[Example]],
         *,
-        nlp: Optional[Language] = None,
-        patterns: Optional[Iterable[Dict[str, Any]]] = None,
+        nlp: ty.Optional[Language] = None,
+        patterns: ty.Optional[ty.Sequence[RulerPattern]] = None,
     ) -> None:
         """Initialize the pipe for training.
 
         Args:
             get_examples: Function that returns a representative sample
                 of gold-standard Example objects.
             nlp: The current nlp object the component is part of.
             patterns: The list of patterns.
         """
         self.clear()
         if patterns:
-            self.add_patterns(patterns)
+            self.add_patterns(patterns)  # type: ignore[arg-type]
 
-    def match(
-        self: SpaczzRuler, doc: Doc
-    ) -> Tuple[
-        List[Tuple[str, int, int]],
-        DefaultDict[str, Dict[Tuple[str, int, int], Any]],
-    ]:
-        """Used in call to find matches in a doc."""
-        fuzzy_matches = []
-        lookup: DefaultDict[str, Dict[Tuple[str, int, int], Any]] = defaultdict(dict)
-        for fuzzy_match in self.fuzzy_matcher(doc):
-            current_ratio = fuzzy_match[3]
-            best_ratio = lookup["ratios"].get(fuzzy_match[:3], 0)
-            if current_ratio > best_ratio:
-                fuzzy_matches.append(fuzzy_match[:3])
-                lookup["ratios"][fuzzy_match[:3]] = current_ratio
-        regex_matches = []
-        for regex_match in self.regex_matcher(doc):
-            current_counts = regex_match[3]
-            best_counts = lookup["counts"].get(regex_match[:3])
-            if not best_counts or sum(current_counts) < sum(best_counts):
-                regex_matches.append(regex_match[:3])
-                lookup["counts"][regex_match[:3]] = current_counts
-        token_matches = []
-        for token_match in self.token_matcher(doc):
-            token_matches.append(token_match[:3])
-            lookup["details"][token_match[:3]] = 1
-        matches = fuzzy_matches + regex_matches + token_matches
-        unique_matches, lookup = self._filter_overlapping_matches(matches, lookup)
-        return unique_matches, lookup
+    def match(self: "SpaczzRuler", doc: Doc) -> ty.List[RulerResult]:
+        """Used in call to find matches in `doc`."""
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="\\[W036")
+            matches: ty.List[ty.Tuple[str, int, int, int, str, SpaczzType]] = (
+                [(*match, "fuzzy") for match in self.fuzzy_matcher(doc)]
+                + [(*match, "regex") for match in self.regex_matcher(doc)]
+                + [(*match, "token") for match in self.token_matcher(doc)]
+            )
+        matches = self._get_final_matches(matches)
+        return sorted(matches, key=lambda x: (x[2] - x[1], -x[1], x[3]), reverse=True)
+
+    def remove(self: "SpaczzRuler", ent_id: str) -> None:
+        """Remove patterns by their `ent_id`."""
+        label_id_pairs = [
+            (label, eid) for (label, eid) in self._ent_ids.values() if eid == ent_id
+        ]
+        if not label_id_pairs:
+            raise ValueError(
+                f"The `ent_id`: '{ent_id}' does not exist within the ruler."  # noqa: B907
+            )
+        created_labels = [
+            self._create_label(label, eid) for (label, eid) in label_id_pairs
+        ]
+        # remove the patterns from self.fuzzy_patterns
+        self._fuzzy_patterns = nest_defaultdict(
+            list,
+            1,
+            {
+                label: val
+                for (label, val) in self._fuzzy_patterns.items()
+                if label not in created_labels
+            },
+        )
+        # remove the patterns from self.regex_patterns
+        self._regex_patterns = nest_defaultdict(
+            list,
+            1,
+            {
+                label: val
+                for (label, val) in self._regex_patterns.items()
+                if label not in created_labels
+            },
+        )
+        # remove the patterns from self.token_pattern
+        self._token_patterns = defaultdict(
+            list,
+            {
+                label: val
+                for (label, val) in self._token_patterns.items()
+                if label not in created_labels
+            },
+        )
+        # remove the patterns from the matchers
+        for label in created_labels:
+            if label in self.fuzzy_matcher:
+                self.fuzzy_matcher.remove(label)
+            elif label in self.regex_matcher:
+                self.regex_matcher.remove(label)
+            else:
+                self.token_matcher.remove(label)
 
-    def score(self: SpaczzRuler, examples: Any, **kwargs: Any) -> Any:
-        """Pipeline scoring for spaCy compatibility."""
+    def score(
+        self: "SpaczzRuler", examples: ty.Iterable[Example], **kwargs: ty.Any
+    ) -> ty.Any:
+        """Pipeline scoring for spaCy >= 3.0, < 3.2 compatibility."""
         validate_examples(examples, "SpaczzRuler.score")
         return get_ner_prf(examples)
 
     def set_annotations(
-        self: SpaczzRuler,
+        self: "SpaczzRuler",
         doc: Doc,
-        matches: List[Tuple[str, int, int]],
-        lookup: DefaultDict[
-            str, Dict[Tuple[str, int, int], Union[int, Tuple[int, int, int]]]
-        ],
+        matches: ty.List[ty.Tuple[str, int, int, int, str, SpaczzType]],
     ) -> None:
         """Modify the document in place."""
         entities = list(doc.ents)
         new_entities = []
-        seen_tokens: Set[int] = set()
-        for match_id, start, end in matches:
+        seen_tokens: ty.Set[int] = set()
+        for match_id, start, end, ratio, pattern, match_type in matches:
             if any(t.ent_type for t in doc[start:end]) and not self.overwrite:
                 continue
             # check for end - 1 here because boundaries are inclusive
             if start not in seen_tokens and end - 1 not in seen_tokens:
                 if match_id in self._ent_ids:
                     label, ent_id = self._ent_ids[match_id]
                     span = Span(doc, start, end, label=label)
                     if ent_id:
                         for token in span:
                             token.ent_id_ = ent_id
                 else:
                     span = Span(doc, start, end, label=match_id)
-                span = self._update_custom_attrs(span, match_id, lookup)
+                span = self._update_custom_attrs(
+                    span,
+                    match_id=match_id,
+                    ratio=ratio,
+                    pattern=pattern,
+                    match_type=match_type,
+                )
                 new_entities.append(span)
                 entities = [
                     e for e in entities if not (e.start < end and e.end > start)
                 ]
                 seen_tokens.update(range(start, end))
-        doc.ents = entities + new_entities
+        doc.ents = tuple(entities + new_entities)  # type: ignore
 
     def from_bytes(
-        self: SpaczzRuler,
+        self: "SpaczzRuler",
         patterns_bytes: bytes,
         *,
-        exclude: Iterable[str] = simple_frozen_list,
-    ) -> SpaczzRuler:
+        exclude: ty.Iterable[str] = SIMPLE_FROZEN_LIST,
+    ) -> "SpaczzRuler":
         """Load the spaczz ruler from a bytestring.
 
         Args:
-            patterns_bytes : The bytestring to load.
+            patterns_bytes: The bytestring to load.
             exclude: For spaCy consistency.
 
         Returns:
             The loaded spaczz ruler.
 
         Example:
             >>> import spacy
@@ -653,15 +721,15 @@
             self.overwrite = cfg.get("overwrite", False)
             self.ent_id_sep = cfg.get("ent_id_sep", DEFAULT_ENT_ID_SEP)
         else:
             self.add_patterns(cfg)
         return self
 
     def to_bytes(
-        self: SpaczzRuler, *, exclude: Iterable[str] = simple_frozen_list
+        self: "SpaczzRuler", *, exclude: ty.Iterable[str] = SIMPLE_FROZEN_LIST
     ) -> bytes:
         """Serialize the spaczz ruler patterns to a bytestring.
 
         Args:
             exclude: For spaCy consistency.
 
         Returns:
@@ -683,31 +751,34 @@
             "ent_id_sep": self.ent_id_sep,
             "patterns": self.patterns,
             "defaults": self.defaults,
         }
         return srsly.msgpack_dumps(serial)
 
     def from_disk(
-        self: SpaczzRuler,
-        path: Union[str, Path],
+        self: "SpaczzRuler",
+        path: ty.Union[str, Path],
         *,
-        exclude: Iterable[str] = simple_frozen_list,
-    ) -> SpaczzRuler:
+        exclude: ty.Iterable[str] = SIMPLE_FROZEN_LIST,
+    ) -> "SpaczzRuler":
         """Load the spaczz ruler from a file.
 
         Expects a file containing newline-delimited JSON (JSONL)
         with one entry per line.
 
         Args:
             path: The JSONL file to load.
             exclude: For spaCy consistency.
 
         Returns:
             The loaded spaczz ruler.
 
+        Raises:
+            ValueError: If `path` does not exist or cannot be accessed.
+
         Example:
             >>> import os
             >>> import tempfile
             >>> import spacy
             >>> from spaczz.pipeline import SpaczzRuler
             >>> nlp = spacy.blank("en")
             >>> ruler = SpaczzRuler(nlp)
@@ -719,18 +790,27 @@
             >>>     new_ruler = new_ruler.from_disk(f"{tmpdir}/ruler")
             >>> "AUTHOR" in new_ruler
             True
         """
         path = ensure_path(path)
         self.clear()
         depr_patterns_path = path.with_suffix(".jsonl")
-        if depr_patterns_path.is_file():
+        if path.suffix == ".jsonl":  # user provides a jsonl
+            if path.is_file():
+                patterns = srsly.read_jsonl(path)
+                self.add_patterns(patterns)
+            else:
+                raise ValueError(
+                    f"Couldn't read SpaczzRuler from '{path}'. "  # noqa: B907
+                    "This file doesn't exist."
+                )
+        elif depr_patterns_path.is_file():
             patterns = srsly.read_jsonl(depr_patterns_path)
             self.add_patterns(patterns)
-        else:
+        elif path.is_dir():
             cfg = {}
             deserializers_patterns = {
                 "patterns": lambda p: self.add_patterns(
                     srsly.read_jsonl(p.with_suffix(".jsonl"))
                 )
             }
             deserializers_cfg = {"cfg": lambda p: cfg.update(srsly.read_json(p))}
@@ -747,21 +827,23 @@
                 )
             if self.defaults.get("token_defaults"):
                 self.token_matcher = TokenMatcher(
                     self.nlp.vocab, **self.defaults["token_defaults"]
                 )
             self.ent_id_sep = cfg.get("ent_id_sep", DEFAULT_ENT_ID_SEP)
             read_from_disk(path, deserializers_patterns, {})
+        else:  # path is not a valid directory or file
+            raise ValueError(f"Could not access f{path}.")
         return self
 
     def to_disk(
-        self: SpaczzRuler,
-        path: Union[str, Path],
+        self: "SpaczzRuler",
+        path: ty.Union[str, Path],
         *,
-        exclude: Iterable[str] = simple_frozen_list,
+        exclude: ty.Iterable[str] = SIMPLE_FROZEN_LIST,
     ) -> None:
         """Save the spaczz ruler patterns to a directory.
 
         The patterns will be saved as newline-delimited JSON (JSONL).
 
         Args:
             path: The JSONL file to save.
@@ -796,67 +878,79 @@
         }
         if path.suffix == ".jsonl":  # user wants to save only JSONL
             srsly.write_jsonl(path, self.patterns)
         else:
             write_to_disk(path, serializers, {})
 
     def _add_patterns(
-        self: SpaczzRuler,
-        fuzzy_patterns: List[Dict[str, Any]],
-        regex_patterns: List[Dict[str, Any]],
-        token_patterns: List[Dict[str, Any]],
+        self: "SpaczzRuler",
+        fuzzy_patterns: ty.List[ty.Dict[str, ty.Any]],
+        regex_patterns: ty.List[ty.Dict[str, ty.Any]],
+        token_patterns: ty.List[ty.Dict[str, ty.Any]],
     ) -> None:
         """Helper function for add_patterns."""
         for entry in fuzzy_patterns + regex_patterns + token_patterns:
             label = entry["label"]
             if "id" in entry:
                 ent_label = label
                 label = self._create_label(label, entry["id"])
                 self._ent_ids[label] = (ent_label, entry["id"])
             pattern = entry["pattern"]
             if isinstance(pattern, Doc):
-                self.fuzzy_patterns[label]["patterns"].append(pattern)
-                self.fuzzy_patterns[label]["kwargs"].append(entry["kwargs"])
+                self._fuzzy_patterns[label]["patterns"].append(pattern)
+                self._fuzzy_patterns[label]["kwargs"].append(entry["kwargs"])
             elif isinstance(pattern, str):
-                self.regex_patterns[label]["patterns"].append(pattern)
-                self.regex_patterns[label]["kwargs"].append(entry["kwargs"])
+                self._regex_patterns[label]["patterns"].append(pattern)
+                self._regex_patterns[label]["kwargs"].append(entry["kwargs"])
             elif isinstance(pattern, list):
-                self.token_patterns[label].append(pattern)
+                self._token_patterns[label].append(pattern)
             else:
                 raise ValueError(
                     (
                         "One or more patterns do not conform",
                         "to spaczz pattern structure:",
                         "{label (str), pattern (str or list), type (str),",
                         "optional kwargs (dict[str, Any]),",
                         "and optional id (str)}.",
                     )
                 )
-        for label, patterns in self.fuzzy_patterns.items():
+        for label, patterns in self._fuzzy_patterns.items():
             self.fuzzy_matcher.add(label, patterns["patterns"], patterns["kwargs"])
-        for label, patterns in self.regex_patterns.items():
+        for label, patterns in self._regex_patterns.items():
             self.regex_matcher.add(label, patterns["patterns"], patterns["kwargs"])
-        for label, _token_patterns in self.token_patterns.items():
-            self.token_matcher.add(label, _token_patterns)
+        for label, token_patterns_ in self._token_patterns.items():
+            self.token_matcher.add(label, token_patterns_)
 
-    def _create_label(self: SpaczzRuler, label: str, ent_id: Union[str, None]) -> str:
+    def _create_label(
+        self: "SpaczzRuler", label: str, ent_id: ty.Union[str, None]
+    ) -> str:
         """Join Entity label with ent_id if the pattern has an id attribute.
 
         Args:
             label: The entity label.
             ent_id: The optional entity id.
 
         Returns:
             The label and ent_id joined with configured ent_id_sep.
         """
         if isinstance(ent_id, str):
-            label = "{}{}{}".format(label, self.ent_id_sep, ent_id)
+            label = f"{label}{self.ent_id_sep}{ent_id}"
         return label
 
-    def _split_label(self: SpaczzRuler, label: str) -> Tuple[str, Union[str, None]]:
+    def _require_patterns(self: "SpaczzRuler") -> None:
+        """Raise a warning if this component has no patterns defined."""
+        if len(self) == 0:
+            warnings.warn(
+                REQUIRE_PATTERNS_WARNING,
+                stacklevel=2,
+            )
+
+    def _split_label(
+        self: "SpaczzRuler", label: str
+    ) -> ty.Tuple[str, ty.Optional[str]]:
         """Split Entity label into ent_label and ent_id if it contains self.ent_id_sep.
 
         Args:
             label: The value of label in a pattern entry
 
         Returns:
             The separated ent_label and optional ent_id.
@@ -865,67 +959,30 @@
             ent_label, ent_id = label.rsplit(self.ent_id_sep, 1)
             return ent_label, ent_id
         else:
             ent_label = label
             return ent_label, None
 
     @staticmethod
-    def _filter_overlapping_matches(
-        matches: List[Tuple[str, int, int]],
-        lookup: DefaultDict[str, Dict[Tuple[str, int, int], Any]],
-    ) -> Tuple[
-        List[Tuple[str, int, int]], DefaultDict[str, Dict[Tuple[str, int, int], Any]]
-    ]:
-        """Prevents multiple match spans from overlapping.
-
-        Expects matches to be pre-sorted by matcher priority,
-        with each matcher's matches being pre-sorted by descending length,
-        then ascending start index, then descending match score
-        If more than one match span includes the same tokens
-        the first of these match spans in matches is kept.
-
-        It also removes non-kept matches from the lookup dict as well.
-
-        Args:
-            matches: List of match span tuples
-                (match_id, start_index, end_index).
-            lookup: Match ratio, count and detail values in
-                a `defaultdict(dict)`.
-
-        Returns:
-            The filtered list of match span tuples.
-        """
-        filtered_matches: List[Tuple[str, int, int]] = []
+    def _get_final_matches(
+        matches: ty.List[RulerResult],
+    ) -> ty.List[RulerResult]:
+        final_matches = []
+        lookup: ty.Dict[ty.Tuple[str, int, int], int] = dict()
         for match in matches:
-            if not set(range(match[1], match[2])).intersection(
-                chain(*[set(range(n[1], n[2])) for n in filtered_matches])
-            ):
-                filtered_matches.append(match)
-                if match in lookup["ratios"]:
-                    _ = lookup["counts"].pop(match, None)
-                    _ = lookup["details"].pop(match, None)
-                elif match in lookup["counts"]:
-                    _ = lookup["details"].pop(match, None)
-        return filtered_matches, lookup
+            ratio = lookup.get(match[:3], 0)
+            if match[3] > ratio:
+                final_matches.append(match)
+                lookup[match[:3]] = ratio
+        return final_matches
 
     @staticmethod
     def _update_custom_attrs(
-        span: Span,
-        match_id: str,
-        lookup: DefaultDict[str, Dict[Tuple[str, int, int], Any]],
+        span: Span, match_id: str, ratio: int, pattern: str, match_type: SpaczzType
     ) -> Span:
         """Update custom attributes for matches."""
-        ratio = lookup["ratios"].get((match_id, span.start, span.end))
-        counts = lookup["counts"].get((match_id, span.start, span.end))
-        details = lookup["details"].get((match_id, span.start, span.end))
         for token in span:
             token._.spaczz_token = True
-            if ratio:
-                token._.spaczz_ratio = ratio
-                token._.spaczz_type = "fuzzy"
-            elif counts:
-                token._.spaczz_counts = counts
-                token._.spaczz_type = "regex"
-            elif details:
-                token._.spaczz_details = details
-                token._.spaczz_type = "token"
+            token._.spaczz_ratio = ratio
+            token._.spaczz_pattern = pattern
+            token._.spaczz_type = match_type
         return span
```

### Comparing `spaczz-0.5.4/src/spaczz/search/regexsearcher.py` & `spaczz-0.6.0a0/src/spaczz/_search/regexsearcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,144 @@
-"""Module for RegexSearcher: multi-token regex matching in spaCy `Doc` objects."""
-from __future__ import annotations
+"""`RegexSearcher` searches for phrase-based regex matches in spaCy `Doc` objects."""
+import typing as ty
 
-from typing import List, Tuple, Union
+try:
+    from typing import Match
+except ImportError:  # pragma: no cover
+    from regex import Match  # type: ignore
 
-from spacy.tokens import Doc, Span
+from spacy.tokens import Doc
+from spacy.tokens import Span
 from spacy.vocab import Vocab
 
-from ..process import map_chars_to_tokens
-from ..regex import RegexConfig
+from .searchutil import filter_overlapping_matches
+from .searchutil import normalize_fuzzy_regex_counts
+from .searchutil import parse_regex
+from ..customtypes import SearchResult
 
 
 class RegexSearcher:
-    """Class for multi-token regex matching in spacy `Doc` objects.
-
-    Regex matching is done on the character level and then
-    mapped back to tokens.
-
-    Attributes:
-        vocab (Vocab): The shared vocabulary.
-            Included for consistency and potential future-state.
-        _config (RegexConfig): The regex config used with the
-            regex searcher.
-    """
+    """Class for phrase-based regex match searching in spaCy `Doc` objects."""
 
     def __init__(
-        self: RegexSearcher, vocab: Vocab, config: Union[str, RegexConfig] = "default"
+        self: "RegexSearcher",
+        vocab: Vocab,
     ) -> None:
-        """Initializes the regex searcher with the given config.
-
-        Args:
-            vocab: A spaCy `Vocab` object.
-                Purely for consistency between spaCy
-                and spaczz matcher APIs for now.
-                spaczz matchers are mostly pure-Python
-                currently and do not share vocabulary
-                with spaCy pipelines.
-            config: Provides the class with predefind regex patterns.
-                Uses the default config if `"default"`, an empty config if `"empty"`,
-                or a custom config by passing a `RegexConfig` object.
-                Default is `"default"`.
-
-        Raises:
-            TypeError: If config is not a `RegexConfig` object.
-        """
+        """Initializes the searcher."""
         self.vocab = vocab
-        if config == "default":
-            self._config = RegexConfig(empty=False)
-        elif config == "empty":
-            self._config = RegexConfig(empty=True)
-        else:
-            if isinstance(config, RegexConfig):
-                self._config = config
-            else:
-                raise TypeError(
-                    (
-                        "config must be one of the strings 'default' or 'empty',",
-                        "or a RegexConfig object not,",
-                        f"config of type: {type(config)}.",
-                    )
-                )
 
     def match(
-        self: RegexSearcher,
+        self: "RegexSearcher",
         doc: Doc,
         query: str,
+        *,
+        ignore_case: bool = True,
+        min_r: int = 75,
         partial: bool = True,
         predef: bool = False,
-    ) -> List[Tuple[int, int, Tuple[int, int, int]]]:
-        """Returns all the regex matches within a doc.
+        fuzzy_weights: str = "indel",
+    ) -> ty.List[SearchResult]:
+        """Performs regex matching on a `Doc` object.
 
         Matches on the character level and then maps matches back
         to tokens. If a character cannot be mapped back to a token it means
-        it is a space tokens are split on, which happens when regex matches
-        produce leading or trailing whitespace. Confirm your regex pattern
+        the character is a space tokens are split on, which happens when regex
+        matches produce leading or trailing whitespace. Confirm your regex pattern
         will not do this to avoid this issue.
 
         To utilize regex flags, use inline flags.
 
         Args:
-            doc: `Doc` object to search over.
-            query: A string to be compiled to regex,
-                or the key name of a predefined regex pattern.
-            partial: Whether partial matches should be extended
-                to existing span boundaries in doc or not, i.e.
-                the regex only matches part of a token or span.
+            doc: `Doc` to search for matches.
+            query: A string to be compiled to regex, or the key name of a predefined
+                regex pattern.
+            ignore_case: Whether to lower-case text before matching.
                 Default is `True`.
+            min_r: Minimum match ratio required for fuzzy regex matching.
+                Default is `75`.
+            fuzzy_weights: Name of weighting method for regex insertion, deletion, and
+                substituion counts. Default is `"indel"`.
+            partial: Whether partial matches should be extended
+                to existing span boundaries in doc or not, e.x. the regex only matches
+                part of a `Token` or `Span`. Default is `True`.
             predef: Whether regex should be interpreted as a key to
                 a predefined regex pattern or not. Default is `False`.
-                The included regexes are:
-                `"dates"`
-                `"times"`
-                `"phones"`
-                `"phones_with_exts"`
-                `"links"`
-                `"emails"`
-                `"ips"`
-                `"ipv6s"`
-                `"prices"`
-                `"hex_colors"`
-                `"credit_cards"`
-                `"btc_addresses"`
-                `"street_addresses"`
-                `"zip_codes"`
-                `"po_boxes"`
-                `"ssn_number"`.
 
         Returns:
-            A list of span start index, end index, fuzzy change count tuples.
-
-        Raises:
-            TypeError: If `doc` is not a `Doc`
-            TypeError: If `query` is not a `str`.
+            List of match tuples each containing a start index, end index,
+            and match ratio.
 
         Example:
             >>> import spacy
-            >>> from spaczz.search import RegexSearcher
+            >>> from spaczz._search import RegexSearcher
             >>> nlp = spacy.blank("en")
             >>> searcher = RegexSearcher(nlp.vocab)
             >>> doc = nlp("My phone number is (555) 555-5555.")
             >>> searcher.match(doc, "phones", predef=True)
-            [(4, 10, (0, 0, 0))]
+            [(4, 10, 100)]
         """
-        if not isinstance(doc, Doc):
-            raise TypeError("doc must be a Doc object.")
-        if isinstance(query, str):
-            compiled_regex = self._config.parse_regex(query, predef)
-        else:
-            raise TypeError(f"query must be a str, not {type(query)}.")
-        matches = []
-        chars_to_tokens = map_chars_to_tokens(doc)
-        for match in compiled_regex.finditer(doc.text):
-            start, end = match.span()
-            counts = match.fuzzy_counts
-            span = doc.char_span(start, end)
-            if span:
-                matches.append((span, counts))
-            else:
-                if partial:
-                    start_token = chars_to_tokens.get(start)
-                    end_token = chars_to_tokens.get(end - 1)
-                    if start_token and end_token:
-                        span = Span(doc, start_token, end_token + 1)
-                        matches.append((span, counts))
-        if matches:
-            return [(match[0].start, match[0].end, match[1]) for match in matches]
-        else:
-            return []
+        compiled_regex = parse_regex(query, predef=predef)
+        char_to_token_map = self._map_chars_to_tokens(doc)
+
+        regex_matches = [
+            self._spans_from_regex(
+                doc, match=match, partial=partial, char_to_token_map=char_to_token_map
+            )
+            for match in compiled_regex.finditer(
+                doc.text.lower() if ignore_case else doc.text
+            )
+        ]
+
+        formatted_matches = [
+            (
+                regex_match[0].start,
+                regex_match[0].end,
+                normalize_fuzzy_regex_counts(
+                    regex_match[0].text,
+                    fuzzy_counts=regex_match[1],
+                    fuzzy_weights=fuzzy_weights,
+                ),
+            )
+            for regex_match in regex_matches
+            if regex_match
+        ]
+
+        return filter_overlapping_matches(
+            sorted(
+                [
+                    formatted_match
+                    for formatted_match in formatted_matches
+                    if formatted_match[2] >= min_r
+                ],
+                key=lambda x: (-x[2], x[0]),
+            )
+        )
+
+    @staticmethod
+    def _map_chars_to_tokens(doc: Doc) -> ty.Dict[int, int]:
+        """Maps characters to tokens."""
+        chars_to_tokens = {}
+        for token in doc:
+            for i in range(token.idx, token.idx + len(token.text)):
+                chars_to_tokens[i] = token.i
+        return chars_to_tokens
+
+    @staticmethod
+    def _spans_from_regex(
+        doc: Doc,
+        match: Match[str],
+        partial: bool,
+        char_to_token_map: ty.Dict[int, int],
+    ) -> ty.Optional[ty.Tuple[Span, ty.Tuple[int, int, int]]]:
+        """Creates `Span` objects from regex matches."""
+        start, end = match.span()
+        counts = getattr(match, "fuzzy_counts", (0, 0, 0))
+        span = doc.char_span(start, end)
+        if span:
+            return (span, counts)
+        if partial:
+            start_token = char_to_token_map.get(start)
+            end_token = char_to_token_map.get(end - 1)
+            if start_token and end_token:
+                span = Span(doc, start_token, end_token + 1)
+                return (span, counts)
+        return None
```

### Comparing `spaczz-0.5.4/src/spaczz/search/tokensearcher.py` & `spaczz-0.6.0a0/src/spaczz/_search/tokensearcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,246 +1,232 @@
 """Module for TokenSearcher: flexible token searching in spaCy `Doc` objects."""
-from __future__ import annotations
-
-from typing import Any, Dict, List, Optional, Tuple, Union
+import itertools
+import typing as ty
 
 import regex
-from spacy.tokens import Doc, Token
+from spacy.tokens import Doc
+from spacy.tokens import Token
 from spacy.vocab import Vocab
 
-from ..process import FuzzyFuncs
-from ..util import n_wise
+from .searchutil import normalize_fuzzy_regex_counts
+from .searchutil import parse_regex
+from ..registry import get_fuzzy_func
 
 
 class TokenSearcher:
-    """Class for flexbile token searching in spaCy `Doc` objects.
-
-    Uses individual (and extended) spaCy token matching patterns to find
-    match candidates. Candidates are used to generate new patterns to add
-    to a spaCy `Matcher`.
-
-    "FUZZY" and "FREGEX" are the two additional spaCy token pattern options.
-
-    For example:
-        {"TEXT": {"FREGEX": "(database){e<=1}"}},
-        {"LOWER": {"FUZZY": "access", "MIN_R": 85, "FUZZY_FUNC": "quick_lev"}}
-
-    Make sure to use uppercase dictionary keys in patterns.
-
-    Attributes:
-        vocab (Vocab): The shared vocabulary.
-            Included for consistency and potential future-state.
-        _fuzzy_funcs (FuzzyFuncs):
-            Container class housing fuzzy matching functions.
-            Functions are accessible via the classes `get()` method
-            by their given key name. The following rapidfuzz matching
-            functions with default settings are available:
-            "simple" = `ratio`
-            "quick" = `QRatio`
-            "quick_lev" = `quick_lev_ratio`
-    """
+    """Class for token-based fuzzy match searching in spaCy `Doc` objects."""
 
-    def __init__(self: TokenSearcher, vocab: Vocab) -> None:
-        """Initializes a token searcher.
-
-        Args:
-            vocab: A spaCy `Vocab` object.
-                Purely for consistency between spaCy
-                and spaczz matcher APIs for now.
-                spaczz matchers are mostly pure-Python
-                currently and do not share vocabulary
-                with spaCy pipelines.
-        """
+    def __init__(self: "TokenSearcher", vocab: Vocab) -> None:
+        """Initializes the searcher."""
         self.vocab = vocab
-        self._fuzzy_funcs: FuzzyFuncs = FuzzyFuncs(match_type="token")
-
-    def fuzzy_compare(
-        self: TokenSearcher,
-        a: str,
-        b: str,
-        ignore_case: bool = True,
-        fuzzy_func: str = "simple",
-    ) -> int:
-        """Peforms fuzzy matching between two strings.
-
-        Applies the given fuzzy matching algorithm (fuzzy_func)
-        to two strings and returns the resulting fuzzy ratio.
-
-        Args:
-            a: First string for comparison.
-            b: Second string for comparison.
-            ignore_case: Whether to lower-case a and b
-                before comparison or not. Default is `True`.
-            fuzzy_func: Key name of fuzzy matching function to use.
-                The following rapidfuzz matching functions with default
-                settings are available:
-                "simple" = `ratio`
-                "quick" = `QRatio`
-                Default is `"simple"`.
-
-        Returns:
-            The fuzzy ratio between a and b.
-
-        Example:
-            >>> import spacy
-            >>> from spaczz.search import TokenSearcher
-            >>> nlp = spacy.blank("en")
-            >>> searcher = TokenSearcher(nlp.vocab)
-            >>> searcher.fuzzy_compare("spaczz", "spacy")
-            73
-        """
-        if ignore_case:
-            a = a.lower()
-            b = b.lower()
-        return round(self._fuzzy_funcs.get(fuzzy_func)(a, b))
 
     def match(
-        self: TokenSearcher,
+        self: "TokenSearcher",
         doc: Doc,
-        pattern: List[Dict[str, Any]],
+        pattern: ty.List[ty.Dict[str, ty.Any]],
         min_r: int = 75,
-        fuzzy_func: str = "simple",
-    ) -> List[List[Optional[Tuple[str, str]]]]:
+    ) -> ty.List[ty.List[ty.Tuple[str, str, int]]]:
         """Finds potential token pattern matches in a `Doc` object.
 
         Make sure to use uppercase dictionary keys in patterns.
 
         Args:
-            doc: `Doc` object to search over.
+            doc: `Doc` object to search for matches.
             pattern: Individual spaCy token pattern.
             min_r: Minimum match ratio required for fuzzy matching.
-                Can be overwritten with token pattern options.
+                Can be overwritten with pattern-level match settings.
                 Default is `75`.
-            fuzzy_func: Fuzzy matching function to use.
-                Can be overwritten with token pattern options.
-                Default is `simple`.
 
         Returns:
             A list of lists with each inner list representing a potential match.
-            The inner lists will be populated with key, value tuples of token matches
-            and `None` for placeholder tokens representing non-fuzzy tokens.
-
-        Raises:
-            TypeError: doc must be a `Doc` object.
-            TypeError: pattern must be a `Sequence`.
-            ValueError: pattern cannot have zero tokens.
+            The inner lists will be populated with key, value, match ratio tuples for
+            matched fuzzy token patterns. Non-fuzzy token patterns will have an empty
+            string key and value, and a match ratio of `100`.
 
         Example:
             >>> import spacy
-            >>> from spaczz.search import TokenSearcher
+            >>> from spaczz._search import TokenSearcher
             >>> nlp = spacy.blank("en")
             >>> searcher = TokenSearcher(nlp)
             >>> doc = nlp("I was prescribed zithramax and advar")
             >>> pattern = [
                 {"TEXT": {"FUZZY": "zithromax"}},
                 {"POS": "CCONJ"},
                 {"TEXT": {"FREGEX": "(advair){e<=1}"}}
                 ]
             >>> searcher.match(doc, pattern)
-            [[('TEXT', 'zithramax'), None, ('TEXT', 'advar')]]
+            [[('TEXT', 'zithramax', 89), ('', '', 100), ('TEXT', 'advar', 91)]]
         """
-        if not isinstance(doc, Doc):
-            raise TypeError("doc must be a Doc object.")
-        if not isinstance(pattern, list):
-            raise TypeError(
-                "pattern must be a list",
-                "Make sure pattern is wrapped in a list.",
-            )
-        if len(pattern) == 0:
-            raise ValueError("pattern cannot have zero tokens.")
         matches = []
-        for seq in n_wise(doc, len(pattern)):
-            seq_matches = self._iter_pattern(seq, pattern, min_r, fuzzy_func)
-            if seq_matches:
-                matches.append(seq_matches)
-        if matches:
-            filtered_matches = [
-                i for n, i in enumerate(matches) if i not in matches[:n]
-            ]
-            return filtered_matches
-        else:
-            return matches
+        matches = [
+            self._iter_pattern(seq, pattern, min_r=min_r)
+            for seq in self._n_wise(doc, len(pattern))
+        ]
+        return [
+            match
+            for i, match in enumerate(matches)
+            if match and match not in matches[:i]
+        ]
 
     @staticmethod
-    def regex_compare(text: str, pattern: str, ignore_case: bool = False) -> bool:
+    def fuzzy_compare(
+        s1: str,
+        s2: str,
+        *,
+        ignore_case: bool = True,
+        min_r: int = 0,
+        fuzzy_func: str = "simple",
+    ) -> int:
+        """Peforms fuzzy matching between two strings.
+
+        Applies the given fuzzy matching algorithm (`fuzzy_func`)
+        to two strings and returns the resulting fuzzy ratio.
+
+        Args:
+            s1: First string for comparison.
+            s2: Second string for comparison.
+            ignore_case: Whether to lower-case `s1` and `s2`
+                before comparison or not. Default is `True`.
+            min_r: Minimum ratio needed to match as a value between `0` and `100`.
+                For ratio < min_r, `0` is returned instead.
+                Default is `0`, which deactivates this behaviour.
+            fuzzy_func: Key name of fuzzy matching function to use.
+
+        Returns:
+            The fuzzy ratio between `s1` and `s2`.
+
+        Example:
+            >>> import spacy
+            >>> from spaczz._search import TokenSearcher
+            >>> nlp = spacy.blank("en")
+            >>> searcher = TokenSearcher(nlp.vocab)
+            >>> searcher.fuzzy_compare("spaczz", "spacy")
+            73
+        """
+        if ignore_case:
+            s1 = s1.lower()
+            s2 = s2.lower()
+
+        return round(get_fuzzy_func(fuzzy_func)(s1, s2, score_cutoff=min_r))
+
+    @staticmethod
+    def regex_compare(
+        text: str,
+        pattern: str,
+        *,
+        ignore_case: bool = False,
+        min_r: int = 0,
+        fuzzy_weights: str = "indel",
+        predef: bool = False,
+    ) -> int:
         """Performs fuzzy-regex supporting regex matching between two strings.
 
         Args:
             text: The string to match against.
             pattern: The regex pattern string.
-            ignore_case: Whether to lower-case text
-                before comparison or not. Default is `False`.
+            ignore_case: Whether to lower-case text before matching.
+                Default is `True`.
+            min_r: Minimum match ratio required for fuzzy regex matching.
+                Default is `75`.
+            fuzzy_weights: Name of weighting method for regex insertion, deletion, and
+                substituion counts.
+            predef: Whether regex should be interpreted as a key to
+                a predefined regex pattern or not. Default is `False`.
 
         Returns:
-            `True` if match, `False` if not.
+            The fuzzy ratio of the pattern to the text based on insertions,
+            substitutions, and deletions.
 
         Example:
             >>> import spacy
-            >>> from spaczz.search import TokenSearcher
+            >>> from spaczz._search import TokenSearcher
             >>> nlp = spacy.blank("en")
             >>> searcher = TokenSearcher(nlp)
             >>> searcher.regex_compare("sequel", "(sql){i<=3}")
-            True
+            67
         """
+        pattern_ = parse_regex(pattern, predef=predef)
         if ignore_case:
             text = text.lower()
-        if regex.match(pattern, text):
-            return True
-        else:
-            return False
+        match = regex.match(pattern_, text)
+        if match:
+            r = normalize_fuzzy_regex_counts(
+                match.group(0),
+                fuzzy_counts=getattr(match, "fuzzy_counts", (0, 0, 0)),
+                fuzzy_weights=fuzzy_weights,
+            )
+            if r >= min_r:
+                return r
+        return 0
 
     def _iter_pattern(
-        self: TokenSearcher,
-        seq: Tuple[Token, ...],
-        pattern: List[Dict[str, Any]],
+        self: "TokenSearcher",
+        seq: ty.Tuple[Token, ...],
+        pattern: ty.List[ty.Dict[str, ty.Any]],
         min_r: int,
-        fuzzy_func: str,
-    ) -> List[Optional[Tuple[str, str]]]:
+    ) -> ty.List[ty.Tuple[str, str, int]]:
         """Evaluates each token in a pattern against a doc token sequence."""
-        seq_matches: List[Optional[Tuple[str, str]]] = []
+        seq_matches: ty.List[ty.Tuple[str, str, int]] = []
         for i, token in enumerate(pattern):
             pattern_dict, case, case_bool = self._parse_case(token)
             if isinstance(pattern_dict, dict):
                 pattern_text, pattern_type = self._parse_type(pattern_dict)
                 if pattern_text and pattern_type == "FUZZY":
-                    if (
-                        self.fuzzy_compare(
-                            seq[i].text,
-                            pattern_text,
-                            case_bool,
-                            pattern_dict.get("FUZZY_FUNC", fuzzy_func),
-                        )
-                        >= pattern_dict.get("MIN_R", min_r)
-                    ):
-                        seq_matches.append((case, seq[i].text))
+                    r = self.fuzzy_compare(
+                        seq[i].text,
+                        pattern_text,
+                        ignore_case=case_bool,
+                        min_r=pattern_dict.get("MIN_R", min_r),
+                        fuzzy_func=pattern_dict.get("FUZZY_FUNC", "simple"),
+                    )
+                    if r:
+                        seq_matches.append((case, seq[i].text, r))
                     else:
                         return []
                 elif pattern_text and pattern_type == "FREGEX":
-                    if self.regex_compare(seq[i].text, pattern_text, case_bool):
-                        seq_matches.append((case, seq[i].text))
+                    r = self.regex_compare(
+                        seq[i].text,
+                        pattern_text,
+                        predef=pattern_dict.get("PREDEF", False),
+                        ignore_case=case_bool,
+                        min_r=pattern_dict.get("MIN_R", min_r),
+                        fuzzy_weights=pattern_dict.get("FUZZY_WEIGHTS", "indel"),
+                    )
+                    if r:
+                        seq_matches.append((case, seq[i].text, r))
                     else:
                         return []
                 else:
-                    seq_matches.append(None)
+                    seq_matches.append(("", "", 100))
             else:
-                seq_matches.append(None)
+                seq_matches.append(("", "", 100))
         return seq_matches
 
     @staticmethod
-    def _parse_case(token: Dict[str, Any]) -> Tuple[Union[str, Dict, None], str, bool]:
+    def _parse_case(
+        token: ty.Dict[str, ty.Any]
+    ) -> ty.Tuple[ty.Union[str, ty.Dict[ty.Any, ty.Any], None], str, bool]:
         """Parses the case of a token pattern."""
-        if token.get("TEXT"):
-            return token.get("TEXT"), "TEXT", False
-        else:
-            return token.get("LOWER"), "LOWER", True
+        text = token.get("TEXT")
+        if text:
+            return text, "TEXT", False
+        return token.get("LOWER"), "LOWER", True
 
     @staticmethod
-    def _parse_type(pattern_dict: Dict[str, Any]) -> Tuple[str, str]:
+    def _parse_type(pattern_dict: ty.Dict[str, ty.Any]) -> ty.Tuple[str, str]:
         """Parses the type of a token pattern."""
         fuzzy_text = pattern_dict.get("FUZZY")
         regex_text = pattern_dict.get("FREGEX")
-        if isinstance(fuzzy_text, str):
+        if fuzzy_text:
             return fuzzy_text, "FUZZY"
-        elif isinstance(regex_text, str):
+        elif regex_text:
             return regex_text, "FREGEX"
-        else:
-            return "", ""
+        return "", ""
+
+    @staticmethod
+    def _n_wise(iterable: ty.Iterable[ty.Any], n: int) -> ty.Iterator[ty.Any]:
+        """Iterates over an iterable in slices of length n by one step at a time."""
+        iterables = itertools.tee(iterable, n)
+        for i in range(len(iterables)):
+            for _ in range(i):
+                next(iterables[i], None)
+        return zip(*iterables)  # noqa B905
```

### Comparing `spaczz-0.5.4/setup.py` & `spaczz-0.6.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,2402 +1,2338 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 7370 6163 7a7a 272c 2027 7370 6163  ['spaczz', 'spac
-00000070: 7a7a 2e6d 6174 6368 6572 272c 2027 7370  zz.matcher', 'sp
-00000080: 6163 7a7a 2e70 6970 656c 696e 6527 2c20  aczz.pipeline', 
-00000090: 2773 7061 637a 7a2e 7265 6765 7827 2c20  'spaczz.regex', 
-000000a0: 2773 7061 637a 7a2e 7365 6172 6368 275d  'spaczz.search']
-000000b0: 0a0a 7061 636b 6167 655f 6461 7461 203d  ..package_data =
-000000c0: 205c 0a7b 2727 3a20 5b27 2a27 5d7d 0a0a   \.{'': ['*']}..
-000000d0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000000e0: 203d 205c 0a5b 2772 6170 6964 6675 7a7a   = \.['rapidfuzz
-000000f0: 3e3d 312c 3c32 272c 2027 7265 6765 783e  >=1,<2', 'regex>
-00000100: 3d32 3032 302e 362e 3827 2c20 2773 7061  =2020.6.8', 'spa
-00000110: 6379 3e3d 322e 322e 302c 3c34 2e30 2e30  cy>=2.2.0,<4.0.0
-00000120: 275d 0a0a 6578 7472 6173 5f72 6571 7569  ']..extras_requi
-00000130: 7265 203d 205c 0a7b 273a 7079 7468 6f6e  re = \.{':python
-00000140: 5f76 6572 7369 6f6e 203c 2022 332e 3822  _version < "3.8"
-00000150: 273a 205b 2769 6d70 6f72 746c 6962 5f6d  ': ['importlib_m
-00000160: 6574 6164 6174 613e 3d31 2e30 2e30 275d  etadata>=1.0.0']
-00000170: 7d0a 0a65 6e74 7279 5f70 6f69 6e74 7320  }..entry_points 
-00000180: 3d20 5c0a 7b27 7370 6163 795f 6661 6374  = \.{'spacy_fact
-00000190: 6f72 6965 7327 3a20 5b27 7370 6163 7a7a  ories': ['spaczz
-000001a0: 5f72 756c 6572 203d 2073 7061 637a 7a2e  _ruler = spaczz.
-000001b0: 7069 7065 6c69 6e65 3a53 7061 637a 7a52  pipeline:SpaczzR
-000001c0: 756c 6572 275d 7d0a 0a73 6574 7570 5f6b  uler']}..setup_k
-000001d0: 7761 7267 7320 3d20 7b0a 2020 2020 276e  wargs = {.    'n
-000001e0: 616d 6527 3a20 2773 7061 637a 7a27 2c0a  ame': 'spaczz',.
-000001f0: 2020 2020 2776 6572 7369 6f6e 273a 2027      'version': '
-00000200: 302e 352e 3427 2c0a 2020 2020 2764 6573  0.5.4',.    'des
-00000210: 6372 6970 7469 6f6e 273a 2027 4164 6473  cription': 'Adds
-00000220: 2066 757a 7a79 206d 6174 6368 696e 6720   fuzzy matching 
-00000230: 616e 6420 6164 6469 7469 6f6e 616c 2072  and additional r
-00000240: 6567 6578 206d 6174 6368 696e 6720 7375  egex matching su
-00000250: 7070 6f72 7420 746f 2073 7061 4379 2e27  pport to spaCy.'
-00000260: 2c0a 2020 2020 276c 6f6e 675f 6465 7363  ,.    'long_desc
-00000270: 7269 7074 696f 6e27 3a20 275b 215b 5465  ription': '[![Te
-00000280: 7374 735d 2868 7474 7073 3a2f 2f67 6974  sts](https://git
-00000290: 6875 622e 636f 6d2f 6761 6e64 6572 7365  hub.com/ganderse
-000002a0: 6e31 3031 2f73 7061 637a 7a2f 776f 726b  n101/spaczz/work
-000002b0: 666c 6f77 732f 5465 7374 732f 6261 6467  flows/Tests/badg
-000002c0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-000002d0: 6769 7468 7562 2e63 6f6d 2f67 616e 6465  github.com/gande
-000002e0: 7273 656e 3130 312f 7370 6163 7a7a 2f61  rsen101/spaczz/a
-000002f0: 6374 696f 6e73 3f77 6f72 6b66 6c6f 773d  ctions?workflow=
-00000300: 5465 7374 7329 5c6e 5b21 5b43 6f64 6563  Tests)\n[![Codec
-00000310: 6f76 5d28 6874 7470 733a 2f2f 636f 6465  ov](https://code
-00000320: 636f 762e 696f 2f67 682f 6761 6e64 6572  cov.io/gh/gander
-00000330: 7365 6e31 3031 2f73 7061 637a 7a2f 6272  sen101/spaczz/br
-00000340: 616e 6368 2f6d 6173 7465 722f 6772 6170  anch/master/grap
-00000350: 682f 6261 6467 652e 7376 6729 5d28 6874  h/badge.svg)](ht
-00000360: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000370: 2f67 682f 6761 6e64 6572 7365 6e31 3031  /gh/gandersen101
-00000380: 2f73 7061 637a 7a29 5c6e 5b21 5b50 7950  /spaczz)\n[![PyP
-00000390: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-000003a0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-000003b0: 2f73 7061 637a 7a2e 7376 6729 5d28 6874  /spaczz.svg)](ht
-000003c0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-000003d0: 726f 6a65 6374 2f73 7061 637a 7a2f 295c  roject/spaczz/)\
-000003e0: 6e5b 215b 5265 6164 2074 6865 2044 6f63  n[![Read the Doc
-000003f0: 735d 2868 7474 7073 3a2f 2f72 6561 6474  s](https://readt
-00000400: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
-00000410: 6374 732f 7370 6163 7a7a 2f62 6164 6765  cts/spaczz/badge
-00000420: 2f29 5d28 6874 7470 733a 2f2f 7370 6163  /)](https://spac
-00000430: 7a7a 2e72 6561 6474 6865 646f 6373 2e69  zz.readthedocs.i
-00000440: 6f2f 295c 6e5c 6e23 2073 7061 637a 7a3a  o/)\n\n# spaczz:
-00000450: 2046 757a 7a79 206d 6174 6368 696e 6720   Fuzzy matching 
-00000460: 616e 6420 6d6f 7265 2066 6f72 2073 7061  and more for spa
-00000470: 4379 5c6e 5c6e 5370 6163 7a7a 2070 726f  Cy\n\nSpaczz pro
-00000480: 7669 6465 7320 6675 7a7a 7920 6d61 7463  vides fuzzy matc
-00000490: 6869 6e67 2061 6e64 2061 6464 6974 696f  hing and additio
-000004a0: 6e61 6c20 7265 6765 7820 6d61 7463 6869  nal regex matchi
-000004b0: 6e67 2066 756e 6374 696f 6e61 6c69 7479  ng functionality
-000004c0: 2066 6f72 205b 7370 6143 795d 2868 7474   for [spaCy](htt
-000004d0: 7073 3a2f 2f73 7061 6379 2e69 6f2f 292e  ps://spacy.io/).
-000004e0: 5c6e 5370 6163 7a7a 5c27 7320 636f 6d70  \nSpaczz\'s comp
-000004f0: 6f6e 656e 7473 2068 6176 6520 7369 6d69  onents have simi
-00000500: 6c61 7220 4150 4973 2074 6f20 7468 6569  lar APIs to thei
-00000510: 7220 7370 6143 7920 636f 756e 7465 7270  r spaCy counterp
-00000520: 6172 7473 2061 6e64 2073 7061 637a 7a20  arts and spaczz 
-00000530: 7069 7065 6c69 6e65 2063 6f6d 706f 6e65  pipeline compone
-00000540: 6e74 7320 6361 6e20 696e 7465 6772 6174  nts can integrat
-00000550: 6520 696e 746f 2073 7061 4379 2070 6970  e into spaCy pip
-00000560: 656c 696e 6573 2077 6865 7265 2074 6865  elines where the
-00000570: 7920 6361 6e20 6265 2073 6176 6564 2f6c  y can be saved/l
-00000580: 6f61 6465 6420 6173 206d 6f64 656c 732e  oaded as models.
-00000590: 5c6e 5c6e 4675 7a7a 7920 6d61 7463 6869  \n\nFuzzy matchi
-000005a0: 6e67 2069 7320 6375 7272 656e 746c 7920  ng is currently 
-000005b0: 7065 7266 6f72 6d65 6420 7769 7468 206d  performed with m
-000005c0: 6174 6368 6572 7320 6672 6f6d 205b 5261  atchers from [Ra
-000005d0: 7069 6446 757a 7a5d 2868 7474 7073 3a2f  pidFuzz](https:/
-000005e0: 2f67 6974 6875 622e 636f 6d2f 6d61 7862  /github.com/maxb
-000005f0: 6163 686d 616e 6e2f 7261 7069 6466 757a  achmann/rapidfuz
-00000600: 7a29 5c27 7320 6675 7a7a 206d 6f64 756c  z)\'s fuzz modul
-00000610: 6520 616e 6420 7265 6765 7820 6d61 7463  e and regex matc
-00000620: 6869 6e67 2063 7572 7265 6e74 6c79 2072  hing currently r
-00000630: 656c 6965 7320 6f6e 2074 6865 205b 7265  elies on the [re
-00000640: 6765 785d 2868 7474 7073 3a2f 2f70 7970  gex](https://pyp
-00000650: 692e 6f72 672f 7072 6f6a 6563 742f 7265  i.org/project/re
-00000660: 6765 782f 2920 6c69 6272 6172 792e 2053  gex/) library. S
-00000670: 7061 637a 7a20 6365 7274 6169 6e6c 7920  paczz certainly 
-00000680: 7461 6b65 7320 6164 6469 7469 6f6e 616c  takes additional
-00000690: 2069 6e66 6c75 656e 6365 2066 726f 6d20   influence from 
-000006a0: 6f74 6865 7220 6c69 6272 6172 6965 7320  other libraries 
-000006b0: 616e 6420 7265 736f 7572 6365 732e 2046  and resources. F
-000006c0: 6f72 2061 6464 6974 696f 6e61 6c20 6465  or additional de
-000006d0: 7461 696c 7320 7365 6520 7468 6520 7265  tails see the re
-000006e0: 6665 7265 6e63 6573 2073 6563 7469 6f6e  ferences section
-000006f0: 2e5c 6e5c 6e2a 2a53 7570 706f 7274 7320  .\n\n**Supports 
-00000700: 7370 6143 7920 7633 2061 6e64 2076 3220  spaCy v3 and v2 
-00000710: 283e 3d20 322e 3229 212a 2a5c 6e5c 6e53  (>= 2.2)!**\n\nS
-00000720: 7061 637a 7a20 6861 7320 6265 656e 2074  paczz has been t
-00000730: 6573 7465 6420 6f6e 2055 6275 6e74 7520  ested on Ubuntu 
-00000740: 3230 2e30 342c 204d 6163 4f53 2031 302e  20.04, MacOS 10.
-00000750: 3135 2c20 616e 6420 5769 6e64 6f77 7320  15, and Windows 
-00000760: 5365 7276 6572 2032 3031 392e 5c6e 5c6e  Server 2019.\n\n
-00000770: 2a76 302e 352e 3420 5265 6c65 6173 6520  *v0.5.4 Release 
-00000780: 4e6f 7465 733a 2a5c 6e2d 2042 7567 4669  Notes:*\n- BugFi
-00000790: 7820 666f 7220 6765 726d 616e 2043 6f6d  x for german Com
-000007a0: 6269 6e61 7469 6f6e 2077 6f72 6473 2066  bination words f
-000007b0: 6f72 2052 6567 6578 5365 6172 6368 6572  or RegexSearcher
-000007c0: 2e5c 6e2d 204f 7468 6572 206d 696e 6f72  .\n- Other minor
-000007d0: 2064 6f63 732f 746f 6f6c 696e 6720 7570   docs/tooling up
-000007e0: 6461 7465 732e 5c6e 5c6e 2a76 302e 352e  dates.\n\n*v0.5.
-000007f0: 3320 5265 6c65 6173 6520 4e6f 7465 733a  3 Release Notes:
-00000800: 2a5c 6e2d 202a 4669 7865 6420 6120 2262  *\n- *Fixed a "b
-00000810: 7567 2220 696e 2074 6865 2060 546f 6b65  ug" in the `Toke
-00000820: 6e4d 6174 6368 6572 602e 2053 7061 637a  nMatcher`. Spacz
-00000830: 7a20 6578 7065 6374 7320 746f 6b65 6e20  z expects token 
-00000840: 6d61 7463 6865 7320 7265 7475 726e 6564  matches returned
-00000850: 2069 6e20 6f72 6465 7220 6f66 2061 7363   in order of asc
-00000860: 656e 6469 6e67 206d 6174 6368 2073 7461  ending match sta
-00000870: 7274 2c20 7468 656e 2064 6573 6365 6e64  rt, then descend
-00000880: 696e 6720 6d61 7463 6820 6c65 6e67 7468  ing match length
-00000890: 2e20 486f 7765 7665 722c 2073 7061 4379  . However, spaCy
-000008a0: 5c27 7320 604d 6174 6368 6572 6020 646f  \'s `Matcher` do
-000008b0: 6573 206e 6f74 2072 6574 7572 6e20 6d61  es not return ma
-000008c0: 7463 6865 7320 696e 2074 6869 7320 6f72  tches in this or
-000008d0: 6465 7220 6279 2064 6566 6175 6c74 2e20  der by default. 
-000008e0: 4164 6465 6420 6120 736f 7274 2069 6e20  Added a sort in 
-000008f0: 7468 6520 6054 6f6b 656e 4d61 7463 6865  the `TokenMatche
-00000900: 7260 2074 6f20 656e 7375 7265 2074 6869  r` to ensure thi
-00000910: 732e 2a5c 6e5c 6e50 6c65 6173 6520 7365  s.*\n\nPlease se
-00000920: 6520 7468 6520 5b63 6861 6e67 656c 6f67  e the [changelog
-00000930: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000940: 2e63 6f6d 2f67 616e 6465 7273 656e 3130  .com/gandersen10
-00000950: 312f 7370 6163 7a7a 2f62 6c6f 622f 6d61  1/spaczz/blob/ma
-00000960: 7374 6572 2f43 4841 4e47 454c 4f47 2e6d  ster/CHANGELOG.m
-00000970: 6429 2066 6f72 2070 7265 7669 6f75 7320  d) for previous 
-00000980: 7265 6c65 6173 6520 6e6f 7465 732e 2054  release notes. T
-00000990: 6869 7320 7769 6c6c 2065 7665 6e74 7561  his will eventua
-000009a0: 6c6c 7920 6265 206d 6f76 6564 2074 6f20  lly be moved to 
-000009b0: 7468 6520 5b52 6561 6420 7468 6520 446f  the [Read the Do
-000009c0: 6373 5d28 6874 7470 733a 2f2f 7370 6163  cs](https://spac
-000009d0: 7a7a 2e72 6561 6474 6865 646f 6373 2e69  zz.readthedocs.i
-000009e0: 6f2f 656e 2f6c 6174 6573 742f 2920 7061  o/en/latest/) pa
-000009f0: 6765 2e5c 6e5c 6e3c 6831 3e54 6162 6c65  ge.\n\n<h1>Table
-00000a00: 206f 6620 436f 6e74 656e 7473 3c73 7061   of Contents<spa
-00000a10: 6e20 636c 6173 733d 2274 6f63 536b 6970  n class="tocSkip
-00000a20: 223e 3c2f 7370 616e 3e3c 2f68 313e 5c6e  "></span></h1>\n
-00000a30: 3c64 6976 2063 6c61 7373 3d22 746f 6322  <div class="toc"
-00000a40: 3e3c 756c 2063 6c61 7373 3d22 746f 632d  ><ul class="toc-
-00000a50: 6974 656d 223e 3c6c 693e 3c73 7061 6e3e  item"><li><span>
-00000a60: 3c61 2068 7265 663d 2223 496e 7374 616c  <a href="#Instal
-00000a70: 6c61 7469 6f6e 2220 6461 7461 2d74 6f63  lation" data-toc
-00000a80: 2d6d 6f64 6966 6965 642d 6964 3d22 496e  -modified-id="In
-00000a90: 7374 616c 6c61 7469 6f6e 2d31 223e 496e  stallation-1">In
-00000aa0: 7374 616c 6c61 7469 6f6e 3c2f 613e 3c2f  stallation</a></
-00000ab0: 7370 616e 3e3c 2f6c 693e 3c6c 693e 3c73  span></li><li><s
-00000ac0: 7061 6e3e 3c61 2068 7265 663d 2223 4261  pan><a href="#Ba
-00000ad0: 7369 632d 5573 6167 6522 2064 6174 612d  sic-Usage" data-
-00000ae0: 746f 632d 6d6f 6469 6669 6564 2d69 643d  toc-modified-id=
-00000af0: 2242 6173 6963 2d55 7361 6765 2d32 223e  "Basic-Usage-2">
-00000b00: 4261 7369 6320 5573 6167 653c 2f61 3e3c  Basic Usage</a><
-00000b10: 2f73 7061 6e3e 3c75 6c20 636c 6173 733d  /span><ul class=
-00000b20: 2274 6f63 2d69 7465 6d22 3e3c 6c69 3e3c  "toc-item"><li><
-00000b30: 7370 616e 3e3c 6120 6872 6566 3d22 2346  span><a href="#F
-00000b40: 757a 7a79 4d61 7463 6865 7222 2064 6174  uzzyMatcher" dat
-00000b50: 612d 746f 632d 6d6f 6469 6669 6564 2d69  a-toc-modified-i
-00000b60: 643d 2246 757a 7a79 4d61 7463 6865 722d  d="FuzzyMatcher-
-00000b70: 322e 3122 3e46 757a 7a79 4d61 7463 6865  2.1">FuzzyMatche
-00000b80: 723c 2f61 3e3c 2f73 7061 6e3e 3c2f 6c69  r</a></span></li
-00000b90: 3e3c 6c69 3e3c 7370 616e 3e3c 6120 6872  ><li><span><a hr
-00000ba0: 6566 3d22 2352 6567 6578 4d61 7463 6865  ef="#RegexMatche
-00000bb0: 7222 2064 6174 612d 746f 632d 6d6f 6469  r" data-toc-modi
-00000bc0: 6669 6564 2d69 643d 2252 6567 6578 4d61  fied-id="RegexMa
-00000bd0: 7463 6865 722d 322e 3222 3e52 6567 6578  tcher-2.2">Regex
-00000be0: 4d61 7463 6865 723c 2f61 3e3c 2f73 7061  Matcher</a></spa
-00000bf0: 6e3e 3c2f 6c69 3e3c 6c69 3e3c 7370 616e  n></li><li><span
-00000c00: 3e3c 6120 6872 6566 3d22 2353 696d 696c  ><a href="#Simil
-00000c10: 6172 6974 794d 6174 6368 6572 2220 6461  arityMatcher" da
-00000c20: 7461 2d74 6f63 2d6d 6f64 6966 6965 642d  ta-toc-modified-
-00000c30: 6964 3d22 5369 6d69 6c61 7269 7479 4d61  id="SimilarityMa
-00000c40: 7463 6865 722d 322e 3322 3e53 696d 696c  tcher-2.3">Simil
-00000c50: 6172 6974 794d 6174 6368 6572 3c2f 613e  arityMatcher</a>
-00000c60: 3c2f 7370 616e 3e3c 2f6c 693e 3c6c 693e  </span></li><li>
-00000c70: 3c73 7061 6e3e 3c61 2068 7265 663d 2223  <span><a href="#
-00000c80: 546f 6b65 6e4d 6174 6368 6572 2220 6461  TokenMatcher" da
-00000c90: 7461 2d74 6f63 2d6d 6f64 6966 6965 642d  ta-toc-modified-
-00000ca0: 6964 3d22 546f 6b65 6e4d 6174 6368 6572  id="TokenMatcher
-00000cb0: 2d32 2e34 223e 546f 6b65 6e4d 6174 6368  -2.4">TokenMatch
-00000cc0: 6572 3c2f 613e 3c2f 7370 616e 3e3c 2f6c  er</a></span></l
-00000cd0: 693e 3c6c 693e 3c73 7061 6e3e 3c61 2068  i><li><span><a h
-00000ce0: 7265 663d 2223 5370 6163 7a7a 5275 6c65  ref="#SpaczzRule
-00000cf0: 7222 2064 6174 612d 746f 632d 6d6f 6469  r" data-toc-modi
-00000d00: 6669 6564 2d69 643d 2253 7061 637a 7a52  fied-id="SpaczzR
-00000d10: 756c 6572 2d32 2e35 223e 5370 6163 7a7a  uler-2.5">Spaczz
-00000d20: 5275 6c65 723c 2f61 3e3c 2f73 7061 6e3e  Ruler</a></span>
-00000d30: 3c2f 6c69 3e3c 6c69 3e3c 7370 616e 3e3c  </li><li><span><
-00000d40: 6120 6872 6566 3d22 2343 7573 746f 6d2d  a href="#Custom-
-00000d50: 4174 7472 6962 7574 6573 2220 6461 7461  Attributes" data
-00000d60: 2d74 6f63 2d6d 6f64 6966 6965 642d 6964  -toc-modified-id
-00000d70: 3d22 4375 7374 6f6d 2d41 7474 7269 6275  ="Custom-Attribu
-00000d80: 7465 732d 322e 3622 3e43 7573 746f 6d20  tes-2.6">Custom 
-00000d90: 4174 7472 6962 7574 6573 3c2f 613e 3c2f  Attributes</a></
-00000da0: 7370 616e 3e3c 2f6c 693e 3c6c 693e 3c73  span></li><li><s
-00000db0: 7061 6e3e 3c61 2068 7265 663d 2223 5361  pan><a href="#Sa
-00000dc0: 7669 6e67 2f4c 6f61 6469 6e67 2220 6461  ving/Loading" da
-00000dd0: 7461 2d74 6f63 2d6d 6f64 6966 6965 642d  ta-toc-modified-
-00000de0: 6964 3d22 5361 7669 6e67 2f4c 6f61 6469  id="Saving/Loadi
-00000df0: 6e67 2d32 2e37 223e 5361 7669 6e67 2f4c  ng-2.7">Saving/L
-00000e00: 6f61 6469 6e67 3c2f 613e 3c2f 7370 616e  oading</a></span
-00000e10: 3e3c 2f6c 693e 3c2f 756c 3e3c 2f6c 693e  ></li></ul></li>
-00000e20: 3c6c 693e 3c73 7061 6e3e 3c61 2068 7265  <li><span><a hre
-00000e30: 663d 2223 4b6e 6f77 6e2d 4973 7375 6573  f="#Known-Issues
-00000e40: 2220 6461 7461 2d74 6f63 2d6d 6f64 6966  " data-toc-modif
-00000e50: 6965 642d 6964 3d22 4b6e 6f77 6e2d 4973  ied-id="Known-Is
-00000e60: 7375 6573 2d33 223e 4b6e 6f77 6e20 4973  sues-3">Known Is
-00000e70: 7375 6573 3c2f 613e 3c2f 7370 616e 3e3c  sues</a></span><
-00000e80: 756c 2063 6c61 7373 3d22 746f 632d 6974  ul class="toc-it
-00000e90: 656d 223e 3c6c 693e 3c73 7061 6e3e 3c61  em"><li><span><a
-00000ea0: 2068 7265 663d 2223 5065 7266 6f72 6d61   href="#Performa
-00000eb0: 6e63 6522 2064 6174 612d 746f 632d 6d6f  nce" data-toc-mo
-00000ec0: 6469 6669 6564 2d69 643d 2250 6572 666f  dified-id="Perfo
-00000ed0: 726d 616e 6365 2d33 2e31 223e 5065 7266  rmance-3.1">Perf
-00000ee0: 6f72 6d61 6e63 653c 2f61 3e3c 2f73 7061  ormance</a></spa
-00000ef0: 6e3e 3c2f 6c69 3e3c 6c69 3e3c 7370 616e  n></li><li><span
-00000f00: 3e3c 6120 6872 6566 3d22 2353 7061 637a  ><a href="#Spacz
-00000f10: 7a52 756c 6572 2d49 6e63 6f6e 7369 7374  zRuler-Inconsist
-00000f20: 656e 6369 6573 2220 6461 7461 2d74 6f63  encies" data-toc
-00000f30: 2d6d 6f64 6966 6965 642d 6964 3d22 5370  -modified-id="Sp
-00000f40: 6163 7a7a 5275 6c65 722d 496e 636f 6e73  aczzRuler-Incons
-00000f50: 6973 7465 6e63 6965 732d 332e 3222 3e53  istencies-3.2">S
-00000f60: 7061 637a 7a52 756c 6572 2049 6e63 6f6e  paczzRuler Incon
-00000f70: 7369 7374 656e 6369 6573 3c2f 613e 3c2f  sistencies</a></
-00000f80: 7370 616e 3e3c 2f6c 693e 3c2f 756c 3e3c  span></li></ul><
-00000f90: 2f6c 693e 3c6c 693e 3c73 7061 6e3e 3c61  /li><li><span><a
-00000fa0: 2068 7265 663d 2223 526f 6164 6d61 7022   href="#Roadmap"
-00000fb0: 2064 6174 612d 746f 632d 6d6f 6469 6669   data-toc-modifi
-00000fc0: 6564 2d69 643d 2252 6f61 646d 6170 2d34  ed-id="Roadmap-4
-00000fd0: 223e 526f 6164 6d61 703c 2f61 3e3c 2f73  ">Roadmap</a></s
-00000fe0: 7061 6e3e 3c2f 6c69 3e3c 6c69 3e3c 7370  pan></li><li><sp
-00000ff0: 616e 3e3c 6120 6872 6566 3d22 2344 6576  an><a href="#Dev
-00001000: 656c 6f70 6d65 6e74 2220 6461 7461 2d74  elopment" data-t
-00001010: 6f63 2d6d 6f64 6966 6965 642d 6964 3d22  oc-modified-id="
-00001020: 4465 7665 6c6f 706d 656e 742d 3522 3e44  Development-5">D
-00001030: 6576 656c 6f70 6d65 6e74 3c2f 613e 3c2f  evelopment</a></
-00001040: 7370 616e 3e3c 2f6c 693e 3c6c 693e 3c73  span></li><li><s
-00001050: 7061 6e3e 3c61 2068 7265 663d 2223 5265  pan><a href="#Re
-00001060: 6665 7265 6e63 6573 2220 6461 7461 2d74  ferences" data-t
-00001070: 6f63 2d6d 6f64 6966 6965 642d 6964 3d22  oc-modified-id="
-00001080: 5265 6665 7265 6e63 6573 2d36 223e 5265  References-6">Re
-00001090: 6665 7265 6e63 6573 3c2f 613e 3c2f 7370  ferences</a></sp
-000010a0: 616e 3e3c 2f6c 693e 3c2f 756c 3e3c 2f64  an></li></ul></d
-000010b0: 6976 3e5c 6e5c 6e23 2320 496e 7374 616c  iv>\n\n## Instal
-000010c0: 6c61 7469 6f6e 5c6e 5c6e 5370 6163 7a7a  lation\n\nSpaczz
-000010d0: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
-000010e0: 6420 7573 696e 6720 7069 702e 5c6e 5c6e  d using pip.\n\n
-000010f0: 5c6e 6060 6070 7974 686f 6e5c 6e70 6970  \n```python\npip
-00001100: 2069 6e73 7461 6c6c 2073 7061 637a 7a5c   install spaczz\
-00001110: 6e60 6060 5c6e 5c6e 2323 2042 6173 6963  n```\n\n## Basic
-00001120: 2055 7361 6765 5c6e 5c6e 5370 6163 7a7a   Usage\n\nSpaczz
-00001130: 5c27 7320 7072 696d 6172 7920 6665 6174  \'s primary feat
-00001140: 7572 6573 2061 7265 2074 6865 2060 4675  ures are the `Fu
-00001150: 7a7a 794d 6174 6368 6572 602c 2060 5265  zzyMatcher`, `Re
-00001160: 6765 784d 6174 6368 6572 602c 2061 6e64  gexMatcher`, and
-00001170: 2022 6675 7a7a 7922 2060 546f 6b65 6e4d   "fuzzy" `TokenM
-00001180: 6174 6368 6572 6020 7468 6174 2066 756e  atcher` that fun
-00001190: 6374 696f 6e20 7369 6d69 6c61 726c 7920  ction similarly 
-000011a0: 746f 2073 7061 4379 5c27 7320 604d 6174  to spaCy\'s `Mat
-000011b0: 6368 6572 6020 616e 6420 6050 6872 6173  cher` and `Phras
-000011c0: 654d 6174 6368 6572 602c 2061 6e64 2074  eMatcher`, and t
-000011d0: 6865 2060 5370 6163 7a7a 5275 6c65 7260  he `SpaczzRuler`
-000011e0: 2077 6869 6368 2069 6e74 6567 7261 7465   which integrate
-000011f0: 7320 7468 6520 7370 6163 7a7a 206d 6174  s the spaczz mat
-00001200: 6368 6572 7320 696e 746f 2061 2073 7061  chers into a spa
-00001210: 4379 2070 6970 656c 696e 6520 636f 6d70  Cy pipeline comp
-00001220: 6f6e 656e 7420 7369 6d69 6c61 7220 746f  onent similar to
-00001230: 2073 7061 4379 5c27 7320 6045 6e74 6974   spaCy\'s `Entit
-00001240: 7952 756c 6572 602e 5c6e 5c6e 2323 2320  yRuler`.\n\n### 
-00001250: 4675 7a7a 794d 6174 6368 6572 5c6e 5c6e  FuzzyMatcher\n\n
-00001260: 5468 6520 6261 7369 6320 7573 6167 6520  The basic usage 
-00001270: 6f66 2074 6865 2066 757a 7a79 206d 6174  of the fuzzy mat
-00001280: 6368 6572 2069 7320 7369 6d69 6c61 7220  cher is similar 
-00001290: 746f 2073 7061 4379 5c27 7320 6050 6872  to spaCy\'s `Phr
-000012a0: 6173 654d 6174 6368 6572 6020 6578 6365  aseMatcher` exce
-000012b0: 7074 2069 7420 7265 7475 726e 7320 7468  pt it returns th
-000012c0: 6520 6675 7a7a 7920 7261 7469 6f20 616c  e fuzzy ratio al
-000012d0: 6f6e 6720 7769 7468 206d 6174 6368 2069  ong with match i
-000012e0: 642c 2073 7461 7274 2061 6e64 2065 6e64  d, start and end
-000012f0: 2069 6e66 6f72 6d61 7469 6f6e 2c20 736f   information, so
-00001300: 206d 616b 6520 7375 7265 2074 6f20 696e   make sure to in
-00001310: 636c 7564 6520 6120 7661 7269 6162 6c65  clude a variable
-00001320: 2066 6f72 2074 6865 2072 6174 696f 2077   for the ratio w
-00001330: 6865 6e20 756e 7061 636b 696e 6720 7265  hen unpacking re
-00001340: 7375 6c74 732e 5c6e 5c6e 5c6e 6060 6070  sults.\n\n\n```p
-00001350: 7974 686f 6e5c 6e69 6d70 6f72 7420 7370  ython\nimport sp
-00001360: 6163 795c 6e66 726f 6d20 7370 6163 7a7a  acy\nfrom spaczz
-00001370: 2e6d 6174 6368 6572 2069 6d70 6f72 7420  .matcher import 
-00001380: 4675 7a7a 794d 6174 6368 6572 5c6e 5c6e  FuzzyMatcher\n\n
-00001390: 6e6c 7020 3d20 7370 6163 792e 626c 616e  nlp = spacy.blan
-000013a0: 6b28 2265 6e22 295c 6e74 6578 7420 3d20  k("en")\ntext = 
-000013b0: 2222 2247 7269 6e74 2041 6e64 6572 736f  """Grint Anderso
-000013c0: 6e20 6372 6561 7465 6420 7370 6163 7a7a  n created spaczz
-000013d0: 2069 6e20 6869 7320 686f 6d65 2061 7420   in his home at 
-000013e0: 3535 3520 4661 6b65 2053 742c 5c6e 4170  555 Fake St,\nAp
-000013f0: 7420 3520 696e 204e 6173 6876 316c 652c  t 5 in Nashv1le,
-00001400: 2054 4e20 3535 3535 352d 3132 3334 2069   TN 55555-1234 i
-00001410: 6e20 7468 6520 5553 2e22 2222 2020 2320  n the US."""  # 
-00001420: 5370 656c 6c69 6e67 2065 7272 6f72 7320  Spelling errors 
-00001430: 696e 7465 6e74 696f 6e61 6c2e 5c6e 646f  intentional.\ndo
-00001440: 6320 3d20 6e6c 7028 7465 7874 295c 6e5c  c = nlp(text)\n\
-00001450: 6e6d 6174 6368 6572 203d 2046 757a 7a79  nmatcher = Fuzzy
-00001460: 4d61 7463 6865 7228 6e6c 702e 766f 6361  Matcher(nlp.voca
-00001470: 6229 5c6e 6d61 7463 6865 722e 6164 6428  b)\nmatcher.add(
-00001480: 224e 414d 4522 2c20 5b6e 6c70 2822 4772  "NAME", [nlp("Gr
-00001490: 616e 7420 416e 6465 7273 656e 2229 5d29  ant Andersen")])
-000014a0: 5c6e 6d61 7463 6865 722e 6164 6428 2247  \nmatcher.add("G
-000014b0: 5045 222c 205b 6e6c 7028 224e 6173 6876  PE", [nlp("Nashv
-000014c0: 696c 6c65 2229 5d29 5c6e 6d61 7463 6865  ille")])\nmatche
-000014d0: 7320 3d20 6d61 7463 6865 7228 646f 6329  s = matcher(doc)
-000014e0: 5c6e 5c6e 666f 7220 6d61 7463 685f 6964  \n\nfor match_id
-000014f0: 2c20 7374 6172 742c 2065 6e64 2c20 7261  , start, end, ra
-00001500: 7469 6f20 696e 206d 6174 6368 6573 3a5c  tio in matches:\
-00001510: 6e20 2020 2070 7269 6e74 286d 6174 6368  n    print(match
-00001520: 5f69 642c 2064 6f63 5b73 7461 7274 3a65  _id, doc[start:e
-00001530: 6e64 5d2c 2072 6174 696f 295c 6e60 6060  nd], ratio)\n```
-00001540: 5c6e 5c6e 2020 2020 4e41 4d45 2047 7269  \n\n    NAME Gri
-00001550: 6e74 2041 6e64 6572 736f 6e20 3836 5c6e  nt Anderson 86\n
-00001560: 2020 2020 4750 4520 4e61 7368 7631 6c65      GPE Nashv1le
-00001570: 2038 325c 6e5c 6e5c 6e55 6e6c 696b 6520   82\n\n\nUnlike 
-00001580: 7370 6143 7920 6d61 7463 6865 7273 2c20  spaCy matchers, 
-00001590: 7370 6163 7a7a 206d 6174 6368 6572 7320  spaczz matchers 
-000015a0: 6172 6520 7772 6974 7465 6e20 696e 2070  are written in p
-000015b0: 7572 6520 5079 7468 6f6e 2e20 5768 696c  ure Python. Whil
-000015c0: 6520 7468 6579 2061 7265 2072 6571 7569  e they are requi
-000015d0: 7265 6420 746f 2068 6176 6520 6120 7370  red to have a sp
-000015e0: 6143 7920 766f 6361 6220 7061 7373 6564  aCy vocab passed
-000015f0: 2074 6f20 7468 656d 2064 7572 696e 6720   to them during 
-00001600: 696e 6974 6961 6c69 7a61 7469 6f6e 2c20  initialization, 
-00001610: 7468 6973 2069 7320 7075 7265 6c79 2066  this is purely f
-00001620: 6f72 2063 6f6e 7369 7374 656e 6379 2061  or consistency a
-00001630: 7320 7468 6520 7370 6163 7a7a 206d 6174  s the spaczz mat
-00001640: 6368 6572 7320 646f 206e 6f74 2075 7365  chers do not use
-00001650: 2063 7572 7265 6e74 6c79 2075 7365 2074   currently use t
-00001660: 6865 2073 7061 4379 2076 6f63 6162 2e20  he spaCy vocab. 
-00001670: 5468 6973 2069 7320 7768 7920 7468 6520  This is why the 
-00001680: 606d 6174 6368 5f69 6460 2061 626f 7665  `match_id` above
-00001690: 2069 7320 7369 6d70 6c79 2061 2073 7472   is simply a str
-000016a0: 696e 6720 696e 7374 6561 6420 6f66 2061  ing instead of a
-000016b0: 6e20 696e 7465 6765 7220 7661 6c75 6520  n integer value 
-000016c0: 6c69 6b65 2069 6e20 7370 6143 7920 6d61  like in spaCy ma
-000016d0: 7463 6865 7273 2e5c 6e5c 6e53 7061 637a  tchers.\n\nSpacz
-000016e0: 7a20 6d61 7463 6865 7273 2063 616e 2061  z matchers can a
-000016f0: 6c73 6f20 6d61 6b65 2075 7365 206f 6620  lso make use of 
-00001700: 6f6e 2d6d 6174 6368 2072 756c 6573 2076  on-match rules v
-00001710: 6961 2063 616c 6c62 6163 6b20 6675 6e63  ia callback func
-00001720: 7469 6f6e 732e 2054 6865 7365 206f 6e2d  tions. These on-
-00001730: 6d61 7463 6820 6361 6c6c 6261 636b 7320  match callbacks 
-00001740: 6e65 6564 2074 6f20 6163 6365 7074 2074  need to accept t
-00001750: 6865 206d 6174 6368 6572 2069 7473 656c  he matcher itsel
-00001760: 662c 2074 6865 2064 6f63 2074 6865 206d  f, the doc the m
-00001770: 6174 6368 6572 2077 6173 2063 616c 6c65  atcher was calle
-00001780: 6420 6f6e 2c20 7468 6520 6d61 7463 6820  d on, the match 
-00001790: 696e 6465 7820 616e 6420 7468 6520 6d61  index and the ma
-000017a0: 7463 6865 7320 7072 6f64 7563 6564 2062  tches produced b
-000017b0: 7920 7468 6520 6d61 7463 6865 722e 5c6e  y the matcher.\n
-000017c0: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e69  \n\n```python\ni
-000017d0: 6d70 6f72 7420 7370 6163 795c 6e66 726f  mport spacy\nfro
-000017e0: 6d20 7370 6163 792e 746f 6b65 6e73 2069  m spacy.tokens i
-000017f0: 6d70 6f72 7420 5370 616e 5c6e 6672 6f6d  mport Span\nfrom
-00001800: 2073 7061 637a 7a2e 6d61 7463 6865 7220   spaczz.matcher 
-00001810: 696d 706f 7274 2046 757a 7a79 4d61 7463  import FuzzyMatc
-00001820: 6865 725c 6e5c 6e6e 6c70 203d 2073 7061  her\n\nnlp = spa
-00001830: 6379 2e62 6c61 6e6b 2822 656e 2229 5c6e  cy.blank("en")\n
-00001840: 7465 7874 203d 2022 2222 4772 696e 7420  text = """Grint 
-00001850: 416e 6465 7273 6f6e 2063 7265 6174 6564  Anderson created
-00001860: 2073 7061 637a 7a20 696e 2068 6973 2068   spaczz in his h
-00001870: 6f6d 6520 6174 2035 3535 2046 616b 6520  ome at 555 Fake 
-00001880: 5374 2c5c 6e41 7074 2035 2069 6e20 4e61  St,\nApt 5 in Na
-00001890: 7368 7631 6c65 2c20 544e 2035 3535 3535  shv1le, TN 55555
-000018a0: 2d31 3233 3420 696e 2074 6865 2055 532e  -1234 in the US.
-000018b0: 2222 2220 2023 2053 7065 6c6c 696e 6720  """  # Spelling 
-000018c0: 6572 726f 7273 2069 6e74 656e 7469 6f6e  errors intention
-000018d0: 616c 2e5c 6e64 6f63 203d 206e 6c70 2874  al.\ndoc = nlp(t
-000018e0: 6578 7429 5c6e 5c6e 5c6e 6465 6620 6164  ext)\n\n\ndef ad
-000018f0: 645f 6e61 6d65 5f65 6e74 286d 6174 6368  d_name_ent(match
-00001900: 6572 2c20 646f 632c 2069 2c20 6d61 7463  er, doc, i, matc
-00001910: 6865 7329 3a5c 6e20 2020 2022 2222 4361  hes):\n    """Ca
-00001920: 6c6c 6261 636b 206f 6e20 6d61 7463 6820  llback on match 
-00001930: 6675 6e63 7469 6f6e 2e20 4164 6473 2022  function. Adds "
-00001940: 4e41 4d45 2220 656e 7469 7469 6573 2074  NAME" entities t
-00001950: 6f20 646f 632e 2222 225c 6e20 2020 2023  o doc."""\n    #
-00001960: 2047 6574 2074 6865 2063 7572 7265 6e74   Get the current
-00001970: 206d 6174 6368 2061 6e64 2063 7265 6174   match and creat
-00001980: 6520 7475 706c 6520 6f66 2065 6e74 6974  e tuple of entit
-00001990: 7920 6c61 6265 6c2c 2073 7461 7274 2061  y label, start a
-000019a0: 6e64 2065 6e64 2e5c 6e20 2020 2023 2041  nd end.\n    # A
-000019b0: 7070 656e 6420 656e 7469 7479 2074 6f20  ppend entity to 
-000019c0: 7468 6520 646f 635c 2773 2065 6e74 6974  the doc\'s entit
-000019d0: 792e 2028 446f 6e5c 2774 206f 7665 7277  y. (Don\'t overw
-000019e0: 7269 7465 2064 6f63 2e65 6e74 7321 295c  rite doc.ents!)\
-000019f0: 6e20 2020 205f 6d61 7463 685f 6964 2c20  n    _match_id, 
-00001a00: 7374 6172 742c 2065 6e64 2c20 5f72 6174  start, end, _rat
-00001a10: 696f 203d 206d 6174 6368 6573 5b69 5d5c  io = matches[i]\
-00001a20: 6e20 2020 2065 6e74 6974 7920 3d20 5370  n    entity = Sp
-00001a30: 616e 2864 6f63 2c20 7374 6172 742c 2065  an(doc, start, e
-00001a40: 6e64 2c20 6c61 6265 6c3d 224e 414d 4522  nd, label="NAME"
-00001a50: 295c 6e20 2020 2064 6f63 2e65 6e74 7320  )\n    doc.ents 
-00001a60: 2b3d 2028 656e 7469 7479 2c29 5c6e 5c6e  += (entity,)\n\n
-00001a70: 5c6e 6d61 7463 6865 7220 3d20 4675 7a7a  \nmatcher = Fuzz
-00001a80: 794d 6174 6368 6572 286e 6c70 2e76 6f63  yMatcher(nlp.voc
-00001a90: 6162 295c 6e6d 6174 6368 6572 2e61 6464  ab)\nmatcher.add
-00001aa0: 2822 4e41 4d45 222c 205b 6e6c 7028 2247  ("NAME", [nlp("G
-00001ab0: 7261 6e74 2041 6e64 6572 7365 6e22 295d  rant Andersen")]
-00001ac0: 2c20 6f6e 5f6d 6174 6368 3d61 6464 5f6e  , on_match=add_n
-00001ad0: 616d 655f 656e 7429 5c6e 6d61 7463 6865  ame_ent)\nmatche
-00001ae0: 7320 3d20 6d61 7463 6865 7228 646f 6329  s = matcher(doc)
-00001af0: 5c6e 5c6e 666f 7220 656e 7420 696e 2064  \n\nfor ent in d
-00001b00: 6f63 2e65 6e74 733a 5c6e 2020 2020 7072  oc.ents:\n    pr
-00001b10: 696e 7428 2865 6e74 2e74 6578 742c 2065  int((ent.text, e
-00001b20: 6e74 2e73 7461 7274 2c20 656e 742e 656e  nt.start, ent.en
-00001b30: 642c 2065 6e74 2e6c 6162 656c 5f29 295c  d, ent.label_))\
-00001b40: 6e60 6060 5c6e 5c6e 2020 2020 285c 2747  n```\n\n    (\'G
-00001b50: 7269 6e74 2041 6e64 6572 736f 6e5c 272c  rint Anderson\',
-00001b60: 2030 2c20 322c 205c 274e 414d 455c 2729   0, 2, \'NAME\')
-00001b70: 5c6e 5c6e 5c6e 4c69 6b65 2073 7061 4379  \n\n\nLike spaCy
-00001b80: 5c27 7320 6045 6e74 6974 7952 756c 6572  \'s `EntityRuler
-00001b90: 602c 2061 2076 6572 7920 7369 6d69 6c61  `, a very simila
-00001ba0: 7220 656e 7469 7479 2075 7064 6174 696e  r entity updatin
-00001bb0: 6720 6c6f 6769 6320 6861 7320 6265 656e  g logic has been
-00001bc0: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-00001bd0: 7468 6520 6053 7061 637a 7a52 756c 6572  the `SpaczzRuler
-00001be0: 602e 2054 6865 2060 5370 6163 7a7a 5275  `. The `SpaczzRu
-00001bf0: 6c65 7260 2061 6c73 6f20 7461 6b65 7320  ler` also takes 
-00001c00: 6361 7265 206f 6620 6861 6e64 6c69 6e67  care of handling
-00001c10: 206f 7665 726c 6170 7069 6e67 206d 6174   overlapping mat
-00001c20: 6368 6573 2e20 4974 2069 7320 6469 7363  ches. It is disc
-00001c30: 7573 7365 6420 696e 2061 206c 6174 6572  ussed in a later
-00001c40: 2073 6563 7469 6f6e 2e5c 6e5c 6e55 6e6c   section.\n\nUnl
-00001c50: 696b 6520 7370 6143 795c 2773 206d 6174  ike spaCy\'s mat
-00001c60: 6368 6572 732c 2072 756c 6573 2061 6464  chers, rules add
-00001c70: 6564 2074 6f20 7370 6163 7a7a 206d 6174  ed to spaczz mat
-00001c80: 6368 6572 7320 6861 7665 206f 7074 696f  chers have optio
-00001c90: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
-00001ca0: 6d65 6e74 7320 7468 6174 2063 616e 206d  ments that can m
-00001cb0: 6f64 6966 7920 7468 6520 6d61 7463 6869  odify the matchi
-00001cc0: 6e67 2062 6568 6176 696f 722e 2054 616b  ng behavior. Tak
-00001cd0: 6520 7468 6520 6265 6c6f 7720 6675 7a7a  e the below fuzz
-00001ce0: 7920 6d61 7463 6869 6e67 2065 7861 6d70  y matching examp
-00001cf0: 6c65 733a 5c6e 5c6e 5c6e 6060 6070 7974  les:\n\n\n```pyt
-00001d00: 686f 6e5c 6e69 6d70 6f72 7420 7370 6163  hon\nimport spac
-00001d10: 795c 6e66 726f 6d20 7370 6163 7a7a 2e6d  y\nfrom spaczz.m
-00001d20: 6174 6368 6572 2069 6d70 6f72 7420 4675  atcher import Fu
-00001d30: 7a7a 794d 6174 6368 6572 5c6e 5c6e 6e6c  zzyMatcher\n\nnl
-00001d40: 7020 3d20 7370 6163 792e 626c 616e 6b28  p = spacy.blank(
-00001d50: 2265 6e22 295c 6e23 204c 6574 5c27 7320  "en")\n# Let\'s 
-00001d60: 6d6f 6469 6679 2074 6865 206f 7264 6572  modify the order
-00001d70: 206f 6620 7468 6520 6e61 6d65 2069 6e20   of the name in 
-00001d80: 7468 6520 7465 7874 2e5c 6e74 6578 7420  the text.\ntext 
-00001d90: 3d20 2222 2241 6e64 6572 736f 6e2c 2047  = """Anderson, G
-00001da0: 7269 6e74 2063 7265 6174 6564 2073 7061  rint created spa
-00001db0: 637a 7a20 696e 2068 6973 2068 6f6d 6520  czz in his home 
-00001dc0: 6174 2035 3535 2046 616b 6520 5374 2c5c  at 555 Fake St,\
-00001dd0: 6e41 7074 2035 2069 6e20 4e61 7368 7631  nApt 5 in Nashv1
-00001de0: 6c65 2c20 544e 2035 3535 3535 2d31 3233  le, TN 55555-123
-00001df0: 3420 696e 2074 6865 2055 532e 2222 2220  4 in the US.""" 
-00001e00: 2023 2053 7065 6c6c 696e 6720 6572 726f   # Spelling erro
-00001e10: 7273 2069 6e74 656e 7469 6f6e 616c 2e5c  rs intentional.\
-00001e20: 6e64 6f63 203d 206e 6c70 2874 6578 7429  ndoc = nlp(text)
-00001e30: 5c6e 5c6e 6d61 7463 6865 7220 3d20 4675  \n\nmatcher = Fu
-00001e40: 7a7a 794d 6174 6368 6572 286e 6c70 2e76  zzyMatcher(nlp.v
-00001e50: 6f63 6162 295c 6e6d 6174 6368 6572 2e61  ocab)\nmatcher.a
-00001e60: 6464 2822 4e41 4d45 222c 205b 6e6c 7028  dd("NAME", [nlp(
-00001e70: 2247 7261 6e74 2041 6e64 6572 7365 6e22  "Grant Andersen"
-00001e80: 295d 295c 6e6d 6174 6368 6573 203d 206d  )])\nmatches = m
-00001e90: 6174 6368 6572 2864 6f63 295c 6e5c 6e23  atcher(doc)\n\n#
-00001ea0: 2054 6865 2064 6566 6175 6c74 2066 757a   The default fuz
-00001eb0: 7a79 206d 6174 6368 696e 6720 7365 7474  zy matching sett
-00001ec0: 696e 6773 2077 696c 6c20 6e6f 7420 6669  ings will not fi
-00001ed0: 6e64 2061 206d 6174 6368 2e5c 6e66 6f72  nd a match.\nfor
-00001ee0: 206d 6174 6368 5f69 642c 2073 7461 7274   match_id, start
-00001ef0: 2c20 656e 642c 2072 6174 696f 2069 6e20  , end, ratio in 
-00001f00: 6d61 7463 6865 733a 5c6e 2020 2020 7072  matches:\n    pr
-00001f10: 696e 7428 6d61 7463 685f 6964 2c20 646f  int(match_id, do
-00001f20: 635b 7374 6172 743a 656e 645d 2c20 7261  c[start:end], ra
-00001f30: 7469 6f29 5c6e 6060 605c 6e5c 6e4e 6578  tio)\n```\n\nNex
-00001f40: 7420 7765 2063 6861 6e67 6520 7468 6520  t we change the 
-00001f50: 6675 7a7a 7920 6d61 7463 6869 6e67 2062  fuzzy matching b
-00001f60: 6568 6176 696f 7220 666f 7220 7468 6520  ehavior for the 
-00001f70: 224e 414d 4522 2072 756c 652e 5c6e 5c6e  "NAME" rule.\n\n
-00001f80: 5c6e 6060 6070 7974 686f 6e5c 6e69 6d70  \n```python\nimp
-00001f90: 6f72 7420 7370 6163 795c 6e66 726f 6d20  ort spacy\nfrom 
-00001fa0: 7370 6163 7a7a 2e6d 6174 6368 6572 2069  spaczz.matcher i
-00001fb0: 6d70 6f72 7420 4675 7a7a 794d 6174 6368  mport FuzzyMatch
-00001fc0: 6572 5c6e 5c6e 6e6c 7020 3d20 7370 6163  er\n\nnlp = spac
-00001fd0: 792e 626c 616e 6b28 2265 6e22 295c 6e23  y.blank("en")\n#
-00001fe0: 204c 6574 5c27 7320 6d6f 6469 6679 2074   Let\'s modify t
-00001ff0: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
-00002000: 6e61 6d65 2069 6e20 7468 6520 7465 7874  name in the text
-00002010: 2e5c 6e74 6578 7420 3d20 2222 2241 6e64  .\ntext = """And
-00002020: 6572 736f 6e2c 2047 7269 6e74 2063 7265  erson, Grint cre
-00002030: 6174 6564 2073 7061 637a 7a20 696e 2068  ated spaczz in h
-00002040: 6973 2068 6f6d 6520 6174 2035 3535 2046  is home at 555 F
-00002050: 616b 6520 5374 2c5c 6e41 7074 2035 2069  ake St,\nApt 5 i
-00002060: 6e20 4e61 7368 7631 6c65 2c20 544e 2035  n Nashv1le, TN 5
-00002070: 3535 3535 2d31 3233 3420 696e 2074 6865  5555-1234 in the
-00002080: 2055 532e 2222 2220 2023 2053 7065 6c6c   US."""  # Spell
-00002090: 696e 6720 6572 726f 7273 2069 6e74 656e  ing errors inten
-000020a0: 7469 6f6e 616c 2e5c 6e64 6f63 203d 206e  tional.\ndoc = n
-000020b0: 6c70 2874 6578 7429 5c6e 5c6e 6d61 7463  lp(text)\n\nmatc
-000020c0: 6865 7220 3d20 4675 7a7a 794d 6174 6368  her = FuzzyMatch
-000020d0: 6572 286e 6c70 2e76 6f63 6162 295c 6e6d  er(nlp.vocab)\nm
-000020e0: 6174 6368 6572 2e61 6464 2822 4e41 4d45  atcher.add("NAME
-000020f0: 222c 205b 6e6c 7028 2247 7261 6e74 2041  ", [nlp("Grant A
-00002100: 6e64 6572 7365 6e22 295d 2c20 6b77 6172  ndersen")], kwar
-00002110: 6773 3d5b 7b22 6675 7a7a 795f 6675 6e63  gs=[{"fuzzy_func
-00002120: 223a 2022 746f 6b65 6e5f 736f 7274 227d  ": "token_sort"}
-00002130: 5d29 5c6e 6d61 7463 6865 7320 3d20 6d61  ])\nmatches = ma
-00002140: 7463 6865 7228 646f 6329 5c6e 5c6e 2320  tcher(doc)\n\n# 
-00002150: 5468 6520 6465 6661 756c 7420 6675 7a7a  The default fuzz
-00002160: 7920 6d61 7463 6869 6e67 2073 6574 7469  y matching setti
-00002170: 6e67 7320 7769 6c6c 206e 6f74 2066 696e  ngs will not fin
-00002180: 6420 6120 6d61 7463 682e 5c6e 666f 7220  d a match.\nfor 
-00002190: 6d61 7463 685f 6964 2c20 7374 6172 742c  match_id, start,
-000021a0: 2065 6e64 2c20 7261 7469 6f20 696e 206d   end, ratio in m
-000021b0: 6174 6368 6573 3a5c 6e20 2020 2070 7269  atches:\n    pri
-000021c0: 6e74 286d 6174 6368 5f69 642c 2064 6f63  nt(match_id, doc
-000021d0: 5b73 7461 7274 3a65 6e64 5d2c 2072 6174  [start:end], rat
-000021e0: 696f 295c 6e60 6060 5c6e 5c6e 2020 2020  io)\n```\n\n    
-000021f0: 4e41 4d45 2041 6e64 6572 736f 6e2c 2047  NAME Anderson, G
-00002200: 7269 6e74 2038 365c 6e5c 6e5c 6e54 6865  rint 86\n\n\nThe
-00002210: 2066 756c 6c20 6c69 7374 206f 6620 6b65   full list of ke
-00002220: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00002230: 6176 6169 6c61 626c 6520 666f 7220 6675  available for fu
-00002240: 7a7a 7920 6d61 7463 6869 6e67 2072 756c  zzy matching rul
-00002250: 6573 2069 6e63 6c75 6465 733a 5c6e 5c6e  es includes:\n\n
-00002260: 2d20 6066 757a 7a79 5f66 756e 6360 3a20  - `fuzzy_func`: 
-00002270: 4b65 7920 6e61 6d65 206f 6620 6675 7a7a  Key name of fuzz
-00002280: 7920 6d61 7463 6869 6e67 2066 756e 6374  y matching funct
-00002290: 696f 6e20 746f 2075 7365 2e20 416c 6c20  ion to use. All 
-000022a0: 7261 7069 6466 757a 7a20 6d61 7463 6869  rapidfuzz matchi
-000022b0: 6e67 2066 756e 6374 696f 6e73 2077 6974  ng functions wit
-000022c0: 6820 6465 6661 756c 7420 7365 7474 696e  h default settin
-000022d0: 6773 2061 7265 2061 7661 696c 6162 6c65  gs are available
-000022e0: 2e20 4465 6661 756c 7420 6973 2060 2273  . Default is `"s
-000022f0: 696d 706c 6522 603a 5c6e 2020 2020 2d20  imple"`:\n    - 
-00002300: 2273 696d 706c 6522 203d 2060 7261 7469  "simple" = `rati
-00002310: 6f60 5c6e 2020 2020 2d20 2270 6172 7469  o`\n    - "parti
-00002320: 616c 2220 3d20 6070 6172 7469 616c 5f72  al" = `partial_r
-00002330: 6174 696f 605c 6e20 2020 202d 2022 746f  atio`\n    - "to
-00002340: 6b65 6e5f 7365 7422 203d 2060 746f 6b65  ken_set" = `toke
-00002350: 6e5f 7365 745f 7261 7469 6f60 5c6e 2020  n_set_ratio`\n  
-00002360: 2020 2d20 2274 6f6b 656e 5f73 6f72 7422    - "token_sort"
-00002370: 203d 2060 746f 6b65 6e5f 736f 7274 5f72   = `token_sort_r
-00002380: 6174 696f 605c 6e20 2020 202d 2022 7061  atio`\n    - "pa
-00002390: 7274 6961 6c5f 746f 6b65 6e5f 7365 7422  rtial_token_set"
-000023a0: 203d 2060 7061 7274 6961 6c5f 746f 6b65   = `partial_toke
-000023b0: 6e5f 7365 745f 7261 7469 6f60 5c6e 2020  n_set_ratio`\n  
-000023c0: 2020 2d20 2270 6172 7469 616c 5f74 6f6b    - "partial_tok
-000023d0: 656e 5f73 6f72 7422 203d 2060 7061 7274  en_sort" = `part
-000023e0: 6961 6c5f 746f 6b65 6e5f 736f 7274 5f72  ial_token_sort_r
-000023f0: 6174 696f 605c 6e20 2020 202d 2022 7175  atio`\n    - "qu
-00002400: 6963 6b22 203d 2060 5152 6174 696f 605c  ick" = `QRatio`\
-00002410: 6e20 2020 202d 2022 7765 6967 6874 6564  n    - "weighted
-00002420: 2220 3d20 6057 5261 7469 6f60 5c6e 2020  " = `WRatio`\n  
-00002430: 2020 2d20 2274 6f6b 656e 2220 3d20 6074    - "token" = `t
-00002440: 6f6b 656e 5f72 6174 696f 602c 5c6e 2020  oken_ratio`,\n  
-00002450: 2020 2d20 2270 6172 7469 616c 5f74 6f6b    - "partial_tok
-00002460: 656e 2220 3d20 6070 6172 7469 616c 5f74  en" = `partial_t
-00002470: 6f6b 656e 5f72 6174 696f 605c 6e20 2020  oken_ratio`\n   
-00002480: 202d 2044 6566 6175 6c74 2069 7320 6022   - Default is `"
-00002490: 7369 6d70 6c65 2260 2e5c 6e2d 2060 6967  simple"`.\n- `ig
-000024a0: 6e6f 7265 5f63 6173 6560 3a20 4966 2073  nore_case`: If s
-000024b0: 7472 696e 6773 2073 686f 756c 6420 6265  trings should be
-000024c0: 206c 6f77 6572 2d63 6173 6564 2062 6566   lower-cased bef
-000024d0: 6f72 6520 636f 6d70 6172 6973 6f6e 206f  ore comparison o
-000024e0: 7220 6e6f 742e 2044 6566 6175 6c74 2069  r not. Default i
-000024f0: 7320 6054 7275 6560 2e5c 6e2d 2060 666c  s `True`.\n- `fl
-00002500: 6578 603a 204e 756d 6265 7220 6f66 2074  ex`: Number of t
-00002510: 6f6b 656e 7320 746f 206d 6f76 6520 6d61  okens to move ma
-00002520: 7463 6820 6d61 7463 6820 626f 756e 6461  tch match bounda
-00002530: 7269 6573 206c 6566 7420 616e 6420 7269  ries left and ri
-00002540: 6768 7420 6475 7269 6e67 206f 7074 696d  ght during optim
-00002550: 697a 6174 696f 6e2e 2043 616e 2062 6520  ization. Can be 
-00002560: 616e 2069 6e74 6567 6572 2076 616c 7565  an integer value
-00002570: 2077 6974 6820 6120 6d61 7820 6f66 2060   with a max of `
-00002580: 6c65 6e28 7175 6572 7929 6020 616e 6420  len(query)` and 
-00002590: 6120 6d69 6e20 6f66 2060 3060 2028 7769  a min of `0` (wi
-000025a0: 6c6c 2077 6172 6e20 616e 6420 6368 616e  ll warn and chan
-000025b0: 6765 2069 6620 6869 6768 6572 206f 7220  ge if higher or 
-000025c0: 6c6f 7765 7229 2c6f 7220 7468 6520 7374  lower),or the st
-000025d0: 7269 6e67 7320 226d 6178 222c 2022 6d69  rings "max", "mi
-000025e0: 6e22 2c20 6f72 2022 6465 6661 756c 7422  n", or "default"
-000025f0: 2e20 4465 6661 756c 7420 6973 2060 2264  . Default is `"d
-00002600: 6566 6175 6c74 2260 3a20 606c 656e 2871  efault"`: `len(q
-00002610: 7565 7279 2920 2f2f 2032 602e 5c6e 2d20  uery) // 2`.\n- 
-00002620: 606d 696e 5f72 3160 3a20 4d69 6e69 6d75  `min_r1`: Minimu
-00002630: 6d20 6d61 7463 6820 7261 7469 6f20 7265  m match ratio re
-00002640: 7175 6972 6564 2066 6f72 7365 6c65 6374  quired forselect
-00002650: 696f 6e20 6475 7269 6e67 2074 6865 2069  ion during the i
-00002660: 6e74 6961 6c20 7365 6172 6368 206f 7665  ntial search ove
-00002670: 7220 646f 632e 2049 6620 6066 6c65 7820  r doc. If `flex 
-00002680: 3d3d 2030 602c 2060 6d69 6e5f 7231 6020  == 0`, `min_r1` 
-00002690: 7769 6c6c 2062 6520 6f76 6572 7772 6974  will be overwrit
-000026a0: 7465 6e20 6279 2060 6d69 6e5f 7232 602e  ten by `min_r2`.
-000026b0: 2049 6620 6066 6c65 7820 3e20 3060 2c20   If `flex > 0`, 
-000026c0: 606d 696e 5f72 3160 206d 7573 7420 6265  `min_r1` must be
-000026d0: 206c 6f77 6572 2074 6861 6e20 606d 696e   lower than `min
-000026e0: 5f72 3260 2061 6e64 2022 6c6f 7722 2069  _r2` and "low" i
-000026f0: 6e20 6765 6e65 7261 6c20 6265 6361 7573  n general becaus
-00002700: 6520 6d61 7463 6820 626f 756e 6461 7269  e match boundari
-00002710: 6573 2061 7265 206e 6f74 2066 6c65 7865  es are not flexe
-00002720: 6420 696e 6974 6961 6c6c 792e 2044 6566  d initially. Def
-00002730: 6175 6c74 2069 7320 6035 3060 2e5c 6e2d  ault is `50`.\n-
-00002740: 2060 6d69 6e5f 7232 603a 204d 696e 696d   `min_r2`: Minim
-00002750: 756d 206d 6174 6368 2072 6174 696f 2072  um match ratio r
-00002760: 6571 7569 7265 6420 666f 7220 7365 6c65  equired for sele
-00002770: 6374 696f 6e20 6475 7269 6e67 206d 6174  ction during mat
-00002780: 6368 206f 7074 696d 697a 6174 696f 6e2e  ch optimization.
-00002790: 204e 6565 6473 2074 6f20 6265 2068 6967   Needs to be hig
-000027a0: 6865 7220 7468 616e 2060 6d69 6e5f 7231  her than `min_r1
-000027b0: 6020 616e 6420 2268 6967 6822 2069 6e20  ` and "high" in 
-000027c0: 6765 6e65 7261 6c20 746f 2065 6e73 7572  general to ensur
-000027d0: 6520 6f6e 6c79 2071 7561 6c69 7479 206d  e only quality m
-000027e0: 6174 6368 6573 2061 7265 2072 6574 7572  atches are retur
-000027f0: 6e65 642e 2044 6566 6175 6c74 2069 7320  ned. Default is 
-00002800: 6037 3560 2e5c 6e2d 2060 7468 7265 7368  `75`.\n- `thresh
-00002810: 603a 2049 6620 7468 6973 2072 6174 696f  `: If this ratio
-00002820: 2069 7320 6578 6365 6564 6564 2069 6e20   is exceeded in 
-00002830: 696e 6974 6961 6c20 7363 616e 2c20 616e  initial scan, an
-00002840: 6420 6066 6c65 7820 3e20 3060 2c20 6e6f  d `flex > 0`, no
-00002850: 206f 7074 696d 697a 6174 696f 6e20 7769   optimization wi
-00002860: 6c6c 2062 6520 6174 7465 6d70 7465 642e  ll be attempted.
-00002870: 2049 6620 6066 6c65 7820 3d3d 2030 602c   If `flex == 0`,
-00002880: 2060 7468 7265 7368 6020 6861 7320 6e6f   `thresh` has no
-00002890: 2065 6666 6563 742e 2044 6566 6175 6c74   effect. Default
-000028a0: 2069 7320 6031 3030 602e 5c6e 5c6e 2323   is `100`.\n\n##
-000028b0: 2320 5265 6765 784d 6174 6368 6572 5c6e  # RegexMatcher\n
-000028c0: 5c6e 5468 6520 6261 7369 6320 7573 6167  \nThe basic usag
-000028d0: 6520 6f66 2074 6865 2072 6567 6578 206d  e of the regex m
-000028e0: 6174 6368 6572 2069 7320 616c 736f 2066  atcher is also f
-000028f0: 6169 726c 7920 7369 6d69 6c61 7220 746f  airly similar to
-00002900: 2073 7061 4379 5c27 7320 6050 6872 6173   spaCy\'s `Phras
-00002910: 654d 6174 6368 6572 602e 2049 7420 6163  eMatcher`. It ac
-00002920: 6365 7074 7320 7265 6765 7820 7061 7474  cepts regex patt
-00002930: 6572 6e73 2061 7320 7374 7269 6e67 7320  erns as strings 
-00002940: 736f 2066 6c61 6773 206d 7573 7420 6265  so flags must be
-00002950: 2069 6e6c 696e 652e 2052 6567 6578 6573   inline. Regexes
-00002960: 2061 7265 2063 6f6d 7069 6c65 6420 7769   are compiled wi
-00002970: 7468 2074 6865 205b 7265 6765 785d 2868  th the [regex](h
-00002980: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00002990: 7072 6f6a 6563 742f 7265 6765 782f 2920  project/regex/) 
-000029a0: 7061 636b 6167 6520 736f 2061 7070 726f  package so appro
-000029b0: 7869 6d61 7465 2022 6675 7a7a 7922 206d  ximate "fuzzy" m
-000029c0: 6174 6368 696e 6720 6973 2073 7570 706f  atching is suppo
-000029d0: 7274 6564 2e20 546f 2070 726f 7669 6465  rted. To provide
-000029e0: 2061 6363 6573 7320 746f 2074 6865 7365   access to these
-000029f0: 2022 6675 7a7a 7922 206d 6174 6368 2072   "fuzzy" match r
-00002a00: 6573 756c 7473 2074 6865 206d 6174 6368  esults the match
-00002a10: 6572 2072 6574 7572 6e73 2074 6865 2066  er returns the f
-00002a20: 757a 7a79 2063 6f75 6e74 2076 616c 7565  uzzy count value
-00002a30: 7320 616c 6f6e 6720 7769 7468 206d 6174  s along with mat
-00002a40: 6368 2069 642c 2073 7461 7274 2061 6e64  ch id, start and
-00002a50: 2065 6e64 2069 6e66 6f72 6d61 7469 6f6e   end information
-00002a60: 2c20 736f 206d 616b 6520 7375 7265 2074  , so make sure t
-00002a70: 6f20 696e 636c 7564 6520 6120 7661 7269  o include a vari
-00002a80: 6162 6c65 2066 6f72 2074 6865 2063 6f75  able for the cou
-00002a90: 6e74 7320 7768 656e 2075 6e70 6163 6b69  nts when unpacki
-00002aa0: 6e67 2072 6573 756c 7473 2e5c 6e5c 6e5c  ng results.\n\n\
-00002ab0: 6e60 6060 7079 7468 6f6e 5c6e 696d 706f  n```python\nimpo
-00002ac0: 7274 2073 7061 6379 5c6e 6672 6f6d 2073  rt spacy\nfrom s
-00002ad0: 7061 637a 7a2e 6d61 7463 6865 7220 696d  paczz.matcher im
-00002ae0: 706f 7274 2052 6567 6578 4d61 7463 6865  port RegexMatche
-00002af0: 725c 6e5c 6e6e 6c70 203d 2073 7061 6379  r\n\nnlp = spacy
-00002b00: 2e62 6c61 6e6b 2822 656e 2229 5c6e 7465  .blank("en")\nte
-00002b10: 7874 203d 2022 2222 416e 6465 7273 6f6e  xt = """Anderson
-00002b20: 2c20 4772 696e 7420 6372 6561 7465 6420  , Grint created 
-00002b30: 7370 6163 7a7a 2069 6e20 6869 7320 686f  spaczz in his ho
-00002b40: 6d65 2061 7420 3535 3520 4661 6b65 2053  me at 555 Fake S
-00002b50: 742c 5c6e 4170 7420 3520 696e 204e 6173  t,\nApt 5 in Nas
-00002b60: 6876 316c 652c 2054 4e20 3535 3535 352d  hv1le, TN 55555-
-00002b70: 3132 3334 2069 6e20 7468 6520 5553 2e22  1234 in the US."
-00002b80: 2222 2020 2320 5370 656c 6c69 6e67 2065  ""  # Spelling e
-00002b90: 7272 6f72 7320 696e 7465 6e74 696f 6e61  rrors intentiona
-00002ba0: 6c2e 5c6e 646f 6320 3d20 6e6c 7028 7465  l.\ndoc = nlp(te
-00002bb0: 7874 295c 6e5c 6e6d 6174 6368 6572 203d  xt)\n\nmatcher =
-00002bc0: 2052 6567 6578 4d61 7463 6865 7228 6e6c   RegexMatcher(nl
-00002bd0: 702e 766f 6361 6229 5c6e 2320 5573 6520  p.vocab)\n# Use 
-00002be0: 696e 6c69 6e65 2066 6c61 6773 2066 6f72  inline flags for
-00002bf0: 2072 6567 6578 2073 7472 696e 6773 2061   regex strings a
-00002c00: 7320 6e65 6564 6564 5c6e 6d61 7463 6865  s needed\nmatche
-00002c10: 722e 6164 6428 5c6e 2020 2020 2241 5054  r.add(\n    "APT
-00002c20: 222c 5c6e 2020 2020 5b5c 6e20 2020 2020  ",\n    [\n     
-00002c30: 2020 2072 2222 2228 3f69 7829 2828 3f3a     r"""(?ix)((?:
-00002c40: 6170 6172 746d 656e 747c 6170 747c 6275  apartment|apt|bu
-00002c50: 696c 6469 6e67 7c62 6c64 677c 666c 6f6f  ilding|bldg|floo
-00002c60: 727c 666c 7c73 7569 7465 7c73 7465 7c75  r|fl|suite|ste|u
-00002c70: 6e69 745c 6e7c 726f 6f6d 7c72 6d7c 6465  nit\n|room|rm|de
-00002c80: 7061 7274 6d65 6e74 7c64 6570 747c 726f  partment|dept|ro
-00002c90: 777c 7277 295c 5c2e 3f5c 5c73 3f29 233f  w|rw)\\.?\\s?)#?
-00002ca0: 5c5c 647b 312c 347d 5b61 2d7a 5d3f 2222  \\d{1,4}[a-z]?""
-00002cb0: 225c 6e20 2020 205d 2c5c 6e29 2020 2320  "\n    ],\n)  # 
-00002cc0: 4e6f 7420 7468 6520 6d6f 7374 2072 6f62  Not the most rob
-00002cd0: 7573 7420 7265 6765 782e 5c6e 6d61 7463  ust regex.\nmatc
-00002ce0: 6865 722e 6164 6428 2247 5045 222c 205b  her.add("GPE", [
-00002cf0: 7222 2855 5341 297b 643c 3d31 7d22 5d29  r"(USA){d<=1}"])
-00002d00: 2020 2320 4675 7a7a 7920 7265 6765 782e    # Fuzzy regex.
-00002d10: 5c6e 6d61 7463 6865 7320 3d20 6d61 7463  \nmatches = matc
-00002d20: 6865 7228 646f 6329 5c6e 5c6e 666f 7220  her(doc)\n\nfor 
-00002d30: 6d61 7463 685f 6964 2c20 7374 6172 742c  match_id, start,
-00002d40: 2065 6e64 2c20 636f 756e 7473 2069 6e20   end, counts in 
-00002d50: 6d61 7463 6865 733a 5c6e 2020 2020 7072  matches:\n    pr
-00002d60: 696e 7428 6d61 7463 685f 6964 2c20 646f  int(match_id, do
-00002d70: 635b 7374 6172 743a 656e 645d 2c20 636f  c[start:end], co
-00002d80: 756e 7473 295c 6e60 6060 5c6e 5c6e 2020  unts)\n```\n\n  
-00002d90: 2020 4150 5420 4170 7420 3520 2830 2c20    APT Apt 5 (0, 
-00002da0: 302c 2030 295c 6e20 2020 2047 5045 2055  0, 0)\n    GPE U
-00002db0: 5320 2830 2c20 302c 2031 295c 6e5c 6e5c  S (0, 0, 1)\n\n\
-00002dc0: 6e53 7061 637a 7a20 6d61 7463 6865 7273  nSpaczz matchers
-00002dd0: 2063 616e 2061 6c73 6f20 6d61 6b65 2075   can also make u
-00002de0: 7365 206f 6620 6f6e 2d6d 6174 6368 2072  se of on-match r
-00002df0: 756c 6573 2076 6961 2063 616c 6c62 6163  ules via callbac
-00002e00: 6b20 6675 6e63 7469 6f6e 732e 2054 6865  k functions. The
-00002e10: 7365 206f 6e2d 6d61 7463 6820 6361 6c6c  se on-match call
-00002e20: 6261 636b 7320 6e65 6564 2074 6f20 6163  backs need to ac
-00002e30: 6365 7074 2074 6865 206d 6174 6368 6572  cept the matcher
-00002e40: 2069 7473 656c 662c 2074 6865 2064 6f63   itself, the doc
-00002e50: 2074 6865 206d 6174 6368 6572 2077 6173   the matcher was
-00002e60: 2063 616c 6c65 6420 6f6e 2c20 7468 6520   called on, the 
-00002e70: 6d61 7463 6820 696e 6465 7820 616e 6420  match index and 
-00002e80: 7468 6520 6d61 7463 6865 7320 7072 6f64  the matches prod
-00002e90: 7563 6564 2062 7920 7468 6520 6d61 7463  uced by the matc
-00002ea0: 6865 722e 2053 6565 2074 6865 2066 757a  her. See the fuz
-00002eb0: 7a79 206d 6174 6368 6572 2075 7361 6765  zy matcher usage
-00002ec0: 2065 7861 6d70 6c65 2061 626f 7665 2066   example above f
-00002ed0: 6f72 2064 6574 6169 6c73 2e5c 6e5c 6e4c  or details.\n\nL
-00002ee0: 696b 6520 7468 6520 6675 7a7a 7920 6d61  ike the fuzzy ma
-00002ef0: 7463 6865 722c 2074 6865 2072 6567 6578  tcher, the regex
-00002f00: 206d 6174 6368 6572 2068 6173 206f 7074   matcher has opt
-00002f10: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
-00002f20: 6775 6d65 6e74 7320 7468 6174 2063 616e  guments that can
-00002f30: 206d 6f64 6966 7920 6d61 7463 6869 6e67   modify matching
-00002f40: 2062 6568 6176 696f 722e 2054 616b 6520   behavior. Take 
-00002f50: 7468 6520 6265 6c6f 7720 7265 6765 7820  the below regex 
-00002f60: 6d61 7463 6869 6e67 2065 7861 6d70 6c65  matching example
-00002f70: 2e5c 6e5c 6e5c 6e60 6060 7079 7468 6f6e  .\n\n\n```python
-00002f80: 5c6e 696d 706f 7274 2073 7061 6379 5c6e  \nimport spacy\n
-00002f90: 6672 6f6d 2073 7061 637a 7a2e 6d61 7463  from spaczz.matc
-00002fa0: 6865 7220 696d 706f 7274 2052 6567 6578  her import Regex
-00002fb0: 4d61 7463 6865 725c 6e5c 6e6e 6c70 203d  Matcher\n\nnlp =
-00002fc0: 2073 7061 6379 2e62 6c61 6e6b 2822 656e   spacy.blank("en
-00002fd0: 2229 5c6e 7465 7874 203d 2022 2222 416e  ")\ntext = """An
-00002fe0: 6465 7273 6f6e 2c20 4772 696e 7420 6372  derson, Grint cr
-00002ff0: 6561 7465 6420 7370 6163 7a7a 2069 6e20  eated spaczz in 
-00003000: 6869 7320 686f 6d65 2061 7420 3535 3520  his home at 555 
-00003010: 4661 6b65 2053 742c 5c6e 4170 7420 3520  Fake St,\nApt 5 
-00003020: 696e 204e 6173 6876 316c 652c 2054 4e20  in Nashv1le, TN 
-00003030: 3535 3535 352d 3132 3334 2069 6e20 7468  55555-1234 in th
-00003040: 6520 5553 412e 2222 2220 2023 2053 7065  e USA."""  # Spe
-00003050: 6c6c 696e 6720 6572 726f 7273 2069 6e74  lling errors int
-00003060: 656e 7469 6f6e 616c 2e20 4e6f 7469 6365  entional. Notice
-00003070: 205c 2755 5341 5c27 2068 6572 652e 5c6e   \'USA\' here.\n
-00003080: 646f 6320 3d20 6e6c 7028 7465 7874 295c  doc = nlp(text)\
-00003090: 6e5c 6e6d 6174 6368 6572 203d 2052 6567  n\nmatcher = Reg
-000030a0: 6578 4d61 7463 6865 7228 6e6c 702e 766f  exMatcher(nlp.vo
-000030b0: 6361 6229 5c6e 2320 5573 6520 696e 6c69  cab)\n# Use inli
-000030c0: 6e65 2066 6c61 6773 2066 6f72 2072 6567  ne flags for reg
-000030d0: 6578 2073 7472 696e 6773 2061 7320 6e65  ex strings as ne
-000030e0: 6564 6564 5c6e 6d61 7463 6865 722e 6164  eded\nmatcher.ad
-000030f0: 6428 5c6e 2020 2020 2253 5452 4545 5422  d(\n    "STREET"
-00003100: 2c20 5b22 7374 7265 6574 5f61 6464 7265  , ["street_addre
-00003110: 7373 6573 225d 2c20 6b77 6172 6773 3d5b  sses"], kwargs=[
-00003120: 7b22 7072 6564 6566 223a 2054 7275 657d  {"predef": True}
-00003130: 5d5c 6e29 2020 2320 5573 6520 7072 6564  ]\n)  # Use pred
-00003140: 6566 696e 6564 2072 6567 6578 2062 7920  efined regex by 
-00003150: 6b65 7920 6e61 6d65 2e5c 6e23 2042 656c  key name.\n# Bel
-00003160: 6f77 2077 696c 6c20 6e6f 7420 6578 7061  ow will not expa
-00003170: 6e64 2070 6172 7469 616c 206d 6174 6368  nd partial match
-00003180: 6573 2074 6f20 7370 616e 2062 6f75 6e64  es to span bound
-00003190: 6172 6965 732e 5c6e 6d61 7463 6865 722e  aries.\nmatcher.
-000031a0: 6164 6428 2247 5045 222c 205b 7222 283f  add("GPE", [r"(?
-000031b0: 6929 5b55 5d28 6e69 7465 647c 5c5c 2e3f  i)[U](nited|\\.?
-000031c0: 2920 3f5b 535d 2874 6174 6573 7c5c 5c2e  ) ?[S](tates|\\.
-000031d0: 3f29 225d 2c20 6b77 6172 6773 3d5b 7b22  ?)"], kwargs=[{"
-000031e0: 7061 7274 6961 6c22 3a20 4661 6c73 657d  partial": False}
-000031f0: 5d29 5c6e 6d61 7463 6865 7320 3d20 6d61  ])\nmatches = ma
-00003200: 7463 6865 7228 646f 6329 5c6e 5c6e 666f  tcher(doc)\n\nfo
-00003210: 7220 6d61 7463 685f 6964 2c20 7374 6172  r match_id, star
-00003220: 742c 2065 6e64 2c20 636f 756e 7473 2069  t, end, counts i
-00003230: 6e20 6d61 7463 6865 733a 5c6e 2020 2020  n matches:\n    
-00003240: 7072 696e 7428 5c6e 2020 2020 2020 2020  print(\n        
-00003250: 6d61 7463 685f 6964 2c20 646f 635b 7374  match_id, doc[st
-00003260: 6172 743a 656e 645d 2c20 636f 756e 7473  art:end], counts
-00003270: 5c6e 2020 2020 2920 2023 2063 6f6d 6d61  \n    )  # comma
-00003280: 2069 6e20 7265 7375 6c74 2069 736e 5c27   in result isn\'
-00003290: 7420 6964 6561 6c20 2d20 7365 6520 2252  t ideal - see "R
-000032a0: 6f61 646d 6170 225c 6e60 6060 5c6e 5c6e  oadmap"\n```\n\n
-000032b0: 2020 2020 5354 5245 4554 2035 3535 2046      STREET 555 F
-000032c0: 616b 6520 5374 2c20 2830 2c20 302c 2030  ake St, (0, 0, 0
-000032d0: 295c 6e5c 6e5c 6e54 6865 2066 756c 6c20  )\n\n\nThe full 
-000032e0: 6c69 7374 206f 6620 6b65 7977 6f72 6420  list of keyword 
-000032f0: 6172 6775 6d65 6e74 7320 6176 6169 6c61  arguments availa
-00003300: 626c 6520 666f 7220 7265 6765 7820 6d61  ble for regex ma
-00003310: 7463 6869 6e67 2072 756c 6573 2069 6e63  tching rules inc
-00003320: 6c75 6465 733a 5c6e 5c6e 2d20 6070 6172  ludes:\n\n- `par
-00003330: 7469 616c 603a 2057 6865 7468 6572 2070  tial`: Whether p
-00003340: 6172 7469 616c 206d 6174 6368 6573 2073  artial matches s
-00003350: 686f 756c 6420 6265 2065 7874 656e 6465  hould be extende
-00003360: 6420 746f 2065 7869 7374 696e 6720 7370  d to existing sp
-00003370: 616e 2062 6f75 6e64 6172 6965 7320 696e  an boundaries in
-00003380: 2064 6f63 206f 7220 6e6f 742c 2069 2e65   doc or not, i.e
-00003390: 2e20 7468 6520 7265 6765 7820 6f6e 6c79  . the regex only
-000033a0: 206d 6174 6368 6573 2070 6172 7420 6f66   matches part of
-000033b0: 2061 2074 6f6b 656e 206f 7220 7370 616e   a token or span
-000033c0: 2e20 4465 6661 756c 7420 6973 2054 7275  . Default is Tru
-000033d0: 652e 5c6e 2d20 6070 7265 6465 6660 3a20  e.\n- `predef`: 
-000033e0: 5768 6574 6865 7220 7468 6520 7265 6765  Whether the rege
-000033f0: 7820 7374 7269 6e67 2073 686f 756c 6420  x string should 
-00003400: 6265 2069 6e74 6572 7072 6574 6564 2061  be interpreted a
-00003410: 7320 6120 6b65 7920 746f 2061 2070 7265  s a key to a pre
-00003420: 6465 6669 6e65 6420 7265 6765 7820 7061  defined regex pa
-00003430: 7474 6572 6e20 6f72 206e 6f74 2e20 4465  ttern or not. De
-00003440: 6661 756c 7420 6973 2046 616c 7365 2e20  fault is False. 
-00003450: 5468 6520 696e 636c 7564 6564 2072 6567  The included reg
-00003460: 6578 6573 2061 7265 3a5c 6e20 2020 202d  exes are:\n    -
-00003470: 2060 2264 6174 6573 2260 5c6e 2020 2020   `"dates"`\n    
-00003480: 2d20 6022 7469 6d65 7322 605c 6e20 2020  - `"times"`\n   
-00003490: 202d 2060 2270 686f 6e65 7322 605c 6e20   - `"phones"`\n 
-000034a0: 2020 202d 2060 2270 686f 6e65 735f 7769     - `"phones_wi
-000034b0: 7468 5f65 7874 7322 605c 6e20 2020 202d  th_exts"`\n    -
-000034c0: 2060 226c 696e 6b73 2260 5c6e 2020 2020   `"links"`\n    
-000034d0: 2d20 6022 656d 6169 6c73 2260 5c6e 2020  - `"emails"`\n  
-000034e0: 2020 2d20 6022 6970 7322 605c 6e20 2020    - `"ips"`\n   
-000034f0: 202d 2060 2269 7076 3673 2260 5c6e 2020   - `"ipv6s"`\n  
-00003500: 2020 2d20 6022 7072 6963 6573 2260 5c6e    - `"prices"`\n
-00003510: 2020 2020 2d20 6022 6865 785f 636f 6c6f      - `"hex_colo
-00003520: 7273 2260 5c6e 2020 2020 2d20 6022 6372  rs"`\n    - `"cr
-00003530: 6564 6974 5f63 6172 6473 2260 5c6e 2020  edit_cards"`\n  
-00003540: 2020 2d20 6022 6274 635f 6164 6472 6573    - `"btc_addres
-00003550: 7365 7322 605c 6e20 2020 202d 2060 2273  ses"`\n    - `"s
-00003560: 7472 6565 745f 6164 6472 6573 7365 7322  treet_addresses"
-00003570: 605c 6e20 2020 202d 2060 227a 6970 5f63  `\n    - `"zip_c
-00003580: 6f64 6573 2260 5c6e 2020 2020 2d20 6022  odes"`\n    - `"
-00003590: 706f 5f62 6f78 6573 2260 5c6e 2020 2020  po_boxes"`\n    
-000035a0: 2d20 6022 7373 6e5f 6e75 6d62 6572 2260  - `"ssn_number"`
-000035b0: 5c6e 5c6e 5468 6520 6162 6f76 6520 7061  \n\nThe above pa
-000035c0: 7474 6572 6e73 2061 7265 2074 6865 2073  tterns are the s
-000035d0: 616d 6520 7468 6174 2074 6865 205b 636f  ame that the [co
-000035e0: 6d6d 6f6e 7265 6765 785d 2868 7474 7073  mmonregex](https
-000035f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
-00003600: 6469 736f 6e6d 6179 2f43 6f6d 6d6f 6e52  disonmay/CommonR
-00003610: 6567 6578 2920 7061 636b 6167 6520 7072  egex) package pr
-00003620: 6f76 6964 6573 2e5c 6e5c 6e23 2323 2053  ovides.\n\n### S
-00003630: 696d 696c 6172 6974 794d 6174 6368 6572  imilarityMatcher
-00003640: 5c6e 5c6e 5468 6520 6261 7369 6320 7573  \n\nThe basic us
-00003650: 6167 6520 6f66 2074 6865 2073 696d 696c  age of the simil
-00003660: 6172 6974 7920 6d61 7463 6865 7220 6973  arity matcher is
-00003670: 2073 696d 696c 6172 2074 6f20 7370 6143   similar to spaC
-00003680: 795c 2773 2060 5068 7261 7365 4d61 7463  y\'s `PhraseMatc
-00003690: 6865 7260 2065 7863 6570 7420 6974 2072  her` except it r
-000036a0: 6574 7572 6e73 2074 6865 2076 6563 746f  eturns the vecto
-000036b0: 7220 7369 6d69 6c61 7269 7479 2072 6174  r similarity rat
-000036c0: 696f 2061 6c6f 6e67 2077 6974 6820 6d61  io along with ma
-000036d0: 7463 6820 6964 2c20 7374 6172 7420 616e  tch id, start an
-000036e0: 6420 656e 6420 696e 666f 726d 6174 696f  d end informatio
-000036f0: 6e2c 2073 6f20 6d61 6b65 2073 7572 6520  n, so make sure 
-00003700: 746f 2069 6e63 6c75 6465 2061 2076 6172  to include a var
-00003710: 6961 626c 6520 666f 7220 7468 6520 7261  iable for the ra
-00003720: 7469 6f20 7768 656e 2075 6e70 6163 6b69  tio when unpacki
-00003730: 6e67 2072 6573 756c 7473 2e5c 6e5c 6e49  ng results.\n\nI
-00003740: 6e20 6f72 6465 7220 746f 2070 726f 6475  n order to produ
-00003750: 6365 206d 6561 6e69 6e67 6675 6c20 7265  ce meaningful re
-00003760: 7375 6c74 7320 6672 6f6d 2074 6865 2073  sults from the s
-00003770: 696d 696c 6172 6974 7920 6d61 7463 6865  imilarity matche
-00003780: 722c 2061 2073 7061 4379 206d 6f64 656c  r, a spaCy model
-00003790: 2077 6974 6820 776f 7264 2076 6563 746f   with word vecto
-000037a0: 7273 2028 6578 2e20 6d65 6469 756d 206f  rs (ex. medium o
-000037b0: 7220 6c61 7267 6520 456e 676c 6973 6820  r large English 
-000037c0: 6d6f 6465 6c73 2920 6d75 7374 2062 6520  models) must be 
-000037d0: 7573 6564 2074 6f20 696e 6974 6961 6c69  used to initiali
-000037e0: 7a65 2074 6865 206d 6174 6368 6572 2c20  ze the matcher, 
-000037f0: 7072 6f63 6573 7320 7468 6520 7461 7267  process the targ
-00003800: 6574 2064 6f63 756d 656e 742c 2061 6e64  et document, and
-00003810: 2070 726f 6365 7373 2061 6e79 2070 6174   process any pat
-00003820: 7465 726e 7320 6164 6465 642e 5c6e 5c6e  terns added.\n\n
-00003830: 5c6e 6060 6070 7974 686f 6e5c 6e69 6d70  \n```python\nimp
-00003840: 6f72 7420 7370 6163 795c 6e66 726f 6d20  ort spacy\nfrom 
-00003850: 7370 6163 7a7a 2e6d 6174 6368 6572 2069  spaczz.matcher i
-00003860: 6d70 6f72 7420 5369 6d69 6c61 7269 7479  mport Similarity
-00003870: 4d61 7463 6865 725c 6e5c 6e6e 6c70 203d  Matcher\n\nnlp =
-00003880: 2073 7061 6379 2e6c 6f61 6428 2265 6e5f   spacy.load("en_
-00003890: 636f 7265 5f77 6562 5f6d 6422 295c 6e74  core_web_md")\nt
-000038a0: 6578 7420 3d20 2249 206c 696b 6520 6170  ext = "I like ap
-000038b0: 706c 6573 2c20 6772 6170 6573 2061 6e64  ples, grapes and
-000038c0: 2062 616e 616e 6173 2e22 5c6e 646f 6320   bananas."\ndoc 
-000038d0: 3d20 6e6c 7028 7465 7874 295c 6e5c 6e23  = nlp(text)\n\n#
-000038e0: 206c 6f77 6572 696e 6720 6d69 6e5f 7232   lowering min_r2
-000038f0: 2066 726f 6d20 6465 6661 756c 7420 6f66   from default of
-00003900: 2037 3520 746f 2070 726f 6475 6365 206d   75 to produce m
-00003910: 6174 6368 6573 2069 6e20 7468 6973 2065  atches in this e
-00003920: 7861 6d70 6c65 5c6e 6d61 7463 6865 7220  xample\nmatcher 
-00003930: 3d20 5369 6d69 6c61 7269 7479 4d61 7463  = SimilarityMatc
-00003940: 6865 7228 6e6c 702e 766f 6361 622c 206d  her(nlp.vocab, m
-00003950: 696e 5f72 323d 3635 295c 6e6d 6174 6368  in_r2=65)\nmatch
-00003960: 6572 2e61 6464 2822 4652 5549 5422 2c20  er.add("FRUIT", 
-00003970: 5b6e 6c70 2822 6672 7569 7422 295d 295c  [nlp("fruit")])\
-00003980: 6e6d 6174 6368 6573 203d 206d 6174 6368  nmatches = match
-00003990: 6572 2864 6f63 295c 6e5c 6e66 6f72 206d  er(doc)\n\nfor m
-000039a0: 6174 6368 5f69 642c 2073 7461 7274 2c20  atch_id, start, 
-000039b0: 656e 642c 2072 6174 696f 2069 6e20 6d61  end, ratio in ma
-000039c0: 7463 6865 733a 5c6e 2020 2020 7072 696e  tches:\n    prin
-000039d0: 7428 6d61 7463 685f 6964 2c20 646f 635b  t(match_id, doc[
-000039e0: 7374 6172 743a 656e 645d 2c20 7261 7469  start:end], rati
-000039f0: 6f29 5c6e 6060 605c 6e5c 6e20 2020 2046  o)\n```\n\n    F
-00003a00: 5255 4954 2061 7070 6c65 7320 3732 5c6e  RUIT apples 72\n
-00003a10: 2020 2020 4652 5549 5420 6772 6170 6573      FRUIT grapes
-00003a20: 2037 325c 6e20 2020 2046 5255 4954 2062   72\n    FRUIT b
-00003a30: 616e 616e 6173 2036 385c 6e5c 6e5c 6e50  ananas 68\n\n\nP
-00003a40: 6c65 6173 6520 6e6f 7465 2074 6861 7420  lease note that 
-00003a50: 6576 656e 2066 6f72 2074 6865 206d 6f73  even for the mos
-00003a60: 746c 7920 7075 7265 2d50 7974 686f 6e20  tly pure-Python 
-00003a70: 7370 6163 7a7a 2c20 7468 6973 2070 726f  spaczz, this pro
-00003a80: 6365 7373 2069 7320 6375 7272 656e 746c  cess is currentl
-00003a90: 7920 6578 7472 656d 656c 7920 736c 6f77  y extremely slow
-00003aa0: 2073 6f20 6265 206d 696e 6466 756c 206f   so be mindful o
-00003ab0: 6620 7468 6520 7363 6f70 6520 696e 2077  f the scope in w
-00003ac0: 6869 6368 2069 7420 6973 2061 7070 6c69  hich it is appli
-00003ad0: 6564 2e20 456e 6162 6c69 6e67 2047 5055  ed. Enabling GPU
-00003ae0: 2073 7570 706f 7274 2069 6e20 7370 6143   support in spaC
-00003af0: 7920 285b 7365 6520 6865 7265 5d28 6874  y ([see here](ht
-00003b00: 7470 733a 2f2f 7370 6163 792e 696f 2f75  tps://spacy.io/u
-00003b10: 7361 6765 2367 7075 2929 2073 686f 756c  sage#gpu)) shoul
-00003b20: 6420 696d 7072 6f76 6520 7468 6520 7370  d improve the sp
-00003b30: 6565 6420 736f 6d65 7768 6174 2c20 6275  eed somewhat, bu
-00003b40: 7420 4920 6265 6c69 6576 6520 7468 6520  t I believe the 
-00003b50: 7072 6f63 6573 7320 7769 6c6c 2073 7469  process will sti
-00003b60: 6c6c 2062 6520 626f 7474 6c65 6e65 636b  ll be bottleneck
-00003b70: 6564 2069 6e20 7468 6520 7075 7265 2d50  ed in the pure-P
-00003b80: 7974 686f 6e20 7365 6172 6368 2061 6c67  ython search alg
-00003b90: 6f72 6974 686d 2075 6e74 696c 2049 2064  orithm until I d
-00003ba0: 6576 656c 6f70 2061 2062 6574 7465 7220  evelop a better 
-00003bb0: 7365 6172 6368 2061 6c67 6f72 6974 686d  search algorithm
-00003bc0: 2061 6e64 2f6f 7220 6472 6f70 2074 6865   and/or drop the
-00003bd0: 2073 6561 7263 6820 746f 206c 6f77 6572   search to lower
-00003be0: 2d6c 6576 656c 2063 6f64 6520 2865 7820  -level code (ex 
-00003bf0: 4329 2e5c 6e5c 6e41 6c73 6f20 6173 2061  C).\n\nAlso as a
-00003c00: 2073 6f6d 6577 6861 7420 6578 7065 7269   somewhat experi
-00003c10: 6d65 6e74 616c 2066 6561 7475 7265 2c20  mental feature, 
-00003c20: 7468 6520 7369 6d69 6c61 7269 7479 206d  the similarity m
-00003c30: 6174 6368 6572 2069 7320 6e6f 7420 6375  atcher is not cu
-00003c40: 7272 656e 746c 7920 7061 7274 206f 6620  rrently part of 
-00003c50: 7468 6520 6053 7061 637a 7a52 756c 6572  the `SpaczzRuler
-00003c60: 6020 6e6f 7220 646f 6573 2069 7420 6861  ` nor does it ha
-00003c70: 7665 2061 2073 6570 6172 6174 6520 7275  ve a separate ru
-00003c80: 6c65 722e 2049 6620 796f 7520 6e65 6564  ler. If you need
-00003c90: 2074 6f20 6164 6420 7369 6d69 6c61 7269   to add similari
-00003ca0: 7479 206d 6174 6368 6573 2074 6f20 6120  ty matches to a 
-00003cb0: 646f 635c 2773 2065 6e74 6974 6965 7320  doc\'s entities 
-00003cc0: 796f 7520 7769 6c6c 206e 6565 6420 746f  you will need to
-00003cd0: 2075 7365 2061 6e20 6f6e 2d6d 6174 6368   use an on-match
-00003ce0: 2063 616c 6c62 6163 6b20 666f 7220 7468   callback for th
-00003cf0: 6520 7469 6d65 2062 6569 6e67 2e20 506c  e time being. Pl
-00003d00: 6561 7365 2073 6565 2074 6865 2066 757a  ease see the fuz
-00003d10: 7a79 206d 6174 6368 6572 206f 6e2d 6d61  zy matcher on-ma
-00003d20: 7463 6820 6361 6c6c 6261 636b 2065 7861  tch callback exa
-00003d30: 6d70 6c65 2061 626f 7665 2066 6f72 2069  mple above for i
-00003d40: 6465 6173 2e20 4966 2074 6865 7265 2069  deas. If there i
-00003d50: 7320 656e 6f75 6768 2069 6e74 6572 6573  s enough interes
-00003d60: 7420 696e 2069 6e74 6567 7261 7469 6e67  t in integrating
-00003d70: 2f63 7265 6174 696e 6720 6120 7275 6c65  /creating a rule
-00003d80: 7220 666f 7220 7468 6520 7369 6d69 6c61  r for the simila
-00003d90: 7269 7479 206d 6174 6368 6572 2074 6869  rity matcher thi
-00003da0: 7320 6361 6e20 6265 2064 6f6e 652e 5c6e  s can be done.\n
-00003db0: 5c6e 5468 6520 6675 6c6c 206c 6973 7420  \nThe full list 
-00003dc0: 6f66 206b 6579 776f 7264 2061 7267 756d  of keyword argum
-00003dd0: 656e 7473 2061 7661 696c 6162 6c65 2066  ents available f
-00003de0: 6f72 2073 696d 696c 6172 6974 7920 6d61  or similarity ma
-00003df0: 7463 6869 6e67 2072 756c 6573 2069 6e63  tching rules inc
-00003e00: 6c75 6465 733a 5c6e 5c6e 2d20 6066 6c65  ludes:\n\n- `fle
-00003e10: 7860 3a20 4e75 6d62 6572 206f 6620 746f  x`: Number of to
-00003e20: 6b65 6e73 2074 6f20 6d6f 7665 206d 6174  kens to move mat
-00003e30: 6368 2073 7061 6e20 626f 756e 6461 7269  ch span boundari
-00003e40: 6573 206c 6566 7420 616e 6420 7269 6768  es left and righ
-00003e50: 7420 6475 7269 6e67 206d 6174 6368 206f  t during match o
-00003e60: 7074 696d 697a 6174 696f 6e2e 2043 616e  ptimization. Can
-00003e70: 2062 6520 616e 2069 6e74 6567 6572 2076   be an integer v
-00003e80: 616c 7565 2077 6974 6820 6120 6d61 7820  alue with a max 
-00003e90: 6f66 2060 6c65 6e28 7175 6572 7929 6020  of `len(query)` 
-00003ea0: 616e 6420 6120 6d69 6e20 6f66 2060 3060  and a min of `0`
-00003eb0: 2028 7769 6c6c 2077 6172 6e20 616e 6420   (will warn and 
-00003ec0: 6368 616e 6765 2069 6620 6869 6768 6572  change if higher
-00003ed0: 206f 7220 6c6f 7765 7229 2c20 6022 6d61   or lower), `"ma
-00003ee0: 7822 602c 2060 226d 696e 2260 2c20 6f72  x"`, `"min"`, or
-00003ef0: 2060 2264 6566 6175 6c74 2260 2e20 4465   `"default"`. De
-00003f00: 6661 756c 7420 6973 2060 2264 6566 6175  fault is `"defau
-00003f10: 6c74 2260 3a20 606c 656e 2871 7565 7279  lt"`: `len(query
-00003f20: 2920 2f2f 2032 602e 5c6e 2d20 606d 696e  ) // 2`.\n- `min
-00003f30: 5f72 3160 3a20 4d69 6e69 6d75 6d20 7369  _r1`: Minimum si
-00003f40: 6d69 6c61 7269 7479 206d 6174 6368 2072  milarity match r
-00003f50: 6174 696f 2072 6571 7569 7265 6420 666f  atio required fo
-00003f60: 7220 7365 6c65 6374 696f 6e20 6475 7269  r selection duri
-00003f70: 6e67 2074 6865 2069 6e74 6961 6c20 7365  ng the intial se
-00003f80: 6172 6368 206f 7665 7220 646f 632e 2054  arch over doc. T
-00003f90: 6869 7320 7368 6f75 6c64 2062 6520 6c6f  his should be lo
-00003fa0: 7765 7220 7468 616e 2060 6d69 6e5f 7232  wer than `min_r2
-00003fb0: 6020 616e 6420 226c 6f77 2220 696e 2067  ` and "low" in g
-00003fc0: 656e 6572 616c 2062 6563 6175 7365 206d  eneral because m
-00003fd0: 6174 6368 2073 7061 6e20 626f 756e 6461  atch span bounda
-00003fe0: 7269 6573 2061 7265 206e 6f74 2066 6c65  ries are not fle
-00003ff0: 7865 6420 696e 6974 6961 6c6c 792e 2060  xed initially. `
-00004000: 3060 206d 6561 6e73 2061 6c6c 2073 7061  0` means all spa
-00004010: 6e73 206f 6620 7175 6572 7920 6c65 6e67  ns of query leng
-00004020: 7468 2069 6e20 646f 6320 7769 6c6c 2068  th in doc will h
-00004030: 6176 6520 7468 6569 7220 626f 756e 6461  ave their bounda
-00004040: 7269 6573 2066 6c65 7865 6420 616e 6420  ries flexed and 
-00004050: 7769 6c6c 2062 6520 7265 2d63 6f6d 7061  will be re-compa
-00004060: 7265 6420 6475 7269 6e67 206d 6174 6368  red during match
-00004070: 206f 7074 696d 697a 6174 696f 6e2e 204c   optimization. L
-00004080: 6f77 6572 2060 6d69 6e5f 7231 6020 7769  ower `min_r1` wi
-00004090: 6c6c 2072 6573 756c 7420 696e 206d 6f72  ll result in mor
-000040a0: 6520 6669 6e65 2d67 7261 696e 6564 206d  e fine-grained m
-000040b0: 6174 6368 696e 6720 6275 7420 7769 6c6c  atching but will
-000040c0: 2072 756e 2073 6c6f 7765 722e 2044 6566   run slower. Def
-000040d0: 6175 6c74 2069 7320 6035 3060 2e5c 6e2d  ault is `50`.\n-
-000040e0: 2060 6d69 6e5f 7232 603a 204d 696e 696d   `min_r2`: Minim
-000040f0: 756d 2073 696d 696c 6172 6974 7920 6d61  um similarity ma
-00004100: 7463 6820 7261 7469 6f20 7265 7175 6972  tch ratio requir
-00004110: 6564 2066 6f72 2073 656c 6563 7469 6f6e  ed for selection
-00004120: 2064 7572 696e 6720 6d61 7463 6820 6f70   during match op
-00004130: 7469 6d69 7a61 7469 6f6e 2e20 5368 6f75  timization. Shou
-00004140: 6c64 2062 6520 6869 6768 6572 2074 6861  ld be higher tha
-00004150: 6e20 606d 696e 5f72 3160 2061 6e64 2022  n `min_r1` and "
-00004160: 6869 6768 2220 696e 2067 656e 6572 616c  high" in general
-00004170: 2074 6f20 656e 7375 7265 206f 6e6c 7920   to ensure only 
-00004180: 7175 616c 6974 7920 6d61 7463 6865 7320  quality matches 
-00004190: 6172 6520 7265 7475 726e 6564 2e20 4465  are returned. De
-000041a0: 6661 756c 7420 6973 2060 3735 602e 5c6e  fault is `75`.\n
-000041b0: 2d20 6074 6872 6573 6860 3a20 4966 2074  - `thresh`: If t
-000041c0: 6869 7320 7261 7469 6f20 6973 2065 7863  his ratio is exc
-000041d0: 6565 6465 6420 696e 2069 6e69 7469 616c  eeded in initial
-000041e0: 2073 6361 6e20 6e6f 206f 7074 696d 697a   scan no optimiz
-000041f0: 6174 696f 6e20 7769 6c6c 2062 6520 6174  ation will be at
-00004200: 7465 6d70 7465 642e 2044 6566 6175 6c74  tempted. Default
-00004210: 2069 7320 6031 3030 602e 5c6e 5c6e 2323   is `100`.\n\n##
-00004220: 2320 546f 6b65 6e4d 6174 6368 6572 5c6e  # TokenMatcher\n
-00004230: 5c6e 5468 6520 6261 7369 6320 7573 6167  \nThe basic usag
-00004240: 6520 6f66 2074 6865 2074 6f6b 656e 206d  e of the token m
-00004250: 6174 6368 6572 2069 7320 7369 6d69 6c61  atcher is simila
-00004260: 7220 746f 2073 7061 4379 5c27 7320 604d  r to spaCy\'s `M
-00004270: 6174 6368 6572 602e 2049 7420 6163 6365  atcher`. It acce
-00004280: 7074 7320 6c61 6265 6c65 6420 7061 7474  pts labeled patt
-00004290: 6572 6e73 2069 6e20 7468 6520 666f 726d  erns in the form
-000042a0: 206f 6620 6c69 7374 7320 6f66 2064 6963   of lists of dic
-000042b0: 7469 6f6e 6172 6965 7320 7768 6572 6520  tionaries where 
-000042c0: 6561 6368 206c 6973 7420 6465 7363 7269  each list descri
-000042d0: 6265 7320 616e 2069 6e64 6976 6964 7561  bes an individua
-000042e0: 6c20 7061 7474 6572 6e20 616e 6420 6561  l pattern and ea
-000042f0: 6368 2064 6963 7469 6f6e 6172 7920 6465  ch dictionary de
-00004300: 7363 7269 6265 7320 616e 2069 6e64 6976  scribes an indiv
-00004310: 6964 7561 6c20 746f 6b65 6e2e 5c6e 5c6e  idual token.\n\n
-00004320: 5468 6520 746f 6b65 6e20 6d61 7463 6865  The token matche
-00004330: 7220 6163 6365 7074 7320 616c 6c20 7468  r accepts all th
-00004340: 6520 7361 6d65 2074 6f6b 656e 2061 7474  e same token att
-00004350: 7269 6275 7465 7320 616e 6420 7061 7474  ributes and patt
-00004360: 6572 6e20 7379 6e74 6178 2061 7320 6974  ern syntax as it
-00004370: 5c27 7320 7370 6143 7920 636f 756e 7465  \'s spaCy counte
-00004380: 7270 6172 7420 6275 7420 6164 6473 2066  rpart but adds f
-00004390: 757a 7a79 2061 6e64 2066 757a 7a79 2d72  uzzy and fuzzy-r
-000043a0: 6567 6578 2073 7570 706f 7274 2e5c 6e5c  egex support.\n\
-000043b0: 6e60 2246 555a 5a59 2260 2061 6e64 2060  n`"FUZZY"` and `
-000043c0: 2246 5245 4745 5822 6020 6172 6520 7468  "FREGEX"` are th
-000043d0: 6520 7477 6f20 6164 6469 7469 6f6e 616c  e two additional
-000043e0: 2073 7061 4379 2074 6f6b 656e 2070 6174   spaCy token pat
-000043f0: 7465 726e 206f 7074 696f 6e73 2e5c 6e5c  tern options.\n\
-00004400: 6e46 6f72 2065 7861 6d70 6c65 3a5c 6e20  nFor example:\n 
-00004410: 2020 2060 7b22 5445 5854 223a 207b 2246     `{"TEXT": {"F
-00004420: 5245 4745 5822 3a20 2228 6461 7461 6261  REGEX": "(databa
-00004430: 7365 297b 653c 3d31 7d22 7d7d 2c60 5c6e  se){e<=1}"}},`\n
-00004440: 2020 2020 607b 224c 4f57 4552 223a 207b      `{"LOWER": {
-00004450: 2246 555a 5a59 223a 2022 6163 6365 7373  "FUZZY": "access
-00004460: 222c 2022 4d49 4e5f 5222 3a20 3835 2c20  ", "MIN_R": 85, 
-00004470: 2246 555a 5a59 5f46 554e 4322 3a20 2271  "FUZZY_FUNC": "q
-00004480: 7569 636b 5f6c 6576 227d 7d60 5c6e 5c6e  uick_lev"}}`\n\n
-00004490: 2a2a 4d61 6b65 2073 7572 6520 746f 2075  **Make sure to u
-000044a0: 7365 2075 7070 6572 6361 7365 2064 6963  se uppercase dic
-000044b0: 7469 6f6e 6172 7920 6b65 7973 2069 6e20  tionary keys in 
-000044c0: 7061 7474 6572 6e73 2e2a 2a5c 6e5c 6e5c  patterns.**\n\n\
-000044d0: 6e60 6060 7079 7468 6f6e 5c6e 696d 706f  n```python\nimpo
-000044e0: 7274 2073 7061 6379 5c6e 6672 6f6d 2073  rt spacy\nfrom s
-000044f0: 7061 637a 7a2e 6d61 7463 6865 7220 696d  paczz.matcher im
-00004500: 706f 7274 2054 6f6b 656e 4d61 7463 6865  port TokenMatche
-00004510: 725c 6e5c 6e23 2055 7369 6e67 206d 6f64  r\n\n# Using mod
-00004520: 656c 2072 6573 756c 7473 206c 696b 6520  el results like 
-00004530: 504f 5320 7461 6767 696e 6720 696e 2074  POS tagging in t
-00004540: 6f6b 656e 2070 6174 7465 726e 7320 7265  oken patterns re
-00004550: 7175 6972 6573 206d 6f64 656c 2074 6861  quires model tha
-00004560: 7420 7072 6f76 6964 6573 2074 6865 7365  t provides these
-00004570: 2e5c 6e6e 6c70 203d 2073 7061 6379 2e6c  .\nnlp = spacy.l
-00004580: 6f61 6428 2265 6e5f 636f 7265 5f77 6562  oad("en_core_web
-00004590: 5f6d 6422 295c 6e74 6578 7420 3d20 2222  _md")\ntext = ""
-000045a0: 2254 6865 206d 616e 6167 6572 2067 6176  "The manager gav
-000045b0: 6520 6d65 2053 514c 2064 6174 6162 6573  e me SQL databes
-000045c0: 4520 6163 6573 7320 736f 206e 6f77 2049  E acess so now I
-000045d0: 2063 616e 2061 6363 6573 2074 6865 2053   can acces the S
-000045e0: 6571 7561 6c20 4442 2e5c 6e4d 7920 6d61  equal DB.\nMy ma
-000045f0: 6e61 6765 725c 2773 206e 616d 6520 6973  nager\'s name is
-00004600: 2047 7266 6965 6c64 2222 225c 6e64 6f63   Grfield"""\ndoc
-00004610: 203d 206e 6c70 2874 6578 7429 5c6e 5c6e   = nlp(text)\n\n
-00004620: 6d61 7463 6865 7220 3d20 546f 6b65 6e4d  matcher = TokenM
-00004630: 6174 6368 6572 2876 6f63 6162 3d6e 6c70  atcher(vocab=nlp
-00004640: 2e76 6f63 6162 295c 6e6d 6174 6368 6572  .vocab)\nmatcher
-00004650: 2e61 6464 285c 6e20 2020 2022 4441 5441  .add(\n    "DATA
-00004660: 222c 5c6e 2020 2020 5b5c 6e20 2020 2020  ",\n    [\n     
-00004670: 2020 205b 5c6e 2020 2020 2020 2020 2020     [\n          
-00004680: 2020 7b22 5445 5854 223a 2022 5351 4c22    {"TEXT": "SQL"
-00004690: 7d2c 5c6e 2020 2020 2020 2020 2020 2020  },\n            
-000046a0: 7b22 4c4f 5745 5222 3a20 7b22 4652 4547  {"LOWER": {"FREG
-000046b0: 4558 223a 2022 2864 6174 6162 6173 6529  EX": "(database)
-000046c0: 7b73 3c3d 317d 227d 7d2c 5c6e 2020 2020  {s<=1}"}},\n    
-000046d0: 2020 2020 2020 2020 7b22 4c4f 5745 5222          {"LOWER"
-000046e0: 3a20 7b22 4655 5a5a 5922 3a20 2261 6363  : {"FUZZY": "acc
-000046f0: 6573 7322 7d7d 2c5c 6e20 2020 2020 2020  ess"}},\n       
-00004700: 205d 2c5c 6e20 2020 2020 2020 205b 7b22   ],\n        [{"
-00004710: 5445 5854 223a 207b 2246 555a 5a59 223a  TEXT": {"FUZZY":
-00004720: 2022 5365 7175 656c 227d 2c20 2250 4f53   "Sequel"}, "POS
-00004730: 223a 2022 5052 4f50 4e22 7d2c 207b 224c  ": "PROPN"}, {"L
-00004740: 4f57 4552 223a 2022 6462 227d 5d2c 5c6e  OWER": "db"}],\n
-00004750: 2020 2020 5d2c 5c6e 295c 6e6d 6174 6368      ],\n)\nmatch
-00004760: 6572 2e61 6464 2822 4e41 4d45 222c 205b  er.add("NAME", [
-00004770: 5b7b 2254 4558 5422 3a20 7b22 4655 5a5a  [{"TEXT": {"FUZZ
-00004780: 5922 3a20 2247 6172 6669 656c 6422 7d7d  Y": "Garfield"}}
-00004790: 5d5d 295c 6e6d 6174 6368 6573 203d 206d  ]])\nmatches = m
-000047a0: 6174 6368 6572 2864 6f63 295c 6e5c 6e66  atcher(doc)\n\nf
-000047b0: 6f72 206d 6174 6368 5f69 642c 2073 7461  or match_id, sta
-000047c0: 7274 2c20 656e 642c 205f 2069 6e20 6d61  rt, end, _ in ma
-000047d0: 7463 6865 733a 2020 2320 4e6f 7465 2074  tches:  # Note t
-000047e0: 6865 205f 2068 6572 652e 2045 7870 6c61  he _ here. Expla
-000047f0: 696e 6564 2062 656c 6f77 2e5c 6e20 2020  ined below.\n   
-00004800: 2070 7269 6e74 286d 6174 6368 5f69 642c   print(match_id,
-00004810: 2064 6f63 5b73 7461 7274 3a65 6e64 5d29   doc[start:end])
-00004820: 5c6e 6060 605c 6e5c 6e20 2020 2044 4154  \n```\n\n    DAT
-00004830: 4120 5351 4c20 6461 7461 6265 7345 2061  A SQL databesE a
-00004840: 6365 7373 5c6e 2020 2020 4441 5441 2053  cess\n    DATA S
-00004850: 6571 7561 6c20 4442 5c6e 2020 2020 4e41  equal DB\n    NA
-00004860: 4d45 2047 7266 6965 6c64 5c6e 5c6e 5c6e  ME Grfield\n\n\n
-00004870: 506c 6561 7365 206e 6f74 6520 7468 6174  Please note that
-00004880: 2074 6865 2077 6179 2074 6865 2074 6f6b   the way the tok
-00004890: 656e 206d 6174 6368 6572 2069 7320 696d  en matcher is im
-000048a0: 706c 656d 656e 7465 6420 646f 6573 206e  plemented does n
-000048b0: 6f74 2063 7572 7265 6e74 6c79 2068 6176  ot currently hav
-000048c0: 6520 6120 7761 7920 746f 2072 6574 7572  e a way to retur
-000048d0: 6e20 6675 7a7a 7920 7261 7469 6f20 6f72  n fuzzy ratio or
-000048e0: 2066 757a 7a79 2d72 6567 6578 2063 6f75   fuzzy-regex cou
-000048f0: 6e74 7320 6c69 6b65 2074 6865 2066 757a  nts like the fuz
-00004900: 7a79 206d 6174 6368 6572 2061 6e64 2072  zy matcher and r
-00004910: 6567 6578 206d 6174 6368 6572 2070 726f  egex matcher pro
-00004920: 7669 6465 2e20 546f 206b 6565 7020 7468  vide. To keep th
-00004930: 6520 4150 4920 636f 6e73 6973 7465 6e74  e API consistent
-00004940: 2c20 7468 6520 746f 6b65 6e20 6d61 7463  , the token matc
-00004950: 6865 7220 7265 7475 726e 7320 6120 706c  her returns a pl
-00004960: 6163 6568 6f6c 6465 7220 6f66 2060 4e6f  aceholder of `No
-00004970: 6e65 6020 6173 2074 6865 2066 6f75 7274  ne` as the fourt
-00004980: 6820 656c 656d 656e 7420 6f66 2074 6865  h element of the
-00004990: 2074 7570 6c65 7320 6974 2072 6574 7572   tuples it retur
-000049a0: 6e73 2c20 736f 2062 6520 7375 7265 2074  ns, so be sure t
-000049b0: 6f20 6163 636f 756e 7420 666f 7220 7468  o account for th
-000049c0: 6973 206c 696b 6520 7765 2064 6964 2077  is like we did w
-000049d0: 6974 6820 605f 6020 696e 2075 6e70 6163  ith `_` in unpac
-000049e0: 6b69 6e67 2061 626f 7665 2e5c 6e5c 6e41  king above.\n\nA
-000049f0: 6c73 6f2c 2065 7665 6e20 7468 6f75 6768  lso, even though
-00004a00: 2074 6865 2074 6f6b 656e 206d 6174 6368   the token match
-00004a10: 6572 2063 616e 2062 6520 6120 6472 6f70  er can be a drop
-00004a20: 2d69 6e20 7265 706c 6163 656d 656e 7420  -in replacement 
-00004a30: 666f 7220 7370 6143 795c 2773 2060 4d61  for spaCy\'s `Ma
-00004a40: 7463 6865 7260 2c20 6974 2069 7320 7374  tcher`, it is st
-00004a50: 696c 6c20 7265 636f 6d6d 656e 6465 6420  ill recommended 
-00004a60: 746f 2075 7365 2073 7061 4379 5c27 7320  to use spaCy\'s 
-00004a70: 604d 6174 6368 6572 6020 6966 2079 6f75  `Matcher` if you
-00004a80: 2064 6f20 6e6f 7420 6e65 6564 2074 6865   do not need the
-00004a90: 2073 7061 637a 7a20 746f 6b65 6e20 6d61   spaczz token ma
-00004aa0: 7463 6865 725c 2773 2066 757a 7a79 2063  tcher\'s fuzzy c
-00004ab0: 6170 6162 696c 6974 6965 7320 2d20 6974  apabilities - it
-00004ac0: 2077 696c 6c20 736c 6f77 2070 726f 6365   will slow proce
-00004ad0: 7373 696e 6720 646f 776e 2075 6e6e 6563  ssing down unnec
-00004ae0: 6573 7361 7269 6c79 2e5c 6e5c 6e23 2323  essarily.\n\n###
-00004af0: 2053 7061 637a 7a52 756c 6572 5c6e 5c6e   SpaczzRuler\n\n
-00004b00: 5468 6520 7370 6163 7a7a 2072 756c 6572  The spaczz ruler
-00004b10: 2063 6f6d 6269 6e65 7320 7468 6520 6675   combines the fu
-00004b20: 7a7a 7920 616e 6420 7265 6765 7820 7068  zzy and regex ph
-00004b30: 7261 7365 206d 6174 6368 6572 732c 2061  rase matchers, a
-00004b40: 6e64 2074 6865 2022 6675 7a7a 7922 2074  nd the "fuzzy" t
-00004b50: 6f6b 656e 206d 6174 6368 6572 2c20 696e  oken matcher, in
-00004b60: 746f 206f 6e65 2070 6970 656c 696e 6520  to one pipeline 
-00004b70: 636f 6d70 6f6e 656e 7420 7468 6174 2063  component that c
-00004b80: 616e 2075 7064 6174 6520 6120 646f 6320  an update a doc 
-00004b90: 656e 7469 7469 6573 2073 696d 696c 6172  entities similar
-00004ba0: 2074 6f20 7370 6143 795c 2773 2060 456e   to spaCy\'s `En
-00004bb0: 7469 7479 5275 6c65 7260 2e5c 6e5c 6e50  tityRuler`.\n\nP
-00004bc0: 6174 7465 726e 7320 6d75 7374 2062 6520  atterns must be 
-00004bd0: 6164 6465 6420 6173 2061 6e20 6974 6572  added as an iter
-00004be0: 6162 6c65 206f 6620 6469 6374 696f 6e61  able of dictiona
-00004bf0: 7269 6573 2069 6e20 7468 6520 666f 726d  ries in the form
-00004c00: 6174 206f 6620 2a7b 6c61 6265 6c20 2873  at of *{label (s
-00004c10: 7472 292c 2070 6174 7465 726e 2873 7472  tr), pattern(str
-00004c20: 206f 7220 6c69 7374 292c 2074 7970 6528   or list), type(
-00004c30: 7374 7229 2c20 6f70 7469 6f6e 616c 206b  str), optional k
-00004c40: 7761 7267 7320 2864 6963 7429 2c20 616e  wargs (dict), an
-00004c50: 6420 6f70 7469 6f6e 616c 2069 6420 2873  d optional id (s
-00004c60: 7472 297d 2a2e 5c6e 5c6e 466f 7220 6578  tr)}*.\n\nFor ex
-00004c70: 616d 706c 652c 2061 2066 757a 7a79 2070  ample, a fuzzy p
-00004c80: 6872 6173 6520 7061 7474 6572 6e3a 5c6e  hrase pattern:\n
-00004c90: 5c6e 607b 5c27 6c61 6265 6c5c 273a 205c  \n`{\'label\': \
-00004ca0: 274f 5247 5c27 2c20 5c27 7061 7474 6572  'ORG\', \'patter
-00004cb0: 6e5c 273a 205c 2741 7070 6c65 5c27 2c20  n\': \'Apple\', 
-00004cc0: 5c27 7479 7065 5c27 3a20 5c27 6675 7a7a  \'type\': \'fuzz
-00004cd0: 795c 272c 205c 276b 7761 7267 735c 273a  y\', \'kwargs\':
-00004ce0: 207b 5c27 6d69 6e5f 7232 5c27 3a20 3930   {\'min_r2\': 90
-00004cf0: 7d7d 605c 6e5c 6e4f 722c 2061 2074 6f6b  }}`\n\nOr, a tok
-00004d00: 656e 2070 6174 7465 726e 3a5c 6e5c 6e60  en pattern:\n\n`
-00004d10: 7b5c 276c 6162 656c 5c27 3a20 5c27 4f52  {\'label\': \'OR
-00004d20: 475c 272c 205c 2770 6174 7465 726e 5c27  G\', \'pattern\'
-00004d30: 3a20 5b7b 5c27 5445 5854 5c27 3a20 7b5c  : [{\'TEXT\': {\
-00004d40: 2746 555a 5a59 5c27 3a20 5c27 4170 706c  'FUZZY\': \'Appl
-00004d50: 655c 277d 7d5d 2c20 5c27 7479 7065 5c27  e\'}}], \'type\'
-00004d60: 3a20 5c27 746f 6b65 6e5c 277d 605c 6e5c  : \'token\'}`\n\
-00004d70: 6e5c 6e60 6060 7079 7468 6f6e 5c6e 696d  n\n```python\nim
-00004d80: 706f 7274 2073 7061 6379 5c6e 6672 6f6d  port spacy\nfrom
-00004d90: 2073 7061 637a 7a2e 7069 7065 6c69 6e65   spaczz.pipeline
-00004da0: 2069 6d70 6f72 7420 5370 6163 7a7a 5275   import SpaczzRu
-00004db0: 6c65 725c 6e5c 6e6e 6c70 203d 2073 7061  ler\n\nnlp = spa
-00004dc0: 6379 2e62 6c61 6e6b 2822 656e 2229 5c6e  cy.blank("en")\n
-00004dd0: 7465 7874 203d 2022 2222 416e 6465 7273  text = """Anders
-00004de0: 6f6e 2c20 4772 696e 7420 6372 6561 7465  on, Grint create
-00004df0: 6420 7370 6163 7a7a 2069 6e20 6869 7320  d spaczz in his 
-00004e00: 686f 6d65 2061 7420 3535 3520 4661 6b65  home at 555 Fake
-00004e10: 2053 742c 5c6e 4170 7420 3520 696e 204e   St,\nApt 5 in N
-00004e20: 6173 6876 316c 652c 2054 4e20 3535 3535  ashv1le, TN 5555
-00004e30: 352d 3132 3334 2069 6e20 7468 6520 5553  5-1234 in the US
-00004e40: 412e 5c6e 536f 6d65 206f 6620 6869 7320  A.\nSome of his 
-00004e50: 6661 766f 7269 7465 2062 616e 6473 2061  favorite bands a
-00004e60: 7265 2043 6f6e 7665 7267 2061 6e64 2050  re Converg and P
-00004e70: 726f 7465 7420 7468 6520 5a65 726f 2e22  rotet the Zero."
-00004e80: 2222 2020 2320 5370 656c 6c69 6e67 2065  ""  # Spelling e
-00004e90: 7272 6f72 7320 696e 7465 6e74 696f 6e61  rrors intentiona
-00004ea0: 6c2e 5c6e 646f 6320 3d20 6e6c 7028 7465  l.\ndoc = nlp(te
-00004eb0: 7874 295c 6e5c 6e70 6174 7465 726e 7320  xt)\n\npatterns 
-00004ec0: 3d20 5b5c 6e20 2020 207b 5c6e 2020 2020  = [\n    {\n    
-00004ed0: 2020 2020 226c 6162 656c 223a 2022 4e41      "label": "NA
-00004ee0: 4d45 222c 5c6e 2020 2020 2020 2020 2270  ME",\n        "p
-00004ef0: 6174 7465 726e 223a 2022 4772 616e 7420  attern": "Grant 
-00004f00: 416e 6465 7273 656e 222c 5c6e 2020 2020  Andersen",\n    
-00004f10: 2020 2020 2274 7970 6522 3a20 2266 757a      "type": "fuz
-00004f20: 7a79 222c 5c6e 2020 2020 2020 2020 226b  zy",\n        "k
-00004f30: 7761 7267 7322 3a20 7b22 6675 7a7a 795f  wargs": {"fuzzy_
-00004f40: 6675 6e63 223a 2022 746f 6b65 6e5f 736f  func": "token_so
-00004f50: 7274 227d 2c5c 6e20 2020 207d 2c5c 6e20  rt"},\n    },\n 
-00004f60: 2020 207b 5c6e 2020 2020 2020 2020 226c     {\n        "l
-00004f70: 6162 656c 223a 2022 5354 5245 4554 222c  abel": "STREET",
-00004f80: 5c6e 2020 2020 2020 2020 2270 6174 7465  \n        "patte
-00004f90: 726e 223a 2022 7374 7265 6574 5f61 6464  rn": "street_add
-00004fa0: 7265 7373 6573 222c 5c6e 2020 2020 2020  resses",\n      
-00004fb0: 2020 2274 7970 6522 3a20 2272 6567 6578    "type": "regex
-00004fc0: 222c 5c6e 2020 2020 2020 2020 226b 7761  ",\n        "kwa
-00004fd0: 7267 7322 3a20 7b22 7072 6564 6566 223a  rgs": {"predef":
-00004fe0: 2054 7275 657d 2c5c 6e20 2020 207d 2c5c   True},\n    },\
-00004ff0: 6e20 2020 207b 226c 6162 656c 223a 2022  n    {"label": "
-00005000: 4750 4522 2c20 2270 6174 7465 726e 223a  GPE", "pattern":
-00005010: 2022 4e61 7368 7669 6c6c 6522 2c20 2274   "Nashville", "t
-00005020: 7970 6522 3a20 2266 757a 7a79 227d 2c5c  ype": "fuzzy"},\
-00005030: 6e20 2020 207b 5c6e 2020 2020 2020 2020  n    {\n        
-00005040: 226c 6162 656c 223a 2022 5a49 5022 2c5c  "label": "ZIP",\
-00005050: 6e20 2020 2020 2020 2022 7061 7474 6572  n        "patter
-00005060: 6e22 3a20 7222 5c5c 6228 3f3a 3535 3535  n": r"\\b(?:5555
-00005070: 3429 7b73 3c3d 317d 283f 3a28 3f3a 5b2d  4){s<=1}(?:(?:[-
-00005080: 5c5c 735d 293f 5c5c 647b 347d 5c5c 6229  \\s])?\\d{4}\\b)
-00005090: 222c 5c6e 2020 2020 2020 2020 2274 7970  ",\n        "typ
-000050a0: 6522 3a20 2272 6567 6578 222c 5c6e 2020  e": "regex",\n  
-000050b0: 2020 7d2c 2020 2320 6675 7a7a 7920 7265    },  # fuzzy re
-000050c0: 6765 785c 6e20 2020 207b 226c 6162 656c  gex\n    {"label
-000050d0: 223a 2022 4750 4522 2c20 2270 6174 7465  ": "GPE", "patte
-000050e0: 726e 223a 2022 283f 6929 5b55 5d28 6e69  rn": "(?i)[U](ni
-000050f0: 7465 647c 5c5c 2e3f 2920 3f5b 535d 2874  ted|\\.?) ?[S](t
-00005100: 6174 6573 7c5c 5c2e 3f29 222c 2022 7479  ates|\\.?)", "ty
-00005110: 7065 223a 2022 7265 6765 7822 7d2c 5c6e  pe": "regex"},\n
-00005120: 2020 2020 7b5c 6e20 2020 2020 2020 2022      {\n        "
-00005130: 6c61 6265 6c22 3a20 2242 414e 4422 2c5c  label": "BAND",\
-00005140: 6e20 2020 2020 2020 2022 7061 7474 6572  n        "patter
-00005150: 6e22 3a20 5b7b 224c 4f57 4552 223a 207b  n": [{"LOWER": {
-00005160: 2246 5245 4745 5822 3a20 2228 636f 6e76  "FREGEX": "(conv
-00005170: 6572 6765 297b 653c 3d31 7d22 7d7d 5d2c  erge){e<=1}"}}],
-00005180: 5c6e 2020 2020 2020 2020 2274 7970 6522  \n        "type"
-00005190: 3a20 2274 6f6b 656e 222c 5c6e 2020 2020  : "token",\n    
-000051a0: 7d2c 5c6e 2020 2020 7b5c 6e20 2020 2020  },\n    {\n     
-000051b0: 2020 2022 6c61 6265 6c22 3a20 2242 414e     "label": "BAN
-000051c0: 4422 2c5c 6e20 2020 2020 2020 2022 7061  D",\n        "pa
-000051d0: 7474 6572 6e22 3a20 5b5c 6e20 2020 2020  ttern": [\n     
-000051e0: 2020 2020 2020 207b 2254 4558 5422 3a20         {"TEXT": 
-000051f0: 7b22 4655 5a5a 5922 3a20 2250 726f 7465  {"FUZZY": "Prote
-00005200: 7374 227d 7d2c 5c6e 2020 2020 2020 2020  st"}},\n        
-00005210: 2020 2020 7b22 4953 5f53 544f 5022 3a20      {"IS_STOP": 
-00005220: 5472 7565 7d2c 5c6e 2020 2020 2020 2020  True},\n        
-00005230: 2020 2020 7b22 5445 5854 223a 207b 2246      {"TEXT": {"F
-00005240: 555a 5a59 223a 2022 4865 726f 227d 7d2c  UZZY": "Hero"}},
-00005250: 5c6e 2020 2020 2020 2020 5d2c 5c6e 2020  \n        ],\n  
-00005260: 2020 2020 2020 2274 7970 6522 3a20 2274        "type": "t
-00005270: 6f6b 656e 222c 5c6e 2020 2020 7d2c 5c6e  oken",\n    },\n
-00005280: 5d5c 6e5c 6e72 756c 6572 203d 2053 7061  ]\n\nruler = Spa
-00005290: 637a 7a52 756c 6572 286e 6c70 295c 6e72  czzRuler(nlp)\nr
-000052a0: 756c 6572 2e61 6464 5f70 6174 7465 726e  uler.add_pattern
-000052b0: 7328 7061 7474 6572 6e73 295c 6e64 6f63  s(patterns)\ndoc
-000052c0: 203d 2072 756c 6572 2864 6f63 295c 6e5c   = ruler(doc)\n\
-000052d0: 6e70 7269 6e74 2822 4675 7a7a 7920 4d61  nprint("Fuzzy Ma
-000052e0: 7463 6865 733a 2229 5c6e 666f 7220 656e  tches:")\nfor en
-000052f0: 7420 696e 2064 6f63 2e65 6e74 733a 5c6e  t in doc.ents:\n
-00005300: 2020 2020 6966 2065 6e74 2e5f 2e73 7061      if ent._.spa
-00005310: 637a 7a5f 7479 7065 203d 3d20 2266 757a  czz_type == "fuz
-00005320: 7a79 223a 5c6e 2020 2020 2020 2020 7072  zy":\n        pr
-00005330: 696e 7428 2865 6e74 2e74 6578 742c 2065  int((ent.text, e
-00005340: 6e74 2e73 7461 7274 2c20 656e 742e 656e  nt.start, ent.en
-00005350: 642c 2065 6e74 2e6c 6162 656c 5f2c 2065  d, ent.label_, e
-00005360: 6e74 2e5f 2e73 7061 637a 7a5f 7261 7469  nt._.spaczz_rati
-00005370: 6f29 295c 6e5c 6e70 7269 6e74 2822 5c5c  o))\n\nprint("\\
-00005380: 6e22 2c20 2252 6567 6578 204d 6174 6368  n", "Regex Match
-00005390: 6573 3a22 2c20 7365 703d 2222 295c 6e66  es:", sep="")\nf
-000053a0: 6f72 2065 6e74 2069 6e20 646f 632e 656e  or ent in doc.en
-000053b0: 7473 3a5c 6e20 2020 2069 6620 656e 742e  ts:\n    if ent.
-000053c0: 5f2e 7370 6163 7a7a 5f74 7970 6520 3d3d  _.spaczz_type ==
-000053d0: 2022 7265 6765 7822 3a5c 6e20 2020 2020   "regex":\n     
-000053e0: 2020 2070 7269 6e74 2828 656e 742e 7465     print((ent.te
-000053f0: 7874 2c20 656e 742e 7374 6172 742c 2065  xt, ent.start, e
-00005400: 6e74 2e65 6e64 2c20 656e 742e 6c61 6265  nt.end, ent.labe
-00005410: 6c5f 2c20 656e 742e 5f2e 7370 6163 7a7a  l_, ent._.spaczz
-00005420: 5f63 6f75 6e74 7329 295c 6e5c 6e70 7269  _counts))\n\npri
-00005430: 6e74 2822 5c5c 6e22 2c20 2254 6f6b 656e  nt("\\n", "Token
-00005440: 204d 6174 6368 6573 3a22 2c20 7365 703d   Matches:", sep=
-00005450: 2222 295c 6e66 6f72 2065 6e74 2069 6e20  "")\nfor ent in 
-00005460: 646f 632e 656e 7473 3a5c 6e20 2020 2069  doc.ents:\n    i
-00005470: 6620 656e 742e 5f2e 7370 6163 7a7a 5f74  f ent._.spaczz_t
-00005480: 7970 6520 3d3d 2022 746f 6b65 6e22 3a5c  ype == "token":\
-00005490: 6e20 2020 2020 2020 2023 202e 5f2e 7370  n        # ._.sp
-000054a0: 6163 7a7a 5f64 6574 6169 6c73 2069 7320  aczz_details is 
-000054b0: 6375 7272 656e 746c 7920 6a75 7374 2070  currently just p
-000054c0: 6c61 6365 686f 6c64 6572 2076 616c 7565  laceholder value
-000054d0: 206f 6620 315c 6e20 2020 2020 2020 2070   of 1\n        p
-000054e0: 7269 6e74 2828 656e 742e 7465 7874 2c20  rint((ent.text, 
-000054f0: 656e 742e 7374 6172 742c 2065 6e74 2e65  ent.start, ent.e
-00005500: 6e64 2c20 656e 742e 6c61 6265 6c5f 2c20  nd, ent.label_, 
-00005510: 656e 742e 5f2e 7370 6163 7a7a 5f64 6574  ent._.spaczz_det
-00005520: 6169 6c73 2929 5c6e 6060 605c 6e5c 6e20  ails))\n```\n\n 
-00005530: 2020 2046 757a 7a79 204d 6174 6368 6573     Fuzzy Matches
-00005540: 3a5c 6e20 2020 2028 5c27 416e 6465 7273  :\n    (\'Anders
-00005550: 6f6e 2c20 4772 696e 745c 272c 2030 2c20  on, Grint\', 0, 
-00005560: 332c 205c 274e 414d 455c 272c 2038 3629  3, \'NAME\', 86)
-00005570: 5c6e 2020 2020 285c 274e 6173 6876 316c  \n    (\'Nashv1l
-00005580: 655c 272c 2031 372c 2031 382c 205c 2747  e\', 17, 18, \'G
-00005590: 5045 5c27 2c20 3832 295c 6e5c 6e20 2020  PE\', 82)\n\n   
-000055a0: 2052 6567 6578 204d 6174 6368 6573 3a5c   Regex Matches:\
-000055b0: 6e20 2020 2028 5c27 3535 3520 4661 6b65  n    (\'555 Fake
-000055c0: 2053 742c 5c27 2c20 392c 2031 332c 205c   St,\', 9, 13, \
-000055d0: 2753 5452 4545 545c 272c 2028 302c 2030  'STREET\', (0, 0
-000055e0: 2c20 3029 295c 6e20 2020 2028 5c27 3535  , 0))\n    (\'55
-000055f0: 3535 352d 3132 3334 5c27 2c20 3230 2c20  555-1234\', 20, 
-00005600: 3233 2c20 5c27 5a49 505c 272c 2028 312c  23, \'ZIP\', (1,
-00005610: 2030 2c20 3029 295c 6e20 2020 2028 5c27   0, 0))\n    (\'
-00005620: 5553 415c 272c 2032 352c 2032 362c 205c  USA\', 25, 26, \
-00005630: 2747 5045 5c27 2c20 2830 2c20 302c 2030  'GPE\', (0, 0, 0
-00005640: 2929 5c6e 5c6e 2020 2020 546f 6b65 6e20  ))\n\n    Token 
-00005650: 4d61 7463 6865 733a 5c6e 2020 2020 285c  Matches:\n    (\
-00005660: 2743 6f6e 7665 7267 5c27 2c20 3334 2c20  'Converg\', 34, 
-00005670: 3335 2c20 5c27 4241 4e44 5c27 2c20 3129  35, \'BAND\', 1)
-00005680: 5c6e 2020 2020 285c 2750 726f 7465 7420  \n    (\'Protet 
-00005690: 7468 6520 5a65 726f 5c27 2c20 3336 2c20  the Zero\', 36, 
-000056a0: 3339 2c20 5c27 4241 4e44 5c27 2c20 3129  39, \'BAND\', 1)
-000056b0: 5c6e 5c6e 5c6e 5765 2073 6565 2069 6e20  \n\n\nWe see in 
-000056c0: 7468 6520 6578 616d 706c 6520 6162 6f76  the example abov
-000056d0: 6520 7468 6174 2077 6520 6172 6520 7265  e that we are re
-000056e0: 6665 7265 6e63 696e 6720 736f 6d65 2063  ferencing some c
-000056f0: 7573 746f 6d20 6174 7472 6962 7574 6573  ustom attributes
-00005700: 2c20 7768 6963 6820 6172 6520 6578 706c  , which are expl
-00005710: 6169 6e65 6420 6265 6c6f 772e 5c6e 5c6e  ained below.\n\n
-00005720: 466f 7220 6d6f 7265 2060 5370 6163 7a7a  For more `Spaczz
-00005730: 5275 6c65 7260 2065 7861 6d70 6c65 7320  Ruler` examples 
-00005740: 7365 6520 5b68 6572 655d 2868 7474 7073  see [here](https
-00005750: 3a2f 2f67 6974 6875 622e 636f 6d2f 6761  ://github.com/ga
-00005760: 6e64 6572 7365 6e31 3031 2f73 7061 637a  ndersen101/spacz
-00005770: 7a2f 626c 6f62 2f6d 6173 7465 722f 6578  z/blob/master/ex
-00005780: 616d 706c 6573 2f66 757a 7a79 5f6d 6174  amples/fuzzy_mat
-00005790: 6368 696e 675f 7477 6561 6b73 2e6d 6429  ching_tweaks.md)
-000057a0: 2e20 496e 2070 6172 7469 6375 6c61 7220  . In particular 
-000057b0: 7468 6973 2070 726f 7669 6465 7320 6465  this provides de
-000057c0: 7461 696c 7320 6162 6f75 7420 7468 6520  tails about the 
-000057d0: 7275 6c65 725c 2773 2073 6f72 7469 6e67  ruler\'s sorting
-000057e0: 2070 726f 6365 7373 2061 6e64 2066 757a   process and fuz
-000057f0: 7a79 206d 6174 6368 696e 6720 7061 7261  zy matching para
-00005800: 6d65 7465 7273 2e5c 6e5c 6e23 2323 2043  meters.\n\n### C
-00005810: 7573 746f 6d20 4174 7472 6962 7574 6573  ustom Attributes
-00005820: 5c6e 5c6e 5370 6163 7a7a 2069 6e69 7469  \n\nSpaczz initi
-00005830: 616c 697a 6573 2073 6f6d 6520 6375 7374  alizes some cust
-00005840: 6f6d 2061 7474 7269 6275 7465 7320 7570  om attributes up
-00005850: 6f6e 2069 6d70 6f72 7469 6e67 2e20 5468  on importing. Th
-00005860: 6573 6520 6172 6520 756e 6465 7220 7370  ese are under sp
-00005870: 6143 795c 2773 2060 2e5f 2e60 2061 7474  aCy\'s `._.` att
-00005880: 7269 6275 7465 2061 6e64 2061 7265 2066  ribute and are f
-00005890: 7572 7468 6572 2070 7265 7065 6e64 6564  urther prepended
-000058a0: 2077 6974 6820 6073 7061 637a 7a5f 6020   with `spaczz_` 
-000058b0: 736f 2074 6865 7265 2073 686f 756c 6420  so there should 
-000058c0: 6265 206e 6f74 2063 6f6e 666c 6963 7473  be not conflicts
-000058d0: 2077 6974 6820 796f 7572 206f 776e 2063   with your own c
-000058e0: 7573 746f 6d20 6174 7472 6962 7574 6573  ustom attributes
-000058f0: 2e20 4966 2074 6865 7265 2061 7265 2073  . If there are s
-00005900: 7061 637a 7a20 7769 6c6c 2066 6f72 6365  paczz will force
-00005910: 206f 7665 7277 7269 7465 2074 6865 6d2e   overwrite them.
-00005920: 5c6e 5c6e 5468 6573 6520 6375 7374 6f6d  \n\nThese custom
-00005930: 2061 7474 7269 6275 7465 7320 6172 6520   attributes are 
-00005940: 6f6e 6c79 2073 6574 2076 6961 2074 6865  only set via the
-00005950: 2073 7061 637a 7a20 7275 6c65 7220 6174   spaczz ruler at
-00005960: 2074 6865 2074 6f6b 656e 206c 6576 656c   the token level
-00005970: 2e20 5370 616e 2061 6e64 2064 6f63 2076  . Span and doc v
-00005980: 6572 7369 6f6e 7320 6f66 2074 6865 7365  ersions of these
-00005990: 2061 7474 7269 6275 7465 7320 6172 6520   attributes are 
-000059a0: 6765 7474 6572 7320 7468 6174 2072 6566  getters that ref
-000059b0: 6572 656e 6365 2074 6865 2074 6f6b 656e  erence the token
-000059c0: 206c 6576 656c 2061 7474 7269 6275 7465   level attribute
-000059d0: 732e 5c6e 5c6e 5468 6520 666f 6c6c 6f77  s.\n\nThe follow
-000059e0: 696e 6720 6054 6f6b 656e 6020 6174 7472  ing `Token` attr
-000059f0: 6962 7574 6573 2061 7265 2061 7661 696c  ibutes are avail
-00005a00: 6162 6c65 2e20 416c 6c20 6172 6520 6d75  able. All are mu
-00005a10: 7461 626c 653a 5c6e 5c6e 2d20 6073 7061  table:\n\n- `spa
-00005a20: 637a 7a5f 746f 6b65 6e60 3a20 6465 6661  czz_token`: defa
-00005a30: 756c 7420 3d20 6046 616c 7365 602e 2042  ult = `False`. B
-00005a40: 6f6f 6c65 616e 2074 6861 7420 6465 6e6f  oolean that deno
-00005a50: 7465 7320 6966 2074 6865 2074 6f6b 656e  tes if the token
-00005a60: 2069 7320 7061 7274 206f 6620 616e 2065   is part of an e
-00005a70: 6e74 2073 6574 2062 7920 7468 6520 7370  nt set by the sp
-00005a80: 6163 7a7a 2072 756c 6572 2e5c 6e2d 2060  aczz ruler.\n- `
-00005a90: 7370 6163 7a7a 5f74 7970 6560 3a20 6465  spaczz_type`: de
-00005aa0: 6661 756c 7420 3d20 604e 6f6e 6560 2e20  fault = `None`. 
-00005ab0: 5374 7269 6e67 2074 6861 7420 7368 6f77  String that show
-00005ac0: 7320 7768 6963 6820 6d61 7463 6865 7220  s which matcher 
-00005ad0: 7072 6f64 7563 6564 2061 6e20 656e 7420  produced an ent 
-00005ae0: 7573 696e 6720 7468 6520 746f 6b65 6e2e  using the token.
-00005af0: 5c6e 2d20 6073 7061 637a 7a5f 7261 7469  \n- `spaczz_rati
-00005b00: 6f60 3a20 6465 6661 756c 7420 3d20 604e  o`: default = `N
-00005b10: 6f6e 6560 2e20 4966 2074 6865 2074 6f6b  one`. If the tok
-00005b20: 656e 2069 7320 7061 7274 206f 6620 6675  en is part of fu
-00005b30: 7a7a 792d 7068 7261 7365 2d6d 6174 6368  zzy-phrase-match
-00005b40: 6564 2065 6e74 2c20 7769 6c6c 2072 6574  ed ent, will ret
-00005b50: 7572 6e20 6675 7a7a 7920 7261 7469 6f2e  urn fuzzy ratio.
-00005b60: 5c6e 2d20 6073 7061 637a 7a5f 636f 756e  \n- `spaczz_coun
-00005b70: 7473 603a 2064 6566 6175 6c74 203d 2060  ts`: default = `
-00005b80: 4e6f 6e65 602e 2049 6620 7468 6520 746f  None`. If the to
-00005b90: 6b65 6e20 6973 2070 6172 7420 6f66 2072  ken is part of r
-00005ba0: 6567 6578 2d70 6872 6173 652d 6d61 7463  egex-phrase-matc
-00005bb0: 6865 6420 656e 742c 2077 696c 6c20 7265  hed ent, will re
-00005bc0: 7475 726e 2066 757a 7a79 2063 6f75 6e74  turn fuzzy count
-00005bd0: 732e 5c6e 2d20 6073 7061 637a 7a5f 6465  s.\n- `spaczz_de
-00005be0: 7461 696c 7360 3a20 6465 6661 756c 7420  tails`: default 
-00005bf0: 3d20 604e 6f6e 6560 2e20 506c 6163 6568  = `None`. Placeh
-00005c00: 6f6c 6465 7220 666f 7220 746f 6b65 6e20  older for token 
-00005c10: 6d61 7463 6865 7220 6675 7a7a 7920 7261  matcher fuzzy ra
-00005c20: 7469 6f2f 636f 756e 7473 2e20 546f 2062  tio/counts. To b
-00005c30: 6520 6465 7665 6c6f 7065 642e 2057 696c  e developed. Wil
-00005c40: 6c20 7265 7475 726e 2031 2069 6620 7468  l return 1 if th
-00005c50: 6520 746f 6b65 6e20 6973 2070 6172 7420  e token is part 
-00005c60: 6f66 2061 2022 6675 7a7a 7922 2d74 6f6b  of a "fuzzy"-tok
-00005c70: 656e 2d6d 6174 6368 6564 2065 6e74 2e5c  en-matched ent.\
-00005c80: 6e5c 6e54 6865 2066 6f6c 6c6f 7769 6e67  n\nThe following
-00005c90: 2060 5370 616e 6020 6174 7472 6962 7574   `Span` attribut
-00005ca0: 6573 2072 6566 6572 656e 6365 2074 6865  es reference the
-00005cb0: 2074 6f6b 656e 2061 7474 7269 6275 7465   token attribute
-00005cc0: 7320 696e 636c 7564 6564 2069 6e20 7468  s included in th
-00005cd0: 6520 7370 616e 2e20 416c 6c20 6172 6520  e span. All are 
-00005ce0: 696d 6d75 7461 626c 653a 5c6e 5c6e 2d20  immutable:\n\n- 
-00005cf0: 6073 7061 637a 7a5f 656e 7460 3a20 6465  `spaczz_ent`: de
-00005d00: 6661 756c 7420 3d20 6046 616c 7365 602e  fault = `False`.
-00005d10: 2042 6f6f 6c65 616e 2074 6861 7420 6465   Boolean that de
-00005d20: 6e6f 7465 7320 6966 2061 6c6c 2074 6f6b  notes if all tok
-00005d30: 656e 7320 696e 2073 7061 6e20 6172 6520  ens in span are 
-00005d40: 7061 7274 206f 6620 616e 2065 6e74 2073  part of an ent s
-00005d50: 6574 2062 7920 7468 6520 7370 6163 7a7a  et by the spaczz
-00005d60: 2072 756c 6572 2e5c 6e2d 2060 7370 6163   ruler.\n- `spac
-00005d70: 7a7a 5f74 7970 6560 3a20 6465 6661 756c  zz_type`: defaul
-00005d80: 7420 3d20 604e 6f6e 6560 2e20 5374 7269  t = `None`. Stri
-00005d90: 6e67 2074 6861 7420 6465 6e6f 7465 7320  ng that denotes 
-00005da0: 7768 6963 6820 6d61 7463 6865 7220 7072  which matcher pr
-00005db0: 6f64 7563 6564 2061 6e20 656e 7420 7573  oduced an ent us
-00005dc0: 696e 6720 7468 6520 696e 636c 7564 6564  ing the included
-00005dd0: 2074 6f6b 656e 732e 5c6e 2d20 6073 7061   tokens.\n- `spa
-00005de0: 637a 7a5f 7479 7065 7360 3a20 6465 6661  czz_types`: defa
-00005df0: 756c 7420 3d20 6073 6574 2829 602e 2053  ult = `set()`. S
-00005e00: 6574 2074 6861 7420 7368 6f77 7320 7768  et that shows wh
-00005e10: 6963 6820 6d61 7463 6865 7273 2070 726f  ich matchers pro
-00005e20: 6475 6365 6420 656e 7473 2075 7369 6e67  duced ents using
-00005e30: 2074 6865 2069 6e63 6c75 6465 6420 746f   the included to
-00005e40: 6b65 6e73 2e20 416e 2065 6e74 6974 7920  kens. An entity 
-00005e50: 7370 616e 2073 686f 756c 6420 6f6e 6c79  span should only
-00005e60: 2068 6176 6520 6f6e 6520 7479 7065 2c20   have one type, 
-00005e70: 6275 7420 7468 6973 2061 6c6c 6f77 7320  but this allows 
-00005e80: 796f 7520 746f 2073 6565 2074 6865 2074  you to see the t
-00005e90: 7970 6573 2069 6e63 6c75 6465 6420 696e  ypes included in
-00005ea0: 2061 6e79 2061 7262 6974 7261 7279 2073   any arbitrary s
-00005eb0: 7061 6e2e 5c6e 2d20 6073 7061 637a 7a5f  pan.\n- `spaczz_
-00005ec0: 7261 7469 6f60 3a20 6465 6661 756c 7420  ratio`: default 
-00005ed0: 3d20 604e 6f6e 6560 2e20 4966 2061 6c6c  = `None`. If all
-00005ee0: 2074 6865 2074 6f6b 656e 7320 696e 2073   the tokens in s
-00005ef0: 7061 6e20 6172 6520 7061 7274 206f 6620  pan are part of 
-00005f00: 6675 7a7a 792d 7068 7261 7365 2d6d 6174  fuzzy-phrase-mat
-00005f10: 6368 6564 2065 6e74 2c20 7769 6c6c 2072  ched ent, will r
-00005f20: 6574 7572 6e20 6675 7a7a 7920 7261 7469  eturn fuzzy rati
-00005f30: 6f2e 5c6e 2d20 6073 7061 637a 7a5f 636f  o.\n- `spaczz_co
-00005f40: 756e 7473 603a 2064 6566 6175 6c74 203d  unts`: default =
-00005f50: 2060 4e6f 6e65 602e 2049 6620 616c 6c20   `None`. If all 
-00005f60: 7468 6520 746f 6b65 6e73 2069 6e20 7370  the tokens in sp
-00005f70: 616e 2061 7265 2070 6172 7420 6f66 2072  an are part of r
-00005f80: 6567 6578 2d70 6872 6173 652d 6d61 7463  egex-phrase-matc
-00005f90: 6865 6420 656e 742c 2077 696c 6c20 7265  hed ent, will re
-00005fa0: 7475 726e 2066 757a 7a79 2063 6f75 6e74  turn fuzzy count
-00005fb0: 732e 5c6e 2d20 6073 7061 637a 7a5f 6465  s.\n- `spaczz_de
-00005fc0: 7461 696c 7360 3a20 6465 6661 756c 7420  tails`: default 
-00005fd0: 3d20 604e 6f6e 6560 2e20 506c 6163 6568  = `None`. Placeh
-00005fe0: 6f6c 6465 7220 666f 7220 746f 6b65 6e20  older for token 
-00005ff0: 6d61 7463 6865 7220 6675 7a7a 7920 7261  matcher fuzzy ra
-00006000: 7469 6f2f 636f 756e 7473 2e20 546f 2062  tio/counts. To b
-00006010: 6520 6465 7665 6c6f 7065 642e 2057 696c  e developed. Wil
-00006020: 6c20 7265 7475 726e 2031 2069 6620 616c  l return 1 if al
-00006030: 6c20 7468 6520 746f 6b65 6e73 2069 6e20  l the tokens in 
-00006040: 7370 616e 2061 7265 2070 6172 7420 6f66  span are part of
-00006050: 2061 2022 6675 7a7a 7922 2d74 6f6b 656e   a "fuzzy"-token
-00006060: 2d6d 6174 6368 6564 2065 6e74 2e5c 6e5c  -matched ent.\n\
-00006070: 6e54 6865 2066 6f6c 6c6f 7769 6e67 2060  nThe following `
-00006080: 446f 6360 2061 7474 7269 6275 7465 7320  Doc` attributes 
-00006090: 7265 6665 7265 6e63 6520 7468 6520 746f  reference the to
-000060a0: 6b65 6e20 6174 7472 6962 7574 6573 2069  ken attributes i
-000060b0: 6e63 6c75 6465 6420 696e 2074 6865 2064  ncluded in the d
-000060c0: 6f63 2e20 416c 6c20 6172 6520 696d 6d75  oc. All are immu
-000060d0: 7461 626c 653a 5c6e 5c6e 2d20 6073 7061  table:\n\n- `spa
-000060e0: 637a 7a5f 646f 6360 3a20 6465 6661 756c  czz_doc`: defaul
-000060f0: 7420 3d20 6046 616c 7365 602e 2042 6f6f  t = `False`. Boo
-00006100: 6c65 616e 2074 6861 7420 6465 6e6f 7465  lean that denote
-00006110: 7320 6966 2061 6e79 2074 6f6b 656e 7320  s if any tokens 
-00006120: 696e 2074 6865 2064 6f63 2061 7265 2070  in the doc are p
-00006130: 6172 7420 6f66 2061 6e20 656e 7420 7365  art of an ent se
-00006140: 7420 6279 2074 6865 2073 7061 637a 7a20  t by the spaczz 
-00006150: 7275 6c65 722e 5c6e 2d20 6073 7061 637a  ruler.\n- `spacz
-00006160: 7a5f 7479 7065 7360 3a20 6465 6661 756c  z_types`: defaul
-00006170: 7420 3d20 6073 6574 2829 602e 2053 6574  t = `set()`. Set
-00006180: 2074 6861 7420 7368 6f77 7320 7768 6963   that shows whic
-00006190: 6820 6d61 7463 6865 7273 2070 726f 6475  h matchers produ
-000061a0: 6365 6420 656e 7473 2069 6e20 7468 6520  ced ents in the 
-000061b0: 646f 632e 5c6e 5c6e 2323 2320 5361 7669  doc.\n\n### Savi
-000061c0: 6e67 2f4c 6f61 6469 6e67 5c6e 5c6e 5468  ng/Loading\n\nTh
-000061d0: 6520 6053 7061 637a 7a52 756c 6572 6020  e `SpaczzRuler` 
-000061e0: 6861 7320 6974 5c27 7320 6f77 6e20 746f  has it\'s own to
-000061f0: 2f66 726f 6d20 6469 736b 2f62 7974 6573  /from disk/bytes
-00006200: 206d 6574 686f 6473 2061 6e64 2077 696c   methods and wil
-00006210: 6c20 6163 6365 7074 2060 636f 6e66 6967  l accept `config
-00006220: 6020 7061 7261 6d65 7465 7273 2070 6173  ` parameters pas
-00006230: 7365 6420 746f 2060 7370 6163 792e 6c6f  sed to `spacy.lo
-00006240: 6164 2829 602e 2049 7420 616c 736f 2068  ad()`. It also h
-00006250: 6173 2069 745c 2773 206f 776e 2073 7061  as it\'s own spa
-00006260: 4379 2066 6163 746f 7279 2065 6e74 7279  Cy factory entry
-00006270: 2070 6f69 6e74 2073 6f20 7370 6143 7920   point so spaCy 
-00006280: 6973 2061 7761 7265 206f 6620 7468 6520  is aware of the 
-00006290: 6053 7061 637a 7a52 756c 6572 602e 2042  `SpaczzRuler`. B
-000062a0: 656c 6f77 2069 7320 616e 2065 7861 6d70  elow is an examp
-000062b0: 6c65 206f 6620 7361 7669 6e67 2061 6e64  le of saving and
-000062c0: 206c 6f61 6469 6e67 2061 2073 7061 6379   loading a spacy
-000062d0: 2070 6970 656c 696e 6520 7769 7468 2074   pipeline with t
-000062e0: 6865 2073 6d61 6c6c 2045 6e67 6c69 7368  he small English
-000062f0: 206d 6f64 656c 2c20 7468 6520 6045 6e74   model, the `Ent
-00006300: 6974 7952 756c 6572 602c 2061 6e64 2074  ityRuler`, and t
-00006310: 6865 2060 5370 6163 7a7a 5275 6c65 7260  he `SpaczzRuler`
-00006320: 2e5c 6e5c 6e5c 6e60 6060 7079 7468 6f6e  .\n\n\n```python
-00006330: 5c6e 696d 706f 7274 2073 7061 6379 5c6e  \nimport spacy\n
-00006340: 6672 6f6d 2073 7061 637a 7a2e 7069 7065  from spaczz.pipe
-00006350: 6c69 6e65 2069 6d70 6f72 7420 5370 6163  line import Spac
-00006360: 7a7a 5275 6c65 725c 6e5c 6e6e 6c70 203d  zzRuler\n\nnlp =
-00006370: 2073 7061 6379 2e6c 6f61 6428 2265 6e5f   spacy.load("en_
-00006380: 636f 7265 5f77 6562 5f73 6d22 295c 6e74  core_web_sm")\nt
-00006390: 6578 7420 3d20 2222 2241 6e64 6572 736f  ext = """Anderso
-000063a0: 6e2c 2047 7269 6e74 2063 7265 6174 6564  n, Grint created
-000063b0: 2073 7061 637a 7a20 696e 2068 6973 2068   spaczz in his h
-000063c0: 6f6d 6520 6174 2035 3535 2046 616b 6520  ome at 555 Fake 
-000063d0: 5374 2c5c 6e41 7074 2035 2069 6e20 4e61  St,\nApt 5 in Na
-000063e0: 7368 7631 6c65 2c20 544e 2035 3535 3535  shv1le, TN 55555
-000063f0: 2d31 3233 3420 696e 2074 6865 2055 5341  -1234 in the USA
-00006400: 2e5c 6e53 6f6d 6520 6f66 2068 6973 2066  .\nSome of his f
-00006410: 6176 6f72 6974 6520 6261 6e64 7320 6172  avorite bands ar
-00006420: 6520 436f 6e76 6572 6720 616e 6420 5072  e Converg and Pr
-00006430: 6f74 6574 2074 6865 205a 6572 6f2e 2222  otet the Zero.""
-00006440: 2220 2023 2053 7065 6c6c 696e 6720 6572  "  # Spelling er
-00006450: 726f 7273 2069 6e74 656e 7469 6f6e 616c  rors intentional
-00006460: 2e5c 6e64 6f63 203d 206e 6c70 2874 6578  .\ndoc = nlp(tex
-00006470: 7429 5c6e 5c6e 666f 7220 656e 7420 696e  t)\n\nfor ent in
-00006480: 2064 6f63 2e65 6e74 733a 5c6e 2020 2020   doc.ents:\n    
-00006490: 7072 696e 7428 2865 6e74 2e74 6578 742c  print((ent.text,
-000064a0: 2065 6e74 2e73 7461 7274 2c20 656e 742e   ent.start, ent.
-000064b0: 656e 642c 2065 6e74 2e6c 6162 656c 5f29  end, ent.label_)
-000064c0: 295c 6e60 6060 5c6e 5c6e 2020 2020 285c  )\n```\n\n    (\
-000064d0: 2741 6e64 6572 736f 6e5c 272c 2030 2c20  'Anderson\', 0, 
-000064e0: 312c 205c 2750 4552 534f 4e5c 2729 5c6e  1, \'PERSON\')\n
-000064f0: 2020 2020 285c 2747 7269 6e74 5c27 2c20      (\'Grint\', 
-00006500: 322c 2033 2c20 5c27 5045 5253 4f4e 5c27  2, 3, \'PERSON\'
-00006510: 295c 6e20 2020 2028 5c27 3535 355c 272c  )\n    (\'555\',
-00006520: 2039 2c20 3130 2c20 5c27 4341 5244 494e   9, 10, \'CARDIN
-00006530: 414c 5c27 295c 6e20 2020 2028 5c27 355c  AL\')\n    (\'5\
-00006540: 272c 2031 352c 2031 362c 205c 2743 4152  ', 15, 16, \'CAR
-00006550: 4449 4e41 4c5c 2729 5c6e 2020 2020 285c  DINAL\')\n    (\
-00006560: 2754 4e20 3535 3535 352d 3132 3334 5c27  'TN 55555-1234\'
-00006570: 2c20 3139 2c20 3233 2c20 5c27 4441 5445  , 19, 23, \'DATE
-00006580: 5c27 295c 6e20 2020 2028 5c27 5553 415c  \')\n    (\'USA\
-00006590: 272c 2032 352c 2032 362c 205c 2747 5045  ', 25, 26, \'GPE
-000065a0: 5c27 295c 6e20 2020 2028 5c27 436f 6e76  \')\n    (\'Conv
-000065b0: 6572 675c 272c 2033 342c 2033 352c 205c  erg\', 34, 35, \
-000065c0: 2750 4552 534f 4e5c 2729 5c6e 2020 2020  'PERSON\')\n    
-000065d0: 285c 2750 726f 7465 745c 272c 2033 362c  (\'Protet\', 36,
-000065e0: 2033 372c 205c 2750 4552 534f 4e5c 2729   37, \'PERSON\')
-000065f0: 5c6e 5c6e 5c6e 5768 696c 6520 7370 6143  \n\n\nWhile spaC
-00006600: 7920 646f 6573 2061 2064 6563 656e 7420  y does a decent 
-00006610: 6a6f 6220 6f66 2069 6465 6e74 6966 7969  job of identifyi
-00006620: 6e67 2074 6861 7420 6e61 6d65 6420 656e  ng that named en
-00006630: 7469 7469 6573 2061 7265 2070 7265 7365  tities are prese
-00006640: 6e74 2069 6e20 7468 6973 2065 7861 6d70  nt in this examp
-00006650: 6c65 2c20 7765 2063 616e 2064 6566 696e  le, we can defin
-00006660: 6974 656c 7920 696d 7072 6f76 6520 7468  itely improve th
-00006670: 6520 6d61 7463 6865 7320 2d20 7061 7274  e matches - part
-00006680: 6963 756c 6172 6c79 2077 6974 6820 7468  icularly with th
-00006690: 6520 7479 7065 7320 6f66 206c 6162 656c  e types of label
-000066a0: 7320 6170 706c 6965 642e 5c6e 5c6e 4c65  s applied.\n\nLe
-000066b0: 745c 2773 2061 6464 2061 6e20 656e 7469  t\'s add an enti
-000066c0: 7479 2072 756c 6572 2066 6f72 2073 6f6d  ty ruler for som
-000066d0: 6520 7275 6c65 732d 6261 7365 6420 6d61  e rules-based ma
-000066e0: 7463 6865 732e 5c6e 5c6e 5c6e 6060 6070  tches.\n\n\n```p
-000066f0: 7974 686f 6e5c 6e66 726f 6d20 7370 6163  ython\nfrom spac
-00006700: 792e 7069 7065 6c69 6e65 2069 6d70 6f72  y.pipeline impor
-00006710: 7420 456e 7469 7479 5275 6c65 725c 6e5c  t EntityRuler\n\
-00006720: 6e65 6e74 6974 795f 7275 6c65 7220 3d20  nentity_ruler = 
-00006730: 6e6c 702e 6164 645f 7069 7065 2822 656e  nlp.add_pipe("en
-00006740: 7469 7479 5f72 756c 6572 222c 2062 6566  tity_ruler", bef
-00006750: 6f72 653d 226e 6572 2229 2023 7370 6143  ore="ner") #spaC
-00006760: 7920 7633 2073 796e 7461 785c 6e65 6e74  y v3 syntax\nent
-00006770: 6974 795f 7275 6c65 722e 6164 645f 7061  ity_ruler.add_pa
-00006780: 7474 6572 6e73 285c 6e20 2020 205b 7b22  tterns(\n    [{"
-00006790: 6c61 6265 6c22 3a20 2247 5045 222c 2022  label": "GPE", "
-000067a0: 7061 7474 6572 6e22 3a20 224e 6173 6876  pattern": "Nashv
-000067b0: 696c 6c65 227d 2c20 7b22 6c61 6265 6c22  ille"}, {"label"
-000067c0: 3a20 2247 5045 222c 2022 7061 7474 6572  : "GPE", "patter
-000067d0: 6e22 3a20 2254 4e22 7d5d 5c6e 295c 6e5c  n": "TN"}]\n)\n\
-000067e0: 6e64 6f63 203d 206e 6c70 2874 6578 7429  ndoc = nlp(text)
-000067f0: 5c6e 5c6e 666f 7220 656e 7420 696e 2064  \n\nfor ent in d
-00006800: 6f63 2e65 6e74 733a 5c6e 2020 2020 7072  oc.ents:\n    pr
-00006810: 696e 7428 2865 6e74 2e74 6578 742c 2065  int((ent.text, e
-00006820: 6e74 2e73 7461 7274 2c20 656e 742e 656e  nt.start, ent.en
-00006830: 642c 2065 6e74 2e6c 6162 656c 5f29 295c  d, ent.label_))\
-00006840: 6e60 6060 5c6e 5c6e 2020 2020 285c 2741  n```\n\n    (\'A
-00006850: 6e64 6572 736f 6e5c 272c 2030 2c20 312c  nderson\', 0, 1,
-00006860: 205c 2750 4552 534f 4e5c 2729 5c6e 2020   \'PERSON\')\n  
-00006870: 2020 285c 2747 7269 6e74 5c27 2c20 322c    (\'Grint\', 2,
-00006880: 2033 2c20 5c27 5045 5253 4f4e 5c27 295c   3, \'PERSON\')\
-00006890: 6e20 2020 2028 5c27 3535 355c 272c 2039  n    (\'555\', 9
-000068a0: 2c20 3130 2c20 5c27 4341 5244 494e 414c  , 10, \'CARDINAL
-000068b0: 5c27 295c 6e20 2020 2028 5c27 355c 272c  \')\n    (\'5\',
-000068c0: 2031 352c 2031 362c 205c 2743 4152 4449   15, 16, \'CARDI
-000068d0: 4e41 4c5c 2729 5c6e 2020 2020 285c 2754  NAL\')\n    (\'T
-000068e0: 4e5c 272c 2031 392c 2032 302c 205c 2747  N\', 19, 20, \'G
-000068f0: 5045 5c27 295c 6e20 2020 2028 5c27 5553  PE\')\n    (\'US
-00006900: 415c 272c 2032 352c 2032 362c 205c 2747  A\', 25, 26, \'G
-00006910: 5045 5c27 295c 6e20 2020 2028 5c27 436f  PE\')\n    (\'Co
-00006920: 6e76 6572 675c 272c 2033 342c 2033 352c  nverg\', 34, 35,
-00006930: 205c 2750 4552 534f 4e5c 2729 5c6e 2020   \'PERSON\')\n  
-00006940: 2020 285c 2750 726f 7465 745c 272c 2033    (\'Protet\', 3
-00006950: 362c 2033 372c 205c 2750 4552 534f 4e5c  6, 37, \'PERSON\
-00006960: 2729 5c6e 5c6e 5c6e 5765 5c27 7265 206d  ')\n\n\nWe\'re m
-00006970: 616b 696e 6720 7072 6f67 7265 7373 2c20  aking progress, 
-00006980: 6275 7420 4e61 7368 7669 6c6c 6520 6973  but Nashville is
-00006990: 2073 7065 6c6c 6564 2077 726f 6e67 2069   spelled wrong i
-000069a0: 6e20 7468 6520 7465 7874 2073 6f20 7468  n the text so th
-000069b0: 6520 656e 7469 7479 2072 756c 6572 2064  e entity ruler d
-000069c0: 6f65 7320 6e6f 7420 6669 6e64 2069 742c  oes not find it,
-000069d0: 2061 6e64 2077 6520 7374 696c 6c20 6861   and we still ha
-000069e0: 7665 206f 7468 6572 2065 6e74 6974 6965  ve other entitie
-000069f0: 7320 746f 2066 6978 2f66 696e 642e 5c6e  s to fix/find.\n
-00006a00: 5c6e 4c65 745c 2773 2061 6464 2061 2073  \nLet\'s add a s
-00006a10: 7061 637a 7a20 7275 6c65 7220 746f 2072  paczz ruler to r
-00006a20: 6f75 6e64 2074 6869 7320 7069 7065 6c69  ound this pipeli
-00006a30: 6e65 206f 7574 2e20 5765 2077 696c 6c20  ne out. We will 
-00006a40: 616c 736f 2069 6e63 6c75 6465 2074 6865  also include the
-00006a50: 2060 7370 6163 7a7a 5f73 7061 6e60 2063   `spaczz_span` c
-00006a60: 7573 746f 6d20 6174 7472 6962 7574 6520  ustom attribute 
-00006a70: 696e 2074 6865 2072 6573 756c 7473 2074  in the results t
-00006a80: 6f20 6465 6e6f 7465 2077 6869 6368 2065  o denote which e
-00006a90: 6e74 6974 6965 7320 7765 7265 2073 6574  ntities were set
-00006aa0: 2076 6961 2073 7061 637a 7a2e 5c6e 5c6e   via spaczz.\n\n
-00006ab0: 5c6e 6060 6070 7974 686f 6e5c 6e73 7061  \n```python\nspa
-00006ac0: 637a 7a5f 7275 6c65 7220 3d20 6e6c 702e  czz_ruler = nlp.
-00006ad0: 6164 645f 7069 7065 2822 7370 6163 7a7a  add_pipe("spaczz
-00006ae0: 5f72 756c 6572 222c 2062 6566 6f72 653d  _ruler", before=
-00006af0: 226e 6572 2229 2023 7370 6143 7920 7633  "ner") #spaCy v3
-00006b00: 2073 796e 7461 785c 6e73 7061 637a 7a5f   syntax\nspaczz_
-00006b10: 7275 6c65 722e 6164 645f 7061 7474 6572  ruler.add_patter
-00006b20: 6e73 285c 6e20 2020 205b 5c6e 2020 2020  ns(\n    [\n    
-00006b30: 2020 2020 7b5c 6e20 2020 2020 2020 2020      {\n         
-00006b40: 2020 2022 6c61 6265 6c22 3a20 224e 414d     "label": "NAM
-00006b50: 4522 2c5c 6e20 2020 2020 2020 2020 2020  E",\n           
-00006b60: 2022 7061 7474 6572 6e22 3a20 2247 7261   "pattern": "Gra
-00006b70: 6e74 2041 6e64 6572 7365 6e22 2c5c 6e20  nt Andersen",\n 
-00006b80: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-00006b90: 223a 2022 6675 7a7a 7922 2c5c 6e20 2020  ": "fuzzy",\n   
-00006ba0: 2020 2020 2020 2020 2022 6b77 6172 6773           "kwargs
-00006bb0: 223a 207b 2266 757a 7a79 5f66 756e 6322  ": {"fuzzy_func"
-00006bc0: 3a20 2274 6f6b 656e 5f73 6f72 7422 7d2c  : "token_sort"},
-00006bd0: 5c6e 2020 2020 2020 2020 7d2c 5c6e 2020  \n        },\n  
-00006be0: 2020 2020 2020 7b5c 6e20 2020 2020 2020        {\n       
-00006bf0: 2020 2020 2022 6c61 6265 6c22 3a20 2253       "label": "S
-00006c00: 5452 4545 5422 2c5c 6e20 2020 2020 2020  TREET",\n       
-00006c10: 2020 2020 2022 7061 7474 6572 6e22 3a20       "pattern": 
-00006c20: 2273 7472 6565 745f 6164 6472 6573 7365  "street_addresse
-00006c30: 7322 2c5c 6e20 2020 2020 2020 2020 2020  s",\n           
-00006c40: 2022 7479 7065 223a 2022 7265 6765 7822   "type": "regex"
-00006c50: 2c5c 6e20 2020 2020 2020 2020 2020 2022  ,\n            "
-00006c60: 6b77 6172 6773 223a 207b 2270 7265 6465  kwargs": {"prede
-00006c70: 6622 3a20 5472 7565 7d2c 5c6e 2020 2020  f": True},\n    
-00006c80: 2020 2020 7d2c 5c6e 2020 2020 2020 2020      },\n        
-00006c90: 7b22 6c61 6265 6c22 3a20 2247 5045 222c  {"label": "GPE",
-00006ca0: 2022 7061 7474 6572 6e22 3a20 224e 6173   "pattern": "Nas
-00006cb0: 6876 696c 6c65 222c 2022 7479 7065 223a  hville", "type":
-00006cc0: 2022 6675 7a7a 7922 7d2c 5c6e 2020 2020   "fuzzy"},\n    
-00006cd0: 2020 2020 7b5c 6e20 2020 2020 2020 2020      {\n         
-00006ce0: 2020 2022 6c61 6265 6c22 3a20 225a 4950     "label": "ZIP
-00006cf0: 222c 5c6e 2020 2020 2020 2020 2020 2020  ",\n            
-00006d00: 2270 6174 7465 726e 223a 2072 225c 5c62  "pattern": r"\\b
-00006d10: 283f 3a35 3535 3534 297b 733c 3d31 7d28  (?:55554){s<=1}(
-00006d20: 3f3a 5b2d 5c5c 735d 5c5c 647b 347d 293f  ?:[-\\s]\\d{4})?
-00006d30: 5c5c 6222 2c5c 6e20 2020 2020 2020 2020  \\b",\n         
-00006d40: 2020 2022 7479 7065 223a 2022 7265 6765     "type": "rege
-00006d50: 7822 2c5c 6e20 2020 2020 2020 207d 2c20  x",\n        }, 
-00006d60: 2023 2066 757a 7a79 2072 6567 6578 5c6e   # fuzzy regex\n
-00006d70: 2020 2020 2020 2020 7b5c 6e20 2020 2020          {\n     
-00006d80: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00006d90: 2242 414e 4422 2c5c 6e20 2020 2020 2020  "BAND",\n       
-00006da0: 2020 2020 2022 7061 7474 6572 6e22 3a20       "pattern": 
-00006db0: 5b7b 224c 4f57 4552 223a 207b 2246 5245  [{"LOWER": {"FRE
-00006dc0: 4745 5822 3a20 2228 636f 6e76 6572 6765  GEX": "(converge
-00006dd0: 297b 653c 3d31 7d22 7d7d 5d2c 5c6e 2020  ){e<=1}"}}],\n  
-00006de0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00006df0: 3a20 2274 6f6b 656e 222c 5c6e 2020 2020  : "token",\n    
-00006e00: 2020 2020 7d2c 5c6e 2020 2020 2020 2020      },\n        
-00006e10: 7b5c 6e20 2020 2020 2020 2020 2020 2022  {\n            "
-00006e20: 6c61 6265 6c22 3a20 2242 414e 4422 2c5c  label": "BAND",\
-00006e30: 6e20 2020 2020 2020 2020 2020 2022 7061  n            "pa
-00006e40: 7474 6572 6e22 3a20 5b5c 6e20 2020 2020  ttern": [\n     
-00006e50: 2020 2020 2020 2020 2020 207b 2254 4558             {"TEX
-00006e60: 5422 3a20 7b22 4655 5a5a 5922 3a20 2250  T": {"FUZZY": "P
-00006e70: 726f 7465 7374 227d 7d2c 5c6e 2020 2020  rotest"}},\n    
-00006e80: 2020 2020 2020 2020 2020 2020 7b22 4953              {"IS
-00006e90: 5f53 544f 5022 3a20 5472 7565 7d2c 5c6e  _STOP": True},\n
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 7b22 5445 5854 223a 207b 2246 555a 5a59  {"TEXT": {"FUZZY
-00006ec0: 223a 2022 4865 726f 227d 7d2c 5c6e 2020  ": "Hero"}},\n  
-00006ed0: 2020 2020 2020 2020 2020 5d2c 5c6e 2020            ],\n  
-00006ee0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00006ef0: 3a20 2274 6f6b 656e 222c 5c6e 2020 2020  : "token",\n    
-00006f00: 2020 2020 7d2c 5c6e 2020 2020 5d5c 6e29      },\n    ]\n)
-00006f10: 5c6e 5c6e 646f 6320 3d20 6e6c 7028 7465  \n\ndoc = nlp(te
-00006f20: 7874 295c 6e5c 6e66 6f72 2065 6e74 2069  xt)\n\nfor ent i
-00006f30: 6e20 646f 632e 656e 7473 3a5c 6e20 2020  n doc.ents:\n   
-00006f40: 2070 7269 6e74 2828 656e 742e 7465 7874   print((ent.text
-00006f50: 2c20 656e 742e 7374 6172 742c 2065 6e74  , ent.start, ent
-00006f60: 2e65 6e64 2c20 656e 742e 6c61 6265 6c5f  .end, ent.label_
-00006f70: 2c20 656e 742e 5f2e 7370 6163 7a7a 5f65  , ent._.spaczz_e
-00006f80: 6e74 2929 5c6e 6060 605c 6e5c 6e20 2020  nt))\n```\n\n   
-00006f90: 2028 5c27 416e 6465 7273 6f6e 2c20 4772   (\'Anderson, Gr
-00006fa0: 696e 745c 272c 2030 2c20 332c 205c 274e  int\', 0, 3, \'N
-00006fb0: 414d 455c 272c 2054 7275 6529 5c6e 2020  AME\', True)\n  
-00006fc0: 2020 285c 2735 3535 2046 616b 6520 5374    (\'555 Fake St
-00006fd0: 2c5c 272c 2039 2c20 3133 2c20 5c27 5354  ,\', 9, 13, \'ST
-00006fe0: 5245 4554 5c27 2c20 5472 7565 295c 6e20  REET\', True)\n 
-00006ff0: 2020 2028 5c27 355c 272c 2031 352c 2031     (\'5\', 15, 1
-00007000: 362c 205c 2743 4152 4449 4e41 4c5c 272c  6, \'CARDINAL\',
-00007010: 2046 616c 7365 295c 6e20 2020 2028 5c27   False)\n    (\'
-00007020: 4e61 7368 7631 6c65 5c27 2c20 3137 2c20  Nashv1le\', 17, 
-00007030: 3138 2c20 5c27 4750 455c 272c 2054 7275  18, \'GPE\', Tru
-00007040: 6529 5c6e 2020 2020 285c 2754 4e5c 272c  e)\n    (\'TN\',
-00007050: 2031 392c 2032 302c 205c 2747 5045 5c27   19, 20, \'GPE\'
-00007060: 2c20 4661 6c73 6529 5c6e 2020 2020 285c  , False)\n    (\
-00007070: 2735 3535 3535 2d31 3233 345c 272c 2032  '55555-1234\', 2
-00007080: 302c 2032 332c 205c 275a 4950 5c27 2c20  0, 23, \'ZIP\', 
-00007090: 5472 7565 295c 6e20 2020 2028 5c27 5553  True)\n    (\'US
-000070a0: 415c 272c 2032 352c 2032 362c 205c 2747  A\', 25, 26, \'G
-000070b0: 5045 5c27 2c20 4661 6c73 6529 5c6e 2020  PE\', False)\n  
-000070c0: 2020 285c 2743 6f6e 7665 7267 5c27 2c20    (\'Converg\', 
-000070d0: 3334 2c20 3335 2c20 5c27 4241 4e44 5c27  34, 35, \'BAND\'
-000070e0: 2c20 5472 7565 295c 6e20 2020 2028 5c27  , True)\n    (\'
-000070f0: 5072 6f74 6574 2074 6865 205a 6572 6f5c  Protet the Zero\
-00007100: 272c 2033 362c 2033 392c 205c 2742 414e  ', 36, 39, \'BAN
-00007110: 445c 272c 2054 7275 6529 5c6e 5c6e 5c6e  D\', True)\n\n\n
-00007120: 4177 6573 6f6d 6521 2054 6865 2073 6d61  Awesome! The sma
-00007130: 6c6c 2045 6e67 6c69 7368 206d 6f64 656c  ll English model
-00007140: 2073 7469 6c6c 206d 616b 6573 2061 206e   still makes a n
-00007150: 616d 6564 2065 6e74 6974 7920 7265 636f  amed entity reco
-00007160: 676e 6974 696f 6e20 6d69 7374 616b 6520  gnition mistake 
-00007170: 2822 3522 2069 6e20 2241 7074 2035 2220  ("5" in "Apt 5" 
-00007180: 6173 2060 4341 5244 494e 414c 6029 2c20  as `CARDINAL`), 
-00007190: 6275 7420 7765 5c27 7265 2073 6174 6973  but we\'re satis
-000071a0: 6669 6564 206f 7665 7261 6c6c 2e5c 6e5c  fied overall.\n\
-000071b0: 6e4c 6574 5c27 7320 7361 7665 2074 6869  nLet\'s save thi
-000071c0: 7320 7069 7065 6c69 6e65 2074 6f20 6469  s pipeline to di
-000071d0: 736b 2061 6e64 206d 616b 6520 7375 7265  sk and make sure
-000071e0: 2077 6520 6361 6e20 6c6f 6164 2069 7420   we can load it 
-000071f0: 6261 636b 2063 6f72 7265 6374 6c79 2e5c  back correctly.\
-00007200: 6e5c 6e5c 6e60 6060 7079 7468 6f6e 5c6e  n\n\n```python\n
-00007210: 6e6c 702e 746f 5f64 6973 6b28 222e 2f65  nlp.to_disk("./e
-00007220: 7861 6d70 6c65 2229 5c6e 6e6c 7020 3d20  xample")\nnlp = 
-00007230: 7370 6163 792e 6c6f 6164 2822 2e2f 6578  spacy.load("./ex
-00007240: 616d 706c 6522 295c 6e6e 6c70 2e70 6970  ample")\nnlp.pip
-00007250: 655f 6e61 6d65 735c 6e60 6060 5c6e 5c6e  e_names\n```\n\n
-00007260: 5c6e 5c6e 5c6e 2020 2020 5b5c 2774 6f6b  \n\n\n    [\'tok
-00007270: 3276 6563 5c27 2c5c 6e20 2020 2020 5c27  2vec\',\n     \'
-00007280: 7461 6767 6572 5c27 2c5c 6e20 2020 2020  tagger\',\n     
-00007290: 5c27 7061 7273 6572 5c27 2c5c 6e20 2020  \'parser\',\n   
-000072a0: 2020 5c27 656e 7469 7479 5f72 756c 6572    \'entity_ruler
-000072b0: 5c27 2c5c 6e20 2020 2020 5c27 7370 6163  \',\n     \'spac
-000072c0: 7a7a 5f72 756c 6572 5c27 2c5c 6e20 2020  zz_ruler\',\n   
-000072d0: 2020 5c27 6e65 725c 272c 5c6e 2020 2020    \'ner\',\n    
-000072e0: 205c 2761 7474 7269 6275 7465 5f72 756c   \'attribute_rul
-000072f0: 6572 5c27 2c5c 6e20 2020 2020 5c27 6c65  er\',\n     \'le
-00007300: 6d6d 6174 697a 6572 5c27 5d5c 6e5c 6e5c  mmatizer\']\n\n\
-00007310: 6e5c 6e57 6520 6361 6e20 6576 656e 2065  n\nWe can even e
-00007320: 6e73 7572 6520 616c 6c20 7468 6520 7370  nsure all the sp
-00007330: 6163 7a7a 2072 756c 6572 2070 6174 7465  aczz ruler patte
-00007340: 726e 7320 6172 6520 7374 696c 6c20 7072  rns are still pr
-00007350: 6573 656e 742e 5c6e 5c6e 5c6e 6060 6070  esent.\n\n\n```p
-00007360: 7974 686f 6e5c 6e73 7061 637a 7a5f 7275  ython\nspaczz_ru
-00007370: 6c65 7220 3d20 6e6c 702e 6765 745f 7069  ler = nlp.get_pi
-00007380: 7065 2822 7370 6163 7a7a 5f72 756c 6572  pe("spaczz_ruler
-00007390: 2229 5c6e 7370 6163 7a7a 5f72 756c 6572  ")\nspaczz_ruler
-000073a0: 2e70 6174 7465 726e 735c 6e60 6060 5c6e  .patterns\n```\n
-000073b0: 5c6e 5c6e 5c6e 5c6e 2020 2020 5b7b 5c27  \n\n\n\n    [{\'
-000073c0: 6c61 6265 6c5c 273a 205c 274e 414d 455c  label\': \'NAME\
-000073d0: 272c 5c6e 2020 2020 2020 5c27 7061 7474  ',\n      \'patt
-000073e0: 6572 6e5c 273a 205c 2747 7261 6e74 2041  ern\': \'Grant A
-000073f0: 6e64 6572 7365 6e5c 272c 5c6e 2020 2020  ndersen\',\n    
-00007400: 2020 5c27 7479 7065 5c27 3a20 5c27 6675    \'type\': \'fu
-00007410: 7a7a 795c 272c 5c6e 2020 2020 2020 5c27  zzy\',\n      \'
-00007420: 6b77 6172 6773 5c27 3a20 7b5c 2766 757a  kwargs\': {\'fuz
-00007430: 7a79 5f66 756e 635c 273a 205c 2774 6f6b  zy_func\': \'tok
-00007440: 656e 5f73 6f72 745c 277d 7d2c 5c6e 2020  en_sort\'}},\n  
-00007450: 2020 207b 5c27 6c61 6265 6c5c 273a 205c     {\'label\': \
-00007460: 2747 5045 5c27 2c20 5c27 7061 7474 6572  'GPE\', \'patter
-00007470: 6e5c 273a 205c 274e 6173 6876 696c 6c65  n\': \'Nashville
-00007480: 5c27 2c20 5c27 7479 7065 5c27 3a20 5c27  \', \'type\': \'
-00007490: 6675 7a7a 795c 277d 2c5c 6e20 2020 2020  fuzzy\'},\n     
-000074a0: 7b5c 276c 6162 656c 5c27 3a20 5c27 5354  {\'label\': \'ST
-000074b0: 5245 4554 5c27 2c5c 6e20 2020 2020 205c  REET\',\n      \
-000074c0: 2770 6174 7465 726e 5c27 3a20 5c27 7374  'pattern\': \'st
-000074d0: 7265 6574 5f61 6464 7265 7373 6573 5c27  reet_addresses\'
-000074e0: 2c5c 6e20 2020 2020 205c 2774 7970 655c  ,\n      \'type\
-000074f0: 273a 205c 2772 6567 6578 5c27 2c5c 6e20  ': \'regex\',\n 
-00007500: 2020 2020 205c 276b 7761 7267 735c 273a       \'kwargs\':
-00007510: 207b 5c27 7072 6564 6566 5c27 3a20 5472   {\'predef\': Tr
-00007520: 7565 7d7d 2c5c 6e20 2020 2020 7b5c 276c  ue}},\n     {\'l
-00007530: 6162 656c 5c27 3a20 5c27 5a49 505c 272c  abel\': \'ZIP\',
-00007540: 5c6e 2020 2020 2020 5c27 7061 7474 6572  \n      \'patter
-00007550: 6e5c 273a 205c 275c 5c5c 5c62 283f 3a35  n\': \'\\\\b(?:5
-00007560: 3535 3534 297b 733c 3d31 7d28 3f3a 5b2d  5554){s<=1}(?:[-
-00007570: 5c5c 5c5c 735d 5c5c 5c5c 647b 347d 293f  \\\\s]\\\\d{4})?
-00007580: 5c5c 5c5c 625c 272c 5c6e 2020 2020 2020  \\\\b\',\n      
-00007590: 5c27 7479 7065 5c27 3a20 5c27 7265 6765  \'type\': \'rege
-000075a0: 785c 277d 2c5c 6e20 2020 2020 7b5c 276c  x\'},\n     {\'l
-000075b0: 6162 656c 5c27 3a20 5c27 4241 4e44 5c27  abel\': \'BAND\'
-000075c0: 2c5c 6e20 2020 2020 205c 2770 6174 7465  ,\n      \'patte
-000075d0: 726e 5c27 3a20 5b7b 5c27 4c4f 5745 525c  rn\': [{\'LOWER\
-000075e0: 273a 207b 5c27 4652 4547 4558 5c27 3a20  ': {\'FREGEX\': 
-000075f0: 5c27 2863 6f6e 7665 7267 6529 7b65 3c3d  \'(converge){e<=
-00007600: 317d 5c27 7d7d 5d2c 5c6e 2020 2020 2020  1}\'}}],\n      
-00007610: 5c27 7479 7065 5c27 3a20 5c27 746f 6b65  \'type\': \'toke
-00007620: 6e5c 277d 2c5c 6e20 2020 2020 7b5c 276c  n\'},\n     {\'l
-00007630: 6162 656c 5c27 3a20 5c27 4241 4e44 5c27  abel\': \'BAND\'
-00007640: 2c5c 6e20 2020 2020 205c 2770 6174 7465  ,\n      \'patte
-00007650: 726e 5c27 3a20 5b7b 5c27 5445 5854 5c27  rn\': [{\'TEXT\'
-00007660: 3a20 7b5c 2746 555a 5a59 5c27 3a20 5c27  : {\'FUZZY\': \'
-00007670: 5072 6f74 6573 745c 277d 7d2c 5c6e 2020  Protest\'}},\n  
-00007680: 2020 2020 207b 5c27 4953 5f53 544f 505c       {\'IS_STOP\
-00007690: 273a 2054 7275 657d 2c5c 6e20 2020 2020  ': True},\n     
-000076a0: 2020 7b5c 2754 4558 545c 273a 207b 5c27    {\'TEXT\': {\'
-000076b0: 4655 5a5a 595c 273a 205c 2748 6572 6f5c  FUZZY\': \'Hero\
-000076c0: 277d 7d5d 2c5c 6e20 2020 2020 205c 2774  '}}],\n      \'t
-000076d0: 7970 655c 273a 205c 2774 6f6b 656e 5c27  ype\': \'token\'
-000076e0: 7d5d 5c6e 5c6e 5c6e 5c6e 2323 204b 6e6f  }]\n\n\n\n## Kno
-000076f0: 776e 2049 7373 7565 735c 6e5c 6e23 2323  wn Issues\n\n###
-00007700: 2050 6572 666f 726d 616e 6365 5c6e 5c6e   Performance\n\n
-00007710: 5468 6520 6d61 696e 2072 6561 736f 6e20  The main reason 
-00007720: 666f 7220 7370 6163 7a7a 5c27 7320 736c  for spaczz\'s sl
-00007730: 6f77 6572 2073 7065 6564 2069 7320 7468  ower speed is th
-00007740: 6174 2074 6865 202a 632a 2069 6e20 6974  at the *c* in it
-00007750: 5c27 7320 6e61 6d65 2069 7320 6e6f 7420  \'s name is not 
-00007760: 6361 7069 7461 6c69 7a65 6420 6c69 6b65  capitalized like
-00007770: 2069 7420 6973 2069 6e20 7370 612a 432a   it is in spa*C*
-00007780: 792e 5c6e 5370 6163 7a7a 2069 7320 7772  y.\nSpaczz is wr
-00007790: 6974 7465 6e20 696e 2070 7572 6520 5079  itten in pure Py
-000077a0: 7468 6f6e 2061 6e64 2069 745c 2773 206d  thon and it\'s m
-000077b0: 6174 6368 6572 7320 646f 206e 6f74 2063  atchers do not c
-000077c0: 7572 7265 6e74 6c79 2075 7469 6c69 7a65  urrently utilize
-000077d0: 2073 7061 4379 206c 616e 6775 6167 6520   spaCy language 
-000077e0: 766f 6361 6275 6c61 7269 6573 2c20 7768  vocabularies, wh
-000077f0: 6963 6820 6d65 616e 7320 666f 6c6c 6f77  ich means follow
-00007800: 696e 6720 6974 5c27 7320 6c6f 6769 6320  ing it\'s logic 
-00007810: 7368 6f75 6c64 2062 6520 6561 7379 2074  should be easy t
-00007820: 6f20 7468 6f73 6520 6661 6d69 6c69 6172  o those familiar
-00007830: 2077 6974 6820 5079 7468 6f6e 2e20 486f   with Python. Ho
-00007840: 7765 7665 7220 7468 6973 206d 6561 6e73  wever this means
-00007850: 2073 7061 637a 7a20 636f 6d70 6f6e 656e   spaczz componen
-00007860: 7473 2077 696c 6c20 7275 6e20 736c 6f77  ts will run slow
-00007870: 6572 2061 6e64 206c 696b 656c 7920 636f  er and likely co
-00007880: 6e73 756d 6520 6d6f 7265 206d 656d 6f72  nsume more memor
-00007890: 7920 7468 616e 2074 6865 6972 2073 7061  y than their spa
-000078a0: 4379 2063 6f75 6e74 6572 7061 7274 732c  Cy counterparts,
-000078b0: 2065 7370 6563 6961 6c6c 7920 6173 206d   especially as m
-000078c0: 6f72 6520 7061 7474 6572 6e73 2061 7265  ore patterns are
-000078d0: 2061 6464 6564 2061 6e64 2064 6f63 756d   added and docum
-000078e0: 656e 7473 2067 6574 206c 6f6e 6765 722e  ents get longer.
-000078f0: 2049 7420 6973 2074 6865 7265 666f 7265   It is therefore
-00007900: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00007910: 7573 6520 7370 6143 7920 636f 6d70 6f6e  use spaCy compon
-00007920: 656e 7473 206c 696b 6520 7468 6520 456e  ents like the En
-00007930: 7469 7479 5275 6c65 7220 666f 7220 656e  tityRuler for en
-00007940: 7469 7469 6573 2077 6974 6820 6c69 7474  tities with litt
-00007950: 6c65 2075 6e63 6572 7461 696e 7479 2c20  le uncertainty, 
-00007960: 6c69 6b65 2063 6f6e 7369 7374 656e 7420  like consistent 
-00007970: 7370 656c 6c69 6e67 2065 7272 6f72 732e  spelling errors.
-00007980: 2055 7365 2073 7061 637a 7a20 636f 6d70   Use spaczz comp
-00007990: 6f6e 656e 7473 2077 6865 6e20 7468 6572  onents when ther
-000079a0: 6520 6172 6520 6e6f 7420 7669 6162 6c65  e are not viable
-000079b0: 2073 7061 4379 2061 6c74 6572 6e61 7469   spaCy alternati
-000079c0: 7665 732e 5c6e 5c6e 4920 616d 2061 6374  ves.\n\nI am act
-000079d0: 6976 656c 7920 776f 726b 696e 6720 6f6e  ively working on
-000079e0: 2070 6572 666f 726d 616e 6365 206f 7074   performance opt
-000079f0: 696d 697a 6174 696f 6e73 2074 6f20 7370  imizations to sp
-00007a00: 6163 7a7a 2062 7574 2069 7420 6973 2061  aczz but it is a
-00007a10: 2067 7261 6475 616c 2070 726f 6365 7373   gradual process
-00007a20: 2e20 416c 676f 7269 7468 6d69 6320 616e  . Algorithmic an
-00007a30: 6420 6f70 7469 6d69 7a61 7469 6f6e 2073  d optimization s
-00007a40: 7567 6765 7374 696f 6e73 2061 7265 2077  uggestions are w
-00007a50: 656c 636f 6d65 2e20 4920 616d 2077 6f72  elcome. I am wor
-00007a60: 6b69 6e67 206f 6e20 6c65 6172 6e69 6e67  king on learning
-00007a70: 2043 2062 7574 2063 7572 7265 6e74 6c79   C but currently
-00007a80: 2043 2d62 6173 6564 2077 6f72 6b20 6973   C-based work is
-00007a90: 206f 7574 7369 6465 206f 6620 6d79 2073   outside of my s
-00007aa0: 6b69 6c6c 2073 6574 2e5c 6e5c 6e54 6865  kill set.\n\nThe
-00007ab0: 2060 4675 7a7a 794d 6174 6368 6572 602c   `FuzzyMatcher`,
-00007ac0: 2061 6e64 2065 7665 6e20 6d6f 7265 2073   and even more s
-00007ad0: 6f2c 2074 6865 2060 5369 6d69 6c61 7269  o, the `Similari
-00007ae0: 7479 4d61 7463 6865 7260 2061 7265 2074  tyMatcher` are t
-00007af0: 6865 2073 6c6f 7765 7374 2073 7061 637a  he slowest spacz
-00007b00: 7a20 636f 6d70 6f6e 656e 7473 2028 616c  z components (al
-00007b10: 7468 6f75 6768 2061 6c6c 6f77 696e 6720  though allowing 
-00007b20: 666f 7220 656e 6f75 6768 2022 6675 7a7a  for enough "fuzz
-00007b30: 7922 206d 6174 6368 6573 2069 6e20 7468  y" matches in th
-00007b40: 6520 6052 6567 6578 4d61 7463 6865 7260  e `RegexMatcher`
-00007b50: 2063 616e 2067 6574 2072 6561 6c6c 7920   can get really 
-00007b60: 736c 6f77 2061 7320 7765 6c6c 292e 2054  slow as well). T
-00007b70: 6865 2070 7269 6d61 7279 206d 6574 686f  he primary metho
-00007b80: 6473 2066 6f72 2073 7065 6564 696e 6720  ds for speeding 
-00007b90: 7468 6573 6520 636f 6d70 6f6e 656e 7473  these components
-00007ba0: 2075 7020 6172 6520 6279 2064 6563 7265   up are by decre
-00007bb0: 6173 696e 6720 7468 6520 6066 6c65 7860  asing the `flex`
-00007bc0: 2070 6172 616d 6574 6572 2074 6f77 6172   parameter towar
-00007bd0: 6473 2060 3060 2c20 6f72 2069 6620 6066  ds `0`, or if `f
-00007be0: 6c65 7820 3e20 3060 2c20 696e 6372 6561  lex > 0`, increa
-00007bf0: 7369 6e67 2074 6865 2060 6d69 6e5f 7231  sing the `min_r1
-00007c00: 6020 7061 7261 6d65 7465 7220 746f 7761  ` parameter towa
-00007c10: 7264 7320 7468 6520 7661 6c75 6520 6f66  rds the value of
-00007c20: 2060 6d69 6e5f 7232 6020 616e 642f 6f72   `min_r2` and/or
-00007c30: 206c 6f77 6572 696e 6720 7468 6520 6074   lowering the `t
-00007c40: 6872 6573 6860 2070 6172 616d 6574 6572  hresh` parameter
-00007c50: 2074 6f77 6172 6473 2060 6d69 6e5f 7232   towards `min_r2
-00007c60: 602e 2042 6520 6177 6172 6520 7468 6174  `. Be aware that
-00007c70: 2061 6c6c 206f 6620 7468 6573 6520 2273   all of these "s
-00007c80: 7065 6564 2d75 7073 2220 636f 6d65 2061  peed-ups" come a
-00007c90: 7420 7468 6520 6f70 706f 7274 756e 6974  t the opportunit
-00007ca0: 7920 636f 7374 206f 6620 706f 7465 6e74  y cost of potent
-00007cb0: 6961 6c6c 7920 696d 7072 6f76 6564 206d  ially improved m
-00007cc0: 6174 6368 6573 2e5c 6e5c 6e41 7320 6d65  atches.\n\nAs me
-00007cd0: 6e74 696f 6e65 6420 696e 2074 6865 2060  ntioned in the `
-00007ce0: 5369 6d69 6c61 7269 7479 4d61 7463 6865  SimilarityMatche
-00007cf0: 7260 2064 6573 6372 6970 7469 6f6e 2c20  r` description, 
-00007d00: 7574 696c 697a 696e 6720 6120 4750 5520  utilizing a GPU 
-00007d10: 7769 6c6c 2061 6c73 6f20 6865 6c70 2073  will also help s
-00007d20: 7065 6564 2075 7020 6974 5c27 7320 6d61  peed up it\'s ma
-00007d30: 7463 6869 6e67 2070 726f 6365 7373 2e5c  tching process.\
-00007d40: 6e5c 6e49 2077 696c 6c20 6c69 6b65 6c79  n\nI will likely
-00007d50: 2074 7279 2074 6f20 6465 7665 6c6f 7020   try to develop 
-00007d60: 736f 6d65 2061 7574 6f6d 6174 6564 2061  some automated a
-00007d70: 6e64 2f6f 7220 6865 7572 6973 7469 632d  nd/or heuristic-
-00007d80: 6261 7365 6420 4150 4920 6f70 7469 6f6e  based API option
-00007d90: 7320 2877 6869 6c65 2072 6574 6169 6e69  s (while retaini
-00007da0: 6e67 2061 6c6c 2074 6865 2063 7572 7265  ng all the curre
-00007db0: 6e74 206f 7074 696f 6e73 2920 696e 2074  nt options) in t
-00007dc0: 6865 2066 7574 7572 6520 746f 2073 696d  he future to sim
-00007dd0: 706c 6966 7920 7468 6973 2022 7475 6e69  plify this "tuni
-00007de0: 6e67 2220 7072 6f63 6573 732e 5c6e 5c6e  ng" process.\n\n
-00007df0: 2323 2320 5370 6163 7a7a 5275 6c65 7220  ### SpaczzRuler 
-00007e00: 496e 636f 6e73 6973 7465 6e63 6965 735c  Inconsistencies\
-00007e10: 6e5c 6e54 6869 7320 6f6e 6520 6973 2070  n\nThis one is p
-00007e20: 6172 7469 6375 6c61 726c 7920 616e 6e6f  articularly anno
-00007e30: 7969 6e67 2066 6f72 206d 6520 6265 6361  ying for me beca
-00007e40: 7573 6520 4920 6275 696c 7420 6d79 7365  use I built myse
-00007e50: 6c66 2069 6e74 6f20 7468 6973 2068 6f6c  lf into this hol
-00007e60: 6520 7472 7969 6e67 2074 6f20 7375 7070  e trying to supp
-00007e70: 6f72 7420 746f 6f20 6d75 6368 2074 6f6f  ort too much too
-00007e80: 2066 6173 742e 2054 6861 7420 6265 696e   fast. That bein
-00007e90: 6720 7361 6964 2049 2068 6176 6520 6164  g said I have ad
-00007ea0: 6472 6573 7365 6420 6d75 6368 206f 6620  dressed much of 
-00007eb0: 7468 6973 2061 7320 6f66 2073 7061 637a  this as of spacz
-00007ec0: 7a20 302e 342e 3220 616e 6420 7769 6c6c  z 0.4.2 and will
-00007ed0: 2063 6f6e 7469 6e75 6520 746f 2069 6d70   continue to imp
-00007ee0: 726f 7665 2074 6865 7365 2069 7373 7565  rove these issue
-00007ef0: 732e 5c6e 5c6e 5370 6163 7a7a 2c20 6c69  s.\n\nSpaczz, li
-00007f00: 6b65 2073 7061 4379 2c20 6861 7320 756e  ke spaCy, has un
-00007f10: 6465 6669 6e65 6420 6265 6861 7669 6f72  defined behavior
-00007f20: 2066 6f72 206d 756c 7469 706c 6520 6c61   for multiple la
-00007f30: 6265 6c73 2028 6f72 206c 6162 656c 2f65  bels (or label/e
-00007f40: 6e74 5f69 6420 636f 6d62 6f73 2920 7368  nt_id combos) sh
-00007f50: 6172 696e 6720 7468 6520 7361 6d65 2070  aring the same p
-00007f60: 6174 7465 726e 2e20 466f 7220 6578 616d  attern. For exam
-00007f70: 706c 652c 2069 6620 796f 7520 6164 6420  ple, if you add 
-00007f80: 7468 6520 7061 7474 6572 6e20 6022 4972  the pattern `"Ir
-00007f90: 656c 616e 6422 6020 6173 2062 6f74 6820  eland"` as both 
-00007fa0: 6022 4750 4522 6020 616e 6420 6022 4e41  `"GPE"` and `"NA
-00007fb0: 4d45 2260 2074 6865 2072 6573 756c 7469  ME"` the resulti
-00007fc0: 6e67 206c 6162 656c 2069 7320 756e 7072  ng label is unpr
-00007fd0: 6564 6963 7461 626c 652e 2046 6f72 2074  edictable. For t
-00007fe0: 6865 206d 6f73 7420 7061 7274 2074 6869  he most part thi
-00007ff0: 7320 6973 6e5c 2774 2061 6e20 6973 7375  s isn\'t an issu
-00008000: 6520 6275 7420 7370 6163 7a7a 2061 6c73  e but spaczz als
-00008010: 6f20 6861 7320 746f 2064 6561 6c20 7769  o has to deal wi
-00008020: 7468 2074 6865 2061 6464 6974 696f 6e61  th the additiona
-00008030: 6c20 7772 696e 6b6c 6520 6f66 2066 757a  l wrinkle of fuz
-00008040: 7a79 206d 6174 6368 6573 2e5c 6e5c 6e46  zy matches.\n\nF
-00008050: 6f72 2065 7861 6d70 6c65 2069 6620 7765  or example if we
-00008060: 2061 7265 206c 6f6f 6b69 6e67 2066 6f72   are looking for
-00008070: 2074 6865 2073 7472 696e 6720 6022 4972   the string `"Ir
-00008080: 656c 616e 6422 6020 616e 6420 6861 7665  eland"` and have
-00008090: 2074 6865 2070 6174 7465 726e 7320 605b   the patterns `[
-000080a0: 2249 7265 6c61 6e64 222c 2022 4963 656c  "Ireland", "Icel
-000080b0: 616e 6422 5d60 2e20 4576 656e 2077 6974  and"]`. Even wit
-000080c0: 6820 6120 7265 7175 6972 6564 206d 6174  h a required mat
-000080d0: 6368 2072 6174 696f 206f 6620 6038 3560  ch ratio of `85`
-000080e0: 2074 6865 7365 2077 696c 6c20 626f 7468   these will both
-000080f0: 206d 6174 6368 2061 7420 6031 3030 6020   match at `100` 
-00008100: 616e 6420 6038 3660 2072 6573 7065 6374  and `86` respect
-00008110: 6976 656c 792e 2057 6865 6e20 6a75 7374  ively. When just
-00008120: 2064 6561 6c69 6e67 2077 6974 6820 6675   dealing with fu
-00008130: 7a7a 7920 6d61 7463 6865 7320 7468 6973  zzy matches this
-00008140: 2069 736e 5c27 7420 616e 2069 7373 7565   isn\'t an issue
-00008150: 2061 7320 7765 2063 616e 2073 6f72 7420   as we can sort 
-00008160: 6279 2064 6573 6365 6e64 696e 6720 6d61  by descending ma
-00008170: 7463 6820 7261 7469 6f2e 2048 6f77 6576  tch ratio. Howev
-00008180: 6572 2077 6861 7420 6966 2074 6865 2060  er what if the `
-00008190: 2249 6365 6c61 6e64 2260 2070 6174 7465  "Iceland"` patte
-000081a0: 726e 2077 6173 2061 2072 6567 6578 2070  rn was a regex p
-000081b0: 6174 7465 726e 2061 6e64 2069 7420 7265  attern and it re
-000081c0: 7475 726e 6564 2061 2074 7570 6c65 206f  turned a tuple o
-000081d0: 6620 6675 7a7a 7920 7265 6765 7820 636f  f fuzzy regex co
-000081e0: 756e 7473 3f20 4f72 2077 6861 7420 6966  unts? Or what if
-000081f0: 2074 6865 2060 2249 6365 6c61 6e64 2260   the `"Iceland"`
-00008200: 2070 6174 7465 726e 2077 6173 2061 2074   pattern was a t
-00008210: 6f6b 656e 2070 6174 7465 726e 2061 6e64  oken pattern and
-00008220: 2074 6865 2060 546f 6b65 6e4d 6174 6368   the `TokenMatch
-00008230: 6572 6020 646f 6573 206e 6f74 2065 7665  er` does not eve
-00008240: 6e20 6375 7272 656e 746c 7920 7072 6f76  n currently prov
-00008250: 6964 6520 6d61 7463 6820 6465 7461 696c  ide match detail
-00008260: 733f 215c 6e5c 6e54 6865 2061 626f 7665  s?!\n\nThe above
-00008270: 2070 726f 626c 656d 2069 7320 7477 6f66   problem is twof
-00008280: 6f6c 642e 2046 6972 7374 2061 6e64 2066  old. First and f
-00008290: 6f72 656d 6f73 742c 2049 206e 6565 6420  oremost, I need 
-000082a0: 746f 2064 6576 656c 6f70 2061 2077 6179  to develop a way
-000082b0: 206f 7220 7761 7973 2074 6f20 636f 6d70   or ways to comp
-000082c0: 6172 6520 6170 706c 6573 2074 6f20 6f72  are apples to or
-000082d0: 616e 6765 7320 2d20 6675 7a7a 7920 7261  anges - fuzzy ra
-000082e0: 7469 6f73 2061 6e64 2066 757a 7a79 2072  tios and fuzzy r
-000082f0: 6567 6578 2063 6f75 6e74 732e 2054 6865  egex counts. The
-00008300: 6e20 4920 6e65 6564 2074 6f20 6669 6775  n I need to figu
-00008310: 7265 206f 7574 2068 6f77 2074 6f20 696e  re out how to in
-00008320: 636c 7564 6520 6d61 7463 6820 6465 7461  clude match deta
-00008330: 696c 7320 6672 6f6d 2074 6865 2060 546f  ils from the `To
-00008340: 6b65 6e4d 6174 6368 6572 6020 7768 6963  kenMatcher` whic
-00008350: 6820 7375 7070 6f72 7473 2062 6f74 6820  h supports both 
-00008360: 6675 7a7a 7920 616e 6420 2266 757a 7a79  fuzzy and "fuzzy
-00008370: 2220 7265 6765 7820 6d61 7463 6865 732e  " regex matches.
-00008380: 5c6e 5c6e 466f 7220 6120 7368 6f72 742d  \n\nFor a short-
-00008390: 7465 726d 2073 6f6c 7574 696f 6e20 4920  term solution I 
-000083a0: 616d 2068 6176 696e 6720 7468 6520 656e  am having the en
-000083b0: 7469 7479 2072 756c 6572 2066 6972 7374  tity ruler first
-000083c0: 2067 6f20 7468 726f 7567 6820 736f 7274   go through sort
-000083d0: 6564 2066 757a 7a79 206d 6174 6368 6573  ed fuzzy matches
-000083e0: 2c20 7468 656e 2073 6f72 7465 6420 7265  , then sorted re
-000083f0: 6765 7820 6d61 7463 6865 732c 2061 6e64  gex matches, and
-00008400: 206c 6173 746c 7920 746f 6b65 6e20 6d61   lastly token ma
-00008410: 7463 6865 732e 2054 6f6b 656e 206d 6174  tches. Token mat
-00008420: 6368 6573 2077 696c 6c20 6f6e 6c79 2062  ches will only b
-00008430: 6520 736f 7274 6564 2062 7920 6c65 6e67  e sorted by leng
-00008440: 7468 206f 6620 6d61 7463 682c 206e 6f74  th of match, not
-00008450: 2071 7561 6c69 7479 2c20 736f 2074 6865   quality, so the
-00008460: 7920 6d61 7920 7072 6f76 6964 6520 696e  y may provide in
-00008470: 636f 6e73 6973 7465 6e74 2072 6573 756c  consistent resul
-00008480: 7473 2e20 5472 7920 746f 2062 6520 6d69  ts. Try to be mi
-00008490: 6e64 6675 6c20 6f66 2079 6f75 7220 746f  ndful of your to
-000084a0: 6b65 6e20 7061 7474 6572 6e73 2e5c 6e5c  ken patterns.\n\
-000084b0: 6e54 6865 7265 2069 7320 6164 6469 7469  nThere is additi
-000084c0: 6f6e 616c 206c 6f67 6963 2069 6e20 706c  onal logic in pl
-000084d0: 6163 6520 746f 2066 696c 7465 7220 6f76  ace to filter ov
-000084e0: 6572 6c61 7070 696e 6720 6d61 7463 6865  erlapping matche
-000084f0: 7320 7072 6573 6572 7669 6e67 2065 6172  s preserving ear
-00008500: 6c69 6572 206d 6174 6368 6573 206f 7665  lier matches ove
-00008510: 7220 6c61 7465 7220 6f6e 6573 2e20 5468  r later ones. Th
-00008520: 6973 206f 7264 6572 206f 6620 7072 696f  is order of prio
-00008530: 7269 7479 2028 6675 7a7a 792c 2072 6567  rity (fuzzy, reg
-00008540: 6578 2c20 746f 6b65 6e29 206d 6179 206e  ex, token) may n
-00008550: 6f74 2062 6520 6964 6561 6c20 666f 7220  ot be ideal for 
-00008560: 6576 6572 796f 6e65 2062 7574 2061 6464  everyone but add
-00008570: 696e 6720 6120 7761 7920 746f 2063 6861  ing a way to cha
-00008580: 6e67 6520 7468 6520 6f72 6465 7220 2873  nge the order (s
-00008590: 6179 2072 6567 6578 2070 6174 7465 726e  ay regex pattern
-000085a0: 7320 6669 7273 7429 2077 6f75 6c64 2061  s first) would a
-000085b0: 2074 656d 706f 7261 7279 2073 6f6c 7574   temporary solut
-000085c0: 696f 6e20 746f 2061 2074 656d 706f 7261  ion to a tempora
-000085d0: 7279 2070 726f 626c 656d 2e5c 6e5c 6e50  ry problem.\n\nP
-000085e0: 6c65 6173 6520 6265 6172 2077 6974 6820  lease bear with 
-000085f0: 6d65 2074 6872 6f75 6768 2074 6865 7365  me through these
-00008600: 2067 726f 7769 6e67 2070 6169 6e73 2e5c   growing pains.\
-00008610: 6e5c 6e23 2320 526f 6164 6d61 705c 6e5c  n\n## Roadmap\n\
-00008620: 6e49 2061 6d20 616c 7761 7973 206f 7065  nI am always ope
-00008630: 6e20 616e 6420 7265 6365 7074 6976 6520  n and receptive 
-00008640: 746f 2066 6561 7475 7265 2072 6571 7565  to feature reque
-00008650: 7374 7320 6275 7420 6a75 7374 2062 6520  sts but just be 
-00008660: 6177 6172 652c 2061 7320 6120 736f 6c6f  aware, as a solo
-00008670: 2d64 6576 2077 6974 6820 6120 6c6f 7420  -dev with a lot 
-00008680: 6c65 6674 2074 6f20 6c65 6172 6e2c 2064  left to learn, d
-00008690: 6576 656c 6f70 6d65 6e74 2063 616e 206d  evelopment can m
-000086a0: 6f76 6520 7072 6574 7479 2073 6c6f 772e  ove pretty slow.
-000086b0: 2054 6865 2066 6f6c 6c6f 7769 6e67 2069   The following i
-000086c0: 7320 6d79 2072 6f61 646d 6170 2066 6f72  s my roadmap for
-000086d0: 2073 7061 637a 7a20 736f 2079 6f75 2063   spaczz so you c
-000086e0: 616e 2073 6565 2077 6865 7265 2069 7373  an see where iss
-000086f0: 7565 7320 7261 6973 6564 206d 6967 6874  ues raised might
-00008700: 2066 6974 2069 6e74 6f20 6d79 2063 7572   fit into my cur
-00008710: 7265 6e74 2070 7269 6f72 6974 6965 732e  rent priorities.
-00008720: 5c6e 5c6e 2a2a 4869 6768 2050 7269 6f72  \n\n**High Prior
-00008730: 6974 792a 2a5c 6e5c 6e31 2e20 4275 6720  ity**\n\n1. Bug 
-00008740: 6669 7865 7320 2d20 626f 7468 2062 7265  fixes - both bre
-00008750: 616b 696e 6720 616e 6420 6265 6861 7669  aking and behavi
-00008760: 6f72 616c 2e20 486f 7065 6675 6c6c 7920  oral. Hopefully 
-00008770: 7468 6573 6520 7769 6c6c 2062 6520 6d69  these will be mi
-00008780: 6e69 6d61 6c2e 5c6e 312e 2045 6173 6520  nimal.\n1. Ease 
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7370 6163  : 2.1.Name: spac
+00000020: 7a7a 0a56 6572 7369 6f6e 3a20 302e 362e  zz.Version: 0.6.
+00000030: 3061 300a 5375 6d6d 6172 793a 2041 6464  0a0.Summary: Add
+00000040: 7320 6675 7a7a 7920 6d61 7463 6869 6e67  s fuzzy matching
+00000050: 2061 6e64 2061 6464 6974 696f 6e61 6c20   and additional 
+00000060: 7265 6765 7820 6d61 7463 6869 6e67 2073  regex matching s
+00000070: 7570 706f 7274 2074 6f20 7370 6143 792e  upport to spaCy.
+00000080: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
+00000090: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+000000a0: 616e 6465 7273 656e 3130 312f 7370 6163  andersen101/spac
+000000b0: 7a7a 0a4c 6963 656e 7365 3a20 4d49 540a  zz.License: MIT.
+000000c0: 4b65 7977 6f72 6473 3a20 6675 7a7a 7920  Keywords: fuzzy 
+000000d0: 6d61 7463 6869 6e67 2c73 7061 6379 2c6e  matching,spacy,n
+000000e0: 6c70 0a41 7574 686f 723a 2047 7261 6e74  lp.Author: Grant
+000000f0: 2041 6e64 6572 7365 6e0a 4175 7468 6f72   Andersen.Author
+00000100: 2d65 6d61 696c 3a20 6761 6e64 6572 7365  -email: ganderse
+00000110: 6e2e 636f 6465 7340 676d 6169 6c2e 636f  n.codes@gmail.co
+00000120: 6d0a 5265 7175 6972 6573 2d50 7974 686f  m.Requires-Pytho
+00000130: 6e3a 203e 3d33 2e37 2c3c 342e 300a 436c  n: >=3.7,<4.0.Cl
+00000140: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000150: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000160: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000170: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000180: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000190: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001d0: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
+000001e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000200: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000210: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000240: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000250: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000260: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+00000270: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000290: 7468 6f6e 203a 3a20 332e 3131 0a52 6571  thon :: 3.11.Req
+000002a0: 7569 7265 732d 4469 7374 3a20 6361 7461  uires-Dist: cata
+000002b0: 6c6f 6775 650a 5265 7175 6972 6573 2d44  logue.Requires-D
+000002c0: 6973 743a 2069 6d70 6f72 746c 6962 5f6d  ist: importlib_m
+000002d0: 6574 6164 6174 6120 3b20 7079 7468 6f6e  etadata ; python
+000002e0: 5f76 6572 7369 6f6e 203c 2022 332e 3822  _version < "3.8"
+000002f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000300: 6e75 6d70 7920 283e 3d31 2e31 352c 3c31  numpy (>=1.15,<1
+00000310: 2e32 3229 203b 2070 7974 686f 6e5f 7665  .22) ; python_ve
+00000320: 7273 696f 6e20 3e3d 2022 332e 3722 2061  rsion >= "3.7" a
+00000330: 6e64 2070 7974 686f 6e5f 7665 7273 696f  nd python_versio
+00000340: 6e20 3c20 2233 2e38 220a 5265 7175 6972  n < "3.8".Requir
+00000350: 6573 2d44 6973 743a 206e 756d 7079 2028  es-Dist: numpy (
+00000360: 3e3d 312e 3137 2e33 2920 3b20 7079 7468  >=1.17.3) ; pyth
+00000370: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2233  on_version >= "3
+00000380: 2e38 2220 616e 6420 7079 7468 6f6e 5f76  .8" and python_v
+00000390: 6572 7369 6f6e 203c 2022 332e 3922 0a52  ersion < "3.9".R
+000003a0: 6571 7569 7265 732d 4469 7374 3a20 6e75  equires-Dist: nu
+000003b0: 6d70 7920 283e 3d31 2e31 392e 3329 203b  mpy (>=1.19.3) ;
+000003c0: 2070 7974 686f 6e5f 7665 7273 696f 6e20   python_version 
+000003d0: 3e3d 2022 332e 3922 2061 6e64 2070 7974  >= "3.9" and pyt
+000003e0: 686f 6e5f 7665 7273 696f 6e20 3c20 2233  hon_version < "3
+000003f0: 2e31 3022 0a52 6571 7569 7265 732d 4469  .10".Requires-Di
+00000400: 7374 3a20 6e75 6d70 7920 283e 3d31 2e32  st: numpy (>=1.2
+00000410: 312e 3229 203b 2070 7974 686f 6e5f 7665  1.2) ; python_ve
+00000420: 7273 696f 6e20 3e3d 2022 332e 3130 2220  rsion >= "3.10" 
+00000430: 616e 6420 7079 7468 6f6e 5f76 6572 7369  and python_versi
+00000440: 6f6e 203c 2022 342e 3022 0a52 6571 7569  on < "4.0".Requi
+00000450: 7265 732d 4469 7374 3a20 7261 7069 6466  res-Dist: rapidf
+00000460: 757a 7a20 283e 3d31 2e30 2e30 290a 5265  uzz (>=1.0.0).Re
+00000470: 7175 6972 6573 2d44 6973 743a 2072 6567  quires-Dist: reg
+00000480: 6578 2028 3e3d 3230 3230 2e36 2e38 290a  ex (>=2020.6.8).
+00000490: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+000004a0: 7061 6379 2028 3e3d 332e 302c 3c34 2e30  pacy (>=3.0,<4.0
+000004b0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+000004c0: 2073 7273 6c79 0a52 6571 7569 7265 732d   srsly.Requires-
+000004d0: 4469 7374 3a20 7479 7069 6e67 5f65 7874  Dist: typing_ext
+000004e0: 656e 7369 6f6e 7320 3b20 7079 7468 6f6e  ensions ; python
+000004f0: 5f76 6572 7369 6f6e 203c 2022 332e 3822  _version < "3.8"
+00000500: 0a50 726f 6a65 6374 2d55 524c 3a20 446f  .Project-URL: Do
+00000510: 6375 6d65 6e74 6174 696f 6e2c 2068 7474  cumentation, htt
+00000520: 7073 3a2f 2f73 7061 637a 7a2e 7265 6164  ps://spaczz.read
+00000530: 7468 6564 6f63 732e 696f 0a50 726f 6a65  thedocs.io.Proje
+00000540: 6374 2d55 524c 3a20 5265 706f 7369 746f  ct-URL: Reposito
+00000550: 7279 2c20 6874 7470 733a 2f2f 6769 7468  ry, https://gith
+00000560: 7562 2e63 6f6d 2f67 616e 6465 7273 656e  ub.com/gandersen
+00000570: 3130 312f 7370 6163 7a7a 0a44 6573 6372  101/spaczz.Descr
+00000580: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+00000590: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+000005a0: 776e 0a0a 5b21 5b54 6573 7473 5d28 6874  wn..[![Tests](ht
+000005b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000005c0: 2f67 616e 6465 7273 656e 3130 312f 7370  /gandersen101/sp
+000005d0: 6163 7a7a 2f77 6f72 6b66 6c6f 7773 2f4c  aczz/workflows/L
+000005e0: 696e 742c 2532 3054 7970 6563 6865 636b  int,%20Typecheck
+000005f0: 2532 3061 6e64 2532 3054 6573 742f 6261  %20and%20Test/ba
+00000600: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
+00000610: 2f2f 6769 7468 7562 2e63 6f6d 2f67 616e  //github.com/gan
+00000620: 6465 7273 656e 3130 312f 7370 6163 7a7a  dersen101/spaczz
+00000630: 2f61 6374 696f 6e73 3f77 6f72 6b66 6c6f  /actions?workflo
+00000640: 773d 4c69 6e74 2c25 3230 5479 7065 6368  w=Lint,%20Typech
+00000650: 6563 6b25 3230 616e 6425 3230 5465 7374  eck%20and%20Test
+00000660: 290a 5b21 5b43 6f64 6563 6f76 5d28 6874  ).[![Codecov](ht
+00000670: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000680: 2f67 682f 6761 6e64 6572 7365 6e31 3031  /gh/gandersen101
+00000690: 2f73 7061 637a 7a2f 6272 616e 6368 2f6d  /spaczz/branch/m
+000006a0: 6173 7465 722f 6772 6170 682f 6261 6467  aster/graph/badg
+000006b0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000006c0: 636f 6465 636f 762e 696f 2f67 682f 6761  codecov.io/gh/ga
+000006d0: 6e64 6572 7365 6e31 3031 2f73 7061 637a  ndersen101/spacz
+000006e0: 7a29 0a5b 215b 5079 5049 5d28 6874 7470  z).[![PyPI](http
+000006f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000700: 696f 2f70 7970 692f 762f 7370 6163 7a7a  io/pypi/v/spaczz
+00000710: 2e73 7667 295d 2868 7474 7073 3a2f 2f70  .svg)](https://p
+00000720: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+00000730: 7370 6163 7a7a 2f29 0a5b 215b 5265 6164  spaczz/).[![Read
+00000740: 2074 6865 2044 6f63 735d 2868 7474 7073   the Docs](https
+00000750: 3a2f 2f72 6561 6474 6865 646f 6373 2e6f  ://readthedocs.o
+00000760: 7267 2f70 726f 6a65 6374 732f 7370 6163  rg/projects/spac
+00000770: 7a7a 2f62 6164 6765 2f29 5d28 6874 7470  zz/badge/)](http
+00000780: 733a 2f2f 7370 6163 7a7a 2e72 6561 6474  s://spaczz.readt
+00000790: 6865 646f 6373 2e69 6f2f 290a 0a23 2073  hedocs.io/)..# s
+000007a0: 7061 637a 7a3a 2046 757a 7a79 206d 6174  paczz: Fuzzy mat
+000007b0: 6368 696e 6720 616e 6420 6d6f 7265 2066  ching and more f
+000007c0: 6f72 2073 7061 4379 0a0a 7370 6163 7a7a  or spaCy..spaczz
+000007d0: 2070 726f 7669 6465 7320 6675 7a7a 7920   provides fuzzy 
+000007e0: 6d61 7463 6869 6e67 2061 6e64 2061 6464  matching and add
+000007f0: 6974 696f 6e61 6c20 7265 6765 7820 6d61  itional regex ma
+00000800: 7463 6869 6e67 2066 756e 6374 696f 6e61  tching functiona
+00000810: 6c69 7479 2066 6f72 205b 7370 6143 795d  lity for [spaCy]
+00000820: 2868 7474 7073 3a2f 2f73 7061 6379 2e69  (https://spacy.i
+00000830: 6f2f 292e 0a73 7061 637a 7a27 7320 636f  o/)..spaczz's co
+00000840: 6d70 6f6e 656e 7473 2068 6176 6520 7369  mponents have si
+00000850: 6d69 6c61 7220 4150 4973 2074 6f20 7468  milar APIs to th
+00000860: 6569 7220 7370 6143 7920 636f 756e 7465  eir spaCy counte
+00000870: 7270 6172 7473 2061 6e64 2073 7061 637a  rparts and spacz
+00000880: 7a20 7069 7065 6c69 6e65 2063 6f6d 706f  z pipeline compo
+00000890: 6e65 6e74 7320 6361 6e20 696e 7465 6772  nents can integr
+000008a0: 6174 6520 696e 746f 2073 7061 4379 2070  ate into spaCy p
+000008b0: 6970 656c 696e 6573 2077 6865 7265 2074  ipelines where t
+000008c0: 6865 7920 6361 6e20 6265 2073 6176 6564  hey can be saved
+000008d0: 2f6c 6f61 6465 6420 6173 206d 6f64 656c  /loaded as model
+000008e0: 732e 0a0a 4675 7a7a 7920 6d61 7463 6869  s...Fuzzy matchi
+000008f0: 6e67 2069 7320 6375 7272 656e 746c 7920  ng is currently 
+00000900: 7065 7266 6f72 6d65 6420 7769 7468 206d  performed with m
+00000910: 6174 6368 6572 7320 6672 6f6d 205b 5261  atchers from [Ra
+00000920: 7069 6446 757a 7a5d 2868 7474 7073 3a2f  pidFuzz](https:/
+00000930: 2f67 6974 6875 622e 636f 6d2f 6d61 7862  /github.com/maxb
+00000940: 6163 686d 616e 6e2f 7261 7069 6466 757a  achmann/rapidfuz
+00000950: 7a29 2773 2066 757a 7a20 6d6f 6475 6c65  z)'s fuzz module
+00000960: 2061 6e64 2072 6567 6578 206d 6174 6368   and regex match
+00000970: 696e 6720 6375 7272 656e 746c 7920 7265  ing currently re
+00000980: 6c69 6573 206f 6e20 7468 6520 5b72 6567  lies on the [reg
+00000990: 6578 5d28 6874 7470 733a 2f2f 7079 7069  ex](https://pypi
+000009a0: 2e6f 7267 2f70 726f 6a65 6374 2f72 6567  .org/project/reg
+000009b0: 6578 2f29 206c 6962 7261 7279 2e20 7370  ex/) library. sp
+000009c0: 6163 7a7a 2063 6572 7461 696e 6c79 2074  aczz certainly t
+000009d0: 616b 6573 2061 6464 6974 696f 6e61 6c20  akes additional 
+000009e0: 696e 666c 7565 6e63 6520 6672 6f6d 206f  influence from o
+000009f0: 7468 6572 206c 6962 7261 7269 6573 2061  ther libraries a
+00000a00: 6e64 2072 6573 6f75 7263 6573 2e20 466f  nd resources. Fo
+00000a10: 7220 6164 6469 7469 6f6e 616c 2064 6574  r additional det
+00000a20: 6169 6c73 2073 6565 2074 6865 2072 6566  ails see the ref
+00000a30: 6572 656e 6365 7320 7365 6374 696f 6e2e  erences section.
+00000a40: 0a0a 2a2a 5375 7070 6f72 7473 2073 7061  ..**Supports spa
+00000a50: 4379 203e 3d20 332e 302a 2a0a 0a73 7061  Cy >= 3.0**..spa
+00000a60: 637a 7a20 6861 7320 6265 656e 2074 6573  czz has been tes
+00000a70: 7465 6420 6f6e 2055 6275 6e74 752c 204d  ted on Ubuntu, M
+00000a80: 6163 4f53 2c20 616e 6420 5769 6e64 6f77  acOS, and Window
+00000a90: 7320 5365 7276 6572 2e0a 0a2a 7630 2e36  s Server...*v0.6
+00000aa0: 2e30 2052 656c 6561 7365 204e 6f74 6573  .0 Release Notes
+00000ab0: 3a2a 0a2d 202a 5265 7475 726e 696e 6720  :*.- *Returning 
+00000ac0: 7468 6520 6d61 7463 6869 6e67 2070 6174  the matching pat
+00000ad0: 7465 726e 2066 6f72 2061 6c6c 206d 6174  tern for all mat
+00000ae0: 6368 6572 732c 2074 6869 7320 6973 2061  chers, this is a
+00000af0: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
+00000b00: 2061 7320 6d61 7463 6865 7320 6172 6520   as matches are 
+00000b10: 6e6f 7720 7475 706c 6573 206f 6620 6c65  now tuples of le
+00000b20: 6e67 7468 2035 2069 6e73 7465 6164 206f  ngth 5 instead o
+00000b30: 6620 342e 2a0a 2d20 2a52 6567 6578 2061  f 4.*.- *Regex a
+00000b40: 6e64 2074 6f6b 656e 206d 6174 6368 6573  nd token matches
+00000b50: 206e 6f77 2072 6574 7572 6e20 6d61 7463   now return matc
+00000b60: 6820 7261 7469 6f73 2e2a 0a2d 202a 5375  h ratios.*.- *Su
+00000b70: 7070 6f72 7420 666f 7220 6070 7974 686f  pport for `pytho
+00000b80: 6e3c 3d33 2e31 312c 3e3d 332e 3760 2c20  n<=3.11,>=3.7`, 
+00000b90: 616c 6f6e 6720 7769 7468 2060 7261 7069  along with `rapi
+00000ba0: 6466 757a 7a3e 3d31 2e30 2e30 602e 0a2d  dfuzz>=1.0.0`..-
+00000bb0: 202a 4472 6f70 7065 6420 7375 7070 6f72   *Dropped suppor
+00000bc0: 7420 666f 7220 7370 6143 7920 7632 2e20  t for spaCy v2. 
+00000bd0: 536f 7272 7920 746f 2064 6f20 7468 6973  Sorry to do this
+00000be0: 2077 6974 686f 7574 2061 2064 6570 7265   without a depre
+00000bf0: 6361 7469 6f6e 2063 7963 6c65 2c20 6275  cation cycle, bu
+00000c00: 7420 4920 7374 6570 7065 6420 6177 6179  t I stepped away
+00000c10: 2066 726f 6d20 7468 6973 2070 726f 6a65   from this proje
+00000c20: 6374 2066 6f72 2061 206c 6f6e 6720 7469  ct for a long ti
+00000c30: 6d65 2e2a 0a2d 202a 5265 6d6f 7665 6420  me.*.- *Removed 
+00000c40: 7375 7070 6f72 7420 6f66 2060 2273 7061  support of `"spa
+00000c50: 637a 7a5f 2260 2070 7265 7072 656e 6465  czz_"` preprende
+00000c60: 6420 6f70 7469 6f6e 616c 2060 5370 6163  d optional `Spac
+00000c70: 7a7a 5275 6c65 7260 2069 6e69 7420 6172  zzRuler` init ar
+00000c80: 6775 6d65 6e74 732e 2041 6c73 6f2c 2073  guments. Also, s
+00000c90: 6f72 7279 2074 6f20 646f 2074 6869 7320  orry to do this 
+00000ca0: 7769 7468 6f75 7420 6120 6465 7072 6563  without a deprec
+00000cb0: 6174 696f 6e20 6379 636c 652e 2a0a 2d20  ation cycle.*.- 
+00000cc0: 2a60 4d61 7463 6865 722e 7069 7065 6020  *`Matcher.pipe` 
+00000cd0: 6d65 7468 6f64 732c 2077 6869 6368 2077  methods, which w
+00000ce0: 6572 6520 6465 7072 6563 6174 6564 2c20  ere deprecated, 
+00000cf0: 6172 6520 6e6f 7720 7265 6d6f 7665 642e  are now removed.
+00000d00: 0a2d 202a 6073 7061 637a 7a5f 7370 616e  .- *`spaczz_span
+00000d10: 6020 6375 7374 6f6d 2061 7474 7269 6275  ` custom attribu
+00000d20: 7465 2c20 7768 6963 6820 7761 7320 6465  te, which was de
+00000d30: 7072 6563 6174 6564 2c20 6973 206e 6f77  precated, is now
+00000d40: 2072 656d 6f76 6564 2e0a 0a50 6c65 6173   removed...Pleas
+00000d50: 6520 7365 6520 7468 6520 5b63 6861 6e67  e see the [chang
+00000d60: 656c 6f67 5d28 6874 7470 733a 2f2f 6769  elog](https://gi
+00000d70: 7468 7562 2e63 6f6d 2f67 616e 6465 7273  thub.com/ganders
+00000d80: 656e 3130 312f 7370 6163 7a7a 2f62 6c6f  en101/spaczz/blo
+00000d90: 622f 6d61 7374 6572 2f43 4841 4e47 454c  b/master/CHANGEL
+00000da0: 4f47 2e6d 6429 2066 6f72 2070 7265 7669  OG.md) for previ
+00000db0: 6f75 7320 7265 6c65 6173 6520 6e6f 7465  ous release note
+00000dc0: 732e 2054 6869 7320 7769 6c6c 2065 7665  s. This will eve
+00000dd0: 6e74 7561 6c6c 7920 6265 206d 6f76 6564  ntually be moved
+00000de0: 2074 6f20 7468 6520 5b52 6561 6420 7468   to the [Read th
+00000df0: 6520 446f 6373 5d28 6874 7470 733a 2f2f  e Docs](https://
+00000e00: 7370 6163 7a7a 2e72 6561 6474 6865 646f  spaczz.readthedo
+00000e10: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000e20: 2920 7061 6765 2e0a 0a3c 6831 3e54 6162  ) page...<h1>Tab
+00000e30: 6c65 206f 6620 436f 6e74 656e 7473 3c73  le of Contents<s
+00000e40: 7061 6e20 636c 6173 733d 2274 6f63 536b  pan class="tocSk
+00000e50: 6970 223e 3c2f 7370 616e 3e3c 2f68 313e  ip"></span></h1>
+00000e60: 0a3c 6469 7620 636c 6173 733d 2274 6f63  .<div class="toc
+00000e70: 223e 3c75 6c20 636c 6173 733d 2274 6f63  "><ul class="toc
+00000e80: 2d69 7465 6d22 3e3c 6c69 3e3c 7370 616e  -item"><li><span
+00000e90: 3e3c 6120 6872 6566 3d22 2349 6e73 7461  ><a href="#Insta
+00000ea0: 6c6c 6174 696f 6e22 2064 6174 612d 746f  llation" data-to
+00000eb0: 632d 6d6f 6469 6669 6564 2d69 643d 2249  c-modified-id="I
+00000ec0: 6e73 7461 6c6c 6174 696f 6e2d 3122 3e49  nstallation-1">I
+00000ed0: 6e73 7461 6c6c 6174 696f 6e3c 2f61 3e3c  nstallation</a><
+00000ee0: 2f73 7061 6e3e 3c2f 6c69 3e3c 6c69 3e3c  /span></li><li><
+00000ef0: 7370 616e 3e3c 6120 6872 6566 3d22 2342  span><a href="#B
+00000f00: 6173 6963 2d55 7361 6765 2220 6461 7461  asic-Usage" data
+00000f10: 2d74 6f63 2d6d 6f64 6966 6965 642d 6964  -toc-modified-id
+00000f20: 3d22 4261 7369 632d 5573 6167 652d 3222  ="Basic-Usage-2"
+00000f30: 3e42 6173 6963 2055 7361 6765 3c2f 613e  >Basic Usage</a>
+00000f40: 3c2f 7370 616e 3e3c 756c 2063 6c61 7373  </span><ul class
+00000f50: 3d22 746f 632d 6974 656d 223e 3c6c 693e  ="toc-item"><li>
+00000f60: 3c73 7061 6e3e 3c61 2068 7265 663d 2223  <span><a href="#
+00000f70: 4675 7a7a 794d 6174 6368 6572 2220 6461  FuzzyMatcher" da
+00000f80: 7461 2d74 6f63 2d6d 6f64 6966 6965 642d  ta-toc-modified-
+00000f90: 6964 3d22 4675 7a7a 794d 6174 6368 6572  id="FuzzyMatcher
+00000fa0: 2d32 2e31 223e 4675 7a7a 794d 6174 6368  -2.1">FuzzyMatch
+00000fb0: 6572 3c2f 613e 3c2f 7370 616e 3e3c 2f6c  er</a></span></l
+00000fc0: 693e 3c6c 693e 3c73 7061 6e3e 3c61 2068  i><li><span><a h
+00000fd0: 7265 663d 2223 5265 6765 784d 6174 6368  ref="#RegexMatch
+00000fe0: 6572 2220 6461 7461 2d74 6f63 2d6d 6f64  er" data-toc-mod
+00000ff0: 6966 6965 642d 6964 3d22 5265 6765 784d  ified-id="RegexM
+00001000: 6174 6368 6572 2d32 2e32 223e 5265 6765  atcher-2.2">Rege
+00001010: 784d 6174 6368 6572 3c2f 613e 3c2f 7370  xMatcher</a></sp
+00001020: 616e 3e3c 2f6c 693e 3c6c 693e 3c73 7061  an></li><li><spa
+00001030: 6e3e 3c61 2068 7265 663d 2223 5369 6d69  n><a href="#Simi
+00001040: 6c61 7269 7479 4d61 7463 6865 7222 2064  larityMatcher" d
+00001050: 6174 612d 746f 632d 6d6f 6469 6669 6564  ata-toc-modified
+00001060: 2d69 643d 2253 696d 696c 6172 6974 794d  -id="SimilarityM
+00001070: 6174 6368 6572 2d32 2e33 223e 5369 6d69  atcher-2.3">Simi
+00001080: 6c61 7269 7479 4d61 7463 6865 723c 2f61  larityMatcher</a
+00001090: 3e3c 2f73 7061 6e3e 3c2f 6c69 3e3c 6c69  ></span></li><li
+000010a0: 3e3c 7370 616e 3e3c 6120 6872 6566 3d22  ><span><a href="
+000010b0: 2354 6f6b 656e 4d61 7463 6865 7222 2064  #TokenMatcher" d
+000010c0: 6174 612d 746f 632d 6d6f 6469 6669 6564  ata-toc-modified
+000010d0: 2d69 643d 2254 6f6b 656e 4d61 7463 6865  -id="TokenMatche
+000010e0: 722d 322e 3422 3e54 6f6b 656e 4d61 7463  r-2.4">TokenMatc
+000010f0: 6865 723c 2f61 3e3c 2f73 7061 6e3e 3c2f  her</a></span></
+00001100: 6c69 3e3c 6c69 3e3c 7370 616e 3e3c 6120  li><li><span><a 
+00001110: 6872 6566 3d22 2353 7061 637a 7a52 756c  href="#SpaczzRul
+00001120: 6572 2220 6461 7461 2d74 6f63 2d6d 6f64  er" data-toc-mod
+00001130: 6966 6965 642d 6964 3d22 5370 6163 7a7a  ified-id="Spaczz
+00001140: 5275 6c65 722d 322e 3522 3e53 7061 637a  Ruler-2.5">Spacz
+00001150: 7a52 756c 6572 3c2f 613e 3c2f 7370 616e  zRuler</a></span
+00001160: 3e3c 2f6c 693e 3c6c 693e 3c73 7061 6e3e  ></li><li><span>
+00001170: 3c61 2068 7265 663d 2223 4375 7374 6f6d  <a href="#Custom
+00001180: 2d41 7474 7269 6275 7465 7322 2064 6174  -Attributes" dat
+00001190: 612d 746f 632d 6d6f 6469 6669 6564 2d69  a-toc-modified-i
+000011a0: 643d 2243 7573 746f 6d2d 4174 7472 6962  d="Custom-Attrib
+000011b0: 7574 6573 2d32 2e36 223e 4375 7374 6f6d  utes-2.6">Custom
+000011c0: 2041 7474 7269 6275 7465 733c 2f61 3e3c   Attributes</a><
+000011d0: 2f73 7061 6e3e 3c2f 6c69 3e3c 6c69 3e3c  /span></li><li><
+000011e0: 7370 616e 3e3c 6120 6872 6566 3d22 2353  span><a href="#S
+000011f0: 6176 696e 672f 4c6f 6164 696e 6722 2064  aving/Loading" d
+00001200: 6174 612d 746f 632d 6d6f 6469 6669 6564  ata-toc-modified
+00001210: 2d69 643d 2253 6176 696e 672f 4c6f 6164  -id="Saving/Load
+00001220: 696e 672d 322e 3722 3e53 6176 696e 672f  ing-2.7">Saving/
+00001230: 4c6f 6164 696e 673c 2f61 3e3c 2f73 7061  Loading</a></spa
+00001240: 6e3e 3c2f 6c69 3e3c 2f75 6c3e 3c2f 6c69  n></li></ul></li
+00001250: 3e3c 6c69 3e3c 7370 616e 3e3c 6120 6872  ><li><span><a hr
+00001260: 6566 3d22 234b 6e6f 776e 2d49 7373 7565  ef="#Known-Issue
+00001270: 7322 2064 6174 612d 746f 632d 6d6f 6469  s" data-toc-modi
+00001280: 6669 6564 2d69 643d 224b 6e6f 776e 2d49  fied-id="Known-I
+00001290: 7373 7565 732d 3322 3e4b 6e6f 776e 2049  ssues-3">Known I
+000012a0: 7373 7565 733c 2f61 3e3c 2f73 7061 6e3e  ssues</a></span>
+000012b0: 3c75 6c20 636c 6173 733d 2274 6f63 2d69  <ul class="toc-i
+000012c0: 7465 6d22 3e3c 6c69 3e3c 7370 616e 3e3c  tem"><li><span><
+000012d0: 6120 6872 6566 3d22 2350 6572 666f 726d  a href="#Perform
+000012e0: 616e 6365 2220 6461 7461 2d74 6f63 2d6d  ance" data-toc-m
+000012f0: 6f64 6966 6965 642d 6964 3d22 5065 7266  odified-id="Perf
+00001300: 6f72 6d61 6e63 652d 332e 3122 3e50 6572  ormance-3.1">Per
+00001310: 666f 726d 616e 6365 3c2f 613e 3c2f 7370  formance</a></sp
+00001320: 616e 3e3c 2f6c 693e 3c2f 756c 3e3c 2f6c  an></li></ul></l
+00001330: 693e 3c6c 693e 3c73 7061 6e3e 3c61 2068  i><li><span><a h
+00001340: 7265 663d 2223 526f 6164 6d61 7022 2064  ref="#Roadmap" d
+00001350: 6174 612d 746f 632d 6d6f 6469 6669 6564  ata-toc-modified
+00001360: 2d69 643d 2252 6f61 646d 6170 2d34 223e  -id="Roadmap-4">
+00001370: 526f 6164 6d61 703c 2f61 3e3c 2f73 7061  Roadmap</a></spa
+00001380: 6e3e 3c2f 6c69 3e3c 6c69 3e3c 7370 616e  n></li><li><span
+00001390: 3e3c 6120 6872 6566 3d22 2344 6576 656c  ><a href="#Devel
+000013a0: 6f70 6d65 6e74 2220 6461 7461 2d74 6f63  opment" data-toc
+000013b0: 2d6d 6f64 6966 6965 642d 6964 3d22 4465  -modified-id="De
+000013c0: 7665 6c6f 706d 656e 742d 3522 3e44 6576  velopment-5">Dev
+000013d0: 656c 6f70 6d65 6e74 3c2f 613e 3c2f 7370  elopment</a></sp
+000013e0: 616e 3e3c 2f6c 693e 3c6c 693e 3c73 7061  an></li><li><spa
+000013f0: 6e3e 3c61 2068 7265 663d 2223 5265 6665  n><a href="#Refe
+00001400: 7265 6e63 6573 2220 6461 7461 2d74 6f63  rences" data-toc
+00001410: 2d6d 6f64 6966 6965 642d 6964 3d22 5265  -modified-id="Re
+00001420: 6665 7265 6e63 6573 2d36 223e 5265 6665  ferences-6">Refe
+00001430: 7265 6e63 6573 3c2f 613e 3c2f 7370 616e  rences</a></span
+00001440: 3e3c 2f6c 693e 3c2f 756c 3e3c 2f64 6976  ></li></ul></div
+00001450: 3e0a 0a23 2320 496e 7374 616c 6c61 7469  >..## Installati
+00001460: 6f6e 0a0a 5370 6163 7a7a 2063 616e 2062  on..Spaczz can b
+00001470: 6520 696e 7374 616c 6c65 6420 7573 696e  e installed usin
+00001480: 6720 7069 702e 0a0a 6060 6070 7974 686f  g pip...```pytho
+00001490: 6e0a 7069 7020 696e 7374 616c 6c20 7370  n.pip install sp
+000014a0: 6163 7a7a 0a60 6060 0a0a 2323 2042 6173  aczz.```..## Bas
+000014b0: 6963 2055 7361 6765 0a0a 5370 6163 7a7a  ic Usage..Spaczz
+000014c0: 2773 2070 7269 6d61 7279 2066 6561 7475  's primary featu
+000014d0: 7265 7320 6172 6520 7468 6520 6046 757a  res are the `Fuz
+000014e0: 7a79 4d61 7463 6865 7260 2c20 6052 6567  zyMatcher`, `Reg
+000014f0: 6578 4d61 7463 6865 7260 2c20 616e 6420  exMatcher`, and 
+00001500: 2266 757a 7a79 2220 6054 6f6b 656e 4d61  "fuzzy" `TokenMa
+00001510: 7463 6865 7260 2074 6861 7420 6675 6e63  tcher` that func
+00001520: 7469 6f6e 2073 696d 696c 6172 6c79 2074  tion similarly t
+00001530: 6f20 7370 6143 7927 7320 604d 6174 6368  o spaCy's `Match
+00001540: 6572 6020 616e 6420 6050 6872 6173 654d  er` and `PhraseM
+00001550: 6174 6368 6572 602c 2061 6e64 2074 6865  atcher`, and the
+00001560: 2060 5370 6163 7a7a 5275 6c65 7260 2077   `SpaczzRuler` w
+00001570: 6869 6368 2069 6e74 6567 7261 7465 7320  hich integrates 
+00001580: 7468 6520 7370 6163 7a7a 206d 6174 6368  the spaczz match
+00001590: 6572 7320 696e 746f 2061 2073 7061 4379  ers into a spaCy
+000015a0: 2070 6970 656c 696e 6520 636f 6d70 6f6e   pipeline compon
+000015b0: 656e 7420 7369 6d69 6c61 7220 746f 2073  ent similar to s
+000015c0: 7061 4379 2773 2060 456e 7469 7479 5275  paCy's `EntityRu
+000015d0: 6c65 7260 2e0a 0a23 2323 2046 757a 7a79  ler`...### Fuzzy
+000015e0: 4d61 7463 6865 720a 0a54 6865 2062 6173  Matcher..The bas
+000015f0: 6963 2075 7361 6765 206f 6620 7468 6520  ic usage of the 
+00001600: 6675 7a7a 7920 6d61 7463 6865 7220 6973  fuzzy matcher is
+00001610: 2073 696d 696c 6172 2074 6f20 7370 6143   similar to spaC
+00001620: 7927 7320 6050 6872 6173 654d 6174 6368  y's `PhraseMatch
+00001630: 6572 6020 6578 6365 7074 2069 7420 7265  er` except it re
+00001640: 7475 726e 7320 7468 6520 6675 7a7a 7920  turns the fuzzy 
+00001650: 7261 7469 6f20 616e 6420 6d61 7463 6865  ratio and matche
+00001660: 6420 7061 7474 6572 6e2c 2061 6c6f 6e67  d pattern, along
+00001670: 2077 6974 6820 6d61 7463 6820 6964 2c20   with match id, 
+00001680: 7374 6172 7420 616e 6420 656e 6420 696e  start and end in
+00001690: 666f 726d 6174 696f 6e2c 2073 6f20 6d61  formation, so ma
+000016a0: 6b65 2073 7572 6520 746f 2069 6e63 6c75  ke sure to inclu
+000016b0: 6465 2076 6172 6961 626c 6573 2066 6f72  de variables for
+000016c0: 2074 6865 2072 6174 696f 2061 6e64 2070   the ratio and p
+000016d0: 6174 7465 726e 2077 6865 6e20 756e 7061  attern when unpa
+000016e0: 636b 696e 6720 7265 7375 6c74 732e 0a0a  cking results...
+000016f0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00001700: 7420 7370 6163 790a 6672 6f6d 2073 7061  t spacy.from spa
+00001710: 637a 7a2e 6d61 7463 6865 7220 696d 706f  czz.matcher impo
+00001720: 7274 2046 757a 7a79 4d61 7463 6865 720a  rt FuzzyMatcher.
+00001730: 0a6e 6c70 203d 2073 7061 6379 2e62 6c61  .nlp = spacy.bla
+00001740: 6e6b 2822 656e 2229 0a74 6578 7420 3d20  nk("en").text = 
+00001750: 2222 2247 7269 6e74 204d 2041 6e64 6572  """Grint M Ander
+00001760: 736f 6e20 6372 6561 7465 6420 7370 6163  son created spac
+00001770: 7a7a 2069 6e20 6869 7320 686f 6d65 2061  zz in his home a
+00001780: 7420 3535 3520 4661 6b65 2053 742c 0a41  t 555 Fake St,.A
+00001790: 7074 2035 2069 6e20 4e61 7368 7631 6c65  pt 5 in Nashv1le
+000017a0: 2c20 544e 2035 3535 3535 2d31 3233 3420  , TN 55555-1234 
+000017b0: 696e 2074 6865 2055 532e 2222 2220 2023  in the US."""  #
+000017c0: 2053 7065 6c6c 696e 6720 6572 726f 7273   Spelling errors
+000017d0: 2069 6e74 656e 7469 6f6e 616c 2e0a 646f   intentional..do
+000017e0: 6320 3d20 6e6c 7028 7465 7874 290a 0a6d  c = nlp(text)..m
+000017f0: 6174 6368 6572 203d 2046 757a 7a79 4d61  atcher = FuzzyMa
+00001800: 7463 6865 7228 6e6c 702e 766f 6361 6229  tcher(nlp.vocab)
+00001810: 0a6d 6174 6368 6572 2e61 6464 2822 4e41  .matcher.add("NA
+00001820: 4d45 222c 205b 6e6c 7028 2247 7261 6e74  ME", [nlp("Grant
+00001830: 2041 6e64 6572 7365 6e22 295d 290a 6d61   Andersen")]).ma
+00001840: 7463 6865 722e 6164 6428 2247 5045 222c  tcher.add("GPE",
+00001850: 205b 6e6c 7028 224e 6173 6876 696c 6c65   [nlp("Nashville
+00001860: 2229 5d29 0a6d 6174 6368 6573 203d 206d  ")]).matches = m
+00001870: 6174 6368 6572 2864 6f63 290a 0a66 6f72  atcher(doc)..for
+00001880: 206d 6174 6368 5f69 642c 2073 7461 7274   match_id, start
+00001890: 2c20 656e 642c 2072 6174 696f 2c20 7061  , end, ratio, pa
+000018a0: 7474 6572 6e20 696e 206d 6174 6368 6573  ttern in matches
+000018b0: 3a0a 2020 2020 7072 696e 7428 6d61 7463  :.    print(matc
+000018c0: 685f 6964 2c20 646f 635b 7374 6172 743a  h_id, doc[start:
+000018d0: 656e 645d 2c20 7261 7469 6f2c 2070 6174  end], ratio, pat
+000018e0: 7465 726e 290a 6060 600a 0a20 2020 204e  tern).```..    N
+000018f0: 414d 4520 4772 696e 7420 4d20 416e 6465  AME Grint M Ande
+00001900: 7273 6f6e 2038 3020 4772 616e 7420 416e  rson 80 Grant An
+00001910: 6465 7273 656e 0a20 2020 2047 5045 204e  dersen.    GPE N
+00001920: 6173 6876 316c 6520 3832 204e 6173 6876  ashv1le 82 Nashv
+00001930: 696c 6c65 0a0a 0a55 6e6c 696b 6520 7370  ille...Unlike sp
+00001940: 6143 7920 6d61 7463 6865 7273 2c20 7370  aCy matchers, sp
+00001950: 6163 7a7a 206d 6174 6368 6572 7320 6172  aczz matchers ar
+00001960: 6520 7772 6974 7465 6e20 696e 2070 7572  e written in pur
+00001970: 6520 5079 7468 6f6e 2e20 5768 696c 6520  e Python. While 
+00001980: 7468 6579 2061 7265 2072 6571 7569 7265  they are require
+00001990: 6420 746f 2068 6176 6520 6120 7370 6143  d to have a spaC
+000019a0: 7920 766f 6361 6220 7061 7373 6564 2074  y vocab passed t
+000019b0: 6f20 7468 656d 2064 7572 696e 6720 696e  o them during in
+000019c0: 6974 6961 6c69 7a61 7469 6f6e 2c20 7468  itialization, th
+000019d0: 6973 2069 7320 7075 7265 6c79 2066 6f72  is is purely for
+000019e0: 2063 6f6e 7369 7374 656e 6379 2061 7320   consistency as 
+000019f0: 7468 6520 7370 6163 7a7a 206d 6174 6368  the spaczz match
+00001a00: 6572 7320 646f 206e 6f74 2075 7365 2063  ers do not use c
+00001a10: 7572 7265 6e74 6c79 2075 7365 2074 6865  urrently use the
+00001a20: 2073 7061 4379 2076 6f63 6162 2e20 5468   spaCy vocab. Th
+00001a30: 6973 2069 7320 7768 7920 7468 6520 606d  is is why the `m
+00001a40: 6174 6368 5f69 6460 2061 626f 7665 2069  atch_id` above i
+00001a50: 7320 7369 6d70 6c79 2061 2073 7472 696e  s simply a strin
+00001a60: 6720 696e 7374 6561 6420 6f66 2061 6e20  g instead of an 
+00001a70: 696e 7465 6765 7220 7661 6c75 6520 6c69  integer value li
+00001a80: 6b65 2069 6e20 7370 6143 7920 6d61 7463  ke in spaCy matc
+00001a90: 6865 7273 2e0a 0a53 7061 637a 7a20 6d61  hers...Spaczz ma
+00001aa0: 7463 6865 7273 2063 616e 2061 6c73 6f20  tchers can also 
+00001ab0: 6d61 6b65 2075 7365 206f 6620 6f6e 2d6d  make use of on-m
+00001ac0: 6174 6368 2072 756c 6573 2076 6961 2063  atch rules via c
+00001ad0: 616c 6c62 6163 6b20 6675 6e63 7469 6f6e  allback function
+00001ae0: 732e 2054 6865 7365 206f 6e2d 6d61 7463  s. These on-matc
+00001af0: 6820 6361 6c6c 6261 636b 7320 6e65 6564  h callbacks need
+00001b00: 2074 6f20 6163 6365 7074 2074 6865 206d   to accept the m
+00001b10: 6174 6368 6572 2069 7473 656c 662c 2074  atcher itself, t
+00001b20: 6865 2064 6f63 2074 6865 206d 6174 6368  he doc the match
+00001b30: 6572 2077 6173 2063 616c 6c65 6420 6f6e  er was called on
+00001b40: 2c20 7468 6520 6d61 7463 6820 696e 6465  , the match inde
+00001b50: 7820 616e 6420 7468 6520 6d61 7463 6865  x and the matche
+00001b60: 7320 7072 6f64 7563 6564 2062 7920 7468  s produced by th
+00001b70: 6520 6d61 7463 6865 722e 0a0a 0a60 6060  e matcher....```
+00001b80: 7079 7468 6f6e 0a69 6d70 6f72 7420 7370  python.import sp
+00001b90: 6163 790a 6672 6f6d 2073 7061 6379 2e74  acy.from spacy.t
+00001ba0: 6f6b 656e 7320 696d 706f 7274 2053 7061  okens import Spa
+00001bb0: 6e0a 6672 6f6d 2073 7061 637a 7a2e 6d61  n.from spaczz.ma
+00001bc0: 7463 6865 7220 696d 706f 7274 2046 757a  tcher import Fuz
+00001bd0: 7a79 4d61 7463 6865 720a 0a6e 6c70 203d  zyMatcher..nlp =
+00001be0: 2073 7061 6379 2e62 6c61 6e6b 2822 656e   spacy.blank("en
+00001bf0: 2229 0a74 6578 7420 3d20 2222 2247 7269  ").text = """Gri
+00001c00: 6e74 204d 2041 6e64 6572 736f 6e20 6372  nt M Anderson cr
+00001c10: 6561 7465 6420 7370 6163 7a7a 2069 6e20  eated spaczz in 
+00001c20: 6869 7320 686f 6d65 2061 7420 3535 3520  his home at 555 
+00001c30: 4661 6b65 2053 742c 0a41 7074 2035 2069  Fake St,.Apt 5 i
+00001c40: 6e20 4e61 7368 7631 6c65 2c20 544e 2035  n Nashv1le, TN 5
+00001c50: 3535 3535 2d31 3233 3420 696e 2074 6865  5555-1234 in the
+00001c60: 2055 532e 2222 2220 2023 2053 7065 6c6c   US."""  # Spell
+00001c70: 696e 6720 6572 726f 7273 2069 6e74 656e  ing errors inten
+00001c80: 7469 6f6e 616c 2e0a 646f 6320 3d20 6e6c  tional..doc = nl
+00001c90: 7028 7465 7874 290a 0a0a 6465 6620 6164  p(text)...def ad
+00001ca0: 645f 6e61 6d65 5f65 6e74 286d 6174 6368  d_name_ent(match
+00001cb0: 6572 2c20 646f 632c 2069 2c20 6d61 7463  er, doc, i, matc
+00001cc0: 6865 7329 3a0a 2020 2020 2222 2243 616c  hes):.    """Cal
+00001cd0: 6c62 6163 6b20 6f6e 206d 6174 6368 2066  lback on match f
+00001ce0: 756e 6374 696f 6e2e 2041 6464 7320 224e  unction. Adds "N
+00001cf0: 414d 4522 2065 6e74 6974 6965 7320 746f  AME" entities to
+00001d00: 2064 6f63 2e22 2222 0a20 2020 2023 2047   doc.""".    # G
+00001d10: 6574 2074 6865 2063 7572 7265 6e74 206d  et the current m
+00001d20: 6174 6368 2061 6e64 2063 7265 6174 6520  atch and create 
+00001d30: 7475 706c 6520 6f66 2065 6e74 6974 7920  tuple of entity 
+00001d40: 6c61 6265 6c2c 2073 7461 7274 2061 6e64  label, start and
+00001d50: 2065 6e64 2e0a 2020 2020 2320 4170 7065   end..    # Appe
+00001d60: 6e64 2065 6e74 6974 7920 746f 2074 6865  nd entity to the
+00001d70: 2064 6f63 2773 2065 6e74 6974 792e 2028   doc's entity. (
+00001d80: 446f 6e27 7420 6f76 6572 7772 6974 6520  Don't overwrite 
+00001d90: 646f 632e 656e 7473 2129 0a20 2020 205f  doc.ents!).    _
+00001da0: 6d61 7463 685f 6964 2c20 7374 6172 742c  match_id, start,
+00001db0: 2065 6e64 2c20 5f72 6174 696f 2c20 5f70   end, _ratio, _p
+00001dc0: 6174 7465 726e 203d 206d 6174 6368 6573  attern = matches
+00001dd0: 5b69 5d0a 2020 2020 656e 7469 7479 203d  [i].    entity =
+00001de0: 2053 7061 6e28 646f 632c 2073 7461 7274   Span(doc, start
+00001df0: 2c20 656e 642c 206c 6162 656c 3d22 4e41  , end, label="NA
+00001e00: 4d45 2229 0a20 2020 2064 6f63 2e65 6e74  ME").    doc.ent
+00001e10: 7320 2b3d 2028 656e 7469 7479 2c29 0a0a  s += (entity,)..
+00001e20: 0a6d 6174 6368 6572 203d 2046 757a 7a79  .matcher = Fuzzy
+00001e30: 4d61 7463 6865 7228 6e6c 702e 766f 6361  Matcher(nlp.voca
+00001e40: 6229 0a6d 6174 6368 6572 2e61 6464 2822  b).matcher.add("
+00001e50: 4e41 4d45 222c 205b 6e6c 7028 2247 7261  NAME", [nlp("Gra
+00001e60: 6e74 2041 6e64 6572 7365 6e22 295d 2c20  nt Andersen")], 
+00001e70: 6f6e 5f6d 6174 6368 3d61 6464 5f6e 616d  on_match=add_nam
+00001e80: 655f 656e 7429 0a6d 6174 6368 6573 203d  e_ent).matches =
+00001e90: 206d 6174 6368 6572 2864 6f63 290a 0a66   matcher(doc)..f
+00001ea0: 6f72 2065 6e74 2069 6e20 646f 632e 656e  or ent in doc.en
+00001eb0: 7473 3a0a 2020 2020 7072 696e 7428 2865  ts:.    print((e
+00001ec0: 6e74 2e74 6578 742c 2065 6e74 2e73 7461  nt.text, ent.sta
+00001ed0: 7274 2c20 656e 742e 656e 642c 2065 6e74  rt, ent.end, ent
+00001ee0: 2e6c 6162 656c 5f29 290a 6060 600a 0a20  .label_)).```.. 
+00001ef0: 2020 2028 2747 7269 6e74 204d 2041 6e64     ('Grint M And
+00001f00: 6572 736f 6e27 2c20 302c 2033 2c20 274e  erson', 0, 3, 'N
+00001f10: 414d 4527 290a 0a0a 4c69 6b65 2073 7061  AME')...Like spa
+00001f20: 4379 2773 2060 456e 7469 7479 5275 6c65  Cy's `EntityRule
+00001f30: 7260 2c20 6120 7665 7279 2073 696d 696c  r`, a very simil
+00001f40: 6172 2065 6e74 6974 7920 7570 6461 7469  ar entity updati
+00001f50: 6e67 206c 6f67 6963 2068 6173 2062 6565  ng logic has bee
+00001f60: 6e20 696d 706c 656d 656e 7465 6420 696e  n implemented in
+00001f70: 2074 6865 2060 5370 6163 7a7a 5275 6c65   the `SpaczzRule
+00001f80: 7260 2e20 5468 6520 6053 7061 637a 7a52  r`. The `SpaczzR
+00001f90: 756c 6572 6020 616c 736f 2074 616b 6573  uler` also takes
+00001fa0: 2063 6172 6520 6f66 2068 616e 646c 696e   care of handlin
+00001fb0: 6720 6f76 6572 6c61 7070 696e 6720 6d61  g overlapping ma
+00001fc0: 7463 6865 732e 2049 7420 6973 2064 6973  tches. It is dis
+00001fd0: 6375 7373 6564 2069 6e20 6120 6c61 7465  cussed in a late
+00001fe0: 7220 7365 6374 696f 6e2e 0a0a 556e 6c69  r section...Unli
+00001ff0: 6b65 2073 7061 4379 2773 206d 6174 6368  ke spaCy's match
+00002000: 6572 732c 2072 756c 6573 2061 6464 6564  ers, rules added
+00002010: 2074 6f20 7370 6163 7a7a 206d 6174 6368   to spaczz match
+00002020: 6572 7320 6861 7665 206f 7074 696f 6e61  ers have optiona
+00002030: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
+00002040: 6e74 7320 7468 6174 2063 616e 206d 6f64  nts that can mod
+00002050: 6966 7920 7468 6520 6d61 7463 6869 6e67  ify the matching
+00002060: 2062 6568 6176 696f 722e 2054 616b 6520   behavior. Take 
+00002070: 7468 6520 6265 6c6f 7720 6675 7a7a 7920  the below fuzzy 
+00002080: 6d61 7463 6869 6e67 2065 7861 6d70 6c65  matching example
+00002090: 733a 0a0a 0a60 6060 7079 7468 6f6e 0a69  s:...```python.i
+000020a0: 6d70 6f72 7420 7370 6163 790a 6672 6f6d  mport spacy.from
+000020b0: 2073 7061 637a 7a2e 6d61 7463 6865 7220   spaczz.matcher 
+000020c0: 696d 706f 7274 2046 757a 7a79 4d61 7463  import FuzzyMatc
+000020d0: 6865 720a 0a6e 6c70 203d 2073 7061 6379  her..nlp = spacy
+000020e0: 2e62 6c61 6e6b 2822 656e 2229 0a23 204c  .blank("en").# L
+000020f0: 6574 2773 206d 6f64 6966 7920 7468 6520  et's modify the 
+00002100: 6f72 6465 7220 6f66 2074 6865 206e 616d  order of the nam
+00002110: 6520 696e 2074 6865 2074 6578 742e 0a74  e in the text..t
+00002120: 6578 7420 3d20 2222 2241 6e64 6572 736f  ext = """Anderso
+00002130: 6e2c 2047 7269 6e74 2063 7265 6174 6564  n, Grint created
+00002140: 2073 7061 637a 7a20 696e 2068 6973 2068   spaczz in his h
+00002150: 6f6d 6520 6174 2035 3535 2046 616b 6520  ome at 555 Fake 
+00002160: 5374 2c0a 4170 7420 3520 696e 204e 6173  St,.Apt 5 in Nas
+00002170: 6876 316c 652c 2054 4e20 3535 3535 352d  hv1le, TN 55555-
+00002180: 3132 3334 2069 6e20 7468 6520 5553 2e22  1234 in the US."
+00002190: 2222 2020 2320 5370 656c 6c69 6e67 2065  ""  # Spelling e
+000021a0: 7272 6f72 7320 696e 7465 6e74 696f 6e61  rrors intentiona
+000021b0: 6c2e 0a64 6f63 203d 206e 6c70 2874 6578  l..doc = nlp(tex
+000021c0: 7429 0a0a 6d61 7463 6865 7220 3d20 4675  t)..matcher = Fu
+000021d0: 7a7a 794d 6174 6368 6572 286e 6c70 2e76  zzyMatcher(nlp.v
+000021e0: 6f63 6162 290a 6d61 7463 6865 722e 6164  ocab).matcher.ad
+000021f0: 6428 224e 414d 4522 2c20 5b6e 6c70 2822  d("NAME", [nlp("
+00002200: 4772 616e 7420 416e 6465 7273 656e 2229  Grant Andersen")
+00002210: 5d29 0a6d 6174 6368 6573 203d 206d 6174  ]).matches = mat
+00002220: 6368 6572 2864 6f63 290a 0a23 2054 6865  cher(doc)..# The
+00002230: 2064 6566 6175 6c74 2066 757a 7a79 206d   default fuzzy m
+00002240: 6174 6368 696e 6720 7365 7474 696e 6773  atching settings
+00002250: 2077 696c 6c20 6e6f 7420 6669 6e64 2061   will not find a
+00002260: 206d 6174 6368 2e0a 666f 7220 6d61 7463   match..for matc
+00002270: 685f 6964 2c20 7374 6172 742c 2065 6e64  h_id, start, end
+00002280: 2c20 7261 7469 6f2c 2070 6174 7465 726e  , ratio, pattern
+00002290: 2069 6e20 6d61 7463 6865 733a 0a20 2020   in matches:.   
+000022a0: 2070 7269 6e74 286d 6174 6368 5f69 642c   print(match_id,
+000022b0: 2064 6f63 5b73 7461 7274 3a65 6e64 5d2c   doc[start:end],
+000022c0: 2072 6174 696f 2c20 7061 7474 6572 6e29   ratio, pattern)
+000022d0: 0a60 6060 0a0a 4e65 7874 2077 6520 6368  .```..Next we ch
+000022e0: 616e 6765 2074 6865 2066 757a 7a79 206d  ange the fuzzy m
+000022f0: 6174 6368 696e 6720 6265 6861 7669 6f72  atching behavior
+00002300: 2066 6f72 2074 6865 2070 6174 7465 726e   for the pattern
+00002310: 2069 6e20 7468 6520 224e 414d 4522 2072   in the "NAME" r
+00002320: 756c 652e 0a0a 0a60 6060 7079 7468 6f6e  ule....```python
+00002330: 0a69 6d70 6f72 7420 7370 6163 790a 6672  .import spacy.fr
+00002340: 6f6d 2073 7061 637a 7a2e 6d61 7463 6865  om spaczz.matche
+00002350: 7220 696d 706f 7274 2046 757a 7a79 4d61  r import FuzzyMa
+00002360: 7463 6865 720a 0a6e 6c70 203d 2073 7061  tcher..nlp = spa
+00002370: 6379 2e62 6c61 6e6b 2822 656e 2229 0a23  cy.blank("en").#
+00002380: 204c 6574 2773 206d 6f64 6966 7920 7468   Let's modify th
+00002390: 6520 6f72 6465 7220 6f66 2074 6865 206e  e order of the n
+000023a0: 616d 6520 696e 2074 6865 2074 6578 742e  ame in the text.
+000023b0: 0a74 6578 7420 3d20 2222 2241 6e64 6572  .text = """Ander
+000023c0: 736f 6e2c 2047 7269 6e74 2063 7265 6174  son, Grint creat
+000023d0: 6564 2073 7061 637a 7a20 696e 2068 6973  ed spaczz in his
+000023e0: 2068 6f6d 6520 6174 2035 3535 2046 616b   home at 555 Fak
+000023f0: 6520 5374 2c0a 4170 7420 3520 696e 204e  e St,.Apt 5 in N
+00002400: 6173 6876 316c 652c 2054 4e20 3535 3535  ashv1le, TN 5555
+00002410: 352d 3132 3334 2069 6e20 7468 6520 5553  5-1234 in the US
+00002420: 2e22 2222 2020 2320 5370 656c 6c69 6e67  ."""  # Spelling
+00002430: 2065 7272 6f72 7320 696e 7465 6e74 696f   errors intentio
+00002440: 6e61 6c2e 0a64 6f63 203d 206e 6c70 2874  nal..doc = nlp(t
+00002450: 6578 7429 0a0a 6d61 7463 6865 7220 3d20  ext)..matcher = 
+00002460: 4675 7a7a 794d 6174 6368 6572 286e 6c70  FuzzyMatcher(nlp
+00002470: 2e76 6f63 6162 290a 6d61 7463 6865 722e  .vocab).matcher.
+00002480: 6164 6428 224e 414d 4522 2c20 5b6e 6c70  add("NAME", [nlp
+00002490: 2822 4772 616e 7420 416e 6465 7273 656e  ("Grant Andersen
+000024a0: 2229 5d2c 206b 7761 7267 733d 5b7b 2266  ")], kwargs=[{"f
+000024b0: 757a 7a79 5f66 756e 6322 3a20 2274 6f6b  uzzy_func": "tok
+000024c0: 656e 5f73 6f72 7422 7d5d 290a 6d61 7463  en_sort"}]).matc
+000024d0: 6865 7320 3d20 6d61 7463 6865 7228 646f  hes = matcher(do
+000024e0: 6329 0a0a 2320 5468 6520 6465 6661 756c  c)..# The defaul
+000024f0: 7420 6675 7a7a 7920 6d61 7463 6869 6e67  t fuzzy matching
+00002500: 2073 6574 7469 6e67 7320 7769 6c6c 206e   settings will n
+00002510: 6f74 2066 696e 6420 6120 6d61 7463 682e  ot find a match.
+00002520: 0a66 6f72 206d 6174 6368 5f69 642c 2073  .for match_id, s
+00002530: 7461 7274 2c20 656e 642c 2072 6174 696f  tart, end, ratio
+00002540: 2c20 7061 7474 6572 6e20 696e 206d 6174  , pattern in mat
+00002550: 6368 6573 3a0a 2020 2020 7072 696e 7428  ches:.    print(
+00002560: 6d61 7463 685f 6964 2c20 646f 635b 7374  match_id, doc[st
+00002570: 6172 743a 656e 645d 2c20 7261 7469 6f2c  art:end], ratio,
+00002580: 2070 6174 7465 726e 290a 6060 600a 0a20   pattern).```.. 
+00002590: 2020 204e 414d 4520 416e 6465 7273 6f6e     NAME Anderson
+000025a0: 2c20 4772 696e 7420 3833 2047 7261 6e74  , Grint 83 Grant
+000025b0: 2041 6e64 6572 7365 6e0a 0a0a 5468 6520   Andersen...The 
+000025c0: 6675 6c6c 206c 6973 7420 6f66 206b 6579  full list of key
+000025d0: 776f 7264 2061 7267 756d 656e 7473 2061  word arguments a
+000025e0: 7661 696c 6162 6c65 2066 6f72 2066 757a  vailable for fuz
+000025f0: 7a79 206d 6174 6368 696e 6720 7365 7474  zy matching sett
+00002600: 696e 6773 2069 6e63 6c75 6465 733a 0a0a  ings includes:..
+00002610: 2d20 6069 676e 6f72 655f 6361 7365 6020  - `ignore_case` 
+00002620: 2862 6f6f 6c29 3a20 5768 6574 6865 7220  (bool): Whether 
+00002630: 746f 206c 6f77 6572 2d63 6173 6520 7465  to lower-case te
+00002640: 7874 2062 6566 6f72 6520 6d61 7463 6869  xt before matchi
+00002650: 6e67 2e20 4465 6661 756c 7420 6973 2060  ng. Default is `
+00002660: 5472 7565 602e 0a2d 2060 6d69 6e5f 7260  True`..- `min_r`
+00002670: 2028 696e 7429 3a20 4d69 6e69 6d75 6d20   (int): Minimum 
+00002680: 6d61 7463 6820 7261 7469 6f20 7265 7175  match ratio requ
+00002690: 6972 6564 2e0a 2d20 6074 6872 6573 6860  ired..- `thresh`
+000026a0: 2028 696e 7429 3a20 4966 2074 6869 7320   (int): If this 
+000026b0: 7261 7469 6f20 6973 2065 7863 6565 6465  ratio is exceede
+000026c0: 6420 696e 2069 6e69 7469 616c 2073 6361  d in initial sca
+000026d0: 6e2c 2061 6e64 2060 666c 6578 203e 2030  n, and `flex > 0
+000026e0: 602c 206e 6f20 6f70 7469 6d69 7a61 7469  `, no optimizati
+000026f0: 6f6e 2077 696c 6c20 6265 2061 7474 656d  on will be attem
+00002700: 7074 6564 2e20 4966 2060 666c 6578 203d  pted. If `flex =
+00002710: 3d20 3060 2c20 6074 6872 6573 6860 2068  = 0`, `thresh` h
+00002720: 6173 206e 6f20 6566 6665 6374 2e20 4465  as no effect. De
+00002730: 6661 756c 7420 6973 2060 3130 3060 2e0a  fault is `100`..
+00002740: 2d20 6066 757a 7a79 5f66 756e 6360 2028  - `fuzzy_func` (
+00002750: 7374 7229 3a20 4b65 7920 6e61 6d65 206f  str): Key name o
+00002760: 6620 6675 7a7a 7920 6d61 7463 6869 6e67  f fuzzy matching
+00002770: 2066 756e 6374 696f 6e20 746f 2075 7365   function to use
+00002780: 2e20 416c 6c20 7261 7069 6466 757a 7a20  . All rapidfuzz 
+00002790: 6d61 7463 6869 6e67 2066 756e 6374 696f  matching functio
+000027a0: 6e73 2077 6974 6820 6465 6661 756c 7420  ns with default 
+000027b0: 7365 7474 696e 6773 2061 7265 2061 7661  settings are ava
+000027c0: 696c 6162 6c65 2e20 4164 6469 7469 6f6e  ilable. Addition
+000027d0: 616c 2066 757a 7a79 206d 6174 6368 696e  al fuzzy matchin
+000027e0: 6720 6675 6e63 7469 6f6e 7320 6361 6e20  g functions can 
+000027f0: 6265 2072 6567 6973 7465 7265 6420 6279  be registered by
+00002800: 2075 7365 7273 2e20 4465 6661 756c 7420   users. Default 
+00002810: 6973 2060 2273 696d 706c 6522 603a 0a20  is `"simple"`:. 
+00002820: 2020 202a 2060 2273 696d 706c 6522 6020     * `"simple"` 
+00002830: 3d20 6072 6174 696f 600a 2020 2020 2a20  = `ratio`.    * 
+00002840: 6022 7061 7274 6961 6c22 6020 3d20 6070  `"partial"` = `p
+00002850: 6172 7469 616c 5f72 6174 696f 600a 2020  artial_ratio`.  
+00002860: 2020 2a20 6022 746f 6b65 6e22 6020 3d20    * `"token"` = 
+00002870: 6074 6f6b 656e 5f72 6174 696f 600a 2020  `token_ratio`.  
+00002880: 2020 2a20 6022 746f 6b65 6e5f 7365 7422    * `"token_set"
+00002890: 6020 3d20 6074 6f6b 656e 5f73 6574 5f72  ` = `token_set_r
+000028a0: 6174 696f 600a 2020 2020 2a20 6022 746f  atio`.    * `"to
+000028b0: 6b65 6e5f 736f 7274 2260 203d 2060 746f  ken_sort"` = `to
+000028c0: 6b65 6e5f 736f 7274 5f72 6174 696f 600a  ken_sort_ratio`.
+000028d0: 2020 2020 2a20 6022 7061 7274 6961 6c5f      * `"partial_
+000028e0: 746f 6b65 6e22 6020 3d20 6070 6172 7469  token"` = `parti
+000028f0: 616c 5f74 6f6b 656e 5f72 6174 696f 600a  al_token_ratio`.
+00002900: 2020 2020 2a20 6022 7061 7274 6961 6c5f      * `"partial_
+00002910: 746f 6b65 6e5f 7365 7422 6020 3d20 6070  token_set"` = `p
+00002920: 6172 7469 616c 5f74 6f6b 656e 5f73 6574  artial_token_set
+00002930: 5f72 6174 696f 600a 2020 2020 2a20 6022  _ratio`.    * `"
+00002940: 7061 7274 6961 6c5f 746f 6b65 6e5f 736f  partial_token_so
+00002950: 7274 2260 203d 2060 7061 7274 6961 6c5f  rt"` = `partial_
+00002960: 746f 6b65 6e5f 736f 7274 5f72 6174 696f  token_sort_ratio
+00002970: 600a 2020 2020 2a20 6022 7765 6967 6874  `.    * `"weight
+00002980: 6564 2260 203d 2060 5752 6174 696f 600a  ed"` = `WRatio`.
+00002990: 2020 2020 2a20 6022 7175 6963 6b22 6020      * `"quick"` 
+000029a0: 3d20 6051 5261 7469 6f60 0a20 2020 202a  = `QRatio`.    *
+000029b0: 2060 2270 6172 7469 616c 5f61 6c69 676e   `"partial_align
+000029c0: 6d65 6e74 2260 203d 2060 7061 7274 6961  ment"` = `partia
+000029d0: 6c5f 7261 7469 6f5f 616c 6967 6e6d 656e  l_ratio_alignmen
+000029e0: 7460 2028 5265 7175 6972 6573 2060 7261  t` (Requires `ra
+000029f0: 7069 6466 757a 7a3e 3d32 2e30 2e33 6029  pidfuzz>=2.0.3`)
+00002a00: 0a2d 2060 666c 6578 6020 2869 6e74 7c4c  .- `flex` (int|L
+00002a10: 6974 6572 616c 5b27 6465 6661 756c 7427  iteral['default'
+00002a20: 2c20 276d 696e 272c 2027 6d61 7827 5d29  , 'min', 'max'])
+00002a30: 3a20 4e75 6d62 6572 206f 6620 746f 6b65  : Number of toke
+00002a40: 6e73 2074 6f20 6d6f 7665 206d 6174 6368  ns to move match
+00002a50: 2062 6f75 6e64 6172 6965 7320 6c65 6674   boundaries left
+00002a60: 2061 6e64 2072 6967 6874 2064 7572 696e   and right durin
+00002a70: 6720 6f70 7469 6d69 7a61 7469 6f6e 2e20  g optimization. 
+00002a80: 4361 6e20 6265 2061 6e20 6069 6e74 6020  Can be an `int` 
+00002a90: 7769 7468 2061 206d 6178 206f 6620 606c  with a max of `l
+00002aa0: 656e 2870 6174 7465 726e 2960 2061 6e64  en(pattern)` and
+00002ab0: 2061 206d 696e 206f 6620 6030 602c 2028   a min of `0`, (
+00002ac0: 7769 6c6c 2077 6172 6e20 616e 6420 6368  will warn and ch
+00002ad0: 616e 6765 2069 6620 6869 6768 6572 206f  ange if higher o
+00002ae0: 7220 6c6f 7765 7229 2e20 6022 6d61 7822  r lower). `"max"
+00002af0: 602c 2060 226d 696e 2260 2c20 6f72 2060  `, `"min"`, or `
+00002b00: 2264 6566 6175 6c74 2260 2061 7265 2061  "default"` are a
+00002b10: 6c73 6f20 7661 6c69 642e 2044 6566 6175  lso valid. Defau
+00002b20: 6c74 2069 7320 6022 6465 6661 756c 7422  lt is `"default"
+00002b30: 603a 2060 6c65 6e28 7061 7474 6572 6e29  `: `len(pattern)
+00002b40: 202f 2f20 3260 2e0a 2d20 606d 696e 5f72   // 2`..- `min_r
+00002b50: 3160 2028 696e 747c 4e6f 6e65 293a 204f  1` (int|None): O
+00002b60: 7074 696f 6e61 6c20 6772 616e 756c 6172  ptional granular
+00002b70: 2063 6f6e 7472 6f6c 206f 7665 7220 7468   control over th
+00002b80: 6520 6d69 6e69 6d75 6d20 6d61 7463 6820  e minimum match 
+00002b90: 7261 7469 6f20 7265 7175 6972 6564 2066  ratio required f
+00002ba0: 6f72 2073 656c 6563 7469 6f6e 2064 7572  or selection dur
+00002bb0: 696e 6720 7468 6520 696e 6974 6961 6c20  ing the initial 
+00002bc0: 7363 616e 2e20 4966 2060 666c 6578 203d  scan. If `flex =
+00002bd0: 3d20 3060 2c20 606d 696e 5f72 3160 2077  = 0`, `min_r1` w
+00002be0: 696c 6c20 6265 206f 7665 7277 7269 7474  ill be overwritt
+00002bf0: 656e 2062 7920 606d 696e 5f72 3260 2e20  en by `min_r2`. 
+00002c00: 4966 2060 666c 6578 203e 2030 602c 2060  If `flex > 0`, `
+00002c10: 6d69 6e5f 7231 6020 6d75 7374 2062 6520  min_r1` must be 
+00002c20: 6c6f 7765 7220 7468 616e 2060 6d69 6e5f  lower than `min_
+00002c30: 7232 6020 616e 6420 226c 6f77 2220 696e  r2` and "low" in
+00002c40: 2067 656e 6572 616c 2062 6563 6175 7365   general because
+00002c50: 206d 6174 6368 2062 6f75 6e64 6172 6965   match boundarie
+00002c60: 7320 6172 6520 6e6f 7420 666c 6578 6564  s are not flexed
+00002c70: 2069 6e69 7469 616c 6c79 2e20 4465 6661   initially. Defa
+00002c80: 756c 7420 6973 2060 4e6f 6e65 602c 2077  ult is `None`, w
+00002c90: 6869 6368 2077 696c 6c20 7265 7375 6c74  hich will result
+00002ca0: 2069 6e20 606d 696e 5f72 3160 2062 6569   in `min_r1` bei
+00002cb0: 6e67 2073 6574 2074 6f20 6072 6f75 6e64  ng set to `round
+00002cc0: 286d 696e 5f72 202f 2031 2e35 2960 2e0a  (min_r / 1.5)`..
+00002cd0: 0a23 2323 2052 6567 6578 4d61 7463 6865  .### RegexMatche
+00002ce0: 720a 0a54 6865 2062 6173 6963 2075 7361  r..The basic usa
+00002cf0: 6765 206f 6620 7468 6520 7265 6765 7820  ge of the regex 
+00002d00: 6d61 7463 6865 7220 6973 2061 6c73 6f20  matcher is also 
+00002d10: 6661 6972 6c79 2073 696d 696c 6172 2074  fairly similar t
+00002d20: 6f20 7370 6143 7927 7320 6050 6872 6173  o spaCy's `Phras
+00002d30: 654d 6174 6368 6572 602e 2049 7420 6163  eMatcher`. It ac
+00002d40: 6365 7074 7320 7265 6765 7820 7061 7474  cepts regex patt
+00002d50: 6572 6e73 2061 7320 7374 7269 6e67 7320  erns as strings 
+00002d60: 736f 2066 6c61 6773 206d 7573 7420 6265  so flags must be
+00002d70: 2069 6e6c 696e 652e 2052 6567 6578 6573   inline. Regexes
+00002d80: 2061 7265 2063 6f6d 7069 6c65 6420 7769   are compiled wi
+00002d90: 7468 2074 6865 205b 7265 6765 785d 2868  th the [regex](h
+00002da0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00002db0: 7072 6f6a 6563 742f 7265 6765 782f 2920  project/regex/) 
+00002dc0: 7061 636b 6167 6520 736f 2061 7070 726f  package so appro
+00002dd0: 7869 6d61 7465 2022 6675 7a7a 7922 206d  ximate "fuzzy" m
+00002de0: 6174 6368 696e 6720 6973 2073 7570 706f  atching is suppo
+00002df0: 7274 6564 2e20 546f 2070 726f 7669 6465  rted. To provide
+00002e00: 2061 6363 6573 7320 746f 2074 6865 7365   access to these
+00002e10: 2022 6675 7a7a 7922 206d 6174 6368 2072   "fuzzy" match r
+00002e20: 6573 756c 7473 2074 6865 206d 6174 6368  esults the match
+00002e30: 6572 2072 6574 7572 6e73 2061 2063 616c  er returns a cal
+00002e40: 6375 6c61 7465 6420 6675 7a7a 7920 7261  culated fuzzy ra
+00002e50: 7469 6f20 616e 6420 6d61 7463 6865 6420  tio and matched 
+00002e60: 7061 7474 6572 6e2c 2061 6c6f 6e67 2077  pattern, along w
+00002e70: 6974 6820 6d61 7463 6820 6964 2c20 7374  ith match id, st
+00002e80: 6172 7420 616e 6420 656e 6420 696e 666f  art and end info
+00002e90: 726d 6174 696f 6e2c 2073 6f20 6d61 6b65  rmation, so make
+00002ea0: 2073 7572 6520 746f 2069 6e63 6c75 6465   sure to include
+00002eb0: 2076 6172 6961 626c 6573 2066 6f72 2074   variables for t
+00002ec0: 6865 2072 6174 696f 2061 6e64 2070 6174  he ratio and pat
+00002ed0: 7465 726e 2077 6865 6e20 756e 7061 636b  tern when unpack
+00002ee0: 696e 6720 7265 7375 6c74 732e 0a0a 0a60  ing results....`
+00002ef0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
+00002f00: 7370 6163 790a 6672 6f6d 2073 7061 637a  spacy.from spacz
+00002f10: 7a2e 6d61 7463 6865 7220 696d 706f 7274  z.matcher import
+00002f20: 2052 6567 6578 4d61 7463 6865 720a 0a6e   RegexMatcher..n
+00002f30: 6c70 203d 2073 7061 6379 2e62 6c61 6e6b  lp = spacy.blank
+00002f40: 2822 656e 2229 0a74 6578 7420 3d20 2222  ("en").text = ""
+00002f50: 2241 6e64 6572 736f 6e2c 2047 7269 6e74  "Anderson, Grint
+00002f60: 2063 7265 6174 6564 2073 7061 637a 7a20   created spaczz 
+00002f70: 696e 2068 6973 2068 6f6d 6520 6174 2035  in his home at 5
+00002f80: 3535 2046 616b 6520 5374 2c0a 4170 7420  55 Fake St,.Apt 
+00002f90: 3520 696e 204e 6173 6876 316c 652c 2054  5 in Nashv1le, T
+00002fa0: 4e20 3535 3535 352d 3132 3334 2069 6e20  N 55555-1234 in 
+00002fb0: 7468 6520 5553 2e22 2222 2020 2320 5370  the US."""  # Sp
+00002fc0: 656c 6c69 6e67 2065 7272 6f72 7320 696e  elling errors in
+00002fd0: 7465 6e74 696f 6e61 6c2e 0a64 6f63 203d  tentional..doc =
+00002fe0: 206e 6c70 2874 6578 7429 0a0a 6d61 7463   nlp(text)..matc
+00002ff0: 6865 7220 3d20 5265 6765 784d 6174 6368  her = RegexMatch
+00003000: 6572 286e 6c70 2e76 6f63 6162 290a 2320  er(nlp.vocab).# 
+00003010: 5573 6520 696e 6c69 6e65 2066 6c61 6773  Use inline flags
+00003020: 2066 6f72 2072 6567 6578 2073 7472 696e   for regex strin
+00003030: 6773 2061 7320 6e65 6564 6564 0a6d 6174  gs as needed.mat
+00003040: 6368 6572 2e61 6464 280a 2020 2020 225a  cher.add(.    "Z
+00003050: 4950 222c 0a20 2020 205b 7222 5c62 5c64  IP",.    [r"\b\d
+00003060: 7b35 7d28 3f3a 5b2d 5c73 5d5c 647b 347d  {5}(?:[-\s]\d{4}
+00003070: 293f 5c62 225d 2c0a 290a 6d61 7463 6865  )?\b"],.).matche
+00003080: 722e 6164 6428 2247 5045 222c 205b 7222  r.add("GPE", [r"
+00003090: 2875 7361 297b 643c 3d31 7d22 5d29 2020  (usa){d<=1}"])  
+000030a0: 2320 4675 7a7a 7920 7265 6765 782e 0a6d  # Fuzzy regex..m
+000030b0: 6174 6368 6573 203d 206d 6174 6368 6572  atches = matcher
+000030c0: 2864 6f63 290a 0a66 6f72 206d 6174 6368  (doc)..for match
+000030d0: 5f69 642c 2073 7461 7274 2c20 656e 642c  _id, start, end,
+000030e0: 2072 6174 696f 2c20 7061 7474 6572 6e20   ratio, pattern 
+000030f0: 696e 206d 6174 6368 6573 3a0a 2020 2020  in matches:.    
+00003100: 7072 696e 7428 6d61 7463 685f 6964 2c20  print(match_id, 
+00003110: 646f 635b 7374 6172 743a 656e 645d 2c20  doc[start:end], 
+00003120: 7261 7469 6f2c 2070 6174 7465 726e 290a  ratio, pattern).
+00003130: 6060 600a 0a20 2020 205a 4950 2035 3535  ```..    ZIP 555
+00003140: 3535 2d31 3233 3420 3130 3020 5c62 5c64  55-1234 100 \b\d
+00003150: 7b35 7d28 3f3a 5b2d 5c73 5d5c 647b 347d  {5}(?:[-\s]\d{4}
+00003160: 293f 5c62 0a20 2020 2047 5045 2055 5320  )?\b.    GPE US 
+00003170: 3830 2028 7573 6129 7b64 3c3d 317d 0a0a  80 (usa){d<=1}..
+00003180: 0a53 7061 637a 7a20 6d61 7463 6865 7273  .Spaczz matchers
+00003190: 2063 616e 2061 6c73 6f20 6d61 6b65 2075   can also make u
+000031a0: 7365 206f 6620 6f6e 2d6d 6174 6368 2072  se of on-match r
+000031b0: 756c 6573 2076 6961 2063 616c 6c62 6163  ules via callbac
+000031c0: 6b20 6675 6e63 7469 6f6e 732e 2054 6865  k functions. The
+000031d0: 7365 206f 6e2d 6d61 7463 6820 6361 6c6c  se on-match call
+000031e0: 6261 636b 7320 6e65 6564 2074 6f20 6163  backs need to ac
+000031f0: 6365 7074 2074 6865 206d 6174 6368 6572  cept the matcher
+00003200: 2069 7473 656c 662c 2074 6865 2064 6f63   itself, the doc
+00003210: 2074 6865 206d 6174 6368 6572 2077 6173   the matcher was
+00003220: 2063 616c 6c65 6420 6f6e 2c20 7468 6520   called on, the 
+00003230: 6d61 7463 6820 696e 6465 7820 616e 6420  match index and 
+00003240: 7468 6520 6d61 7463 6865 7320 7072 6f64  the matches prod
+00003250: 7563 6564 2062 7920 7468 6520 6d61 7463  uced by the matc
+00003260: 6865 722e 2053 6565 2074 6865 2066 757a  her. See the fuz
+00003270: 7a79 206d 6174 6368 6572 2075 7361 6765  zy matcher usage
+00003280: 2065 7861 6d70 6c65 2061 626f 7665 2066   example above f
+00003290: 6f72 2064 6574 6169 6c73 2e0a 0a4c 696b  or details...Lik
+000032a0: 6520 7468 6520 6675 7a7a 7920 6d61 7463  e the fuzzy matc
+000032b0: 6865 722c 2074 6865 2072 6567 6578 206d  her, the regex m
+000032c0: 6174 6368 6572 2068 6173 206f 7074 696f  atcher has optio
+000032d0: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+000032e0: 6d65 6e74 7320 7468 6174 2063 616e 206d  ments that can m
+000032f0: 6f64 6966 7920 6d61 7463 6869 6e67 2062  odify matching b
+00003300: 6568 6176 696f 722e 2054 616b 6520 7468  ehavior. Take th
+00003310: 6520 6265 6c6f 7720 7265 6765 7820 6d61  e below regex ma
+00003320: 7463 6869 6e67 2065 7861 6d70 6c65 2e0a  tching example..
+00003330: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00003340: 7274 2073 7061 6379 0a66 726f 6d20 7370  rt spacy.from sp
+00003350: 6163 7a7a 2e6d 6174 6368 6572 2069 6d70  aczz.matcher imp
+00003360: 6f72 7420 5265 6765 784d 6174 6368 6572  ort RegexMatcher
+00003370: 0a0a 6e6c 7020 3d20 7370 6163 792e 626c  ..nlp = spacy.bl
+00003380: 616e 6b28 2265 6e22 290a 7465 7874 203d  ank("en").text =
+00003390: 2022 2222 416e 6465 7273 6f6e 2c20 4772   """Anderson, Gr
+000033a0: 696e 7420 6372 6561 7465 6420 7370 6163  int created spac
+000033b0: 7a7a 2069 6e20 6869 7320 686f 6d65 2061  zz in his home a
+000033c0: 7420 3535 3520 4661 6b65 2053 742c 0a41  t 555 Fake St,.A
+000033d0: 7074 2035 2069 6e20 4e61 7368 7631 6c65  pt 5 in Nashv1le
+000033e0: 2c20 544e 2035 3535 3535 2d31 3233 3420  , TN 55555-1234 
+000033f0: 696e 2074 6865 2055 5341 2e22 2222 2020  in the USA."""  
+00003400: 2320 5370 656c 6c69 6e67 2065 7272 6f72  # Spelling error
+00003410: 7320 696e 7465 6e74 696f 6e61 6c2e 204e  s intentional. N
+00003420: 6f74 6963 6520 2755 5341 2720 6865 7265  otice 'USA' here
+00003430: 2e0a 646f 6320 3d20 6e6c 7028 7465 7874  ..doc = nlp(text
+00003440: 290a 0a6d 6174 6368 6572 203d 2052 6567  )..matcher = Reg
+00003450: 6578 4d61 7463 6865 7228 6e6c 702e 766f  exMatcher(nlp.vo
+00003460: 6361 6229 0a23 2055 7365 2069 6e6c 696e  cab).# Use inlin
+00003470: 6520 666c 6167 7320 666f 7220 7265 6765  e flags for rege
+00003480: 7820 7374 7269 6e67 7320 6173 206e 6565  x strings as nee
+00003490: 6465 640a 6d61 7463 6865 722e 6164 6428  ded.matcher.add(
+000034a0: 0a20 2020 2022 5354 5245 4554 222c 205b  .    "STREET", [
+000034b0: 2273 7472 6565 745f 6164 6472 6573 7365  "street_addresse
+000034c0: 7322 5d2c 206b 7761 7267 733d 5b7b 2270  s"], kwargs=[{"p
+000034d0: 7265 6465 6622 3a20 5472 7565 7d5d 0a29  redef": True}].)
+000034e0: 2020 2320 5573 6520 7072 6564 6566 696e    # Use predefin
+000034f0: 6564 2072 6567 6578 2062 7920 6b65 7920  ed regex by key 
+00003500: 6e61 6d65 2e0a 2320 4265 6c6f 7720 7769  name..# Below wi
+00003510: 6c6c 206e 6f74 2065 7870 616e 6420 7061  ll not expand pa
+00003520: 7274 6961 6c20 6d61 7463 6865 7320 746f  rtial matches to
+00003530: 2073 7061 6e20 626f 756e 6461 7269 6573   span boundaries
+00003540: 2e0a 6d61 7463 6865 722e 6164 6428 2247  ..matcher.add("G
+00003550: 5045 222c 205b 7222 283f 6929 5b55 5d28  PE", [r"(?i)[U](
+00003560: 6e69 7465 647c 5c2e 3f29 203f 5b53 5d28  nited|\.?) ?[S](
+00003570: 7461 7465 737c 5c2e 3f29 225d 2c20 6b77  tates|\.?)"], kw
+00003580: 6172 6773 3d5b 7b22 7061 7274 6961 6c22  args=[{"partial"
+00003590: 3a20 4661 6c73 657d 5d29 0a6d 6174 6368  : False}]).match
+000035a0: 6573 203d 206d 6174 6368 6572 2864 6f63  es = matcher(doc
+000035b0: 290a 0a66 6f72 206d 6174 6368 5f69 642c  )..for match_id,
+000035c0: 2073 7461 7274 2c20 656e 642c 2072 6174   start, end, rat
+000035d0: 696f 2c20 7061 7474 6572 6e20 696e 206d  io, pattern in m
+000035e0: 6174 6368 6573 3a0a 2020 2020 7072 696e  atches:.    prin
+000035f0: 7428 0a20 2020 2020 2020 206d 6174 6368  t(.        match
+00003600: 5f69 642c 2064 6f63 5b73 7461 7274 3a65  _id, doc[start:e
+00003610: 6e64 5d2c 2072 6174 696f 2c20 7061 7474  nd], ratio, patt
+00003620: 6572 6e0a 2020 2020 2920 2023 2063 6f6d  ern.    )  # com
+00003630: 6d61 2069 6e20 7265 7375 6c74 2069 736e  ma in result isn
+00003640: 2774 2069 6465 616c 202d 2073 6565 2022  't ideal - see "
+00003650: 526f 6164 6d61 7022 0a60 6060 0a0a 2020  Roadmap".```..  
+00003660: 2020 5354 5245 4554 2035 3535 2046 616b    STREET 555 Fak
+00003670: 6520 5374 2c20 3130 3020 7374 7265 6574  e St, 100 street
+00003680: 5f61 6464 7265 7373 6573 0a0a 0a54 6865  _addresses...The
+00003690: 2066 756c 6c20 6c69 7374 206f 6620 6b65   full list of ke
+000036a0: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+000036b0: 6176 6169 6c61 626c 6520 666f 7220 7265  available for re
+000036c0: 6765 7820 6d61 7463 6869 6e67 2073 6574  gex matching set
+000036d0: 7469 6e67 7320 696e 636c 7564 6573 3a0a  tings includes:.
+000036e0: 0a2d 2060 6967 6e6f 7265 5f63 6173 6560  .- `ignore_case`
+000036f0: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+00003700: 2074 6f20 6c6f 7765 722d 6361 7365 2074   to lower-case t
+00003710: 6578 7420 6265 666f 7265 206d 6174 6368  ext before match
+00003720: 696e 672e 2044 6566 6175 6c74 2069 7320  ing. Default is 
+00003730: 6054 7275 6560 2e0a 2d20 606d 696e 5f72  `True`..- `min_r
+00003740: 6020 2869 6e74 293a 204d 696e 696d 756d  ` (int): Minimum
+00003750: 206d 6174 6368 2072 6174 696f 2072 6571   match ratio req
+00003760: 7569 7265 642e 0a2d 2060 6675 7a7a 795f  uired..- `fuzzy_
+00003770: 7765 6967 6874 7360 2028 7374 7229 3a20  weights` (str): 
+00003780: 4e61 6d65 206f 6620 7765 6967 6874 696e  Name of weightin
+00003790: 6720 6d65 7468 6f64 2066 6f72 2072 6567  g method for reg
+000037a0: 6578 2069 6e73 6572 7469 6f6e 2c20 6465  ex insertion, de
+000037b0: 6c65 7469 6f6e 2c20 616e 6420 7375 6273  letion, and subs
+000037c0: 7469 7475 696f 6e20 636f 756e 7473 2e20  tituion counts. 
+000037d0: 4164 6469 7469 6f6e 616c 2077 6569 6768  Additional weigh
+000037e0: 7469 6e67 206d 6574 686f 6473 2063 616e  ting methods can
+000037f0: 2062 6520 7265 6769 7374 6572 6564 2062   be registered b
+00003800: 7920 7573 6572 732e 2044 6566 6175 6c74  y users. Default
+00003810: 2069 7320 6022 696e 6465 6c22 602e 0a20   is `"indel"`.. 
+00003820: 2020 202a 2060 2269 6e64 656c 2260 203d     * `"indel"` =
+00003830: 2060 2831 2c20 312c 2032 2960 0a20 2020   `(1, 1, 2)`.   
+00003840: 202a 2060 226c 6576 2260 203d 2060 2831   * `"lev"` = `(1
+00003850: 2c20 312c 2031 2960 0a2d 2060 7061 7274  , 1, 1)`.- `part
+00003860: 6961 6c60 3a20 2862 6f6f 6c29 3a20 5768  ial`: (bool): Wh
+00003870: 6574 6865 7220 7061 7274 6961 6c20 6d61  ether partial ma
+00003880: 7463 6865 7320 7368 6f75 6c64 2062 6520  tches should be 
+00003890: 6578 7465 6e64 6564 2074 6f20 6054 6f6b  extended to `Tok
+000038a0: 656e 6020 6f72 2060 5370 616e 6020 626f  en` or `Span` bo
+000038b0: 756e 6461 7269 6573 2069 6e20 6064 6f63  undaries in `doc
+000038c0: 6020 6f72 206e 6f74 2e20 466f 7220 6578  ` or not. For ex
+000038d0: 616d 706c 652c 2074 6865 2072 6567 6578  ample, the regex
+000038e0: 206f 6e6c 7920 6d61 7463 6865 7320 7061   only matches pa
+000038f0: 7274 206f 6620 6120 6054 6f6b 656e 6020  rt of a `Token` 
+00003900: 6f72 2060 5370 616e 6020 696e 2060 646f  or `Span` in `do
+00003910: 6360 2e20 4465 6661 756c 7420 6973 2060  c`. Default is `
+00003920: 5472 7565 602e 0a2d 2060 7072 6564 6566  True`..- `predef
+00003930: 6020 2873 7472 696e 6729 3a20 5768 6574  ` (string): Whet
+00003940: 6865 7220 7468 6520 7265 6765 7820 7374  her the regex st
+00003950: 7269 6e67 2073 686f 756c 6420 6265 2069  ring should be i
+00003960: 6e74 6572 7072 6574 6564 2061 7320 6120  nterpreted as a 
+00003970: 6b65 7920 746f 2061 2070 7265 6465 6669  key to a predefi
+00003980: 6e65 6420 7265 6765 7820 7061 7474 6572  ned regex patter
+00003990: 6e20 6f72 206e 6f74 2e20 4164 6469 7469  n or not. Additi
+000039a0: 6f6e 616c 2070 7265 6465 6669 6e65 6420  onal predefined 
+000039b0: 7265 6765 7820 7061 7474 6572 6e73 2063  regex patterns c
+000039c0: 616e 2062 6520 7265 6769 7374 6572 6564  an be registered
+000039d0: 2062 7920 7573 6572 732e 2044 6566 6175   by users. Defau
+000039e0: 6c74 2069 7320 6046 616c 7365 2e60 0a20  lt is `False.`. 
+000039f0: 2020 202a 2060 2264 6174 6573 2260 0a20     * `"dates"`. 
+00003a00: 2020 202a 2060 2274 696d 6573 2260 0a20     * `"times"`. 
+00003a10: 2020 202a 2060 2270 686f 6e65 7322 600a     * `"phones"`.
+00003a20: 2020 2020 2a20 6022 7068 6f6e 6573 5f77      * `"phones_w
+00003a30: 6974 685f 6578 7473 2260 0a20 2020 202a  ith_exts"`.    *
+00003a40: 2060 226c 696e 6b73 2260 0a20 2020 202a   `"links"`.    *
+00003a50: 2060 2265 6d61 696c 7322 600a 2020 2020   `"emails"`.    
+00003a60: 2a20 6022 6970 7322 600a 2020 2020 2a20  * `"ips"`.    * 
+00003a70: 6022 6970 7636 7322 600a 2020 2020 2a20  `"ipv6s"`.    * 
+00003a80: 6022 7072 6963 6573 2260 0a20 2020 202a  `"prices"`.    *
+00003a90: 2060 2268 6578 5f63 6f6c 6f72 7322 600a   `"hex_colors"`.
+00003aa0: 2020 2020 2a20 6022 6372 6564 6974 5f63      * `"credit_c
+00003ab0: 6172 6473 2260 0a20 2020 202a 2060 2262  ards"`.    * `"b
+00003ac0: 7463 5f61 6464 7265 7373 6573 2260 0a20  tc_addresses"`. 
+00003ad0: 2020 202a 2060 2273 7472 6565 745f 6164     * `"street_ad
+00003ae0: 6472 6573 7365 7322 600a 2020 2020 2a20  dresses"`.    * 
+00003af0: 6022 7a69 705f 636f 6465 7322 600a 2020  `"zip_codes"`.  
+00003b00: 2020 2a20 6022 706f 5f62 6f78 6573 2260    * `"po_boxes"`
+00003b10: 0a20 2020 202a 2060 2273 736e 5f6e 756d  .    * `"ssn_num
+00003b20: 6265 7273 2260 0a0a 2323 2320 5369 6d69  bers"`..### Simi
+00003b30: 6c61 7269 7479 4d61 7463 6865 720a 0a54  larityMatcher..T
+00003b40: 6865 2062 6173 6963 2075 7361 6765 206f  he basic usage o
+00003b50: 6620 7468 6520 7369 6d69 6c61 7269 7479  f the similarity
+00003b60: 206d 6174 6368 6572 2069 7320 7369 6d69   matcher is simi
+00003b70: 6c61 7220 746f 2073 7061 4379 2773 2060  lar to spaCy's `
+00003b80: 5068 7261 7365 4d61 7463 6865 7260 2065  PhraseMatcher` e
+00003b90: 7863 6570 7420 6974 2072 6574 7572 6e73  xcept it returns
+00003ba0: 2074 6865 2076 6563 746f 7220 7369 6d69   the vector simi
+00003bb0: 6c61 7269 7479 2072 6174 696f 2061 6e64  larity ratio and
+00003bc0: 206d 6174 6368 6564 2070 6174 7465 726e   matched pattern
+00003bd0: 2c20 616c 6f6e 6720 7769 7468 206d 6174  , along with mat
+00003be0: 6368 2069 642c 2073 7461 7274 2061 6e64  ch id, start and
+00003bf0: 2065 6e64 2069 6e66 6f72 6d61 7469 6f6e   end information
+00003c00: 2c20 736f 206d 616b 6520 7375 7265 2074  , so make sure t
+00003c10: 6f20 696e 636c 7564 6520 7661 7269 6162  o include variab
+00003c20: 6c65 7320 666f 7220 7468 6520 7261 7469  les for the rati
+00003c30: 6f20 616e 6420 7061 7474 6572 6e20 7768  o and pattern wh
+00003c40: 656e 2075 6e70 6163 6b69 6e67 2072 6573  en unpacking res
+00003c50: 756c 7473 2e0a 0a49 6e20 6f72 6465 7220  ults...In order 
+00003c60: 746f 2070 726f 6475 6365 206d 6561 6e69  to produce meani
+00003c70: 6e67 6675 6c20 7265 7375 6c74 7320 6672  ngful results fr
+00003c80: 6f6d 2074 6865 2073 696d 696c 6172 6974  om the similarit
+00003c90: 7920 6d61 7463 6865 722c 2061 2073 7061  y matcher, a spa
+00003ca0: 4379 206d 6f64 656c 2077 6974 6820 776f  Cy model with wo
+00003cb0: 7264 2076 6563 746f 7273 2028 6578 2e20  rd vectors (ex. 
+00003cc0: 6d65 6469 756d 206f 7220 6c61 7267 6520  medium or large 
+00003cd0: 456e 676c 6973 6820 6d6f 6465 6c73 2920  English models) 
+00003ce0: 6d75 7374 2062 6520 7573 6564 2074 6f20  must be used to 
+00003cf0: 696e 6974 6961 6c69 7a65 2074 6865 206d  initialize the m
+00003d00: 6174 6368 6572 2c20 7072 6f63 6573 7320  atcher, process 
+00003d10: 7468 6520 7461 7267 6574 2064 6f63 756d  the target docum
+00003d20: 656e 742c 2061 6e64 2070 726f 6365 7373  ent, and process
+00003d30: 2061 6e79 2070 6174 7465 726e 7320 6164   any patterns ad
+00003d40: 6465 642e 0a0a 0a60 6060 7079 7468 6f6e  ded....```python
+00003d50: 0a69 6d70 6f72 7420 7370 6163 790a 6672  .import spacy.fr
+00003d60: 6f6d 2073 7061 637a 7a2e 6d61 7463 6865  om spaczz.matche
+00003d70: 7220 696d 706f 7274 2053 696d 696c 6172  r import Similar
+00003d80: 6974 794d 6174 6368 6572 0a0a 6e6c 7020  ityMatcher..nlp 
+00003d90: 3d20 7370 6163 792e 6c6f 6164 2822 656e  = spacy.load("en
+00003da0: 5f63 6f72 655f 7765 625f 6d64 2229 0a74  _core_web_md").t
+00003db0: 6578 7420 3d20 2249 206c 696b 6520 6170  ext = "I like ap
+00003dc0: 706c 6573 2c20 6772 6170 6573 2061 6e64  ples, grapes and
+00003dd0: 2062 616e 616e 6173 2e22 0a64 6f63 203d   bananas.".doc =
+00003de0: 206e 6c70 2874 6578 7429 0a0a 2320 6c6f   nlp(text)..# lo
+00003df0: 7765 7269 6e67 206d 696e 5f72 3220 6672  wering min_r2 fr
+00003e00: 6f6d 2064 6566 6175 6c74 206f 6620 3735  om default of 75
+00003e10: 2074 6f20 7072 6f64 7563 6520 6d61 7463   to produce matc
+00003e20: 6865 7320 696e 2074 6869 7320 6578 616d  hes in this exam
+00003e30: 706c 650a 6d61 7463 6865 7220 3d20 5369  ple.matcher = Si
+00003e40: 6d69 6c61 7269 7479 4d61 7463 6865 7228  milarityMatcher(
+00003e50: 6e6c 702e 766f 6361 622c 206d 696e 5f72  nlp.vocab, min_r
+00003e60: 323d 3635 290a 6d61 7463 6865 722e 6164  2=65).matcher.ad
+00003e70: 6428 2246 5255 4954 222c 205b 6e6c 7028  d("FRUIT", [nlp(
+00003e80: 2266 7275 6974 2229 5d29 0a6d 6174 6368  "fruit")]).match
+00003e90: 6573 203d 206d 6174 6368 6572 2864 6f63  es = matcher(doc
+00003ea0: 290a 0a66 6f72 206d 6174 6368 5f69 642c  )..for match_id,
+00003eb0: 2073 7461 7274 2c20 656e 642c 2072 6174   start, end, rat
+00003ec0: 696f 2c20 7061 7474 6572 6e20 696e 206d  io, pattern in m
+00003ed0: 6174 6368 6573 3a0a 2020 2020 7072 696e  atches:.    prin
+00003ee0: 7428 6d61 7463 685f 6964 2c20 646f 635b  t(match_id, doc[
+00003ef0: 7374 6172 743a 656e 645d 2c20 7261 7469  start:end], rati
+00003f00: 6f2c 2070 6174 7465 726e 290a 6060 600a  o, pattern).```.
+00003f10: 0a20 2020 2046 5255 4954 2061 7070 6c65  .    FRUIT apple
+00003f20: 7320 3730 2066 7275 6974 0a20 2020 2046  s 70 fruit.    F
+00003f30: 5255 4954 2067 7261 7065 7320 3733 2066  RUIT grapes 73 f
+00003f40: 7275 6974 0a20 2020 2046 5255 4954 2062  ruit.    FRUIT b
+00003f50: 616e 616e 6173 2037 3020 6672 7569 740a  ananas 70 fruit.
+00003f60: 0a0a 506c 6561 7365 206e 6f74 6520 7468  ..Please note th
+00003f70: 6174 2065 7665 6e20 666f 7220 7468 6520  at even for the 
+00003f80: 6d6f 7374 6c79 2070 7572 652d 5079 7468  mostly pure-Pyth
+00003f90: 6f6e 2073 7061 637a 7a2c 2074 6869 7320  on spaczz, this 
+00003fa0: 7072 6f63 6573 7320 6973 2063 7572 7265  process is curre
+00003fb0: 6e74 6c79 2065 7874 7265 6d65 6c79 2073  ntly extremely s
+00003fc0: 6c6f 7720 736f 2062 6520 6d69 6e64 6675  low so be mindfu
+00003fd0: 6c20 6f66 2074 6865 2073 636f 7065 2069  l of the scope i
+00003fe0: 6e20 7768 6963 6820 6974 2069 7320 6170  n which it is ap
+00003ff0: 706c 6965 642e 2045 6e61 626c 696e 6720  plied. Enabling 
+00004000: 4750 5520 7375 7070 6f72 7420 696e 2073  GPU support in s
+00004010: 7061 4379 2028 5b73 6565 2068 6572 655d  paCy ([see here]
+00004020: 2868 7474 7073 3a2f 2f73 7061 6379 2e69  (https://spacy.i
+00004030: 6f2f 7573 6167 6523 6770 7529 2920 7368  o/usage#gpu)) sh
+00004040: 6f75 6c64 2069 6d70 726f 7665 2074 6865  ould improve the
+00004050: 2073 7065 6564 2073 6f6d 6577 6861 742c   speed somewhat,
+00004060: 2062 7574 2049 2062 656c 6965 7665 2074   but I believe t
+00004070: 6865 2070 726f 6365 7373 2077 696c 6c20  he process will 
+00004080: 7374 696c 6c20 6265 2062 6f74 746c 656e  still be bottlen
+00004090: 6563 6b65 6420 696e 2074 6865 2070 7572  ecked in the pur
+000040a0: 652d 5079 7468 6f6e 2073 6561 7263 6820  e-Python search 
+000040b0: 616c 676f 7269 7468 6d20 756e 7469 6c20  algorithm until 
+000040c0: 4920 6465 7665 6c6f 7020 6120 6265 7474  I develop a bett
+000040d0: 6572 2073 6561 7263 6820 616c 676f 7269  er search algori
+000040e0: 7468 6d20 616e 642f 6f72 2064 726f 7020  thm and/or drop 
+000040f0: 7468 6520 7365 6172 6368 2074 6f20 6c6f  the search to lo
+00004100: 7765 722d 6c65 7665 6c20 636f 6465 2028  wer-level code (
+00004110: 6578 2043 292e 0a0a 416c 736f 2061 7320  ex C)...Also as 
+00004120: 6120 736f 6d65 7768 6174 2065 7870 6572  a somewhat exper
+00004130: 696d 656e 7461 6c20 6665 6174 7572 652c  imental feature,
+00004140: 2074 6865 2073 696d 696c 6172 6974 7920   the similarity 
+00004150: 6d61 7463 6865 7220 6973 206e 6f74 2063  matcher is not c
+00004160: 7572 7265 6e74 6c79 2070 6172 7420 6f66  urrently part of
+00004170: 2074 6865 2060 5370 6163 7a7a 5275 6c65   the `SpaczzRule
+00004180: 7260 206e 6f72 2064 6f65 7320 6974 2068  r` nor does it h
+00004190: 6176 6520 6120 7365 7061 7261 7465 2072  ave a separate r
+000041a0: 756c 6572 2e20 4966 2079 6f75 206e 6565  uler. If you nee
+000041b0: 6420 746f 2061 6464 2073 696d 696c 6172  d to add similar
+000041c0: 6974 7920 6d61 7463 6865 7320 746f 2061  ity matches to a
+000041d0: 2060 446f 6360 2773 2065 6e74 6974 6965   `Doc`'s entitie
+000041e0: 7320 796f 7520 7769 6c6c 206e 6565 6420  s you will need 
+000041f0: 746f 2075 7365 2061 6e20 6f6e 2d6d 6174  to use an on-mat
+00004200: 6368 2063 616c 6c62 6163 6b20 666f 7220  ch callback for 
+00004210: 7468 6520 7469 6d65 2062 6569 6e67 2e20  the time being. 
+00004220: 506c 6561 7365 2073 6565 2074 6865 2066  Please see the f
+00004230: 757a 7a79 206d 6174 6368 6572 206f 6e2d  uzzy matcher on-
+00004240: 6d61 7463 6820 6361 6c6c 6261 636b 2065  match callback e
+00004250: 7861 6d70 6c65 2061 626f 7665 2066 6f72  xample above for
+00004260: 2069 6465 6173 2e20 4966 2074 6865 7265   ideas. If there
+00004270: 2069 7320 656e 6f75 6768 2069 6e74 6572   is enough inter
+00004280: 6573 7420 696e 2069 6e74 6567 7261 7469  est in integrati
+00004290: 6e67 2f63 7265 6174 696e 6720 6120 7275  ng/creating a ru
+000042a0: 6c65 7220 666f 7220 7468 6520 7369 6d69  ler for the simi
+000042b0: 6c61 7269 7479 206d 6174 6368 6572 2074  larity matcher t
+000042c0: 6869 7320 6361 6e20 6265 2064 6f6e 652e  his can be done.
+000042d0: 0a0a 5468 6520 6675 6c6c 206c 6973 7420  ..The full list 
+000042e0: 6f66 206b 6579 776f 7264 2061 7267 756d  of keyword argum
+000042f0: 656e 7473 2061 7661 696c 6162 6c65 2066  ents available f
+00004300: 6f72 2073 696d 696c 6172 6974 7920 6d61  or similarity ma
+00004310: 7463 6869 6e67 2073 6574 7469 6e67 7320  tching settings 
+00004320: 696e 636c 7564 6573 3a0a 0a2d 2060 6967  includes:..- `ig
+00004330: 6e6f 7265 5f63 6173 6560 2028 626f 6f6c  nore_case` (bool
+00004340: 293a 2057 6865 7468 6572 2074 6f20 6c6f  ): Whether to lo
+00004350: 7765 722d 6361 7365 2074 6578 7420 6265  wer-case text be
+00004360: 666f 7265 2066 757a 7a79 206d 6174 6368  fore fuzzy match
+00004370: 696e 672e 2044 6566 6175 6c74 2069 7320  ing. Default is 
+00004380: 6054 7275 6560 2e0a 2d20 606d 696e 5f72  `True`..- `min_r
+00004390: 6020 2869 6e74 293a 204d 696e 696d 756d  ` (int): Minimum
+000043a0: 206d 6174 6368 2072 6174 696f 2072 6571   match ratio req
+000043b0: 7569 7265 642e 0a2d 2060 7468 7265 7368  uired..- `thresh
+000043c0: 6020 2869 6e74 293a 2049 6620 7468 6973  ` (int): If this
+000043d0: 2072 6174 696f 2069 7320 6578 6365 6564   ratio is exceed
+000043e0: 6564 2069 6e20 696e 6974 6961 6c20 7363  ed in initial sc
+000043f0: 616e 2c20 616e 6420 6066 6c65 7820 3e20  an, and `flex > 
+00004400: 3060 2c20 6e6f 206f 7074 696d 697a 6174  0`, no optimizat
+00004410: 696f 6e20 7769 6c6c 2062 6520 6174 7465  ion will be atte
+00004420: 6d70 7465 642e 2049 6620 6066 6c65 7820  mpted. If `flex 
+00004430: 3d3d 2030 602c 2060 7468 7265 7368 6020  == 0`, `thresh` 
+00004440: 6861 7320 6e6f 2065 6666 6563 742e 2044  has no effect. D
+00004450: 6566 6175 6c74 2069 7320 6031 3030 602e  efault is `100`.
+00004460: 0a2d 2060 666c 6578 6020 2869 6e74 7c4c  .- `flex` (int|L
+00004470: 6974 6572 616c 5b27 6465 6661 756c 7427  iteral['default'
+00004480: 2c20 276d 696e 272c 2027 6d61 7827 5d29  , 'min', 'max'])
+00004490: 3a20 4e75 6d62 6572 206f 6620 746f 6b65  : Number of toke
+000044a0: 6e73 2074 6f20 6d6f 7665 206d 6174 6368  ns to move match
+000044b0: 2062 6f75 6e64 6172 6965 7320 6c65 6674   boundaries left
+000044c0: 2061 6e64 2072 6967 6874 2064 7572 696e   and right durin
+000044d0: 6720 6f70 7469 6d69 7a61 7469 6f6e 2e20  g optimization. 
+000044e0: 4361 6e20 6265 2061 6e20 6069 6e74 6020  Can be an `int` 
+000044f0: 7769 7468 2061 206d 6178 206f 6620 606c  with a max of `l
+00004500: 656e 2870 6174 7465 726e 2960 2061 6e64  en(pattern)` and
+00004510: 2061 206d 696e 206f 6620 6030 602c 2028   a min of `0`, (
+00004520: 7769 6c6c 2077 6172 6e20 616e 6420 6368  will warn and ch
+00004530: 616e 6765 2069 6620 6869 6768 6572 206f  ange if higher o
+00004540: 7220 6c6f 7765 7229 2e20 6022 6d61 7822  r lower). `"max"
+00004550: 602c 2060 226d 696e 2260 2c20 6f72 2060  `, `"min"`, or `
+00004560: 2264 6566 6175 6c74 2260 2061 7265 2061  "default"` are a
+00004570: 6c73 6f20 7661 6c69 642e 2044 6566 6175  lso valid. Defau
+00004580: 6c74 2069 7320 6022 6465 6661 756c 7422  lt is `"default"
+00004590: 603a 2060 6c65 6e28 7061 7474 6572 6e29  `: `len(pattern)
+000045a0: 202f 2f20 3260 2e0a 2d20 606d 696e 5f72   // 2`..- `min_r
+000045b0: 3160 2028 696e 747c 4e6f 6e65 293a 204f  1` (int|None): O
+000045c0: 7074 696f 6e61 6c20 6772 616e 756c 6172  ptional granular
+000045d0: 2063 6f6e 7472 6f6c 206f 7665 7220 7468   control over th
+000045e0: 6520 6d69 6e69 6d75 6d20 6d61 7463 6820  e minimum match 
+000045f0: 7261 7469 6f20 7265 7175 6972 6564 2066  ratio required f
+00004600: 6f72 2073 656c 6563 7469 6f6e 2064 7572  or selection dur
+00004610: 696e 6720 7468 6520 696e 6974 6961 6c20  ing the initial 
+00004620: 7363 616e 2e20 4966 2060 666c 6578 203d  scan. If `flex =
+00004630: 3d20 3060 2c20 606d 696e 5f72 3160 2077  = 0`, `min_r1` w
+00004640: 696c 6c20 6265 206f 7665 7277 7269 7474  ill be overwritt
+00004650: 656e 2062 7920 606d 696e 5f72 3260 2e20  en by `min_r2`. 
+00004660: 4966 2060 666c 6578 203e 2030 602c 2060  If `flex > 0`, `
+00004670: 6d69 6e5f 7231 6020 6d75 7374 2062 6520  min_r1` must be 
+00004680: 6c6f 7765 7220 7468 616e 2060 6d69 6e5f  lower than `min_
+00004690: 7232 6020 616e 6420 226c 6f77 2220 696e  r2` and "low" in
+000046a0: 2067 656e 6572 616c 2062 6563 6175 7365   general because
+000046b0: 206d 6174 6368 2062 6f75 6e64 6172 6965   match boundarie
+000046c0: 7320 6172 6520 6e6f 7420 666c 6578 6564  s are not flexed
+000046d0: 2069 6e69 7469 616c 6c79 2e20 4465 6661   initially. Defa
+000046e0: 756c 7420 6973 2060 4e6f 6e65 602c 2077  ult is `None`, w
+000046f0: 6869 6368 2077 696c 6c20 7265 7375 6c74  hich will result
+00004700: 2069 6e20 606d 696e 5f72 3160 2062 6569   in `min_r1` bei
+00004710: 6e67 2073 6574 2074 6f20 6072 6f75 6e64  ng set to `round
+00004720: 286d 696e 5f72 202f 2031 2e35 2960 2e0a  (min_r / 1.5)`..
+00004730: 2d20 606d 696e 5f72 3260 2028 696e 747c  - `min_r2` (int|
+00004740: 4e6f 6e65 293a 204f 7074 696f 6e61 6c20  None): Optional 
+00004750: 6772 616e 756c 6172 2063 6f6e 7472 6f6c  granular control
+00004760: 206f 7665 7220 7468 6520 6d69 6e69 6d75   over the minimu
+00004770: 6d20 6d61 7463 6820 7261 7469 6f20 7265  m match ratio re
+00004780: 7175 6972 6564 2066 6f72 2073 656c 6563  quired for selec
+00004790: 7469 6f6e 2064 7572 696e 6720 6d61 7463  tion during matc
+000047a0: 6820 6f70 7469 6d69 7a61 7469 6f6e 2e20  h optimization. 
+000047b0: 4e65 6564 7320 746f 2062 6520 6869 6768  Needs to be high
+000047c0: 6572 2074 6861 6e20 606d 696e 5f72 3160  er than `min_r1`
+000047d0: 2061 6e64 2022 6869 6768 2220 696e 2067   and "high" in g
+000047e0: 656e 6572 616c 2074 6f20 656e 7375 7265  eneral to ensure
+000047f0: 206f 6e6c 7920 7175 616c 6974 7920 6d61   only quality ma
+00004800: 7463 6865 7320 6172 6520 7265 7475 726e  tches are return
+00004810: 6564 2e20 4465 6661 756c 7420 6973 2060  ed. Default is `
+00004820: 4e6f 6e65 602c 2077 6869 6368 2077 696c  None`, which wil
+00004830: 6c20 7265 7375 6c74 2069 6e20 606d 696e  l result in `min
+00004840: 5f72 3260 2062 6569 6e67 2073 6574 2074  _r2` being set t
+00004850: 6f20 606d 696e 5f72 602e 0a0a 2323 2320  o `min_r`...### 
+00004860: 546f 6b65 6e4d 6174 6368 6572 0a0a 2a4e  TokenMatcher..*N
+00004870: 6f74 653a 2073 7061 4379 2773 2060 4d61  ote: spaCy's `Ma
+00004880: 7463 6865 7260 206e 6f77 2073 7570 706f  tcher` now suppo
+00004890: 7274 7320 5b66 757a 7a79 206d 6174 6368  rts [fuzzy match
+000048a0: 696e 675d 2868 7474 7073 3a2f 2f73 7061  ing](https://spa
+000048b0: 6379 2e69 6f2f 7573 6167 652f 7633 2d35  cy.io/usage/v3-5
+000048c0: 2366 757a 7a79 292c 2073 6f20 756e 6c65  #fuzzy), so unle
+000048d0: 7373 2079 6f75 206e 6565 6420 6120 7370  ss you need a sp
+000048e0: 6563 6966 6963 2066 6561 7475 7265 2066  ecific feature f
+000048f0: 726f 6d20 7370 6163 7a7a 2773 2060 546f  rom spaczz's `To
+00004900: 6b65 6e4d 6174 6368 6572 602c 2069 7420  kenMatcher`, it 
+00004910: 6973 2068 6967 686c 7920 7265 636f 6d6d  is highly recomm
+00004920: 656e 6465 6420 746f 2075 7365 2073 7061  ended to use spa
+00004930: 4379 2773 206d 7563 6820 6661 7374 6572  Cy's much faster
+00004940: 2060 4d61 7463 6865 7260 2e2a 0a0a 5468   `Matcher`.*..Th
+00004950: 6520 6261 7369 6320 7573 6167 6520 6f66  e basic usage of
+00004960: 2074 6865 2074 6f6b 656e 206d 6174 6368   the token match
+00004970: 6572 2069 7320 7369 6d69 6c61 7220 746f  er is similar to
+00004980: 2073 7061 4379 2773 2060 4d61 7463 6865   spaCy's `Matche
+00004990: 7260 2e20 4974 2061 6363 6570 7473 206c  r`. It accepts l
+000049a0: 6162 656c 6564 2070 6174 7465 726e 7320  abeled patterns 
+000049b0: 696e 2074 6865 2066 6f72 6d20 6f66 206c  in the form of l
+000049c0: 6973 7473 206f 6620 6469 6374 696f 6e61  ists of dictiona
+000049d0: 7269 6573 2077 6865 7265 2065 6163 6820  ries where each 
+000049e0: 6c69 7374 2064 6573 6372 6962 6573 2061  list describes a
+000049f0: 6e20 696e 6469 7669 6475 616c 2070 6174  n individual pat
+00004a00: 7465 726e 2061 6e64 2065 6163 6820 6469  tern and each di
+00004a10: 6374 696f 6e61 7279 2064 6573 6372 6962  ctionary describ
+00004a20: 6573 2061 6e20 696e 6469 7669 6475 616c  es an individual
+00004a30: 2074 6f6b 656e 2e0a 0a54 6865 2074 6f6b   token...The tok
+00004a40: 656e 206d 6174 6368 6572 2061 6363 6570  en matcher accep
+00004a50: 7473 2061 6c6c 2074 6865 2073 616d 6520  ts all the same 
+00004a60: 746f 6b65 6e20 6174 7472 6962 7574 6573  token attributes
+00004a70: 2061 6e64 2070 6174 7465 726e 2073 796e   and pattern syn
+00004a80: 7461 7820 6173 2069 7427 7320 7370 6143  tax as it's spaC
+00004a90: 7920 636f 756e 7465 7270 6172 7420 6275  y counterpart bu
+00004aa0: 7420 6164 6473 2066 757a 7a79 2061 6e64  t adds fuzzy and
+00004ab0: 2066 757a 7a79 2d72 6567 6578 2073 7570   fuzzy-regex sup
+00004ac0: 706f 7274 2e0a 0a60 2246 555a 5a59 2260  port...`"FUZZY"`
+00004ad0: 2061 6e64 2060 2246 5245 4745 5822 6020   and `"FREGEX"` 
+00004ae0: 6172 6520 7468 6520 7477 6f20 6164 6469  are the two addi
+00004af0: 7469 6f6e 616c 2073 7061 4379 2074 6f6b  tional spaCy tok
+00004b00: 656e 2070 6174 7465 726e 206f 7074 696f  en pattern optio
+00004b10: 6e73 2e0a 0a46 6f72 2065 7861 6d70 6c65  ns...For example
+00004b20: 3a0a 0a60 6060 7079 7468 6f6e 0a5b 0a20  :..```python.[. 
+00004b30: 2020 207b 2254 4558 5422 3a20 7b22 4652     {"TEXT": {"FR
+00004b40: 4547 4558 223a 2022 2864 6174 6162 6173  EGEX": "(databas
+00004b50: 6529 7b65 3c3d 317d 227d 7d2c 0a20 2020  e){e<=1}"}},.   
+00004b60: 207b 224c 4f57 4552 223a 207b 2246 555a   {"LOWER": {"FUZ
+00004b70: 5a59 223a 2022 6163 6365 7373 222c 2022  ZY": "access", "
+00004b80: 4d49 4e5f 5222 3a20 3835 2c20 2246 555a  MIN_R": 85, "FUZ
+00004b90: 5a59 5f46 554e 4322 3a20 2271 7569 636b  ZY_FUNC": "quick
+00004ba0: 5f6c 6576 227d 7d2c 0a5d 0a60 6060 0a0a  _lev"}},.].```..
+00004bb0: 2a2a 4d61 6b65 2073 7572 6520 746f 2075  **Make sure to u
+00004bc0: 7365 2075 7070 6572 6361 7365 2064 6963  se uppercase dic
+00004bd0: 7469 6f6e 6172 7920 6b65 7973 2069 6e20  tionary keys in 
+00004be0: 7061 7474 6572 6e73 2e2a 2a0a 0a54 6865  patterns.**..The
+00004bf0: 2066 756c 6c20 6c69 7374 206f 6620 6b65   full list of ke
+00004c00: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
+00004c10: 6176 6169 6c61 626c 6520 666f 7220 746f  available for to
+00004c20: 6b65 6e20 6d61 7463 6869 6e67 2073 6574  ken matching set
+00004c30: 7469 6e67 7320 696e 636c 7564 6573 3a0a  tings includes:.
+00004c40: 0a2d 2060 6967 6e6f 7265 5f63 6173 6560  .- `ignore_case`
+00004c50: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+00004c60: 2074 6f20 6c6f 7765 722d 6361 7365 2074   to lower-case t
+00004c70: 6578 7420 6265 666f 7265 206d 6174 6368  ext before match
+00004c80: 696e 672e 2043 616e 206f 6e6c 7920 6265  ing. Can only be
+00004c90: 2073 6574 2061 7420 7468 6520 7061 7474   set at the patt
+00004ca0: 6572 6e20 6c65 7665 6c2e 2046 6f72 2022  ern level. For "
+00004cb0: 4655 5a5a 5922 2061 6e64 2022 4652 4547  FUZZY" and "FREG
+00004cc0: 4558 2220 7061 7474 6572 6e73 2e20 4465  EX" patterns. De
+00004cd0: 6661 756c 7420 6973 2060 5472 7565 602e  fault is `True`.
+00004ce0: 0a2d 2060 6d69 6e5f 7260 2028 696e 7429  .- `min_r` (int)
+00004cf0: 3a20 4d69 6e69 6d75 6d20 6d61 7463 6820  : Minimum match 
+00004d00: 7261 7469 6f20 7265 7175 6972 6564 2e20  ratio required. 
+00004d10: 466f 7220 2246 555a 5a59 2220 616e 6420  For "FUZZY" and 
+00004d20: 2246 5245 4745 5822 2070 6174 7465 726e  "FREGEX" pattern
+00004d30: 732e 0a2d 2060 6675 7a7a 795f 6675 6e63  s..- `fuzzy_func
+00004d40: 6020 2873 7472 293a 204b 6579 206e 616d  ` (str): Key nam
+00004d50: 6520 6f66 2066 757a 7a79 206d 6174 6368  e of fuzzy match
+00004d60: 696e 6720 6675 6e63 7469 6f6e 2074 6f20  ing function to 
+00004d70: 7573 652e 2043 616e 206f 6e6c 7920 6265  use. Can only be
+00004d80: 2073 6574 2061 7420 7468 6520 7061 7474   set at the patt
+00004d90: 6572 6e20 6c65 7665 6c2e 2046 6f72 2022  ern level. For "
+00004da0: 4655 5a5a 5922 2070 6174 7465 726e 7320  FUZZY" patterns 
+00004db0: 6f6e 6c79 2e20 416c 6c20 7261 7069 6466  only. All rapidf
+00004dc0: 757a 7a20 6d61 7463 6869 6e67 2066 756e  uzz matching fun
+00004dd0: 6374 696f 6e73 2077 6974 6820 6465 6661  ctions with defa
+00004de0: 756c 7420 7365 7474 696e 6773 2061 7265  ult settings are
+00004df0: 2061 7661 696c 6162 6c65 2c20 686f 7765   available, howe
+00004e00: 7665 7220 616e 7920 746f 6b65 6e2d 6261  ver any token-ba
+00004e10: 7365 6420 6675 6e63 7469 6f6e 7320 7072  sed functions pr
+00004e20: 6f76 6964 6520 6e6f 2075 7469 6c69 7479  ovide no utility
+00004e30: 2061 7420 7468 6520 696e 6469 7669 6475   at the individu
+00004e40: 616c 2074 6f6b 656e 206c 6576 656c 2e20  al token level. 
+00004e50: 4164 6469 7469 6f6e 616c 2066 757a 7a79  Additional fuzzy
+00004e60: 206d 6174 6368 696e 6720 6675 6e63 7469   matching functi
+00004e70: 6f6e 7320 6361 6e20 6265 2072 6567 6973  ons can be regis
+00004e80: 7465 7265 6420 6279 2075 7365 7273 2e20  tered by users. 
+00004e90: 496e 636c 7564 6564 2c20 616e 6420 7573  Included, and us
+00004ea0: 6566 756c 2c20 6675 6e63 7469 6f6e 7320  eful, functions 
+00004eb0: 6172 6520 2874 6865 2064 6566 6175 6c74  are (the default
+00004ec0: 2069 7320 6073 696d 706c 6560 293a 0a20   is `simple`):. 
+00004ed0: 2020 202a 2060 2273 696d 706c 6522 6020     * `"simple"` 
+00004ee0: 3d20 6072 6174 696f 600a 2020 2020 2a20  = `ratio`.    * 
+00004ef0: 6022 7061 7274 6961 6c22 6020 3d20 6070  `"partial"` = `p
+00004f00: 6172 7469 616c 5f72 6174 696f 600a 2020  artial_ratio`.  
+00004f10: 2020 2a20 6022 7175 6963 6b22 6020 3d20    * `"quick"` = 
+00004f20: 6051 5261 7469 6f60 0a20 2020 202a 2060  `QRatio`.    * `
+00004f30: 2270 6172 7469 616c 5f61 6c69 676e 6d65  "partial_alignme
+00004f40: 6e74 2260 203d 2060 7061 7274 6961 6c5f  nt"` = `partial_
+00004f50: 7261 7469 6f5f 616c 6967 6e6d 656e 7460  ratio_alignment`
+00004f60: 2028 5265 7175 6972 6573 2060 7261 7069   (Requires `rapi
+00004f70: 6466 757a 7a3e 3d32 2e30 2e33 6029 0a2d  dfuzz>=2.0.3`).-
+00004f80: 2060 6675 7a7a 795f 7765 6967 6874 7360   `fuzzy_weights`
+00004f90: 2028 7374 7229 3a20 4e61 6d65 206f 6620   (str): Name of 
+00004fa0: 7765 6967 6874 696e 6720 6d65 7468 6f64  weighting method
+00004fb0: 2066 6f72 2072 6567 6578 2069 6e73 6572   for regex inser
+00004fc0: 7469 6f6e 2c20 6465 6c65 7469 6f6e 2c20  tion, deletion, 
+00004fd0: 616e 6420 7375 6273 7469 7475 696f 6e20  and substituion 
+00004fe0: 636f 756e 7473 2e20 4164 6469 7469 6f6e  counts. Addition
+00004ff0: 616c 2077 6569 6768 7469 6e67 206d 6574  al weighting met
+00005000: 686f 6473 2063 616e 2062 6520 7265 6769  hods can be regi
+00005010: 7374 6572 6564 2062 7920 7573 6572 732e  stered by users.
+00005020: 2044 6566 6175 6c74 2069 7320 6022 696e   Default is `"in
+00005030: 6465 6c22 602e 0a20 2020 202a 2060 2269  del"`..    * `"i
+00005040: 6e64 656c 2260 203d 2060 2831 2c20 312c  ndel"` = `(1, 1,
+00005050: 2032 2960 0a20 2020 202a 2060 226c 6576   2)`.    * `"lev
+00005060: 2260 203d 2060 2831 2c20 312c 2031 2960  "` = `(1, 1, 1)`
+00005070: 0a2d 2060 7072 6564 6566 603a 2057 6865  .- `predef`: Whe
+00005080: 7468 6572 2072 6567 6578 2073 686f 756c  ther regex shoul
+00005090: 6420 6265 2069 6e74 6572 7072 6574 6564  d be interpreted
+000050a0: 2061 7320 6120 6b65 7920 746f 2061 2070   as a key to a p
+000050b0: 7265 6465 6669 6e65 6420 7265 6765 7820  redefined regex 
+000050c0: 7061 7474 6572 6e20 6f72 206e 6f74 2e20  pattern or not. 
+000050d0: 4361 6e20 6f6e 6c79 2062 6520 7365 7420  Can only be set 
+000050e0: 6174 2074 6865 2070 6174 7465 726e 206c  at the pattern l
+000050f0: 6576 656c 2e20 466f 7220 2246 5245 4745  evel. For "FREGE
+00005100: 5822 2070 6174 7465 726e 7320 6f6e 6c79  X" patterns only
+00005110: 2e20 4465 6661 756c 7420 6973 2060 4661  . Default is `Fa
+00005120: 6c73 6560 2e0a 0a0a 6060 6070 7974 686f  lse`....```pytho
+00005130: 6e0a 696d 706f 7274 2073 7061 6379 0a66  n.import spacy.f
+00005140: 726f 6d20 7370 6163 7a7a 2e6d 6174 6368  rom spaczz.match
+00005150: 6572 2069 6d70 6f72 7420 546f 6b65 6e4d  er import TokenM
+00005160: 6174 6368 6572 0a0a 2320 5573 696e 6720  atcher..# Using 
+00005170: 6d6f 6465 6c20 7265 7375 6c74 7320 6c69  model results li
+00005180: 6b65 2050 4f53 2074 6167 6769 6e67 2069  ke POS tagging i
+00005190: 6e20 746f 6b65 6e20 7061 7474 6572 6e73  n token patterns
+000051a0: 2072 6571 7569 7265 7320 6d6f 6465 6c20   requires model 
+000051b0: 7468 6174 2070 726f 7669 6465 7320 7468  that provides th
+000051c0: 6573 652e 0a6e 6c70 203d 2073 7061 6379  ese..nlp = spacy
+000051d0: 2e6c 6f61 6428 2265 6e5f 636f 7265 5f77  .load("en_core_w
+000051e0: 6562 5f6d 6422 290a 7465 7874 203d 2022  eb_md").text = "
+000051f0: 2222 5468 6520 6d61 6e61 6765 7220 6761  ""The manager ga
+00005200: 7665 206d 6520 5351 4c20 6461 7461 6265  ve me SQL databe
+00005210: 7345 2061 6365 7373 2073 6f20 6e6f 7720  sE acess so now 
+00005220: 4920 6361 6e20 6163 6365 7320 7468 6520  I can acces the 
+00005230: 5365 7175 616c 2044 422e 0a4d 7920 6d61  Sequal DB..My ma
+00005240: 6e61 6765 7227 7320 6e61 6d65 2069 7320  nager's name is 
+00005250: 4772 6669 656c 6422 2222 0a64 6f63 203d  Grfield""".doc =
+00005260: 206e 6c70 2874 6578 7429 0a0a 6d61 7463   nlp(text)..matc
+00005270: 6865 7220 3d20 546f 6b65 6e4d 6174 6368  her = TokenMatch
+00005280: 6572 2876 6f63 6162 3d6e 6c70 2e76 6f63  er(vocab=nlp.voc
+00005290: 6162 290a 6d61 7463 6865 722e 6164 6428  ab).matcher.add(
+000052a0: 0a20 2020 2022 4441 5441 222c 0a20 2020  .    "DATA",.   
+000052b0: 205b 0a20 2020 2020 2020 205b 0a20 2020   [.        [.   
+000052c0: 2020 2020 2020 2020 207b 2254 4558 5422           {"TEXT"
+000052d0: 3a20 2253 514c 227d 2c0a 2020 2020 2020  : "SQL"},.      
+000052e0: 2020 2020 2020 7b22 4c4f 5745 5222 3a20        {"LOWER": 
+000052f0: 7b22 4652 4547 4558 223a 2022 2864 6174  {"FREGEX": "(dat
+00005300: 6162 6173 6529 7b73 3c3d 317d 227d 7d2c  abase){s<=1}"}},
+00005310: 0a20 2020 2020 2020 2020 2020 207b 224c  .            {"L
+00005320: 4f57 4552 223a 207b 2246 555a 5a59 223a  OWER": {"FUZZY":
+00005330: 2022 6163 6365 7373 227d 7d2c 0a20 2020   "access"}},.   
+00005340: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00005350: 5b7b 2254 4558 5422 3a20 7b22 4655 5a5a  [{"TEXT": {"FUZZ
+00005360: 5922 3a20 2253 6571 7565 6c22 7d2c 2022  Y": "Sequel"}, "
+00005370: 504f 5322 3a20 2250 524f 504e 227d 2c20  POS": "PROPN"}, 
+00005380: 7b22 4c4f 5745 5222 3a20 2264 6222 7d5d  {"LOWER": "db"}]
+00005390: 2c0a 2020 2020 5d2c 0a29 0a6d 6174 6368  ,.    ],.).match
+000053a0: 6572 2e61 6464 2822 4e41 4d45 222c 205b  er.add("NAME", [
+000053b0: 5b7b 2254 4558 5422 3a20 7b22 4655 5a5a  [{"TEXT": {"FUZZ
+000053c0: 5922 3a20 2247 6172 6669 656c 6422 7d7d  Y": "Garfield"}}
+000053d0: 5d5d 290a 6d61 7463 6865 7320 3d20 6d61  ]]).matches = ma
+000053e0: 7463 6865 7228 646f 6329 0a0a 666f 7220  tcher(doc)..for 
+000053f0: 6d61 7463 685f 6964 2c20 7374 6172 742c  match_id, start,
+00005400: 2065 6e64 2c20 7261 7469 6f2c 2070 6174   end, ratio, pat
+00005410: 7465 726e 2069 6e20 6d61 7463 6865 733a  tern in matches:
+00005420: 0a20 2020 2070 7269 6e74 286d 6174 6368  .    print(match
+00005430: 5f69 642c 2064 6f63 5b73 7461 7274 3a65  _id, doc[start:e
+00005440: 6e64 5d2c 2072 6174 696f 2c20 7061 7474  nd], ratio, patt
+00005450: 6572 6e29 0a60 6060 0a0a 2020 2020 4441  ern).```..    DA
+00005460: 5441 2053 514c 2064 6174 6162 6573 4520  TA SQL databesE 
+00005470: 6163 6573 7320 3931 205b 7b22 5445 5854  acess 91 [{"TEXT
+00005480: 223a 2253 514c 227d 2c7b 224c 4f57 4552  ":"SQL"},{"LOWER
+00005490: 223a 7b22 4652 4547 4558 223a 2228 6461  ":{"FREGEX":"(da
+000054a0: 7461 6261 7365 297b 733c 3d31 7d22 7d7d  tabase){s<=1}"}}
+000054b0: 2c7b 224c 4f57 4552 223a 7b22 4655 5a5a  ,{"LOWER":{"FUZZ
+000054c0: 5922 3a22 6163 6365 7373 227d 7d5d 0a20  Y":"access"}}]. 
+000054d0: 2020 2044 4154 4120 5365 7175 616c 2044     DATA Sequal D
+000054e0: 4220 3837 205b 7b22 5445 5854 223a 7b22  B 87 [{"TEXT":{"
+000054f0: 4655 5a5a 5922 3a22 5365 7175 656c 227d  FUZZY":"Sequel"}
+00005500: 2c22 504f 5322 3a22 5052 4f50 4e22 7d2c  ,"POS":"PROPN"},
+00005510: 7b22 4c4f 5745 5222 3a22 6462 227d 5d0a  {"LOWER":"db"}].
+00005520: 2020 2020 4e41 4d45 2047 7266 6965 6c64      NAME Grfield
+00005530: 2039 3320 5b7b 2254 4558 5422 3a7b 2246   93 [{"TEXT":{"F
+00005540: 555a 5a59 223a 2247 6172 6669 656c 6422  UZZY":"Garfield"
+00005550: 7d7d 5d0a 0a0a 4576 656e 2074 686f 7567  }}]...Even thoug
+00005560: 6820 7468 6520 746f 6b65 6e20 6d61 7463  h the token matc
+00005570: 6865 7220 6361 6e20 6265 2061 2064 726f  her can be a dro
+00005580: 702d 696e 2072 6570 6c61 6365 6d65 6e74  p-in replacement
+00005590: 2066 6f72 2073 7061 4379 2773 2060 4d61   for spaCy's `Ma
+000055a0: 7463 6865 7260 2c20 6974 2069 7320 7374  tcher`, it is st
+000055b0: 696c 6c20 7265 636f 6d6d 656e 6465 6420  ill recommended 
+000055c0: 746f 2075 7365 2073 7061 4379 2773 2060  to use spaCy's `
+000055d0: 4d61 7463 6865 7260 2069 6620 796f 7520  Matcher` if you 
+000055e0: 646f 206e 6f74 206e 6565 6420 7468 6520  do not need the 
+000055f0: 7370 6163 7a7a 2074 6f6b 656e 206d 6174  spaczz token mat
+00005600: 6368 6572 2773 2066 757a 7a79 2063 6170  cher's fuzzy cap
+00005610: 6162 696c 6974 6965 7320 2d20 6974 2077  abilities - it w
+00005620: 696c 6c20 736c 6f77 2070 726f 6365 7373  ill slow process
+00005630: 696e 6720 646f 776e 2075 6e6e 6563 6573  ing down unneces
+00005640: 7361 7269 6c79 2e0a 0a2a 5265 6d69 6e64  sarily...*Remind
+00005650: 6572 3a20 7370 6143 7927 7320 604d 6174  er: spaCy's `Mat
+00005660: 6368 6572 6020 6e6f 7720 7375 7070 6f72  cher` now suppor
+00005670: 7473 205b 6675 7a7a 7920 6d61 7463 6869  ts [fuzzy matchi
+00005680: 6e67 5d28 6874 7470 733a 2f2f 7370 6163  ng](https://spac
+00005690: 792e 696f 2f75 7361 6765 2f76 332d 3523  y.io/usage/v3-5#
+000056a0: 6675 7a7a 7929 2c20 736f 2075 6e6c 6573  fuzzy), so unles
+000056b0: 7320 796f 7520 6e65 6564 2061 2073 7065  s you need a spe
+000056c0: 6369 6669 6320 6665 6174 7572 6520 6672  cific feature fr
+000056d0: 6f6d 2073 7061 637a 7a27 7320 6054 6f6b  om spaczz's `Tok
+000056e0: 656e 4d61 7463 6865 7260 2c20 6974 2069  enMatcher`, it i
+000056f0: 7320 6869 6768 6c79 2072 6563 6f6d 6d65  s highly recomme
+00005700: 6e64 6564 2074 6f20 7573 6520 7370 6143  nded to use spaC
+00005710: 7927 7320 6d75 6368 2066 6173 7465 7220  y's much faster 
+00005720: 604d 6174 6368 6572 602e 2a0a 0a23 2323  `Matcher`.*..###
+00005730: 2053 7061 637a 7a52 756c 6572 0a0a 5468   SpaczzRuler..Th
+00005740: 6520 7370 6163 7a7a 2072 756c 6572 2063  e spaczz ruler c
+00005750: 6f6d 6269 6e65 7320 7468 6520 6675 7a7a  ombines the fuzz
+00005760: 7920 616e 6420 7265 6765 7820 7068 7261  y and regex phra
+00005770: 7365 206d 6174 6368 6572 732c 2061 6e64  se matchers, and
+00005780: 2074 6865 2022 6675 7a7a 7922 2074 6f6b   the "fuzzy" tok
+00005790: 656e 206d 6174 6368 6572 2c20 696e 746f  en matcher, into
+000057a0: 206f 6e65 2070 6970 656c 696e 6520 636f   one pipeline co
+000057b0: 6d70 6f6e 656e 7420 7468 6174 2063 616e  mponent that can
+000057c0: 2075 7064 6174 6520 6120 6044 6f63 2e65   update a `Doc.e
+000057d0: 6e74 7360 2073 696d 696c 6172 2074 6f20  nts` similar to 
+000057e0: 7370 6143 7927 7320 6045 6e74 6974 7952  spaCy's `EntityR
+000057f0: 756c 6572 602e 0a0a 5061 7474 6572 6e73  uler`...Patterns
+00005800: 206d 7573 7420 6265 2061 6464 6564 2061   must be added a
+00005810: 7320 616e 2069 7465 7261 626c 6520 6f66  s an iterable of
+00005820: 2064 6963 7469 6f6e 6172 6965 7320 696e   dictionaries in
+00005830: 2074 6865 2066 6f72 6d61 7420 6f66 202a   the format of *
+00005840: 7b6c 6162 656c 2028 7374 7229 2c20 7061  {label (str), pa
+00005850: 7474 6572 6e28 7374 7220 6f72 206c 6973  ttern(str or lis
+00005860: 7429 2c20 7479 7065 2873 7472 292c 206f  t), type(str), o
+00005870: 7074 696f 6e61 6c20 6b77 6172 6773 2028  ptional kwargs (
+00005880: 6469 6374 292c 2061 6e64 206f 7074 696f  dict), and optio
+00005890: 6e61 6c20 6964 2028 7374 7229 7d2a 2e0a  nal id (str)}*..
+000058a0: 0a46 6f72 2065 7861 6d70 6c65 2c20 6120  .For example, a 
+000058b0: 6675 7a7a 7920 7068 7261 7365 2070 6174  fuzzy phrase pat
+000058c0: 7465 726e 3a0a 0a60 7b27 6c61 6265 6c27  tern:..`{'label'
+000058d0: 3a20 274f 5247 272c 2027 7061 7474 6572  : 'ORG', 'patter
+000058e0: 6e27 3a20 2741 7070 6c65 2720 276b 7761  n': 'Apple' 'kwa
+000058f0: 7267 7327 3a20 7b27 6d69 6e5f 7232 273a  rgs': {'min_r2':
+00005900: 2039 307d 2c20 2774 7970 6527 3a20 2766   90}, 'type': 'f
+00005910: 757a 7a79 277d 600a 0a4f 722c 2061 2074  uzzy'}`..Or, a t
+00005920: 6f6b 656e 2070 6174 7465 726e 3a0a 0a60  oken pattern:..`
+00005930: 7b27 6c61 6265 6c27 3a20 274f 5247 272c  {'label': 'ORG',
+00005940: 2027 7061 7474 6572 6e27 3a20 5b7b 2754   'pattern': [{'T
+00005950: 4558 5427 3a20 7b27 4655 5a5a 5927 3a20  EXT': {'FUZZY': 
+00005960: 2741 7070 6c65 277d 7d5d 2c20 2774 7970  'Apple'}}], 'typ
+00005970: 6527 3a20 2774 6f6b 656e 277d 600a 0a0a  e': 'token'}`...
+00005980: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00005990: 2073 7061 6379 0a66 726f 6d20 7370 6163   spacy.from spac
+000059a0: 7a7a 2e70 6970 656c 696e 6520 696d 706f  zz.pipeline impo
+000059b0: 7274 2053 7061 637a 7a52 756c 6572 0a0a  rt SpaczzRuler..
+000059c0: 6e6c 7020 3d20 7370 6163 792e 626c 616e  nlp = spacy.blan
+000059d0: 6b28 2265 6e22 290a 7465 7874 203d 2022  k("en").text = "
+000059e0: 2222 416e 6465 7273 6f6e 2c20 4772 696e  ""Anderson, Grin
+000059f0: 7420 6372 6561 7465 6420 7370 6163 7a7a  t created spaczz
+00005a00: 2069 6e20 6869 7320 686f 6d65 2061 7420   in his home at 
+00005a10: 3535 3520 4661 6b65 2053 742c 0a41 7074  555 Fake St,.Apt
+00005a20: 2035 2069 6e20 4e61 7368 7631 6c65 2c20   5 in Nashv1le, 
+00005a30: 544e 2035 3535 3535 2d31 3233 3420 696e  TN 55555-1234 in
+00005a40: 2074 6865 2055 5341 2e0a 536f 6d65 206f   the USA..Some o
+00005a50: 6620 6869 7320 6661 766f 7269 7465 2062  f his favorite b
+00005a60: 616e 6473 2061 7265 2043 6f6e 7665 7267  ands are Converg
+00005a70: 2061 6e64 2050 726f 7465 7420 7468 6520   and Protet the 
+00005a80: 5a65 726f 2e22 2222 2020 2320 5370 656c  Zero."""  # Spel
+00005a90: 6c69 6e67 2065 7272 6f72 7320 696e 7465  ling errors inte
+00005aa0: 6e74 696f 6e61 6c2e 0a64 6f63 203d 206e  ntional..doc = n
+00005ab0: 6c70 2874 6578 7429 0a0a 7061 7474 6572  lp(text)..patter
+00005ac0: 6e73 203d 205b 0a20 2020 207b 0a20 2020  ns = [.    {.   
+00005ad0: 2020 2020 2022 6c61 6265 6c22 3a20 224e       "label": "N
+00005ae0: 414d 4522 2c0a 2020 2020 2020 2020 2270  AME",.        "p
+00005af0: 6174 7465 726e 223a 2022 4772 616e 7420  attern": "Grant 
+00005b00: 416e 6465 7273 656e 222c 0a20 2020 2020  Andersen",.     
+00005b10: 2020 2022 7479 7065 223a 2022 6675 7a7a     "type": "fuzz
+00005b20: 7922 2c0a 2020 2020 2020 2020 226b 7761  y",.        "kwa
+00005b30: 7267 7322 3a20 7b22 6675 7a7a 795f 6675  rgs": {"fuzzy_fu
+00005b40: 6e63 223a 2022 746f 6b65 6e5f 736f 7274  nc": "token_sort
+00005b50: 227d 2c0a 2020 2020 7d2c 0a20 2020 207b  "},.    },.    {
+00005b60: 0a20 2020 2020 2020 2022 6c61 6265 6c22  .        "label"
+00005b70: 3a20 2253 5452 4545 5422 2c0a 2020 2020  : "STREET",.    
+00005b80: 2020 2020 2270 6174 7465 726e 223a 2022      "pattern": "
+00005b90: 7374 7265 6574 5f61 6464 7265 7373 6573  street_addresses
+00005ba0: 222c 0a20 2020 2020 2020 2022 7479 7065  ",.        "type
+00005bb0: 223a 2022 7265 6765 7822 2c0a 2020 2020  ": "regex",.    
+00005bc0: 2020 2020 226b 7761 7267 7322 3a20 7b22      "kwargs": {"
+00005bd0: 7072 6564 6566 223a 2054 7275 657d 2c0a  predef": True},.
+00005be0: 2020 2020 7d2c 0a20 2020 207b 226c 6162      },.    {"lab
+00005bf0: 656c 223a 2022 4750 4522 2c20 2270 6174  el": "GPE", "pat
+00005c00: 7465 726e 223a 2022 4e61 7368 7669 6c6c  tern": "Nashvill
+00005c10: 6522 2c20 2274 7970 6522 3a20 2266 757a  e", "type": "fuz
+00005c20: 7a79 227d 2c0a 2020 2020 7b0a 2020 2020  zy"},.    {.    
+00005c30: 2020 2020 226c 6162 656c 223a 2022 5a49      "label": "ZI
+00005c40: 5022 2c0a 2020 2020 2020 2020 2270 6174  P",.        "pat
+00005c50: 7465 726e 223a 2072 225c 6228 3f3a 3535  tern": r"\b(?:55
+00005c60: 3535 3429 7b73 3c3d 317d 283f 3a28 3f3a  554){s<=1}(?:(?:
+00005c70: 5b2d 5c73 5d29 3f5c 647b 347d 5c62 2922  [-\s])?\d{4}\b)"
+00005c80: 2c0a 2020 2020 2020 2020 2274 7970 6522  ,.        "type"
+00005c90: 3a20 2272 6567 6578 222c 0a20 2020 207d  : "regex",.    }
+00005ca0: 2c20 2023 2066 757a 7a79 2072 6567 6578  ,  # fuzzy regex
+00005cb0: 0a20 2020 207b 226c 6162 656c 223a 2022  .    {"label": "
+00005cc0: 4750 4522 2c20 2270 6174 7465 726e 223a  GPE", "pattern":
+00005cd0: 2022 283f 6929 5b55 5d28 6e69 7465 647c   "(?i)[U](nited|
+00005ce0: 5c2e 3f29 203f 5b53 5d28 7461 7465 737c  \.?) ?[S](tates|
+00005cf0: 5c2e 3f29 222c 2022 7479 7065 223a 2022  \.?)", "type": "
+00005d00: 7265 6765 7822 7d2c 0a20 2020 207b 0a20  regex"},.    {. 
+00005d10: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00005d20: 2242 414e 4422 2c0a 2020 2020 2020 2020  "BAND",.        
+00005d30: 2270 6174 7465 726e 223a 205b 7b22 4c4f  "pattern": [{"LO
+00005d40: 5745 5222 3a20 7b22 4652 4547 4558 223a  WER": {"FREGEX":
+00005d50: 2022 2863 6f6e 7665 7267 6529 7b65 3c3d   "(converge){e<=
+00005d60: 317d 227d 7d5d 2c0a 2020 2020 2020 2020  1}"}}],.        
+00005d70: 2274 7970 6522 3a20 2274 6f6b 656e 222c  "type": "token",
+00005d80: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00005d90: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00005da0: 4241 4e44 222c 0a20 2020 2020 2020 2022  BAND",.        "
+00005db0: 7061 7474 6572 6e22 3a20 5b0a 2020 2020  pattern": [.    
+00005dc0: 2020 2020 2020 2020 7b22 5445 5854 223a          {"TEXT":
+00005dd0: 207b 2246 555a 5a59 223a 2022 5072 6f74   {"FUZZY": "Prot
+00005de0: 6573 7422 7d7d 2c0a 2020 2020 2020 2020  est"}},.        
+00005df0: 2020 2020 7b22 4953 5f53 544f 5022 3a20      {"IS_STOP": 
+00005e00: 5472 7565 7d2c 0a20 2020 2020 2020 2020  True},.         
+00005e10: 2020 207b 2254 4558 5422 3a20 7b22 4655     {"TEXT": {"FU
+00005e20: 5a5a 5922 3a20 2248 6572 6f22 7d7d 2c0a  ZZY": "Hero"}},.
+00005e30: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00005e40: 2020 2022 7479 7065 223a 2022 746f 6b65     "type": "toke
+00005e50: 6e22 2c0a 2020 2020 7d2c 0a5d 0a0a 7275  n",.    },.]..ru
+00005e60: 6c65 7220 3d20 5370 6163 7a7a 5275 6c65  ler = SpaczzRule
+00005e70: 7228 6e6c 7029 0a72 756c 6572 2e61 6464  r(nlp).ruler.add
+00005e80: 5f70 6174 7465 726e 7328 7061 7474 6572  _patterns(patter
+00005e90: 6e73 290a 646f 6320 3d20 7275 6c65 7228  ns).doc = ruler(
+00005ea0: 646f 6329 0a0a 0a66 6f72 2065 6e74 2069  doc)...for ent i
+00005eb0: 6e20 646f 632e 656e 7473 3a0a 2020 2020  n doc.ents:.    
+00005ec0: 7072 696e 7428 0a20 2020 2020 2020 2028  print(.        (
+00005ed0: 0a20 2020 2020 2020 2020 2020 2065 6e74  .            ent
+00005ee0: 2e74 6578 742c 0a20 2020 2020 2020 2020  .text,.         
+00005ef0: 2020 2065 6e74 2e73 7461 7274 2c0a 2020     ent.start,.  
+00005f00: 2020 2020 2020 2020 2020 656e 742e 656e            ent.en
+00005f10: 642c 0a20 2020 2020 2020 2020 2020 2065  d,.            e
+00005f20: 6e74 2e6c 6162 656c 5f2c 0a20 2020 2020  nt.label_,.     
+00005f30: 2020 2020 2020 2065 6e74 2e5f 2e73 7061         ent._.spa
+00005f40: 637a 7a5f 7261 7469 6f2c 0a20 2020 2020  czz_ratio,.     
+00005f50: 2020 2020 2020 2065 6e74 2e5f 2e73 7061         ent._.spa
+00005f60: 637a 7a5f 7479 7065 2c0a 2020 2020 2020  czz_type,.      
+00005f70: 2020 2020 2020 656e 742e 5f2e 7370 6163        ent._.spac
+00005f80: 7a7a 5f70 6174 7465 726e 2c0a 2020 2020  zz_pattern,.    
+00005f90: 2020 2020 290a 2020 2020 290a 6060 600a      ).    ).```.
+00005fa0: 0a20 2020 2028 2741 6e64 6572 736f 6e2c  .    ('Anderson,
+00005fb0: 2047 7269 6e74 272c 2030 2c20 332c 2027   Grint', 0, 3, '
+00005fc0: 4e41 4d45 272c 2038 332c 2027 6675 7a7a  NAME', 83, 'fuzz
+00005fd0: 7927 2c20 2747 7261 6e74 2041 6e64 6572  y', 'Grant Ander
+00005fe0: 7365 6e27 290a 2020 2020 2827 3535 3520  sen').    ('555 
+00005ff0: 4661 6b65 2053 742c 272c 2039 2c20 3133  Fake St,', 9, 13
+00006000: 2c20 2753 5452 4545 5427 2c20 3130 302c  , 'STREET', 100,
+00006010: 2027 7265 6765 7827 2c20 2773 7472 6565   'regex', 'stree
+00006020: 745f 6164 6472 6573 7365 7327 290a 2020  t_addresses').  
+00006030: 2020 2827 4e61 7368 7631 6c65 272c 2031    ('Nashv1le', 1
+00006040: 372c 2031 382c 2027 4750 4527 2c20 3832  7, 18, 'GPE', 82
+00006050: 2c20 2766 757a 7a79 272c 2027 4e61 7368  , 'fuzzy', 'Nash
+00006060: 7669 6c6c 6527 290a 2020 2020 2827 3535  ville').    ('55
+00006070: 3535 352d 3132 3334 272c 2032 302c 2032  555-1234', 20, 2
+00006080: 332c 2027 5a49 5027 2c20 3930 2c20 2772  3, 'ZIP', 90, 'r
+00006090: 6567 6578 272c 2027 5c5c 6228 3f3a 3535  egex', '\\b(?:55
+000060a0: 3535 3429 7b73 3c3d 317d 283f 3a28 3f3a  554){s<=1}(?:(?:
+000060b0: 5b2d 5c5c 735d 293f 5c5c 647b 347d 5c5c  [-\\s])?\\d{4}\\
+000060c0: 6229 2729 0a20 2020 2028 2755 5341 272c  b)').    ('USA',
+000060d0: 2032 352c 2032 362c 2027 4750 4527 2c20   25, 26, 'GPE', 
+000060e0: 3130 302c 2027 7265 6765 7827 2c20 2728  100, 'regex', '(
+000060f0: 3f69 295b 555d 286e 6974 6564 7c5c 5c2e  ?i)[U](nited|\\.
+00006100: 3f29 203f 5b53 5d28 7461 7465 737c 5c5c  ?) ?[S](tates|\\
+00006110: 2e3f 2927 290a 2020 2020 2827 436f 6e76  .?)').    ('Conv
+00006120: 6572 6727 2c20 3334 2c20 3335 2c20 2742  erg', 34, 35, 'B
+00006130: 414e 4427 2c20 3933 2c20 2774 6f6b 656e  AND', 93, 'token
+00006140: 272c 2027 5b7b 224c 4f57 4552 223a 7b22  ', '[{"LOWER":{"
+00006150: 4652 4547 4558 223a 2228 636f 6e76 6572  FREGEX":"(conver
+00006160: 6765 297b 653c 3d31 7d22 7d7d 5d27 290a  ge){e<=1}"}}]').
+00006170: 2020 2020 2827 5072 6f74 6574 2074 6865      ('Protet the
+00006180: 205a 6572 6f27 2c20 3336 2c20 3339 2c20   Zero', 36, 39, 
+00006190: 2742 414e 4427 2c20 3839 2c20 2774 6f6b  'BAND', 89, 'tok
+000061a0: 656e 272c 2027 5b7b 2254 4558 5422 3a7b  en', '[{"TEXT":{
+000061b0: 2246 555a 5a59 223a 2250 726f 7465 7374  "FUZZY":"Protest
+000061c0: 227d 7d2c 7b22 4953 5f53 544f 5022 3a74  "}},{"IS_STOP":t
+000061d0: 7275 657d 2c7b 2254 4558 5422 3a7b 2246  rue},{"TEXT":{"F
+000061e0: 555a 5a59 223a 2248 6572 6f22 7d7d 5d27  UZZY":"Hero"}}]'
+000061f0: 290a 0a0a 5765 2073 6565 2069 6e20 7468  )...We see in th
+00006200: 6520 6578 616d 706c 6520 6162 6f76 6520  e example above 
+00006210: 7468 6174 2077 6520 6172 6520 7265 6665  that we are refe
+00006220: 7265 6e63 696e 6720 736f 6d65 2063 7573  rencing some cus
+00006230: 746f 6d20 6174 7472 6962 7574 6573 2c20  tom attributes, 
+00006240: 7768 6963 6820 6172 6520 6578 706c 6169  which are explai
+00006250: 6e65 6420 6265 6c6f 772e 0a0a 466f 7220  ned below...For 
+00006260: 6d6f 7265 2060 5370 6163 7a7a 5275 6c65  more `SpaczzRule
+00006270: 7260 2065 7861 6d70 6c65 7320 7365 6520  r` examples see 
+00006280: 5b68 6572 655d 2868 7474 7073 3a2f 2f67  [here](https://g
+00006290: 6974 6875 622e 636f 6d2f 6761 6e64 6572  ithub.com/gander
+000062a0: 7365 6e31 3031 2f73 7061 637a 7a2f 626c  sen101/spaczz/bl
+000062b0: 6f62 2f6d 6173 7465 722f 6578 616d 706c  ob/master/exampl
+000062c0: 6573 2f66 757a 7a79 5f6d 6174 6368 696e  es/fuzzy_matchin
+000062d0: 675f 7477 6561 6b73 2e69 7079 6e62 292e  g_tweaks.ipynb).
+000062e0: 2049 6e20 7061 7274 6963 756c 6172 2074   In particular t
+000062f0: 6869 7320 7072 6f76 6964 6573 2064 6574  his provides det
+00006300: 6169 6c73 2061 626f 7574 2074 6865 2072  ails about the r
+00006310: 756c 6572 2773 2073 6f72 7469 6e67 2070  uler's sorting p
+00006320: 726f 6365 7373 2061 6e64 2066 757a 7a79  rocess and fuzzy
+00006330: 206d 6174 6368 696e 6720 7061 7261 6d65   matching parame
+00006340: 7465 7273 2e0a 0a23 2323 2043 7573 746f  ters...### Custo
+00006350: 6d20 4174 7472 6962 7574 6573 0a0a 5370  m Attributes..Sp
+00006360: 6163 7a7a 2069 6e69 7469 616c 697a 6573  aczz initializes
+00006370: 2073 6f6d 6520 6375 7374 6f6d 2061 7474   some custom att
+00006380: 7269 6275 7465 7320 7570 6f6e 2069 6d70  ributes upon imp
+00006390: 6f72 7469 6e67 2e20 5468 6573 6520 6172  orting. These ar
+000063a0: 6520 756e 6465 7220 7370 6143 7927 7320  e under spaCy's 
+000063b0: 602e 5f2e 6020 6174 7472 6962 7574 6520  `._.` attribute 
+000063c0: 616e 6420 6172 6520 6675 7274 6865 7220  and are further 
+000063d0: 7072 6570 656e 6465 6420 7769 7468 2060  prepended with `
+000063e0: 7370 6163 7a7a 5f60 2073 6f20 7468 6572  spaczz_` so ther
+000063f0: 6520 7368 6f75 6c64 2062 6520 6e6f 7420  e should be not 
+00006400: 636f 6e66 6c69 6374 7320 7769 7468 2079  conflicts with y
+00006410: 6f75 7220 6f77 6e20 6375 7374 6f6d 2061  our own custom a
+00006420: 7474 7269 6275 7465 732e 2049 6620 7468  ttributes. If th
+00006430: 6572 6520 6172 6520 7370 6163 7a7a 2077  ere are spaczz w
+00006440: 696c 6c20 666f 7263 6520 6f76 6572 7772  ill force overwr
+00006450: 6974 6520 7468 656d 2e0a 0a54 6865 7365  ite them...These
+00006460: 2063 7573 746f 6d20 6174 7472 6962 7574   custom attribut
+00006470: 6573 2061 7265 206f 6e6c 7920 7365 7420  es are only set 
+00006480: 7669 6120 7468 6520 7370 6163 7a7a 2072  via the spaczz r
+00006490: 756c 6572 2061 7420 7468 6520 746f 6b65  uler at the toke
+000064a0: 6e20 6c65 7665 6c2e 2053 7061 6e20 616e  n level. Span an
+000064b0: 6420 646f 6320 7665 7273 696f 6e73 206f  d doc versions o
+000064c0: 6620 7468 6573 6520 6174 7472 6962 7574  f these attribut
+000064d0: 6573 2061 7265 2067 6574 7465 7273 2074  es are getters t
+000064e0: 6861 7420 7265 6665 7265 6e63 6520 7468  hat reference th
+000064f0: 6520 746f 6b65 6e20 6c65 7665 6c20 6174  e token level at
+00006500: 7472 6962 7574 6573 2e0a 0a54 6865 2066  tributes...The f
+00006510: 6f6c 6c6f 7769 6e67 2060 546f 6b65 6e60  ollowing `Token`
+00006520: 2061 7474 7269 6275 7465 7320 6172 6520   attributes are 
+00006530: 6176 6169 6c61 626c 652e 2041 6c6c 2061  available. All a
+00006540: 7265 206d 7574 6162 6c65 3a0a 0a2d 2060  re mutable:..- `
+00006550: 7370 6163 7a7a 5f74 6f6b 656e 603a 2064  spaczz_token`: d
+00006560: 6566 6175 6c74 203d 2060 4661 6c73 6560  efault = `False`
+00006570: 2e20 426f 6f6c 6561 6e20 7468 6174 2064  . Boolean that d
+00006580: 656e 6f74 6573 2069 6620 7468 6520 746f  enotes if the to
+00006590: 6b65 6e20 6973 2070 6172 7420 6f66 2061  ken is part of a
+000065a0: 6e20 656e 7469 7479 2073 6574 2062 7920  n entity set by 
+000065b0: 7468 6520 7370 6163 7a7a 2072 756c 6572  the spaczz ruler
+000065c0: 2e0a 2d20 6073 7061 637a 7a5f 7479 7065  ..- `spaczz_type
+000065d0: 603a 2064 6566 6175 6c74 203d 2060 4e6f  `: default = `No
+000065e0: 6e65 602e 2053 7472 696e 6720 7468 6174  ne`. String that
+000065f0: 2073 686f 7773 2077 6869 6368 206d 6174   shows which mat
+00006600: 6368 6572 2070 726f 6475 6365 6420 616e  cher produced an
+00006610: 2065 6e74 6974 7920 7573 696e 6720 7468   entity using th
+00006620: 6520 746f 6b65 6e2e 0a2d 2060 7370 6163  e token..- `spac
+00006630: 7a7a 5f72 6174 696f 603a 2064 6566 6175  zz_ratio`: defau
+00006640: 6c74 203d 2060 4e6f 6e65 602e 2049 6620  lt = `None`. If 
+00006650: 7468 6520 746f 6b65 6e20 6973 2070 6172  the token is par
+00006660: 7420 6f66 2061 206d 6174 6368 6564 2065  t of a matched e
+00006670: 6e74 6974 792c 2069 7420 7769 6c6c 2072  ntity, it will r
+00006680: 6574 7572 6e20 6675 7a7a 7920 7261 7469  eturn fuzzy rati
+00006690: 6f2e 0a2d 2060 7370 6163 7a7a 5f70 6174  o..- `spaczz_pat
+000066a0: 7465 726e 603a 2064 6566 6175 6c74 203d  tern`: default =
+000066b0: 2060 4e6f 6e65 602e 2049 6620 7468 6520   `None`. If the 
+000066c0: 746f 6b65 6e20 6973 2070 6172 7420 6f66  token is part of
+000066d0: 2061 206d 6174 6368 6564 2065 6e74 6974   a matched entit
+000066e0: 792c 2069 7420 7769 6c6c 2072 6574 7572  y, it will retur
+000066f0: 6e20 7468 6520 7061 7474 6572 6e20 6173  n the pattern as
+00006700: 2061 2073 7472 696e 6720 284a 534f 4e2d   a string (JSON-
+00006710: 666f 726d 6174 7465 6420 666f 7220 746f  formatted for to
+00006720: 6b65 6e20 7061 7474 6572 6e73 2920 7468  ken patterns) th
+00006730: 6174 2070 726f 6475 6365 6420 7468 6520  at produced the 
+00006740: 6d61 7463 682e 0a0a 5468 6520 666f 6c6c  match...The foll
+00006750: 6f77 696e 6720 6053 7061 6e60 2061 7474  owing `Span` att
+00006760: 7269 6275 7465 7320 7265 6665 7265 6e63  ributes referenc
+00006770: 6520 7468 6520 746f 6b65 6e20 6174 7472  e the token attr
+00006780: 6962 7574 6573 2069 6e63 6c75 6465 6420  ibutes included 
+00006790: 696e 2074 6865 2073 7061 6e2e 2041 6c6c  in the span. All
+000067a0: 2061 7265 2069 6d6d 7574 6162 6c65 3a0a   are immutable:.
+000067b0: 0a2d 2060 7370 6163 7a7a 5f65 6e74 603a  .- `spaczz_ent`:
+000067c0: 2064 6566 6175 6c74 203d 2060 4661 6c73   default = `Fals
+000067d0: 6560 2e20 426f 6f6c 6561 6e20 7468 6174  e`. Boolean that
+000067e0: 2064 656e 6f74 6573 2069 6620 616c 6c20   denotes if all 
+000067f0: 746f 6b65 6e73 2069 6e20 7468 6520 7370  tokens in the sp
+00006800: 616e 2061 7265 2070 6172 7420 6f66 2061  an are part of a
+00006810: 6e20 656e 7469 7479 2073 6574 2062 7920  n entity set by 
+00006820: 7468 6520 7370 6163 7a7a 2072 756c 6572  the spaczz ruler
+00006830: 2e0a 2d20 6073 7061 637a 7a5f 7479 7065  ..- `spaczz_type
+00006840: 603a 2064 6566 6175 6c74 203d 2060 4e6f  `: default = `No
+00006850: 6e65 602e 2053 7472 696e 6720 7468 6174  ne`. String that
+00006860: 2064 656e 6f74 6573 2077 6869 6368 206d   denotes which m
+00006870: 6174 6368 6572 2070 726f 6475 6365 6420  atcher produced 
+00006880: 616e 2065 6e74 6974 7920 7573 696e 6720  an entity using 
+00006890: 7468 6520 696e 636c 7564 6564 2074 6f6b  the included tok
+000068a0: 656e 732e 0a2d 2060 7370 6163 7a7a 5f74  ens..- `spaczz_t
+000068b0: 7970 6573 603a 2064 6566 6175 6c74 203d  ypes`: default =
+000068c0: 2060 7365 7428 2960 2e20 5365 7420 7468   `set()`. Set th
+000068d0: 6174 2073 686f 7773 2077 6869 6368 206d  at shows which m
+000068e0: 6174 6368 6572 7320 7072 6f64 7563 6564  atchers produced
+000068f0: 2065 6e74 6974 6965 7320 7573 696e 6720   entities using 
+00006900: 7468 6520 696e 636c 7564 6564 2074 6f6b  the included tok
+00006910: 656e 732e 2041 6e20 656e 7469 7479 2073  ens. An entity s
+00006920: 7061 6e20 7368 6f75 6c64 206f 6e6c 7920  pan should only 
+00006930: 6861 7665 206f 6e65 2074 7970 652c 2062  have one type, b
+00006940: 7574 2074 6869 7320 616c 6c6f 7773 2079  ut this allows y
+00006950: 6f75 2074 6f20 7365 6520 7468 6520 7479  ou to see the ty
+00006960: 7065 7320 696e 636c 7564 6564 2069 6e20  pes included in 
+00006970: 616e 7920 6172 6269 7472 6172 7920 7370  any arbitrary sp
+00006980: 616e 2e0a 2d20 6073 7061 637a 7a5f 7261  an..- `spaczz_ra
+00006990: 7469 6f60 3a20 6465 6661 756c 7420 3d20  tio`: default = 
+000069a0: 604e 6f6e 6560 2e20 4966 2061 6c6c 2074  `None`. If all t
+000069b0: 6865 2074 6f6b 656e 7320 696e 2073 7061  he tokens in spa
+000069c0: 6e20 6172 6520 7061 7274 206f 6620 6120  n are part of a 
+000069d0: 6d61 7463 6865 6420 656e 7469 7479 2c20  matched entity, 
+000069e0: 6974 2077 696c 6c20 7265 7475 726e 2074  it will return t
+000069f0: 6865 2066 757a 7a79 2072 6174 696f 2e0a  he fuzzy ratio..
+00006a00: 2d20 6073 7061 637a 7a5f 7061 7474 6572  - `spaczz_patter
+00006a10: 6e60 3a20 6465 6661 756c 7420 3d20 604e  n`: default = `N
+00006a20: 6f6e 6560 2e20 4966 2061 6c6c 2074 6865  one`. If all the
+00006a30: 2074 6f6b 656e 7320 696e 2061 2073 7061   tokens in a spa
+00006a40: 6e20 6172 6520 7061 7274 206f 6620 6120  n are part of a 
+00006a50: 6d61 7463 6865 6420 656e 7469 7479 2c20  matched entity, 
+00006a60: 6974 2077 696c 6c20 7265 7475 726e 2074  it will return t
+00006a70: 6865 2070 6174 7465 726e 2061 7320 6120  he pattern as a 
+00006a80: 7374 7269 6e67 2028 4a53 4f4e 2d66 6f72  string (JSON-for
+00006a90: 6d61 7474 6564 2066 6f72 2074 6f6b 656e  matted for token
+00006aa0: 2070 6174 7465 726e 7329 2074 6861 7420   patterns) that 
+00006ab0: 7072 6f64 7563 6564 2074 6865 206d 6174  produced the mat
+00006ac0: 6368 2e0a 0a54 6865 2066 6f6c 6c6f 7769  ch...The followi
+00006ad0: 6e67 2060 446f 6360 2061 7474 7269 6275  ng `Doc` attribu
+00006ae0: 7465 7320 7265 6665 7265 6e63 6520 7468  tes reference th
+00006af0: 6520 746f 6b65 6e20 6174 7472 6962 7574  e token attribut
+00006b00: 6573 2069 6e63 6c75 6465 6420 696e 2074  es included in t
+00006b10: 6865 2064 6f63 2e20 416c 6c20 6172 6520  he doc. All are 
+00006b20: 696d 6d75 7461 626c 653a 0a0a 2d20 6073  immutable:..- `s
+00006b30: 7061 637a 7a5f 646f 6360 3a20 6465 6661  paczz_doc`: defa
+00006b40: 756c 7420 3d20 6046 616c 7365 602e 2042  ult = `False`. B
+00006b50: 6f6f 6c65 616e 2074 6861 7420 6465 6e6f  oolean that deno
+00006b60: 7465 7320 6966 2061 6e79 2074 6f6b 656e  tes if any token
+00006b70: 7320 696e 2074 6865 2064 6f63 2061 7265  s in the doc are
+00006b80: 2070 6172 7420 6f66 2061 6e20 656e 7469   part of an enti
+00006b90: 7479 2073 6574 2062 7920 7468 6520 7370  ty set by the sp
+00006ba0: 6163 7a7a 2072 756c 6572 2e0a 2d20 6073  aczz ruler..- `s
+00006bb0: 7061 637a 7a5f 7479 7065 7360 3a20 6465  paczz_types`: de
+00006bc0: 6661 756c 7420 3d20 6073 6574 2829 602e  fault = `set()`.
+00006bd0: 2053 6574 2074 6861 7420 7368 6f77 7320   Set that shows 
+00006be0: 7768 6963 6820 6d61 7463 6865 7273 2070  which matchers p
+00006bf0: 726f 6475 6365 6420 656e 7469 7469 6573  roduced entities
+00006c00: 2069 6e20 7468 6520 646f 632e 0a0a 2323   in the doc...##
+00006c10: 2320 5361 7669 6e67 2f4c 6f61 6469 6e67  # Saving/Loading
+00006c20: 0a0a 5468 6520 6053 7061 637a 7a52 756c  ..The `SpaczzRul
+00006c30: 6572 6020 6861 7320 6974 2773 206f 776e  er` has it's own
+00006c40: 2074 6f2f 6672 6f6d 2064 6973 6b2f 6279   to/from disk/by
+00006c50: 7465 7320 6d65 7468 6f64 7320 616e 6420  tes methods and 
+00006c60: 7769 6c6c 2061 6363 6570 7420 6063 6f6e  will accept `con
+00006c70: 6669 6760 2070 6172 616d 6574 6572 7320  fig` parameters 
+00006c80: 7061 7373 6564 2074 6f20 6073 7061 6379  passed to `spacy
+00006c90: 2e6c 6f61 6428 2960 2e20 4974 2061 6c73  .load()`. It als
+00006ca0: 6f20 6861 7320 6974 2773 206f 776e 2073  o has it's own s
+00006cb0: 7061 4379 2066 6163 746f 7279 2065 6e74  paCy factory ent
+00006cc0: 7279 2070 6f69 6e74 2073 6f20 7370 6143  ry point so spaC
+00006cd0: 7920 6973 2061 7761 7265 206f 6620 7468  y is aware of th
+00006ce0: 6520 6053 7061 637a 7a52 756c 6572 602e  e `SpaczzRuler`.
+00006cf0: 2042 656c 6f77 2069 7320 616e 2065 7861   Below is an exa
+00006d00: 6d70 6c65 206f 6620 7361 7669 6e67 2061  mple of saving a
+00006d10: 6e64 206c 6f61 6469 6e67 2061 2073 7061  nd loading a spa
+00006d20: 6379 2070 6970 656c 696e 6520 7769 7468  cy pipeline with
+00006d30: 2074 6865 2073 6d61 6c6c 2045 6e67 6c69   the small Engli
+00006d40: 7368 206d 6f64 656c 2c20 7468 6520 6045  sh model, the `E
+00006d50: 6e74 6974 7952 756c 6572 602c 2061 6e64  ntityRuler`, and
+00006d60: 2074 6865 2060 5370 6163 7a7a 5275 6c65   the `SpaczzRule
+00006d70: 7260 2e0a 0a0a 6060 6070 7974 686f 6e0a  r`....```python.
+00006d80: 696d 706f 7274 2073 7061 6379 0a66 726f  import spacy.fro
+00006d90: 6d20 7370 6163 7a7a 2e70 6970 656c 696e  m spaczz.pipelin
+00006da0: 6520 696d 706f 7274 2053 7061 637a 7a52  e import SpaczzR
+00006db0: 756c 6572 0a0a 6e6c 7020 3d20 7370 6163  uler..nlp = spac
+00006dc0: 792e 6c6f 6164 2822 656e 5f63 6f72 655f  y.load("en_core_
+00006dd0: 7765 625f 6d64 2229 0a74 6578 7420 3d20  web_md").text = 
+00006de0: 2222 2241 6e64 6572 736f 6e2c 2047 7269  """Anderson, Gri
+00006df0: 6e74 2063 7265 6174 6564 2073 7061 637a  nt created spacz
+00006e00: 7a20 696e 2068 6973 2068 6f6d 6520 6174  z in his home at
+00006e10: 2035 3535 2046 616b 6520 5374 2c0a 4170   555 Fake St,.Ap
+00006e20: 7420 3520 696e 204e 6173 6876 316c 652c  t 5 in Nashv1le,
+00006e30: 2054 4e20 3535 3535 352d 3132 3334 2069   TN 55555-1234 i
+00006e40: 6e20 7468 6520 5553 412e 0a53 6f6d 6520  n the USA..Some 
+00006e50: 6f66 2068 6973 2066 6176 6f72 6974 6520  of his favorite 
+00006e60: 6261 6e64 7320 6172 6520 436f 6e76 6572  bands are Conver
+00006e70: 6720 616e 6420 5072 6f74 6574 2074 6865  g and Protet the
+00006e80: 205a 6572 6f2e 2222 2220 2023 2053 7065   Zero."""  # Spe
+00006e90: 6c6c 696e 6720 6572 726f 7273 2069 6e74  lling errors int
+00006ea0: 656e 7469 6f6e 616c 2e0a 646f 6320 3d20  entional..doc = 
+00006eb0: 6e6c 7028 7465 7874 290a 0a66 6f72 2065  nlp(text)..for e
+00006ec0: 6e74 2069 6e20 646f 632e 656e 7473 3a0a  nt in doc.ents:.
+00006ed0: 2020 2020 7072 696e 7428 2865 6e74 2e74      print((ent.t
+00006ee0: 6578 742c 2065 6e74 2e73 7461 7274 2c20  ext, ent.start, 
+00006ef0: 656e 742e 656e 642c 2065 6e74 2e6c 6162  ent.end, ent.lab
+00006f00: 656c 5f29 290a 6060 600a 0a20 2020 2028  el_)).```..    (
+00006f10: 2741 6e64 6572 736f 6e2c 2047 7269 6e74  'Anderson, Grint
+00006f20: 272c 2030 2c20 332c 2027 4f52 4727 290a  ', 0, 3, 'ORG').
+00006f30: 2020 2020 2827 3535 3527 2c20 392c 2031      ('555', 9, 1
+00006f40: 302c 2027 4341 5244 494e 414c 2729 0a20  0, 'CARDINAL'). 
+00006f50: 2020 2028 2741 7074 2035 272c 2031 342c     ('Apt 5', 14,
+00006f60: 2031 362c 2027 5052 4f44 5543 5427 290a   16, 'PRODUCT').
+00006f70: 2020 2020 2827 4e61 7368 7631 6c65 272c      ('Nashv1le',
+00006f80: 2031 372c 2031 382c 2027 4750 4527 290a   17, 18, 'GPE').
+00006f90: 2020 2020 2827 544e 2035 3535 3535 2d31      ('TN 55555-1
+00006fa0: 3233 3427 2c20 3139 2c20 3233 2c20 274f  234', 19, 23, 'O
+00006fb0: 5247 2729 0a20 2020 2028 2755 5341 272c  RG').    ('USA',
+00006fc0: 2032 352c 2032 362c 2027 4750 4527 290a   25, 26, 'GPE').
+00006fd0: 2020 2020 2827 436f 6e76 6572 6727 2c20      ('Converg', 
+00006fe0: 3334 2c20 3335 2c20 2750 4552 534f 4e27  34, 35, 'PERSON'
+00006ff0: 290a 2020 2020 2827 5a65 726f 272c 2033  ).    ('Zero', 3
+00007000: 382c 2033 392c 2027 4341 5244 494e 414c  8, 39, 'CARDINAL
+00007010: 2729 0a0a 0a57 6869 6c65 2073 7061 4379  ')...While spaCy
+00007020: 2064 6f65 7320 6120 6465 6365 6e74 206a   does a decent j
+00007030: 6f62 206f 6620 6964 656e 7469 6679 696e  ob of identifyin
+00007040: 6720 7468 6174 206e 616d 6564 2065 6e74  g that named ent
+00007050: 6974 6965 7320 6172 6520 7072 6573 656e  ities are presen
+00007060: 7420 696e 2074 6869 7320 6578 616d 706c  t in this exampl
+00007070: 652c 2077 6520 6361 6e20 6465 6669 6e69  e, we can defini
+00007080: 7465 6c79 2069 6d70 726f 7665 2074 6865  tely improve the
+00007090: 206d 6174 6368 6573 202d 2070 6172 7469   matches - parti
+000070a0: 6375 6c61 726c 7920 7769 7468 2074 6865  cularly with the
+000070b0: 2074 7970 6573 206f 6620 6c61 6265 6c73   types of labels
+000070c0: 2061 7070 6c69 6564 2e0a 0a4c 6574 2773   applied...Let's
+000070d0: 2061 6464 2061 6e20 656e 7469 7479 2072   add an entity r
+000070e0: 756c 6572 2066 6f72 2073 6f6d 6520 7275  uler for some ru
+000070f0: 6c65 732d 6261 7365 6420 6d61 7463 6865  les-based matche
+00007100: 732e 0a0a 0a60 6060 7079 7468 6f6e 0a66  s....```python.f
+00007110: 726f 6d20 7370 6163 792e 7069 7065 6c69  rom spacy.pipeli
+00007120: 6e65 2069 6d70 6f72 7420 456e 7469 7479  ne import Entity
+00007130: 5275 6c65 720a 0a65 6e74 6974 795f 7275  Ruler..entity_ru
+00007140: 6c65 7220 3d20 6e6c 702e 6164 645f 7069  ler = nlp.add_pi
+00007150: 7065 2822 656e 7469 7479 5f72 756c 6572  pe("entity_ruler
+00007160: 222c 2062 6566 6f72 653d 226e 6572 2229  ", before="ner")
+00007170: 2023 7370 6143 7920 7633 2073 796e 7461   #spaCy v3 synta
+00007180: 780a 656e 7469 7479 5f72 756c 6572 2e61  x.entity_ruler.a
+00007190: 6464 5f70 6174 7465 726e 7328 0a20 2020  dd_patterns(.   
+000071a0: 205b 7b22 6c61 6265 6c22 3a20 2247 5045   [{"label": "GPE
+000071b0: 222c 2022 7061 7474 6572 6e22 3a20 224e  ", "pattern": "N
+000071c0: 6173 6876 696c 6c65 227d 2c20 7b22 6c61  ashville"}, {"la
+000071d0: 6265 6c22 3a20 2247 5045 222c 2022 7061  bel": "GPE", "pa
+000071e0: 7474 6572 6e22 3a20 2254 4e22 7d5d 0a29  ttern": "TN"}].)
+000071f0: 0a0a 646f 6320 3d20 6e6c 7028 7465 7874  ..doc = nlp(text
+00007200: 290a 0a66 6f72 2065 6e74 2069 6e20 646f  )..for ent in do
+00007210: 632e 656e 7473 3a0a 2020 2020 7072 696e  c.ents:.    prin
+00007220: 7428 2865 6e74 2e74 6578 742c 2065 6e74  t((ent.text, ent
+00007230: 2e73 7461 7274 2c20 656e 742e 656e 642c  .start, ent.end,
+00007240: 2065 6e74 2e6c 6162 656c 5f29 290a 6060   ent.label_)).``
+00007250: 600a 0a20 2020 2028 2741 6e64 6572 736f  `..    ('Anderso
+00007260: 6e2c 2047 7269 6e74 272c 2030 2c20 332c  n, Grint', 0, 3,
+00007270: 2027 4f52 4727 290a 2020 2020 2827 3535   'ORG').    ('55
+00007280: 3527 2c20 392c 2031 302c 2027 4341 5244  5', 9, 10, 'CARD
+00007290: 494e 414c 2729 0a20 2020 2028 2741 7074  INAL').    ('Apt
+000072a0: 2035 272c 2031 342c 2031 362c 2027 5052   5', 14, 16, 'PR
+000072b0: 4f44 5543 5427 290a 2020 2020 2827 4e61  ODUCT').    ('Na
+000072c0: 7368 7631 6c65 272c 2031 372c 2031 382c  shv1le', 17, 18,
+000072d0: 2027 4750 4527 290a 2020 2020 2827 544e   'GPE').    ('TN
+000072e0: 272c 2031 392c 2032 302c 2027 4750 4527  ', 19, 20, 'GPE'
+000072f0: 290a 2020 2020 2827 5553 4127 2c20 3235  ).    ('USA', 25
+00007300: 2c20 3236 2c20 2747 5045 2729 0a20 2020  , 26, 'GPE').   
+00007310: 2028 2743 6f6e 7665 7267 272c 2033 342c   ('Converg', 34,
+00007320: 2033 352c 2027 5045 5253 4f4e 2729 0a20   35, 'PERSON'). 
+00007330: 2020 2028 275a 6572 6f27 2c20 3338 2c20     ('Zero', 38, 
+00007340: 3339 2c20 2743 4152 4449 4e41 4c27 290a  39, 'CARDINAL').
+00007350: 0a0a 5765 2772 6520 6d61 6b69 6e67 2070  ..We're making p
+00007360: 726f 6772 6573 732c 2062 7574 204e 6173  rogress, but Nas
+00007370: 6876 696c 6c65 2069 7320 7370 656c 6c65  hville is spelle
+00007380: 6420 7772 6f6e 6720 696e 2074 6865 2074  d wrong in the t
+00007390: 6578 7420 736f 2074 6865 2065 6e74 6974  ext so the entit
+000073a0: 7920 7275 6c65 7220 646f 6573 206e 6f74  y ruler does not
+000073b0: 2066 696e 6420 6974 2c20 616e 6420 7765   find it, and we
+000073c0: 2073 7469 6c6c 2068 6176 6520 6f74 6865   still have othe
+000073d0: 7220 656e 7469 7469 6573 2074 6f20 6669  r entities to fi
+000073e0: 782f 6669 6e64 2e0a 0a4c 6574 2773 2061  x/find...Let's a
+000073f0: 6464 2061 2073 7061 637a 7a20 7275 6c65  dd a spaczz rule
+00007400: 7220 746f 2072 6f75 6e64 2074 6869 7320  r to round this 
+00007410: 7069 7065 6c69 6e65 206f 7574 2e20 5765  pipeline out. We
+00007420: 2077 696c 6c20 616c 736f 2069 6e63 6c75   will also inclu
+00007430: 6465 2074 6865 2060 7370 6163 7a7a 5f73  de the `spaczz_s
+00007440: 7061 6e60 2063 7573 746f 6d20 6174 7472  pan` custom attr
+00007450: 6962 7574 6520 696e 2074 6865 2072 6573  ibute in the res
+00007460: 756c 7473 2074 6f20 6465 6e6f 7465 2077  ults to denote w
+00007470: 6869 6368 2065 6e74 6974 6965 7320 7765  hich entities we
+00007480: 7265 2073 6574 2076 6961 2073 7061 637a  re set via spacz
+00007490: 7a2e 0a0a 0a60 6060 7079 7468 6f6e 0a73  z....```python.s
+000074a0: 7061 637a 7a5f 7275 6c65 7220 3d20 6e6c  paczz_ruler = nl
+000074b0: 702e 6164 645f 7069 7065 2822 7370 6163  p.add_pipe("spac
+000074c0: 7a7a 5f72 756c 6572 222c 2062 6566 6f72  zz_ruler", befor
+000074d0: 653d 226e 6572 2229 2023 7370 6143 7920  e="ner") #spaCy 
+000074e0: 7633 2073 796e 7461 780a 7370 6163 7a7a  v3 syntax.spaczz
+000074f0: 5f72 756c 6572 2e61 6464 5f70 6174 7465  _ruler.add_patte
+00007500: 726e 7328 0a20 2020 205b 0a20 2020 2020  rns(.    [.     
+00007510: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00007520: 2022 6c61 6265 6c22 3a20 224e 414d 4522   "label": "NAME"
+00007530: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
+00007540: 6174 7465 726e 223a 2022 4772 616e 7420  attern": "Grant 
+00007550: 416e 6465 7273 656e 222c 0a20 2020 2020  Andersen",.     
+00007560: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00007570: 6675 7a7a 7922 2c0a 2020 2020 2020 2020  fuzzy",.        
+00007580: 2020 2020 226b 7761 7267 7322 3a20 7b22      "kwargs": {"
+00007590: 6675 7a7a 795f 6675 6e63 223a 2022 746f  fuzzy_func": "to
+000075a0: 6b65 6e5f 736f 7274 227d 2c0a 2020 2020  ken_sort"},.    
+000075b0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+000075c0: 0a20 2020 2020 2020 2020 2020 2022 6c61  .            "la
+000075d0: 6265 6c22 3a20 2253 5452 4545 5422 2c0a  bel": "STREET",.
+000075e0: 2020 2020 2020 2020 2020 2020 2270 6174              "pat
+000075f0: 7465 726e 223a 2022 7374 7265 6574 5f61  tern": "street_a
+00007600: 6464 7265 7373 6573 222c 0a20 2020 2020  ddresses",.     
+00007610: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00007620: 7265 6765 7822 2c0a 2020 2020 2020 2020  regex",.        
+00007630: 2020 2020 226b 7761 7267 7322 3a20 7b22      "kwargs": {"
+00007640: 7072 6564 6566 223a 2054 7275 657d 2c0a  predef": True},.
+00007650: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00007660: 2020 207b 226c 6162 656c 223a 2022 4750     {"label": "GP
+00007670: 4522 2c20 2270 6174 7465 726e 223a 2022  E", "pattern": "
+00007680: 4e61 7368 7669 6c6c 6522 2c20 2274 7970  Nashville", "typ
+00007690: 6522 3a20 2266 757a 7a79 227d 2c0a 2020  e": "fuzzy"},.  
+000076a0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000076b0: 2020 2020 226c 6162 656c 223a 2022 5a49      "label": "ZI
+000076c0: 5022 2c0a 2020 2020 2020 2020 2020 2020  P",.            
+000076d0: 2270 6174 7465 726e 223a 2072 225c 6228  "pattern": r"\b(
+000076e0: 3f3a 3535 3535 3429 7b73 3c3d 317d 283f  ?:55554){s<=1}(?
+000076f0: 3a5b 2d5c 735d 5c64 7b34 7d29 3f5c 6222  :[-\s]\d{4})?\b"
+00007700: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00007710: 7970 6522 3a20 2272 6567 6578 222c 0a20  ype": "regex",. 
+00007720: 2020 2020 2020 207d 2c20 2023 2066 757a         },  # fuz
+00007730: 7a79 2072 6567 6578 0a20 2020 2020 2020  zy regex.       
+00007740: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00007750: 6c61 6265 6c22 3a20 2242 414e 4422 2c0a  label": "BAND",.
+00007760: 2020 2020 2020 2020 2020 2020 2270 6174              "pat
+00007770: 7465 726e 223a 205b 7b22 4c4f 5745 5222  tern": [{"LOWER"
+00007780: 3a20 7b22 4652 4547 4558 223a 2022 2863  : {"FREGEX": "(c
+00007790: 6f6e 7665 7267 6529 7b65 3c3d 317d 227d  onverge){e<=1}"}
+000077a0: 7d5d 2c0a 2020 2020 2020 2020 2020 2020  }],.            
+000077b0: 2274 7970 6522 3a20 2274 6f6b 656e 222c  "type": "token",
+000077c0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000077d0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000077e0: 2020 226c 6162 656c 223a 2022 4241 4e44    "label": "BAND
+000077f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00007800: 7061 7474 6572 6e22 3a20 5b0a 2020 2020  pattern": [.    
+00007810: 2020 2020 2020 2020 2020 2020 7b22 5445              {"TE
+00007820: 5854 223a 207b 2246 555a 5a59 223a 2022  XT": {"FUZZY": "
+00007830: 5072 6f74 6573 7422 7d7d 2c0a 2020 2020  Protest"}},.    
+00007840: 2020 2020 2020 2020 2020 2020 7b22 4953              {"IS
+00007850: 5f53 544f 5022 3a20 5472 7565 7d2c 0a20  _STOP": True},. 
+00007860: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00007870: 2254 4558 5422 3a20 7b22 4655 5a5a 5922  "TEXT": {"FUZZY"
+00007880: 3a20 2248 6572 6f22 7d7d 2c0a 2020 2020  : "Hero"}},.    
+00007890: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+000078a0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+000078b0: 746f 6b65 6e22 2c0a 2020 2020 2020 2020  token",.        
+000078c0: 7d2c 0a20 2020 205d 0a29 0a0a 646f 6320  },.    ].)..doc 
+000078d0: 3d20 6e6c 7028 7465 7874 290a 0a66 6f72  = nlp(text)..for
+000078e0: 2065 6e74 2069 6e20 646f 632e 656e 7473   ent in doc.ents
+000078f0: 3a0a 2020 2020 7072 696e 7428 2865 6e74  :.    print((ent
+00007900: 2e74 6578 742c 2065 6e74 2e73 7461 7274  .text, ent.start
+00007910: 2c20 656e 742e 656e 642c 2065 6e74 2e6c  , ent.end, ent.l
+00007920: 6162 656c 5f2c 2065 6e74 2e5f 2e73 7061  abel_, ent._.spa
+00007930: 637a 7a5f 656e 7429 290a 6060 600a 0a20  czz_ent)).```.. 
+00007940: 2020 2028 2741 6e64 6572 736f 6e2c 2047     ('Anderson, G
+00007950: 7269 6e74 272c 2030 2c20 332c 2027 4e41  rint', 0, 3, 'NA
+00007960: 4d45 272c 2054 7275 6529 0a20 2020 2028  ME', True).    (
+00007970: 2735 3535 2046 616b 6520 5374 2c27 2c20  '555 Fake St,', 
+00007980: 392c 2031 332c 2027 5354 5245 4554 272c  9, 13, 'STREET',
+00007990: 2054 7275 6529 0a20 2020 2028 2741 7074   True).    ('Apt
+000079a0: 2035 272c 2031 342c 2031 362c 2027 5052   5', 14, 16, 'PR
+000079b0: 4f44 5543 5427 2c20 4661 6c73 6529 0a20  ODUCT', False). 
+000079c0: 2020 2028 274e 6173 6876 316c 6527 2c20     ('Nashv1le', 
+000079d0: 3137 2c20 3138 2c20 2747 5045 272c 2054  17, 18, 'GPE', T
+000079e0: 7275 6529 0a20 2020 2028 2754 4e27 2c20  rue).    ('TN', 
+000079f0: 3139 2c20 3230 2c20 2747 5045 272c 2046  19, 20, 'GPE', F
+00007a00: 616c 7365 290a 2020 2020 2827 3535 3535  alse).    ('5555
+00007a10: 352d 3132 3334 272c 2032 302c 2032 332c  5-1234', 20, 23,
+00007a20: 2027 5a49 5027 2c20 5472 7565 290a 2020   'ZIP', True).  
+00007a30: 2020 2827 5553 4127 2c20 3235 2c20 3236    ('USA', 25, 26
+00007a40: 2c20 2747 5045 272c 2046 616c 7365 290a  , 'GPE', False).
+00007a50: 2020 2020 2827 436f 6e76 6572 6727 2c20      ('Converg', 
+00007a60: 3334 2c20 3335 2c20 2742 414e 4427 2c20  34, 35, 'BAND', 
+00007a70: 5472 7565 290a 2020 2020 2827 5072 6f74  True).    ('Prot
+00007a80: 6574 2074 6865 205a 6572 6f27 2c20 3336  et the Zero', 36
+00007a90: 2c20 3339 2c20 2742 414e 4427 2c20 5472  , 39, 'BAND', Tr
+00007aa0: 7565 290a 0a0a 4177 6573 6f6d 6521 2054  ue)...Awesome! T
+00007ab0: 6865 2073 6d61 6c6c 2045 6e67 6c69 7368  he small English
+00007ac0: 206d 6f64 656c 2073 7469 6c6c 206d 616b   model still mak
+00007ad0: 6573 2061 206e 616d 6564 2065 6e74 6974  es a named entit
+00007ae0: 7920 7265 636f 676e 6974 696f 6e20 6d69  y recognition mi
+00007af0: 7374 616b 6520 2822 3522 2069 6e20 2241  stake ("5" in "A
+00007b00: 7074 2035 2220 6173 2060 4341 5244 494e  pt 5" as `CARDIN
+00007b10: 414c 6029 2c20 6275 7420 7765 2772 6520  AL`), but we're 
+00007b20: 7361 7469 7366 6965 6420 6f76 6572 616c  satisfied overal
+00007b30: 6c2e 0a0a 4c65 7427 7320 7361 7665 2074  l...Let's save t
+00007b40: 6869 7320 7069 7065 6c69 6e65 2074 6f20  his pipeline to 
+00007b50: 6469 736b 2061 6e64 206d 616b 6520 7375  disk and make su
+00007b60: 7265 2077 6520 6361 6e20 6c6f 6164 2069  re we can load i
+00007b70: 7420 6261 636b 2063 6f72 7265 6374 6c79  t back correctly
+00007b80: 2e0a 0a0a 6060 6070 7974 686f 6e0a 696d  ....```python.im
+00007b90: 706f 7274 2074 656d 7066 696c 650a 0a77  port tempfile..w
+00007ba0: 6974 6820 7465 6d70 6669 6c65 2e54 656d  ith tempfile.Tem
+00007bb0: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
+00007bc0: 2920 6173 2074 6d70 5f64 6972 3a0a 2020  ) as tmp_dir:.  
+00007bd0: 2020 6e6c 702e 746f 5f64 6973 6b28 6622    nlp.to_disk(f"
+00007be0: 7b74 6d70 5f64 6972 7d2f 6578 616d 706c  {tmp_dir}/exampl
+00007bf0: 655f 7069 7065 6c69 6e65 2229 0a20 2020  e_pipeline").   
+00007c00: 206e 6c70 203d 2073 7061 6379 2e6c 6f61   nlp = spacy.loa
+00007c10: 6428 6622 7b74 6d70 5f64 6972 7d2f 6578  d(f"{tmp_dir}/ex
+00007c20: 616d 706c 655f 7069 7065 6c69 6e65 2229  ample_pipeline")
+00007c30: 0a0a 6e6c 702e 7069 7065 5f6e 616d 6573  ..nlp.pipe_names
+00007c40: 0a60 6060 0a0a 0a0a 0a20 2020 205b 2774  .```.....    ['t
+00007c50: 6f6b 3276 6563 272c 0a20 2020 2020 2774  ok2vec',.     't
+00007c60: 6167 6765 7227 2c0a 2020 2020 2027 7061  agger',.     'pa
+00007c70: 7273 6572 272c 0a20 2020 2020 2761 7474  rser',.     'att
+00007c80: 7269 6275 7465 5f72 756c 6572 272c 0a20  ribute_ruler',. 
+00007c90: 2020 2020 276c 656d 6d61 7469 7a65 7227      'lemmatizer'
+00007ca0: 2c0a 2020 2020 2027 656e 7469 7479 5f72  ,.     'entity_r
+00007cb0: 756c 6572 272c 0a20 2020 2020 2773 7061  uler',.     'spa
+00007cc0: 637a 7a5f 7275 6c65 7227 2c0a 2020 2020  czz_ruler',.    
+00007cd0: 2027 6e65 7227 5d0a 0a0a 0a57 6520 6361   'ner']....We ca
+00007ce0: 6e20 6576 656e 2065 6e73 7572 6520 616c  n even ensure al
+00007cf0: 6c20 7468 6520 7370 6163 7a7a 2072 756c  l the spaczz rul
+00007d00: 6572 2070 6174 7465 726e 7320 6172 6520  er patterns are 
+00007d10: 7374 696c 6c20 7072 6573 656e 742e 0a0a  still present...
+00007d20: 0a60 6060 7079 7468 6f6e 0a73 7061 637a  .```python.spacz
+00007d30: 7a5f 7275 6c65 7220 3d20 6e6c 702e 6765  z_ruler = nlp.ge
+00007d40: 745f 7069 7065 2822 7370 6163 7a7a 5f72  t_pipe("spaczz_r
+00007d50: 756c 6572 2229 0a73 7061 637a 7a5f 7275  uler").spaczz_ru
+00007d60: 6c65 722e 7061 7474 6572 6e73 0a60 6060  ler.patterns.```
+00007d70: 0a0a 0a0a 0a20 2020 205b 7b27 6c61 6265  .....    [{'labe
+00007d80: 6c27 3a20 274e 414d 4527 2c0a 2020 2020  l': 'NAME',.    
+00007d90: 2020 2770 6174 7465 726e 273a 2027 4772    'pattern': 'Gr
+00007da0: 616e 7420 416e 6465 7273 656e 272c 0a20  ant Andersen',. 
+00007db0: 2020 2020 2027 7479 7065 273a 2027 6675       'type': 'fu
+00007dc0: 7a7a 7927 2c0a 2020 2020 2020 276b 7761  zzy',.      'kwa
+00007dd0: 7267 7327 3a20 7b27 6675 7a7a 795f 6675  rgs': {'fuzzy_fu
+00007de0: 6e63 273a 2027 746f 6b65 6e5f 736f 7274  nc': 'token_sort
+00007df0: 277d 7d2c 0a20 2020 2020 7b27 6c61 6265  '}},.     {'labe
+00007e00: 6c27 3a20 2747 5045 272c 2027 7061 7474  l': 'GPE', 'patt
+00007e10: 6572 6e27 3a20 274e 6173 6876 696c 6c65  ern': 'Nashville
+00007e20: 272c 2027 7479 7065 273a 2027 6675 7a7a  ', 'type': 'fuzz
+00007e30: 7927 7d2c 0a20 2020 2020 7b27 6c61 6265  y'},.     {'labe
+00007e40: 6c27 3a20 2753 5452 4545 5427 2c0a 2020  l': 'STREET',.  
+00007e50: 2020 2020 2770 6174 7465 726e 273a 2027      'pattern': '
+00007e60: 7374 7265 6574 5f61 6464 7265 7373 6573  street_addresses
+00007e70: 272c 0a20 2020 2020 2027 7479 7065 273a  ',.      'type':
+00007e80: 2027 7265 6765 7827 2c0a 2020 2020 2020   'regex',.      
+00007e90: 276b 7761 7267 7327 3a20 7b27 7072 6564  'kwargs': {'pred
+00007ea0: 6566 273a 2054 7275 657d 7d2c 0a20 2020  ef': True}},.   
+00007eb0: 2020 7b27 6c61 6265 6c27 3a20 275a 4950    {'label': 'ZIP
+00007ec0: 272c 0a20 2020 2020 2027 7061 7474 6572  ',.      'patter
+00007ed0: 6e27 3a20 275c 5c62 283f 3a35 3535 3534  n': '\\b(?:55554
+00007ee0: 297b 733c 3d31 7d28 3f3a 5b2d 5c5c 735d  ){s<=1}(?:[-\\s]
+00007ef0: 5c5c 647b 347d 293f 5c5c 6227 2c0a 2020  \\d{4})?\\b',.  
+00007f00: 2020 2020 2774 7970 6527 3a20 2772 6567      'type': 'reg
+00007f10: 6578 277d 2c0a 2020 2020 207b 276c 6162  ex'},.     {'lab
+00007f20: 656c 273a 2027 4241 4e44 272c 0a20 2020  el': 'BAND',.   
+00007f30: 2020 2027 7061 7474 6572 6e27 3a20 5b7b     'pattern': [{
+00007f40: 274c 4f57 4552 273a 207b 2746 5245 4745  'LOWER': {'FREGE
+00007f50: 5827 3a20 2728 636f 6e76 6572 6765 297b  X': '(converge){
+00007f60: 653c 3d31 7d27 7d7d 5d2c 0a20 2020 2020  e<=1}'}}],.     
+00007f70: 2027 7479 7065 273a 2027 746f 6b65 6e27   'type': 'token'
+00007f80: 7d2c 0a20 2020 2020 7b27 6c61 6265 6c27  },.     {'label'
+00007f90: 3a20 2742 414e 4427 2c0a 2020 2020 2020  : 'BAND',.      
+00007fa0: 2770 6174 7465 726e 273a 205b 7b27 5445  'pattern': [{'TE
+00007fb0: 5854 273a 207b 2746 555a 5a59 273a 2027  XT': {'FUZZY': '
+00007fc0: 5072 6f74 6573 7427 7d7d 2c0a 2020 2020  Protest'}},.    
+00007fd0: 2020 207b 2749 535f 5354 4f50 273a 2054     {'IS_STOP': T
+00007fe0: 7275 657d 2c0a 2020 2020 2020 207b 2754  rue},.       {'T
+00007ff0: 4558 5427 3a20 7b27 4655 5a5a 5927 3a20  EXT': {'FUZZY': 
+00008000: 2748 6572 6f27 7d7d 5d2c 0a20 2020 2020  'Hero'}}],.     
+00008010: 2027 7479 7065 273a 2027 746f 6b65 6e27   'type': 'token'
+00008020: 7d5d 0a0a 0a0a 2323 204b 6e6f 776e 2049  }]....## Known I
+00008030: 7373 7565 730a 0a23 2323 2050 6572 666f  ssues..### Perfo
+00008040: 726d 616e 6365 0a0a 5468 6520 6d61 696e  rmance..The main
+00008050: 2072 6561 736f 6e20 666f 7220 7370 6163   reason for spac
+00008060: 7a7a 2773 2073 6c6f 7765 7220 7370 6565  zz's slower spee
+00008070: 6420 6973 2074 6861 7420 7468 6520 2a63  d is that the *c
+00008080: 2a20 696e 2069 7427 7320 6e61 6d65 2069  * in it's name i
+00008090: 7320 6e6f 7420 6361 7069 7461 6c69 7a65  s not capitalize
+000080a0: 6420 6c69 6b65 2069 7420 6973 2069 6e20  d like it is in 
+000080b0: 7370 612a 432a 792e 0a53 7061 637a 7a20  spa*C*y..Spaczz 
+000080c0: 6973 2077 7269 7474 656e 2069 6e20 7075  is written in pu
+000080d0: 7265 2050 7974 686f 6e20 616e 6420 6974  re Python and it
+000080e0: 2773 206d 6174 6368 6572 7320 646f 206e  's matchers do n
+000080f0: 6f74 2063 7572 7265 6e74 6c79 2075 7469  ot currently uti
+00008100: 6c69 7a65 2073 7061 4379 206c 616e 6775  lize spaCy langu
+00008110: 6167 6520 766f 6361 6275 6c61 7269 6573  age vocabularies
+00008120: 2c20 7768 6963 6820 6d65 616e 7320 666f  , which means fo
+00008130: 6c6c 6f77 696e 6720 6974 2773 206c 6f67  llowing it's log
+00008140: 6963 2073 686f 756c 6420 6265 2065 6173  ic should be eas
+00008150: 7920 746f 2074 686f 7365 2066 616d 696c  y to those famil
+00008160: 6961 7220 7769 7468 2050 7974 686f 6e2e  iar with Python.
+00008170: 2048 6f77 6576 6572 2074 6869 7320 6d65   However this me
+00008180: 616e 7320 7370 6163 7a7a 2063 6f6d 706f  ans spaczz compo
+00008190: 6e65 6e74 7320 7769 6c6c 2072 756e 2073  nents will run s
+000081a0: 6c6f 7765 7220 616e 6420 6c69 6b65 6c79  lower and likely
+000081b0: 2063 6f6e 7375 6d65 206d 6f72 6520 6d65   consume more me
+000081c0: 6d6f 7279 2074 6861 6e20 7468 6569 7220  mory than their 
+000081d0: 7370 6143 7920 636f 756e 7465 7270 6172  spaCy counterpar
+000081e0: 7473 2c20 6573 7065 6369 616c 6c79 2061  ts, especially a
+000081f0: 7320 6d6f 7265 2070 6174 7465 726e 7320  s more patterns 
+00008200: 6172 6520 6164 6465 6420 616e 6420 646f  are added and do
+00008210: 6375 6d65 6e74 7320 6765 7420 6c6f 6e67  cuments get long
+00008220: 6572 2e20 4974 2069 7320 7468 6572 6566  er. It is theref
+00008230: 6f72 6520 7265 636f 6d6d 656e 6465 6420  ore recommended 
+00008240: 746f 2075 7365 2073 7061 4379 2063 6f6d  to use spaCy com
+00008250: 706f 6e65 6e74 7320 6c69 6b65 2074 6865  ponents like the
+00008260: 2045 6e74 6974 7952 756c 6572 2066 6f72   EntityRuler for
+00008270: 2065 6e74 6974 6965 7320 7769 7468 206c   entities with l
+00008280: 6974 746c 6520 756e 6365 7274 6169 6e74  ittle uncertaint
+00008290: 792c 206c 696b 6520 636f 6e73 6973 7465  y, like consiste
+000082a0: 6e74 2073 7065 6c6c 696e 6720 6572 726f  nt spelling erro
+000082b0: 7273 2e20 5573 6520 7370 6163 7a7a 2063  rs. Use spaczz c
+000082c0: 6f6d 706f 6e65 6e74 7320 7768 656e 2074  omponents when t
+000082d0: 6865 7265 2061 7265 206e 6f74 2076 6961  here are not via
+000082e0: 626c 6520 7370 6143 7920 616c 7465 726e  ble spaCy altern
+000082f0: 6174 6976 6573 2e0a 0a49 2061 6d20 2a6e  atives...I am *n
+00008300: 6f74 2a20 6375 7272 656e 746c 7920 776f  ot* currently wo
+00008310: 726b 696e 6720 6f6e 2070 6572 666f 726d  rking on perform
+00008320: 616e 6365 206f 7074 696d 697a 6174 696f  ance optimizatio
+00008330: 6e73 2074 6f20 7370 6163 7a7a 2c20 6275  ns to spaczz, bu
+00008340: 7420 616c 676f 7269 7468 6d69 6320 616e  t algorithmic an
+00008350: 6420 6f70 7469 6d69 7a61 7469 6f6e 2073  d optimization s
+00008360: 7567 6765 7374 696f 6e73 2061 7265 2077  uggestions are w
+00008370: 656c 636f 6d65 2e0a 0a54 6865 2070 7269  elcome...The pri
+00008380: 6d61 7279 206d 6574 686f 6473 2066 6f72  mary methods for
+00008390: 2073 7065 6564 696e 6720 7570 2074 6865   speeding up the
+000083a0: 2060 4675 7a7a 794d 6174 6368 6572 6020   `FuzzyMatcher` 
+000083b0: 616e 6420 6053 696d 696c 6172 6974 794d  and `SimilarityM
+000083c0: 6174 6368 6572 6020 6172 6520 6279 2064  atcher` are by d
+000083d0: 6563 7265 6173 696e 6720 7468 6520 6066  ecreasing the `f
+000083e0: 6c65 7860 2070 6172 616d 6574 6572 2074  lex` parameter t
+000083f0: 6f77 6172 6473 2060 3060 2c20 6f72 2069  owards `0`, or i
+00008400: 6620 6066 6c65 7820 3e20 3060 2c20 696e  f `flex > 0`, in
+00008410: 6372 6561 7369 6e67 2074 6865 2060 6d69  creasing the `mi
+00008420: 6e5f 7231 6020 7061 7261 6d65 7465 7220  n_r1` parameter 
+00008430: 746f 7761 7264 7320 7468 6520 7661 6c75  towards the valu
+00008440: 6520 6f66 2060 6d69 6e5f 7232 6020 616e  e of `min_r2` an
+00008450: 642f 6f72 206c 6f77 6572 696e 6720 7468  d/or lowering th
+00008460: 6520 6074 6872 6573 6860 2070 6172 616d  e `thresh` param
+00008470: 6574 6572 2074 6f77 6172 6473 2060 6d69  eter towards `mi
+00008480: 6e5f 7232 602e 2042 6520 6177 6172 6520  n_r2`. Be aware 
+00008490: 7468 6174 2061 6c6c 206f 6620 7468 6573  that all of thes
+000084a0: 6520 2273 7065 6564 2d75 7073 2220 636f  e "speed-ups" co
+000084b0: 6d65 2061 7420 7468 6520 6f70 706f 7274  me at the opport
+000084c0: 756e 6974 7920 636f 7374 206f 6620 706f  unity cost of po
+000084d0: 7465 6e74 6961 6c6c 7920 696d 7072 6f76  tentially improv
+000084e0: 6564 206d 6174 6368 6573 2e0a 0a41 7320  ed matches...As 
+000084f0: 6d65 6e74 696f 6e65 6420 696e 2074 6865  mentioned in the
+00008500: 2060 5369 6d69 6c61 7269 7479 4d61 7463   `SimilarityMatc
+00008510: 6865 7260 2064 6573 6372 6970 7469 6f6e  her` description
+00008520: 2c20 7574 696c 697a 696e 6720 6120 4750  , utilizing a GP
+00008530: 5520 6d61 7920 616c 736f 2068 656c 7020  U may also help 
+00008540: 7370 6565 6420 7570 2069 7427 7320 6d61  speed up it's ma
+00008550: 7463 6869 6e67 2070 726f 6365 7373 2e0a  tching process..
+00008560: 0a23 2320 526f 6164 6d61 700a 0a49 2061  .## Roadmap..I a
+00008570: 6d20 616c 7761 7973 206f 7065 6e20 616e  m always open an
+00008580: 6420 7265 6365 7074 6976 6520 746f 2066  d receptive to f
+00008590: 6561 7475 7265 2072 6571 7565 7374 7320  eature requests 
+000085a0: 6275 7420 6a75 7374 2062 6520 6177 6172  but just be awar
+000085b0: 652c 2061 7320 6120 736f 6c6f 2d64 6576  e, as a solo-dev
+000085c0: 2077 6974 6820 6120 6c6f 7420 6c65 6674   with a lot left
+000085d0: 2074 6f20 6c65 6172 6e2c 2064 6576 656c   to learn, devel
+000085e0: 6f70 6d65 6e74 2063 616e 206d 6f76 6520  opment can move 
+000085f0: 7072 6574 7479 2073 6c6f 772e 2054 6865  pretty slow. The
+00008600: 2066 6f6c 6c6f 7769 6e67 2069 7320 6d79   following is my
+00008610: 2072 6f61 646d 6170 2066 6f72 2073 7061   roadmap for spa
+00008620: 637a 7a20 736f 2079 6f75 2063 616e 2073  czz so you can s
+00008630: 6565 2077 6865 7265 2069 7373 7565 7320  ee where issues 
+00008640: 7261 6973 6564 206d 6967 6874 2066 6974  raised might fit
+00008650: 2069 6e74 6f20 6d79 2063 7572 7265 6e74   into my current
+00008660: 2070 7269 6f72 6974 6965 732e 0a0a 2a4e   priorities...*N
+00008670: 6f74 653a 2077 6869 6c65 2049 2077 616e  ote: while I wan
+00008680: 7420 746f 206b 6565 7020 6073 7061 637a  t to keep `spacz
+00008690: 7a60 2066 756e 6374 696f 6e61 6c2c 2049  z` functional, I
+000086a0: 2061 6d20 2a2a 6e6f 742a 2a20 6163 7469   am **not** acti
+000086b0: 7665 6c79 2064 6576 656c 6f70 696e 6720  vely developing 
+000086c0: 6974 2e20 4920 7472 7920 746f 2062 6520  it. I try to be 
+000086d0: 7265 7370 6f6e 7369 7665 2074 6f20 6973  responsive to is
+000086e0: 7375 6573 2061 6e64 2072 6571 7565 7374  sues and request
+000086f0: 7320 6275 7420 7468 6973 2070 726f 6a65  s but this proje
+00008700: 6374 2069 7320 6e6f 7420 6375 7272 656e  ct is not curren
+00008710: 746c 7920 6120 666f 6375 7320 6f66 206d  tly a focus of m
+00008720: 696e 652e 2a0a 0a2a 2a48 6967 6820 5072  ine.*..**High Pr
+00008730: 696f 7269 7479 2a2a 0a0a 312e 2042 7567  iority**..1. Bug
+00008740: 2066 6978 6573 202d 2062 6f74 6820 6272   fixes - both br
+00008750: 6561 6b69 6e67 2061 6e64 2062 6568 6176  eaking and behav
+00008760: 696f 7261 6c2e 2048 6f70 6566 756c 6c79  ioral. Hopefully
+00008770: 2074 6865 7365 2077 696c 6c20 6265 206d   these will be m
+00008780: 696e 696d 616c 2e0a 312e 2045 6173 6520  inimal..1. Ease 
 00008790: 6f66 2075 7365 2061 6e64 2065 7272 6f72  of use and error
 000087a0: 2f77 6172 6e69 6e67 2068 616e 646c 696e  /warning handlin
 000087b0: 6720 616e 6420 6d65 7373 6167 696e 6720  g and messaging 
-000087c0: 656e 6861 6e63 656d 656e 7473 2e5c 6e31  enhancements.\n1
-000087d0: 2e20 4275 696c 6469 6e67 206f 7574 2052  . Building out R
-000087e0: 6561 6420 7468 6520 446f 6373 2e5c 6e31  ead the Docs.\n1
-000087f0: 2e20 4120 6d65 7468 6f64 2066 6f72 2063  . A method for c
-00008800: 6f6d 7061 7269 6e67 2066 757a 7a79 2072  omparing fuzzy r
-00008810: 6174 696f 7320 616e 6420 6675 7a7a 7920  atios and fuzzy 
-00008820: 7265 6765 7820 636f 756e 7473 2e5c 6e31  regex counts.\n1
-00008830: 2e20 4120 7761 7920 746f 2072 6574 7572  . A way to retur
-00008840: 6e20 6d61 7463 6820 6465 7461 696c 7320  n match details 
-00008850: 6672 6f6d 2074 6865 2060 546f 6b65 6e4d  from the `TokenM
-00008860: 6174 6368 6572 602e 5c6e 312e 204f 7074  atcher`.\n1. Opt
-00008870: 696f 6e20 746f 2070 7269 6f72 6974 697a  ion to prioritiz
-00008880: 6520 6d61 7463 6820 7175 616c 6974 7920  e match quality 
-00008890: 6f76 6572 206c 656e 6774 6820 616e 642f  over length and/
-000088a0: 6f72 2077 6569 6768 696e 6720 6f70 7469  or weighing opti
-000088b0: 6f6e 732e 5c6e 312e 2050 726f 6669 6c69  ons.\n1. Profili
-000088c0: 6e67 202d 2068 6f70 6566 756c 6c79 2074  ng - hopefully t
-000088d0: 6f20 6669 6e64 2022 6561 7379 2220 7065  o find "easy" pe
-000088e0: 7266 6f72 6d61 6e63 6520 6f70 7469 6d69  rformance optimi
-000088f0: 7a61 7469 6f6e 732e 5c6e 5c6e 2a2a 456e  zations.\n\n**En
-00008900: 6861 6e63 656d 656e 7473 2a2a 5c6e 5c6e  hancements**\n\n
-00008910: 312e 2041 5049 2073 7570 706f 7274 2066  1. API support f
-00008920: 6f72 2061 6464 696e 6720 7573 6572 2d64  or adding user-d
-00008930: 6566 696e 6564 2072 6567 6578 6573 2074  efined regexes t
-00008940: 6f20 7468 6520 7072 6564 6566 696e 6564  o the predefined
-00008950: 2072 6567 6578 2e5c 6e20 2020 2031 2e20   regex.\n    1. 
-00008960: 5361 7669 6e67 2074 6865 7365 2061 6464  Saving these add
-00008970: 6974 696f 6e61 6c20 7072 6564 6566 696e  itional predefin
-00008980: 6564 2072 6567 6578 6573 2061 7320 7061  ed regexes as pa
-00008990: 7274 206f 6620 7468 6520 5370 6163 7a7a  rt of the Spaczz
-000089a0: 5275 6c65 7220 7769 6c6c 2061 6c73 6f20  Ruler will also 
-000089b0: 6265 2073 7570 706f 7274 6564 2e5c 6e31  be supported.\n1
-000089c0: 2e20 456e 7469 7479 2073 7461 7274 2f65  . Entity start/e
-000089d0: 6e64 2074 7269 6d6d 696e 6720 6f6e 2074  nd trimming on t
-000089e0: 6865 2074 6f6b 656e 206c 6576 656c 2074  he token level t
-000089f0: 6f20 7072 6576 656e 7420 6675 7a7a 7920  o prevent fuzzy 
-00008a00: 616e 6420 7265 6765 7820 7068 7261 7365  and regex phrase
-00008a10: 206d 6174 6368 6573 2066 726f 6d20 7374   matches from st
-00008a20: 6172 7469 6e67 2f65 6e64 696e 6720 7769  arting/ending wi
-00008a30: 7468 2075 6e77 616e 7465 6420 746f 6b65  th unwanted toke
-00008a40: 6e73 2c20 692e 652e 2073 7061 6365 732f  ns, i.e. spaces/
-00008a50: 7075 6e63 7475 6174 696f 6e2e 5c6e 5c6e  punctuation.\n\n
-00008a60: 2a2a 4c6f 6e67 2d48 6f72 697a 6f6e 2050  **Long-Horizon P
-00008a70: 6572 666f 726d 616e 6365 2045 6e68 616e  erformance Enhan
-00008a80: 6365 6d65 6e74 732a 2a5c 6e5c 6e31 2e20  cements**\n\n1. 
-00008a90: 4861 7669 6e67 2073 7061 637a 7a20 6d61  Having spaczz ma
-00008aa0: 7463 6865 7273 2075 7469 6c69 7a65 2073  tchers utilize s
-00008ab0: 7061 4379 2076 6f63 6162 756c 6172 6965  paCy vocabularie
-00008ac0: 732e 5c6e 312e 2052 6577 7269 7465 2074  s.\n1. Rewrite t
-00008ad0: 6865 2070 6872 6173 6520 616e 6420 746f  he phrase and to
-00008ae0: 6b65 6e20 7365 6172 6368 696e 6720 616c  ken searching al
-00008af0: 676f 7269 7468 6d73 2069 6e20 4379 7468  gorithms in Cyth
-00008b00: 6f6e 2074 6f20 7574 696c 697a 6520 4320  on to utilize C 
-00008b10: 7370 6565 642e 5c6e 2020 2020 312e 2054  speed.\n    1. T
-00008b20: 7279 2074 6f20 696e 7465 6772 6174 6520  ry to integrate 
-00008b30: 636c 6f73 656c 7920 7769 7468 2073 7061  closely with spa
-00008b40: 4379 2e5c 6e5c 6e23 2320 4465 7665 6c6f  Cy.\n\n## Develo
-00008b50: 706d 656e 745c 6e5c 6e50 756c 6c20 7265  pment\n\nPull re
-00008b60: 7175 6573 7473 2061 6e64 2063 6f6e 7472  quests and contr
-00008b70: 6962 7574 6f72 7320 6172 6520 7765 6c63  ibutors are welc
-00008b80: 6f6d 652e 5c6e 5c6e 7370 6163 7a7a 2069  ome.\n\nspaczz i
-00008b90: 7320 6c69 6e74 6564 2077 6974 6820 5b46  s linted with [F
-00008ba0: 6c61 6b65 385d 2868 7474 7073 3a2f 2f66  lake8](https://f
-00008bb0: 6c61 6b65 382e 7079 6371 612e 6f72 672f  lake8.pycqa.org/
-00008bc0: 656e 2f6c 6174 6573 742f 292c 2066 6f72  en/latest/), for
-00008bd0: 6d61 7474 6564 2077 6974 6820 5b42 6c61  matted with [Bla
-00008be0: 636b 5d28 6874 7470 733a 2f2f 626c 6163  ck](https://blac
-00008bf0: 6b2e 7265 6164 7468 6564 6f63 732e 696f  k.readthedocs.io
-00008c00: 2f65 6e2f 7374 6162 6c65 2f29 2c20 7479  /en/stable/), ty
-00008c10: 7065 2d63 6865 636b 6564 2077 6974 6820  pe-checked with 
-00008c20: 5b4d 7950 795d 2868 7474 703a 2f2f 6d79  [MyPy](http://my
-00008c30: 7079 2d6c 616e 672e 6f72 672f 2920 2861  py-lang.org/) (a
-00008c40: 6c74 686f 7567 6820 7468 6973 2063 6f75  lthough this cou
-00008c50: 6c64 2062 656e 6566 6974 2066 726f 6d20  ld benefit from 
-00008c60: 696d 7072 6f76 6564 2073 7065 6369 6669  improved specifi
-00008c70: 6369 7479 292c 2074 6573 7465 6420 7769  city), tested wi
-00008c80: 7468 205b 5079 7465 7374 5d28 6874 7470  th [Pytest](http
-00008c90: 733a 2f2f 646f 6373 2e70 7974 6573 742e  s://docs.pytest.
-00008ca0: 6f72 672f 656e 2f73 7461 626c 652f 292c  org/en/stable/),
-00008cb0: 2061 7574 6f6d 6174 6564 2077 6974 6820   automated with 
-00008cc0: 5b4e 6f78 5d28 6874 7470 733a 2f2f 6e6f  [Nox](https://no
-00008cd0: 782e 7468 6561 2e63 6f64 6573 2f65 6e2f  x.thea.codes/en/
-00008ce0: 7374 6162 6c65 2f29 2c20 616e 6420 6275  stable/), and bu
-00008cf0: 696c 742f 7061 636b 6167 6564 2077 6974  ilt/packaged wit
-00008d00: 6820 5b50 6f65 7472 795d 2868 7474 7073  h [Poetry](https
-00008d10: 3a2f 2f70 7974 686f 6e2d 706f 6574 7279  ://python-poetry
-00008d20: 2e6f 7267 2f29 2e20 5468 6572 6520 6172  .org/). There ar
-00008d30: 6520 6120 6665 7720 6f74 6865 7220 6465  e a few other de
-00008d40: 7665 6c6f 706d 656e 7420 746f 6f6c 7320  velopment tools 
-00008d50: 6465 7461 696c 6564 2069 6e20 7468 6520  detailed in the 
-00008d60: 6e6f 7866 696c 652e 7079 2c20 616c 6f6e  noxfile.py, alon
-00008d70: 6720 7769 7468 2047 6974 2070 7265 2d63  g with Git pre-c
-00008d80: 6f6d 6d69 7420 686f 6f6b 732e 5c6e 5c6e  ommit hooks.\n\n
-00008d90: 546f 2063 6f6e 7472 6962 7574 6520 746f  To contribute to
-00008da0: 2073 7061 637a 7a5c 2773 2064 6576 656c   spaczz\'s devel
-00008db0: 6f70 6d65 6e74 2c20 666f 726b 2074 6865  opment, fork the
-00008dc0: 2072 6570 6f73 6974 6f72 7920 7468 656e   repository then
-00008dd0: 2069 6e73 7461 6c6c 2073 7061 637a 7a20   install spaczz 
-00008de0: 616e 6420 6974 5c27 7320 6465 7620 6465  and it\'s dev de
-00008df0: 7065 6e64 656e 6369 6573 2077 6974 6820  pendencies with 
-00008e00: 506f 6574 7279 2e20 4966 2079 6f75 5c27  Poetry. If you\'
-00008e10: 7265 2069 6e74 6572 6573 7465 6420 696e  re interested in
-00008e20: 2062 6569 6e67 2061 2072 6567 756c 6172   being a regular
-00008e30: 2063 6f6e 7472 6962 7574 6f72 2070 6c65   contributor ple
-00008e40: 6173 6520 636f 6e74 6163 7420 6d65 2064  ase contact me d
-00008e50: 6972 6563 746c 792e 5c6e 5c6e 5c6e 6060  irectly.\n\n\n``
-00008e60: 6070 7974 686f 6e5c 6e70 6f65 7472 7920  `python\npoetry 
-00008e70: 696e 7374 616c 6c20 2320 5769 7468 696e  install # Within
-00008e80: 2073 7061 637a 7a5c 2773 2072 6f6f 7420   spaczz\'s root 
-00008e90: 6469 7265 6374 6f72 792e 5c6e 6060 605c  directory.\n```\
-00008ea0: 6e5c 6e49 206b 6565 7020 4e6f 7820 616e  n\nI keep Nox an
-00008eb0: 6420 7072 652d 636f 6d6d 6974 206f 7574  d pre-commit out
-00008ec0: 7369 6465 206f 6620 6d79 2070 6f65 7472  side of my poetr
-00008ed0: 7920 656e 7669 726f 6e6d 656e 7420 6173  y environment as
-00008ee0: 2070 6172 7420 6f66 206d 7920 5079 7468   part of my Pyth
-00008ef0: 6f6e 2074 6f6f 6c63 6861 696e 2065 6e76  on toolchain env
-00008f00: 6972 6f6e 6d65 6e74 732e 2057 6974 6820  ironments. With 
-00008f10: 7072 652d 636f 6d6d 6974 2069 6e73 7461  pre-commit insta
-00008f20: 6c6c 6564 2079 6f75 206d 6179 2061 6c73  lled you may als
-00008f30: 6f20 6e65 6564 2074 6f20 7275 6e20 7468  o need to run th
-00008f40: 6520 6265 6c6f 7720 746f 2063 6f6d 6d69  e below to commi
-00008f50: 7420 6368 616e 6765 732e 5c6e 5c6e 5c6e  t changes.\n\n\n
-00008f60: 6060 6070 7974 686f 6e5c 6e70 7265 2d63  ```python\npre-c
-00008f70: 6f6d 6d69 7420 696e 7374 616c 6c5c 6e60  ommit install\n`
-00008f80: 6060 5c6e 5c6e 5468 6520 6f6e 6c79 206f  ``\n\nThe only o
-00008f90: 7468 6572 2070 6163 6b61 6765 2074 6861  ther package tha
-00008fa0: 7420 7769 6c6c 206e 6f74 2062 6520 696e  t will not be in
-00008fb0: 7374 616c 6c65 6420 7669 6120 506f 6574  stalled via Poet
-00008fc0: 7279 2062 7574 2069 7320 7573 6564 2066  ry but is used f
-00008fd0: 6f72 2074 6573 7469 6e67 2061 6e64 2069  or testing and i
-00008fe0: 6e2d 646f 6375 6d65 6e74 6174 696f 6e20  n-documentation 
-00008ff0: 6578 616d 706c 6573 2069 7320 7468 6520  examples is the 
-00009000: 7370 6143 7920 6d65 6469 756d 2045 6e67  spaCy medium Eng
-00009010: 6c69 7368 206d 6f64 656c 2028 6065 6e2d  lish model (`en-
-00009020: 636f 7265 2d77 6562 2d6d 6460 292e 2054  core-web-md`). T
-00009030: 6869 7320 7769 6c6c 206e 6565 6420 746f  his will need to
-00009040: 2062 6520 696e 7374 616c 6c65 6420 7365   be installed se
-00009050: 7061 7261 7465 6c79 2e20 5468 6520 636f  parately. The co
-00009060: 6d6d 616e 6420 6265 6c6f 7720 7368 6f75  mmand below shou
-00009070: 6c64 2064 6f20 7468 6520 7472 6963 6b3a  ld do the trick:
-00009080: 5c6e 5c6e 5c6e 6060 6070 7974 686f 6e5c  \n\n\n```python\
-00009090: 6e70 6f65 7472 7920 7275 6e20 7079 7468  npoetry run pyth
-000090a0: 6f6e 202d 6d20 7370 6163 7920 646f 776e  on -m spacy down
-000090b0: 6c6f 6164 2022 656e 5f63 6f72 655f 7765  load "en_core_we
-000090c0: 625f 6d64 225c 6e60 6060 5c6e 5c6e 2323  b_md"\n```\n\n##
-000090d0: 2052 6566 6572 656e 6365 735c 6e5c 6e2d   References\n\n-
-000090e0: 2053 7061 637a 7a20 7472 6965 7320 746f   Spaczz tries to
-000090f0: 2073 7461 7920 6173 2063 6c6f 7365 2074   stay as close t
-00009100: 6f20 5b73 7061 4379 5d28 6874 7470 733a  o [spaCy](https:
-00009110: 2f2f 7370 6163 792e 696f 2f29 5c27 7320  //spacy.io/)\'s 
-00009120: 4150 4920 6173 2070 6f73 7369 626c 652e  API as possible.
-00009130: 2057 6865 6e65 7665 7220 6974 206d 6164   Whenever it mad
-00009140: 6520 7365 6e73 6520 746f 2075 7365 2065  e sense to use e
-00009150: 7869 7374 696e 6720 7370 6143 7920 636f  xisting spaCy co
-00009160: 6465 2077 6974 6869 6e20 7370 6163 7a7a  de within spaczz
-00009170: 2074 6869 7320 7761 7320 646f 6e65 2e5c   this was done.\
-00009180: 6e2d 2046 757a 7a79 206d 6174 6368 696e  n- Fuzzy matchin
-00009190: 6720 6973 2070 6572 666f 726d 6564 2075  g is performed u
-000091a0: 7369 6e67 205b 5261 7069 6446 757a 7a5d  sing [RapidFuzz]
-000091b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000091c0: 636f 6d2f 6d61 7862 6163 686d 616e 6e2f  com/maxbachmann/
-000091d0: 7261 7069 6466 757a 7a29 2e5c 6e2d 2052  rapidfuzz).\n- R
-000091e0: 6567 6578 6573 2061 7265 2070 6572 666f  egexes are perfo
-000091f0: 726d 6564 2075 7369 6e67 2074 6865 205b  rmed using the [
-00009200: 7265 6765 785d 2868 7474 7073 3a2f 2f70  regex](https://p
-00009210: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00009220: 7265 6765 782f 2920 6c69 6272 6172 792e  regex/) library.
-00009230: 5c6e 2d20 5468 6520 7365 6172 6368 2061  \n- The search a
-00009240: 6c67 6f72 6974 686d 2066 6f72 2070 6872  lgorithm for phr
-00009250: 6173 6564 2d62 6173 6564 2066 757a 7a79  ased-based fuzzy
-00009260: 2061 6e64 2073 696d 696c 6172 6974 7920   and similarity 
-00009270: 6d61 7463 6869 6e67 2077 6173 2068 6561  matching was hea
-00009280: 7669 6c79 2069 6e66 6c75 6e63 6564 2062  vily influnced b
-00009290: 7920 5374 6163 6b20 4f76 6572 666c 6f77  y Stack Overflow
-000092a0: 2075 7365 7220 556c 6620 4173 6c61 6b5c   user Ulf Aslak\
-000092b0: 2773 2061 6e73 7765 7220 696e 2074 6869  's answer in thi
-000092c0: 7320 5b74 6872 6561 645d 2868 7474 7073  s [thread](https
-000092d0: 3a2f 2f73 7461 636b 6f76 6572 666c 6f77  ://stackoverflow
-000092e0: 2e63 6f6d 2f71 7565 7374 696f 6e73 2f33  .com/questions/3
-000092f0: 3630 3133 3239 352f 6669 6e64 2d62 6573  6013295/find-bes
-00009300: 742d 7375 6273 7472 696e 672d 6d61 7463  t-substring-matc
-00009310: 6829 2e5c 6e2d 2053 7061 637a 7a5c 2773  h).\n- Spaczz\'s
-00009320: 2070 7265 6465 6669 6e65 6420 7265 6765   predefined rege
-00009330: 7820 7061 7474 6572 6e73 2077 6572 6520  x patterns were 
-00009340: 626f 7272 6f77 6564 2066 726f 6d20 7468  borrowed from th
-00009350: 6520 5b63 6f6d 6d6f 6e72 6567 6578 5d28  e [commonregex](
-00009360: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00009370: 6f6d 2f6d 6164 6973 6f6e 6d61 792f 436f  om/madisonmay/Co
-00009380: 6d6d 6f6e 5265 6765 7829 2070 6163 6b61  mmonRegex) packa
-00009390: 6765 2e5c 6e2d 2053 7061 637a 7a5c 2773  ge.\n- Spaczz\'s
-000093a0: 2064 6576 656c 6f70 6d65 6e74 2061 6e64   development and
-000093b0: 2043 492f 4344 2070 6174 7465 726e 7320   CI/CD patterns 
-000093c0: 7765 7265 2069 6e73 7069 7265 6420 6279  were inspired by
-000093d0: 2043 6c61 7564 696f 204a 6f6c 6f77 6963   Claudio Jolowic
-000093e0: 7a5c 2773 205b 2a48 7970 6572 6d6f 6465  z\'s [*Hypermode
-000093f0: 726e 2050 7974 686f 6e2a 5d28 6874 7470  rn Python*](http
-00009400: 733a 2f2f 636a 6f6c 6f77 6963 7a2e 6769  s://cjolowicz.gi
-00009410: 7468 7562 2e69 6f2f 706f 7374 732f 6879  thub.io/posts/hy
-00009420: 7065 726d 6f64 6572 6e2d 7079 7468 6f6e  permodern-python
-00009430: 2d30 312d 7365 7475 702f 2920 6172 7469  -01-setup/) arti
-00009440: 636c 6520 7365 7269 6573 2e5c 6e27 2c0a  cle series.\n',.
-00009450: 2020 2020 2761 7574 686f 7227 3a20 2747      'author': 'G
-00009460: 7261 6e74 2041 6e64 6572 7365 6e27 2c0a  rant Andersen',.
-00009470: 2020 2020 2761 7574 686f 725f 656d 6169      'author_emai
-00009480: 6c27 3a20 2767 616e 6465 7273 656e 2e63  l': 'gandersen.c
-00009490: 6f64 6573 4067 6d61 696c 2e63 6f6d 272c  odes@gmail.com',
-000094a0: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-000094b0: 273a 204e 6f6e 652c 0a20 2020 2027 6d61  ': None,.    'ma
-000094c0: 696e 7461 696e 6572 5f65 6d61 696c 273a  intainer_email':
-000094d0: 204e 6f6e 652c 0a20 2020 2027 7572 6c27   None,.    'url'
-000094e0: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-000094f0: 622e 636f 6d2f 6761 6e64 6572 7365 6e31  b.com/gandersen1
-00009500: 3031 2f73 7061 637a 7a27 2c0a 2020 2020  01/spaczz',.    
-00009510: 2770 6163 6b61 6765 5f64 6972 273a 2070  'package_dir': p
-00009520: 6163 6b61 6765 5f64 6972 2c0a 2020 2020  ackage_dir,.    
-00009530: 2770 6163 6b61 6765 7327 3a20 7061 636b  'packages': pack
-00009540: 6167 6573 2c0a 2020 2020 2770 6163 6b61  ages,.    'packa
-00009550: 6765 5f64 6174 6127 3a20 7061 636b 6167  ge_data': packag
-00009560: 655f 6461 7461 2c0a 2020 2020 2769 6e73  e_data,.    'ins
-00009570: 7461 6c6c 5f72 6571 7569 7265 7327 3a20  tall_requires': 
-00009580: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00009590: 2c0a 2020 2020 2765 7874 7261 735f 7265  ,.    'extras_re
-000095a0: 7175 6972 6527 3a20 6578 7472 6173 5f72  quire': extras_r
-000095b0: 6571 7569 7265 2c0a 2020 2020 2765 6e74  equire,.    'ent
-000095c0: 7279 5f70 6f69 6e74 7327 3a20 656e 7472  ry_points': entr
-000095d0: 795f 706f 696e 7473 2c0a 2020 2020 2770  y_points,.    'p
-000095e0: 7974 686f 6e5f 7265 7175 6972 6573 273a  ython_requires':
-000095f0: 2027 3e3d 332e 372c 3c34 2e30 272c 0a7d   '>=3.7,<4.0',.}
-00009600: 0a0a 0a73 6574 7570 282a 2a73 6574 7570  ...setup(**setup
-00009610: 5f6b 7761 7267 7329 0a                   _kwargs).
+000087c0: 656e 6861 6e63 656d 656e 7473 2e0a 312e  enhancements..1.
+000087d0: 2042 7569 6c64 696e 6720 6f75 7420 5265   Building out Re
+000087e0: 6164 2074 6865 2044 6f63 732e 0a31 2e20  ad the Docs..1. 
+000087f0: 4f70 7469 6f6e 2074 6f20 7072 696f 7269  Option to priori
+00008800: 7469 7a65 206d 6174 6368 2071 7561 6c69  tize match quali
+00008810: 7479 206f 7665 7220 6c65 6e67 7468 2061  ty over length a
+00008820: 6e64 2f6f 7220 7765 6967 6869 6e67 206f  nd/or weighing o
+00008830: 7074 696f 6e73 2e0a 312e 2050 726f 6669  ptions..1. Profi
+00008840: 6c69 6e67 202d 2068 6f70 6566 756c 6c79  ling - hopefully
+00008850: 2074 6f20 6669 6e64 2022 6561 7379 2220   to find "easy" 
+00008860: 7065 7266 6f72 6d61 6e63 6520 6f70 7469  performance opti
+00008870: 6d69 7a61 7469 6f6e 732e 0a0a 2a2a 456e  mizations...**En
+00008880: 6861 6e63 656d 656e 7473 2a2a 0a0a 312e  hancements**..1.
+00008890: 2048 6176 696e 6720 7370 6163 7a7a 206d   Having spaczz m
+000088a0: 6174 6368 6572 7320 7574 696c 697a 6520  atchers utilize 
+000088b0: 7370 6143 7920 766f 6361 6275 6c61 7269  spaCy vocabulari
+000088c0: 6573 2e0a 312e 2052 6577 7269 7465 2074  es..1. Rewrite t
+000088d0: 6865 2070 6872 6173 6520 616e 6420 746f  he phrase and to
+000088e0: 6b65 6e20 7365 6172 6368 696e 6720 616c  ken searching al
+000088f0: 676f 7269 7468 6d73 2069 6e20 4379 7468  gorithms in Cyth
+00008900: 6f6e 2074 6f20 7574 696c 697a 6520 4320  on to utilize C 
+00008910: 7370 6565 642e 0a20 2020 2031 2e20 5472  speed..    1. Tr
+00008920: 7920 746f 2069 6e74 6567 7261 7465 2063  y to integrate c
+00008930: 6c6f 7365 7220 7769 7468 2073 7061 4379  loser with spaCy
+00008940: 2e0a 0a23 2320 4465 7665 6c6f 706d 656e  ...## Developmen
+00008950: 740a 0a50 756c 6c20 7265 7175 6573 7473  t..Pull requests
+00008960: 2061 6e64 2063 6f6e 7472 6962 7574 6f72   and contributor
+00008970: 7320 6172 6520 7765 6c63 6f6d 652e 0a0a  s are welcome...
+00008980: 7370 6163 7a7a 2069 7320 6c69 6e74 6564  spaczz is linted
+00008990: 2077 6974 6820 5b46 6c61 6b65 385d 2868   with [Flake8](h
+000089a0: 7474 7073 3a2f 2f66 6c61 6b65 382e 7079  ttps://flake8.py
+000089b0: 6371 612e 6f72 672f 656e 2f6c 6174 6573  cqa.org/en/lates
+000089c0: 742f 292c 2066 6f72 6d61 7474 6564 2077  t/), formatted w
+000089d0: 6974 6820 5b42 6c61 636b 5d28 6874 7470  ith [Black](http
+000089e0: 733a 2f2f 626c 6163 6b2e 7265 6164 7468  s://black.readth
+000089f0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+00008a00: 6c65 2f29 2c20 7479 7065 2d63 6865 636b  le/), type-check
+00008a10: 6564 2077 6974 6820 5b4d 7950 795d 2868  ed with [MyPy](h
+00008a20: 7474 703a 2f2f 6d79 7079 2d6c 616e 672e  ttp://mypy-lang.
+00008a30: 6f72 672f 2920 2861 6c74 686f 7567 6820  org/) (although 
+00008a40: 7468 6973 2063 6f75 6c64 2062 656e 6566  this could benef
+00008a50: 6974 2066 726f 6d20 696d 7072 6f76 6564  it from improved
+00008a60: 2073 7065 6369 6669 6369 7479 292c 2074   specificity), t
+00008a70: 6573 7465 6420 7769 7468 205b 5079 7465  ested with [Pyte
+00008a80: 7374 5d28 6874 7470 733a 2f2f 646f 6373  st](https://docs
+00008a90: 2e70 7974 6573 742e 6f72 672f 656e 2f73  .pytest.org/en/s
+00008aa0: 7461 626c 652f 292c 2061 7574 6f6d 6174  table/), automat
+00008ab0: 6564 2077 6974 6820 5b4e 6f78 5d28 6874  ed with [Nox](ht
+00008ac0: 7470 733a 2f2f 6e6f 782e 7468 6561 2e63  tps://nox.thea.c
+00008ad0: 6f64 6573 2f65 6e2f 7374 6162 6c65 2f29  odes/en/stable/)
+00008ae0: 2c20 616e 6420 6275 696c 742f 7061 636b  , and built/pack
+00008af0: 6167 6564 2077 6974 6820 5b50 6f65 7472  aged with [Poetr
+00008b00: 795d 2868 7474 7073 3a2f 2f70 7974 686f  y](https://pytho
+00008b10: 6e2d 706f 6574 7279 2e6f 7267 2f29 2e20  n-poetry.org/). 
+00008b20: 5468 6572 6520 6172 6520 6120 6665 7720  There are a few 
+00008b30: 6f74 6865 7220 6465 7665 6c6f 706d 656e  other developmen
+00008b40: 7420 746f 6f6c 7320 6465 7461 696c 6564  t tools detailed
+00008b50: 2069 6e20 7468 6520 6e6f 7866 696c 652e   in the noxfile.
+00008b60: 7079 2c20 616c 6f6e 6720 7769 7468 2047  py, along with G
+00008b70: 6974 2070 7265 2d63 6f6d 6d69 7420 686f  it pre-commit ho
+00008b80: 6f6b 732e 0a0a 546f 2063 6f6e 7472 6962  oks...To contrib
+00008b90: 7574 6520 746f 2073 7061 637a 7a27 7320  ute to spaczz's 
+00008ba0: 6465 7665 6c6f 706d 656e 742c 2066 6f72  development, for
+00008bb0: 6b20 7468 6520 7265 706f 7369 746f 7279  k the repository
+00008bc0: 2074 6865 6e20 696e 7374 616c 6c20 7370   then install sp
+00008bd0: 6163 7a7a 2061 6e64 2069 7427 7320 6465  aczz and it's de
+00008be0: 7620 6465 7065 6e64 656e 6369 6573 2077  v dependencies w
+00008bf0: 6974 6820 506f 6574 7279 2e20 4966 2079  ith Poetry. If y
+00008c00: 6f75 2772 6520 696e 7465 7265 7374 6564  ou're interested
+00008c10: 2069 6e20 6265 696e 6720 6120 7265 6775   in being a regu
+00008c20: 6c61 7220 636f 6e74 7269 6275 746f 7220  lar contributor 
+00008c30: 706c 6561 7365 2063 6f6e 7461 6374 206d  please contact m
+00008c40: 6520 6469 7265 6374 6c79 2e0a 0a60 6060  e directly...```
+00008c50: 7079 7468 6f6e 0a70 6f65 7472 7920 696e  python.poetry in
+00008c60: 7374 616c 6c20 2320 5769 7468 696e 2073  stall # Within s
+00008c70: 7061 637a 7a27 7320 726f 6f74 2064 6972  paczz's root dir
+00008c80: 6563 746f 7279 2e0a 6060 600a 0a49 206b  ectory..```..I k
+00008c90: 6565 7020 4e6f 7820 616e 6420 7072 652d  eep Nox and pre-
+00008ca0: 636f 6d6d 6974 206f 7574 7369 6465 206f  commit outside o
+00008cb0: 6620 6d79 2070 6f65 7472 7920 656e 7669  f my poetry envi
+00008cc0: 726f 6e6d 656e 7420 6173 2070 6172 7420  ronment as part 
+00008cd0: 6f66 206d 7920 5079 7468 6f6e 2074 6f6f  of my Python too
+00008ce0: 6c63 6861 696e 2065 6e76 6972 6f6e 6d65  lchain environme
+00008cf0: 6e74 732e 2057 6974 6820 7072 652d 636f  nts. With pre-co
+00008d00: 6d6d 6974 2069 6e73 7461 6c6c 6564 2079  mmit installed y
+00008d10: 6f75 206d 6179 2061 6c73 6f20 6e65 6564  ou may also need
+00008d20: 2074 6f20 7275 6e20 7468 6520 6265 6c6f   to run the belo
+00008d30: 7720 746f 2063 6f6d 6d69 7420 6368 616e  w to commit chan
+00008d40: 6765 732e 0a0a 6060 6070 7974 686f 6e0a  ges...```python.
+00008d50: 7072 652d 636f 6d6d 6974 2069 6e73 7461  pre-commit insta
+00008d60: 6c6c 0a60 6060 0a0a 5468 6520 6f6e 6c79  ll.```..The only
+00008d70: 206f 7468 6572 2070 6163 6b61 6765 2074   other package t
+00008d80: 6861 7420 7769 6c6c 206e 6f74 2062 6520  hat will not be 
+00008d90: 696e 7374 616c 6c65 6420 7669 6120 506f  installed via Po
+00008da0: 6574 7279 2062 7574 2069 7320 7573 6564  etry but is used
+00008db0: 2066 6f72 2074 6573 7469 6e67 2061 6e64   for testing and
+00008dc0: 2069 6e2d 646f 6375 6d65 6e74 6174 696f   in-documentatio
+00008dd0: 6e20 6578 616d 706c 6573 2069 7320 7468  n examples is th
+00008de0: 6520 7370 6143 7920 6d65 6469 756d 2045  e spaCy medium E
+00008df0: 6e67 6c69 7368 206d 6f64 656c 2028 6065  nglish model (`e
+00008e00: 6e2d 636f 7265 2d77 6562 2d6d 6460 292e  n-core-web-md`).
+00008e10: 2054 6869 7320 7769 6c6c 206e 6565 6420   This will need 
+00008e20: 746f 2062 6520 696e 7374 616c 6c65 6420  to be installed 
+00008e30: 7365 7061 7261 7465 6c79 2e20 5468 6520  separately. The 
+00008e40: 636f 6d6d 616e 6420 6265 6c6f 7720 7368  command below sh
+00008e50: 6f75 6c64 2064 6f20 7468 6520 7472 6963  ould do the tric
+00008e60: 6b3a 0a0a 6060 6070 7974 686f 6e0a 706f  k:..```python.po
+00008e70: 6574 7279 2072 756e 2070 7974 686f 6e20  etry run python 
+00008e80: 2d6d 2073 7061 6379 2064 6f77 6e6c 6f61  -m spacy downloa
+00008e90: 6420 2265 6e5f 636f 7265 5f77 6562 5f6d  d "en_core_web_m
+00008ea0: 6422 0a60 6060 0a0a 2323 2052 6566 6572  d".```..## Refer
+00008eb0: 656e 6365 730a 0a2d 2073 7061 637a 7a20  ences..- spaczz 
+00008ec0: 7472 6965 7320 746f 2073 7461 7920 6173  tries to stay as
+00008ed0: 2063 6c6f 7365 2074 6f20 5b73 7061 4379   close to [spaCy
+00008ee0: 5d28 6874 7470 733a 2f2f 7370 6163 792e  ](https://spacy.
+00008ef0: 696f 2f29 2773 2041 5049 2061 7320 706f  io/)'s API as po
+00008f00: 7373 6962 6c65 2e20 5768 656e 6576 6572  ssible. Whenever
+00008f10: 2069 7420 6d61 6465 2073 656e 7365 2074   it made sense t
+00008f20: 6f20 7573 6520 6578 6973 7469 6e67 2073  o use existing s
+00008f30: 7061 4379 2063 6f64 6520 7769 7468 696e  paCy code within
+00008f40: 2073 7061 637a 7a20 7468 6973 2077 6173   spaczz this was
+00008f50: 2064 6f6e 652e 0a2d 2046 757a 7a79 206d   done..- Fuzzy m
+00008f60: 6174 6368 696e 6720 6973 2070 6572 666f  atching is perfo
+00008f70: 726d 6564 2075 7369 6e67 205b 5261 7069  rmed using [Rapi
+00008f80: 6446 757a 7a5d 2868 7474 7073 3a2f 2f67  dFuzz](https://g
+00008f90: 6974 6875 622e 636f 6d2f 6d61 7862 6163  ithub.com/maxbac
+00008fa0: 686d 616e 6e2f 7261 7069 6466 757a 7a29  hmann/rapidfuzz)
+00008fb0: 2e0a 2d20 5265 6765 7865 7320 6172 6520  ..- Regexes are 
+00008fc0: 7065 7266 6f72 6d65 6420 7573 696e 6720  performed using 
+00008fd0: 7468 6520 5b72 6567 6578 5d28 6874 7470  the [regex](http
+00008fe0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00008ff0: 6a65 6374 2f72 6567 6578 2f29 206c 6962  ject/regex/) lib
+00009000: 7261 7279 2e0a 2d20 5468 6520 7365 6172  rary..- The sear
+00009010: 6368 2061 6c67 6f72 6974 686d 2066 6f72  ch algorithm for
+00009020: 2070 6872 6173 6564 2d62 6173 6564 2066   phrased-based f
+00009030: 757a 7a79 2061 6e64 2073 696d 696c 6172  uzzy and similar
+00009040: 6974 7920 6d61 7463 6869 6e67 2077 6173  ity matching was
+00009050: 2068 6561 7669 6c79 2069 6e66 6c75 6e63   heavily influnc
+00009060: 6564 2062 7920 5374 6163 6b20 4f76 6572  ed by Stack Over
+00009070: 666c 6f77 2075 7365 7220 556c 6620 4173  flow user Ulf As
+00009080: 6c61 6b27 7320 616e 7377 6572 2069 6e20  lak's answer in 
+00009090: 7468 6973 205b 7468 7265 6164 5d28 6874  this [thread](ht
+000090a0: 7470 733a 2f2f 7374 6163 6b6f 7665 7266  tps://stackoverf
+000090b0: 6c6f 772e 636f 6d2f 7175 6573 7469 6f6e  low.com/question
+000090c0: 732f 3336 3031 3332 3935 2f66 696e 642d  s/36013295/find-
+000090d0: 6265 7374 2d73 7562 7374 7269 6e67 2d6d  best-substring-m
+000090e0: 6174 6368 292e 0a2d 2073 7061 637a 7a27  atch)..- spaczz'
+000090f0: 7320 7072 6564 6566 696e 6564 2072 6567  s predefined reg
+00009100: 6578 2070 6174 7465 726e 7320 7765 7265  ex patterns were
+00009110: 2062 6f72 726f 7765 6420 6672 6f6d 2074   borrowed from t
+00009120: 6865 205b 636f 6d6d 6f6e 7265 6765 785d  he [commonregex]
+00009130: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00009140: 636f 6d2f 6d61 6469 736f 6e6d 6179 2f43  com/madisonmay/C
+00009150: 6f6d 6d6f 6e52 6567 6578 2920 7061 636b  ommonRegex) pack
+00009160: 6167 652e 0a2d 2073 7061 637a 7a27 7320  age..- spaczz's 
+00009170: 6465 7665 6c6f 706d 656e 7420 616e 6420  development and 
+00009180: 4349 2f43 4420 7061 7474 6572 6e73 2077  CI/CD patterns w
+00009190: 6572 6520 696e 7370 6972 6564 2062 7920  ere inspired by 
+000091a0: 436c 6175 6469 6f20 4a6f 6c6f 7769 637a  Claudio Jolowicz
+000091b0: 2773 205b 2a48 7970 6572 6d6f 6465 726e  's [*Hypermodern
+000091c0: 2050 7974 686f 6e2a 5d28 6874 7470 733a   Python*](https:
+000091d0: 2f2f 636a 6f6c 6f77 6963 7a2e 6769 7468  //cjolowicz.gith
+000091e0: 7562 2e69 6f2f 706f 7374 732f 6879 7065  ub.io/posts/hype
+000091f0: 726d 6f64 6572 6e2d 7079 7468 6f6e 2d30  rmodern-python-0
+00009200: 312d 7365 7475 702f 2920 6172 7469 636c  1-setup/) articl
+00009210: 6520 7365 7269 6573 2e0a 0a              e series...
```

