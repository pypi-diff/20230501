# Comparing `tmp/PyQt6_QScintilla-2.13.4.tar.gz` & `tmp/PyQt6_QScintilla-2.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_QScintilla-2.13.4.tar", last modified: Sun Jan 15 18:13:46 2023, max compression
+gzip compressed data, was "PyQt6_QScintilla-2.14.0.tar", last modified: Thu Apr 27 16:09:49 2023, max compression
```

## Comparing `PyQt6_QScintilla-2.13.4.tar` & `PyQt6_QScintilla-2.14.0.tar`

### file list

```diff
@@ -1,430 +1,451 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.165274 PyQt6_QScintilla-2.13.4/
--rw-r--r--   0 phil       (501) staff       (20)   240098 2023-01-15 18:13:45.212464 PyQt6_QScintilla-2.13.4/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-01-15 18:13:44.325130 PyQt6_QScintilla-2.13.4/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)    27846 2023-01-15 17:58:20.417585 PyQt6_QScintilla-2.13.4/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1911 2023-01-15 18:13:46.165391 PyQt6_QScintilla-2.13.4/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1564 2023-01-15 18:13:45.440194 PyQt6_QScintilla-2.13.4/README
--rw-r--r--   0 phil       (501) staff       (20)     7485 2023-01-15 18:13:45.474804 PyQt6_QScintilla-2.13.4/project.py
--rw-r--r--   0 phil       (501) staff       (20)      553 2023-01-15 18:13:45.439719 PyQt6_QScintilla-2.13.4/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.113292 PyQt6_QScintilla-2.13.4/qsci/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.113343 PyQt6_QScintilla-2.13.4/qsci/api/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.119413 PyQt6_QScintilla-2.13.4/qsci/api/python/
--rw-r--r--   0 phil       (501) staff       (20)   172772 2023-01-15 17:58:19.862833 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.4.api
--rw-r--r--   0 phil       (501) staff       (20)   199839 2023-01-15 17:58:19.862648 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.5.api
--rw-r--r--   0 phil       (501) staff       (20)   191764 2023-01-15 17:58:19.863017 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.6.api
--rw-r--r--   0 phil       (501) staff       (20)   192152 2023-01-15 17:58:19.871169 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.7.api
--rw-r--r--   0 phil       (501) staff       (20)   175453 2023-01-15 17:58:19.864737 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.1.api
--rw-r--r--   0 phil       (501) staff       (20)   233448 2023-01-15 17:58:20.424322 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.10.api
--rw-r--r--   0 phil       (501) staff       (20)   243538 2023-01-15 17:58:20.427384 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.11.api
--rw-r--r--   0 phil       (501) staff       (20)   156049 2023-01-15 17:58:19.864151 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.2.api
--rw-r--r--   0 phil       (501) staff       (20)   254493 2023-01-15 17:58:19.872206 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.3.api
--rw-r--r--   0 phil       (501) staff       (20)   246543 2023-01-15 17:58:19.881223 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.4.api
--rw-r--r--   0 phil       (501) staff       (20)   238049 2023-01-15 17:58:19.867051 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.5.api
--rw-r--r--   0 phil       (501) staff       (20)   234256 2023-01-15 17:58:19.879612 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.6.api
--rw-r--r--   0 phil       (501) staff       (20)   233756 2023-01-15 17:58:19.870914 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.7.api
--rw-r--r--   0 phil       (501) staff       (20)   235810 2023-01-15 17:58:20.430016 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.8.api
--rw-r--r--   0 phil       (501) staff       (20)   227832 2023-01-15 17:58:20.433097 PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.9.api
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.068217 PyQt6_QScintilla-2.13.4/scintilla/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.058095 PyQt6_QScintilla-2.13.4/scintilla/include/
--rw-r--r--   0 phil       (501) staff       (20)     4124 2023-01-15 17:58:19.834536 PyQt6_QScintilla-2.13.4/scintilla/include/ILexer.h
--rw-r--r--   0 phil       (501) staff       (20)      607 2023-01-15 17:58:19.832960 PyQt6_QScintilla-2.13.4/scintilla/include/ILoader.h
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-01-15 17:58:19.801143 PyQt6_QScintilla-2.13.4/scintilla/include/License.txt
--rw-r--r--   0 phil       (501) staff       (20)    15732 2023-01-15 17:58:19.835575 PyQt6_QScintilla-2.13.4/scintilla/include/Platform.h
--rw-r--r--   0 phil       (501) staff       (20)    52975 2023-01-15 17:58:19.852696 PyQt6_QScintilla-2.13.4/scintilla/include/SciLexer.h
--rw-r--r--   0 phil       (501) staff       (20)      822 2023-01-15 17:58:19.838041 PyQt6_QScintilla-2.13.4/scintilla/include/Sci_Position.h
--rw-r--r--   0 phil       (501) staff       (20)    39252 2023-01-15 17:58:19.849765 PyQt6_QScintilla-2.13.4/scintilla/include/Scintilla.h
--rw-r--r--   0 phil       (501) staff       (20)   151936 2023-01-15 17:58:19.838756 PyQt6_QScintilla-2.13.4/scintilla/include/Scintilla.iface
--rw-r--r--   0 phil       (501) staff       (20)     2646 2023-01-15 17:58:19.834725 PyQt6_QScintilla-2.13.4/scintilla/include/ScintillaWidget.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.054585 PyQt6_QScintilla-2.13.4/scintilla/lexers/
--rw-r--r--   0 phil       (501) staff       (20)    12485 2023-01-15 17:58:19.833987 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexA68k.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7680 2023-01-15 17:58:19.829417 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAPDL.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7365 2023-01-15 17:58:19.831694 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexASY.cpp
--rw-r--r--   0 phil       (501) staff       (20)    29486 2023-01-15 17:58:19.840774 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAU3.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6762 2023-01-15 17:58:19.836433 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAVE.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8571 2023-01-15 17:58:19.835285 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAVS.cpp
--rw-r--r--   0 phil       (501) staff       (20)    19666 2023-01-15 17:58:19.838394 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAbaqus.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11716 2023-01-15 17:58:19.854552 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAda.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13719 2023-01-15 17:58:19.840177 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAsm.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5275 2023-01-15 17:58:19.851256 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAsn1.cpp
--rw-r--r--   0 phil       (501) staff       (20)    30635 2023-01-15 17:58:19.841256 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBaan.cpp
--rw-r--r--   0 phil       (501) staff       (20)    27588 2023-01-15 17:58:19.838030 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBash.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16591 2023-01-15 17:58:19.835784 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBasic.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17352 2023-01-15 17:58:19.831127 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBatch.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8737 2023-01-15 17:58:19.833840 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBibTeX.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6474 2023-01-15 17:58:19.842604 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBullant.cpp
--rw-r--r--   0 phil       (501) staff       (20)    22108 2023-01-15 17:58:19.838948 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCLW.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12466 2023-01-15 17:58:19.837620 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCOBOL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    58102 2023-01-15 17:58:19.842453 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCPP.cpp
--rw-r--r--   0 phil       (501) staff       (20)    18495 2023-01-15 17:58:19.856909 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCSS.cpp
--rw-r--r--   0 phil       (501) staff       (20)    14510 2023-01-15 17:58:19.842070 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCaml.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15711 2023-01-15 17:58:19.853772 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCmake.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16780 2023-01-15 17:58:19.843511 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCoffeeScript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5705 2023-01-15 17:58:19.840088 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexConf.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7221 2023-01-15 17:58:19.839134 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCrontab.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6336 2023-01-15 17:58:19.833383 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCsound.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16777 2023-01-15 17:58:19.835814 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexD.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9146 2023-01-15 17:58:19.844341 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexDMAP.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8358 2023-01-15 17:58:19.840636 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexDMIS.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6360 2023-01-15 17:58:19.839831 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexDiff.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15652 2023-01-15 17:58:19.844468 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexECL.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9531 2023-01-15 17:58:19.858631 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexEDIFACT.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8188 2023-01-15 17:58:19.843600 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexEScript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7601 2023-01-15 17:58:19.855765 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexEiffel.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16475 2023-01-15 17:58:19.845325 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexErlang.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13292 2023-01-15 17:58:19.842270 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexErrorList.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12296 2023-01-15 17:58:19.841857 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexFlagship.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5318 2023-01-15 17:58:19.835132 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexForth.cpp
--rw-r--r--   0 phil       (501) staff       (20)    24685 2023-01-15 17:58:19.839677 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexFortran.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6977 2023-01-15 17:58:19.846152 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexGAP.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8904 2023-01-15 17:58:19.842446 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexGui4Cli.cpp
--rw-r--r--   0 phil       (501) staff       (20)    81836 2023-01-15 17:58:19.843369 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexHTML.cpp
--rw-r--r--   0 phil       (501) staff       (20)    36346 2023-01-15 17:58:19.846935 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexHaskell.cpp
--rw-r--r--   0 phil       (501) staff       (20)    29024 2023-01-15 17:58:19.860779 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexHex.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2500 2023-01-15 17:58:19.845160 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexIndent.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8369 2023-01-15 17:58:19.857043 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexInno.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13704 2023-01-15 17:58:19.847351 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexJSON.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16299 2023-01-15 17:58:19.844175 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexKVIrc.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3747 2023-01-15 17:58:19.843157 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexKix.cpp
--rw-r--r--   0 phil       (501) staff       (20)    28943 2023-01-15 17:58:19.838759 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLPeg.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15494 2023-01-15 17:58:19.841398 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLaTeX.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8300 2023-01-15 17:58:19.848362 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLisp.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6042 2023-01-15 17:58:19.844033 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLout.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16099 2023-01-15 17:58:19.845375 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLua.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5444 2023-01-15 17:58:19.848733 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMMIXAL.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5257 2023-01-15 17:58:19.862394 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMPT.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11271 2023-01-15 17:58:19.846492 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMSSQL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13633 2023-01-15 17:58:19.858548 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMagik.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4391 2023-01-15 17:58:19.848725 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMake.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15564 2023-01-15 17:58:19.845923 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMarkdown.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12124 2023-01-15 17:58:19.844675 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMatlab.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4997 2023-01-15 17:58:19.840417 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMaxima.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10974 2023-01-15 17:58:19.843334 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMetapost.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16541 2023-01-15 17:58:19.850282 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexModula.cpp
--rw-r--r--   0 phil       (501) staff       (20)    18626 2023-01-15 17:58:19.846606 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMySQL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13810 2023-01-15 17:58:19.846800 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexNimrod.cpp
--rw-r--r--   0 phil       (501) staff       (20)    18818 2023-01-15 17:58:19.851074 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexNsis.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1098 2023-01-15 17:58:19.864089 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexNull.cpp
--rw-r--r--   0 phil       (501) staff       (20)    19685 2023-01-15 17:58:19.848453 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexOScript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9768 2023-01-15 17:58:19.860464 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexOpal.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12578 2023-01-15 17:58:19.850692 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPB.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5609 2023-01-15 17:58:19.847353 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPLM.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6620 2023-01-15 17:58:19.846070 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPO.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9536 2023-01-15 17:58:19.842295 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPOV.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12511 2023-01-15 17:58:19.844779 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPS.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20877 2023-01-15 17:58:19.853035 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPascal.cpp
--rw-r--r--   0 phil       (501) staff       (20)    57970 2023-01-15 17:58:19.850455 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPerl.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20435 2023-01-15 17:58:19.848995 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPowerPro.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7966 2023-01-15 17:58:19.853559 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPowerShell.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20629 2023-01-15 17:58:19.866086 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexProgress.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5518 2023-01-15 17:58:19.849919 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexProps.cpp
--rw-r--r--   0 phil       (501) staff       (20)    32996 2023-01-15 17:58:19.863310 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPython.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6264 2023-01-15 17:58:19.852375 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexR.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10729 2023-01-15 17:58:19.849327 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRebol.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11302 2023-01-15 17:58:19.848284 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRegistry.cpp
--rw-r--r--   0 phil       (501) staff       (20)    70986 2023-01-15 17:58:19.845886 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRuby.cpp
--rw-r--r--   0 phil       (501) staff       (20)    24817 2023-01-15 17:58:19.847352 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRust.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7803 2023-01-15 17:58:19.855313 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSAS.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5888 2023-01-15 17:58:19.852057 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSML.cpp
--rw-r--r--   0 phil       (501) staff       (20)    31189 2023-01-15 17:58:19.851465 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSQL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11010 2023-01-15 17:58:19.855800 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSTTXT.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11945 2023-01-15 17:58:19.867754 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexScriptol.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8980 2023-01-15 17:58:19.851619 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSmalltalk.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4744 2023-01-15 17:58:19.864472 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSorcus.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9048 2023-01-15 17:58:19.854971 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSpecman.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6085 2023-01-15 17:58:19.851323 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSpice.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7292 2023-01-15 17:58:19.850148 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexStata.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11159 2023-01-15 17:58:19.847684 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTACL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    37477 2023-01-15 17:58:19.851267 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTADS3.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11157 2023-01-15 17:58:19.857150 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTAL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11073 2023-01-15 17:58:19.854084 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTCL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16671 2023-01-15 17:58:19.853624 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTCMD.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13999 2023-01-15 17:58:19.857644 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTeX.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17089 2023-01-15 17:58:19.870046 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTxt2tags.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9851 2023-01-15 17:58:19.854959 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVB.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20499 2023-01-15 17:58:19.866004 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVHDL.cpp
--rw-r--r--   0 phil       (501) staff       (20)    35586 2023-01-15 17:58:19.857523 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVerilog.cpp
--rw-r--r--   0 phil       (501) staff       (20)    17725 2023-01-15 17:58:19.853544 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVisualProlog.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12465 2023-01-15 17:58:19.852126 PyQt6_QScintilla-2.13.4/scintilla/lexers/LexYAML.cpp
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-01-15 17:58:19.801143 PyQt6_QScintilla-2.13.4/scintilla/lexers/License.txt
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.067777 PyQt6_QScintilla-2.13.4/scintilla/lexlib/
--rw-r--r--   0 phil       (501) staff       (20)     2177 2023-01-15 17:58:19.850852 PyQt6_QScintilla-2.13.4/scintilla/lexlib/Accessor.cpp
--rw-r--r--   0 phil       (501) staff       (20)      829 2023-01-15 17:58:19.852961 PyQt6_QScintilla-2.13.4/scintilla/lexlib/Accessor.h
--rw-r--r--   0 phil       (501) staff       (20)    37773 2023-01-15 17:58:19.859597 PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterCategory.cpp
--rw-r--r--   0 phil       (501) staff       (20)      850 2023-01-15 17:58:19.855923 PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterCategory.h
--rw-r--r--   0 phil       (501) staff       (20)     1077 2023-01-15 17:58:19.855405 PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterSet.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4516 2023-01-15 17:58:19.858826 PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterSet.h
--rw-r--r--   0 phil       (501) staff       (20)     2820 2023-01-15 17:58:19.871410 PyQt6_QScintilla-2.13.4/scintilla/lexlib/DefaultLexer.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2336 2023-01-15 17:58:19.856462 PyQt6_QScintilla-2.13.4/scintilla/lexlib/DefaultLexer.h
--rw-r--r--   0 phil       (501) staff       (20)     5530 2023-01-15 17:58:19.868004 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexAccessor.h
--rw-r--r--   0 phil       (501) staff       (20)     3161 2023-01-15 17:58:19.858838 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerBase.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2261 2023-01-15 17:58:19.855771 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerBase.h
--rw-r--r--   0 phil       (501) staff       (20)     3025 2023-01-15 17:58:19.854411 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerModule.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2498 2023-01-15 17:58:19.852426 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerModule.h
--rw-r--r--   0 phil       (501) staff       (20)     1963 2023-01-15 17:58:19.854390 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerNoExceptions.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1135 2023-01-15 17:58:19.861715 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerNoExceptions.h
--rw-r--r--   0 phil       (501) staff       (20)     1494 2023-01-15 17:58:19.857324 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerSimple.cpp
--rw-r--r--   0 phil       (501) staff       (20)      809 2023-01-15 17:58:19.856837 PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerSimple.h
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-01-15 17:58:19.801143 PyQt6_QScintilla-2.13.4/scintilla/lexlib/License.txt
--rw-r--r--   0 phil       (501) staff       (20)     3453 2023-01-15 17:58:19.859888 PyQt6_QScintilla-2.13.4/scintilla/lexlib/OptionSet.h
--rw-r--r--   0 phil       (501) staff       (20)     4334 2023-01-15 17:58:19.872813 PyQt6_QScintilla-2.13.4/scintilla/lexlib/PropSetSimple.cpp
--rw-r--r--   0 phil       (501) staff       (20)      725 2023-01-15 17:58:19.857513 PyQt6_QScintilla-2.13.4/scintilla/lexlib/PropSetSimple.h
--rw-r--r--   0 phil       (501) staff       (20)     3003 2023-01-15 17:58:19.869463 PyQt6_QScintilla-2.13.4/scintilla/lexlib/SparseState.h
--rw-r--r--   0 phil       (501) staff       (20)      853 2023-01-15 17:58:19.859778 PyQt6_QScintilla-2.13.4/scintilla/lexlib/StringCopy.h
--rw-r--r--   0 phil       (501) staff       (20)     1550 2023-01-15 17:58:19.857030 PyQt6_QScintilla-2.13.4/scintilla/lexlib/StyleContext.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6026 2023-01-15 17:58:19.856117 PyQt6_QScintilla-2.13.4/scintilla/lexlib/StyleContext.h
--rw-r--r--   0 phil       (501) staff       (20)     4592 2023-01-15 17:58:19.854653 PyQt6_QScintilla-2.13.4/scintilla/lexlib/SubStyles.h
--rw-r--r--   0 phil       (501) staff       (20)     6887 2023-01-15 17:58:19.856249 PyQt6_QScintilla-2.13.4/scintilla/lexlib/WordList.cpp
--rw-r--r--   0 phil       (501) staff       (20)      965 2023-01-15 17:58:19.863192 PyQt6_QScintilla-2.13.4/scintilla/lexlib/WordList.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.092862 PyQt6_QScintilla-2.13.4/scintilla/src/
--rw-r--r--   0 phil       (501) staff       (20)     7326 2023-01-15 17:58:19.890769 PyQt6_QScintilla-2.13.4/scintilla/src/AutoComplete.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2786 2023-01-15 17:58:19.906299 PyQt6_QScintilla-2.13.4/scintilla/src/AutoComplete.h
--rw-r--r--   0 phil       (501) staff       (20)    11394 2023-01-15 17:58:19.897288 PyQt6_QScintilla-2.13.4/scintilla/src/CallTip.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2821 2023-01-15 17:58:19.894647 PyQt6_QScintilla-2.13.4/scintilla/src/CallTip.h
--rw-r--r--   0 phil       (501) staff       (20)    25198 2023-01-15 17:58:19.896474 PyQt6_QScintilla-2.13.4/scintilla/src/CaseConvert.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1601 2023-01-15 17:58:19.889894 PyQt6_QScintilla-2.13.4/scintilla/src/CaseConvert.h
--rw-r--r--   0 phil       (501) staff       (20)     1711 2023-01-15 17:58:19.893834 PyQt6_QScintilla-2.13.4/scintilla/src/CaseFolder.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1010 2023-01-15 17:58:19.908192 PyQt6_QScintilla-2.13.4/scintilla/src/CaseFolder.h
--rw-r--r--   0 phil       (501) staff       (20)     4777 2023-01-15 17:58:19.895204 PyQt6_QScintilla-2.13.4/scintilla/src/Catalogue.cpp
--rw-r--r--   0 phil       (501) staff       (20)      623 2023-01-15 17:58:19.904669 PyQt6_QScintilla-2.13.4/scintilla/src/Catalogue.h
--rw-r--r--   0 phil       (501) staff       (20)    36730 2023-01-15 17:58:19.904064 PyQt6_QScintilla-2.13.4/scintilla/src/CellBuffer.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7215 2023-01-15 17:58:19.911771 PyQt6_QScintilla-2.13.4/scintilla/src/CellBuffer.h
--rw-r--r--   0 phil       (501) staff       (20)     1588 2023-01-15 17:58:19.892929 PyQt6_QScintilla-2.13.4/scintilla/src/CharClassify.cpp
--rw-r--r--   0 phil       (501) staff       (20)      930 2023-01-15 17:58:19.907386 PyQt6_QScintilla-2.13.4/scintilla/src/CharClassify.h
--rw-r--r--   0 phil       (501) staff       (20)    11872 2023-01-15 17:58:19.899832 PyQt6_QScintilla-2.13.4/scintilla/src/ContractionState.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1694 2023-01-15 17:58:19.895866 PyQt6_QScintilla-2.13.4/scintilla/src/ContractionState.h
--rw-r--r--   0 phil       (501) staff       (20)     1107 2023-01-15 17:58:19.898094 PyQt6_QScintilla-2.13.4/scintilla/src/DBCS.cpp
--rw-r--r--   0 phil       (501) staff       (20)      397 2023-01-15 17:58:19.891666 PyQt6_QScintilla-2.13.4/scintilla/src/DBCS.h
--rw-r--r--   0 phil       (501) staff       (20)     9522 2023-01-15 17:58:19.895626 PyQt6_QScintilla-2.13.4/scintilla/src/Decoration.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2072 2023-01-15 17:58:19.909381 PyQt6_QScintilla-2.13.4/scintilla/src/Decoration.h
--rw-r--r--   0 phil       (501) staff       (20)    98470 2023-01-15 17:58:19.899143 PyQt6_QScintilla-2.13.4/scintilla/src/Document.cpp
--rw-r--r--   0 phil       (501) staff       (20)    21627 2023-01-15 17:58:19.907038 PyQt6_QScintilla-2.13.4/scintilla/src/Document.h
--rw-r--r--   0 phil       (501) staff       (20)     1867 2023-01-15 17:58:19.905374 PyQt6_QScintilla-2.13.4/scintilla/src/EditModel.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1486 2023-01-15 17:58:19.913244 PyQt6_QScintilla-2.13.4/scintilla/src/EditModel.h
--rw-r--r--   0 phil       (501) staff       (20)   101652 2023-01-15 17:58:20.440426 PyQt6_QScintilla-2.13.4/scintilla/src/EditView.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7923 2023-01-15 17:58:19.908850 PyQt6_QScintilla-2.13.4/scintilla/src/EditView.h
--rw-r--r--   0 phil       (501) staff       (20)   248617 2023-01-15 17:58:19.910461 PyQt6_QScintilla-2.13.4/scintilla/src/Editor.cpp
--rw-r--r--   0 phil       (501) staff       (20)    23032 2023-01-15 17:58:19.898031 PyQt6_QScintilla-2.13.4/scintilla/src/Editor.h
--rw-r--r--   0 phil       (501) staff       (20)      970 2023-01-15 17:58:19.899677 PyQt6_QScintilla-2.13.4/scintilla/src/ElapsedPeriod.h
--rw-r--r--   0 phil       (501) staff       (20)     3570 2023-01-15 17:58:19.893291 PyQt6_QScintilla-2.13.4/scintilla/src/ExternalLexer.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2094 2023-01-15 17:58:19.897260 PyQt6_QScintilla-2.13.4/scintilla/src/ExternalLexer.h
--rw-r--r--   0 phil       (501) staff       (20)      813 2023-01-15 17:58:19.910440 PyQt6_QScintilla-2.13.4/scintilla/src/FontQuality.h
--rw-r--r--   0 phil       (501) staff       (20)     7835 2023-01-15 17:58:19.901482 PyQt6_QScintilla-2.13.4/scintilla/src/Indicator.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1674 2023-01-15 17:58:19.908367 PyQt6_QScintilla-2.13.4/scintilla/src/Indicator.h
--rw-r--r--   0 phil       (501) staff       (20)      735 2023-01-15 17:58:19.906455 PyQt6_QScintilla-2.13.4/scintilla/src/IntegerRectangle.h
--rw-r--r--   0 phil       (501) staff       (20)     5434 2023-01-15 17:58:19.914592 PyQt6_QScintilla-2.13.4/scintilla/src/KeyMap.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1331 2023-01-15 17:58:19.900301 PyQt6_QScintilla-2.13.4/scintilla/src/KeyMap.h
--rw-r--r--   0 phil       (501) staff       (20)      854 2023-01-15 17:58:19.801143 PyQt6_QScintilla-2.13.4/scintilla/src/License.txt
--rw-r--r--   0 phil       (501) staff       (20)    15402 2023-01-15 17:58:19.910637 PyQt6_QScintilla-2.13.4/scintilla/src/LineMarker.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1510 2023-01-15 17:58:19.911650 PyQt6_QScintilla-2.13.4/scintilla/src/LineMarker.h
--rw-r--r--   0 phil       (501) staff       (20)    16819 2023-01-15 17:58:19.901555 PyQt6_QScintilla-2.13.4/scintilla/src/MarginView.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1576 2023-01-15 17:58:19.901215 PyQt6_QScintilla-2.13.4/scintilla/src/MarginView.h
--rw-r--r--   0 phil       (501) staff       (20)     5803 2023-01-15 17:58:19.894973 PyQt6_QScintilla-2.13.4/scintilla/src/Partitioning.h
--rw-r--r--   0 phil       (501) staff       (20)    12933 2023-01-15 17:58:19.898958 PyQt6_QScintilla-2.13.4/scintilla/src/PerLine.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5100 2023-01-15 17:58:19.911455 PyQt6_QScintilla-2.13.4/scintilla/src/PerLine.h
--rw-r--r--   0 phil       (501) staff       (20)      827 2023-01-15 17:58:19.902910 PyQt6_QScintilla-2.13.4/scintilla/src/Position.h
--rw-r--r--   0 phil       (501) staff       (20)    20501 2023-01-15 17:58:19.910377 PyQt6_QScintilla-2.13.4/scintilla/src/PositionCache.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7771 2023-01-15 17:58:19.908092 PyQt6_QScintilla-2.13.4/scintilla/src/PositionCache.h
--rw-r--r--   0 phil       (501) staff       (20)    26564 2023-01-15 17:58:19.916826 PyQt6_QScintilla-2.13.4/scintilla/src/RESearch.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1744 2023-01-15 17:58:19.901748 PyQt6_QScintilla-2.13.4/scintilla/src/RESearch.h
--rw-r--r--   0 phil       (501) staff       (20)     9604 2023-01-15 17:58:19.913539 PyQt6_QScintilla-2.13.4/scintilla/src/RunStyles.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2148 2023-01-15 17:58:19.912604 PyQt6_QScintilla-2.13.4/scintilla/src/RunStyles.h
--rw-r--r--   0 phil       (501) staff       (20)      305 2023-01-15 17:58:19.903399 PyQt6_QScintilla-2.13.4/scintilla/src/SciTE.properties
--rw-r--r--   0 phil       (501) staff       (20)    30781 2023-01-15 17:58:19.903636 PyQt6_QScintilla-2.13.4/scintilla/src/ScintillaBase.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3124 2023-01-15 17:58:19.896806 PyQt6_QScintilla-2.13.4/scintilla/src/ScintillaBase.h
--rw-r--r--   0 phil       (501) staff       (20)    10711 2023-01-15 17:58:19.901182 PyQt6_QScintilla-2.13.4/scintilla/src/Selection.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5757 2023-01-15 17:58:19.912543 PyQt6_QScintilla-2.13.4/scintilla/src/Selection.h
--rw-r--r--   0 phil       (501) staff       (20)     5323 2023-01-15 17:58:19.904300 PyQt6_QScintilla-2.13.4/scintilla/src/SparseVector.h
--rw-r--r--   0 phil       (501) staff       (20)    10129 2023-01-15 17:58:19.913409 PyQt6_QScintilla-2.13.4/scintilla/src/SplitVector.h
--rw-r--r--   0 phil       (501) staff       (20)     4388 2023-01-15 17:58:19.910043 PyQt6_QScintilla-2.13.4/scintilla/src/Style.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2412 2023-01-15 17:58:19.918378 PyQt6_QScintilla-2.13.4/scintilla/src/Style.h
--rw-r--r--   0 phil       (501) staff       (20)    10279 2023-01-15 17:58:19.903849 PyQt6_QScintilla-2.13.4/scintilla/src/UniConversion.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2825 2023-01-15 17:58:19.915012 PyQt6_QScintilla-2.13.4/scintilla/src/UniConversion.h
--rw-r--r--   0 phil       (501) staff       (20)      820 2023-01-15 17:58:19.914438 PyQt6_QScintilla-2.13.4/scintilla/src/UniqueString.h
--rw-r--r--   0 phil       (501) staff       (20)    19320 2023-01-15 17:58:19.905853 PyQt6_QScintilla-2.13.4/scintilla/src/ViewStyle.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6791 2023-01-15 17:58:19.905932 PyQt6_QScintilla-2.13.4/scintilla/src/ViewStyle.h
--rw-r--r--   0 phil       (501) staff       (20)    10701 2023-01-15 17:58:19.898875 PyQt6_QScintilla-2.13.4/scintilla/src/XPM.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3597 2023-01-15 17:58:19.902813 PyQt6_QScintilla-2.13.4/scintilla/src/XPM.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.112851 PyQt6_QScintilla-2.13.4/sip/
--rw-r--r--   0 phil       (501) staff       (20)     1525 2023-01-15 18:13:45.465741 PyQt6_QScintilla-2.13.4/sip/qsciabstractapis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2048 2023-01-15 18:13:45.459332 PyQt6_QScintilla-2.13.4/sip/qsciapis.sip
--rw-r--r--   0 phil       (501) staff       (20)     3643 2023-01-15 18:13:45.466507 PyQt6_QScintilla-2.13.4/sip/qscicommand.sip
--rw-r--r--   0 phil       (501) staff       (20)     1463 2023-01-15 18:13:45.458409 PyQt6_QScintilla-2.13.4/sip/qscicommandset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1085 2023-01-15 18:13:45.470950 PyQt6_QScintilla-2.13.4/sip/qscidocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     3663 2023-01-15 18:13:45.464095 PyQt6_QScintilla-2.13.4/sip/qscilexer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2089 2023-01-15 18:13:45.460616 PyQt6_QScintilla-2.13.4/sip/qscilexeravs.sip
--rw-r--r--   0 phil       (501) staff       (20)     2194 2023-01-15 18:13:45.472979 PyQt6_QScintilla-2.13.4/sip/qscilexerbash.sip
--rw-r--r--   0 phil       (501) staff       (20)     1712 2023-01-15 18:13:45.441861 PyQt6_QScintilla-2.13.4/sip/qscilexerbatch.sip
--rw-r--r--   0 phil       (501) staff       (20)     2000 2023-01-15 18:13:45.465455 PyQt6_QScintilla-2.13.4/sip/qscilexercmake.sip
--rw-r--r--   0 phil       (501) staff       (20)     2854 2023-01-15 18:13:45.458983 PyQt6_QScintilla-2.13.4/sip/qscilexercoffeescript.sip
--rw-r--r--   0 phil       (501) staff       (20)     4497 2023-01-15 18:13:45.454312 PyQt6_QScintilla-2.13.4/sip/qscilexercpp.sip
--rw-r--r--   0 phil       (501) staff       (20)     1448 2023-01-15 18:13:45.473535 PyQt6_QScintilla-2.13.4/sip/qscilexercsharp.sip
--rw-r--r--   0 phil       (501) staff       (20)     2568 2023-01-15 18:13:45.467090 PyQt6_QScintilla-2.13.4/sip/qscilexercss.sip
--rw-r--r--   0 phil       (501) staff       (20)     1460 2023-01-15 18:13:45.456532 PyQt6_QScintilla-2.13.4/sip/qscilexercustom.sip
--rw-r--r--   0 phil       (501) staff       (20)     2660 2023-01-15 18:13:45.459814 PyQt6_QScintilla-2.13.4/sip/qscilexerd.sip
--rw-r--r--   0 phil       (501) staff       (20)     1614 2023-01-15 18:13:45.464744 PyQt6_QScintilla-2.13.4/sip/qscilexerdiff.sip
--rw-r--r--   0 phil       (501) staff       (20)     1547 2023-01-15 18:13:45.467419 PyQt6_QScintilla-2.13.4/sip/qscilexeredifact.sip
--rw-r--r--   0 phil       (501) staff       (20)     1251 2023-01-15 18:13:45.454855 PyQt6_QScintilla-2.13.4/sip/qscilexerfortran.sip
--rw-r--r--   0 phil       (501) staff       (20)     2096 2023-01-15 18:13:45.472540 PyQt6_QScintilla-2.13.4/sip/qscilexerfortran77.sip
--rw-r--r--   0 phil       (501) staff       (20)     5292 2023-01-15 18:13:45.444099 PyQt6_QScintilla-2.13.4/sip/qscilexerhtml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1303 2023-01-15 18:13:45.443112 PyQt6_QScintilla-2.13.4/sip/qscilexeridl.sip
--rw-r--r--   0 phil       (501) staff       (20)     1226 2023-01-15 18:13:45.473245 PyQt6_QScintilla-2.13.4/sip/qscilexerjava.sip
--rw-r--r--   0 phil       (501) staff       (20)     1476 2023-01-15 18:13:45.454590 PyQt6_QScintilla-2.13.4/sip/qscilexerjavascript.sip
--rw-r--r--   0 phil       (501) staff       (20)     2161 2023-01-15 18:13:45.461485 PyQt6_QScintilla-2.13.4/sip/qscilexerjson.sip
--rw-r--r--   0 phil       (501) staff       (20)     2316 2023-01-15 18:13:45.444558 PyQt6_QScintilla-2.13.4/sip/qscilexerlua.sip
--rw-r--r--   0 phil       (501) staff       (20)     1630 2023-01-15 18:13:45.453237 PyQt6_QScintilla-2.13.4/sip/qscilexermakefile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1903 2023-01-15 18:13:45.471382 PyQt6_QScintilla-2.13.4/sip/qscilexermarkdown.sip
--rw-r--r--   0 phil       (501) staff       (20)     1588 2023-01-15 18:13:45.440987 PyQt6_QScintilla-2.13.4/sip/qscilexermatlab.sip
--rw-r--r--   0 phil       (501) staff       (20)     1274 2023-01-15 18:13:45.463559 PyQt6_QScintilla-2.13.4/sip/qscilexeroctave.sip
--rw-r--r--   0 phil       (501) staff       (20)     2574 2023-01-15 18:13:45.442715 PyQt6_QScintilla-2.13.4/sip/qscilexerpascal.sip
--rw-r--r--   0 phil       (501) staff       (20)     3226 2023-01-15 18:13:45.463272 PyQt6_QScintilla-2.13.4/sip/qscilexerperl.sip
--rw-r--r--   0 phil       (501) staff       (20)     2023 2023-01-15 18:13:45.456944 PyQt6_QScintilla-2.13.4/sip/qscilexerpo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2322 2023-01-15 18:13:45.452526 PyQt6_QScintilla-2.13.4/sip/qscilexerpostscript.sip
--rw-r--r--   0 phil       (501) staff       (20)     2335 2023-01-15 18:13:45.462518 PyQt6_QScintilla-2.13.4/sip/qscilexerpov.sip
--rw-r--r--   0 phil       (501) staff       (20)     1964 2023-01-15 18:13:45.452907 PyQt6_QScintilla-2.13.4/sip/qscilexerproperties.sip
--rw-r--r--   0 phil       (501) staff       (20)     3334 2023-01-15 18:13:45.455417 PyQt6_QScintilla-2.13.4/sip/qscilexerpython.sip
--rw-r--r--   0 phil       (501) staff       (20)     2660 2023-01-15 18:13:45.462053 PyQt6_QScintilla-2.13.4/sip/qscilexerruby.sip
--rw-r--r--   0 phil       (501) staff       (20)     1590 2023-01-15 18:13:45.472067 PyQt6_QScintilla-2.13.4/sip/qscilexerspice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2764 2023-01-15 18:13:45.457466 PyQt6_QScintilla-2.13.4/sip/qscilexersql.sip
--rw-r--r--   0 phil       (501) staff       (20)     2195 2023-01-15 18:13:45.458113 PyQt6_QScintilla-2.13.4/sip/qscilexertcl.sip
--rw-r--r--   0 phil       (501) staff       (20)     1935 2023-01-15 18:13:45.453609 PyQt6_QScintilla-2.13.4/sip/qscilexertex.sip
--rw-r--r--   0 phil       (501) staff       (20)     3027 2023-01-15 18:13:45.456241 PyQt6_QScintilla-2.13.4/sip/qscilexerverilog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2409 2023-01-15 18:13:45.461073 PyQt6_QScintilla-2.13.4/sip/qscilexervhdl.sip
--rw-r--r--   0 phil       (501) staff       (20)     1665 2023-01-15 18:13:45.460146 PyQt6_QScintilla-2.13.4/sip/qscilexerxml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1950 2023-01-15 18:13:45.442246 PyQt6_QScintilla-2.13.4/sip/qscilexeryaml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1381 2023-01-15 18:13:45.471694 PyQt6_QScintilla-2.13.4/sip/qscimacro.sip
--rw-r--r--   0 phil       (501) staff       (20)     1027 2023-01-15 18:13:45.455680 PyQt6_QScintilla-2.13.4/sip/qscimod5.sip
--rw-r--r--   0 phil       (501) staff       (20)     1027 2023-01-15 18:13:45.457662 PyQt6_QScintilla-2.13.4/sip/qscimod6.sip
--rw-r--r--   0 phil       (501) staff       (20)     3410 2023-01-15 18:13:45.441512 PyQt6_QScintilla-2.13.4/sip/qscimodcommon.sip
--rw-r--r--   0 phil       (501) staff       (20)     1656 2023-01-15 18:13:45.465050 PyQt6_QScintilla-2.13.4/sip/qsciprinter.sip
--rw-r--r--   0 phil       (501) staff       (20)    18318 2023-01-15 18:13:45.470209 PyQt6_QScintilla-2.13.4/sip/qsciscintilla.sip
--rw-r--r--   0 phil       (501) staff       (20)    43649 2023-01-15 18:13:45.452046 PyQt6_QScintilla-2.13.4/sip/qsciscintillabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-01-15 18:13:45.470693 PyQt6_QScintilla-2.13.4/sip/qscistyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     1169 2023-01-15 18:13:45.464353 PyQt6_QScintilla-2.13.4/sip/qscistyledtext.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.146576 PyQt6_QScintilla-2.13.4/src/
--rw-r--r--   0 phil       (501) staff       (20)     9925 2023-01-15 18:13:45.279007 PyQt6_QScintilla-2.13.4/src/InputMethod.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7215 2023-01-15 18:13:45.229681 PyQt6_QScintilla-2.13.4/src/ListBoxQt.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2639 2023-01-15 18:13:45.355883 PyQt6_QScintilla-2.13.4/src/ListBoxQt.h
--rw-r--r--   0 phil       (501) staff       (20)     2863 2023-01-15 18:13:45.330165 PyQt6_QScintilla-2.13.4/src/MacPasteboardMime.cpp
--rw-r--r--   0 phil       (501) staff       (20)    23192 2023-01-15 18:13:45.360647 PyQt6_QScintilla-2.13.4/src/PlatQt.cpp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.165042 PyQt6_QScintilla-2.13.4/src/Qsci/
--rw-r--r--   0 phil       (501) staff       (20)     3627 2023-01-15 18:13:45.411413 PyQt6_QScintilla-2.13.4/src/Qsci/qsciabstractapis.h
--rw-r--r--   0 phil       (501) staff       (20)     8302 2023-01-15 18:13:45.280261 PyQt6_QScintilla-2.13.4/src/Qsci/qsciapis.h
--rw-r--r--   0 phil       (501) staff       (20)    14883 2023-01-15 18:13:45.283941 PyQt6_QScintilla-2.13.4/src/Qsci/qscicommand.h
--rw-r--r--   0 phil       (501) staff       (20)     2811 2023-01-15 18:13:45.422887 PyQt6_QScintilla-2.13.4/src/Qsci/qscicommandset.h
--rw-r--r--   0 phil       (501) staff       (20)     1901 2023-01-15 18:13:45.254657 PyQt6_QScintilla-2.13.4/src/Qsci/qscidocument.h
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-01-15 18:13:45.396975 PyQt6_QScintilla-2.13.4/src/Qsci/qsciglobal.h
--rw-r--r--   0 phil       (501) staff       (20)    13065 2023-01-15 18:13:45.268063 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexer.h
--rw-r--r--   0 phil       (501) staff       (20)     5290 2023-01-15 18:13:45.397959 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeravs.h
--rw-r--r--   0 phil       (501) staff       (20)     4875 2023-01-15 18:13:45.235972 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerbash.h
--rw-r--r--   0 phil       (501) staff       (20)     3432 2023-01-15 18:13:45.333685 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerbatch.h
--rw-r--r--   0 phil       (501) staff       (20)     4744 2023-01-15 18:13:45.241027 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercmake.h
--rw-r--r--   0 phil       (501) staff       (20)     8627 2023-01-15 18:13:45.331659 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercoffeescript.h
--rw-r--r--   0 phil       (501) staff       (20)    13427 2023-01-15 18:13:45.286112 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercpp.h
--rw-r--r--   0 phil       (501) staff       (20)     2586 2023-01-15 18:13:45.262622 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercsharp.h
--rw-r--r--   0 phil       (501) staff       (20)     7687 2023-01-15 18:13:45.437540 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercss.h
--rw-r--r--   0 phil       (501) staff       (20)     3655 2023-01-15 18:13:45.254209 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercustom.h
--rw-r--r--   0 phil       (501) staff       (20)     7509 2023-01-15 18:13:45.430118 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerd.h
--rw-r--r--   0 phil       (501) staff       (20)     3001 2023-01-15 18:13:45.266096 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerdiff.h
--rw-r--r--   0 phil       (501) staff       (20)     2846 2023-01-15 18:13:45.276829 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeredifact.h
--rw-r--r--   0 phil       (501) staff       (20)     1968 2023-01-15 18:13:45.437966 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerfortran.h
--rw-r--r--   0 phil       (501) staff       (20)     5055 2023-01-15 18:13:45.294315 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerfortran77.h
--rw-r--r--   0 phil       (501) staff       (20)    14535 2023-01-15 18:13:45.329441 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerhtml.h
--rw-r--r--   0 phil       (501) staff       (20)     2158 2023-01-15 18:13:45.272519 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeridl.h
--rw-r--r--   0 phil       (501) staff       (20)     1791 2023-01-15 18:13:45.418969 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerjava.h
--rw-r--r--   0 phil       (501) staff       (20)     2711 2023-01-15 18:13:45.428159 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerjavascript.h
--rw-r--r--   0 phil       (501) staff       (20)     5543 2023-01-15 18:13:45.269793 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerjson.h
--rw-r--r--   0 phil       (501) staff       (20)     6049 2023-01-15 18:13:45.435340 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerlua.h
--rw-r--r--   0 phil       (501) staff       (20)     3127 2023-01-15 18:13:45.334360 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexermakefile.h
--rw-r--r--   0 phil       (501) staff       (20)     4181 2023-01-15 18:13:45.268874 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexermarkdown.h
--rw-r--r--   0 phil       (501) staff       (20)     3031 2023-01-15 18:13:45.355406 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexermatlab.h
--rw-r--r--   0 phil       (501) staff       (20)     1957 2023-01-15 18:13:45.310597 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeroctave.h
--rw-r--r--   0 phil       (501) staff       (20)     7197 2023-01-15 18:13:45.427344 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpascal.h
--rw-r--r--   0 phil       (501) staff       (20)     8811 2023-01-15 18:13:45.312986 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerperl.h
--rw-r--r--   0 phil       (501) staff       (20)     4776 2023-01-15 18:13:45.422293 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpo.h
--rw-r--r--   0 phil       (501) staff       (20)     5883 2023-01-15 18:13:45.291071 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpostscript.h
--rw-r--r--   0 phil       (501) staff       (20)     6188 2023-01-15 18:13:45.227749 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpov.h
--rw-r--r--   0 phil       (501) staff       (20)     4714 2023-01-15 18:13:45.324885 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerproperties.h
--rw-r--r--   0 phil       (501) staff       (20)    10679 2023-01-15 18:13:45.409389 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpython.h
--rw-r--r--   0 phil       (501) staff       (20)     6813 2023-01-15 18:13:45.321375 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerruby.h
--rw-r--r--   0 phil       (501) staff       (20)     3059 2023-01-15 18:13:45.277490 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerspice.h
--rw-r--r--   0 phil       (501) staff       (20)     8893 2023-01-15 18:13:45.317207 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexersql.h
--rw-r--r--   0 phil       (501) staff       (20)     5523 2023-01-15 18:13:45.252143 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexertcl.h
--rw-r--r--   0 phil       (501) staff       (20)     5076 2023-01-15 18:13:45.289918 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexertex.h
--rw-r--r--   0 phil       (501) staff       (20)     8086 2023-01-15 18:13:45.226590 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerverilog.h
--rw-r--r--   0 phil       (501) staff       (20)     6446 2023-01-15 18:13:45.332908 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexervhdl.h
--rw-r--r--   0 phil       (501) staff       (20)     3458 2023-01-15 18:13:45.396562 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerxml.h
--rw-r--r--   0 phil       (501) staff       (20)     4424 2023-01-15 18:13:45.237638 PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeryaml.h
--rw-r--r--   0 phil       (501) staff       (20)     2786 2023-01-15 18:13:45.354105 PyQt6_QScintilla-2.13.4/src/Qsci/qscimacro.h
--rw-r--r--   0 phil       (501) staff       (20)     4423 2023-01-15 18:13:45.335510 PyQt6_QScintilla-2.13.4/src/Qsci/qsciprinter.h
--rw-r--r--   0 phil       (501) staff       (20)    86598 2023-01-15 18:13:45.225114 PyQt6_QScintilla-2.13.4/src/Qsci/qsciscintilla.h
--rw-r--r--   0 phil       (501) staff       (20)    89972 2023-01-15 18:13:45.353468 PyQt6_QScintilla-2.13.4/src/Qsci/qsciscintillabase.h
--rw-r--r--   0 phil       (501) staff       (20)     6226 2023-01-15 18:13:45.401388 PyQt6_QScintilla-2.13.4/src/Qsci/qscistyle.h
--rw-r--r--   0 phil       (501) staff       (20)     1898 2023-01-15 18:13:45.418539 PyQt6_QScintilla-2.13.4/src/Qsci/qscistyledtext.h
--rw-r--r--   0 phil       (501) staff       (20)    22478 2023-01-15 18:13:45.392674 PyQt6_QScintilla-2.13.4/src/SciAccessibility.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4634 2023-01-15 18:13:45.236748 PyQt6_QScintilla-2.13.4/src/SciAccessibility.h
--rw-r--r--   0 phil       (501) staff       (20)     4754 2023-01-15 18:13:45.410829 PyQt6_QScintilla-2.13.4/src/SciClasses.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-01-15 18:13:45.407615 PyQt6_QScintilla-2.13.4/src/SciClasses.h
--rw-r--r--   0 phil       (501) staff       (20)    19373 2023-01-15 18:13:45.406928 PyQt6_QScintilla-2.13.4/src/ScintillaQt.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4225 2023-01-15 18:13:45.297308 PyQt6_QScintilla-2.13.4/src/ScintillaQt.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.145820 PyQt6_QScintilla-2.13.4/src/features/
--rw-r--r--   0 phil       (501) staff       (20)      534 2023-01-15 18:13:45.287886 PyQt6_QScintilla-2.13.4/src/features/qscintilla2.prf
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-01-15 18:13:46.146224 PyQt6_QScintilla-2.13.4/src/features_staticlib/
--rw-r--r--   0 phil       (501) staff       (20)      507 2023-01-15 18:13:45.411856 PyQt6_QScintilla-2.13.4/src/features_staticlib/qscintilla2.prf
--rw-r--r--   0 phil       (501) staff       (20)     1423 2023-01-15 18:13:45.409783 PyQt6_QScintilla-2.13.4/src/qsciabstractapis.cpp
--rw-r--r--   0 phil       (501) staff       (20)    24667 2023-01-15 18:13:45.248675 PyQt6_QScintilla-2.13.4/src/qsciapis.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3394 2023-01-15 18:13:45.363715 PyQt6_QScintilla-2.13.4/src/qscicommand.cpp
--rw-r--r--   0 phil       (501) staff       (20)    27482 2023-01-15 18:13:45.234874 PyQt6_QScintilla-2.13.4/src/qscicommandset.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3793 2023-01-15 18:13:45.388758 PyQt6_QScintilla-2.13.4/src/qscidocument.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16881 2023-01-15 18:13:45.434210 PyQt6_QScintilla-2.13.4/src/qscilexer.cpp
--rw-r--r--   0 phil       (501) staff       (20)    14533 2023-01-15 18:13:45.250941 PyQt6_QScintilla-2.13.4/src/qscilexeravs.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8166 2023-01-15 18:13:45.326682 PyQt6_QScintilla-2.13.4/src/qscilexerbash.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4490 2023-01-15 18:13:45.293417 PyQt6_QScintilla-2.13.4/src/qscilexerbatch.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8247 2023-01-15 18:13:45.403007 PyQt6_QScintilla-2.13.4/src/qscilexercmake.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10030 2023-01-15 18:13:45.240065 PyQt6_QScintilla-2.13.4/src/qscilexercoffeescript.cpp
--rw-r--r--   0 phil       (501) staff       (20)    20137 2023-01-15 18:13:45.276147 PyQt6_QScintilla-2.13.4/src/qscilexercpp.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3237 2023-01-15 18:13:45.354781 PyQt6_QScintilla-2.13.4/src/qscilexercsharp.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10573 2023-01-15 18:13:45.362877 PyQt6_QScintilla-2.13.4/src/qscilexercss.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2683 2023-01-15 18:13:45.258486 PyQt6_QScintilla-2.13.4/src/qscilexercustom.cpp
--rw-r--r--   0 phil       (501) staff       (20)    10175 2023-01-15 18:13:45.243421 PyQt6_QScintilla-2.13.4/src/qscilexerd.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3146 2023-01-15 18:13:45.436180 PyQt6_QScintilla-2.13.4/src/qscilexerdiff.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2815 2023-01-15 18:13:45.386860 PyQt6_QScintilla-2.13.4/src/qscilexeredifact.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4910 2023-01-15 18:13:45.281698 PyQt6_QScintilla-2.13.4/src/qscilexerfortran.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7062 2023-01-15 18:13:45.322939 PyQt6_QScintilla-2.13.4/src/qscilexerfortran77.cpp
--rw-r--r--   0 phil       (501) staff       (20)    30776 2023-01-15 18:13:45.308324 PyQt6_QScintilla-2.13.4/src/qscilexerhtml.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3629 2023-01-15 18:13:45.302286 PyQt6_QScintilla-2.13.4/src/qscilexeridl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1776 2023-01-15 18:13:45.334811 PyQt6_QScintilla-2.13.4/src/qscilexerjava.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3207 2023-01-15 18:13:45.280971 PyQt6_QScintilla-2.13.4/src/qscilexerjavascript.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6285 2023-01-15 18:13:45.413474 PyQt6_QScintilla-2.13.4/src/qscilexerjson.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8617 2023-01-15 18:13:45.310134 PyQt6_QScintilla-2.13.4/src/qscilexerlua.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3418 2023-01-15 18:13:45.311470 PyQt6_QScintilla-2.13.4/src/qscilexermakefile.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6253 2023-01-15 18:13:45.394254 PyQt6_QScintilla-2.13.4/src/qscilexermarkdown.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3405 2023-01-15 18:13:45.288953 PyQt6_QScintilla-2.13.4/src/qscilexermatlab.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1970 2023-01-15 18:13:45.428762 PyQt6_QScintilla-2.13.4/src/qscilexeroctave.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9835 2023-01-15 18:13:45.296455 PyQt6_QScintilla-2.13.4/src/qscilexerpascal.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15626 2023-01-15 18:13:45.426045 PyQt6_QScintilla-2.13.4/src/qscilexerperl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4596 2023-01-15 18:13:45.262118 PyQt6_QScintilla-2.13.4/src/qscilexerpo.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13559 2023-01-15 18:13:45.315730 PyQt6_QScintilla-2.13.4/src/qscilexerpostscript.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12918 2023-01-15 18:13:45.421235 PyQt6_QScintilla-2.13.4/src/qscilexerpov.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4689 2023-01-15 18:13:45.318305 PyQt6_QScintilla-2.13.4/src/qscilexerproperties.cpp
--rw-r--r--   0 phil       (501) staff       (20)    11799 2023-01-15 18:13:45.260959 PyQt6_QScintilla-2.13.4/src/qscilexerpython.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9035 2023-01-15 18:13:45.417991 PyQt6_QScintilla-2.13.4/src/qscilexerruby.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5256 2023-01-15 18:13:45.324032 PyQt6_QScintilla-2.13.4/src/qscilexerspice.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13713 2023-01-15 18:13:45.265446 PyQt6_QScintilla-2.13.4/src/qscilexersql.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13475 2023-01-15 18:13:45.271978 PyQt6_QScintilla-2.13.4/src/qscilexertcl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9867 2023-01-15 18:13:45.320134 PyQt6_QScintilla-2.13.4/src/qscilexertex.cpp
--rw-r--r--   0 phil       (501) staff       (20)    15610 2023-01-15 18:13:45.257741 PyQt6_QScintilla-2.13.4/src/qscilexerverilog.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9890 2023-01-15 18:13:45.415661 PyQt6_QScintilla-2.13.4/src/qscilexervhdl.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5283 2023-01-15 18:13:45.253547 PyQt6_QScintilla-2.13.4/src/qscilexerxml.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5531 2023-01-15 18:13:45.292363 PyQt6_QScintilla-2.13.4/src/qscilexeryaml.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7469 2023-01-15 18:13:45.395905 PyQt6_QScintilla-2.13.4/src/qscimacro.cpp
--rw-r--r--   0 phil       (501) staff       (20)    13920 2023-01-15 18:13:45.400231 PyQt6_QScintilla-2.13.4/src/qscintilla.pro
--rw-r--r--   0 phil       (501) staff       (20)    44424 2023-01-15 17:58:19.884372 PyQt6_QScintilla-2.13.4/src/qscintilla_cs.qm
--rw-r--r--   0 phil       (501) staff       (20)    79869 2023-01-15 17:58:19.887293 PyQt6_QScintilla-2.13.4/src/qscintilla_de.qm
--rw-r--r--   0 phil       (501) staff       (20)    81850 2023-01-15 17:58:19.897471 PyQt6_QScintilla-2.13.4/src/qscintilla_es.qm
--rw-r--r--   0 phil       (501) staff       (20)    53842 2023-01-15 17:58:19.886677 PyQt6_QScintilla-2.13.4/src/qscintilla_fr.qm
--rw-r--r--   0 phil       (501) staff       (20)    49459 2023-01-15 17:58:19.893320 PyQt6_QScintilla-2.13.4/src/qscintilla_pt_br.qm
--rw-r--r--   0 phil       (501) staff       (20)     5046 2023-01-15 18:13:45.439047 PyQt6_QScintilla-2.13.4/src/qsciprinter.cpp
--rw-r--r--   0 phil       (501) staff       (20)   113524 2023-01-15 18:13:45.386075 PyQt6_QScintilla-2.13.4/src/qsciscintilla.cpp
--rw-r--r--   0 phil       (501) staff       (20)    21788 2023-01-15 18:13:45.301631 PyQt6_QScintilla-2.13.4/src/qsciscintillabase.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5035 2023-01-15 18:13:45.387890 PyQt6_QScintilla-2.13.4/src/qscistyle.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1620 2023-01-15 18:13:45.430574 PyQt6_QScintilla-2.13.4/src/qscistyledtext.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.664997 PyQt6_QScintilla-2.14.0/
+-rw-r--r--   0 phil       (501) staff       (20)   243812 2023-04-27 16:09:48.659561 PyQt6_QScintilla-2.14.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-27 16:09:47.663220 PyQt6_QScintilla-2.14.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)    28049 2023-04-27 15:54:13.221252 PyQt6_QScintilla-2.14.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1911 2023-04-27 16:09:49.665136 PyQt6_QScintilla-2.14.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1564 2023-04-27 16:09:48.942340 PyQt6_QScintilla-2.14.0/README
+-rw-r--r--   0 phil       (501) staff       (20)     7485 2023-04-27 16:09:48.985963 PyQt6_QScintilla-2.14.0/project.py
+-rw-r--r--   0 phil       (501) staff       (20)      553 2023-04-27 16:09:48.941855 PyQt6_QScintilla-2.14.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.608302 PyQt6_QScintilla-2.14.0/qsci/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.608352 PyQt6_QScintilla-2.14.0/qsci/api/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.614210 PyQt6_QScintilla-2.14.0/qsci/api/python/
+-rw-r--r--   0 phil       (501) staff       (20)   172772 2023-04-27 15:54:13.263872 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.4.api
+-rw-r--r--   0 phil       (501) staff       (20)   199839 2023-04-27 15:54:13.263463 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.5.api
+-rw-r--r--   0 phil       (501) staff       (20)   191764 2023-04-27 15:54:13.259922 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.6.api
+-rw-r--r--   0 phil       (501) staff       (20)   192152 2023-04-27 15:54:13.262933 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.7.api
+-rw-r--r--   0 phil       (501) staff       (20)   175453 2023-04-27 15:54:13.262669 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.1.api
+-rw-r--r--   0 phil       (501) staff       (20)   233448 2023-04-27 15:54:13.263802 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.10.api
+-rw-r--r--   0 phil       (501) staff       (20)   243538 2023-04-27 15:54:13.263478 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.11.api
+-rw-r--r--   0 phil       (501) staff       (20)   156049 2023-04-27 15:54:13.263519 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.2.api
+-rw-r--r--   0 phil       (501) staff       (20)   254493 2023-04-27 15:54:13.278213 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.3.api
+-rw-r--r--   0 phil       (501) staff       (20)   246543 2023-04-27 15:54:13.263311 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.4.api
+-rw-r--r--   0 phil       (501) staff       (20)   238049 2023-04-27 15:54:13.275161 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.5.api
+-rw-r--r--   0 phil       (501) staff       (20)   234256 2023-04-27 15:54:13.269879 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.6.api
+-rw-r--r--   0 phil       (501) staff       (20)   233756 2023-04-27 15:54:13.269916 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.7.api
+-rw-r--r--   0 phil       (501) staff       (20)   235810 2023-04-27 15:54:13.269971 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.8.api
+-rw-r--r--   0 phil       (501) staff       (20)   227832 2023-04-27 15:54:13.266211 PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.9.api
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.562578 PyQt6_QScintilla-2.14.0/scintilla/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.552287 PyQt6_QScintilla-2.14.0/scintilla/include/
+-rw-r--r--   0 phil       (501) staff       (20)     4124 2023-04-27 15:54:13.238178 PyQt6_QScintilla-2.14.0/scintilla/include/ILexer.h
+-rw-r--r--   0 phil       (501) staff       (20)      607 2023-04-27 15:54:13.236543 PyQt6_QScintilla-2.14.0/scintilla/include/ILoader.h
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/include/License.txt
+-rw-r--r--   0 phil       (501) staff       (20)    15732 2023-04-27 15:54:13.238441 PyQt6_QScintilla-2.14.0/scintilla/include/Platform.h
+-rw-r--r--   0 phil       (501) staff       (20)    52975 2023-04-27 15:54:13.255597 PyQt6_QScintilla-2.14.0/scintilla/include/SciLexer.h
+-rw-r--r--   0 phil       (501) staff       (20)      822 2023-04-27 15:54:13.237904 PyQt6_QScintilla-2.14.0/scintilla/include/Sci_Position.h
+-rw-r--r--   0 phil       (501) staff       (20)    39252 2023-04-27 15:54:13.251609 PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.h
+-rw-r--r--   0 phil       (501) staff       (20)   151936 2023-04-27 15:54:13.246147 PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.iface
+-rw-r--r--   0 phil       (501) staff       (20)     2646 2023-04-27 15:54:13.242743 PyQt6_QScintilla-2.14.0/scintilla/include/ScintillaWidget.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.548966 PyQt6_QScintilla-2.14.0/scintilla/lexers/
+-rw-r--r--   0 phil       (501) staff       (20)    12485 2023-04-27 15:54:13.242410 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexA68k.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7680 2023-04-27 15:54:13.239503 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAPDL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7365 2023-04-27 15:54:13.239854 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexASY.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    29486 2023-04-27 15:54:13.241423 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAU3.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6762 2023-04-27 15:54:13.239403 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVE.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8571 2023-04-27 15:54:13.237915 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    19666 2023-04-27 15:54:13.240012 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAbaqus.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11716 2023-04-27 15:54:13.256846 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAda.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13719 2023-04-27 15:54:13.239256 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5275 2023-04-27 15:54:13.252788 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsn1.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    30635 2023-04-27 15:54:13.247915 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBaan.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    27588 2023-04-27 15:54:13.244645 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBash.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16591 2023-04-27 15:54:13.243983 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBasic.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17352 2023-04-27 15:54:13.240788 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBatch.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8737 2023-04-27 15:54:13.241023 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBibTeX.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6474 2023-04-27 15:54:13.242658 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBullant.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    22108 2023-04-27 15:54:13.240934 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCLW.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12466 2023-04-27 15:54:13.239317 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCOBOL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    58102 2023-04-27 15:54:13.243039 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCPP.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    18495 2023-04-27 15:54:13.257892 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCSS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    14510 2023-04-27 15:54:13.240688 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCaml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15711 2023-04-27 15:54:13.254063 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCmake.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16780 2023-04-27 15:54:13.249365 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCoffeeScript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5705 2023-04-27 15:54:13.245799 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexConf.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7221 2023-04-27 15:54:13.245325 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCrontab.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6336 2023-04-27 15:54:13.241978 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCsound.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16777 2023-04-27 15:54:13.242696 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexD.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9146 2023-04-27 15:54:13.244061 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMAP.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8358 2023-04-27 15:54:13.242147 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMIS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6360 2023-04-27 15:54:13.240565 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDiff.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15652 2023-04-27 15:54:13.244655 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexECL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9531 2023-04-27 15:54:13.259121 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEDIFACT.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8188 2023-04-27 15:54:13.242100 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEScript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7601 2023-04-27 15:54:13.255433 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEiffel.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16475 2023-04-27 15:54:13.250724 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErlang.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13292 2023-04-27 15:54:13.247434 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErrorList.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12296 2023-04-27 15:54:13.246526 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFlagship.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5318 2023-04-27 15:54:13.243277 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexForth.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    24685 2023-04-27 15:54:13.244503 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFortran.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6977 2023-04-27 15:54:13.245578 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGAP.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8904 2023-04-27 15:54:13.243539 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGui4Cli.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    81836 2023-04-27 15:54:13.243810 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHTML.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    36346 2023-04-27 15:54:13.247195 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHaskell.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    29024 2023-04-27 15:54:13.261376 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2500 2023-04-27 15:54:13.243561 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexIndent.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8369 2023-04-27 15:54:13.256471 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexInno.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13704 2023-04-27 15:54:13.252060 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexJSON.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16299 2023-04-27 15:54:13.248659 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKVIrc.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3747 2023-04-27 15:54:13.247771 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKix.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    28943 2023-04-27 15:54:13.245085 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLPeg.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15494 2023-04-27 15:54:13.245963 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLaTeX.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8300 2023-04-27 15:54:13.247012 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLisp.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6042 2023-04-27 15:54:13.245231 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLout.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16099 2023-04-27 15:54:13.245523 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLua.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5444 2023-04-27 15:54:13.248148 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMMIXAL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5257 2023-04-27 15:54:13.263030 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMPT.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11271 2023-04-27 15:54:13.244978 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMSSQL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13633 2023-04-27 15:54:13.257633 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMagik.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4391 2023-04-27 15:54:13.253264 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMake.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15564 2023-04-27 15:54:13.250039 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMarkdown.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12124 2023-04-27 15:54:13.248924 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMatlab.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4997 2023-04-27 15:54:13.246245 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMaxima.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10974 2023-04-27 15:54:13.247301 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMetapost.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16541 2023-04-27 15:54:13.248209 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexModula.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    18626 2023-04-27 15:54:13.247013 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMySQL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13810 2023-04-27 15:54:13.247177 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNimrod.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    18818 2023-04-27 15:54:13.249687 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNsis.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1098 2023-04-27 15:54:13.264094 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNull.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    19685 2023-04-27 15:54:13.246945 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOScript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9768 2023-04-27 15:54:13.258854 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOpal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12578 2023-04-27 15:54:13.254552 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPB.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5609 2023-04-27 15:54:13.251164 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPLM.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6620 2023-04-27 15:54:13.250194 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPO.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9536 2023-04-27 15:54:13.247546 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPOV.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12511 2023-04-27 15:54:13.248420 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20877 2023-04-27 15:54:13.250007 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPascal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    57970 2023-04-27 15:54:13.249765 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPerl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20435 2023-04-27 15:54:13.248844 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerPro.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7966 2023-04-27 15:54:13.250838 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerShell.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20629 2023-04-27 15:54:13.265287 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProgress.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5518 2023-04-27 15:54:13.248474 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProps.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    32996 2023-04-27 15:54:13.261171 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPython.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6264 2023-04-27 15:54:13.255686 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexR.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10729 2023-04-27 15:54:13.252533 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRebol.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11302 2023-04-27 15:54:13.251447 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRegistry.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    70986 2023-04-27 15:54:13.250491 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRuby.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    24817 2023-04-27 15:54:13.250393 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRust.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7803 2023-04-27 15:54:13.251042 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSAS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5888 2023-04-27 15:54:13.250975 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSML.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    31189 2023-04-27 15:54:13.250716 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSQL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11010 2023-04-27 15:54:13.251902 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSTTXT.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11945 2023-04-27 15:54:13.266468 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexScriptol.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8980 2023-04-27 15:54:13.249848 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSmalltalk.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4744 2023-04-27 15:54:13.262753 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSorcus.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9048 2023-04-27 15:54:13.256744 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpecman.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6085 2023-04-27 15:54:13.253750 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpice.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7292 2023-04-27 15:54:13.252647 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexStata.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11159 2023-04-27 15:54:13.251662 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTACL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    37477 2023-04-27 15:54:13.253259 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTADS3.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11157 2023-04-27 15:54:13.252245 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTAL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11073 2023-04-27 15:54:13.252466 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    16671 2023-04-27 15:54:13.253061 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCMD.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13999 2023-04-27 15:54:13.253314 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTeX.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17089 2023-04-27 15:54:13.267696 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTxt2tags.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9851 2023-04-27 15:54:13.251294 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVB.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20499 2023-04-27 15:54:13.264173 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVHDL.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    35586 2023-04-27 15:54:13.258343 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVerilog.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17725 2023-04-27 15:54:13.255315 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVisualProlog.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12465 2023-04-27 15:54:13.253919 PyQt6_QScintilla-2.14.0/scintilla/lexers/LexYAML.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/lexers/License.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.562198 PyQt6_QScintilla-2.14.0/scintilla/lexlib/
+-rw-r--r--   0 phil       (501) staff       (20)     2177 2023-04-27 15:54:13.252824 PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      829 2023-04-27 15:54:13.254318 PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.h
+-rw-r--r--   0 phil       (501) staff       (20)    37773 2023-04-27 15:54:13.254459 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      850 2023-04-27 15:54:13.253830 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.h
+-rw-r--r--   0 phil       (501) staff       (20)     1077 2023-04-27 15:54:13.254103 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4516 2023-04-27 15:54:13.254516 PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.h
+-rw-r--r--   0 phil       (501) staff       (20)     2820 2023-04-27 15:54:13.268772 PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2336 2023-04-27 15:54:13.252761 PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.h
+-rw-r--r--   0 phil       (501) staff       (20)     5532 2023-04-27 15:54:13.265663 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexAccessor.h
+-rw-r--r--   0 phil       (501) staff       (20)     3161 2023-04-27 15:54:13.259515 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2261 2023-04-27 15:54:13.256387 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.h
+-rw-r--r--   0 phil       (501) staff       (20)     3025 2023-04-27 15:54:13.255020 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2498 2023-04-27 15:54:13.253738 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.h
+-rw-r--r--   0 phil       (501) staff       (20)     1963 2023-04-27 15:54:13.255371 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1135 2023-04-27 15:54:13.255610 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.h
+-rw-r--r--   0 phil       (501) staff       (20)     1494 2023-04-27 15:54:13.254952 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      809 2023-04-27 15:54:13.254939 PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.h
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/lexlib/License.txt
+-rw-r--r--   0 phil       (501) staff       (20)     3453 2023-04-27 15:54:13.255662 PyQt6_QScintilla-2.14.0/scintilla/lexlib/OptionSet.h
+-rw-r--r--   0 phil       (501) staff       (20)     4334 2023-04-27 15:54:13.270663 PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      725 2023-04-27 15:54:13.253632 PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.h
+-rw-r--r--   0 phil       (501) staff       (20)     3003 2023-04-27 15:54:13.266862 PyQt6_QScintilla-2.14.0/scintilla/lexlib/SparseState.h
+-rw-r--r--   0 phil       (501) staff       (20)      853 2023-04-27 15:54:13.260592 PyQt6_QScintilla-2.14.0/scintilla/lexlib/StringCopy.h
+-rw-r--r--   0 phil       (501) staff       (20)     1550 2023-04-27 15:54:13.257279 PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6026 2023-04-27 15:54:13.256286 PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.h
+-rw-r--r--   0 phil       (501) staff       (20)     4592 2023-04-27 15:54:13.254766 PyQt6_QScintilla-2.14.0/scintilla/lexlib/SubStyles.h
+-rw-r--r--   0 phil       (501) staff       (20)     6887 2023-04-27 15:54:13.256610 PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      965 2023-04-27 15:54:13.256426 PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.586403 PyQt6_QScintilla-2.14.0/scintilla/src/
+-rw-r--r--   0 phil       (501) staff       (20)     7326 2023-04-27 15:54:13.286351 PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2023-04-27 15:54:13.290783 PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.h
+-rw-r--r--   0 phil       (501) staff       (20)    11394 2023-04-27 15:54:13.284049 PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2821 2023-04-27 15:54:13.287896 PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.h
+-rw-r--r--   0 phil       (501) staff       (20)    25198 2023-04-27 15:54:13.281777 PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1601 2023-04-27 15:54:13.284193 PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.h
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2023-04-27 15:54:13.288850 PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1010 2023-04-27 15:54:13.291137 PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.h
+-rw-r--r--   0 phil       (501) staff       (20)     4777 2023-04-27 15:54:13.299833 PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      623 2023-04-27 15:54:13.294417 PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.h
+-rw-r--r--   0 phil       (501) staff       (20)    36730 2023-04-27 15:54:13.294797 PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7215 2023-04-27 15:54:13.291463 PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.h
+-rw-r--r--   0 phil       (501) staff       (20)     1588 2023-04-27 15:54:13.287277 PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      930 2023-04-27 15:54:13.291716 PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.h
+-rw-r--r--   0 phil       (501) staff       (20)    11872 2023-04-27 15:54:13.286254 PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1694 2023-04-27 15:54:13.289026 PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.h
+-rw-r--r--   0 phil       (501) staff       (20)     1107 2023-04-27 15:54:13.282737 PyQt6_QScintilla-2.14.0/scintilla/src/DBCS.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      397 2023-04-27 15:54:13.285971 PyQt6_QScintilla-2.14.0/scintilla/src/DBCS.h
+-rw-r--r--   0 phil       (501) staff       (20)     9522 2023-04-27 15:54:13.289880 PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2072 2023-04-27 15:54:13.292044 PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.h
+-rw-r--r--   0 phil       (501) staff       (20)    98470 2023-04-27 15:54:13.303656 PyQt6_QScintilla-2.14.0/scintilla/src/Document.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    21627 2023-04-27 15:54:13.296216 PyQt6_QScintilla-2.14.0/scintilla/src/Document.h
+-rw-r--r--   0 phil       (501) staff       (20)     1867 2023-04-27 15:54:13.296191 PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1486 2023-04-27 15:54:13.292670 PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.h
+-rw-r--r--   0 phil       (501) staff       (20)   101652 2023-04-27 15:54:13.290169 PyQt6_QScintilla-2.14.0/scintilla/src/EditView.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7923 2023-04-27 15:54:13.292887 PyQt6_QScintilla-2.14.0/scintilla/src/EditView.h
+-rw-r--r--   0 phil       (501) staff       (20)   248617 2023-04-27 15:54:13.296479 PyQt6_QScintilla-2.14.0/scintilla/src/Editor.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    23032 2023-04-27 15:54:13.290857 PyQt6_QScintilla-2.14.0/scintilla/src/Editor.h
+-rw-r--r--   0 phil       (501) staff       (20)      970 2023-04-27 15:54:13.283574 PyQt6_QScintilla-2.14.0/scintilla/src/ElapsedPeriod.h
+-rw-r--r--   0 phil       (501) staff       (20)     3570 2023-04-27 15:54:13.287221 PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2094 2023-04-27 15:54:13.290982 PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.h
+-rw-r--r--   0 phil       (501) staff       (20)      813 2023-04-27 15:54:13.293071 PyQt6_QScintilla-2.14.0/scintilla/src/FontQuality.h
+-rw-r--r--   0 phil       (501) staff       (20)     7835 2023-04-27 15:54:13.305306 PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1674 2023-04-27 15:54:13.297523 PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.h
+-rw-r--r--   0 phil       (501) staff       (20)      735 2023-04-27 15:54:13.297276 PyQt6_QScintilla-2.14.0/scintilla/src/IntegerRectangle.h
+-rw-r--r--   0 phil       (501) staff       (20)     5434 2023-04-27 15:54:13.293661 PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1331 2023-04-27 15:54:13.291212 PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.h
+-rw-r--r--   0 phil       (501) staff       (20)      854 2023-04-27 15:54:13.218300 PyQt6_QScintilla-2.14.0/scintilla/src/License.txt
+-rw-r--r--   0 phil       (501) staff       (20)    15402 2023-04-27 15:54:13.294466 PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1510 2023-04-27 15:54:13.299705 PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.h
+-rw-r--r--   0 phil       (501) staff       (20)    16819 2023-04-27 15:54:13.292530 PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1576 2023-04-27 15:54:13.284513 PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.h
+-rw-r--r--   0 phil       (501) staff       (20)     5803 2023-04-27 15:54:13.288173 PyQt6_QScintilla-2.14.0/scintilla/src/Partitioning.h
+-rw-r--r--   0 phil       (501) staff       (20)    12933 2023-04-27 15:54:13.292625 PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5100 2023-04-27 15:54:13.294183 PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.h
+-rw-r--r--   0 phil       (501) staff       (20)      827 2023-04-27 15:54:13.306439 PyQt6_QScintilla-2.14.0/scintilla/src/Position.h
+-rw-r--r--   0 phil       (501) staff       (20)    20501 2023-04-27 15:54:13.300405 PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7771 2023-04-27 15:54:13.300098 PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.h
+-rw-r--r--   0 phil       (501) staff       (20)    26564 2023-04-27 15:54:13.295605 PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1744 2023-04-27 15:54:13.292693 PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.h
+-rw-r--r--   0 phil       (501) staff       (20)     9604 2023-04-27 15:54:13.295932 PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2148 2023-04-27 15:54:13.300899 PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.h
+-rw-r--r--   0 phil       (501) staff       (20)      305 2023-04-27 15:54:13.293599 PyQt6_QScintilla-2.14.0/scintilla/src/SciTE.properties
+-rw-r--r--   0 phil       (501) staff       (20)    30781 2023-04-27 15:54:13.286747 PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3124 2023-04-27 15:54:13.289188 PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.h
+-rw-r--r--   0 phil       (501) staff       (20)    10711 2023-04-27 15:54:13.294313 PyQt6_QScintilla-2.14.0/scintilla/src/Selection.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5757 2023-04-27 15:54:13.295658 PyQt6_QScintilla-2.14.0/scintilla/src/Selection.h
+-rw-r--r--   0 phil       (501) staff       (20)     5323 2023-04-27 15:54:13.307420 PyQt6_QScintilla-2.14.0/scintilla/src/SparseVector.h
+-rw-r--r--   0 phil       (501) staff       (20)    10129 2023-04-27 15:54:13.301804 PyQt6_QScintilla-2.14.0/scintilla/src/SplitVector.h
+-rw-r--r--   0 phil       (501) staff       (20)     4388 2023-04-27 15:54:13.301084 PyQt6_QScintilla-2.14.0/scintilla/src/Style.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2412 2023-04-27 15:54:13.296808 PyQt6_QScintilla-2.14.0/scintilla/src/Style.h
+-rw-r--r--   0 phil       (501) staff       (20)    10279 2023-04-27 15:54:13.294066 PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2825 2023-04-27 15:54:13.297512 PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.h
+-rw-r--r--   0 phil       (501) staff       (20)      820 2023-04-27 15:54:13.301907 PyQt6_QScintilla-2.14.0/scintilla/src/UniqueString.h
+-rw-r--r--   0 phil       (501) staff       (20)    19320 2023-04-27 15:54:13.295349 PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6791 2023-04-27 15:54:13.287998 PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.h
+-rw-r--r--   0 phil       (501) staff       (20)    10701 2023-04-27 15:54:13.290545 PyQt6_QScintilla-2.14.0/scintilla/src/XPM.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3597 2023-04-27 15:54:13.295701 PyQt6_QScintilla-2.14.0/scintilla/src/XPM.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.607818 PyQt6_QScintilla-2.14.0/sip/
+-rw-r--r--   0 phil       (501) staff       (20)     1525 2023-04-27 16:09:48.974880 PyQt6_QScintilla-2.14.0/sip/qsciabstractapis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2048 2023-04-27 16:09:48.967333 PyQt6_QScintilla-2.14.0/sip/qsciapis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3643 2023-04-27 16:09:48.975800 PyQt6_QScintilla-2.14.0/sip/qscicommand.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1463 2023-04-27 16:09:48.965856 PyQt6_QScintilla-2.14.0/sip/qscicommandset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1085 2023-04-27 16:09:48.980998 PyQt6_QScintilla-2.14.0/sip/qscidocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3663 2023-04-27 16:09:48.973005 PyQt6_QScintilla-2.14.0/sip/qscilexer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2286 2023-04-27 16:09:48.959830 PyQt6_QScintilla-2.14.0/sip/qscilexerasm.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2089 2023-04-27 16:09:48.969112 PyQt6_QScintilla-2.14.0/sip/qscilexeravs.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2194 2023-04-27 16:09:48.983574 PyQt6_QScintilla-2.14.0/sip/qscilexerbash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1712 2023-04-27 16:09:48.944691 PyQt6_QScintilla-2.14.0/sip/qscilexerbatch.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2000 2023-04-27 16:09:48.974554 PyQt6_QScintilla-2.14.0/sip/qscilexercmake.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2854 2023-04-27 16:09:48.966904 PyQt6_QScintilla-2.14.0/sip/qscilexercoffeescript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4497 2023-04-27 16:09:48.960731 PyQt6_QScintilla-2.14.0/sip/qscilexercpp.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1448 2023-04-27 16:09:48.984206 PyQt6_QScintilla-2.14.0/sip/qscilexercsharp.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2568 2023-04-27 16:09:48.976395 PyQt6_QScintilla-2.14.0/sip/qscilexercss.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1460 2023-04-27 16:09:48.963633 PyQt6_QScintilla-2.14.0/sip/qscilexercustom.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2660 2023-04-27 16:09:48.967929 PyQt6_QScintilla-2.14.0/sip/qscilexerd.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1614 2023-04-27 16:09:48.973702 PyQt6_QScintilla-2.14.0/sip/qscilexerdiff.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1547 2023-04-27 16:09:48.976771 PyQt6_QScintilla-2.14.0/sip/qscilexeredifact.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1251 2023-04-27 16:09:48.961355 PyQt6_QScintilla-2.14.0/sip/qscilexerfortran.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2096 2023-04-27 16:09:48.982992 PyQt6_QScintilla-2.14.0/sip/qscilexerfortran77.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1692 2023-04-27 16:09:48.966278 PyQt6_QScintilla-2.14.0/sip/qscilexerhex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5292 2023-04-27 16:09:48.947204 PyQt6_QScintilla-2.14.0/sip/qscilexerhtml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1303 2023-04-27 16:09:48.946041 PyQt6_QScintilla-2.14.0/sip/qscilexeridl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1271 2023-04-27 16:09:48.961653 PyQt6_QScintilla-2.14.0/sip/qscilexerintelhex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1226 2023-04-27 16:09:48.983876 PyQt6_QScintilla-2.14.0/sip/qscilexerjava.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1476 2023-04-27 16:09:48.961064 PyQt6_QScintilla-2.14.0/sip/qscilexerjavascript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2161 2023-04-27 16:09:48.970175 PyQt6_QScintilla-2.14.0/sip/qscilexerjson.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2316 2023-04-27 16:09:48.947761 PyQt6_QScintilla-2.14.0/sip/qscilexerlua.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1630 2023-04-27 16:09:48.958857 PyQt6_QScintilla-2.14.0/sip/qscilexermakefile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1903 2023-04-27 16:09:48.981759 PyQt6_QScintilla-2.14.0/sip/qscilexermarkdown.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1216 2023-04-27 16:09:48.968599 PyQt6_QScintilla-2.14.0/sip/qscilexermasm.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1588 2023-04-27 16:09:48.943235 PyQt6_QScintilla-2.14.0/sip/qscilexermatlab.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1216 2023-04-27 16:09:48.981296 PyQt6_QScintilla-2.14.0/sip/qscilexernasm.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1274 2023-04-27 16:09:48.972389 PyQt6_QScintilla-2.14.0/sip/qscilexeroctave.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2574 2023-04-27 16:09:48.945723 PyQt6_QScintilla-2.14.0/sip/qscilexerpascal.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3226 2023-04-27 16:09:48.972086 PyQt6_QScintilla-2.14.0/sip/qscilexerperl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2023 2023-04-27 16:09:48.964117 PyQt6_QScintilla-2.14.0/sip/qscilexerpo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2322 2023-04-27 16:09:48.958000 PyQt6_QScintilla-2.14.0/sip/qscilexerpostscript.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2335 2023-04-27 16:09:48.971355 PyQt6_QScintilla-2.14.0/sip/qscilexerpov.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1964 2023-04-27 16:09:48.958460 PyQt6_QScintilla-2.14.0/sip/qscilexerproperties.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3334 2023-04-27 16:09:48.962350 PyQt6_QScintilla-2.14.0/sip/qscilexerpython.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2660 2023-04-27 16:09:48.970798 PyQt6_QScintilla-2.14.0/sip/qscilexerruby.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1590 2023-04-27 16:09:48.982494 PyQt6_QScintilla-2.14.0/sip/qscilexerspice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2764 2023-04-27 16:09:48.964750 PyQt6_QScintilla-2.14.0/sip/qscilexersql.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1243 2023-04-27 16:09:48.984508 PyQt6_QScintilla-2.14.0/sip/qscilexersrec.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2195 2023-04-27 16:09:48.965515 PyQt6_QScintilla-2.14.0/sip/qscilexertcl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1257 2023-04-27 16:09:48.943594 PyQt6_QScintilla-2.14.0/sip/qscilexertekhex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1935 2023-04-27 16:09:48.959317 PyQt6_QScintilla-2.14.0/sip/qscilexertex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3027 2023-04-27 16:09:48.963305 PyQt6_QScintilla-2.14.0/sip/qscilexerverilog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2409 2023-04-27 16:09:48.969670 PyQt6_QScintilla-2.14.0/sip/qscilexervhdl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1665 2023-04-27 16:09:48.968298 PyQt6_QScintilla-2.14.0/sip/qscilexerxml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1950 2023-04-27 16:09:48.945157 PyQt6_QScintilla-2.14.0/sip/qscilexeryaml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1381 2023-04-27 16:09:48.982095 PyQt6_QScintilla-2.14.0/sip/qscimacro.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1027 2023-04-27 16:09:48.962584 PyQt6_QScintilla-2.14.0/sip/qscimod5.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1027 2023-04-27 16:09:48.964979 PyQt6_QScintilla-2.14.0/sip/qscimod6.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3603 2023-04-27 16:09:48.944269 PyQt6_QScintilla-2.14.0/sip/qscimodcommon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1656 2023-04-27 16:09:48.974063 PyQt6_QScintilla-2.14.0/sip/qsciprinter.sip
+-rw-r--r--   0 phil       (501) staff       (20)    18318 2023-04-27 16:09:48.980172 PyQt6_QScintilla-2.14.0/sip/qsciscintilla.sip
+-rw-r--r--   0 phil       (501) staff       (20)    44084 2023-04-27 16:09:48.957408 PyQt6_QScintilla-2.14.0/sip/qsciscintillabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-27 16:09:48.980715 PyQt6_QScintilla-2.14.0/sip/qscistyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1169 2023-04-27 16:09:48.973292 PyQt6_QScintilla-2.14.0/sip/qscistyledtext.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.643552 PyQt6_QScintilla-2.14.0/src/
+-rw-r--r--   0 phil       (501) staff       (20)     9963 2023-04-27 16:09:48.742697 PyQt6_QScintilla-2.14.0/src/InputMethod.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7215 2023-04-27 16:09:48.680251 PyQt6_QScintilla-2.14.0/src/ListBoxQt.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2639 2023-04-27 16:09:48.840247 PyQt6_QScintilla-2.14.0/src/ListBoxQt.h
+-rw-r--r--   0 phil       (501) staff       (20)     2863 2023-04-27 16:09:48.808678 PyQt6_QScintilla-2.14.0/src/MacPasteboardMime.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    23192 2023-04-27 16:09:48.846629 PyQt6_QScintilla-2.14.0/src/PlatQt.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.664736 PyQt6_QScintilla-2.14.0/src/Qsci/
+-rw-r--r--   0 phil       (501) staff       (20)     3627 2023-04-27 16:09:48.908858 PyQt6_QScintilla-2.14.0/src/Qsci/qsciabstractapis.h
+-rw-r--r--   0 phil       (501) staff       (20)     8302 2023-04-27 16:09:48.744123 PyQt6_QScintilla-2.14.0/src/Qsci/qsciapis.h
+-rw-r--r--   0 phil       (501) staff       (20)    14883 2023-04-27 16:09:48.748310 PyQt6_QScintilla-2.14.0/src/Qsci/qscicommand.h
+-rw-r--r--   0 phil       (501) staff       (20)     2811 2023-04-27 16:09:48.922221 PyQt6_QScintilla-2.14.0/src/Qsci/qscicommandset.h
+-rw-r--r--   0 phil       (501) staff       (20)     1901 2023-04-27 16:09:48.710894 PyQt6_QScintilla-2.14.0/src/Qsci/qscidocument.h
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-04-27 16:09:48.890407 PyQt6_QScintilla-2.14.0/src/Qsci/qsciglobal.h
+-rw-r--r--   0 phil       (501) staff       (20)    13290 2023-04-27 16:09:48.727875 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexer.h
+-rw-r--r--   0 phil       (501) staff       (20)     6123 2023-04-27 16:09:48.754058 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerasm.h
+-rw-r--r--   0 phil       (501) staff       (20)     5290 2023-04-27 16:09:48.892386 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeravs.h
+-rw-r--r--   0 phil       (501) staff       (20)     4875 2023-04-27 16:09:48.687619 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbash.h
+-rw-r--r--   0 phil       (501) staff       (20)     3432 2023-04-27 16:09:48.812588 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbatch.h
+-rw-r--r--   0 phil       (501) staff       (20)     4744 2023-04-27 16:09:48.694534 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercmake.h
+-rw-r--r--   0 phil       (501) staff       (20)     8627 2023-04-27 16:09:48.810364 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercoffeescript.h
+-rw-r--r--   0 phil       (501) staff       (20)    13427 2023-04-27 16:09:48.750961 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercpp.h
+-rw-r--r--   0 phil       (501) staff       (20)     2586 2023-04-27 16:09:48.720724 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercsharp.h
+-rw-r--r--   0 phil       (501) staff       (20)     7687 2023-04-27 16:09:48.939775 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercss.h
+-rw-r--r--   0 phil       (501) staff       (20)     3655 2023-04-27 16:09:48.710421 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercustom.h
+-rw-r--r--   0 phil       (501) staff       (20)     7509 2023-04-27 16:09:48.930437 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerd.h
+-rw-r--r--   0 phil       (501) staff       (20)     3001 2023-04-27 16:09:48.725566 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerdiff.h
+-rw-r--r--   0 phil       (501) staff       (20)     2846 2023-04-27 16:09:48.740068 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeredifact.h
+-rw-r--r--   0 phil       (501) staff       (20)     1968 2023-04-27 16:09:48.940246 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran.h
+-rw-r--r--   0 phil       (501) staff       (20)     5055 2023-04-27 16:09:48.762214 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran77.h
+-rw-r--r--   0 phil       (501) staff       (20)     3360 2023-04-27 16:09:48.891243 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhex.h
+-rw-r--r--   0 phil       (501) staff       (20)    14535 2023-04-27 16:09:48.807867 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhtml.h
+-rw-r--r--   0 phil       (501) staff       (20)     2158 2023-04-27 16:09:48.734476 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeridl.h
+-rw-r--r--   0 phil       (501) staff       (20)     2014 2023-04-27 16:09:48.728471 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerintelhex.h
+-rw-r--r--   0 phil       (501) staff       (20)     1791 2023-04-27 16:09:48.917596 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjava.h
+-rw-r--r--   0 phil       (501) staff       (20)     2711 2023-04-27 16:09:48.928381 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjavascript.h
+-rw-r--r--   0 phil       (501) staff       (20)     5543 2023-04-27 16:09:48.730669 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjson.h
+-rw-r--r--   0 phil       (501) staff       (20)     6049 2023-04-27 16:09:48.937158 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerlua.h
+-rw-r--r--   0 phil       (501) staff       (20)     3127 2023-04-27 16:09:48.813323 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermakefile.h
+-rw-r--r--   0 phil       (501) staff       (20)     4181 2023-04-27 16:09:48.729469 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermarkdown.h
+-rw-r--r--   0 phil       (501) staff       (20)     1696 2023-04-27 16:09:48.724823 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermasm.h
+-rw-r--r--   0 phil       (501) staff       (20)     3031 2023-04-27 16:09:48.839671 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermatlab.h
+-rw-r--r--   0 phil       (501) staff       (20)     1696 2023-04-27 16:09:48.892836 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexernasm.h
+-rw-r--r--   0 phil       (501) staff       (20)     1957 2023-04-27 16:09:48.781796 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeroctave.h
+-rw-r--r--   0 phil       (501) staff       (20)     7197 2023-04-27 16:09:48.927776 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpascal.h
+-rw-r--r--   0 phil       (501) staff       (20)     8811 2023-04-27 16:09:48.784814 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerperl.h
+-rw-r--r--   0 phil       (501) staff       (20)     4776 2023-04-27 16:09:48.921569 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpo.h
+-rw-r--r--   0 phil       (501) staff       (20)     5883 2023-04-27 16:09:48.758076 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpostscript.h
+-rw-r--r--   0 phil       (501) staff       (20)     6188 2023-04-27 16:09:48.677956 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpov.h
+-rw-r--r--   0 phil       (501) staff       (20)     4714 2023-04-27 16:09:48.802461 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerproperties.h
+-rw-r--r--   0 phil       (501) staff       (20)    10679 2023-04-27 16:09:48.906499 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpython.h
+-rw-r--r--   0 phil       (501) staff       (20)     6813 2023-04-27 16:09:48.794779 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerruby.h
+-rw-r--r--   0 phil       (501) staff       (20)     3059 2023-04-27 16:09:48.740813 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerspice.h
+-rw-r--r--   0 phil       (501) staff       (20)     8893 2023-04-27 16:09:48.789876 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersql.h
+-rw-r--r--   0 phil       (501) staff       (20)     1957 2023-04-27 16:09:48.733961 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersrec.h
+-rw-r--r--   0 phil       (501) staff       (20)     5523 2023-04-27 16:09:48.707696 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertcl.h
+-rw-r--r--   0 phil       (501) staff       (20)     1992 2023-04-27 16:09:48.930913 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertekhex.h
+-rw-r--r--   0 phil       (501) staff       (20)     5076 2023-04-27 16:09:48.756289 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertex.h
+-rw-r--r--   0 phil       (501) staff       (20)     8086 2023-04-27 16:09:48.676613 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerverilog.h
+-rw-r--r--   0 phil       (501) staff       (20)     6446 2023-04-27 16:09:48.811795 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexervhdl.h
+-rw-r--r--   0 phil       (501) staff       (20)     3458 2023-04-27 16:09:48.889956 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerxml.h
+-rw-r--r--   0 phil       (501) staff       (20)     4424 2023-04-27 16:09:48.689510 PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeryaml.h
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2023-04-27 16:09:48.838141 PyQt6_QScintilla-2.14.0/src/Qsci/qscimacro.h
+-rw-r--r--   0 phil       (501) staff       (20)     4423 2023-04-27 16:09:48.814604 PyQt6_QScintilla-2.14.0/src/Qsci/qsciprinter.h
+-rw-r--r--   0 phil       (501) staff       (20)    86594 2023-04-27 16:09:48.674896 PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintilla.h
+-rw-r--r--   0 phil       (501) staff       (20)    89964 2023-04-27 16:09:48.837397 PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintillabase.h
+-rw-r--r--   0 phil       (501) staff       (20)     6226 2023-04-27 16:09:48.897008 PyQt6_QScintilla-2.14.0/src/Qsci/qscistyle.h
+-rw-r--r--   0 phil       (501) staff       (20)     1898 2023-04-27 16:09:48.917148 PyQt6_QScintilla-2.14.0/src/Qsci/qscistyledtext.h
+-rw-r--r--   0 phil       (501) staff       (20)    21851 2023-04-27 16:09:48.885387 PyQt6_QScintilla-2.14.0/src/SciAccessibility.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4457 2023-04-27 16:09:48.688490 PyQt6_QScintilla-2.14.0/src/SciAccessibility.h
+-rw-r--r--   0 phil       (501) staff       (20)     4754 2023-04-27 16:09:48.908201 PyQt6_QScintilla-2.14.0/src/SciClasses.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-04-27 16:09:48.904397 PyQt6_QScintilla-2.14.0/src/SciClasses.h
+-rw-r--r--   0 phil       (501) staff       (20)    19373 2023-04-27 16:09:48.903648 PyQt6_QScintilla-2.14.0/src/ScintillaQt.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4225 2023-04-27 16:09:48.765916 PyQt6_QScintilla-2.14.0/src/ScintillaQt.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.642716 PyQt6_QScintilla-2.14.0/src/features/
+-rw-r--r--   0 phil       (501) staff       (20)      534 2023-04-27 16:09:48.752675 PyQt6_QScintilla-2.14.0/src/features/qscintilla2.prf
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-27 16:09:49.643155 PyQt6_QScintilla-2.14.0/src/features_staticlib/
+-rw-r--r--   0 phil       (501) staff       (20)      507 2023-04-27 16:09:48.909333 PyQt6_QScintilla-2.14.0/src/features_staticlib/qscintilla2.prf
+-rw-r--r--   0 phil       (501) staff       (20)     1423 2023-04-27 16:09:48.906974 PyQt6_QScintilla-2.14.0/src/qsciabstractapis.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    24667 2023-04-27 16:09:48.703639 PyQt6_QScintilla-2.14.0/src/qsciapis.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3394 2023-04-27 16:09:48.850463 PyQt6_QScintilla-2.14.0/src/qscicommand.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    27482 2023-04-27 16:09:48.686351 PyQt6_QScintilla-2.14.0/src/qscicommandset.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3793 2023-04-27 16:09:48.880447 PyQt6_QScintilla-2.14.0/src/qscidocument.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17245 2023-04-27 16:09:48.935842 PyQt6_QScintilla-2.14.0/src/qscilexer.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    23577 2023-04-27 16:09:48.798328 PyQt6_QScintilla-2.14.0/src/qscilexerasm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    14533 2023-04-27 16:09:48.706333 PyQt6_QScintilla-2.14.0/src/qscilexeravs.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8166 2023-04-27 16:09:48.804610 PyQt6_QScintilla-2.14.0/src/qscilexerbash.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4490 2023-04-27 16:09:48.761107 PyQt6_QScintilla-2.14.0/src/qscilexerbatch.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8247 2023-04-27 16:09:48.898948 PyQt6_QScintilla-2.14.0/src/qscilexercmake.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10030 2023-04-27 16:09:48.692369 PyQt6_QScintilla-2.14.0/src/qscilexercoffeescript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    20137 2023-04-27 16:09:48.739306 PyQt6_QScintilla-2.14.0/src/qscilexercpp.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3237 2023-04-27 16:09:48.838945 PyQt6_QScintilla-2.14.0/src/qscilexercsharp.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10573 2023-04-27 16:09:48.849444 PyQt6_QScintilla-2.14.0/src/qscilexercss.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2683 2023-04-27 16:09:48.715596 PyQt6_QScintilla-2.14.0/src/qscilexercustom.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    10175 2023-04-27 16:09:48.697359 PyQt6_QScintilla-2.14.0/src/qscilexerd.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3146 2023-04-27 16:09:48.938131 PyQt6_QScintilla-2.14.0/src/qscilexerdiff.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2815 2023-04-27 16:09:48.878232 PyQt6_QScintilla-2.14.0/src/qscilexeredifact.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4910 2023-04-27 16:09:48.745753 PyQt6_QScintilla-2.14.0/src/qscilexerfortran.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7062 2023-04-27 16:09:48.800214 PyQt6_QScintilla-2.14.0/src/qscilexerfortran77.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3604 2023-04-27 16:09:48.693457 PyQt6_QScintilla-2.14.0/src/qscilexerhex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    30776 2023-04-27 16:09:48.778974 PyQt6_QScintilla-2.14.0/src/qscilexerhtml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3629 2023-04-27 16:09:48.771886 PyQt6_QScintilla-2.14.0/src/qscilexeridl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1542 2023-04-27 16:09:48.711359 PyQt6_QScintilla-2.14.0/src/qscilexerintelhex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1776 2023-04-27 16:09:48.813773 PyQt6_QScintilla-2.14.0/src/qscilexerjava.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3207 2023-04-27 16:09:48.744981 PyQt6_QScintilla-2.14.0/src/qscilexerjavascript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6285 2023-04-27 16:09:48.911265 PyQt6_QScintilla-2.14.0/src/qscilexerjson.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8617 2023-04-27 16:09:48.781297 PyQt6_QScintilla-2.14.0/src/qscilexerlua.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3418 2023-04-27 16:09:48.782843 PyQt6_QScintilla-2.14.0/src/qscilexermakefile.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6253 2023-04-27 16:09:48.887234 PyQt6_QScintilla-2.14.0/src/qscilexermarkdown.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1269 2023-04-27 16:09:48.709700 PyQt6_QScintilla-2.14.0/src/qscilexermasm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3405 2023-04-27 16:09:48.755210 PyQt6_QScintilla-2.14.0/src/qscilexermatlab.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1268 2023-04-27 16:09:48.880865 PyQt6_QScintilla-2.14.0/src/qscilexernasm.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1970 2023-04-27 16:09:48.928904 PyQt6_QScintilla-2.14.0/src/qscilexeroctave.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9835 2023-04-27 16:09:48.764873 PyQt6_QScintilla-2.14.0/src/qscilexerpascal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15626 2023-04-27 16:09:48.926257 PyQt6_QScintilla-2.14.0/src/qscilexerperl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4596 2023-04-27 16:09:48.720128 PyQt6_QScintilla-2.14.0/src/qscilexerpo.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13559 2023-04-27 16:09:48.788011 PyQt6_QScintilla-2.14.0/src/qscilexerpostscript.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12918 2023-04-27 16:09:48.920444 PyQt6_QScintilla-2.14.0/src/qscilexerpov.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4689 2023-04-27 16:09:48.791260 PyQt6_QScintilla-2.14.0/src/qscilexerproperties.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    11799 2023-04-27 16:09:48.718691 PyQt6_QScintilla-2.14.0/src/qscilexerpython.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9035 2023-04-27 16:09:48.916627 PyQt6_QScintilla-2.14.0/src/qscilexerruby.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5256 2023-04-27 16:09:48.801461 PyQt6_QScintilla-2.14.0/src/qscilexerspice.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13713 2023-04-27 16:09:48.724342 PyQt6_QScintilla-2.14.0/src/qscilexersql.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1549 2023-04-27 16:09:48.840728 PyQt6_QScintilla-2.14.0/src/qscilexersrec.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    13475 2023-04-27 16:09:48.733407 PyQt6_QScintilla-2.14.0/src/qscilexertcl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1603 2023-04-27 16:09:48.756764 PyQt6_QScintilla-2.14.0/src/qscilexertekhex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9867 2023-04-27 16:09:48.793221 PyQt6_QScintilla-2.14.0/src/qscilexertex.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    15610 2023-04-27 16:09:48.714834 PyQt6_QScintilla-2.14.0/src/qscilexerverilog.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9890 2023-04-27 16:09:48.913854 PyQt6_QScintilla-2.14.0/src/qscilexervhdl.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5283 2023-04-27 16:09:48.709286 PyQt6_QScintilla-2.14.0/src/qscilexerxml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5531 2023-04-27 16:09:48.759750 PyQt6_QScintilla-2.14.0/src/qscilexeryaml.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7469 2023-04-27 16:09:48.889189 PyQt6_QScintilla-2.14.0/src/qscimacro.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    14299 2023-04-27 16:09:48.895625 PyQt6_QScintilla-2.14.0/src/qscintilla.pro
+-rw-r--r--   0 phil       (501) staff       (20)    44424 2023-04-27 15:54:13.281422 PyQt6_QScintilla-2.14.0/src/qscintilla_cs.qm
+-rw-r--r--   0 phil       (501) staff       (20)    82744 2023-04-27 15:54:13.293213 PyQt6_QScintilla-2.14.0/src/qscintilla_de.qm
+-rw-r--r--   0 phil       (501) staff       (20)    81850 2023-04-27 15:54:13.290333 PyQt6_QScintilla-2.14.0/src/qscintilla_es.qm
+-rw-r--r--   0 phil       (501) staff       (20)    53842 2023-04-27 15:54:13.284613 PyQt6_QScintilla-2.14.0/src/qscintilla_fr.qm
+-rw-r--r--   0 phil       (501) staff       (20)    49459 2023-04-27 15:54:13.281912 PyQt6_QScintilla-2.14.0/src/qscintilla_pt_br.qm
+-rw-r--r--   0 phil       (501) staff       (20)     5046 2023-04-27 16:09:48.941504 PyQt6_QScintilla-2.14.0/src/qsciprinter.cpp
+-rw-r--r--   0 phil       (501) staff       (20)   113218 2023-04-27 16:09:48.877355 PyQt6_QScintilla-2.14.0/src/qsciscintilla.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    21783 2023-04-27 16:09:48.771123 PyQt6_QScintilla-2.14.0/src/qsciscintillabase.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5035 2023-04-27 16:09:48.879430 PyQt6_QScintilla-2.14.0/src/qscistyle.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1620 2023-04-27 16:09:48.931347 PyQt6_QScintilla-2.14.0/src/qscistyledtext.cpp
```

### Comparing `PyQt6_QScintilla-2.13.4/ChangeLog` & `PyQt6_QScintilla-2.14.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,117 @@
+2023-04-24  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qt/qsciscintilla.cpp:
+	Fixed a regression in QSciScintilla::text().
+	[b748338e45bb] [2.14.0]
+
+2023-04-20  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* qt/qsciscintilla.cpp:
+	Use SCI_ADDTEXT rather than SCI_SETTEXT to set the text so tht
+	embedded zero bytes can be loaded.
+	[774bcbca48b9]
+
+	* NEWS, qt/InputMethod.cpp, qt/SciAccessibility.cpp,
+	qt/SciAccessibility.h, qt/qscilexer.cpp, qt/qscilexer.h,
+	qt/qsciscintilla.cpp, qt/qsciscintillabase.cpp,
+	qt/qsciscintillabase.h:
+	Refactored the conversions from bytes to a QString to allow for
+	embedded zero bytes and to remove duplicated code.
+	[c8eb0d943c07]
+
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qt/qscintilla_cs.ts, qt/qscintilla_de.qm, qt/qscintilla_de.ts,
+	qt/qscintilla_es.ts, qt/qscintilla_fr.ts, qt/qscintilla_pt_br.ts:
+	Fixed the .ts files.
+	[5d000fe9301e]
+
+2023-03-28  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* Python/sip/qscilexerasm.sip, Python/sip/qscilexermasm.sip,
+	Python/sip/qscilexernasm.sip, Python/sip/qscimodcommon.sip,
+	Python/sip/qsciscintillabase.sip:
+	Implemented the Python wrappers for the assembler lexers.
+	[0030fcf7a208]
+
+	* qt/qscintilla_cs.ts, qt/qscintilla_de.ts, qt/qscintilla_es.ts,
+	qt/qscintilla_fr.ts, qt/qscintilla_pt_br.ts:
+	Updated the translation source files.
+	[0fb2491bb039]
+
+	* qt/qscilexer.cpp, qt/qscilexer.h, qt/qscilexerasm.cpp,
+	qt/qscilexerasm.h, qt/qsciscintillabase.h:
+	Completed the implementation of the assember lexers. Note we choose
+	not to support explicit fold points.
+	[629503d9342b]
+
+	* NEWS, qt/qsciscintilla.cpp, qt/qsciscintilla.h,
+	qt/qsciscintillabase.cpp, qt/qsciscintillabase.h:
+	Removed a Qt4 compatibility macro.
+	[4b23653f3e5c]
+
+	* qt/qscilexerasm.cpp, qt/qscilexerasm.h:
+	Added the support for compact and multi-line comment folding to
+	QsciLexerAsm.
+	[708bed0e9e2d]
+
+2023-03-27  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qt/qscilexerasm.cpp, qt/qscilexerasm.h,
+	qt/qscilexerintelhex.cpp, qt/qscilexermasm.cpp, qt/qscilexermasm.h,
+	qt/qscilexernasm.cpp, qt/qscilexernasm.h, qt/qscilexertekhex.cpp,
+	qt/qscintilla.pro:
+	Initial implementation of the QsciLexerAsm, QsciLexerMASM and
+	QsciLexerNASM classes.
+	[f216dfe8a7a9]
+
+2023-03-26  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* Python/sip/qscilexerintelhex.sip, Python/sip/qscilexersrec.sip,
+	Python/sip/qscilexertekhex.sip, Python/sip/qscimodcommon.sip,
+	Python/sip/qsciscintillabase.sip:
+	Completed the new Python wrappers.
+	[9acd96c733d2]
+
+	* Python/sip/qscilexerhex.sip, Python/sip/qscilexerintelhex.sip,
+	Python/sip/qscilexersrec.sip, Python/sip/qscilexertekhex.sip:
+	Added the Python bindings for the new lexer classes.
+	[7882938747c0]
+
+	* qt/qscintilla_cs.ts, qt/qscintilla_de.ts, qt/qscintilla_es.ts,
+	qt/qscintilla_fr.ts, qt/qscintilla_pt_br.ts:
+	Updated the translation source files.
+	[ee55692ee907]
+
+	* NEWS, qt/qscilexerhex.cpp, qt/qscilexerhex.h,
+	qt/qscilexerintelhex.cpp, qt/qscilexerintelhex.h,
+	qt/qscilexersrec.cpp, qt/qscilexersrec.h, qt/qscilexertekhex.cpp,
+	qt/qscilexertekhex.h, qt/qscintilla.pro:
+	Added the QsciLexerHex, QsciLexerIntelHex, QsciLexerSRec and
+	QsciLexerTekHex classes.
+	[5e1cb8b52206]
+
+	* Merged the 2.13-maint branch.
+	[a9480b2f6bdb]
+
+2023-03-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, lexlib/LexAccessor.h:
+	Disabled an assert() in the lexer library as the following code
+	handles the case anyway. The real bug is probably in the HTML lexer
+	triggered when the HTML has embedded DTD.
+	[6452e3b634b6] <2.13-maint>
+
+2023-01-15  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 2.13.4 for changeset b2c87a81f0c3
+	[d2bc1ac10aa3] <2.13-maint>
+
 2022-12-06  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, src/EditView.cxx:
 	Fixed horizontally scrolled text overwriting margins when EOLs are
 	visible.
 	[b2c87a81f0c3] [2.13.4] <2.13-maint>
```

### Comparing `PyQt6_QScintilla-2.13.4/LICENSE` & `PyQt6_QScintilla-2.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/NEWS` & `PyQt6_QScintilla-2.14.0/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v2.14.0 24th April 2023
+  - Added the QsciLexerAsm, QsciLexerMASM and QsciLexerNASM classes.
+  - Added the QsciLexerHex, QsciLexerIntelHex, QsciLexerSRec and
+    QsciLexerTekHex classes.
+  - Bug fixes.
+
 v2.13.4 6th December 2022
   - Added the .api files for Python v3.10 and v3.11.
   - Bug fixes.
 
 v2.13.3 25th April 2022
   - Bug fixes.
```

### Comparing `PyQt6_QScintilla-2.13.4/PKG-INFO` & `PyQt6_QScintilla-2.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-QScintilla
-Version: 2.13.4
+Version: 2.14.0
 Requires-Python: >=3.7
 Summary: Python bindings for the QScintilla programmers editor widget
 Home-Page: https://www.riverbankcomputing.com/software/qscintilla/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.0.3)
```

### Comparing `PyQt6_QScintilla-2.13.4/README` & `PyQt6_QScintilla-2.14.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/project.py` & `PyQt6_QScintilla-2.14.0/project.py`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/pyproject.toml` & `PyQt6_QScintilla-2.14.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6.0.2, <7", "PyQt-builder >=1.6, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-QScintilla"
-version = "2.13.4"
+version = "2.14.0"
 summary = "Python bindings for the QScintilla programmers editor widget"
 home-page = "https://www.riverbankcomputing.com/software/qscintilla/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.0.3)"
```

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.4.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.4.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.5.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.5.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.6.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.6.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-2.7.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-2.7.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.1.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.1.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.10.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.10.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.11.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.11.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.2.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.2.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.3.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.3.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.4.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.4.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.5.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.5.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.6.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.6.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.7.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.7.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.8.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.8.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/qsci/api/python/Python-3.9.api` & `PyQt6_QScintilla-2.14.0/qsci/api/python/Python-3.9.api`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/ILexer.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/ILexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/ILoader.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/ILoader.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/License.txt` & `PyQt6_QScintilla-2.14.0/scintilla/include/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/Platform.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/Platform.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/SciLexer.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/SciLexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/Sci_Position.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/Sci_Position.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/Scintilla.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/Scintilla.iface` & `PyQt6_QScintilla-2.14.0/scintilla/include/Scintilla.iface`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/include/ScintillaWidget.h` & `PyQt6_QScintilla-2.14.0/scintilla/include/ScintillaWidget.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexA68k.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexA68k.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAPDL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAPDL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexASY.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexASY.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAU3.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAU3.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAVE.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVE.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAVS.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAVS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAbaqus.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAbaqus.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAda.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAda.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAsm.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsm.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexAsn1.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexAsn1.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBaan.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBaan.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBash.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBash.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBasic.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBasic.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBatch.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBatch.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBibTeX.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBibTeX.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexBullant.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexBullant.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCLW.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCLW.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCOBOL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCOBOL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCPP.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCPP.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCSS.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCSS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCaml.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCaml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCmake.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCmake.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCoffeeScript.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCoffeeScript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexConf.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexConf.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCrontab.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCrontab.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexCsound.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexCsound.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexD.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexD.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexDMAP.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMAP.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexDMIS.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDMIS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexDiff.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexDiff.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexECL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexECL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexEDIFACT.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEDIFACT.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexEScript.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEScript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexEiffel.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexEiffel.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexErlang.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErlang.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexErrorList.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexErrorList.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexFlagship.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFlagship.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexForth.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexForth.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexFortran.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexFortran.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexGAP.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGAP.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexGui4Cli.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexGui4Cli.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexHTML.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHTML.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexHaskell.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHaskell.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexHex.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexHex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexIndent.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexIndent.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexInno.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexInno.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexJSON.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexJSON.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexKVIrc.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKVIrc.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexKix.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexKix.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLPeg.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLPeg.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLaTeX.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLaTeX.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLisp.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLisp.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLout.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLout.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexLua.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexLua.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMMIXAL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMMIXAL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMPT.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMPT.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMSSQL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMSSQL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMagik.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMagik.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMake.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMake.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMarkdown.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMarkdown.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMatlab.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMatlab.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMaxima.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMaxima.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMetapost.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMetapost.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexModula.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexModula.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexMySQL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexMySQL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexNimrod.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNimrod.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexNsis.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNsis.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexNull.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexNull.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexOScript.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOScript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexOpal.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexOpal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPB.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPB.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPLM.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPLM.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPO.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPO.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPOV.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPOV.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPS.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPascal.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPascal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPerl.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPerl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPowerPro.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerPro.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPowerShell.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPowerShell.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexProgress.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProgress.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexProps.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexProps.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexPython.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexPython.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexR.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexR.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRebol.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRebol.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRegistry.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRegistry.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRuby.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRuby.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexRust.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexRust.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSAS.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSAS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSML.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSML.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSQL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSQL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSTTXT.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSTTXT.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexScriptol.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexScriptol.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSmalltalk.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSmalltalk.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSorcus.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSorcus.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSpecman.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpecman.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexSpice.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexSpice.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexStata.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexStata.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTACL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTACL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTADS3.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTADS3.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTAL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTAL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTCL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTCMD.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTCMD.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTeX.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTeX.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexTxt2tags.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexTxt2tags.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVB.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVB.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVHDL.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVHDL.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVerilog.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVerilog.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexVisualProlog.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexVisualProlog.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/LexYAML.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/LexYAML.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexers/License.txt` & `PyQt6_QScintilla-2.14.0/scintilla/lexers/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/Accessor.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/Accessor.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/Accessor.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterCategory.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterCategory.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterCategory.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterSet.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/CharacterSet.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/CharacterSet.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/DefaultLexer.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/DefaultLexer.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/DefaultLexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexAccessor.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexAccessor.h`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 	}
 	void StartSegment(Sci_PositionU pos) {
 		startSeg = pos;
 	}
 	void ColourTo(Sci_PositionU pos, int chAttr) {
 		// Only perform styling if non empty range
 		if (pos != startSeg - 1) {
-			assert(pos >= startSeg);
+			//assert(pos >= startSeg);
 			if (pos < startSeg) {
 				return;
 			}
 
 			if (validLen + (pos - startSeg + 1) >= bufferSize)
 				Flush();
 			const char attr = static_cast<char>(chAttr);
```

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerBase.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerBase.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerBase.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerModule.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerModule.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerModule.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerNoExceptions.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerNoExceptions.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerNoExceptions.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerSimple.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/LexerSimple.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/LexerSimple.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/License.txt` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/OptionSet.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/OptionSet.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/PropSetSimple.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/PropSetSimple.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/PropSetSimple.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/SparseState.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/SparseState.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/StringCopy.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/StringCopy.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/StyleContext.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/StyleContext.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/StyleContext.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/SubStyles.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/SubStyles.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/WordList.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/lexlib/WordList.h` & `PyQt6_QScintilla-2.14.0/scintilla/lexlib/WordList.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/AutoComplete.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/AutoComplete.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/AutoComplete.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CallTip.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CallTip.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/CallTip.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CaseConvert.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CaseConvert.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/CaseConvert.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CaseFolder.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CaseFolder.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/CaseFolder.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Catalogue.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Catalogue.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Catalogue.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CellBuffer.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CellBuffer.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/CellBuffer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CharClassify.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/CharClassify.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/CharClassify.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ContractionState.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ContractionState.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/ContractionState.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/DBCS.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/DBCS.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Decoration.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Decoration.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Decoration.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Document.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Document.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Document.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Document.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/EditModel.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/EditModel.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/EditModel.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/EditView.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/EditView.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/EditView.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/EditView.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Editor.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Editor.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Editor.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Editor.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ElapsedPeriod.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/ElapsedPeriod.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ExternalLexer.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ExternalLexer.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/ExternalLexer.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/FontQuality.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/FontQuality.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Indicator.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Indicator.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Indicator.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/IntegerRectangle.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/IntegerRectangle.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/KeyMap.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/KeyMap.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/KeyMap.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/License.txt` & `PyQt6_QScintilla-2.14.0/scintilla/src/License.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/LineMarker.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/LineMarker.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/LineMarker.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/MarginView.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/MarginView.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/MarginView.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Partitioning.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Partitioning.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/PerLine.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/PerLine.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/PerLine.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Position.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Position.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/PositionCache.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/PositionCache.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/PositionCache.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/RESearch.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/RESearch.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/RESearch.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/RunStyles.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/RunStyles.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/RunStyles.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ScintillaBase.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ScintillaBase.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/ScintillaBase.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Selection.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Selection.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Selection.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Selection.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/SparseVector.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/SparseVector.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/SplitVector.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/SplitVector.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Style.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/Style.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/Style.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/Style.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/UniConversion.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/UniConversion.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/UniConversion.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/UniqueString.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/UniqueString.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ViewStyle.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/ViewStyle.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/ViewStyle.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/XPM.cpp` & `PyQt6_QScintilla-2.14.0/scintilla/src/XPM.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/scintilla/src/XPM.h` & `PyQt6_QScintilla-2.14.0/scintilla/src/XPM.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qsciabstractapis.sip` & `PyQt6_QScintilla-2.14.0/sip/qsciabstractapis.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qsciapis.sip` & `PyQt6_QScintilla-2.14.0/sip/qsciapis.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscicommand.sip` & `PyQt6_QScintilla-2.14.0/sip/qscicommand.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscicommandset.sip` & `PyQt6_QScintilla-2.14.0/sip/qscicommandset.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscidocument.sip` & `PyQt6_QScintilla-2.14.0/sip/qscidocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexer.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexeravs.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexeravs.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerbash.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerbash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerbatch.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerbatch.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexercmake.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexercmake.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexercoffeescript.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexercoffeescript.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexercpp.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexercpp.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexercsharp.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexercsharp.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexercss.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexercss.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexercustom.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexercustom.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerd.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerd.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerdiff.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerdiff.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexeredifact.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexeredifact.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerfortran.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerfortran.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerfortran77.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerfortran77.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerhtml.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerhtml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexeridl.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexeridl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerjava.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerjava.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerjavascript.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerjavascript.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerjson.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerjson.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerlua.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerlua.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexermakefile.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexermakefile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexermarkdown.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexermarkdown.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexermatlab.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexermatlab.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexeroctave.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexeroctave.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerpascal.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerpascal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerperl.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerperl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerpo.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerpo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerpostscript.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerpostscript.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerpov.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerpov.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerproperties.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerproperties.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerpython.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerpython.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerruby.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerruby.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerspice.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerspice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexersql.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexersql.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexertcl.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexertcl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexertex.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexertex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerverilog.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerverilog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexervhdl.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexervhdl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexerxml.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexerxml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscilexeryaml.sip` & `PyQt6_QScintilla-2.14.0/sip/qscilexeryaml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscimacro.sip` & `PyQt6_QScintilla-2.14.0/sip/qscimacro.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscimod5.sip` & `PyQt6_QScintilla-2.14.0/sip/qscimod5.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscimod6.sip` & `PyQt6_QScintilla-2.14.0/sip/qscimod6.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscimodcommon.sip` & `PyQt6_QScintilla-2.14.0/sip/qscimodcommon.sip`

 * *Files 8% similar despite different names*

```diff
@@ -56,48 +56,55 @@
 %Include qsciscintilla.sip
 %Include qsciabstractapis.sip
 %Include qsciapis.sip
 %Include qscicommand.sip
 %Include qscicommandset.sip
 %Include qscidocument.sip
 %Include qscilexer.sip
+%Include qscilexerasm.sip
 %Include qscilexeravs.sip
 %Include qscilexerbash.sip
 %Include qscilexerbatch.sip
 %Include qscilexercmake.sip
 %Include qscilexercoffeescript.sip
 %Include qscilexercpp.sip
 %Include qscilexercsharp.sip
 %Include qscilexercss.sip
 %Include qscilexercustom.sip
 %Include qscilexerd.sip
 %Include qscilexerdiff.sip
 %Include qscilexerfortran.sip
 %Include qscilexerfortran77.sip
+%Include qscilexerhex.sip
 %Include qscilexerhtml.sip
 %Include qscilexeridl.sip
+%Include qscilexerintelhex.sip
 %Include qscilexerjava.sip
 %Include qscilexerjavascript.sip
 %Include qscilexerjson.sip
 %Include qscilexerlua.sip
 %Include qscilexermakefile.sip
 %Include qscilexermarkdown.sip
+%Include qscilexermasm.sip
 %Include qscilexermatlab.sip
+%Include qscilexernasm.sip
 %Include qscilexeroctave.sip
 %Include qscilexerpascal.sip
 %Include qscilexerperl.sip
 %Include qscilexerpostscript.sip
 %Include qscilexerpo.sip
 %Include qscilexerpov.sip
 %Include qscilexerproperties.sip
 %Include qscilexerpython.sip
 %Include qscilexerruby.sip
 %Include qscilexerspice.sip
 %Include qscilexersql.sip
+%Include qscilexersrec.sip
 %Include qscilexertcl.sip
+%Include qscilexertekhex.sip
 %Include qscilexertex.sip
 %Include qscilexerverilog.sip
 %Include qscilexervhdl.sip
 %Include qscilexerxml.sip
 %Include qscilexeryaml.sip
 %Include qscimacro.sip
 %Include qsciprinter.sip
```

### Comparing `PyQt6_QScintilla-2.13.4/sip/qsciprinter.sip` & `PyQt6_QScintilla-2.14.0/sip/qsciprinter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qsciscintilla.sip` & `PyQt6_QScintilla-2.14.0/sip/qsciscintilla.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qsciscintillabase.sip` & `PyQt6_QScintilla-2.14.0/sip/qsciscintillabase.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1392,58 +1392,65 @@
 
 %ConvertToSubClassCode
 static struct class_graph {
     const char *name;
     sipTypeDef **type;
     int yes, no;
 } graph[] = {
-    {sipName_QsciLexer, &sipType_QsciLexer, 4, 1},
-    {sipName_QsciAbstractAPIs, &sipType_QsciAbstractAPIs, 43, 2},
+    {sipName_QsciAbstractAPIs, &sipType_QsciAbstractAPIs, 4, 1},
+    {sipName_QsciLexer, &sipType_QsciLexer, 5, 2},
     {sipName_QsciMacro, &sipType_QsciMacro, -1, 3},
-    {sipName_QsciScintillaBase, &sipType_QsciScintillaBase, 44, -1},
-    {sipName_QsciLexerSQL, &sipType_QsciLexerSQL, -1, 5},
-    {sipName_QsciLexerMakefile, &sipType_QsciLexerMakefile, -1, 6},
-    {sipName_QsciLexerAVS, &sipType_QsciLexerAVS, -1, 7},
-    {sipName_QsciLexerDiff, &sipType_QsciLexerDiff, -1, 8},
-    {sipName_QsciLexerPython, &sipType_QsciLexerPython, -1, 9},
-    {sipName_QsciLexerPO, &sipType_QsciLexerPO, -1, 10},
-    {sipName_QsciLexerCoffeeScript, &sipType_QsciLexerCoffeeScript, -1, 11},
-    {sipName_QsciLexerPostScript, &sipType_QsciLexerPostScript, -1, 12},
-    {sipName_QsciLexerPOV, &sipType_QsciLexerPOV, -1, 13},
-    {sipName_QsciLexerRuby, &sipType_QsciLexerRuby, -1, 14},
-    {sipName_QsciLexerJSON, &sipType_QsciLexerJSON, -1, 15},
-    {sipName_QsciLexerVerilog, &sipType_QsciLexerVerilog, -1, 16},
-    {sipName_QsciLexerProperties, &sipType_QsciLexerProperties, -1, 17},
-    {sipName_QsciLexerCMake, &sipType_QsciLexerCMake, -1, 18},
-    {sipName_QsciLexerD, &sipType_QsciLexerD, -1, 19},
-    {sipName_QsciLexerLua, &sipType_QsciLexerLua, -1, 20},
-    {sipName_QsciLexerPerl, &sipType_QsciLexerPerl, -1, 21},
-    {sipName_QsciLexerBash, &sipType_QsciLexerBash, -1, 22},
-    {sipName_QsciLexerFortran77, &sipType_QsciLexerFortran77, 36, 23},
-    {sipName_QsciLexerVHDL, &sipType_QsciLexerVHDL, -1, 24},
-    {sipName_QsciLexerCSS, &sipType_QsciLexerCSS, -1, 25},
-    {sipName_QsciLexerSpice, &sipType_QsciLexerSpice, -1, 26},
-    {sipName_QsciLexerBatch, &sipType_QsciLexerBatch, -1, 27},
-    {sipName_QsciLexerHTML, &sipType_QsciLexerHTML, 37, 28},
-    {sipName_QsciLexerCustom, &sipType_QsciLexerCustom, -1, 29},
-    {sipName_QsciLexerMatlab, &sipType_QsciLexerMatlab, 38, 30},
-    {sipName_QsciLexerPascal, &sipType_QsciLexerPascal, -1, 31},
-    {sipName_QsciLexerTCL, &sipType_QsciLexerTCL, -1, 32},
-    {sipName_QsciLexerMarkdown, &sipType_QsciLexerMarkdown, -1, 33},
-    {sipName_QsciLexerTeX, &sipType_QsciLexerTeX, -1, 34},
-    {sipName_QsciLexerCPP, &sipType_QsciLexerCPP, 39, 35},
+    {sipName_QsciScintillaBase, &sipType_QsciScintillaBase, 51, -1},
+    {sipName_QsciAPIs, &sipType_QsciAPIs, -1, -1},
+    {sipName_QsciLexerAVS, &sipType_QsciLexerAVS, -1, 6},
+    {sipName_QsciLexerAsm, &sipType_QsciLexerAsm, 39, 7},
+    {sipName_QsciLexerBash, &sipType_QsciLexerBash, -1, 8},
+    {sipName_QsciLexerBatch, &sipType_QsciLexerBatch, -1, 9},
+    {sipName_QsciLexerCMake, &sipType_QsciLexerCMake, -1, 10},
+    {sipName_QsciLexerCPP, &sipType_QsciLexerCPP, 41, 11},
+    {sipName_QsciLexerCSS, &sipType_QsciLexerCSS, -1, 12},
+    {sipName_QsciLexerCoffeeScript, &sipType_QsciLexerCoffeeScript, -1, 13},
+    {sipName_QsciLexerCustom, &sipType_QsciLexerCustom, -1, 14},
+    {sipName_QsciLexerD, &sipType_QsciLexerD, -1, 15},
+    {sipName_QsciLexerDiff, &sipType_QsciLexerDiff, -1, 16},
+    {sipName_QsciLexerFortran77, &sipType_QsciLexerFortran77, 45, 17},
+    {sipName_QsciLexerHTML, &sipType_QsciLexerHTML, 46, 18},
+    {sipName_QsciLexerHex, &sipType_QsciLexerHex, 47, 19},
+    {sipName_QsciLexerJSON, &sipType_QsciLexerJSON, -1, 20},
+    {sipName_QsciLexerLua, &sipType_QsciLexerLua, -1, 21},
+    {sipName_QsciLexerMakefile, &sipType_QsciLexerMakefile, -1, 22},
+    {sipName_QsciLexerMarkdown, &sipType_QsciLexerMarkdown, -1, 23},
+    {sipName_QsciLexerMatlab, &sipType_QsciLexerMatlab, 50, 24},
+    {sipName_QsciLexerPO, &sipType_QsciLexerPO, -1, 25},
+    {sipName_QsciLexerPOV, &sipType_QsciLexerPOV, -1, 26},
+    {sipName_QsciLexerPascal, &sipType_QsciLexerPascal, -1, 27},
+    {sipName_QsciLexerPerl, &sipType_QsciLexerPerl, -1, 28},
+    {sipName_QsciLexerPostScript, &sipType_QsciLexerPostScript, -1, 29},
+    {sipName_QsciLexerProperties, &sipType_QsciLexerProperties, -1, 30},
+    {sipName_QsciLexerPython, &sipType_QsciLexerPython, -1, 31},
+    {sipName_QsciLexerRuby, &sipType_QsciLexerRuby, -1, 32},
+    {sipName_QsciLexerSQL, &sipType_QsciLexerSQL, -1, 33},
+    {sipName_QsciLexerSpice, &sipType_QsciLexerSpice, -1, 34},
+    {sipName_QsciLexerTCL, &sipType_QsciLexerTCL, -1, 35},
+    {sipName_QsciLexerTeX, &sipType_QsciLexerTeX, -1, 36},
+    {sipName_QsciLexerVHDL, &sipType_QsciLexerVHDL, -1, 37},
+    {sipName_QsciLexerVerilog, &sipType_QsciLexerVerilog, -1, 38},
     {sipName_QsciLexerYAML, &sipType_QsciLexerYAML, -1, -1},
+    {sipName_QsciLexerMASM, &sipType_QsciLexerMASM, -1, 40},
+    {sipName_QsciLexerNASM, &sipType_QsciLexerNASM, -1, -1},
+    {sipName_QsciLexerCSharp, &sipType_QsciLexerCSharp, -1, 42},
+    {sipName_QsciLexerIDL, &sipType_QsciLexerIDL, -1, 43},
+    {sipName_QsciLexerJava, &sipType_QsciLexerJava, -1, 44},
+    {sipName_QsciLexerJavaScript, &sipType_QsciLexerJavaScript, -1, -1},
     {sipName_QsciLexerFortran, &sipType_QsciLexerFortran, -1, -1},
     {sipName_QsciLexerXML, &sipType_QsciLexerXML, -1, -1},
+    {sipName_QsciLexerIntelHex, &sipType_QsciLexerIntelHex, -1, 48},
+    {sipName_QsciLexerSRec, &sipType_QsciLexerSRec, -1, 49},
+    {sipName_QsciLexerTekHex, &sipType_QsciLexerTekHex, -1, -1},
     {sipName_QsciLexerOctave, &sipType_QsciLexerOctave, -1, -1},
-    {sipName_QsciLexerCSharp, &sipType_QsciLexerCSharp, -1, 40},
-    {sipName_QsciLexerJavaScript, &sipType_QsciLexerJavaScript, -1, 41},
-    {sipName_QsciLexerIDL, &sipType_QsciLexerIDL, -1, 42},
-    {sipName_QsciLexerJava, &sipType_QsciLexerJava, -1, -1},
-    {sipName_QsciAPIs, &sipType_QsciAPIs, -1, -1},
     {sipName_QsciScintilla, &sipType_QsciScintilla, -1, -1},
 };
 
 int i = 0;
 
 sipType = NULL;
```

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscistyle.sip` & `PyQt6_QScintilla-2.14.0/sip/qscistyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/sip/qscistyledtext.sip` & `PyQt6_QScintilla-2.14.0/sip/qscistyledtext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/InputMethod.cpp` & `PyQt6_QScintilla-2.14.0/src/InputMethod.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -260,22 +260,22 @@
 
             Sci_TextRange textRange;
             textRange.chrg = charRange;
             textRange.lpstrText = buffer.data();
 
             SendScintilla(SCI_GETTEXTRANGE, 0, (sptr_t)&textRange);
 
-            return bytesAsText(buffer.constData());
+            return bytesAsText(buffer.constData(), buffer.size());
         }
 
         case Qt::ImCurrentSelection:
         {
-            QVarLengthArray<char,1024> buffer(SendScintilla(SCI_GETSELTEXT));
+            QVarLengthArray<char,1024> buffer(SendScintilla(SCI_GETSELTEXT) + 1);
             SendScintilla(SCI_GETSELTEXT, 0, (sptr_t)buffer.data());
 
-            return bytesAsText(buffer.constData());
+            return bytesAsText(buffer.constData(), buffer.size() - 1);
         }
 
         default:
             return QVariant();
     }
 }
```

### Comparing `PyQt6_QScintilla-2.13.4/src/ListBoxQt.cpp` & `PyQt6_QScintilla-2.14.0/src/ListBoxQt.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/ListBoxQt.h` & `PyQt6_QScintilla-2.14.0/src/ListBoxQt.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/MacPasteboardMime.cpp` & `PyQt6_QScintilla-2.14.0/src/MacPasteboardMime.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/PlatQt.cpp` & `PyQt6_QScintilla-2.14.0/src/PlatQt.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qsciabstractapis.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qsciabstractapis.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qsciapis.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qsciapis.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscicommand.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscicommand.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscicommandset.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscicommandset.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscidocument.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscidocument.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qsciglobal.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qsciglobal.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 #ifndef QSCIGLOBAL_H
 #define QSCIGLOBAL_H
 
 #include <qglobal.h>
 
 
-#define QSCINTILLA_VERSION      0x020d04
-#define QSCINTILLA_VERSION_STR  "2.13.4"
+#define QSCINTILLA_VERSION      0x020e00
+#define QSCINTILLA_VERSION_STR  "2.14.0"
 
 
 // We only support Qt v5.11 and later.
 #if QT_VERSION < 0x050b00
 #error "Qt v5.11.0 or later is required"
 #endif
```

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexer.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexer.h`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,20 @@
 
     //! The lexer's properties are written to the settings \a qs.
     //! \a prefix (which has a trailing '/') should be used as a prefix to
     //! the key of each setting.  true is returned if there is no error.
     //!
     virtual bool writeProperties(QSettings &qs,const QString &prefix) const;
 
+    //! \internal Convert a QString to encoded bytes.
+    QByteArray textAsBytes(const QString &text) const;
+
+    //! \internal Convert encoded bytes to a QString.
+    QString bytesAsText(const char *bytes, int size) const;
+
 private:
     struct StyleData {
         QFont font;
         QColor color;
         QColor paper;
         bool eol_fill;
     };
```

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeravs.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeravs.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerbash.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbash.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerbatch.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerbatch.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercmake.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercmake.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercoffeescript.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercoffeescript.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercpp.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercpp.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercsharp.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercsharp.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercss.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercss.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexercustom.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexercustom.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerd.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerd.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerdiff.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerdiff.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeredifact.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeredifact.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerfortran.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerfortran77.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerfortran77.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerhtml.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerhtml.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeridl.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeridl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerjava.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjava.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerjavascript.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjavascript.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerjson.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerjson.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerlua.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerlua.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexermakefile.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermakefile.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexermarkdown.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermarkdown.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexermatlab.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexermatlab.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeroctave.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeroctave.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpascal.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpascal.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerperl.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerperl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpo.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpo.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpostscript.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpostscript.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpov.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpov.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerproperties.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerproperties.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerpython.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerpython.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerruby.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerruby.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerspice.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerspice.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexersql.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexersql.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexertcl.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertcl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexertex.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexertex.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerverilog.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerverilog.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexervhdl.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexervhdl.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexerxml.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexerxml.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscilexeryaml.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscilexeryaml.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscimacro.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscimacro.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qsciprinter.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qsciprinter.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qsciscintilla.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintilla.h`

 * *Files 0% similar despite different names*

```diff
@@ -2238,15 +2238,15 @@
 
     bool ensureRW();
     void insertAtPos(const QString &text, int pos);
     static int mapModifiers(int modifiers);
 
     QString wordAtPosition(int position) const;
 
-    ScintillaBytes styleText(const QList<QsciStyledText> &styled_text,
+    QByteArray styleText(const QList<QsciStyledText> &styled_text,
             char **styles, int style_offset = 0);
 
     struct FindState
     {
         enum Status
         {
             Finding,
```

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qsciscintillabase.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qsciscintillabase.h`

 * *Files 0% similar despite different names*

```diff
@@ -3841,24 +3841,23 @@
 
     //! \internal Re-implemented to handle scrolling.
     virtual void scrollContentsBy(int dx, int dy);
 
     //! \internal This helps to work around some Scintilla bugs.
     void setScrollBars();
 
-    //! \internal Qt4, Qt5 portability.
-    typedef QByteArray ScintillaBytes;
-
-#define ScintillaBytesConstData(b)  (b).constData()
-
     //! \internal Convert a QString to encoded bytes.
-    ScintillaBytes textAsBytes(const QString &text) const;
+    QByteArray textAsBytes(const QString &text) const;
 
     //! \internal Convert encoded bytes to a QString.
-    QString bytesAsText(const char *bytes) const;
+    QString bytesAsText(const char *bytes, int size) const;
+
+    //! Give access to the text convertors.
+    friend class QsciAccessibleScintillaBase;
+    friend class QsciLexer;
 
     //! \internal A helper for QsciScintilla::contextMenuEvent().
     bool contextMenuNeeded(int x, int y) const;
 
 private slots:
     void handleVSb(int value);
     void handleHSb(int value);
```

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscistyle.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscistyle.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/Qsci/qscistyledtext.h` & `PyQt6_QScintilla-2.14.0/src/Qsci/qscistyledtext.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/SciAccessibility.cpp` & `PyQt6_QScintilla-2.14.0/src/SciAccessibility.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 // Update the accessibility when text has been inserted.
 void QsciAccessibleScintillaBase::textInserted(QsciScintillaBase *sb,
         int position, const char *text, int length)
 {
     Q_ASSERT(text);
 
-    QString new_text = bytesAsText(sb, text, length);
+    QString new_text = sb->bytesAsText(text, length);
     int offset = positionAsOffset(sb, position);
 
     QAccessibleTextInsertEvent ev(sb, offset, new_text);
     QAccessible::updateAccessibility(&ev);
 }
 
 
@@ -216,15 +216,15 @@
 
 // Update the accessibility when text has been deleted.
 void QsciAccessibleScintillaBase::textDeleted(QsciScintillaBase *sb,
         int position, const char *text, int length)
 {
     Q_ASSERT(text);
 
-    QString old_text = bytesAsText(sb, text, length);
+    QString old_text = sb->bytesAsText(text, length);
     int offset = positionAsOffset(sb, position);
 
     QAccessibleTextRemoveEvent ev(sb, offset, old_text);
     QAccessible::updateAccessibility(&ev);
 }
 
 
@@ -355,37 +355,15 @@
         int start_position, int end_position)
 {
     QByteArray bytes(end_position - start_position + 1, '\0');
 
     sb->SendScintilla(QsciScintillaBase::SCI_GETTEXTRANGE, start_position,
             end_position, bytes.data());
 
-    return bytesAsText(sb, bytes.constData(), bytes.size() - 1);
-}
-
-
-// Convert bytes to text.
-QString QsciAccessibleScintillaBase::bytesAsText(QsciScintillaBase *sb,
-        const char *bytes, int length)
-{
-    if (sb->SendScintilla(QsciScintillaBase::SCI_GETCODEPAGE) == QsciScintillaBase::SC_CP_UTF8)
-        return QString::fromUtf8(bytes, length);
-
-    return QString::fromLatin1(bytes, length);
-}
-
-
-// Convert text to bytes.
-QByteArray QsciAccessibleScintillaBase::textAsBytes(QsciScintillaBase *sb,
-        const QString &text)
-{
-    if (sb->SendScintilla(QsciScintillaBase::SCI_GETCODEPAGE) == QsciScintillaBase::SC_CP_UTF8)
-        return text.toUtf8();
-
-    return text.toLatin1();
+    return sb->bytesAsText(bytes.constData(), bytes.size() - 1);
 }
 
 
 // Convert a byte position to a character offset.
 int QsciAccessibleScintillaBase::positionAsOffset(QsciScintillaBase *sb,
         int position)
 {
@@ -698,27 +676,27 @@
 
 // Insert some text.
 void QsciAccessibleScintillaBase::insertText(int offset, const QString &text)
 {
     QsciScintillaBase *sb = sciWidget();
 
     sb->SendScintilla(QsciScintillaBase::SCI_INSERTTEXT,
-            offsetAsPosition(sb, offset), textAsBytes(sb, text).constData());
+            offsetAsPosition(sb, offset), sb->textAsBytes(text).constData());
 }
 
 
 // Replace some text.
 void QsciAccessibleScintillaBase::replaceText(int startOffset, int endOffset,
         const QString &text)
 {
     QsciScintillaBase *sb = sciWidget();
 
     addSelection(startOffset, endOffset);
     sb->SendScintilla(QsciScintillaBase::SCI_REPLACESEL,
-            textAsBytes(sb, text).constData());
+            sb->textAsBytes(text).constData());
 }
 
 
 // Return the state.
 QAccessible::State QsciAccessibleScintillaBase::state() const
 {
     QAccessible::State st = QAccessibleWidget::state();
```

### Comparing `PyQt6_QScintilla-2.13.4/src/SciAccessibility.h` & `PyQt6_QScintilla-2.14.0/src/SciAccessibility.h`

 * *Files 3% similar despite different names*

```diff
@@ -98,17 +98,14 @@
     QsciScintillaBase *sciWidget() const;
     int validPosition(int offset) const;
     static bool boundaries(QsciScintillaBase *sb, int position,
             QAccessible::TextBoundaryType boundaryType, int *start_position,
             int *end_position);
     static QString textRange(QsciScintillaBase *sb, int start_position,
             int end_position);
-    static QString bytesAsText(QsciScintillaBase *sb, const char *bytes,
-            int length);
-    static QByteArray textAsBytes(QsciScintillaBase *sb, const QString &text);
     static int positionAsOffset(QsciScintillaBase *sb, int position);
     static void positionRangeAsOffsetRange(QsciScintillaBase *sb,
             int start_position, int end_position, int *startOffset,
             int *endOffset);
     static int offsetAsPosition(QsciScintillaBase *sb, int offset);
     static QString colourAsRGB(int colour);
     static void addAttribute(QString &attrs, const char *name,
```

### Comparing `PyQt6_QScintilla-2.13.4/src/SciClasses.cpp` & `PyQt6_QScintilla-2.14.0/src/SciClasses.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/SciClasses.h` & `PyQt6_QScintilla-2.14.0/src/SciClasses.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/ScintillaQt.cpp` & `PyQt6_QScintilla-2.14.0/src/ScintillaQt.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/ScintillaQt.h` & `PyQt6_QScintilla-2.14.0/src/ScintillaQt.h`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/features/qscintilla2.prf` & `PyQt6_QScintilla-2.14.0/src/features/qscintilla2.prf`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qsciabstractapis.cpp` & `PyQt6_QScintilla-2.14.0/src/qsciabstractapis.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qsciapis.cpp` & `PyQt6_QScintilla-2.14.0/src/qsciapis.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscicommand.cpp` & `PyQt6_QScintilla-2.14.0/src/qscicommand.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscicommandset.cpp` & `PyQt6_QScintilla-2.14.0/src/qscicommandset.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscidocument.cpp` & `PyQt6_QScintilla-2.14.0/src/qscidocument.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexer.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexer.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -725,7 +725,25 @@
         for (int i = 0; i <= QsciScintillaBase::STYLE_MAX; ++i)
             if (!description(i).isEmpty())
                 setPaper(c, i);
 
         emit paperChanged(c, QsciScintillaBase::STYLE_DEFAULT);
     }
 }
+
+
+// Encode a QString as bytes.
+QByteArray QsciLexer::textAsBytes(const QString &text) const
+{
+    Q_ASSERT(attached_editor);
+
+    return attached_editor->textAsBytes(text);
+}
+
+
+// Decode bytes as a QString.
+QString QsciLexer::bytesAsText(const char *bytes, int size) const
+{
+    Q_ASSERT(attached_editor);
+
+    return attached_editor->bytesAsText(bytes, size);
+}
```

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexeravs.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexeravs.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerbash.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerbash.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerbatch.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerbatch.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexercmake.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexercmake.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexercoffeescript.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexercoffeescript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexercpp.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexercpp.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexercsharp.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexercsharp.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexercss.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexercss.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexercustom.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexercustom.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerd.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerd.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerdiff.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerdiff.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexeredifact.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexeredifact.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerfortran.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerfortran.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerfortran77.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerfortran77.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerhtml.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerhtml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexeridl.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexeridl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerjava.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerjava.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerjavascript.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerjavascript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerjson.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerjson.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerlua.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerlua.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexermakefile.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexermakefile.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexermarkdown.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexermarkdown.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexermatlab.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexermatlab.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexeroctave.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexeroctave.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerpascal.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerpascal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerperl.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerperl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerpo.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerpo.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerpostscript.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerpostscript.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerpov.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerpov.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerproperties.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerproperties.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerpython.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerpython.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerruby.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerruby.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerspice.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerspice.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexersql.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexersql.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexertcl.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexertcl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexertex.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexertex.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerverilog.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerverilog.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexervhdl.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexervhdl.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexerxml.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexerxml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscilexeryaml.cpp` & `PyQt6_QScintilla-2.14.0/src/qscilexeryaml.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscimacro.cpp` & `PyQt6_QScintilla-2.14.0/src/qscimacro.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscintilla.pro` & `PyQt6_QScintilla-2.14.0/src/qscintilla.pro`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # then you may purchase a commercial license.  For more information contact
 # info@riverbankcomputing.com.
 # 
 # This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 # WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-!win32:VERSION = 15.1.1
+!win32:VERSION = 15.2.0
 
 TEMPLATE = lib
 CONFIG += qt warn_off thread exceptions hide_symbols
 
 CONFIG(debug, debug|release) {
     mac: {
         TARGET = qscintilla2_qt$${QT_MAJOR_VERSION}_debug
@@ -99,49 +99,56 @@
     ./Qsci/qsciscintillabase.h \
     ./Qsci/qsciabstractapis.h \
     ./Qsci/qsciapis.h \
     ./Qsci/qscicommand.h \
     ./Qsci/qscicommandset.h \
     ./Qsci/qscidocument.h \
     ./Qsci/qscilexer.h \
+    ./Qsci/qscilexerasm.h \
     ./Qsci/qscilexeravs.h \
     ./Qsci/qscilexerbash.h \
     ./Qsci/qscilexerbatch.h \
     ./Qsci/qscilexercmake.h \
     ./Qsci/qscilexercoffeescript.h \
     ./Qsci/qscilexercpp.h \
     ./Qsci/qscilexercsharp.h \
     ./Qsci/qscilexercss.h \
     ./Qsci/qscilexercustom.h \
     ./Qsci/qscilexerd.h \
     ./Qsci/qscilexerdiff.h \
     ./Qsci/qscilexeredifact.h \
     ./Qsci/qscilexerfortran.h \
     ./Qsci/qscilexerfortran77.h \
+    ./Qsci/qscilexerhex.h \
     ./Qsci/qscilexerhtml.h \
     ./Qsci/qscilexeridl.h \
+    ./Qsci/qscilexerintelhex.h \
     ./Qsci/qscilexerjava.h \
     ./Qsci/qscilexerjavascript.h \
     ./Qsci/qscilexerjson.h \
     ./Qsci/qscilexerlua.h \
     ./Qsci/qscilexermakefile.h \
     ./Qsci/qscilexermarkdown.h \
+    ./Qsci/qscilexermasm.h \
     ./Qsci/qscilexermatlab.h \
+    ./Qsci/qscilexernasm.h \
     ./Qsci/qscilexeroctave.h \
     ./Qsci/qscilexerpascal.h \
     ./Qsci/qscilexerperl.h \
     ./Qsci/qscilexerpostscript.h \
     ./Qsci/qscilexerpo.h \
     ./Qsci/qscilexerpov.h \
     ./Qsci/qscilexerproperties.h \
     ./Qsci/qscilexerpython.h \
     ./Qsci/qscilexerruby.h \
     ./Qsci/qscilexerspice.h \
     ./Qsci/qscilexersql.h \
+    ./Qsci/qscilexersrec.h \
     ./Qsci/qscilexertcl.h \
+    ./Qsci/qscilexertekhex.h \
     ./Qsci/qscilexertex.h \
     ./Qsci/qscilexerverilog.h \
     ./Qsci/qscilexervhdl.h \
     ./Qsci/qscilexerxml.h \
     ./Qsci/qscilexeryaml.h \
     ./Qsci/qscimacro.h \
     ./Qsci/qscistyle.h \
@@ -218,49 +225,56 @@
     qsciscintillabase.cpp \
     qsciabstractapis.cpp \
     qsciapis.cpp \
     qscicommand.cpp \
     qscicommandset.cpp \
     qscidocument.cpp \
     qscilexer.cpp \
+    qscilexerasm.cpp \
     qscilexeravs.cpp \
     qscilexerbash.cpp \
     qscilexerbatch.cpp \
     qscilexercmake.cpp \
     qscilexercoffeescript.cpp \
     qscilexercpp.cpp \
     qscilexercsharp.cpp \
     qscilexercss.cpp \
     qscilexercustom.cpp \
     qscilexerd.cpp \
     qscilexerdiff.cpp \
     qscilexeredifact.cpp \
     qscilexerfortran.cpp \
     qscilexerfortran77.cpp \
+    qscilexerhex.cpp \
     qscilexerhtml.cpp \
     qscilexeridl.cpp \
+    qscilexerintelhex.cpp \
     qscilexerjava.cpp \
     qscilexerjavascript.cpp \
     qscilexerjson.cpp \
     qscilexerlua.cpp \
     qscilexermakefile.cpp \
     qscilexermarkdown.cpp \
+    qscilexermasm.cpp \
     qscilexermatlab.cpp \
+    qscilexernasm.cpp \
     qscilexeroctave.cpp \
     qscilexerpascal.cpp \
     qscilexerperl.cpp \
     qscilexerpostscript.cpp \
     qscilexerpo.cpp \
     qscilexerpov.cpp \
     qscilexerproperties.cpp \
     qscilexerpython.cpp \
     qscilexerruby.cpp \
     qscilexerspice.cpp \
     qscilexersql.cpp \
+    qscilexersrec.cpp \
     qscilexertcl.cpp \
+    qscilexertekhex.cpp \
     qscilexertex.cpp \
     qscilexerverilog.cpp \
     qscilexervhdl.cpp \
     qscilexerxml.cpp \
     qscilexeryaml.cpp \
     qscimacro.cpp \
     qscistyle.cpp \
```

### Comparing `PyQt6_QScintilla-2.13.4/src/qscintilla_cs.qm` & `PyQt6_QScintilla-2.14.0/src/qscintilla_cs.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscintilla_de.qm` & `PyQt6_QScintilla-2.14.0/src/qscintilla_de.qm`

 * *Files 1% similar despite different names*

```diff
@@ -1,4992 +1,5172 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: 4200 0018 9800 004e 6900 00aa 7200 0051  B......Ni...r..Q
-00000020: c900 00e5 b800 0055 3400 00d7 d000 0055  .......U4......U
-00000030: 3400 00f4 bd00 005a 7700 005f 9200 005a  4......Zw.._...Z
-00000040: 7700 00a5 ab00 00d4 7700 0113 4a00 04a7  w.......w...J...
-00000050: d400 011e 8600 04e8 9800 00d6 4e00 0530  ............N..0
-00000060: 4b00 00bb 1300 0548 3500 00e3 ac00 05a9  K......H5.......
-00000070: d400 00a9 7400 05ac f400 00e4 7300 05ac  ....t.......s...
-00000080: f400 0106 de00 0949 2400 004c 2000 0949  .......I$..L ..I
-00000090: 2400 010d 2f00 12dd 5400 00bc 4700 2783  $.../...T...G.'.
-000000a0: 7400 00c4 7000 295b c400 00a7 4700 2aa6  t...p.)[....G.*.
-000000b0: 7900 011d 8d00 2b8b af00 011e 0000 2bc4  y.....+.......+.
-000000c0: af00 011e 4900 390e 0700 0090 d800 426d  ....I.9.......Bm
-000000d0: ad00 00ce 0c00 4786 8100 008b 0800 4898  ......G.......H.
-000000e0: 8900 00d0 2a00 4c99 6200 0038 e100 4c99  ....*.L.b..8..L.
-000000f0: 6200 00b4 9000 4c99 6200 00d5 7f00 4c99  b.....L.b.....L.
-00000100: 6200 00f1 b800 4d27 e300 00c1 3400 4e96  b.....M'....4.N.
-00000110: c000 0106 4300 5278 bc00 003d 5200 5278  ....C.Rx...=R.Rx
-00000120: bc00 003f 3000 5278 bc00 007a fe00 5278  ...?0.Rx...z..Rx
-00000130: bc00 00af ee00 568a a500 002b b200 5c83  ......V....+..\.
-00000140: b500 0060 7c00 5c83 b500 00ff 6900 5e0a  ...`|.\.....i.^.
-00000150: 7400 00a1 b100 63b6 c200 00fa 7100 6fba  t.....c.....q.o.
-00000160: b400 008a 7100 73e0 e700 00a0 7e00 7aaa  ....q.s.....~.z.
-00000170: fe00 00f6 1400 7b90 0700 007d a700 7c3e  ......{....}..|>
-00000180: 0400 0048 9900 9656 4500 00f3 8000 9eeb  ...H...VE.......
-00000190: 0500 001a 7100 a3b3 d200 0092 4200 a5d2  ....q.......B...
-000001a0: f700 0081 1100 ad34 7e00 0079 b600 b6da  .......4~..y....
-000001b0: b400 008f a800 c71a f400 00f8 ff00 cc2f  .............../
-000001c0: f500 0028 f900 ccdb 8500 00c5 f300 cee5  ...(............
-000001d0: 2500 004d 0700 e46f f200 00b1 3a00 e46f  %..M...o....:..o
-000001e0: f200 00b5 0500 f365 e200 00a8 5401 05ba  .......e....T...
-000001f0: a500 002a 1f01 1726 0200 0003 0701 1ef5  ...*...&........
-00000200: 5e00 0078 5e01 2035 2700 0046 d101 2826  ^..x^. 5'..F..(&
-00000210: 3b00 0111 7601 2fc0 ab00 003e 7001 3311  ;...v./....>p.3.
-00000220: f900 00d0 c501 3a8d eb00 003f cf01 3d5a  ......:....?..=Z
-00000230: d400 0017 4101 466b 7900 00db 2601 52bd  ....A.Fky...&.R.
-00000240: 3500 001e e201 65f6 9e00 0032 d301 77a7  5.....e....2..w.
-00000250: 7400 0033 4c01 77a7 7400 0061 5001 77a7  t..3L.w.t..aP.w.
-00000260: 7400 006a dc01 77a7 7400 00a9 a101 7b82  t..j..w.t.....{.
-00000270: d500 002d d001 7bf2 0200 0021 7301 7fc3  ...-..{....!s...
-00000280: 7400 009a f601 7fe4 6900 0065 6201 99f5  t.......i..eb...
-00000290: 3400 00c3 3201 9b25 d400 0022 3401 a414  4...2..%..."4...
-000002a0: f400 0096 b201 a8b8 f400 0103 6401 a93e  ............d..>
-000002b0: 5e00 0110 8a01 a96c 2200 00df d601 b22f  ^......l"....../
-000002c0: 5700 00c1 6d01 b485 7500 0030 5801 c16d  W...m...u..0X..m
-000002d0: 8500 00c6 8101 c16d 8500 00f7 0201 c16d  .......m.......m
-000002e0: 8500 0100 b401 c16d 8500 0107 cc01 d0e6  .......m........
-000002f0: d400 0035 3e01 d0e6 d400 0039 bb01 d0e6  ...5>......9....
-00000300: d400 003d 0e01 d0e6 d400 0055 7801 d0e6  ...=.......Ux...
-00000310: d400 0067 6f01 d0e6 d400 006d a201 d0e6  ...go......m....
-00000320: d400 007a b601 d0e6 d400 00af ac01 d0e6  ...z............
-00000330: d400 00bf a301 d0e6 d400 00ce 5a01 d0e6  ............Z...
-00000340: d400 00d7 2301 d0e6 d400 00e3 2601 d0e6  ....#.......&...
-00000350: d400 00e9 9b01 d0e6 d400 00f3 d101 d0e6  ................
-00000360: d400 00f9 5701 d0e6 d400 0108 8f01 d0e6  ....W...........
-00000370: d400 011b e701 d127 7200 011d 3201 d2fb  .......'r...2...
-00000380: 8900 00d1 b801 d58b f400 0103 ef01 dafa  ................
-00000390: 2e00 0006 ea01 e08e 8900 005a d501 e09e  ...........Z....
-000003a0: 8900 005b 2301 e0fe 8900 005a 8701 e205  ...[#......Z....
-000003b0: 1200 00e8 eb01 e2f8 b300 0044 8701 e540  ...........D...@
-000003c0: 5500 0000 3801 e5b1 e500 0000 bf02 09aa  U...8...........
-000003d0: c500 0081 f802 0cb1 d700 00ec 6402 21cd  ............d.!.
-000003e0: c200 011b 5102 231d f500 00f4 1402 4e68  ....Q.#.......Nh
-000003f0: f800 002b 5102 64fc b900 00d3 7a02 66c1  ...+Q.d.....z.f.
-00000400: 0400 0049 1402 6810 3200 0009 1d02 8065  ...I..h.2......e
-00000410: 9e00 0115 3202 819c 5500 00c3 9502 8285  ....2...U.......
-00000420: 8300 0111 ec02 87f3 7d00 00bb 4f02 9862  ........}...O..b
-00000430: ce00 0109 3c02 a25f d700 0099 8e02 b68a  ....<.._........
-00000440: a500 011d c602 c834 7700 004c 7502 d00a  .......4w..Lu...
-00000450: b500 010a 2e02 d339 5500 000d 3202 d370  .......9U...2..p
-00000460: c500 000d e402 d3ab 9e00 0117 2c02 d53b  ............,..;
-00000470: 2500 0109 e202 f164 f200 004e c602 f164  %......d...N...d
-00000480: f200 010f e203 0440 0200 00fe 4003 0ac8  .......@....@...
-00000490: 2c00 00e3 6f03 0e06 7500 002b 0303 104f  ,...o...u..+...O
-000004a0: e500 002a ab03 370c 9200 006b a903 3c39  ...*..7....k..<9
-000004b0: 7400 0006 9003 4ae8 3800 0074 0703 56ee  t.....J.8..t..V.
-000004c0: 8900 0033 9603 57b3 9400 008c 1503 6dfe  ...3..W.......m.
-000004d0: 4400 001b 5a03 81d1 5500 0001 4403 8513  D...Z...U...D...
-000004e0: 2400 0088 c303 85ae 0200 0097 9503 88be  $...............
-000004f0: f500 00dd d203 8c84 b400 0020 b603 8f4d  ........... ...M
-00000500: be00 00ff 9903 94e4 de00 0061 a303 a5ed  ...........a....
-00000510: 1500 0030 dc03 aa7b 0700 0041 7f03 b99a  ...0...{...A....
-00000520: a400 0047 4503 bcc8 2400 006c fb03 c16f  ...GE...$..l...o
-00000530: b500 00f6 7903 cf1c a500 0001 f103 d537  ....y..........7
-00000540: 5400 00cc 1b03 dfea 1500 00c4 d503 e18f  T...............
-00000550: 1400 005e de03 f13f 9200 009a a103 f333  ...^...?.......3
-00000560: 1300 0031 d403 f8c5 f200 0004 8504 06b2  ...1............
-00000570: 3300 0118 3b04 07e7 9700 008d e104 248a  3...;.........$.
-00000580: 0500 0022 9c04 349c 2500 005a 1804 51f1  ..."..4.%..Z..Q.
-00000590: a500 001b eb04 5ba5 e500 001f 9204 5bee  ......[.......[.
-000005a0: 7500 001f 3604 668a d300 0060 1904 6c26  u...6.f....`..l&
-000005b0: f700 0097 db04 7f08 4500 000c 6404 8d5a  ........E...d..Z
-000005c0: 6b00 0117 e204 8f89 4700 0059 7f04 960d  k.......G..Y....
-000005d0: 8500 0014 8704 9849 bc00 0000 0004 a1ae  .......I........
-000005e0: 6300 004d 6e04 a45b 7400 0063 7204 ac2c  c..Mn..[t..cr..,
-000005f0: a500 011e c604 b9c3 7400 0063 1d04 c1d3  ........t..c....
-00000600: 7e00 0001 a304 c5b0 b900 008b df04 d03a  ~..............:
-00000610: c200 0034 9304 d228 5400 00c1 b904 d509  ...4...(T.......
-00000620: 3400 009d ab04 d549 9e00 010e 6804 d7eb  4......I....h...
-00000630: a400 00a6 f104 dbd9 e500 0015 f504 e358  ...............X
-00000640: 7c00 00f2 5c04 eb7a c200 0073 9104 f427  |...\..z...s...'
-00000650: f400 006e 2b04 f7f9 4400 010c d404 ffbb  ...n+...D.......
-00000660: 9300 00bc 9505 05df 1400 00a0 be05 07bd  ................
-00000670: 0e00 0068 9305 07bd 0e00 00ad 8705 07bd  ...h............
-00000680: 0e00 00db c305 07bd 0e00 00f4 e805 0d9f  ................
-00000690: 9500 0044 3b05 0d9f 9500 00aa 2505 0df2  ...D;.......%...
-000006a0: f700 0093 ee05 0e76 7800 000f ba05 1736  .......vx......6
-000006b0: ee00 00de 3005 1736 ee00 0103 2505 1763  ....0..6....%..c
-000006c0: 7400 0084 9d05 2054 e400 007d 4105 243c  t..... T...}A.$<
-000006d0: c400 0090 7e05 2a8e 7400 00c2 0605 2c5f  ....~.*.t.....,_
-000006e0: 9700 0083 1105 40d9 4100 0070 7905 40d9  ......@.A..py.@.
-000006f0: 4100 00b2 c805 40d9 4100 00ca 3505 40d9  A.....@.A...5.@.
-00000700: 4100 00fc 4805 40d9 4100 0104 3a05 40d9  A...H.@.A...:.@.
-00000710: 4200 0070 ca05 40d9 4200 00b3 1b05 40d9  B..p..@.B.....@.
-00000720: 4200 00ca 8805 40d9 4200 00fc 9b05 40d9  B.....@.B.....@.
-00000730: 4200 0104 8d05 40d9 4300 0071 1b05 40d9  B.....@.C..q..@.
-00000740: 4300 00b3 6e05 40d9 4300 00ca db05 40d9  C...n.@.C.....@.
-00000750: 4300 00fc ee05 40d9 4300 0104 e005 40d9  C.....@.C.....@.
-00000760: 4400 00b3 c105 40d9 4400 00fd 4105 40d9  D.....@.D...A.@.
-00000770: 4400 0105 3305 41e3 1300 005e 9905 4207  D...3.A....^..B.
-00000780: 9400 006f 3805 48a6 f400 00aa 9d05 5b93  ...o8.H.......[.
-00000790: f400 006b 5a05 5c38 c200 0036 3c05 5c38  ...kZ.\8...6<.\8
-000007a0: c200 0039 fe05 5c38 c200 0040 1305 5c38  ...9..\8...@..\8
-000007b0: c200 0055 ba05 5c38 c200 0067 ba05 5c38  ...U..\8...g..\8
-000007c0: c200 006e 8905 5c38 c200 007b 3405 5c38  ...n..\8...{4.\8
-000007d0: c200 00ab f505 5c38 c200 00b0 d205 5c38  ......\8......\8
-000007e0: c200 00bf e805 5c38 c200 00c7 7d05 5c38  ......\8....}.\8
-000007f0: c200 00ce ed05 5c38 c200 00d7 6605 5c38  ......\8....f.\8
-00000800: c200 00e3 e005 5c38 c200 00e9 e005 5c38  ......\8......\8
-00000810: c200 00f4 5305 5c38 c200 00f9 9905 5c38  ....S.\8......\8
-00000820: c200 00fe fa05 5c38 c200 0102 1605 5c38  ......\8......\8
-00000830: c200 0108 d205 5c38 c200 0116 bc05 5c38  ......\8......\8
-00000840: c200 011c 2a05 6b03 0500 0027 a705 7218  ....*.k....'..r.
-00000850: f300 0057 6a05 7218 f300 0068 f305 7218  ...Wj.r....h..r.
-00000860: f300 0118 cc05 73bd fe00 0036 a405 7642  ......s....6..vB
-00000870: 1900 00d8 4105 7b3a 9500 0017 eb05 901c  ....A.{:........
-00000880: 5e00 0115 9705 9982 8200 003a c505 9982  ^..........:....
-00000890: 8200 00dc bd05 a88d c400 00b5 4f05 ab35  ............O..5
-000008a0: 0200 0034 ff05 ab35 0200 0039 7b05 ab35  ...4...5...9{..5
-000008b0: 0200 0045 4205 ab35 0200 0065 1a05 ab35  ...EB..5...e...5
-000008c0: 0200 006d 6505 ab35 0200 007a 1405 ab35  ...me..5...z...5
-000008d0: 0200 00af 6d05 ab35 0200 00bf 6105 ab35  ....m..5....a..5
-000008e0: 0200 00c7 3e05 ab35 0200 00cd ca05 ab35  ....>..5.......5
-000008f0: 0200 00d6 e305 ab35 0200 00e9 5905 ab35  .......5....Y..5
-00000900: 0200 00f3 4005 ab35 0200 00f7 fa05 ab35  ....@..5.......5
-00000910: 0200 00fe b905 ab35 0200 0101 9605 ab35  .......5.......5
-00000920: 0200 0108 4f05 ab35 0200 010c 2705 ab35  ....O..5....'..5
-00000930: 0200 011b a705 ab90 4700 0040 b405 ab90  ........G..@....
-00000940: 4700 006f 9805 ab90 4700 00ac e805 ab90  G..o....G.......
-00000950: 4700 00b1 7f05 ab90 4700 00c9 2305 ab90  G.......G...#...
-00000960: 4700 010a 7305 ab90 4700 0119 6305 afca  G...s...G...c...
-00000970: 8200 0101 d505 b039 5c00 00f5 ac05 b039  .......9\......9
-00000980: 5c00 0106 ab05 ba3a 3400 00f0 d505 c0be  \......:4.......
-00000990: 1c00 0002 ac05 d0e4 4500 0007 4305 daa7  ........E...C...
-000009a0: 9300 00e1 db05 e2af 7400 00ab 4e05 f18e  ........t...N...
-000009b0: d400 008f 2205 f883 8400 0005 9b06 19f9  ...."...........
-000009c0: e500 0023 c606 2771 cb00 00cb 9506 296e  ...#..'q......)n
-000009d0: 1400 0029 ac06 2ac4 c300 00c8 ba06 38cd  ...)..*.......8.
-000009e0: d200 0051 9006 3f5e 7400 008c c506 5ded  ...Q..?^t.....].
-000009f0: 7500 002d 2806 5f70 d400 0033 0e06 6f3f  u..-(._p...3..o?
-00000a00: 4300 011a 4c06 7dda 1b00 0057 1406 7dda  C...L.}....W..}.
-00000a10: 1b00 0068 3406 7dda 1b00 007b a806 7eaf  ...h4.}....{..~.
-00000a20: 1800 0074 bd06 93cf 6400 001e 4806 9c28  ...t....d...H..(
-00000a30: 2700 00a6 3106 a0ab 2e00 0073 cd06 b695  '...1......s....
-00000a40: a700 0086 f006 bd90 c700 009c 6306 c700  ............c...
-00000a50: 2300 00b6 0606 c890 0200 0036 6b06 c890  #..........6k...
-00000a60: 0200 003a 2e06 c890 0200 003d 8406 c890  ...:.......=....
-00000a70: 0200 0055 e906 c890 0200 005e 6006 c890  ...U.......^`...
-00000a80: 0200 0067 f206 c890 0200 006e b606 c890  ...g.......n....
-00000a90: 0200 007b 6906 c890 0200 00ac 2506 c890  ...{i.......%...
-00000aa0: 0200 00b1 0106 c890 0200 00b4 c706 c890  ................
-00000ab0: 0200 00c0 1a06 c890 0200 00c8 2006 c890  ............ ...
-00000ac0: 0200 00cf 1f06 c890 0200 00d7 9606 c890  ................
-00000ad0: 0200 00ea 1206 c890 0200 00f4 8306 c890  ................
-00000ae0: 0200 00f9 c806 c890 0200 0102 4506 c890  ............E...
-00000af0: 0200 0109 0206 c890 0200 0116 ef06 c890  ................
-00000b00: 0200 011c 5a06 d1bd 3800 001d b106 d2e7  ....Z...8.......
-00000b10: 1500 00c2 6006 d487 8400 003c 5006 e0e6  ....`......<P...
-00000b20: a700 009f a207 070e 9700 00b0 6907 0877  ............i..w
-00000b30: d400 005d 3b07 0fa7 9500 000e 9607 0fee  ...];...........
-00000b40: 0500 000f 2807 17a9 2200 008e 6807 2936  ....(..."...h.)6
-00000b50: 2500 0008 6707 297f b500 0007 b107 2a79  %...g.).......*y
-00000b60: 5900 005c 6d07 34fb 9b00 0041 f607 359c  Y..\m.4....A..5.
-00000b70: 7400 0065 c307 367c d400 00fa db07 38b8  t..e..6|......8.
-00000b80: f400 0105 8607 400f 4500 0023 3307 43ab  ......@.E..#3.C.
-00000b90: b300 00e4 1607 5f75 e200 0097 5907 6218  ......_u....Y.b.
-00000ba0: 1200 0058 6807 642a 1900 00d9 8707 642a  ...Xh.d*......d*
-00000bb0: 6900 00d8 9407 642a c900 00da 7a07 642a  i.....d*....z.d*
-00000bc0: f900 00da d007 69f8 1400 005d e707 6d90  ......i....]..m.
-00000bd0: 3b00 00b6 f507 aaac 9200 00f5 e007 aab6  ;...............
-00000be0: c400 00f6 4507 aba4 0700 00ee 7307 aba4  ....E.......s...
-00000bf0: 7700 00ee 2a07 aba4 d700 00ee bc07 aba4  w...*...........
-00000c00: e700 00ef 0507 aba6 7700 00ed e107 ae08  ........w.......
-00000c10: d700 006e ed07 af4c c400 0054 8207 dc8c  ...n...L...T....
-00000c20: a400 0090 2207 ddc0 a900 00a0 1d07 e0e4  ...."...........
-00000c30: 8400 007c d907 e66b d400 0056 ae07 f0d3  ...|...k...V....
-00000c40: 0700 0040 4408 0099 e400 00a2 a708 095f  ...@D.........._
-00000c50: a400 0087 fc08 1f07 fe00 0111 0b08 2640  ..............&@
-00000c60: c500 0024 4508 26e5 b500 0096 3408 2a0f  ...$E.&.....4.*.
-00000c70: 0700 0093 0c08 2bfc 8900 00d5 b208 3367  ......+.......3g
-00000c80: 9400 0006 3908 3c2e 1400 0026 6308 466b  ....9.<....&c.Fk
-00000c90: 7900 00d8 ea08 4b41 5c00 0059 1608 5d44  y.....KA\..Y..]D
-00000ca0: a300 00b8 0308 6931 4b00 003e f508 6a58  ......i1K..>..jX
-00000cb0: 3200 0077 c908 6abd 8200 0010 5508 6ad9  2..w..j.....U.j.
-00000cc0: e400 0047 9908 6ae8 3200 0077 7408 6f31  ...G..j.2..wt.o1
-00000cd0: a400 0025 e108 7cd6 5e00 0002 5708 80d3  ...%..|.^...W...
-00000ce0: 1700 0089 8408 839b f200 00bb ba08 839c  ................
-00000cf0: 4200 00ff 2b08 87e3 2200 006b 2408 87e3  B...+..."..k$...
-00000d00: 2200 00ae 3308 87e3 2200 00cc fc08 8a6c  "...3..."......l
-00000d10: 5400 0011 7c08 8f7e e500 003d bf08 8f7e  T...|..~...=...~
-00000d20: e500 0041 4408 8f7e e500 0060 aa08 8f7e  ...AD..~...`...~
-00000d30: e500 00b5 8308 959f 0400 0049 9508 95b2  ...........I....
-00000d40: b400 007e bc08 a632 6300 00c8 5908 aa4e  ...~...2c...Y..N
-00000d50: a500 002e f408 b09c 3200 00a7 9b08 bafb  ........2.......
-00000d60: c500 00c7 0208 c0d2 1400 004f 6608 d82c  ...........Of..,
-00000d70: 3700 004b 6c08 df60 0700 00e2 3f08 e5ad  7..Kl..`....?...
-00000d80: 0400 0045 0908 e5ad 0400 0064 d808 e8f3  ...E.......d....
-00000d90: e400 00a4 4808 ec89 0700 0080 1708 f617  ....H...........
-00000da0: fb00 0113 a808 f61e 3200 0088 5c08 f9a6  ........2...\...
-00000db0: 9400 0003 d008 fe40 7400 0075 2b09 097e  .......@t..u+..~
-00000dc0: d500 0003 7109 0be8 5700 00eb 3009 2630  ....q...W...0.&0
-00000dd0: 2700 0036 d709 2630 2700 00eb cd09 33f8  '..6..&0'.....3.
-00000de0: a400 0016 9909 3f33 e400 00a5 3b09 407c  ......?3....;.@|
-00000df0: 5500 00a6 7c09 4185 8300 0050 5c09 4185  U...|.A....P\.A.
-00000e00: 8300 0112 9809 4451 9c00 00e2 ab09 66cc  ......DQ......f.
-00000e10: c900 00ac a809 6f94 a000 00a4 b809 8f2f  ......o......../
-00000e20: 0400 010c 6a09 9040 7400 00fb 8d09 9e9e  ....j..@t.......
-00000e30: 3200 004e 0b09 9e9e 3200 010d 8809 a89f  2..N....2.......
-00000e40: d700 0089 eb09 acf7 f700 00a8 fa09 af0e  ................
-00000e50: b200 003c a109 b15e f700 009b e209 b2b9  ...<...^........
-00000e60: 1700 0056 2209 b401 d700 0034 1c09 b401  ...V"......4....
-00000e70: d700 0038 6909 b401 d700 0043 c409 b401  ...8i......C....
-00000e80: d700 005b f609 b401 d700 0064 0209 b401  ...[.......d....
-00000e90: d700 0079 3909 b401 d700 00be e709 b401  ...y9...........
-00000ea0: d700 00d4 4509 b401 d700 00e7 fe09 b401  ....E...........
-00000eb0: d700 00f1 4009 b401 d700 00f7 8309 bab0  ....@...........
-00000ec0: 0e00 00e5 f509 c958 2400 00d0 5909 dbed  .......X$...Y...
-00000ed0: 3d00 00d7 fb09 f9d7 2400 0066 300a 0069  =.......$..f0..i
-00000ee0: e400 0012 b70a 052c 4500 00ef cd0a 06f3  .......,E.......
-00000ef0: 5700 003f 620a 0ccf 3500 0018 f00a 13ef  W..?b...5.......
-00000f00: d400 0099 400a 18ea 3400 0095 240a 1f3d  ....@...4...$..=
-00000f10: 5700 0051 0a0a 209c 6200 00ba b90a 209c  W..Q.. .b..... .
-00000f20: 8200 00ba 050a 209c 9200 00ba 5f0a 209c  ...... ....._. .
-00000f30: a200 00b9 510a 209c b200 00b9 ab0a 209c  ....Q. ....... .
-00000f40: d200 00b8 f70a 2217 1500 000b 620a 27e7  ......".....b.'.
-00000f50: 3400 0042 ed0a 29ec d700 004a c50a 2ab2  4..B..)....J..*.
-00000f60: 5300 0037 b80a 2ab2 5300 00d1 7b0a 2ab2  S..7..*.S...{.*.
-00000f70: 5300 00ef 4e0a 2b4f 3400 00e0 f40a 30e8  S...N.+O4.....0.
-00000f80: 8200 00cd 720a 4659 9e00 006f d50a 4971  ....r.FY...o..Iq
-00000f90: 3e00 003a 680a 53e6 b500 00e6 360a 53e6  >..:h.S.....6.S.
-00000fa0: b500 00ef 8b0a 5a8c 7300 0114 860a 5aff  ......Z.s.....Z.
-00000fb0: 5500 002f a80a 5e17 d700 0051 fb0a 5e17  U../..^....Q..^.
-00000fc0: d700 0114 090a 6438 0400 0072 e80a 6438  ......d8...r..d8
-00000fd0: 0400 00be 380a 6438 0400 00fd 940a 6438  ....8.d8......d8
-00000fe0: 0400 0105 d70a 643c 1400 0037 f50a 643c  ......d<...7..d<
-00000ff0: 1400 003b da0a 643c 1400 003d fa0a 643c  ...;..d<...=..d<
-00001000: 1400 0073 1d0a 643c 1400 0078 1e0a 643c  ...s..d<...x..d<
-00001010: 1400 00ae 6b0a 643c 1400 00b4 140a 643c  ....k.d<......d<
-00001020: 1400 00be 6f0a 643c 1400 00c0 c40a 643c  ....o.d<......d<
-00001030: 1400 00c6 470a 643c 1400 00d2 3f0a 643c  ....G.d<....?.d<
-00001040: 1400 00e0 b30a 643c 1400 00e4 eb0a 643c  ......d<......d<
-00001050: 1400 00e6 7a0a 643c 1400 00f0 1b0a 643c  ....z.d<......d<
-00001060: 1400 00f6 c80a 643c 1400 00fd ca0a 643c  ......d<......d<
-00001070: 1400 00ff ec0a 643c 1400 0107 460a 643c  ......d<....F.d<
-00001080: 1400 010b ad0a 643c 1400 011a dd0a 647f  ......d<......d.
-00001090: 3400 0042 3a0a 679b 2400 0103 b20a 68c1  4..B:.g.$.....h.
-000010a0: d200 00e7 040a 6b9f 2c00 00bc 0c0a 6b9f  ......k.,.....k.
-000010b0: 2c00 0106 750a 7165 9200 0089 2d0a 7328  ,...u.qe....-.s(
-000010c0: 0e00 00df 420a 7c04 8700 0043 330a 92e0  ....B.|....C3...
-000010d0: 9200 0076 3e0a 95f8 2400 0091 d50a 9cb5  ...v>...$.......
-000010e0: 6400 00d2 f90a a1fa 5200 005b 710a a9ec  d.......R..[q...
-000010f0: 2500 0013 ea0a b0d6 4200 0085 520a bc8c  %.......B...R...
-00001100: 7400 0033 e40a bc8c 7400 0038 300a bc8c  t..3....t..80...
-00001110: 7400 003c 160a bc8c 7400 003e 360a bc8c  t..<....t..>6...
-00001120: 7400 0043 8c0a bc8c 7400 005b be0a bc8c  t..C....t..[....
-00001130: 7400 0063 c10a bc8c 7400 006c c50a bc8c  t..c....t..l....
-00001140: 7400 0073 580a bc8c 7400 0076 020a bc8c  t..sX...t..v....
-00001150: 7400 0078 a70a bc8c 7400 00a9 ec0a bc8c  t..x....t.......
-00001160: 7400 00af 350a bc8c 7400 00b4 530a bc8c  t...5...t...S...
-00001170: 7400 00b7 370a bc8c 7400 00be ac0a bc8c  t...7...t.......
-00001180: 7400 00c0 fd0a bc8c 7400 00c6 ca0a bc8c  t.......t.......
-00001190: 7400 00cd 370a bc8c 7400 00d2 c00a bc8c  t...7...t.......
-000011a0: 7400 00e1 9c0a bc8c 7400 00e5 2c0a bc8c  t.......t...,...
-000011b0: 7400 00e7 430a bc8c 7400 00f0 9c0a bc8c  t...C...t.......
-000011c0: 7400 00f7 4b0a bc8c 7400 00fe 060a bc8c  t...K...t.......
-000011d0: 7400 0100 fd0a bc8c 7400 0106 0b0a bc8c  t.......t.......
-000011e0: 7400 0108 160a bc8c 7400 010b eb0a bc8c  t.......t.......
-000011f0: 7400 011b 180a c6ed e400 0116 0d0a d17a  t..............z
-00001200: e400 008b 750a e85a 5400 0095 6b0a f313  ....u..ZT...k...
-00001210: a500 001c 950a f35a 3500 001d 230b 02f8  .......Z5...#...
-00001220: 0700 00c4 1a0b 0d5f b400 0098 f00b 0e3f  ......._.......?
-00001230: 0400 0094 6e0b 1aa2 b400 00c5 5c0b 228f  ....n.......\.".
-00001240: 8500 0031 5c0b 2418 e700 00e7 7e0b 2495  ...1\.$.....~.$.
-00001250: 7400 00cb 2e0b 27ac 6400 002c b70b 28a0  t.....'.d..,..(.
-00001260: 8400 00a3 380b 3888 3500 0026 e70b 3b32  ....8.8.5..&..;2
-00001270: c800 001f ee0b 3b5e b700 0085 ad0b 41be  ......;^......A.
-00001280: 5c00 001e 8a0b 45d7 c400 00a2 290b 5fa0  \.....E.....)._.
-00001290: d400 0021 0e0b 6356 e500 0071 da0b 6419  ...!..cV...q..d.
-000012a0: f300 00b1 be0b 644e a400 00f2 900b 6514  ......dN......e.
-000012b0: 8400 00a7 f60b 70d3 4300 0064 820b 765d  ......p.C..d..v]
-000012c0: 7700 0042 7a0b 765d 7700 0062 a10b 768f  w..Bz.v]w..b..v.
-000012d0: b800 0071 6c0b 7d54 f400 0046 6e0b 8034  ...ql.}T...Fn..4
-000012e0: 2400 00a1 420b 81f4 c900 00dc 1b0b 8525  $...B..........%
-000012f0: a400 004e 670b 8fd4 1500 005a 4d0b 8fd4  ...Ng......ZM...
-00001300: 1500 008a cd0b 8fd4 1500 0107 0b0b a3dc  ................
-00001310: 0c00 011e fc0b a3fc 0c00 002e ae0b aca2  ................
-00001320: 3b00 0119 a60b bf79 0200 0020 530b c77c  ;......y... S..|
-00001330: 1200 0053 540b c77c 1200 0066 fa0b c77c  ...ST..|...f...|
-00001340: 1200 00f8 930b ca42 7500 00de fa0b cf7a  .......Bu......z
-00001350: 4400 0015 6a0b d395 e500 00c7 ac0b db27  D...j..........'
-00001360: 2800 0072 2a0b dcb6 f400 0024 f20b dd4f  (..r*......$...O
-00001370: 0500 00e8 780b dd4f 0500 00f1 eb0b ecc6  ....x..O........
-00001380: 3400 003a f90b ecc6 3400 00dc f10b f17f  4..:....4.......
-00001390: 2900 00de 700c 02d8 9700 0094 bd0c 09f0  )...p...........
-000013a0: 4500 0098 990c 0d29 8b00 00e6 b70c 0d29  E......).......)
-000013b0: 8b00 0100 260c 0d29 8b00 0107 810c 0fd6  ....&..)........
-000013c0: 7400 0076 e40c 1a46 4200 0109 8f0c 1c0d  t..v...FB.......
-000013d0: 5800 0100 700c 2301 d700 00ea 4e0c 3ed6  X...p.#.....N.>.
-000013e0: 0200 009b 930c 4aac 8e00 0034 c60c 4aac  ......J....4..J.
-000013f0: 8e00 003e ba0c 4aac 8e00 00fe 7e0c 4b86  ...>..J.....~.K.
-00001400: 4200 0075 980c 574c 8500 00e1 410c 57f6  B..u..WL....A.W.
-00001410: dc00 0080 b00c 66ce f200 005d a50c 6adf  ......f....]..j.
-00001420: e300 00b7 740c 6f05 c200 0039 140c 6f05  ....t.o....9..o.
-00001430: c200 00d6 7c0c 6f05 c200 00f2 d90c a71d  ....|.o.........
-00001440: 2700 008b 390c af2c 1400 006c 670c c10f  '...9..,...lg...
-00001450: c500 00e5 6b0c c81b 6b00 004f e90c c8fc  ....k...k..O....
-00001460: 2500 00c5 ba0c c8fc 2500 011c 940c d041  %.......%......A
-00001470: 8e00 007a 590c d0e6 b700 008e a70c dd01  ...zY...........
-00001480: 4700 0045 de0c e721 0400 010f 760c f104  G..E...!....v...
-00001490: 1400 0054 1e0c f4cf 7200 011c cf0c f7ef  ...T....r.......
-000014a0: c400 0087 9a0c fb27 d700 0095 b00c fbf3  .......'........
-000014b0: 7500 000a 9a0c fe78 8e00 007f 920d 120d  u......x........
-000014c0: 2e00 00d2 7a0d 120d 2e00 00f0 560d 13a6  ....z.......V...
-000014d0: 4500 00a5 d60d 27b8 3400 002c 4c0d 3193  E.....'.4..,L.1.
-000014e0: 3500 00b5 c10d 3934 3300 00ae a50d 4026  5.....943.....@&
-000014f0: 3400 009e 470d 402a 2400 009e 030d 5fe1  4...G.@*$....._.
-00001500: 1300 00ad e50d 63a5 6200 0078 e50d 747d  ......c.b..x..t}
-00001510: 3400 0035 800d 747d 3400 006d e20d 747d  4..5..t}4..m..t}
-00001520: 3400 00ab a90d 747d 3400 00b0 1e0d 747d  4.....t}4.....t}
-00001530: 3400 00ce 9f0d 747d 3400 0116 6d0d 7774  4.....t}4...m.wt
-00001540: bc00 0052 740d 8289 d400 0053 c00d 845c  ...Rt......S...\
-00001550: 5200 00d5 f50d 8504 e300 005c d70d 8797  R..........\....
-00001560: b400 010e f90d 8c3f 4400 0081 9d0d 94b9  .......?D.......
-00001570: a200 004f 100d 94b9 a200 0110 300d 9d49  ...O........0..I
-00001580: 6700 0058 b80d 9d49 6700 006a 030d 9d49  g..X...Ig..j...I
-00001590: 6700 0070 1d0d 9d49 6700 007c 750d 9d49  g..p...Ig..|u..I
-000015a0: 6700 00ad 280d 9d49 6700 00b2 6a0d 9d49  g...(..Ig...j..I
-000015b0: 6700 00c9 d70d 9d49 6700 00cf c90d 9d49  g......Ig......I
-000015c0: 6700 00ed 800d 9d49 6700 010a b30d 9d49  g......Ig......I
-000015d0: 6700 0119 ea0d a105 8400 0045 810d abe3  g..........E....
-000015e0: 7400 0052 fa0d abe3 7400 0066 970d abe3  t..R....t..f....
-000015f0: 7400 00f8 390d ba75 7400 0102 7e0d c260  t...9..ut...~..`
-00001600: e500 0098 530d d72e 8400 00a3 bd0d dc7d  ....S..........}
-00001610: 6e00 0117 920d dd16 1400 0035 cb0d e487  n..........5....
-00001620: ce00 004a 300d e59c 1200 00c2 dc0d f179  ...J0..........y
-00001630: 1200 0084 3c0e 02d3 5700 00a8 9f0e 0642  ....<...W......B
-00001640: 8200 0048 100e 0d63 f200 0009 da0e 0f0b  ...H...c........
-00001650: e900 005f bc0e 27bb d200 0012 1b0e 390c  ..._..'.......9.
-00001660: 8500 0083 aa0e 3da4 6500 009a 1b0e 4732  ......=.e.....G2
-00001670: 1200 0076 900e 4818 4900 00aa ef0e 4fa8  ...v..H.I.....O.
-00001680: 0900 00d4 bd0e 5689 c700 009d 0d0e 57b4  ......V.......W.
-00001690: 5c00 0093 990e 5d8b 6700 0086 3a0e 6596  \.....].g...:.e.
-000016a0: 5400 008d 990e 6877 8400 0091 710e 69e5  T.....hw....q.i.
-000016b0: 7200 009f 600e 6c1e 6400 007e 4c0e 77e6  r...`.l.d..~L.w.
-000016c0: 6700 009e d90e 7b0f d400 0082 b70e 87f3  g.....{.........
-000016d0: 2d00 00bd bf0e 90da 4300 00df 850e 91f3  -.......C.......
-000016e0: e200 00fa 010e 9b26 3400 008d 4f0e a14e  .......&4...O..N
-000016f0: a500 0019 ce0e a308 c700 003b 6e0e a308  ...........;n...
-00001700: c700 0057 fd0e a308 c700 005f 270e a308  ...W......._'...
-00001710: c700 0069 8f0e a308 c700 007c 040e a308  ...i.......|....
-00001720: c700 00c0 560e a308 c700 00cf 5b0e a308  ....V.......[...
-00001730: c700 00dd 660e a308 c700 00ea c20e a308  ....f...........
-00001740: c700 00f5 400e a308 c700 00fb dd0e a3f5  ....@...........
-00001750: 4200 007f 350e a55f 0700 006a 6a0e a5bf  B...5.._...jj...
-00001760: b400 0082 5b0e ad29 7700 00ec f50e b40e  ....[..)w.......
-00001770: ce00 010d e80e b8a4 3400 0101 350e c6a6  ........4...5...
-00001780: 1400 00fb 300e c76e 0400 0013 480e c8d9  ....0..n....H...
-00001790: a400 0062 150e d04c 8400 0010 ee0e d36b  ...b...L.......k
-000017a0: 4300 00c9 620e e07c a500 0004 e80e eb6a  C...b..|.......j
-000017b0: 8500 0074 710e ec73 3400 010b 600e f60a  ...tq..s4...`...
-000017c0: 3500 0028 740e f6b2 e500 00b8 a00e fe32  5..(t..........2
-000017d0: 0e00 0055 000e fe32 0e00 0092 930f 1840  ...U...2.......@
-000017e0: 9200 0085 010f 2205 7700 00e0 580f 237d  ......".w...X.#}
-000017f0: 7700 0060 e30f 2781 5b00 00cc 7c0f 32a1  w..`..'.[...|.2.
-00001800: 8500 005e 1f0f 342b 3400 002b e70f 38db  ...^..4+4..+..8.
-00001810: 3400 0032 620f 393c 3300 00bd 230f 466b  4..2b.9<3...#.Fk
-00001820: 7900 00d9 dd0f 52ce 9200 009b 4e0f 6d25  y.....R.....N.m%
-00001830: 7700 0102 df0f 7540 d400 0037 6b0f 7540  w.....u@...7k.u@
-00001840: d400 0040 f50f 7540 d400 010b 120f 84d5  ...@..u@........
-00001850: 2400 006c 0a0f 8932 1400 0097 010f 9029  $..l...2.......)
-00001860: 7400 0004 290f b56e 4500 002e 410f c096  t...)..nE...A...
-00001870: 5400 009e 910f c494 9400 0077 2a0f c4d4  T..........w*...
-00001880: 1400 0021 d90f cdc1 2300 00b6 700f dce5  ...!....#...p...
-00001890: 2500 0025 5f0f e1b2 c400 00e4 a70f e539  %..%_..........9
-000018a0: 7200 00ac 5f0f f9ac 9500 0072 9c69 0001  r..._......r.i..
-000018b0: 1f44 0300 0000 1200 4100 6200 6200 7200  .D......A.b.b.r.
-000018c0: 6500 6300 6800 6500 6e08 0000 0000 0600  e.c.h.e.n.......
-000018d0: 0000 0643 616e 6365 6c07 0000 000b 5173  ...Cancel.....Qs
-000018e0: 6369 436f 6d6d 616e 6401 0300 0000 4800  ciCommand.....H.
-000018f0: 4100 7500 7300 7700 6100 6800 6c00 2000  A.u.s.w.a.h.l. .
-00001900: 6900 6e00 2000 4b00 6c00 6500 6900 6e00  i.n. .K.l.e.i.n.
-00001910: 6200 7500 6300 6800 7300 7400 6100 6200  b.u.c.h.s.t.a.b.
-00001920: 6500 6e00 2000 7500 6d00 7700 6100 6e00  e.n. .u.m.w.a.n.
-00001930: 6400 6500 6c00 6e08 0000 0000 0600 0000  d.e.l.n.........
-00001940: 1f43 6f6e 7665 7274 2073 656c 6563 7469  .Convert selecti
-00001950: 6f6e 2074 6f20 6c6f 7765 7220 6361 7365  on to lower case
-00001960: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
-00001970: 0103 0000 0046 0041 0075 0073 0077 0061  .....F.A.u.s.w.a
-00001980: 0068 006c 0020 0069 006e 0020 0047 0072  .h.l. .i.n. .G.r
-00001990: 006f 00df 0062 0075 0063 0068 0073 0074  .o...b.u.c.h.s.t
-000019a0: 0061 0062 0065 006e 0020 0075 006d 0077  .a.b.e.n. .u.m.w
-000019b0: 0061 006e 0064 0065 006c 006e 0800 0000  .a.n.d.e.l.n....
-000019c0: 0006 0000 001f 436f 6e76 6572 7420 7365  ......Convert se
-000019d0: 6c65 6374 696f 6e20 746f 2075 7070 6572  lection to upper
-000019e0: 2063 6173 6507 0000 000b 5173 6369 436f   case.....QsciCo
-000019f0: 6d6d 616e 6401 0300 0000 2e00 4100 6b00  mmand.......A.k.
-00001a00: 7400 7500 6500 6c00 6c00 6500 2000 5a00  t.u.e.l.l.e. .Z.
-00001a10: 6500 6900 6c00 6500 2000 6b00 6f00 7000  e.i.l.e. .k.o.p.
-00001a20: 6900 6500 7200 6500 6e08 0000 0000 0600  i.e.r.e.n.......
-00001a30: 0000 1143 6f70 7920 6375 7272 656e 7420  ...Copy current 
-00001a40: 6c69 6e65 0700 0000 0b51 7363 6943 6f6d  line.....QsciCom
-00001a50: 6d61 6e64 0103 0000 0020 0041 0075 0073  mand..... .A.u.s
-00001a60: 0077 0061 0068 006c 0020 006b 006f 0070  .w.a.h.l. .k.o.p
-00001a70: 0069 0065 0072 0065 006e 0800 0000 0006  .i.e.r.e.n......
-00001a80: 0000 000e 436f 7079 2073 656c 6563 7469  ....Copy selecti
-00001a90: 6f6e 0700 0000 0b51 7363 6943 6f6d 6d61  on.....QsciComma
-00001aa0: 6e64 0103 0000 0036 0041 006b 0074 0075  nd.....6.A.k.t.u
-00001ab0: 0065 006c 006c 0065 0020 005a 0065 0069  .e.l.l.e. .Z.e.i
-00001ac0: 006c 0065 0020 0061 0075 0073 0073 0063  .l.e. .a.u.s.s.c
-00001ad0: 0068 006e 0065 0069 0064 0065 006e 0800  .h.n.e.i.d.e.n..
-00001ae0: 0000 0006 0000 0010 4375 7420 6375 7272  ........Cut curr
-00001af0: 656e 7420 6c69 6e65 0700 0000 0b51 7363  ent line.....Qsc
-00001b00: 6943 6f6d 6d61 6e64 0103 0000 0028 0041  iCommand.....(.A
-00001b10: 0075 0073 0077 0061 0068 006c 0020 0061  .u.s.w.a.h.l. .a
-00001b20: 0075 0073 0073 0063 0068 006e 0065 0069  .u.s.s.c.h.n.e.i
-00001b30: 0064 0065 006e 0800 0000 0006 0000 000d  .d.e.n..........
-00001b40: 4375 7420 7365 6c65 6374 696f 6e07 0000  Cut selection...
-00001b50: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00001b60: 0000 2800 4500 6900 6e00 6500 2000 4500  ..(.E.i.n.e. .E.
-00001b70: 6200 6500 6e00 6500 2000 6100 7500 7300  b.e.n.e. .a.u.s.
-00001b80: 7200 fc00 6300 6b00 6500 6e08 0000 0000  r...c.k.e.n.....
-00001b90: 0600 0000 1344 652d 696e 6465 6e74 206f  .....De-indent o
-00001ba0: 6e65 206c 6576 656c 0700 0000 0b51 7363  ne level.....Qsc
-00001bb0: 6943 6f6d 6d61 6e64 0103 0000 0032 0041  iCommand.....2.A
-00001bc0: 006b 0074 0075 0065 006c 006c 0065 0073  .k.t.u.e.l.l.e.s
-00001bd0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-00001be0: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
-00001bf0: 0800 0000 0006 0000 0018 4465 6c65 7465  ..........Delete
-00001c00: 2063 7572 7265 6e74 2063 6861 7261 6374   current charact
-00001c10: 6572 0700 0000 0b51 7363 6943 6f6d 6d61  er.....QsciComma
-00001c20: 6e64 0103 0000 002c 0041 006b 0074 0075  nd.....,.A.k.t.u
-00001c30: 0065 006c 006c 0065 0020 005a 0065 0069  .e.l.l.e. .Z.e.i
-00001c40: 006c 0065 0020 006c 00f6 0073 0063 0068  .l.e. .l...s.c.h
-00001c50: 0065 006e 0800 0000 0006 0000 0013 4465  .e.n..........De
-00001c60: 6c65 7465 2063 7572 7265 6e74 206c 696e  lete current lin
-00001c70: 6507 0000 000b 5173 6369 436f 6d6d 616e  e.....QsciComman
-00001c80: 6401 0300 0000 2600 5a00 6500 6900 6c00  d.....&.Z.e.i.l.
-00001c90: 6500 2000 6c00 6900 6e00 6b00 7300 2000  e. .l.i.n.k.s. .
-00001ca0: 6c00 f600 7300 6300 6800 6500 6e08 0000  l...s.c.h.e.n...
-00001cb0: 0000 0600 0000 1344 656c 6574 6520 6c69  .......Delete li
-00001cc0: 6e65 2074 6f20 6c65 6674 0700 0000 0b51  ne to left.....Q
-00001cd0: 7363 6943 6f6d 6d61 6e64 0103 0000 0028  sciCommand.....(
-00001ce0: 005a 0065 0069 006c 0065 0020 0072 0065  .Z.e.i.l.e. .r.e
-00001cf0: 0063 0068 0074 0073 0020 006c 00f6 0073  .c.h.t.s. .l...s
-00001d00: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-00001d10: 0014 4465 6c65 7465 206c 696e 6520 746f  ..Delete line to
-00001d20: 2072 6967 6874 0700 0000 0b51 7363 6943   right.....QsciC
-00001d30: 6f6d 6d61 6e64 0103 0000 002a 005a 0065  ommand.....*.Z.e
-00001d40: 0069 0063 0068 0065 006e 0020 006c 0069  .i.c.h.e.n. .l.i
-00001d50: 006e 006b 0073 0020 006c 00f6 0073 0063  .n.k.s. .l...s.c
-00001d60: 0068 0065 006e 0800 0000 0006 0000 0019  .h.e.n..........
-00001d70: 4465 6c65 7465 2070 7265 7669 6f75 7320  Delete previous 
-00001d80: 6368 6172 6163 7465 7207 0000 000b 5173  character.....Qs
-00001d90: 6369 436f 6d6d 616e 6401 0300 0000 6200  ciCommand.....b.
-00001da0: 5a00 6500 6900 6300 6800 6500 6e00 2000  Z.e.i.c.h.e.n. .
-00001db0: 6c00 6900 6e00 6b00 7300 2000 6c00 f600  l.i.n.k.s. .l...
-00001dc0: 7300 6300 6800 6500 6e00 2c00 2000 7700  s.c.h.e.n.,. .w.
-00001dd0: 6500 6e00 6e00 2000 6e00 6900 6300 6800  e.n.n. .n.i.c.h.
-00001de0: 7400 2000 6100 6d00 2000 5a00 6500 6900  t. .a.m. .Z.e.i.
-00001df0: 6c00 6500 6e00 6100 6e00 6600 6100 6e00  l.e.n.a.n.f.a.n.
-00001e00: 6708 0000 0000 0600 0000 3144 656c 6574  g.........1Delet
-00001e10: 6520 7072 6576 696f 7573 2063 6861 7261  e previous chara
-00001e20: 6374 6572 2069 6620 6e6f 7420 6174 2073  cter if not at s
-00001e30: 7461 7274 206f 6620 6c69 6e65 0700 0000  tart of line....
-00001e40: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
-00001e50: 005e 0052 0065 0063 0068 0074 0073 0020  .^.R.e.c.h.t.s. 
-00001e60: 0062 0069 0073 0020 007a 0075 006d 0020  .b.i.s. .z.u.m. 
-00001e70: 0045 006e 0064 0065 0020 0064 0065 0073  .E.n.d.e. .d.e.s
-00001e80: 0020 006e 00e4 0063 0068 0073 0074 0065  . .n...c.h.s.t.e
-00001e90: 006e 0020 0057 006f 0072 0074 0065 0073  .n. .W.o.r.t.e.s
-00001ea0: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
-00001eb0: 0800 0000 0006 0000 0020 4465 6c65 7465  ......... Delete
-00001ec0: 2072 6967 6874 2074 6f20 656e 6420 6f66   right to end of
-00001ed0: 206e 6578 7420 776f 7264 0700 0000 0b51   next word.....Q
-00001ee0: 7363 6943 6f6d 6d61 6e64 0103 0000 0024  sciCommand.....$
-00001ef0: 0057 006f 0072 0074 0020 006c 0069 006e  .W.o.r.t. .l.i.n
-00001f00: 006b 0073 0020 006c 00f6 0073 0063 0068  .k.s. .l...s.c.h
-00001f10: 0065 006e 0800 0000 0006 0000 0013 4465  .e.n..........De
-00001f20: 6c65 7465 2077 6f72 6420 746f 206c 6566  lete word to lef
-00001f30: 7407 0000 000b 5173 6369 436f 6d6d 616e  t.....QsciComman
-00001f40: 6401 0300 0000 2600 5700 6f00 7200 7400  d.....&.W.o.r.t.
-00001f50: 2000 7200 6500 6300 6800 7400 7300 2000   .r.e.c.h.t.s. .
-00001f60: 6c00 f600 7300 6300 6800 6500 6e08 0000  l...s.c.h.e.n...
-00001f70: 0000 0600 0000 1444 656c 6574 6520 776f  .......Delete wo
-00001f80: 7264 2074 6f20 7269 6768 7407 0000 000b  rd to right.....
-00001f90: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00001fa0: 2600 4100 7500 7300 7700 6100 6800 6c00  &.A.u.s.w.a.h.l.
-00001fb0: 2000 6400 7500 7000 6c00 6900 7a00 6900   .d.u.p.l.i.z.i.
-00001fc0: 6500 7200 6500 6e08 0000 0000 0600 0000  e.r.e.n.........
-00001fd0: 1344 7570 6c69 6361 7465 2073 656c 6563  .Duplicate selec
-00001fe0: 7469 6f6e 0700 0000 0b51 7363 6943 6f6d  tion.....QsciCom
-00001ff0: 6d61 6e64 0103 0000 0034 0041 006b 0074  mand.....4.A.k.t
-00002000: 0075 0065 006c 006c 0065 0020 005a 0065  .u.e.l.l.e. .Z.e
-00002010: 0069 006c 0065 0020 0064 0075 0070 006c  .i.l.e. .d.u.p.l
-00002020: 0069 007a 0069 0065 0072 0065 006e 0800  .i.z.i.e.r.e.n..
-00002030: 0000 0006 0000 001a 4475 706c 6963 6174  ........Duplicat
-00002040: 6520 7468 6520 6375 7272 656e 7420 6c69  e the current li
-00002050: 6e65 0700 0000 0b51 7363 6943 6f6d 6d61  ne.....QsciComma
-00002060: 6e64 0103 0000 006c 0052 0065 0063 0068  nd.....l.R.e.c.h
-00002070: 0074 0065 0063 006b 0069 0067 0065 0020  .t.e.c.k.i.g.e. 
-00002080: 0041 0075 0073 0077 0061 0068 006c 0020  .A.u.s.w.a.h.l. 
-00002090: 0075 006d 0020 0065 0069 006e 0065 0020  .u.m. .e.i.n.e. 
-000020a0: 005a 0065 0069 006c 0065 0020 006e 0061  .Z.e.i.l.e. .n.a
-000020b0: 0063 0068 0020 0075 006e 0074 0065 006e  .c.h. .u.n.t.e.n
-000020c0: 0020 0065 0072 0077 0065 0069 0074 0065  . .e.r.w.e.i.t.e
-000020d0: 0072 006e 0800 0000 0006 0000 002a 4578  .r.n.........*Ex
-000020e0: 7465 6e64 2072 6563 7461 6e67 756c 6172  tend rectangular
-000020f0: 2073 656c 6563 7469 6f6e 2064 6f77 6e20   selection down 
-00002100: 6f6e 6520 6c69 6e65 0700 0000 0b51 7363  one line.....Qsc
-00002110: 6943 6f6d 6d61 6e64 0103 0000 006c 0052  iCommand.....l.R
-00002120: 0065 0063 0068 0074 0065 0063 006b 0069  .e.c.h.t.e.c.k.i
-00002130: 0067 0065 0020 0041 0075 0073 0077 0061  .g.e. .A.u.s.w.a
-00002140: 0068 006c 0020 0075 006d 0020 0065 0069  .h.l. .u.m. .e.i
-00002150: 006e 0065 0020 0053 0065 0069 0074 0065  .n.e. .S.e.i.t.e
-00002160: 0020 006e 0061 0063 0068 0020 0075 006e  . .n.a.c.h. .u.n
-00002170: 0074 0065 006e 0020 0065 0072 0077 0065  .t.e.n. .e.r.w.e
-00002180: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
-00002190: 0000 002a 4578 7465 6e64 2072 6563 7461  ...*Extend recta
-000021a0: 6e67 756c 6172 2073 656c 6563 7469 6f6e  ngular selection
-000021b0: 2064 6f77 6e20 6f6e 6520 7061 6765 0700   down one page..
-000021c0: 0000 0b51 7363 6943 6f6d 6d61 6e64 0103  ...QsciCommand..
-000021d0: 0000 006e 0052 0065 0063 0068 0074 0065  ...n.R.e.c.h.t.e
-000021e0: 0063 006b 0069 0067 0065 0020 0041 0075  .c.k.i.g.e. .A.u
-000021f0: 0073 0077 0061 0068 006c 0020 0075 006d  .s.w.a.h.l. .u.m
-00002200: 0020 0065 0069 006e 0020 005a 0065 0069  . .e.i.n. .Z.e.i
-00002210: 0063 0068 0065 006e 0020 006e 0061 0063  .c.h.e.n. .n.a.c
-00002220: 0068 0020 006c 0069 006e 006b 0073 0020  .h. .l.i.n.k.s. 
-00002230: 0065 0072 0077 0065 0069 0074 0065 0072  .e.r.w.e.i.t.e.r
-00002240: 006e 0800 0000 0006 0000 002f 4578 7465  .n........./Exte
-00002250: 6e64 2072 6563 7461 6e67 756c 6172 2073  nd rectangular s
-00002260: 656c 6563 7469 6f6e 206c 6566 7420 6f6e  election left on
-00002270: 6520 6368 6172 6163 7465 7207 0000 000b  e character.....
-00002280: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00002290: 7000 5200 6500 6300 6800 7400 6500 6300  p.R.e.c.h.t.e.c.
-000022a0: 6b00 6900 6700 6500 2000 4100 7500 7300  k.i.g.e. .A.u.s.
-000022b0: 7700 6100 6800 6c00 2000 7500 6d00 2000  w.a.h.l. .u.m. .
-000022c0: 6500 6900 6e00 2000 5a00 6500 6900 6300  e.i.n. .Z.e.i.c.
-000022d0: 6800 6500 6e00 2000 6e00 6100 6300 6800  h.e.n. .n.a.c.h.
-000022e0: 2000 7200 6500 6300 6800 7400 7300 2000   .r.e.c.h.t.s. .
-000022f0: 6500 7200 7700 6500 6900 7400 6500 7200  e.r.w.e.i.t.e.r.
-00002300: 6e08 0000 0000 0600 0000 3045 7874 656e  n.........0Exten
-00002310: 6420 7265 6374 616e 6775 6c61 7220 7365  d rectangular se
-00002320: 6c65 6374 696f 6e20 7269 6768 7420 6f6e  lection right on
-00002330: 6520 6368 6172 6163 7465 7207 0000 000b  e character.....
-00002340: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00002350: 7400 5200 6500 6300 6800 7400 6500 6300  t.R.e.c.h.t.e.c.
-00002360: 6b00 6900 6700 6500 2000 4100 7500 7300  k.i.g.e. .A.u.s.
-00002370: 7700 6100 6800 6c00 2000 7a00 7500 6d00  w.a.h.l. .z.u.m.
-00002380: 2000 4500 6e00 6400 6500 2000 6400 6500   .E.n.d.e. .d.e.
-00002390: 7200 2000 4400 6f00 6b00 7500 6d00 6500  r. .D.o.k.u.m.e.
-000023a0: 6e00 7400 6500 6e00 7a00 6500 6900 6c00  n.t.e.n.z.e.i.l.
-000023b0: 6500 2000 6500 7200 7700 6500 6900 7400  e. .e.r.w.e.i.t.
-000023c0: 6500 7200 6e08 0000 0000 0600 0000 3445  e.r.n.........4E
-000023d0: 7874 656e 6420 7265 6374 616e 6775 6c61  xtend rectangula
-000023e0: 7220 7365 6c65 6374 696f 6e20 746f 2065  r selection to e
-000023f0: 6e64 206f 6620 646f 6375 6d65 6e74 206c  nd of document l
-00002400: 696e 6507 0000 000b 5173 6369 436f 6d6d  ine.....QsciComm
-00002410: 616e 6401 0300 0000 9a00 5200 6500 6300  and.......R.e.c.
-00002420: 6800 7400 6500 6300 6b00 6900 6700 6500  h.t.e.c.k.i.g.e.
-00002430: 2000 4100 7500 7300 7700 6100 6800 6c00   .A.u.s.w.a.h.l.
-00002440: 2000 7a00 7500 6d00 2000 6500 7200 7300   .z.u.m. .e.r.s.
-00002450: 7400 6500 6e00 2000 7300 6900 6300 6800  t.e.n. .s.i.c.h.
-00002460: 7400 6200 6100 7200 6500 6e00 2000 5a00  t.b.a.r.e.n. .Z.
-00002470: 6500 6900 6300 6800 6500 6e00 2000 6400  e.i.c.h.e.n. .d.
-00002480: 6500 7200 2000 4400 6f00 6b00 7500 6d00  e.r. .D.o.k.u.m.
-00002490: 6500 6e00 7400 7a00 6500 6900 6c00 6500  e.n.t.z.e.i.l.e.
-000024a0: 2000 6500 7200 7700 6500 6900 7400 6500   .e.r.w.e.i.t.e.
-000024b0: 7200 6e08 0000 0000 0600 0000 4845 7874  r.n.........HExt
-000024c0: 656e 6420 7265 6374 616e 6775 6c61 7220  end rectangular 
-000024d0: 7365 6c65 6374 696f 6e20 746f 2066 6972  selection to fir
-000024e0: 7374 2076 6973 6962 6c65 2063 6861 7261  st visible chara
-000024f0: 6374 6572 2069 6e20 646f 6375 6d65 6e74  cter in document
-00002500: 206c 696e 6507 0000 000b 5173 6369 436f   line.....QsciCo
-00002510: 6d6d 616e 6401 0300 0000 7800 5200 6500  mmand.....x.R.e.
-00002520: 6300 6800 7400 6500 6300 6b00 6900 6700  c.h.t.e.c.k.i.g.
-00002530: 6500 2000 4100 7500 7300 7700 6100 6800  e. .A.u.s.w.a.h.
-00002540: 6c00 2000 7a00 7500 6d00 2000 4200 6500  l. .z.u.m. .B.e.
-00002550: 6700 6900 6e00 6e00 2000 6400 6500 7200  g.i.n.n. .d.e.r.
-00002560: 2000 4400 6f00 6b00 7500 6d00 6500 6e00   .D.o.k.u.m.e.n.
-00002570: 7400 6500 6e00 7a00 6500 6900 6c00 6500  t.e.n.z.e.i.l.e.
-00002580: 2000 6500 7200 7700 6500 6900 7400 6500   .e.r.w.e.i.t.e.
-00002590: 7200 6e08 0000 0000 0600 0000 3645 7874  r.n.........6Ext
-000025a0: 656e 6420 7265 6374 616e 6775 6c61 7220  end rectangular 
-000025b0: 7365 6c65 6374 696f 6e20 746f 2073 7461  selection to sta
-000025c0: 7274 206f 6620 646f 6375 6d65 6e74 206c  rt of document l
-000025d0: 696e 6507 0000 000b 5173 6369 436f 6d6d  ine.....QsciComm
-000025e0: 616e 6401 0300 0000 6a00 5200 6500 6300  and.....j.R.e.c.
-000025f0: 6800 7400 6500 6300 6b00 6900 6700 6500  h.t.e.c.k.i.g.e.
-00002600: 2000 4100 7500 7300 7700 6100 6800 6c00   .A.u.s.w.a.h.l.
-00002610: 2000 7500 6d00 2000 6500 6900 6e00 6500   .u.m. .e.i.n.e.
-00002620: 2000 5a00 6500 6900 6c00 6500 2000 6e00   .Z.e.i.l.e. .n.
-00002630: 6100 6300 6800 2000 6f00 6200 6500 6e00  a.c.h. .o.b.e.n.
-00002640: 2000 6500 7200 7700 6500 6900 7400 6500   .e.r.w.e.i.t.e.
-00002650: 7200 6e08 0000 0000 0600 0000 2845 7874  r.n.........(Ext
-00002660: 656e 6420 7265 6374 616e 6775 6c61 7220  end rectangular 
-00002670: 7365 6c65 6374 696f 6e20 7570 206f 6e65  selection up one
-00002680: 206c 696e 6507 0000 000b 5173 6369 436f   line.....QsciCo
-00002690: 6d6d 616e 6401 0300 0000 6a00 5200 6500  mmand.....j.R.e.
-000026a0: 6300 6800 7400 6500 6300 6b00 6900 6700  c.h.t.e.c.k.i.g.
-000026b0: 6500 2000 4100 7500 7300 7700 6100 6800  e. .A.u.s.w.a.h.
-000026c0: 6c00 2000 7500 6d00 2000 6500 6900 6e00  l. .u.m. .e.i.n.
-000026d0: 6500 2000 5300 6500 6900 7400 6500 2000  e. .S.e.i.t.e. .
-000026e0: 6e00 6100 6300 6800 2000 6f00 6200 6500  n.a.c.h. .o.b.e.
-000026f0: 6e00 2000 6500 7200 7700 6500 6900 7400  n. .e.r.w.e.i.t.
-00002700: 6500 7200 6e08 0000 0000 0600 0000 2845  e.r.n.........(E
-00002710: 7874 656e 6420 7265 6374 616e 6775 6c61  xtend rectangula
-00002720: 7220 7365 6c65 6374 696f 6e20 7570 206f  r selection up o
-00002730: 6e65 2070 6167 6507 0000 000b 5173 6369  ne page.....Qsci
-00002740: 436f 6d6d 616e 6401 0300 0000 5400 4100  Command.....T.A.
-00002750: 7500 7300 7700 6100 6800 6c00 2000 7500  u.s.w.a.h.l. .u.
-00002760: 6d00 2000 6500 6900 6e00 6500 2000 5a00  m. .e.i.n.e. .Z.
-00002770: 6500 6900 6c00 6500 2000 6e00 6100 6300  e.i.l.e. .n.a.c.
-00002780: 6800 2000 7500 6e00 7400 6500 6e00 2000  h. .u.n.t.e.n. .
-00002790: 6500 7200 7700 6500 6900 7400 6500 7200  e.r.w.e.i.t.e.r.
-000027a0: 6e08 0000 0000 0600 0000 1e45 7874 656e  n..........Exten
-000027b0: 6420 7365 6c65 6374 696f 6e20 646f 776e  d selection down
-000027c0: 206f 6e65 206c 696e 6507 0000 000b 5173   one line.....Qs
-000027d0: 6369 436f 6d6d 616e 6401 0300 0000 5400  ciCommand.....T.
-000027e0: 4100 7500 7300 7700 6100 6800 6c00 2000  A.u.s.w.a.h.l. .
-000027f0: 7500 6d00 2000 6500 6900 6e00 6500 2000  u.m. .e.i.n.e. .
-00002800: 5300 6500 6900 7400 6500 2000 6e00 6100  S.e.i.t.e. .n.a.
-00002810: 6300 6800 2000 7500 6e00 7400 6500 6e00  c.h. .u.n.t.e.n.
-00002820: 2000 6500 7200 7700 6500 6900 7400 6500   .e.r.w.e.i.t.e.
-00002830: 7200 6e08 0000 0000 0600 0000 1e45 7874  r.n..........Ext
-00002840: 656e 6420 7365 6c65 6374 696f 6e20 646f  end selection do
-00002850: 776e 206f 6e65 2070 6167 6507 0000 000b  wn one page.....
-00002860: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00002870: 5800 4100 7500 7300 7700 6100 6800 6c00  X.A.u.s.w.a.h.l.
-00002880: 2000 7500 6d00 2000 6500 6900 6e00 6500   .u.m. .e.i.n.e.
-00002890: 6e00 2000 4100 6200 7300 6100 7400 7a00  n. .A.b.s.a.t.z.
-000028a0: 2000 6e00 6100 6300 6800 2000 7500 6e00   .n.a.c.h. .u.n.
-000028b0: 7400 6500 6e00 2000 6500 7200 7700 6500  t.e.n. .e.r.w.e.
-000028c0: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
-000028d0: 0000 2345 7874 656e 6420 7365 6c65 6374  ..#Extend select
-000028e0: 696f 6e20 646f 776e 206f 6e65 2070 6172  ion down one par
-000028f0: 6167 7261 7068 0700 0000 0b51 7363 6943  agraph.....QsciC
-00002900: 6f6d 6d61 6e64 0103 0000 0056 0041 0075  ommand.....V.A.u
-00002910: 0073 0077 0061 0068 006c 0020 0075 006d  .s.w.a.h.l. .u.m
-00002920: 0020 0065 0069 006e 0020 005a 0065 0069  . .e.i.n. .Z.e.i
-00002930: 0063 0068 0065 006e 0020 006e 0061 0063  .c.h.e.n. .n.a.c
-00002940: 0068 0020 006c 0069 006e 006b 0073 0020  .h. .l.i.n.k.s. 
-00002950: 0065 0072 0077 0065 0069 0074 0065 0072  .e.r.w.e.i.t.e.r
-00002960: 006e 0800 0000 0006 0000 0023 4578 7465  .n.........#Exte
-00002970: 6e64 2073 656c 6563 7469 6f6e 206c 6566  nd selection lef
-00002980: 7420 6f6e 6520 6368 6172 6163 7465 7207  t one character.
-00002990: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
-000029a0: 0300 0000 5000 4100 7500 7300 7700 6100  ....P.A.u.s.w.a.
-000029b0: 6800 6c00 2000 7500 6d00 2000 6500 6900  h.l. .u.m. .e.i.
-000029c0: 6e00 2000 5700 6f00 7200 7400 2000 6e00  n. .W.o.r.t. .n.
-000029d0: 6100 6300 6800 2000 6c00 6900 6e00 6b00  a.c.h. .l.i.n.k.
-000029e0: 7300 2000 6500 7200 7700 6500 6900 7400  s. .e.r.w.e.i.t.
-000029f0: 6500 7200 6e08 0000 0000 0600 0000 1e45  e.r.n..........E
-00002a00: 7874 656e 6420 7365 6c65 6374 696f 6e20  xtend selection 
-00002a10: 6c65 6674 206f 6e65 2077 6f72 6407 0000  left one word...
-00002a20: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00002a30: 0000 5c00 4100 7500 7300 7700 6100 6800  ..\.A.u.s.w.a.h.
-00002a40: 6c00 2000 7500 6d00 2000 6500 6900 6e00  l. .u.m. .e.i.n.
-00002a50: 6500 6e00 2000 5700 6f00 7200 7400 7400  e.n. .W.o.r.t.t.
-00002a60: 6500 6900 6c00 2000 6e00 6100 6300 6800  e.i.l. .n.a.c.h.
-00002a70: 2000 6c00 6900 6e00 6b00 7300 2000 6500   .l.i.n.k.s. .e.
-00002a80: 7200 7700 6500 6900 7400 6500 7200 6e08  r.w.e.i.t.e.r.n.
-00002a90: 0000 0000 0600 0000 2345 7874 656e 6420  ........#Extend 
-00002aa0: 7365 6c65 6374 696f 6e20 6c65 6674 206f  selection left o
-00002ab0: 6e65 2077 6f72 6420 7061 7274 0700 0000  ne word part....
-00002ac0: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
-00002ad0: 0058 0041 0075 0073 0077 0061 0068 006c  .X.A.u.s.w.a.h.l
-00002ae0: 0020 0075 006d 0020 0065 0069 006e 0020  . .u.m. .e.i.n. 
-00002af0: 005a 0065 0069 0063 0068 0065 006e 0020  .Z.e.i.c.h.e.n. 
-00002b00: 006e 0061 0063 0068 0020 0072 0065 0063  .n.a.c.h. .r.e.c
-00002b10: 0068 0074 0073 0020 0065 0072 0077 0065  .h.t.s. .e.r.w.e
-00002b20: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
-00002b30: 0000 0024 4578 7465 6e64 2073 656c 6563  ...$Extend selec
-00002b40: 7469 6f6e 2072 6967 6874 206f 6e65 2063  tion right one c
-00002b50: 6861 7261 6374 6572 0700 0000 0b51 7363  haracter.....Qsc
-00002b60: 6943 6f6d 6d61 6e64 0103 0000 0052 0041  iCommand.....R.A
-00002b70: 0075 0073 0077 0061 0068 006c 0020 0075  .u.s.w.a.h.l. .u
-00002b80: 006d 0020 0065 0069 006e 0020 0057 006f  .m. .e.i.n. .W.o
-00002b90: 0072 0074 0020 006e 0061 0063 0068 0020  .r.t. .n.a.c.h. 
-00002ba0: 0072 0065 0063 0068 0074 0073 0020 0065  .r.e.c.h.t.s. .e
-00002bb0: 0072 0077 0065 0069 0074 0065 0072 006e  .r.w.e.i.t.e.r.n
-00002bc0: 0800 0000 0006 0000 001f 4578 7465 6e64  ..........Extend
-00002bd0: 2073 656c 6563 7469 6f6e 2072 6967 6874   selection right
-00002be0: 206f 6e65 2077 6f72 6407 0000 000b 5173   one word.....Qs
-00002bf0: 6369 436f 6d6d 616e 6401 0300 0000 5e00  ciCommand.....^.
-00002c00: 4100 7500 7300 7700 6100 6800 6c00 2000  A.u.s.w.a.h.l. .
-00002c10: 7500 6d00 2000 6500 6900 6e00 6500 6e00  u.m. .e.i.n.e.n.
-00002c20: 2000 5700 6f00 7200 7400 7400 6500 6900   .W.o.r.t.t.e.i.
-00002c30: 6c00 2000 6e00 6100 6300 6800 2000 7200  l. .n.a.c.h. .r.
-00002c40: 6500 6300 6800 7400 7300 2000 6500 7200  e.c.h.t.s. .e.r.
-00002c50: 7700 6500 6900 7400 6500 7200 6e08 0000  w.e.i.t.e.r.n...
-00002c60: 0000 0600 0000 2445 7874 656e 6420 7365  ......$Extend se
-00002c70: 6c65 6374 696f 6e20 7269 6768 7420 6f6e  lection right on
-00002c80: 6520 776f 7264 2070 6172 7407 0000 000b  e word part.....
-00002c90: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00002ca0: 5600 4100 7500 7300 7700 6100 6800 6c00  V.A.u.s.w.a.h.l.
-00002cb0: 2000 7a00 7500 6d00 2000 4500 6e00 6400   .z.u.m. .E.n.d.
-00002cc0: 6500 2000 6400 6500 7200 2000 4100 6e00  e. .d.e.r. .A.n.
-00002cd0: 7a00 6500 6900 6700 6500 7a00 6500 6900  z.e.i.g.e.z.e.i.
-00002ce0: 6c00 6500 2000 6500 7200 7700 6500 6900  l.e. .e.r.w.e.i.
-00002cf0: 7400 6500 7200 6e08 0000 0000 0600 0000  t.e.r.n.........
-00002d00: 2745 7874 656e 6420 7365 6c65 6374 696f  'Extend selectio
-00002d10: 6e20 746f 2065 6e64 206f 6620 6469 7370  n to end of disp
-00002d20: 6c61 7920 6c69 6e65 0700 0000 0b51 7363  lay line.....Qsc
-00002d30: 6943 6f6d 6d61 6e64 0103 0000 0090 0052  iCommand.......R
-00002d40: 0065 0063 0068 0074 0065 0063 006b 0069  .e.c.h.t.e.c.k.i
-00002d50: 0067 0065 0020 0041 0075 0073 0077 0061  .g.e. .A.u.s.w.a
-00002d60: 0068 006c 0020 007a 0075 006d 0020 0045  .h.l. .z.u.m. .E
-00002d70: 006e 0064 0065 0020 0064 0065 0072 0020  .n.d.e. .d.e.r. 
-00002d80: 0044 006f 006b 0075 006d 0065 006e 0074  .D.o.k.u.m.e.n.t
-00002d90: 0065 006e 002d 0020 006f 0064 0065 0072  .e.n.-. .o.d.e.r
-00002da0: 0020 0041 006e 007a 0065 0069 0067 0065  . .A.n.z.e.i.g.e
-00002db0: 007a 0065 0069 006c 0065 0020 0065 0072  .z.e.i.l.e. .e.r
-00002dc0: 0077 0065 0069 0074 0065 0072 006e 0800  .w.e.i.t.e.r.n..
-00002dd0: 0000 0006 0000 0033 4578 7465 6e64 2073  .......3Extend s
-00002de0: 656c 6563 7469 6f6e 2074 6f20 656e 6420  election to end 
-00002df0: 6f66 2064 6973 706c 6179 206f 7220 646f  of display or do
-00002e00: 6375 6d65 6e74 206c 696e 6507 0000 000b  cument line.....
-00002e10: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00002e20: 4800 4100 7500 7300 7700 6100 6800 6c00  H.A.u.s.w.a.h.l.
-00002e30: 2000 7a00 7500 6d00 2000 4400 6f00 6b00   .z.u.m. .D.o.k.
-00002e40: 7500 6d00 6500 6e00 7400 6500 6e00 6500  u.m.e.n.t.e.n.e.
-00002e50: 6e00 6400 6500 2000 6500 7200 7700 6500  n.d.e. .e.r.w.e.
-00002e60: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
-00002e70: 0000 2345 7874 656e 6420 7365 6c65 6374  ..#Extend select
-00002e80: 696f 6e20 746f 2065 6e64 206f 6620 646f  ion to end of do
-00002e90: 6375 6d65 6e74 0700 0000 0b51 7363 6943  cument.....QsciC
-00002ea0: 6f6d 6d61 6e64 0103 0000 005c 0041 0075  ommand.....\.A.u
-00002eb0: 0073 0077 0061 0068 006c 0020 007a 0075  .s.w.a.h.l. .z.u
-00002ec0: 006d 0020 0045 006e 0064 0065 0020 0064  .m. .E.n.d.e. .d
-00002ed0: 0065 0072 0020 0044 006f 006b 0075 006d  .e.r. .D.o.k.u.m
-00002ee0: 0065 006e 0074 0065 006e 007a 0065 0069  .e.n.t.e.n.z.e.i
-00002ef0: 006c 0065 0020 0065 0072 0077 0065 0069  .l.e. .e.r.w.e.i
-00002f00: 0074 0065 0072 006e 0800 0000 0006 0000  .t.e.r.n........
-00002f10: 0028 4578 7465 6e64 2073 656c 6563 7469  .(Extend selecti
-00002f20: 6f6e 2074 6f20 656e 6420 6f66 2064 6f63  on to end of doc
-00002f30: 756d 656e 7420 6c69 6e65 0700 0000 0b51  ument line.....Q
-00002f40: 7363 6943 6f6d 6d61 6e64 0103 0000 0064  sciCommand.....d
-00002f50: 0041 0075 0073 0077 0061 0068 006c 0020  .A.u.s.w.a.h.l. 
-00002f60: 0062 0069 0073 0020 007a 0075 006d 0020  .b.i.s. .z.u.m. 
-00002f70: 0045 006e 0064 0065 0020 0064 0065 0073  .E.n.d.e. .d.e.s
-00002f80: 0020 006e 00e4 0063 0068 0073 0074 0065  . .n...c.h.s.t.e
-00002f90: 006e 0020 0057 006f 0072 0074 0065 0073  .n. .W.o.r.t.e.s
-00002fa0: 0020 0065 0072 0077 0065 0069 0074 0065  . .e.r.w.e.i.t.e
-00002fb0: 0072 006e 0800 0000 0006 0000 0024 4578  .r.n.........$Ex
-00002fc0: 7465 6e64 2073 656c 6563 7469 6f6e 2074  tend selection t
-00002fd0: 6f20 656e 6420 6f66 206e 6578 7420 776f  o end of next wo
-00002fe0: 7264 0700 0000 0b51 7363 6943 6f6d 6d61  rd.....QsciComma
-00002ff0: 6e64 0103 0000 0062 0041 0075 0073 0077  nd.....b.A.u.s.w
-00003000: 0061 0068 006c 0020 0062 0069 0073 0020  .a.h.l. .b.i.s. 
-00003010: 007a 0075 006d 0020 0045 006e 0064 0065  .z.u.m. .E.n.d.e
-00003020: 0020 0064 0065 0073 0020 0076 006f 0072  . .d.e.s. .v.o.r
-00003030: 0069 0067 0065 006e 0020 0057 006f 0072  .i.g.e.n. .W.o.r
-00003040: 0074 0065 0073 0020 0065 0072 0077 0065  .t.e.s. .e.r.w.e
-00003050: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
-00003060: 0000 0028 4578 7465 6e64 2073 656c 6563  ...(Extend selec
-00003070: 7469 6f6e 2074 6f20 656e 6420 6f66 2070  tion to end of p
-00003080: 7265 7669 6f75 7320 776f 7264 0700 0000  revious word....
-00003090: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
-000030a0: 009e 0041 0075 0073 0077 0061 0068 006c  ...A.u.s.w.a.h.l
-000030b0: 0020 007a 0075 006d 0020 0065 0072 0073  . .z.u.m. .e.r.s
-000030c0: 0074 0065 006e 0020 0073 0069 0063 0068  .t.e.n. .s.i.c.h
-000030d0: 0074 0062 0061 0072 0065 006e 0020 005a  .t.b.a.r.e.n. .Z
-000030e0: 0065 0069 0063 0068 0065 006e 0020 0064  .e.i.c.h.e.n. .d
-000030f0: 0065 0072 0020 0044 006f 006b 0075 006d  .e.r. .D.o.k.u.m
-00003100: 0065 006e 0074 002d 0020 006f 0064 0065  .e.n.t.-. .o.d.e
-00003110: 0072 0020 0041 006e 007a 0065 0069 0067  .r. .A.n.z.e.i.g
-00003120: 0065 007a 0065 0069 006c 0065 0020 0065  .e.z.e.i.l.e. .e
-00003130: 0072 0077 0065 0069 0074 0065 0072 006e  .r.w.e.i.t.e.r.n
-00003140: 0800 0000 0006 0000 0047 4578 7465 6e64  .........GExtend
-00003150: 2073 656c 6563 7469 6f6e 2074 6f20 6669   selection to fi
-00003160: 7273 7420 7669 7369 626c 6520 6368 6172  rst visible char
-00003170: 6163 7465 7220 696e 2064 6973 706c 6179  acter in display
-00003180: 206f 7220 646f 6375 6d65 6e74 206c 696e   or document lin
-00003190: 6507 0000 000b 5173 6369 436f 6d6d 616e  e.....QsciComman
-000031a0: 6401 0300 0000 8200 4100 7500 7300 7700  d.......A.u.s.w.
-000031b0: 6100 6800 6c00 2000 7a00 7500 6d00 2000  a.h.l. .z.u.m. .
-000031c0: 6500 7200 7300 7400 6500 6e00 2000 7300  e.r.s.t.e.n. .s.
-000031d0: 6900 6300 6800 7400 6200 6100 7200 6500  i.c.h.t.b.a.r.e.
-000031e0: 6e00 2000 5a00 6500 6900 6300 6800 6500  n. .Z.e.i.c.h.e.
-000031f0: 6e00 2000 6400 6500 7200 2000 4400 6f00  n. .d.e.r. .D.o.
-00003200: 6b00 7500 6d00 6500 6e00 7400 7a00 6500  k.u.m.e.n.t.z.e.
-00003210: 6900 6c00 6500 2000 6500 7200 7700 6500  i.l.e. .e.r.w.e.
-00003220: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
-00003230: 0000 3c45 7874 656e 6420 7365 6c65 6374  ..<Extend select
-00003240: 696f 6e20 746f 2066 6972 7374 2076 6973  ion to first vis
-00003250: 6962 6c65 2063 6861 7261 6374 6572 2069  ible character i
-00003260: 6e20 646f 6375 6d65 6e74 206c 696e 6507  n document line.
-00003270: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
-00003280: 0300 0000 5a00 4100 7500 7300 7700 6100  ....Z.A.u.s.w.a.
-00003290: 6800 6c00 2000 7a00 7500 6d00 2000 4200  h.l. .z.u.m. .B.
-000032a0: 6500 6700 6900 6e00 6e00 2000 6400 6500  e.g.i.n.n. .d.e.
-000032b0: 7200 2000 4100 6e00 7a00 6500 6900 6700  r. .A.n.z.e.i.g.
-000032c0: 6500 7a00 6500 6900 6c00 6500 2000 6500  e.z.e.i.l.e. .e.
-000032d0: 7200 7700 6500 6900 7400 6500 7200 6e08  r.w.e.i.t.e.r.n.
-000032e0: 0000 0000 0600 0000 2945 7874 656e 6420  ........)Extend 
-000032f0: 7365 6c65 6374 696f 6e20 746f 2073 7461  selection to sta
-00003300: 7274 206f 6620 6469 7370 6c61 7920 6c69  rt of display li
-00003310: 6e65 0700 0000 0b51 7363 6943 6f6d 6d61  ne.....QsciComma
-00003320: 6e64 0103 0000 0094 0052 0065 0063 0068  nd.......R.e.c.h
-00003330: 0074 0065 0063 006b 0069 0067 0065 0020  .t.e.c.k.i.g.e. 
-00003340: 0041 0075 0073 0077 0061 0068 006c 0020  .A.u.s.w.a.h.l. 
-00003350: 007a 0075 006d 0020 0042 0065 0067 0069  .z.u.m. .B.e.g.i
-00003360: 006e 006e 0020 0064 0065 0072 0020 0044  .n.n. .d.e.r. .D
-00003370: 006f 006b 0075 006d 0065 006e 0074 0065  .o.k.u.m.e.n.t.e
-00003380: 006e 002d 0020 006f 0064 0065 0072 0020  .n.-. .o.d.e.r. 
-00003390: 0041 006e 007a 0065 0069 0067 0065 007a  .A.n.z.e.i.g.e.z
-000033a0: 0065 0069 006c 0065 0020 0065 0072 0077  .e.i.l.e. .e.r.w
-000033b0: 0065 0069 0074 0065 0072 006e 0800 0000  .e.i.t.e.r.n....
-000033c0: 0006 0000 0035 4578 7465 6e64 2073 656c  .....5Extend sel
-000033d0: 6563 7469 6f6e 2074 6f20 7374 6172 7420  ection to start 
-000033e0: 6f66 2064 6973 706c 6179 206f 7220 646f  of display or do
-000033f0: 6375 6d65 6e74 206c 696e 6507 0000 000b  cument line.....
-00003400: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00003410: 4c00 4100 7500 7300 7700 6100 6800 6c00  L.A.u.s.w.a.h.l.
-00003420: 2000 7a00 7500 6d00 2000 4400 6f00 6b00   .z.u.m. .D.o.k.
-00003430: 7500 6d00 6500 6e00 7400 6500 6e00 6100  u.m.e.n.t.e.n.a.
-00003440: 6e00 6600 6100 6e00 6700 2000 6500 7200  n.f.a.n.g. .e.r.
-00003450: 7700 6500 6900 7400 6500 7200 6e08 0000  w.e.i.t.e.r.n...
-00003460: 0000 0600 0000 2545 7874 656e 6420 7365  ......%Extend se
-00003470: 6c65 6374 696f 6e20 746f 2073 7461 7274  lection to start
-00003480: 206f 6620 646f 6375 6d65 6e74 0700 0000   of document....
-00003490: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
-000034a0: 0060 0041 0075 0073 0077 0061 0068 006c  .`.A.u.s.w.a.h.l
-000034b0: 0020 007a 0075 006d 0020 0042 0065 0067  . .z.u.m. .B.e.g
-000034c0: 0069 006e 006e 0020 0064 0065 0072 0020  .i.n.n. .d.e.r. 
-000034d0: 0044 006f 006b 0075 006d 0065 006e 0074  .D.o.k.u.m.e.n.t
-000034e0: 0065 006e 007a 0065 0069 006c 0065 0020  .e.n.z.e.i.l.e. 
-000034f0: 0065 0072 0077 0065 0069 0074 0065 0072  .e.r.w.e.i.t.e.r
-00003500: 006e 0800 0000 0006 0000 002a 4578 7465  .n.........*Exte
-00003510: 6e64 2073 656c 6563 7469 6f6e 2074 6f20  nd selection to 
-00003520: 7374 6172 7420 6f66 2064 6f63 756d 656e  start of documen
-00003530: 7420 6c69 6e65 0700 0000 0b51 7363 6943  t line.....QsciC
-00003540: 6f6d 6d61 6e64 0103 0000 0052 0041 0075  ommand.....R.A.u
-00003550: 0073 0077 0061 0068 006c 0020 0075 006d  .s.w.a.h.l. .u.m
-00003560: 0020 0065 0069 006e 0065 0020 005a 0065  . .e.i.n.e. .Z.e
-00003570: 0069 006c 0065 0020 006e 0061 0063 0068  .i.l.e. .n.a.c.h
-00003580: 0020 006f 0062 0065 006e 0020 0065 0072  . .o.b.e.n. .e.r
-00003590: 0077 0065 0069 0074 0065 0072 006e 0800  .w.e.i.t.e.r.n..
-000035a0: 0000 0006 0000 001c 4578 7465 6e64 2073  ........Extend s
-000035b0: 656c 6563 7469 6f6e 2075 7020 6f6e 6520  election up one 
-000035c0: 6c69 6e65 0700 0000 0b51 7363 6943 6f6d  line.....QsciCom
-000035d0: 6d61 6e64 0103 0000 0052 0041 0075 0073  mand.....R.A.u.s
-000035e0: 0077 0061 0068 006c 0020 0075 006d 0020  .w.a.h.l. .u.m. 
-000035f0: 0065 0069 006e 0065 0020 0053 0065 0069  .e.i.n.e. .S.e.i
-00003600: 0074 0065 0020 006e 0061 0063 0068 0020  .t.e. .n.a.c.h. 
-00003610: 006f 0062 0065 006e 0020 0065 0072 0077  .o.b.e.n. .e.r.w
-00003620: 0065 0069 0074 0065 0072 006e 0800 0000  .e.i.t.e.r.n....
-00003630: 0006 0000 001c 4578 7465 6e64 2073 656c  ......Extend sel
-00003640: 6563 7469 6f6e 2075 7020 6f6e 6520 7061  ection up one pa
-00003650: 6765 0700 0000 0b51 7363 6943 6f6d 6d61  ge.....QsciComma
-00003660: 6e64 0103 0000 0056 0041 0075 0073 0077  nd.....V.A.u.s.w
-00003670: 0061 0068 006c 0020 0075 006d 0020 0065  .a.h.l. .u.m. .e
-00003680: 0069 006e 0065 006e 0020 0041 0062 0073  .i.n.e.n. .A.b.s
-00003690: 0061 0074 007a 0020 006e 0061 0063 0068  .a.t.z. .n.a.c.h
-000036a0: 0020 006f 0062 0065 006e 0020 0065 0072  . .o.b.e.n. .e.r
-000036b0: 0077 0065 0069 0074 0065 0072 006e 0800  .w.e.i.t.e.r.n..
-000036c0: 0000 0006 0000 0021 4578 7465 6e64 2073  .......!Extend s
-000036d0: 656c 6563 7469 6f6e 2075 7020 6f6e 6520  election up one 
-000036e0: 7061 7261 6772 6170 6807 0000 000b 5173  paragraph.....Qs
-000036f0: 6369 436f 6d6d 616e 6401 0300 0000 1a00  ciCommand.......
-00003700: 5300 6500 6900 7400 6500 6e00 7500 6d00  S.e.i.t.e.n.u.m.
-00003710: 6200 7200 7500 6300 6808 0000 0000 0600  b.r.u.c.h.......
-00003720: 0000 0846 6f72 6d66 6565 6407 0000 000b  ...Formfeed.....
-00003730: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
-00003740: 2800 4500 6900 6e00 6500 2000 4500 6200  (.E.i.n.e. .E.b.
-00003750: 6500 6e00 6500 2000 6500 6900 6e00 7200  e.n.e. .e.i.n.r.
-00003760: fc00 6300 6b00 6500 6e08 0000 0000 0600  ..c.k.e.n.......
-00003770: 0000 1049 6e64 656e 7420 6f6e 6520 6c65  ...Indent one le
-00003780: 7665 6c07 0000 000b 5173 6369 436f 6d6d  vel.....QsciComm
-00003790: 616e 6401 0300 0000 2600 4e00 6500 7500  and.....&.N.e.u.
-000037a0: 6500 2000 5a00 6500 6900 6c00 6500 2000  e. .Z.e.i.l.e. .
-000037b0: 6500 6900 6e00 6600 fc00 6700 6500 6e08  e.i.n.f...g.e.n.
-000037c0: 0000 0000 0600 0000 0e49 6e73 6572 7420  .........Insert 
-000037d0: 6e65 776c 696e 6507 0000 000b 5173 6369  newline.....Qsci
-000037e0: 436f 6d6d 616e 6401 0300 0000 2a00 4500  Command.....*.E.
-000037f0: 6900 6e00 6500 2000 5a00 6500 6900 6c00  i.n.e. .Z.e.i.l.
-00003800: 6500 2000 6e00 6100 6300 6800 2000 7500  e. .n.a.c.h. .u.
-00003810: 6e00 7400 6500 6e08 0000 0000 0600 0000  n.t.e.n.........
-00003820: 124d 6f76 6520 646f 776e 206f 6e65 206c  .Move down one l
-00003830: 696e 6507 0000 000b 5173 6369 436f 6d6d  ine.....QsciComm
-00003840: 616e 6401 0300 0000 2a00 4500 6900 6e00  and.....*.E.i.n.
-00003850: 6500 2000 5300 6500 6900 7400 6500 2000  e. .S.e.i.t.e. .
-00003860: 6e00 6100 6300 6800 2000 7500 6e00 7400  n.a.c.h. .u.n.t.
-00003870: 6500 6e08 0000 0000 0600 0000 124d 6f76  e.n..........Mov
-00003880: 6520 646f 776e 206f 6e65 2070 6167 6507  e down one page.
-00003890: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
-000038a0: 0300 0000 2e00 4500 6900 6e00 6500 6e00  ......E.i.n.e.n.
-000038b0: 2000 4100 6200 7300 6100 7400 7a00 2000   .A.b.s.a.t.z. .
-000038c0: 6e00 6100 6300 6800 2000 7500 6e00 7400  n.a.c.h. .u.n.t.
-000038d0: 6500 6e08 0000 0000 0600 0000 174d 6f76  e.n..........Mov
-000038e0: 6520 646f 776e 206f 6e65 2070 6172 6167  e down one parag
-000038f0: 7261 7068 0700 0000 0b51 7363 6943 6f6d  raph.....QsciCom
-00003900: 6d61 6e64 0103 0000 002c 0045 0069 006e  mand.....,.E.i.n
-00003910: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-00003920: 0020 006e 0061 0063 0068 0020 006c 0069  . .n.a.c.h. .l.i
-00003930: 006e 006b 0073 0800 0000 0006 0000 0017  .n.k.s..........
-00003940: 4d6f 7665 206c 6566 7420 6f6e 6520 6368  Move left one ch
-00003950: 6172 6163 7465 7207 0000 000b 5173 6369  aracter.....Qsci
-00003960: 436f 6d6d 616e 6401 0300 0000 2600 4500  Command.....&.E.
-00003970: 6900 6e00 2000 5700 6f00 7200 7400 2000  i.n. .W.o.r.t. .
-00003980: 6e00 6100 6300 6800 2000 6c00 6900 6e00  n.a.c.h. .l.i.n.
-00003990: 6b00 7308 0000 0000 0600 0000 124d 6f76  k.s..........Mov
-000039a0: 6520 6c65 6674 206f 6e65 2077 6f72 6407  e left one word.
-000039b0: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
-000039c0: 0300 0000 2e00 4500 6900 6e00 2000 5700  ......E.i.n. .W.
-000039d0: 6f00 7200 7400 7400 6500 6900 6c00 2000  o.r.t.t.e.i.l. .
-000039e0: 6e00 6100 6300 6800 2000 6c00 6900 6e00  n.a.c.h. .l.i.n.
-000039f0: 6b00 7308 0000 0000 0600 0000 174d 6f76  k.s..........Mov
-00003a00: 6520 6c65 6674 206f 6e65 2077 6f72 6420  e left one word 
-00003a10: 7061 7274 0700 0000 0b51 7363 6943 6f6d  part.....QsciCom
-00003a20: 6d61 6e64 0103 0000 002e 0045 0069 006e  mand.......E.i.n
-00003a30: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-00003a40: 0020 006e 0061 0063 0068 0020 0072 0065  . .n.a.c.h. .r.e
-00003a50: 0063 0068 0074 0073 0800 0000 0006 0000  .c.h.t.s........
-00003a60: 0018 4d6f 7665 2072 6967 6874 206f 6e65  ..Move right one
-00003a70: 2063 6861 7261 6374 6572 0700 0000 0b51   character.....Q
-00003a80: 7363 6943 6f6d 6d61 6e64 0103 0000 0028  sciCommand.....(
-00003a90: 0045 0069 006e 0020 0057 006f 0072 0074  .E.i.n. .W.o.r.t
-00003aa0: 0020 006e 0061 0063 0068 0020 0072 0065  . .n.a.c.h. .r.e
-00003ab0: 0063 0068 0074 0073 0800 0000 0006 0000  .c.h.t.s........
-00003ac0: 0013 4d6f 7665 2072 6967 6874 206f 6e65  ..Move right one
-00003ad0: 2077 6f72 6407 0000 000b 5173 6369 436f   word.....QsciCo
-00003ae0: 6d6d 616e 6401 0300 0000 3000 4500 6900  mmand.....0.E.i.
-00003af0: 6e00 2000 5700 6f00 7200 7400 7400 6500  n. .W.o.r.t.t.e.
-00003b00: 6900 6c00 2000 6e00 6100 6300 6800 2000  i.l. .n.a.c.h. .
-00003b10: 7200 6500 6300 6800 7400 7308 0000 0000  r.e.c.h.t.s.....
-00003b20: 0600 0000 184d 6f76 6520 7269 6768 7420  .....Move right 
-00003b30: 6f6e 6520 776f 7264 2070 6172 7407 0000  one word part...
-00003b40: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00003b50: 0000 5600 4100 7500 7300 6700 6500 7700  ..V.A.u.s.g.e.w.
-00003b60: e400 6800 6c00 7400 6500 2000 5a00 6500  ..h.l.t.e. .Z.e.
-00003b70: 6900 6c00 6500 6e00 2000 7500 6d00 2000  i.l.e.n. .u.m. .
-00003b80: 6500 6900 6e00 6500 2000 5a00 6500 6900  e.i.n.e. .Z.e.i.
-00003b90: 6c00 6500 2000 6e00 6100 6300 6800 2000  l.e. .n.a.c.h. .
-00003ba0: 7500 6e00 7400 6500 6e08 0000 0000 0600  u.n.t.e.n.......
-00003bb0: 0000 214d 6f76 6520 7365 6c65 6374 6564  ..!Move selected
-00003bc0: 206c 696e 6573 2064 6f77 6e20 6f6e 6520   lines down one 
-00003bd0: 6c69 6e65 0700 0000 0b51 7363 6943 6f6d  line.....QsciCom
-00003be0: 6d61 6e64 0103 0000 0054 0041 0075 0073  mand.....T.A.u.s
-00003bf0: 0067 0065 0077 00e4 0068 006c 0074 0065  .g.e.w...h.l.t.e
-00003c00: 0020 005a 0065 0069 006c 0065 006e 0020  . .Z.e.i.l.e.n. 
-00003c10: 0075 006d 0020 0065 0069 006e 0065 0020  .u.m. .e.i.n.e. 
-00003c20: 005a 0065 0069 006c 0065 0020 006e 0061  .Z.e.i.l.e. .n.a
-00003c30: 0063 0068 0020 006f 0062 0065 006e 0800  .c.h. .o.b.e.n..
-00003c40: 0000 0006 0000 001f 4d6f 7665 2073 656c  ........Move sel
-00003c50: 6563 7465 6420 6c69 6e65 7320 7570 206f  ected lines up o
-00003c60: 6e65 206c 696e 6507 0000 000b 5173 6369  ne line.....Qsci
-00003c70: 436f 6d6d 616e 6401 0300 0000 4400 5a00  Command.....D.Z.
-00003c80: 7500 6d00 2000 4500 6e00 6400 6500 2000  u.m. .E.n.d.e. .
-00003c90: 6400 6500 7200 2000 4100 6e00 7a00 6500  d.e.r. .A.n.z.e.
-00003ca0: 6900 6700 6500 7a00 6500 6900 6c00 6500  i.g.e.z.e.i.l.e.
-00003cb0: 2000 7300 7000 7200 6900 6e00 6700 6500   .s.p.r.i.n.g.e.
-00003cc0: 6e08 0000 0000 0600 0000 1b4d 6f76 6520  n..........Move 
-00003cd0: 746f 2065 6e64 206f 6620 6469 7370 6c61  to end of displa
-00003ce0: 7920 6c69 6e65 0700 0000 0b51 7363 6943  y line.....QsciC
-00003cf0: 6f6d 6d61 6e64 0103 0000 0066 005a 0075  ommand.....f.Z.u
-00003d00: 006d 0020 0045 006e 0064 0065 0020 0064  .m. .E.n.d.e. .d
-00003d10: 0065 0072 0020 0044 006f 006b 0075 006d  .e.r. .D.o.k.u.m
-00003d20: 0065 006e 0074 0065 006e 002d 0020 006f  .e.n.t.e.n.-. .o
-00003d30: 0064 0065 0072 0020 0041 006e 007a 0065  .d.e.r. .A.n.z.e
-00003d40: 0069 0067 0065 007a 0065 0069 006c 0065  .i.g.e.z.e.i.l.e
-00003d50: 0020 0073 0070 0072 0069 006e 0067 0065  . .s.p.r.i.n.g.e
-00003d60: 006e 0800 0000 0006 0000 0027 4d6f 7665  .n.........'Move
-00003d70: 2074 6f20 656e 6420 6f66 2064 6973 706c   to end of displ
-00003d80: 6179 206f 7220 646f 6375 6d65 6e74 206c  ay or document l
-00003d90: 696e 6507 0000 000b 5173 6369 436f 6d6d  ine.....QsciComm
-00003da0: 616e 6401 0300 0000 3600 5a00 7500 6d00  and.....6.Z.u.m.
-00003db0: 2000 4400 6f00 6b00 7500 6d00 6500 6e00   .D.o.k.u.m.e.n.
-00003dc0: 7400 6500 6e00 6500 6e00 6400 6500 2000  t.e.n.e.n.d.e. .
-00003dd0: 7300 7000 7200 6900 6e00 6700 6500 6e08  s.p.r.i.n.g.e.n.
-00003de0: 0000 0000 0600 0000 174d 6f76 6520 746f  .........Move to
-00003df0: 2065 6e64 206f 6620 646f 6375 6d65 6e74   end of document
-00003e00: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
-00003e10: 0103 0000 0046 005a 0075 006d 0020 0045  .....F.Z.u.m. .E
-00003e20: 006e 0064 0065 0020 0064 0065 0072 0020  .n.d.e. .d.e.r. 
-00003e30: 0044 006f 006b 0075 006d 0065 006e 0074  .D.o.k.u.m.e.n.t
-00003e40: 007a 0065 0069 006c 0065 0020 0073 0070  .z.e.i.l.e. .s.p
-00003e50: 0072 0069 006e 0067 0065 006e 0800 0000  .r.i.n.g.e.n....
-00003e60: 0006 0000 001c 4d6f 7665 2074 6f20 656e  ......Move to en
-00003e70: 6420 6f66 2064 6f63 756d 656e 7420 6c69  d of document li
-00003e80: 6e65 0700 0000 0b51 7363 6943 6f6d 6d61  ne.....QsciComma
-00003e90: 6e64 0103 0000 004a 005a 0075 006d 0020  nd.....J.Z.u.m. 
-00003ea0: 0045 006e 0064 0065 0020 0064 0065 0073  .E.n.d.e. .d.e.s
-00003eb0: 0020 006e 00e4 0063 0068 0073 0074 0065  . .n...c.h.s.t.e
-00003ec0: 006e 0020 0057 006f 0072 0074 0065 0073  .n. .W.o.r.t.e.s
-00003ed0: 0020 0073 0070 0072 0069 006e 0067 0065  . .s.p.r.i.n.g.e
-00003ee0: 006e 0800 0000 0006 0000 0018 4d6f 7665  .n..........Move
-00003ef0: 2074 6f20 656e 6420 6f66 206e 6578 7420   to end of next 
-00003f00: 776f 7264 0700 0000 0b51 7363 6943 6f6d  word.....QsciCom
-00003f10: 6d61 6e64 0103 0000 0048 005a 0075 006d  mand.....H.Z.u.m
-00003f20: 0020 0045 006e 0064 0065 0020 0064 0065  . .E.n.d.e. .d.e
-00003f30: 0073 0020 0076 006f 0072 0069 0067 0065  .s. .v.o.r.i.g.e
-00003f40: 006e 0020 0057 006f 0072 0074 0065 0073  .n. .W.o.r.t.e.s
-00003f50: 0020 0073 0070 0072 0069 006e 0067 0065  . .s.p.r.i.n.g.e
-00003f60: 006e 0800 0000 0006 0000 001c 4d6f 7665  .n..........Move
-00003f70: 2074 6f20 656e 6420 6f66 2070 7265 7669   to end of previ
-00003f80: 6f75 7320 776f 7264 0700 0000 0b51 7363  ous word.....Qsc
-00003f90: 6943 6f6d 6d61 6e64 0103 0000 0070 005a  iCommand.....p.Z
-00003fa0: 0075 006d 0020 0065 0072 0073 0074 0065  .u.m. .e.r.s.t.e
-00003fb0: 006e 0020 0073 0069 0063 0068 0074 0062  .n. .s.i.c.h.t.b
-00003fc0: 0061 0072 0065 006e 0020 005a 0065 0069  .a.r.e.n. .Z.e.i
-00003fd0: 0063 0068 0065 006e 0020 0064 0065 0072  .c.h.e.n. .d.e.r
-00003fe0: 0020 0044 006f 006b 0075 006d 0065 006e  . .D.o.k.u.m.e.n
-00003ff0: 0074 007a 0065 0069 006c 0065 0020 0073  .t.z.e.i.l.e. .s
-00004000: 0070 0072 0069 006e 0067 0065 006e 0800  .p.r.i.n.g.e.n..
-00004010: 0000 0006 0000 0030 4d6f 7665 2074 6f20  .......0Move to 
-00004020: 6669 7273 7420 7669 7369 626c 6520 6368  first visible ch
-00004030: 6172 6163 7465 7220 696e 2064 6f63 756d  aracter in docum
-00004040: 656e 7420 6c69 6e65 0700 0000 0b51 7363  ent line.....Qsc
-00004050: 6943 6f6d 6d61 6e64 0103 0000 0072 005a  iCommand.....r.Z
-00004060: 0075 006d 0020 0065 0072 0073 0074 0065  .u.m. .e.r.s.t.e
-00004070: 006e 0020 0061 006e 0067 0065 007a 0065  .n. .a.n.g.e.z.e
-00004080: 0069 0067 0074 0065 006e 0020 005a 0065  .i.g.t.e.n. .Z.e
-00004090: 0069 0063 0068 0065 006e 0020 0064 0065  .i.c.h.e.n. .d.e
-000040a0: 0072 0020 0044 006f 006b 0075 006d 0065  .r. .D.o.k.u.m.e
-000040b0: 006e 0074 007a 0065 0069 006c 0065 0020  .n.t.z.e.i.l.e. 
-000040c0: 0073 0070 0072 0069 006e 0067 0065 006e  .s.p.r.i.n.g.e.n
-000040d0: 0800 0000 0006 0000 003b 4d6f 7665 2074  .........;Move t
-000040e0: 6f20 6669 7273 7420 7669 7369 626c 6520  o first visible 
-000040f0: 6368 6172 6163 7465 7220 6f66 2064 6973  character of dis
-00004100: 706c 6179 2069 6e20 646f 6375 6d65 6e74  play in document
-00004110: 206c 696e 6507 0000 000b 5173 6369 436f   line.....QsciCo
-00004120: 6d6d 616e 6401 0300 0000 4800 5a00 7500  mmand.....H.Z.u.
-00004130: 6d00 2000 4200 6500 6700 6900 6e00 6e00  m. .B.e.g.i.n.n.
-00004140: 2000 6400 6500 7200 2000 4100 6e00 7a00   .d.e.r. .A.n.z.
-00004150: 6500 6900 6700 6500 7a00 6500 6900 6c00  e.i.g.e.z.e.i.l.
-00004160: 6500 2000 7300 7000 7200 6900 6e00 6700  e. .s.p.r.i.n.g.
-00004170: 6500 6e08 0000 0000 0600 0000 1d4d 6f76  e.n..........Mov
-00004180: 6520 746f 2073 7461 7274 206f 6620 6469  e to start of di
-00004190: 7370 6c61 7920 6c69 6e65 0700 0000 0b51  splay line.....Q
-000041a0: 7363 6943 6f6d 6d61 6e64 0103 0000 006a  sciCommand.....j
-000041b0: 005a 0075 006d 0020 0042 0065 0067 0069  .Z.u.m. .B.e.g.i
-000041c0: 006e 006e 0020 0064 0065 0072 0020 0044  .n.n. .d.e.r. .D
-000041d0: 006f 006b 0075 006d 0065 006e 0074 0065  .o.k.u.m.e.n.t.e
-000041e0: 006e 002d 0020 006f 0064 0065 0072 0020  .n.-. .o.d.e.r. 
-000041f0: 0041 006e 007a 0065 0069 0067 0065 007a  .A.n.z.e.i.g.e.z
-00004200: 0065 0069 006c 0065 0020 0073 0070 0072  .e.i.l.e. .s.p.r
-00004210: 0069 006e 0067 0065 006e 0800 0000 0006  .i.n.g.e.n......
-00004220: 0000 0029 4d6f 7665 2074 6f20 7374 6172  ...)Move to star
-00004230: 7420 6f66 2064 6973 706c 6179 206f 7220  t of display or 
-00004240: 646f 6375 6d65 6e74 206c 696e 6507 0000  document line...
-00004250: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00004260: 0000 3a00 5a00 7500 6d00 2000 4400 6f00  ..:.Z.u.m. .D.o.
-00004270: 6b00 7500 6d00 6500 6e00 7400 6500 6e00  k.u.m.e.n.t.e.n.
-00004280: 6100 6e00 6600 6100 6e00 6700 2000 7300  a.n.f.a.n.g. .s.
-00004290: 7000 7200 6900 6e00 6700 6500 6e08 0000  p.r.i.n.g.e.n...
-000042a0: 0000 0600 0000 194d 6f76 6520 746f 2073  .......Move to s
-000042b0: 7461 7274 206f 6620 646f 6375 6d65 6e74  tart of document
-000042c0: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
-000042d0: 0103 0000 004e 005a 0075 006d 0020 0042  .....N.Z.u.m. .B
-000042e0: 0065 0067 0069 006e 006e 0020 0064 0065  .e.g.i.n.n. .d.e
-000042f0: 0072 0020 0044 006f 006b 0075 006d 0065  .r. .D.o.k.u.m.e
-00004300: 006e 0074 0065 006e 007a 0065 0069 006c  .n.t.e.n.z.e.i.l
-00004310: 0065 0020 0073 0070 0072 0069 006e 0067  .e. .s.p.r.i.n.g
-00004320: 0065 006e 0800 0000 0006 0000 001e 4d6f  .e.n..........Mo
-00004330: 7665 2074 6f20 7374 6172 7420 6f66 2064  ve to start of d
-00004340: 6f63 756d 656e 7420 6c69 6e65 0700 0000  ocument line....
-00004350: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
-00004360: 0028 0045 0069 006e 0065 0020 005a 0065  .(.E.i.n.e. .Z.e
-00004370: 0069 006c 0065 0020 006e 0061 0063 0068  .i.l.e. .n.a.c.h
-00004380: 0020 006f 0062 0065 006e 0800 0000 0006  . .o.b.e.n......
-00004390: 0000 0010 4d6f 7665 2075 7020 6f6e 6520  ....Move up one 
-000043a0: 6c69 6e65 0700 0000 0b51 7363 6943 6f6d  line.....QsciCom
-000043b0: 6d61 6e64 0103 0000 001e 0045 0069 006e  mand.......E.i.n
-000043c0: 0065 0020 0053 0065 0069 0074 0065 0020  .e. .S.e.i.t.e. 
-000043d0: 0068 006f 0063 0068 0800 0000 0006 0000  .h.o.c.h........
-000043e0: 0010 4d6f 7665 2075 7020 6f6e 6520 7061  ..Move up one pa
-000043f0: 6765 0700 0000 0b51 7363 6943 6f6d 6d61  ge.....QsciComma
-00004400: 6e64 0103 0000 002c 0045 0069 006e 0065  nd.....,.E.i.n.e
-00004410: 006e 0020 0041 0062 0073 0061 0074 007a  .n. .A.b.s.a.t.z
-00004420: 0020 006e 0061 0063 0068 0020 006f 0062  . .n.a.c.h. .o.b
-00004430: 0065 006e 0800 0000 0006 0000 0015 4d6f  .e.n..........Mo
-00004440: 7665 2075 7020 6f6e 6520 7061 7261 6772  ve up one paragr
-00004450: 6170 6807 0000 000b 5173 6369 436f 6d6d  aph.....QsciComm
-00004460: 616e 6401 0300 0000 1000 4500 6900 6e00  and.......E.i.n.
-00004470: 6600 fc00 6700 6500 6e08 0000 0000 0600  f...g.e.n.......
-00004480: 0000 0550 6173 7465 0700 0000 0b51 7363  ...Paste.....Qsc
-00004490: 6943 6f6d 6d61 6e64 0103 0000 0034 004c  iCommand.....4.L
-000044a0: 0065 0074 007a 0074 0065 006e 0020 0042  .e.t.z.t.e.n. .B
-000044b0: 0065 0066 0065 0068 006c 0020 0077 0069  .e.f.e.h.l. .w.i
-000044c0: 0065 0064 0065 0072 0068 006f 006c 0065  .e.d.e.r.h.o.l.e
-000044d0: 006e 0800 0000 0006 0000 0011 5265 646f  .n..........Redo
-000044e0: 206c 6173 7420 636f 6d6d 616e 6407 0000   last command...
-000044f0: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00004500: 0000 3200 5a00 7500 6d00 2000 4400 6f00  ..2.Z.u.m. .D.o.
-00004510: 6b00 7500 6d00 6500 6e00 7400 6500 6e00  k.u.m.e.n.t.e.n.
-00004520: 6500 6e00 6400 6500 2000 7200 6f00 6c00  e.n.d.e. .r.o.l.
-00004530: 6c00 6500 6e08 0000 0000 0600 0000 1953  l.e.n..........S
-00004540: 6372 6f6c 6c20 746f 2065 6e64 206f 6620  croll to end of 
-00004550: 646f 6375 6d65 6e74 0700 0000 0b51 7363  document.....Qsc
-00004560: 6943 6f6d 6d61 6e64 0103 0000 0036 005a  iCommand.....6.Z
-00004570: 0075 006d 0020 0044 006f 006b 0075 006d  .u.m. .D.o.k.u.m
-00004580: 0065 006e 0074 0065 006e 0061 006e 0066  .e.n.t.e.n.a.n.f
-00004590: 0061 006e 0067 0020 0072 006f 006c 006c  .a.n.g. .r.o.l.l
-000045a0: 0065 006e 0800 0000 0006 0000 001b 5363  .e.n..........Sc
-000045b0: 726f 6c6c 2074 6f20 7374 6172 7420 6f66  roll to start of
-000045c0: 2064 6f63 756d 656e 7407 0000 000b 5173   document.....Qs
-000045d0: 6369 436f 6d6d 616e 6401 0300 0000 6000  ciCommand.....`.
-000045e0: 5600 6500 7200 7400 6900 6300 6100 6c00  V.e.r.t.i.c.a.l.
-000045f0: 2000 7200 6f00 6c00 6c00 6500 6e00 2c00   .r.o.l.l.e.n.,.
-00004600: 2000 7500 6d00 2000 6100 6b00 7400 7500   .u.m. .a.k.t.u.
-00004610: 6500 6c00 6c00 6500 2000 5a00 6500 6900  e.l.l.e. .Z.e.i.
-00004620: 6c00 6500 2000 7a00 7500 2000 7a00 6500  l.e. .z.u. .z.e.
-00004630: 6e00 7400 7200 6900 6500 7200 6500 6e08  n.t.r.i.e.r.e.n.
-00004640: 0000 0000 0600 0000 2853 6372 6f6c 6c20  ........(Scroll 
-00004650: 7665 7274 6963 616c 6c79 2074 6f20 6365  vertically to ce
-00004660: 6e74 7265 2063 7572 7265 6e74 206c 696e  ntre current lin
-00004670: 6507 0000 000b 5173 6369 436f 6d6d 616e  e.....QsciComman
-00004680: 6401 0300 0000 3800 4500 6900 6e00 6500  d.....8.E.i.n.e.
-00004690: 2000 5a00 6500 6900 6c00 6500 2000 6e00   .Z.e.i.l.e. .n.
-000046a0: 6100 6300 6800 2000 7500 6e00 7400 6500  a.c.h. .u.n.t.e.
-000046b0: 6e00 2000 7200 6f00 6c00 6c00 6500 6e08  n. .r.o.l.l.e.n.
-000046c0: 0000 0000 0600 0000 1953 6372 6f6c 6c20  .........Scroll 
-000046d0: 7669 6577 2064 6f77 6e20 6f6e 6520 6c69  view down one li
-000046e0: 6e65 0700 0000 0b51 7363 6943 6f6d 6d61  ne.....QsciComma
-000046f0: 6e64 0103 0000 0036 0045 0069 006e 0065  nd.....6.E.i.n.e
-00004700: 0020 005a 0065 0069 006c 0065 0020 006e  . .Z.e.i.l.e. .n
-00004710: 0061 0063 0068 0020 006f 0062 0065 006e  .a.c.h. .o.b.e.n
-00004720: 0020 0072 006f 006c 006c 0065 006e 0800  . .r.o.l.l.e.n..
-00004730: 0000 0006 0000 0017 5363 726f 6c6c 2076  ........Scroll v
-00004740: 6965 7720 7570 206f 6e65 206c 696e 6507  iew up one line.
-00004750: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
-00004760: 0300 0000 1c00 4100 6c00 6c00 6500 2000  ......A.l.l.e. .
-00004770: 6100 7500 7300 7700 e400 6800 6c00 6500  a.u.s.w...h.l.e.
-00004780: 6e08 0000 0000 0600 0000 0a53 656c 6563  n..........Selec
-00004790: 7420 616c 6c07 0000 000b 5173 6369 436f  t all.....QsciCo
-000047a0: 6d6d 616e 6401 0300 0000 6c00 4100 7500  mmand.....l.A.u.
-000047b0: 7300 7700 6100 6800 6c00 2000 2200 7300  s.w.a.h.l. .".s.
-000047c0: 7400 6f00 7400 7400 6500 7200 6e00 6400  t.o.t.t.e.r.n.d.
-000047d0: 2200 2000 7500 6d00 2000 6500 6900 6e00  ". .u.m. .e.i.n.
-000047e0: 6500 2000 5300 6500 6900 7400 6500 2000  e. .S.e.i.t.e. .
-000047f0: 6e00 6100 6300 6800 2000 7500 6e00 7400  n.a.c.h. .u.n.t.
-00004800: 6500 6e00 2000 6500 7200 7700 6500 6900  e.n. .e.r.w.e.i.
-00004810: 7400 6500 7200 6e08 0000 0000 0600 0000  t.e.r.n.........
-00004820: 2853 7475 7474 6572 6564 2065 7874 656e  (Stuttered exten
-00004830: 6420 7365 6c65 6374 696f 6e20 646f 776e  d selection down
-00004840: 206f 6e65 2070 6167 6507 0000 000b 5173   one page.....Qs
-00004850: 6369 436f 6d6d 616e 6401 0300 0000 6a00  ciCommand.....j.
-00004860: 4100 7500 7300 7700 6100 6800 6c00 2000  A.u.s.w.a.h.l. .
-00004870: 2200 7300 7400 6f00 7400 7400 6500 7200  ".s.t.o.t.t.e.r.
-00004880: 6e00 6400 2200 2000 7500 6d00 2000 6500  n.d.". .u.m. .e.
-00004890: 6900 6e00 6500 2000 5300 6500 6900 7400  i.n.e. .S.e.i.t.
-000048a0: 6500 2000 6e00 6100 6300 6800 2000 6f00  e. .n.a.c.h. .o.
-000048b0: 6200 6500 6e00 2000 6500 7200 7700 6500  b.e.n. .e.r.w.e.
-000048c0: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
-000048d0: 0000 2653 7475 7474 6572 6564 2065 7874  ..&Stuttered ext
-000048e0: 656e 6420 7365 6c65 6374 696f 6e20 7570  end selection up
-000048f0: 206f 6e65 2070 6167 6507 0000 000b 5173   one page.....Qs
-00004900: 6369 436f 6d6d 616e 6401 0300 0000 4800  ciCommand.....H.
-00004910: 2200 5300 7400 6f00 7400 7400 6500 7200  ".S.t.o.t.t.e.r.
-00004920: 6e00 6400 2200 2000 7500 6d00 2000 6500  n.d.". .u.m. .e.
-00004930: 6900 6e00 6500 2000 5300 6500 6900 7400  i.n.e. .S.e.i.t.
-00004940: 6500 2000 6e00 6100 6300 6800 2000 7500  e. .n.a.c.h. .u.
-00004950: 6e00 7400 6500 6e08 0000 0000 0600 0000  n.t.e.n.........
-00004960: 1c53 7475 7474 6572 6564 206d 6f76 6520  .Stuttered move 
-00004970: 646f 776e 206f 6e65 2070 6167 6507 0000  down one page...
-00004980: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00004990: 0000 4600 2200 5300 7400 6f00 7400 7400  ..F.".S.t.o.t.t.
-000049a0: 6500 7200 6e00 6400 2200 2000 7500 6d00  e.r.n.d.". .u.m.
-000049b0: 2000 6500 6900 6e00 6500 2000 5300 6500   .e.i.n.e. .S.e.
-000049c0: 6900 7400 6500 2000 6e00 6100 6300 6800  i.t.e. .n.a.c.h.
-000049d0: 2000 6f00 6200 6500 6e08 0000 0000 0600   .o.b.e.n.......
-000049e0: 0000 1a53 7475 7474 6572 6564 206d 6f76  ...Stuttered mov
-000049f0: 6520 7570 206f 6e65 2070 6167 6507 0000  e up one page...
-00004a00: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00004a10: 0000 4200 4500 6900 6e00 6600 fc00 6700  ..B.E.i.n.f...g.
-00004a20: 6500 6e00 2f00 dc00 6200 6500 7200 7300  e.n./...b.e.r.s.
-00004a30: 6300 6800 7200 6500 6900 6200 6500 6e00  c.h.r.e.i.b.e.n.
-00004a40: 2000 7500 6d00 7300 6300 6800 6100 6c00   .u.m.s.c.h.a.l.
-00004a50: 7400 6500 6e08 0000 0000 0600 0000 1654  t.e.n..........T
-00004a60: 6f67 676c 6520 696e 7365 7274 2f6f 7665  oggle insert/ove
-00004a70: 7274 7970 6507 0000 000b 5173 6369 436f  rtype.....QsciCo
-00004a80: 6d6d 616e 6401 0300 0000 4a00 4100 6b00  mmand.....J.A.k.
-00004a90: 7400 7500 6500 6c00 6c00 6500 2000 7500  t.u.e.l.l.e. .u.
-00004aa0: 6e00 6400 2000 7600 6f00 7200 6800 6500  n.d. .v.o.r.h.e.
-00004ab0: 7200 6900 6700 6500 2000 5a00 6500 6900  r.i.g.e. .Z.e.i.
-00004ac0: 6c00 6500 2000 7400 6100 7500 7300 6300  l.e. .t.a.u.s.c.
-00004ad0: 6800 6500 6e08 0000 0000 0600 0000 2454  h.e.n.........$T
-00004ae0: 7261 6e73 706f 7365 2063 7572 7265 6e74  ranspose current
-00004af0: 2061 6e64 2070 7265 7669 6f75 7320 6c69   and previous li
-00004b00: 6e65 7307 0000 000b 5173 6369 436f 6d6d  nes.....QsciComm
-00004b10: 616e 6401 0300 0000 4000 4c00 6500 7400  and.....@.L.e.t.
-00004b20: 7a00 7400 6500 6e00 2000 4200 6500 6600  z.t.e.n. .B.e.f.
-00004b30: 6500 6800 6c00 2000 7200 fc00 6300 6b00  e.h.l. .r...c.k.
-00004b40: 6700 e400 6e00 6700 6900 6700 2000 6d00  g...n.g.i.g. .m.
-00004b50: 6100 6300 6800 6500 6e08 0000 0000 0600  a.c.h.e.n.......
-00004b60: 0000 1155 6e64 6f20 6c61 7374 2063 6f6d  ...Undo last com
-00004b70: 6d61 6e64 0700 0000 0b51 7363 6943 6f6d  mand.....QsciCom
-00004b80: 6d61 6e64 0103 0000 0014 0056 0065 0072  mand.......V.e.r
-00004b90: 0067 0072 00f6 00df 0065 0072 006e 0800  .g.r.....e.r.n..
-00004ba0: 0000 0006 0000 0007 5a6f 6f6d 2069 6e07  ........Zoom in.
-00004bb0: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
-00004bc0: 0300 0000 1600 5600 6500 7200 6b00 6c00  ......V.e.r.k.l.
-00004bd0: 6500 6900 6e00 6500 7200 6e08 0000 0000  e.i.n.e.r.n.....
-00004be0: 0600 0000 085a 6f6f 6d20 6f75 7407 0000  .....Zoom out...
-00004bf0: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
-00004c00: 0000 1c00 4200 6c00 6f00 6300 6b00 6b00  ....B.l.o.c.k.k.
-00004c10: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-00004c20: 0000 0000 0600 0000 0d42 6c6f 636b 2063  .........Block c
-00004c30: 6f6d 6d65 6e74 0700 0000 0c51 7363 694c  omment.....QsciL
-00004c40: 6578 6572 4156 5301 0300 0000 2000 4300  exerAVS..... .C.
-00004c50: 6c00 6900 7000 2000 4500 6900 6700 6500  l.i.p. .E.i.g.e.
-00004c60: 6e00 7300 6300 6800 6100 6600 7408 0000  n.s.c.h.a.f.t...
-00004c70: 0000 0600 0000 0d43 6c69 7020 7072 6f70  .......Clip prop
-00004c80: 6572 7479 0700 0000 0c51 7363 694c 6578  erty.....QsciLex
-00004c90: 6572 4156 5301 0300 0000 1000 5300 7400  erAVS.......S.t.
-00004ca0: 6100 6e00 6400 6100 7200 6408 0000 0000  a.n.d.a.r.d.....
-00004cb0: 0600 0000 0744 6566 6175 6c74 0700 0000  .....Default....
-00004cc0: 0c51 7363 694c 6578 6572 4156 5301 0300  .QsciLexerAVS...
-00004cd0: 0000 4200 5a00 6500 6900 6300 6800 6500  ..B.Z.e.i.c.h.e.
-00004ce0: 6e00 6b00 6500 7400 7400 6500 2000 6900  n.k.e.t.t.e. .i.
-00004cf0: 6e00 2000 4100 6e00 6600 fc00 6800 7200  n. .A.n.f...h.r.
-00004d00: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
-00004d10: 6800 6500 6e08 0000 0000 0600 0000 1444  h.e.n..........D
-00004d20: 6f75 626c 652d 7175 6f74 6564 2073 7472  ouble-quoted str
-00004d30: 696e 6707 0000 000c 5173 6369 4c65 7865  ing.....QsciLexe
-00004d40: 7241 5653 0103 0000 000c 0046 0069 006c  rAVS.......F.i.l
-00004d50: 0074 0065 0072 0800 0000 0006 0000 0006  .t.e.r..........
-00004d60: 4669 6c74 6572 0700 0000 0c51 7363 694c  Filter.....QsciL
-00004d70: 6578 6572 4156 5301 0300 0000 1000 4600  exerAVS.......F.
-00004d80: 7500 6e00 6b00 7400 6900 6f00 6e08 0000  u.n.k.t.i.o.n...
-00004d90: 0000 0600 0000 0846 756e 6374 696f 6e07  .......Function.
-00004da0: 0000 000c 5173 6369 4c65 7865 7241 5653  ....QsciLexerAVS
-00004db0: 0103 0000 0014 0042 0065 007a 0065 0069  .......B.e.z.e.i
-00004dc0: 0063 0068 006e 0065 0072 0800 0000 0006  .c.h.n.e.r......
-00004dd0: 0000 000a 4964 656e 7469 6669 6572 0700  ....Identifier..
-00004de0: 0000 0c51 7363 694c 6578 6572 4156 5301  ...QsciLexerAVS.
-00004df0: 0300 0000 1a00 5300 6300 6800 6c00 fc00  ......S.c.h.l...
-00004e00: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
-00004e10: 0000 0000 0600 0000 074b 6579 776f 7264  .........Keyword
-00004e20: 0700 0000 0c51 7363 694c 6578 6572 4156  .....QsciLexerAV
-00004e30: 5301 0300 0000 1e00 5a00 6500 6900 6c00  S.......Z.e.i.l.
-00004e40: 6500 6e00 6b00 6f00 6d00 6d00 6500 6e00  e.n.k.o.m.m.e.n.
-00004e50: 7400 6100 7208 0000 0000 0600 0000 0c4c  t.a.r..........L
-00004e60: 696e 6520 636f 6d6d 656e 7407 0000 000c  ine comment.....
-00004e70: 5173 6369 4c65 7865 7241 5653 0103 0000  QsciLexerAVS....
-00004e80: 003c 0056 0065 0072 0073 0063 0068 0061  .<.V.e.r.s.c.h.a
-00004e90: 0063 0068 0074 0065 006c 0074 0065 0072  .c.h.t.e.l.t.e.r
-00004ea0: 0020 0042 006c 006f 0063 006b 006b 006f  . .B.l.o.c.k.k.o
-00004eb0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-00004ec0: 0000 0006 0000 0014 4e65 7374 6564 2062  ........Nested b
-00004ed0: 6c6f 636b 2063 6f6d 6d65 6e74 0700 0000  lock comment....
-00004ee0: 0c51 7363 694c 6578 6572 4156 5301 0300  .QsciLexerAVS...
-00004ef0: 0000 0800 5a00 6100 6800 6c08 0000 0000  ....Z.a.h.l.....
-00004f00: 0600 0000 064e 756d 6265 7207 0000 000c  .....Number.....
-00004f10: 5173 6369 4c65 7865 7241 5653 0103 0000  QsciLexerAVS....
-00004f20: 0010 004f 0070 0065 0072 0061 0074 006f  ...O.p.e.r.a.t.o
-00004f30: 0072 0800 0000 0006 0000 0008 4f70 6572  .r..........Oper
-00004f40: 6174 6f72 0700 0000 0c51 7363 694c 6578  ator.....QsciLex
-00004f50: 6572 4156 5301 0300 0000 0c00 5000 6c00  erAVS.......P.l.
-00004f60: 7500 6700 6900 6e08 0000 0000 0600 0000  u.g.i.n.........
-00004f70: 0650 6c75 6769 6e07 0000 000c 5173 6369  .Plugin.....Qsci
-00004f80: 4c65 7865 7241 5653 0103 0000 0058 005a  LexerAVS.....X.Z
-00004f90: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-00004fa0: 0074 0074 0065 0020 0069 006e 0020 0064  .t.t.e. .i.n. .d
-00004fb0: 0072 0065 0069 0066 0061 0063 0068 0065  .r.e.i.f.a.c.h.e
-00004fc0: 006e 0020 0041 006e 0066 00fc 0068 0072  .n. .A.n.f...h.r
-00004fd0: 0075 006e 0067 0073 007a 0065 0069 0063  .u.n.g.s.z.e.i.c
-00004fe0: 0068 0065 006e 0800 0000 0006 0000 001b  .h.e.n..........
-00004ff0: 5472 6970 6c65 2064 6f75 626c 652d 7175  Triple double-qu
-00005000: 6f74 6564 2073 7472 696e 6707 0000 000c  oted string.....
-00005010: 5173 6369 4c65 7865 7241 5653 0103 0000  QsciLexerAVS....
-00005020: 0020 004e 0075 0074 007a 0065 0072 0020  . .N.u.t.z.e.r. 
-00005030: 0064 0065 0066 0069 006e 0069 0065 0072  .d.e.f.i.n.i.e.r
-00005040: 0074 0800 0000 0006 0000 000c 5573 6572  .t..........User
-00005050: 2064 6566 696e 6564 0700 0000 0c51 7363   defined.....Qsc
-00005060: 694c 6578 6572 4156 5301 0300 0000 1200  iLexerAVS.......
-00005070: 4200 6100 6300 6b00 7400 6900 6300 6b00  B.a.c.k.t.i.c.k.
-00005080: 7308 0000 0000 0600 0000 0942 6163 6b74  s..........Backt
-00005090: 6963 6b73 0700 0000 0d51 7363 694c 6578  icks.....QsciLex
-000050a0: 6572 4261 7368 0103 0000 0012 004b 006f  erBash.......K.o
-000050b0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-000050c0: 0000 0006 0000 0007 436f 6d6d 656e 7407  ........Comment.
-000050d0: 0000 000d 5173 6369 4c65 7865 7242 6173  ....QsciLexerBas
-000050e0: 6801 0300 0000 1000 5300 7400 6100 6e00  h.......S.t.a.n.
-000050f0: 6400 6100 7200 6408 0000 0000 0600 0000  d.a.r.d.........
-00005100: 0744 6566 6175 6c74 0700 0000 0d51 7363  .Default.....Qsc
-00005110: 694c 6578 6572 4261 7368 0103 0000 0042  iLexerBash.....B
-00005120: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-00005130: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
-00005140: 0041 006e 0066 00fc 0068 0072 0075 006e  .A.n.f...h.r.u.n
-00005150: 0067 0073 007a 0065 0069 0063 0068 0065  .g.s.z.e.i.c.h.e
-00005160: 006e 0800 0000 0006 0000 0014 446f 7562  .n..........Doub
-00005170: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
-00005180: 0700 0000 0d51 7363 694c 6578 6572 4261  .....QsciLexerBa
-00005190: 7368 0103 0000 000c 0046 0065 0068 006c  sh.......F.e.h.l
-000051a0: 0065 0072 0800 0000 0006 0000 0005 4572  .e.r..........Er
-000051b0: 726f 7207 0000 000d 5173 6369 4c65 7865  ror.....QsciLexe
-000051c0: 7242 6173 6801 0300 0000 2e00 4800 6500  rBash.......H.e.
-000051d0: 7200 6500 2000 4400 6f00 6b00 7500 6d00  r.e. .D.o.k.u.m.
-000051e0: 6500 6e00 7400 2d00 4200 6500 6700 7200  e.n.t.-.B.e.g.r.
-000051f0: 6500 6e00 7a00 6500 7208 0000 0000 0600  e.n.z.e.r.......
-00005200: 0000 1748 6572 6520 646f 6375 6d65 6e74  ...Here document
-00005210: 2064 656c 696d 6974 6572 0700 0000 0d51   delimiter.....Q
-00005220: 7363 694c 6578 6572 4261 7368 0103 0000  sciLexerBash....
-00005230: 0014 0042 0065 007a 0065 0069 0063 0068  ...B.e.z.e.i.c.h
-00005240: 006e 0065 0072 0800 0000 0006 0000 000a  .n.e.r..........
-00005250: 4964 656e 7469 6669 6572 0700 0000 0d51  Identifier.....Q
-00005260: 7363 694c 6578 6572 4261 7368 0103 0000  sciLexerBash....
-00005270: 001a 0053 0063 0068 006c 00fc 0073 0073  ...S.c.h.l...s.s
-00005280: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
-00005290: 0006 0000 0007 4b65 7977 6f72 6407 0000  ......Keyword...
-000052a0: 000d 5173 6369 4c65 7865 7242 6173 6801  ..QsciLexerBash.
-000052b0: 0300 0000 0800 5a00 6100 6800 6c08 0000  ......Z.a.h.l...
-000052c0: 0000 0600 0000 064e 756d 6265 7207 0000  .......Number...
-000052d0: 000d 5173 6369 4c65 7865 7242 6173 6801  ..QsciLexerBash.
-000052e0: 0300 0000 1000 4f00 7000 6500 7200 6100  ......O.p.e.r.a.
-000052f0: 7400 6f00 7208 0000 0000 0600 0000 084f  t.o.r..........O
-00005300: 7065 7261 746f 7207 0000 000d 5173 6369  perator.....Qsci
-00005310: 4c65 7865 7242 6173 6801 0300 0000 2800  LexerBash.....(.
-00005320: 5000 6100 7200 6100 6d00 6500 7400 6500  P.a.r.a.m.e.t.e.
-00005330: 7200 6500 7200 7700 6500 6900 7400 6500  r.e.r.w.e.i.t.e.
-00005340: 7200 7500 6e00 6708 0000 0000 0600 0000  r.u.n.g.........
-00005350: 1350 6172 616d 6574 6572 2065 7870 616e  .Parameter expan
-00005360: 7369 6f6e 0700 0000 0d51 7363 694c 6578  sion.....QsciLex
-00005370: 6572 4261 7368 0103 0000 000c 0053 006b  erBash.......S.k
-00005380: 0061 006c 0061 0072 0800 0000 0006 0000  .a.l.a.r........
-00005390: 0006 5363 616c 6172 0700 0000 0d51 7363  ..Scalar.....Qsc
-000053a0: 694c 6578 6572 4261 7368 0103 0000 0038  iLexerBash.....8
-000053b0: 0048 0065 0072 0065 0020 0044 006f 006b  .H.e.r.e. .D.o.k
-000053c0: 0075 006d 0065 006e 0074 0020 0069 006e  .u.m.e.n.t. .i.n
-000053d0: 0020 0048 006f 0063 0068 006b 006f 006d  . .H.o.c.h.k.o.m
-000053e0: 006d 0061 0074 0061 0800 0000 0006 0000  .m.a.t.a........
-000053f0: 001b 5369 6e67 6c65 2d71 756f 7465 6420  ..Single-quoted 
-00005400: 6865 7265 2064 6f63 756d 656e 7407 0000  here document...
-00005410: 000d 5173 6369 4c65 7865 7242 6173 6801  ..QsciLexerBash.
-00005420: 0300 0000 3600 5a00 6500 6900 6300 6800  ....6.Z.e.i.c.h.
-00005430: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
-00005440: 6900 6e00 2000 4800 6f00 6300 6800 6b00  i.n. .H.o.c.h.k.
-00005450: 6f00 6d00 6d00 6100 7400 6108 0000 0000  o.m.m.a.t.a.....
-00005460: 0600 0000 1453 696e 676c 652d 7175 6f74  .....Single-quot
-00005470: 6564 2073 7472 696e 6707 0000 000d 5173  ed string.....Qs
-00005480: 6369 4c65 7865 7242 6173 6801 0300 0000  ciLexerBash.....
-00005490: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
-000054a0: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
-000054b0: 6d65 6e74 0700 0000 0e51 7363 694c 6578  ment.....QsciLex
-000054c0: 6572 4261 7463 6801 0300 0000 1000 5300  erBatch.......S.
-000054d0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
-000054e0: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
-000054f0: 0000 0e51 7363 694c 6578 6572 4261 7463  ...QsciLexerBatc
-00005500: 6801 0300 0000 1e00 4500 7800 7400 6500  h.......E.x.t.e.
-00005510: 7200 6e00 6500 7200 2000 4200 6500 6600  r.n.e.r. .B.e.f.
-00005520: 6500 6800 6c08 0000 0000 0600 0000 1045  e.h.l..........E
-00005530: 7874 6572 6e61 6c20 636f 6d6d 616e 6407  xternal command.
-00005540: 0000 000e 5173 6369 4c65 7865 7242 6174  ....QsciLexerBat
-00005550: 6368 0103 0000 0034 0022 0042 0065 0066  ch.....4.".B.e.f
-00005560: 0065 0068 006c 0020 0076 0065 0072 0062  .e.h.l. .v.e.r.b
-00005570: 0065 0072 0067 0065 006e 0022 0020 005a  .e.r.g.e.n.". .Z
-00005580: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
-00005590: 0006 0000 0016 4869 6465 2063 6f6d 6d61  ......Hide comma
-000055a0: 6e64 2063 6861 7261 6374 6572 0700 0000  nd character....
-000055b0: 0e51 7363 694c 6578 6572 4261 7463 6801  .QsciLexerBatch.
-000055c0: 0300 0000 1a00 5300 6300 6800 6c00 fc00  ......S.c.h.l...
-000055d0: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
-000055e0: 0000 0000 0600 0000 074b 6579 776f 7264  .........Keyword
-000055f0: 0700 0000 0e51 7363 694c 6578 6572 4261  .....QsciLexerBa
-00005600: 7463 6801 0300 0000 0a00 4d00 6100 7200  tch.......M.a.r.
-00005610: 6b00 6508 0000 0000 0600 0000 054c 6162  k.e..........Lab
-00005620: 656c 0700 0000 0e51 7363 694c 6578 6572  el.....QsciLexer
-00005630: 4261 7463 6801 0300 0000 1000 4f00 7000  Batch.......O.p.
-00005640: 6500 7200 6100 7400 6f00 7208 0000 0000  e.r.a.t.o.r.....
-00005650: 0600 0000 084f 7065 7261 746f 7207 0000  .....Operator...
-00005660: 000e 5173 6369 4c65 7865 7242 6174 6368  ..QsciLexerBatch
-00005670: 0103 0000 0010 0056 0061 0072 0069 0061  .......V.a.r.i.a
-00005680: 0062 006c 0065 0800 0000 0006 0000 0008  .b.l.e..........
-00005690: 5661 7269 6162 6c65 0700 0000 0e51 7363  Variable.....Qsc
-000056a0: 694c 6578 6572 4261 7463 6801 0300 0000  iLexerBatch.....
-000056b0: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
-000056c0: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
-000056d0: 6d65 6e74 0700 0000 0e51 7363 694c 6578  ment.....QsciLex
-000056e0: 6572 434d 616b 6501 0300 0000 1000 5300  erCMake.......S.
-000056f0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
-00005700: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
-00005710: 0000 0e51 7363 694c 6578 6572 434d 616b  ...QsciLexerCMak
-00005720: 6501 0300 0000 1a00 4600 4f00 5200 4500  e.......F.O.R.E.
-00005730: 4100 4300 4800 2000 4200 6c00 6f00 6300  A.C.H. .B.l.o.c.
-00005740: 6b08 0000 0000 0600 0000 0d46 4f52 4541  k..........FOREA
-00005750: 4348 2062 6c6f 636b 0700 0000 0e51 7363  CH block.....Qsc
-00005760: 694c 6578 6572 434d 616b 6501 0300 0000  iLexerCMake.....
-00005770: 1000 4600 7500 6e00 6b00 7400 6900 6f00  ..F.u.n.k.t.i.o.
-00005780: 6e08 0000 0000 0600 0000 0846 756e 6374  n..........Funct
-00005790: 696f 6e07 0000 000e 5173 6369 4c65 7865  ion.....QsciLexe
-000057a0: 7243 4d61 6b65 0103 0000 0010 0049 0046  rCMake.......I.F
-000057b0: 0020 0042 006c 006f 0063 006b 0800 0000  . .B.l.o.c.k....
-000057c0: 0006 0000 0008 4946 2062 6c6f 636b 0700  ......IF block..
-000057d0: 0000 0e51 7363 694c 6578 6572 434d 616b  ...QsciLexerCMak
-000057e0: 6501 0300 0000 0a00 4d00 6100 7200 6b00  e.......M.a.r.k.
-000057f0: 6508 0000 0000 0600 0000 054c 6162 656c  e..........Label
-00005800: 0700 0000 0e51 7363 694c 6578 6572 434d  .....QsciLexerCM
-00005810: 616b 6501 0300 0000 3800 4c00 6900 6e00  ake.....8.L.i.n.
-00005820: 6b00 7300 2000 7100 7500 6f00 7400 6900  k.s. .q.u.o.t.i.
-00005830: 6500 7200 7400 6500 2000 5a00 6500 6900  e.r.t.e. .Z.e.i.
-00005840: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00005850: 6508 0000 0000 0600 0000 124c 6566 7420  e..........Left 
-00005860: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
-00005870: 000e 5173 6369 4c65 7865 7243 4d61 6b65  ..QsciLexerCMake
-00005880: 0103 0000 0016 004d 0041 0043 0052 004f  .......M.A.C.R.O
-00005890: 0020 0042 006c 006f 0063 006b 0800 0000  . .B.l.o.c.k....
-000058a0: 0006 0000 000b 4d41 4352 4f20 626c 6f63  ......MACRO bloc
-000058b0: 6b07 0000 000e 5173 6369 4c65 7865 7243  k.....QsciLexerC
-000058c0: 4d61 6b65 0103 0000 0008 005a 0061 0068  Make.......Z.a.h
-000058d0: 006c 0800 0000 0006 0000 0006 4e75 6d62  .l..........Numb
-000058e0: 6572 0700 0000 0e51 7363 694c 6578 6572  er.....QsciLexer
-000058f0: 434d 616b 6501 0300 0000 3a00 5200 6500  CMake.....:.R.e.
-00005900: 6300 6800 7400 7300 2000 7100 7500 6f00  c.h.t.s. .q.u.o.
-00005910: 7400 6900 6500 7200 7400 6500 2000 5a00  t.i.e.r.t.e. .Z.
-00005920: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-00005930: 7400 7400 6508 0000 0000 0600 0000 1352  t.t.e..........R
-00005940: 6967 6874 2071 756f 7465 6420 7374 7269  ight quoted stri
-00005950: 6e67 0700 0000 0e51 7363 694c 6578 6572  ng.....QsciLexer
-00005960: 434d 616b 6501 0300 0000 1800 5a00 6500  CMake.......Z.e.
-00005970: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
-00005980: 7400 6508 0000 0000 0600 0000 0653 7472  t.e..........Str
-00005990: 696e 6707 0000 000e 5173 6369 4c65 7865  ing.....QsciLexe
-000059a0: 7243 4d61 6b65 0103 0000 0020 004e 0075  rCMake..... .N.u
-000059b0: 0074 007a 0065 0072 0020 0064 0065 0066  .t.z.e.r. .d.e.f
-000059c0: 0069 006e 0069 0065 0072 0074 0800 0000  .i.n.i.e.r.t....
-000059d0: 0006 0000 000c 5573 6572 2064 6566 696e  ......User defin
-000059e0: 6564 0700 0000 0e51 7363 694c 6578 6572  ed.....QsciLexer
-000059f0: 434d 616b 6501 0300 0000 1000 5600 6100  CMake.......V.a.
-00005a00: 7200 6900 6100 6200 6c00 6508 0000 0000  r.i.a.b.l.e.....
-00005a10: 0600 0000 0856 6172 6961 626c 6507 0000  .....Variable...
-00005a20: 000e 5173 6369 4c65 7865 7243 4d61 6b65  ..QsciLexerCMake
-00005a30: 0103 0000 003c 0056 0061 0072 0069 0061  .....<.V.a.r.i.a
-00005a40: 0062 006c 0065 0020 0069 006e 0020 0065  .b.l.e. .i.n. .e
-00005a50: 0069 006e 0065 0072 0020 005a 0065 0069  .i.n.e.r. .Z.e.i
-00005a60: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00005a70: 0065 0800 0000 0006 0000 0018 5661 7269  .e..........Vari
-00005a80: 6162 6c65 2077 6974 6869 6e20 6120 7374  able within a st
-00005a90: 7269 6e67 0700 0000 0e51 7363 694c 6578  ring.....QsciLex
-00005aa0: 6572 434d 616b 6501 0300 0000 1600 5700  erCMake.......W.
-00005ab0: 4800 4900 4c00 4500 2000 4200 6c00 6f00  H.I.L.E. .B.l.o.
-00005ac0: 6300 6b08 0000 0000 0600 0000 0b57 4849  c.k..........WHI
-00005ad0: 4c45 2062 6c6f 636b 0700 0000 0e51 7363  LE block.....Qsc
-00005ae0: 694c 6578 6572 434d 616b 6501 0300 0000  iLexerCMake.....
-00005af0: 1600 4300 2000 4b00 6f00 6d00 6d00 6500  ..C. .K.o.m.m.e.
-00005b00: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
-00005b10: 0943 2063 6f6d 6d65 6e74 0700 0000 0c51  .C comment.....Q
-00005b20: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
-00005b30: 4000 5500 6e00 6900 6e00 7400 6500 7200  @.U.n.i.n.t.e.r.
-00005b40: 7000 7200 6500 7400 6900 6500 7200 7400  p.r.e.t.i.e.r.t.
-00005b50: 6500 2000 4300 2300 2000 5a00 6500 6900  e. .C.#. .Z.e.i.
-00005b60: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00005b70: 6508 0000 0000 0600 0000 1243 2320 7665  e..........C# ve
-00005b80: 7262 6174 696d 2073 7472 696e 6707 0000  rbatim string...
-00005b90: 000c 5173 6369 4c65 7865 7243 5050 0103  ..QsciLexerCPP..
-00005ba0: 0000 001a 0043 002b 002b 0020 004b 006f  .....C.+.+. .K.o
-00005bb0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-00005bc0: 0000 0006 0000 000b 432b 2b20 636f 6d6d  ........C++ comm
-00005bd0: 656e 7407 0000 000c 5173 6369 4c65 7865  ent.....QsciLexe
-00005be0: 7243 5050 0103 0000 002a 0052 006f 0068  rCPP.....*.R.o.h
-00005bf0: 0065 0020 0043 002b 002b 0020 005a 0065  .e. .C.+.+. .Z.e
-00005c00: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-00005c10: 0074 0065 0800 0000 0006 0000 000e 432b  .t.e..........C+
-00005c20: 2b20 7261 7720 7374 7269 6e67 0700 0000  + raw string....
-00005c30: 0c51 7363 694c 6578 6572 4350 5001 0300  .QsciLexerCPP...
-00005c40: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
-00005c50: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
-00005c60: 6175 6c74 0700 0000 0c51 7363 694c 6578  ault.....QsciLex
-00005c70: 6572 4350 5001 0300 0000 4200 5a00 6500  erCPP.....B.Z.e.
-00005c80: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
-00005c90: 7400 6500 2000 6900 6e00 2000 4100 6e00  t.e. .i.n. .A.n.
-00005ca0: 6600 fc00 6800 7200 7500 6e00 6700 7300  f...h.r.u.n.g.s.
-00005cb0: 7a00 6500 6900 6300 6800 6500 6e08 0000  z.e.i.c.h.e.n...
-00005cc0: 0000 0600 0000 1444 6f75 626c 652d 7175  .......Double-qu
-00005cd0: 6f74 6564 2073 7472 696e 6707 0000 000c  oted string.....
-00005ce0: 5173 6369 4c65 7865 7243 5050 0103 0000  QsciLexerCPP....
-00005cf0: 001c 0045 0073 0063 0061 0070 0065 002d  ...E.s.c.a.p.e.-
-00005d00: 0053 0065 0071 0075 0065 006e 007a 0800  .S.e.q.u.e.n.z..
-00005d10: 0000 0006 0000 000f 4573 6361 7065 2073  ........Escape s
-00005d20: 6571 7565 6e63 6507 0000 000c 5173 6369  equence.....Qsci
-00005d30: 4c65 7865 7243 5050 0103 0000 0046 0047  LexerCPP.....F.G
-00005d40: 006c 006f 0062 0061 006c 0065 0020 004b  .l.o.b.a.l.e. .K
-00005d50: 006c 0061 0073 0073 0065 006e 0020 0075  .l.a.s.s.e.n. .u
-00005d60: 006e 0064 0020 0054 0079 0070 0064 0065  .n.d. .T.y.p.d.e
-00005d70: 0066 0069 006e 0069 0074 0069 006f 006e  .f.i.n.i.t.i.o.n
-00005d80: 0065 006e 0800 0000 0006 0000 001b 476c  .e.n..........Gl
-00005d90: 6f62 616c 2063 6c61 7373 6573 2061 6e64  obal classes and
-00005da0: 2074 7970 6564 6566 7307 0000 000c 5173   typedefs.....Qs
-00005db0: 6369 4c65 7865 7243 5050 0103 0000 0010  ciLexerCPP......
-00005dc0: 0049 0044 004c 0020 0055 0055 0049 0044  .I.D.L. .U.U.I.D
-00005dd0: 0800 0000 0006 0000 0008 4944 4c20 5555  ..........IDL UU
-00005de0: 4944 0700 0000 0c51 7363 694c 6578 6572  ID.....QsciLexer
-00005df0: 4350 5001 0300 0000 1400 4200 6500 7a00  CPP.......B.e.z.
-00005e00: 6500 6900 6300 6800 6e00 6500 7208 0000  e.i.c.h.n.e.r...
-00005e10: 0000 0600 0000 0a49 6465 6e74 6966 6965  .......Identifie
-00005e20: 7207 0000 000c 5173 6369 4c65 7865 7243  r.....QsciLexerC
-00005e30: 5050 0103 0000 002a 0049 006e 0061 006b  PP.....*.I.n.a.k
-00005e40: 0074 0069 0076 0065 0072 0020 0043 0020  .t.i.v.e.r. .C. 
-00005e50: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
-00005e60: 0072 0800 0000 0006 0000 0012 496e 6163  .r..........Inac
-00005e70: 7469 7665 2043 2063 6f6d 6d65 6e74 0700  tive C comment..
-00005e80: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
-00005e90: 0300 0000 5400 4900 6e00 6100 6b00 7400  ....T.I.n.a.k.t.
-00005ea0: 6900 7600 6500 2c00 2000 5500 6e00 6900  i.v.e.,. .U.n.i.
-00005eb0: 6e00 7400 6500 7200 7000 7200 6500 7400  n.t.e.r.p.r.e.t.
-00005ec0: 6900 6500 7200 7400 6500 2000 4300 2300  i.e.r.t.e. .C.#.
-00005ed0: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
-00005ee0: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
-00005ef0: 0000 1b49 6e61 6374 6976 6520 4323 2076  ...Inactive C# v
-00005f00: 6572 6261 7469 6d20 7374 7269 6e67 0700  erbatim string..
-00005f10: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
-00005f20: 0300 0000 2e00 4900 6e00 6100 6b00 7400  ......I.n.a.k.t.
-00005f30: 6900 7600 6500 7200 2000 4300 2b00 2b00  i.v.e.r. .C.+.+.
-00005f40: 2000 4b00 6f00 6d00 6d00 6500 6e00 7400   .K.o.m.m.e.n.t.
-00005f50: 6100 7208 0000 0000 0600 0000 1449 6e61  a.r..........Ina
-00005f60: 6374 6976 6520 432b 2b20 636f 6d6d 656e  ctive C++ commen
-00005f70: 7407 0000 000c 5173 6369 4c65 7865 7243  t.....QsciLexerC
-00005f80: 5050 0103 0000 003c 0049 006e 0061 006b  PP.....<.I.n.a.k
-00005f90: 0074 0069 0076 0065 0020 0072 006f 0068  .t.i.v.e. .r.o.h
-00005fa0: 0065 0020 0043 002b 002b 0020 005a 0065  .e. .C.+.+. .Z.e
-00005fb0: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-00005fc0: 0074 0065 0800 0000 0006 0000 0017 496e  .t.e..........In
-00005fd0: 6163 7469 7665 2043 2b2b 2072 6177 2073  active C++ raw s
-00005fe0: 7472 696e 6707 0000 000c 5173 6369 4c65  tring.....QsciLe
-00005ff0: 7865 7243 5050 0103 0000 0022 0049 006e  xerCPP.....".I.n
-00006000: 0061 006b 0074 0069 0076 0065 0020 0049  .a.k.t.i.v.e. .I
-00006010: 0044 004c 0020 0055 0055 0049 0044 0800  .D.L. .U.U.I.D..
-00006020: 0000 0006 0000 0011 496e 6163 7469 7665  ........Inactive
-00006030: 2049 444c 2055 5549 4407 0000 000c 5173   IDL UUID.....Qs
-00006040: 6369 4c65 7865 7243 5050 0103 0000 003e  ciLexerCPP.....>
-00006050: 0049 006e 0061 006b 0074 0069 0076 0065  .I.n.a.k.t.i.v.e
-00006060: 0073 0020 004a 0061 0076 0061 0044 006f  .s. .J.a.v.a.D.o
-00006070: 0063 0020 0053 0063 0068 006c 00fc 0073  .c. .S.c.h.l...s
-00006080: 0073 0065 006c 0077 006f 0072 0074 0800  .s.e.l.w.o.r.t..
-00006090: 0000 0006 0000 0018 496e 6163 7469 7665  ........Inactive
-000060a0: 204a 6176 6144 6f63 206b 6579 776f 7264   JavaDoc keyword
-000060b0: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-000060c0: 5001 0300 0000 4a00 4900 6e00 6100 6b00  P.....J.I.n.a.k.
-000060d0: 7400 6900 7600 6500 7200 2000 4a00 6100  t.i.v.e.r. .J.a.
-000060e0: 7600 6100 4400 6f00 6300 2000 5300 6300  v.a.D.o.c. .S.c.
-000060f0: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
-00006100: 6f00 7200 7400 6600 6500 6800 6c00 6500  o.r.t.f.e.h.l.e.
-00006110: 7208 0000 0000 0600 0000 1e49 6e61 6374  r..........Inact
-00006120: 6976 6520 4a61 7661 446f 6320 6b65 7977  ive JavaDoc keyw
-00006130: 6f72 6420 6572 726f 7207 0000 000c 5173  ord error.....Qs
-00006140: 6369 4c65 7865 7243 5050 0103 0000 003a  ciLexerCPP.....:
-00006150: 0049 006e 0061 006b 0074 0069 0076 0065  .I.n.a.k.t.i.v.e
-00006160: 0072 0020 004a 0061 0076 0061 0044 006f  .r. .J.a.v.a.D.o
-00006170: 0063 0020 0043 0020 004b 006f 006d 006d  .c. .C. .K.o.m.m
-00006180: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
-00006190: 0000 0020 496e 6163 7469 7665 204a 6176  ... Inactive Jav
-000061a0: 6144 6f63 2073 7479 6c65 2043 2063 6f6d  aDoc style C com
-000061b0: 6d65 6e74 0700 0000 0c51 7363 694c 6578  ment.....QsciLex
-000061c0: 6572 4350 5001 0300 0000 3e00 4900 6e00  erCPP.....>.I.n.
-000061d0: 6100 6b00 7400 6900 7600 6500 7200 2000  a.k.t.i.v.e.r. .
-000061e0: 4a00 6100 7600 6100 4400 6f00 6300 2000  J.a.v.a.D.o.c. .
-000061f0: 4300 2b00 2b00 2000 4b00 6f00 6d00 6d00  C.+.+. .K.o.m.m.
-00006200: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
-00006210: 0000 2249 6e61 6374 6976 6520 4a61 7661  .."Inactive Java
-00006220: 446f 6320 7374 796c 6520 432b 2b20 636f  Doc style C++ co
-00006230: 6d6d 656e 7407 0000 000c 5173 6369 4c65  mment.....QsciLe
-00006240: 7865 7243 5050 0103 0000 004e 0049 006e  xerCPP.....N.I.n
-00006250: 0061 006b 0074 0069 0076 0065 0072 0020  .a.k.t.i.v.e.r. 
-00006260: 004a 0061 0076 0061 0044 006f 0063 0020  .J.a.v.a.D.o.c. 
-00006270: 0050 0072 00e4 0070 0072 006f 007a 0065  .P.r...p.r.o.z.e
-00006280: 0073 0073 006f 0072 006b 006f 006d 006d  .s.s.o.r.k.o.m.m
-00006290: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
-000062a0: 0000 002c 496e 6163 7469 7665 204a 6176  ...,Inactive Jav
-000062b0: 6144 6f63 2073 7479 6c65 2070 7265 2d70  aDoc style pre-p
-000062c0: 726f 6365 7373 6f72 2063 6f6d 6d65 6e74  rocessor comment
-000062d0: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-000062e0: 5001 0300 0000 4e00 4a00 6100 7600 6100  P.....N.J.a.v.a.
-000062f0: 5300 6300 7200 6900 7000 7400 2000 4900  S.c.r.i.p.t. .I.
-00006300: 6e00 6100 6b00 7400 6900 7600 6500 7200  n.a.k.t.i.v.e.r.
-00006310: 2000 5200 6500 6700 7500 6c00 e400 7200   .R.e.g.u.l...r.
-00006320: 6500 7200 2000 4100 7500 7300 6400 7200  e.r. .A.u.s.d.r.
-00006330: 7500 6300 6b08 0000 0000 0600 0000 2649  u.c.k.........&I
-00006340: 6e61 6374 6976 6520 4a61 7661 5363 7269  nactive JavaScri
-00006350: 7074 2072 6567 756c 6172 2065 7870 7265  pt regular expre
-00006360: 7373 696f 6e07 0000 000c 5173 6369 4c65  ssion.....QsciLe
-00006370: 7865 7243 5050 0103 0000 0066 0049 006e  xerCPP.....f.I.n
-00006380: 0061 006b 0074 0069 0076 0065 0020 0050  .a.k.t.i.v.e. .P
-00006390: 0069 006b 0065 0020 005a 0065 0069 0063  .i.k.e. .Z.e.i.c
-000063a0: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
-000063b0: 0020 0069 006e 0020 0027 0023 002d 0041  . .i.n. .'.#.-.A
-000063c0: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
-000063d0: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
-000063e0: 0027 0800 0000 0006 0000 0020 496e 6163  .'......... Inac
-000063f0: 7469 7665 2050 696b 6520 6861 7368 2d71  tive Pike hash-q
-00006400: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
-00006410: 0c51 7363 694c 6578 6572 4350 5001 0300  .QsciLexerCPP...
-00006420: 0000 6800 4900 6e00 6100 6b00 7400 6900  ..h.I.n.a.k.t.i.
-00006430: 7600 6500 2000 5600 6100 6c00 6100 2000  v.e. .V.a.l.a. .
-00006440: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
-00006450: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
-00006460: 6400 7200 6500 6900 6600 6100 6300 6800  d.r.e.i.f.a.c.h.
-00006470: 6500 6e00 2000 4800 6f00 6300 6800 6b00  e.n. .H.o.c.h.k.
-00006480: 6f00 6d00 6d00 6100 7400 6108 0000 0000  o.m.m.a.t.a.....
-00006490: 0600 0000 2b49 6e61 6374 6976 6520 5661  ....+Inactive Va
-000064a0: 6c61 2074 7269 706c 652d 7175 6f74 6564  la triple-quoted
-000064b0: 2076 6572 6261 7469 6d20 7374 7269 6e67   verbatim string
-000064c0: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-000064d0: 5001 0300 0000 2400 4900 6e00 6100 6b00  P.....$.I.n.a.k.
-000064e0: 7400 6900 7600 6500 7200 2000 5300 7400  t.i.v.e.r. .S.t.
-000064f0: 6100 6e00 6400 6100 7200 6408 0000 0000  a.n.d.a.r.d.....
-00006500: 0600 0000 1049 6e61 6374 6976 6520 6465  .....Inactive de
-00006510: 6661 756c 7407 0000 000c 5173 6369 4c65  fault.....QsciLe
-00006520: 7865 7243 5050 0103 0000 0054 0049 006e  xerCPP.....T.I.n
-00006530: 0061 006b 0074 0069 0076 0065 0020 005a  .a.k.t.i.v.e. .Z
-00006540: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-00006550: 0074 0074 0065 0020 0069 006e 0020 0041  .t.t.e. .i.n. .A
-00006560: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
-00006570: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
-00006580: 0800 0000 0006 0000 001d 496e 6163 7469  ..........Inacti
-00006590: 7665 2064 6f75 626c 652d 7175 6f74 6564  ve double-quoted
-000065a0: 2073 7472 696e 6707 0000 000c 5173 6369   string.....Qsci
-000065b0: 4c65 7865 7243 5050 0103 0000 002e 0049  LexerCPP.......I
-000065c0: 006e 0061 006b 0074 0069 0076 0065 0020  .n.a.k.t.i.v.e. 
-000065d0: 0045 0073 0063 0061 0070 0065 002d 0053  .E.s.c.a.p.e.-.S
-000065e0: 0065 0071 0075 0065 006e 007a 0800 0000  .e.q.u.e.n.z....
-000065f0: 0006 0000 0018 496e 6163 7469 7665 2065  ......Inactive e
-00006600: 7363 6170 6520 7365 7175 656e 6365 0700  scape sequence..
-00006610: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
-00006620: 0300 0000 5800 4900 6e00 6100 6b00 7400  ....X.I.n.a.k.t.
-00006630: 6900 7600 6500 2000 6700 6c00 6f00 6200  i.v.e. .g.l.o.b.
-00006640: 6100 6c00 6500 2000 4b00 6c00 6100 7300  a.l.e. .K.l.a.s.
-00006650: 7300 6500 6e00 2000 7500 6e00 6400 2000  s.e.n. .u.n.d. .
-00006660: 5400 7900 7000 6400 6500 6600 6900 6e00  T.y.p.d.e.f.i.n.
-00006670: 6900 7400 6900 6f00 6e00 6500 6e08 0000  i.t.i.o.n.e.n...
-00006680: 0000 0600 0000 2449 6e61 6374 6976 6520  ......$Inactive 
-00006690: 676c 6f62 616c 2063 6c61 7373 6573 2061  global classes a
-000066a0: 6e64 2074 7970 6564 6566 7307 0000 000c  nd typedefs.....
-000066b0: 5173 6369 4c65 7865 7243 5050 0103 0000  QsciLexerCPP....
-000066c0: 0028 0049 006e 0061 006b 0074 0069 0076  .(.I.n.a.k.t.i.v
-000066d0: 0065 0072 0020 0042 0065 007a 0065 0069  .e.r. .B.e.z.e.i
-000066e0: 0063 0068 006e 0065 0072 0800 0000 0006  .c.h.n.e.r......
-000066f0: 0000 0013 496e 6163 7469 7665 2069 6465  ....Inactive ide
-00006700: 6e74 6966 6965 7207 0000 000c 5173 6369  ntifier.....Qsci
-00006710: 4c65 7865 7243 5050 0103 0000 002e 0049  LexerCPP.......I
-00006720: 006e 0061 006b 0074 0069 0076 0065 0073  .n.a.k.t.i.v.e.s
-00006730: 0020 0053 0063 0068 006c 00fc 0073 0073  . .S.c.h.l...s.s
-00006740: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
-00006750: 0006 0000 0010 496e 6163 7469 7665 206b  ......Inactive k
-00006760: 6579 776f 7264 0700 0000 0c51 7363 694c  eyword.....QsciL
-00006770: 6578 6572 4350 5001 0300 0000 1a00 4900  exerCPP.......I.
-00006780: 6e00 6100 6b00 7400 6900 7600 6500 2000  n.a.k.t.i.v.e. .
-00006790: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
-000067a0: 0f49 6e61 6374 6976 6520 6e75 6d62 6572  .Inactive number
-000067b0: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-000067c0: 5001 0300 0000 2400 4900 6e00 6100 6b00  P.....$.I.n.a.k.
-000067d0: 7400 6900 7600 6500 7200 2000 4f00 7000  t.i.v.e.r. .O.p.
-000067e0: 6500 7200 6100 7400 6f00 7208 0000 0000  e.r.a.t.o.r.....
-000067f0: 0600 0000 1149 6e61 6374 6976 6520 6f70  .....Inactive op
-00006800: 6572 6174 6f72 0700 0000 0c51 7363 694c  erator.....QsciL
-00006810: 6578 6572 4350 5001 0300 0000 4200 4900  exerCPP.....B.I.
-00006820: 6e00 6100 6b00 7400 6900 7600 6500 7200  n.a.k.t.i.v.e.r.
-00006830: 2000 4300 2000 5000 7200 e400 7000 7200   .C. .P.r...p.r.
-00006840: 6f00 7a00 6500 7300 7300 6f00 7200 6b00  o.z.e.s.s.o.r.k.
-00006850: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-00006860: 0000 0000 0600 0000 2049 6e61 6374 6976  ........ Inactiv
-00006870: 6520 7072 652d 7072 6f63 6573 736f 7220  e pre-processor 
-00006880: 4320 636f 6d6d 656e 7407 0000 000c 5173  C comment.....Qs
-00006890: 6369 4c65 7865 7243 5050 0103 0000 0036  ciLexerCPP.....6
-000068a0: 0049 006e 0061 006b 0074 0069 0076 0065  .I.n.a.k.t.i.v.e
-000068b0: 0072 0020 0050 0072 00e4 0070 0072 006f  .r. .P.r...p.r.o
-000068c0: 007a 0065 0073 0073 006f 0072 0062 006c  .z.e.s.s.o.r.b.l
-000068d0: 006f 0063 006b 0800 0000 0006 0000 001c  .o.c.k..........
-000068e0: 496e 6163 7469 7665 2070 7265 2d70 726f  Inactive pre-pro
-000068f0: 6365 7373 6f72 2062 6c6f 636b 0700 0000  cessor block....
-00006900: 0c51 7363 694c 6578 6572 4350 5001 0300  .QsciLexerCPP...
-00006910: 0000 6200 4900 6e00 6100 6b00 7400 6900  ..b.I.n.a.k.t.i.
-00006920: 7600 6500 2000 7300 6500 6b00 7500 6e00  v.e. .s.e.k.u.n.
-00006930: 6400 e400 7200 6500 2000 5300 6300 6800  d...r.e. .S.c.h.
-00006940: 6c00 7500 7300 7300 6500 6c00 7700 f600  l.u.s.s.e.l.w...
-00006950: 7200 7400 6500 7200 2000 7500 6e00 6400  r.t.e.r. .u.n.d.
-00006960: 2000 4200 6500 7a00 6500 6900 6300 6800   .B.e.z.e.i.c.h.
-00006970: 6e00 6500 7208 0000 0000 0600 0000 2b49  n.e.r.........+I
-00006980: 6e61 6374 6976 6520 7365 636f 6e64 6172  nactive secondar
-00006990: 7920 6b65 7977 6f72 6473 2061 6e64 2069  y keywords and i
-000069a0: 6465 6e74 6966 6965 7273 0700 0000 0c51  dentifiers.....Q
-000069b0: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
-000069c0: 4800 4900 6e00 6100 6b00 7400 6900 7600  H.I.n.a.k.t.i.v.
-000069d0: 6500 2000 5a00 6500 6900 6300 6800 6500  e. .Z.e.i.c.h.e.
-000069e0: 6e00 6b00 6500 7400 7400 6500 2000 6900  n.k.e.t.t.e. .i.
-000069f0: 6e00 2000 4800 6f00 6300 6800 6b00 6f00  n. .H.o.c.h.k.o.
-00006a00: 6d00 6d00 6100 7400 6108 0000 0000 0600  m.m.a.t.a.......
-00006a10: 0000 1d49 6e61 6374 6976 6520 7369 6e67  ...Inactive sing
-00006a20: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
-00006a30: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-00006a40: 5001 0300 0000 3600 4900 6e00 6100 6b00  P.....6.I.n.a.k.
-00006a50: 7400 6900 7600 6500 2000 4100 7500 6600  t.i.v.e. .A.u.f.
-00006a60: 6700 6100 6200 6500 6e00 6d00 6100 7200  g.a.b.e.n.m.a.r.
-00006a70: 6b00 6900 6500 7200 7500 6e00 6708 0000  k.i.e.r.u.n.g...
-00006a80: 0000 0600 0000 1449 6e61 6374 6976 6520  .......Inactive 
-00006a90: 7461 736b 206d 6172 6b65 7207 0000 000c  task marker.....
-00006aa0: 5173 6369 4c65 7865 7243 5050 0103 0000  QsciLexerCPP....
-00006ab0: 0040 0049 006e 0061 006b 0074 0069 0076  .@.I.n.a.k.t.i.v
-00006ac0: 0065 0020 0075 006e 0062 0065 0065 006e  .e. .u.n.b.e.e.n
-00006ad0: 0064 0065 0074 0065 0020 005a 0065 0069  .d.e.t.e. .Z.e.i
-00006ae0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00006af0: 0065 0800 0000 0006 0000 0018 496e 6163  .e..........Inac
-00006b00: 7469 7665 2075 6e63 6c6f 7365 6420 7374  tive unclosed st
-00006b10: 7269 6e67 0700 0000 0c51 7363 694c 6578  ring.....QsciLex
-00006b20: 6572 4350 5001 0300 0000 4800 4900 6e00  erCPP.....H.I.n.
-00006b30: 6100 6b00 7400 6900 7600 6500 7300 2000  a.k.t.i.v.e.s. .
-00006b40: 4e00 7500 7400 7a00 6500 7200 2000 6400  N.u.t.z.e.r. .d.
-00006b50: 6500 6600 6900 6e00 6900 6500 7200 7400  e.f.i.n.i.e.r.t.
-00006b60: 6500 7300 2000 4c00 6900 7400 6500 7200  e.s. .L.i.t.e.r.
-00006b70: 6100 6c08 0000 0000 0600 0000 1d49 6e61  a.l..........Ina
-00006b80: 6374 6976 6520 7573 6572 2d64 6566 696e  ctive user-defin
-00006b90: 6564 206c 6974 6572 616c 0700 0000 0c51  ed literal.....Q
-00006ba0: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
-00006bb0: 2a00 4a00 6100 7600 6100 4400 6f00 6300  *.J.a.v.a.D.o.c.
-00006bc0: 2000 5300 6300 6800 6c00 fc00 7300 7300   .S.c.h.l...s.s.
-00006bd0: 6500 6c00 7700 6f00 7200 7408 0000 0000  e.l.w.o.r.t.....
-00006be0: 0600 0000 0f4a 6176 6144 6f63 206b 6579  .....JavaDoc key
-00006bf0: 776f 7264 0700 0000 0c51 7363 694c 6578  word.....QsciLex
-00006c00: 6572 4350 5001 0300 0000 3600 4a00 6100  erCPP.....6.J.a.
-00006c10: 7600 6100 4400 6f00 6300 2000 5300 6300  v.a.D.o.c. .S.c.
-00006c20: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
-00006c30: 6f00 7200 7400 6600 6500 6800 6c00 6500  o.r.t.f.e.h.l.e.
-00006c40: 7208 0000 0000 0600 0000 154a 6176 6144  r..........JavaD
-00006c50: 6f63 206b 6579 776f 7264 2065 7272 6f72  oc keyword error
-00006c60: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-00006c70: 5001 0300 0000 2600 4a00 6100 7600 6100  P.....&.J.a.v.a.
-00006c80: 4400 6f00 6300 2000 4300 2000 4b00 6f00  D.o.c. .C. .K.o.
-00006c90: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
-00006ca0: 0000 0600 0000 174a 6176 6144 6f63 2073  .......JavaDoc s
-00006cb0: 7479 6c65 2043 2063 6f6d 6d65 6e74 0700  tyle C comment..
-00006cc0: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
-00006cd0: 0300 0000 2a00 4a00 6100 7600 6100 4400  ....*.J.a.v.a.D.
-00006ce0: 6f00 6300 2000 4300 2b00 2b00 2000 4b00  o.c. .C.+.+. .K.
-00006cf0: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-00006d00: 0000 0000 0600 0000 194a 6176 6144 6f63  .........JavaDoc
-00006d10: 2073 7479 6c65 2043 2b2b 2063 6f6d 6d65   style C++ comme
-00006d20: 6e74 0700 0000 0c51 7363 694c 6578 6572  nt.....QsciLexer
-00006d30: 4350 5001 0300 0000 3a00 4a00 6100 7600  CPP.....:.J.a.v.
-00006d40: 6100 4400 6f00 6300 2000 5000 7200 e400  a.D.o.c. .P.r...
-00006d50: 7000 7200 6f00 7a00 6500 7300 7300 6f00  p.r.o.z.e.s.s.o.
-00006d60: 7200 6b00 6f00 6d00 6d00 6500 6e00 7400  r.k.o.m.m.e.n.t.
-00006d70: 6100 7208 0000 0000 0600 0000 234a 6176  a.r.........#Jav
-00006d80: 6144 6f63 2073 7479 6c65 2070 7265 2d70  aDoc style pre-p
-00006d90: 726f 6365 7373 6f72 2063 6f6d 6d65 6e74  rocessor comment
-00006da0: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
-00006db0: 5001 0300 0000 3a00 4a00 6100 7600 6100  P.....:.J.a.v.a.
-00006dc0: 5300 6300 7200 6900 7000 7400 2000 5200  S.c.r.i.p.t. .R.
-00006dd0: 6500 6700 7500 6c00 e400 7200 6500 7200  e.g.u.l...r.e.r.
-00006de0: 2000 4100 7500 7300 6400 7200 7500 6300   .A.u.s.d.r.u.c.
-00006df0: 6b08 0000 0000 0600 0000 1d4a 6176 6153  k..........JavaS
-00006e00: 6372 6970 7420 7265 6775 6c61 7220 6578  cript regular ex
-00006e10: 7072 6573 7369 6f6e 0700 0000 0c51 7363  pression.....Qsc
-00006e20: 694c 6578 6572 4350 5001 0300 0000 1a00  iLexerCPP.......
-00006e30: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
-00006e40: 6c00 7700 6f00 7200 7408 0000 0000 0600  l.w.o.r.t.......
-00006e50: 0000 074b 6579 776f 7264 0700 0000 0c51  ...Keyword.....Q
-00006e60: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
-00006e70: 0800 5a00 6100 6800 6c08 0000 0000 0600  ..Z.a.h.l.......
-00006e80: 0000 064e 756d 6265 7207 0000 000c 5173  ...Number.....Qs
-00006e90: 6369 4c65 7865 7243 5050 0103 0000 0010  ciLexerCPP......
-00006ea0: 004f 0070 0065 0072 0061 0074 006f 0072  .O.p.e.r.a.t.o.r
-00006eb0: 0800 0000 0006 0000 0008 4f70 6572 6174  ..........Operat
-00006ec0: 6f72 0700 0000 0c51 7363 694c 6578 6572  or.....QsciLexer
-00006ed0: 4350 5001 0300 0000 5400 5000 6900 6b00  CPP.....T.P.i.k.
-00006ee0: 6500 2000 5a00 6500 6900 6300 6800 6500  e. .Z.e.i.c.h.e.
-00006ef0: 6e00 6b00 6500 7400 7400 6500 2000 6900  n.k.e.t.t.e. .i.
-00006f00: 6e00 2000 2700 2300 2d00 4100 6e00 6600  n. .'.#.-.A.n.f.
-00006f10: fc00 6800 7200 7500 6e00 6700 7300 7a00  ..h.r.u.n.g.s.z.
-00006f20: 6500 6900 6300 6800 6500 6e00 2708 0000  e.i.c.h.e.n.'...
-00006f30: 0000 0600 0000 1750 696b 6520 6861 7368  .......Pike hash
-00006f40: 2d71 756f 7465 6420 7374 7269 6e67 0700  -quoted string..
-00006f50: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
-00006f60: 0300 0000 2e00 4300 2000 5000 7200 e400  ......C. .P.r...
-00006f70: 7000 7200 6f00 7a00 6500 7300 7300 6f00  p.r.o.z.e.s.s.o.
-00006f80: 7200 6b00 6f00 6d00 6d00 6500 6e00 7400  r.k.o.m.m.e.n.t.
-00006f90: 6100 7208 0000 0000 0600 0000 1750 7265  a.r..........Pre
-00006fa0: 2d70 726f 6365 7373 6f72 2043 2063 6f6d  -processor C com
-00006fb0: 6d65 6e74 0700 0000 0c51 7363 694c 6578  ment.....QsciLex
-00006fc0: 6572 4350 5001 0300 0000 2200 5000 7200  erCPP.....".P.r.
-00006fd0: e400 7000 7200 6f00 7a00 6500 7300 7300  ..p.r.o.z.e.s.s.
-00006fe0: 6f00 7200 6200 6c00 6f00 6300 6b08 0000  o.r.b.l.o.c.k...
-00006ff0: 0000 0600 0000 1350 7265 2d70 726f 6365  .......Pre-proce
-00007000: 7373 6f72 2062 6c6f 636b 0700 0000 0c51  ssor block.....Q
+00000010: a700 0000 0264 6542 0000 19a8 0000 4e69  .....deB......Ni
+00000020: 0000 b496 0000 51c9 0000 efdc 0000 5534  ......Q.......U4
+00000030: 0000 e1f4 0000 5534 0000 fee1 0000 5a77  ......U4......Zw
+00000040: 0000 648f 0000 5a77 0000 aaa8 0000 d477  ..d...Zw.......w
+00000050: 0001 1d6e 0004 a7d4 0001 28aa 0004 e898  ...n......(.....
+00000060: 0000 e072 0005 304b 0000 c537 0005 4835  ...r..0K...7..H5
+00000070: 0000 edd0 0005 a9d4 0000 b398 0005 acf4  ................
+00000080: 0000 ee97 0005 acf4 0001 1102 0009 4924  ..............I$
+00000090: 0000 50e3 0009 4924 0001 1753 0012 dd54  ..P...I$...S...T
+000000a0: 0000 c66b 0027 8374 0000 ce94 0029 5bc4  ...k.'.t.....)[.
+000000b0: 0000 ac44 002a a679 0001 27b1 002b 8baf  ...D.*.y..'..+..
+000000c0: 0001 2824 002b c4af 0001 286d 0039 0e07  ..($.+....(m.9..
+000000d0: 0000 95d5 0042 6dad 0000 d830 0047 8681  .....Bm....0.G..
+000000e0: 0000 9005 0048 9889 0000 da4e 004c 9962  .....H.....N.L.b
+000000f0: 0000 3da4 004c 9962 0000 beb4 004c 9962  ..=..L.b.....L.b
+00000100: 0000 dfa3 004c 9962 0000 fbdc 004d 27e3  .....L.b.....M'.
+00000110: 0000 cb58 004e 96c0 0001 1067 0052 78bc  ...X.N.....g.Rx.
+00000120: 0000 4215 0052 78bc 0000 43f3 0052 78bc  ..B..Rx...C..Rx.
+00000130: 0000 7ffb 0052 78bc 0000 ba12 0056 8aa5  .....Rx......V..
+00000140: 0000 2bb2 005c 83b5 0000 6579 005c 83b5  ..+..\....ey.\..
+00000150: 0001 098d 005e 0a74 0000 a6ae 0063 b6c2  .....^.t.....c..
+00000160: 0001 0495 006f bab4 0000 8f6e 0073 e0e7  .....o.....n.s..
+00000170: 0000 a57b 007a aafe 0001 0038 007b 9007  ...{.z.....8.{..
+00000180: 0000 82a4 007c 3e04 0000 4d5c 007e bc9e  .....|>...M\.~..
+00000190: 0000 3a25 0096 5645 0000 fda4 009e eb05  ..:%..VE........
+000001a0: 0000 1a71 00a3 b3d2 0000 973f 00a5 d2f7  ...q.......?....
+000001b0: 0000 860e 00ad 347e 0000 7eb3 00b6 dab4  ......4~..~.....
+000001c0: 0000 94a5 00c7 1af4 0001 0323 00cc 2ff5  ...........#../.
+000001d0: 0000 28f9 00cc db85 0000 d017 00ce e525  ..(............%
+000001e0: 0000 51ca 00e4 6ff2 0000 bb5e 00e4 6ff2  ..Q...o....^..o.
+000001f0: 0000 bf29 00f3 65e2 0000 ad51 0105 baa5  ...)..e....Q....
+00000200: 0000 2a1f 0117 2602 0000 0307 011e f55e  ..*...&........^
+00000210: 0000 7d5b 0120 3527 0000 4b94 0128 263b  ..}[. 5'..K..(&;
+00000220: 0001 1b9a 012f c0ab 0000 4333 0133 11f9  ...../....C3.3..
+00000230: 0000 dae9 013a 8deb 0000 4492 013d 5ad4  .....:....D..=Z.
+00000240: 0000 1741 0146 6b79 0000 e54a 0152 bd35  ...A.Fky...J.R.5
+00000250: 0000 1ee2 0165 f69e 0000 32d3 0177 a774  .....e....2..w.t
+00000260: 0000 334c 0177 a774 0000 37b8 0177 a774  ..3L.w.t..7..w.t
+00000270: 0000 664d 0177 a774 0000 6fd9 0177 a774  ..fM.w.t..o..w.t
+00000280: 0000 b3c5 017b 82d5 0000 2dd0 017b f202  .....{....-..{..
+00000290: 0000 2173 017f c374 0000 9ff3 017f e469  ..!s...t.......i
+000002a0: 0000 6a5f 0199 f534 0000 cd56 019b 25d4  ..j_...4...V..%.
+000002b0: 0000 2234 01a4 14f4 0000 9baf 01a8 b8f4  .."4............
+000002c0: 0001 0d88 01a9 3e5e 0001 1aae 01a9 6c22  ......>^......l"
+000002d0: 0000 e9fa 01b2 2f57 0000 cb91 01b4 8575  ....../W.......u
+000002e0: 0000 3058 01c1 6d85 0000 d0a5 01c1 6d85  ..0X..m.......m.
+000002f0: 0001 0126 01c1 6d85 0001 0ad8 01c1 6d85  ...&..m.......m.
+00000300: 0001 11f0 01d0 e6d4 0000 353e 01d0 e6d4  ..........5>....
+00000310: 0000 3e7e 01d0 e6d4 0000 41d1 01d0 e6d4  ..>~......A.....
+00000320: 0000 5a3b 01d0 e6d4 0000 6c6c 01d0 e6d4  ..Z;......ll....
+00000330: 0000 729f 01d0 e6d4 0000 7fb3 01d0 e6d4  ..r.............
+00000340: 0000 b9d0 01d0 e6d4 0000 c9c7 01d0 e6d4  ................
+00000350: 0000 d87e 01d0 e6d4 0000 e147 01d0 e6d4  ...~.......G....
+00000360: 0000 ed4a 01d0 e6d4 0000 f3bf 01d0 e6d4  ...J............
+00000370: 0000 fdf5 01d0 e6d4 0001 037b 01d0 e6d4  ...........{....
+00000380: 0001 12b3 01d0 e6d4 0001 260b 01d1 2772  ..........&...'r
+00000390: 0001 2756 01d2 fb89 0000 dbdc 01d5 8bf4  ..'V............
+000003a0: 0001 0e13 01da fa2e 0000 06ea 01e0 8e89  ................
+000003b0: 0000 5f98 01e0 9e89 0000 5fe6 01e0 fe89  .._......._.....
+000003c0: 0000 5f4a 01e2 0512 0000 f30f 01e2 f8b3  .._J............
+000003d0: 0000 494a 01e5 4055 0000 0038 01e5 b1e5  ..IJ..@U...8....
+000003e0: 0000 00bf 0209 aac5 0000 86f5 020c b1d7  ................
+000003f0: 0000 f688 0221 cdc2 0001 2575 0223 1df5  .....!....%u.#..
+00000400: 0000 fe38 024e 68f8 0000 2b51 0264 fcb9  ...8.Nh...+Q.d..
+00000410: 0000 dd9e 0266 c104 0000 4dd7 0268 1032  .....f....M..h.2
+00000420: 0000 091d 0280 659e 0001 1f56 0281 9c55  ......e....V...U
+00000430: 0000 cdb9 0282 8583 0001 1c10 0287 f37d  ...............}
+00000440: 0000 c573 0298 62ce 0001 1360 02a2 5fd7  ...s..b....`.._.
+00000450: 0000 9e8b 02b6 8aa5 0001 27ea 02c8 3477  ..........'...4w
+00000460: 0000 5138 02d0 0ab5 0001 1452 02d3 3955  ..Q8.......R..9U
+00000470: 0000 0d32 02d3 70c5 0000 0de4 02d3 ab9e  ...2..p.........
+00000480: 0001 2150 02d5 3b25 0001 1406 02f1 64f2  ..!P..;%......d.
+00000490: 0000 5389 02f1 64f2 0001 1a06 0303 2fc3  ..S...d......./.
+000004a0: 0000 aef1 0304 4002 0001 0864 0308 eabd  ......@....d....
+000004b0: 0000 b06a 030a c82c 0000 ed93 030e 0675  ...j...,.......u
+000004c0: 0000 2b03 0310 4fe5 0000 2aab 0337 0c92  ..+...O...*..7..
+000004d0: 0000 70a6 033c 3974 0000 0690 034a e838  ..p..<9t.....J.8
+000004e0: 0000 7904 0356 ee89 0000 3396 0357 b394  ..y..V....3..W..
+000004f0: 0000 9112 036d fe44 0000 1b5a 0381 d155  .....m.D...Z...U
+00000500: 0000 0144 0385 1324 0000 8dc0 0385 ae02  ...D...$........
+00000510: 0000 9c92 0388 bef5 0000 e7f6 038c 84b4  ................
+00000520: 0000 20b6 038f 4dbe 0001 09bd 0394 e4de  .. ...M.........
+00000530: 0000 66a0 03a5 ed15 0000 30dc 03aa 7b07  ..f.......0...{.
+00000540: 0000 4642 03b9 9aa4 0000 4c08 03bc c824  ..FB......L....$
+00000550: 0000 71f8 03c1 6fb5 0001 009d 03cf 1ca5  ..q...o.........
+00000560: 0000 01f1 03d5 3754 0000 d63f 03df ea15  ......7T...?....
+00000570: 0000 cef9 03e1 8f14 0000 63db 03e3 ced4  ..........c.....
+00000580: 0000 b151 03f1 0e14 0000 b1a0 03f1 3f92  ...Q..........?.
+00000590: 0000 9f9e 03f3 3313 0000 31d4 03f8 c5f2  ......3...1.....
+000005a0: 0000 0485 0406 b233 0001 225f 0407 e797  .......3.."_....
+000005b0: 0000 92de 0424 8a05 0000 229c 0434 9c25  .....$...."..4.%
+000005c0: 0000 5edb 044d 5095 0000 b336 0451 f1a5  ..^..MP....6.Q..
+000005d0: 0000 1beb 045b a5e5 0000 1f92 045b ee75  .....[.......[.u
+000005e0: 0000 1f36 0466 8ad3 0000 6516 046c 26f7  ...6.f....e..l&.
+000005f0: 0000 9cd8 047f 0845 0000 0c64 048d 5a6b  .......E...d..Zk
+00000600: 0001 2206 048f 8947 0000 5e42 0496 0d85  .."....G..^B....
+00000610: 0000 1487 0498 49bc 0000 0000 04a1 ae63  ......I........c
+00000620: 0000 5231 04a4 5b74 0000 686f 04a6 bff5  ..R1..[t..ho....
+00000630: 0000 388a 04ac 2ca5 0001 28ea 04b9 c374  ..8...,...(....t
+00000640: 0000 681a 04c1 d37e 0000 01a3 04c5 b0b9  ..h....~........
+00000650: 0000 90dc 04d0 3ac2 0000 3493 04d2 2854  ......:...4...(T
+00000660: 0000 cbdd 04d5 0934 0000 a2a8 04d5 499e  .......4......I.
+00000670: 0001 188c 04d7 eba4 0000 abee 04db d9e5  ................
+00000680: 0000 15f5 04e3 587c 0000 fc80 04eb 7ac2  ......X|......z.
+00000690: 0000 788e 04f4 27f4 0000 7328 04f7 f944  ..x...'...s(...D
+000006a0: 0001 16f8 04ff bb93 0000 c6b9 0505 df14  ................
+000006b0: 0000 a5bb 0507 bd0e 0000 6d90 0507 bd0e  ..........m.....
+000006c0: 0000 b7ab 0507 bd0e 0000 e5e7 0507 bd0e  ................
+000006d0: 0000 ff0c 050d 9f95 0000 48fe 050d 9f95  ..........H.....
+000006e0: 0000 b449 050d f2f7 0000 98eb 050e 7678  ...I..........vx
+000006f0: 0000 0fba 0517 36ee 0000 e854 0517 36ee  ......6....T..6.
+00000700: 0001 0d49 0517 6374 0000 899a 0520 54e4  ...I..ct..... T.
+00000710: 0000 823e 0524 3cc4 0000 957b 052a 8e74  ...>.$<....{.*.t
+00000720: 0000 cc2a 052c 5f97 0000 880e 0540 d941  ...*.,_......@.A
+00000730: 0000 7576 0540 d941 0000 bcec 0540 d941  ..uv.@.A.....@.A
+00000740: 0000 d459 0540 d941 0001 066c 0540 d941  ...Y.@.A...l.@.A
+00000750: 0001 0e5e 0540 d942 0000 75c7 0540 d942  ...^.@.B..u..@.B
+00000760: 0000 bd3f 0540 d942 0000 d4ac 0540 d942  ...?.@.B.....@.B
+00000770: 0001 06bf 0540 d942 0001 0eb1 0540 d943  .....@.B.....@.C
+00000780: 0000 7618 0540 d943 0000 bd92 0540 d943  ..v..@.C.....@.C
+00000790: 0000 d4ff 0540 d943 0001 0712 0540 d943  .....@.C.....@.C
+000007a0: 0001 0f04 0540 d944 0000 bde5 0540 d944  .....@.D.....@.D
+000007b0: 0001 0765 0540 d944 0001 0f57 0541 e313  ...e.@.D...W.A..
+000007c0: 0000 6396 0542 0794 0000 7435 0548 a6f4  ..c..B....t5.H..
+000007d0: 0000 b4c1 055b 93f4 0000 7057 055c 38c2  .....[....pW.\8.
+000007e0: 0000 363c 055c 38c2 0000 3b11 055c 38c2  ..6<.\8...;..\8.
+000007f0: 0000 3ec1 055c 38c2 0000 44d6 055c 38c2  ..>..\8...D..\8.
+00000800: 0000 5a7d 055c 38c2 0000 6cb7 055c 38c2  ..Z}.\8...l..\8.
+00000810: 0000 7386 055c 38c2 0000 8031 055c 38c2  ..s..\8....1.\8.
+00000820: 0000 b619 055c 38c2 0000 baf6 055c 38c2  .....\8......\8.
+00000830: 0000 ca0c 055c 38c2 0000 d1a1 055c 38c2  .....\8......\8.
+00000840: 0000 d911 055c 38c2 0000 e18a 055c 38c2  .....\8......\8.
+00000850: 0000 ee04 055c 38c2 0000 f404 055c 38c2  .....\8......\8.
+00000860: 0000 fe77 055c 38c2 0001 03bd 055c 38c2  ...w.\8......\8.
+00000870: 0001 091e 055c 38c2 0001 0c3a 055c 38c2  .....\8....:.\8.
+00000880: 0001 12f6 055c 38c2 0001 20e0 055c 38c2  .....\8... ..\8.
+00000890: 0001 264e 056b 0305 0000 27a7 0572 18f3  ..&N.k....'..r..
+000008a0: 0000 5c2d 0572 18f3 0000 6df0 0572 18f3  ..\-.r....m..r..
+000008b0: 0001 22f0 0573 bdfe 0000 36a4 0576 4219  .."..s....6..vB.
+000008c0: 0000 e265 057b 3a95 0000 17eb 0590 1c5e  ...e.{:........^
+000008d0: 0001 1fbb 0599 8282 0000 3f88 0599 8282  ..........?.....
+000008e0: 0000 e6e1 05a8 8dc4 0000 bf73 05ab 3502  ...........s..5.
+000008f0: 0000 34ff 05ab 3502 0000 3ad2 05ab 3502  ..4...5...:...5.
+00000900: 0000 3e3e 05ab 3502 0000 4a05 05ab 3502  ..>>..5...J...5.
+00000910: 0000 6a17 05ab 3502 0000 7262 05ab 3502  ..j...5...rb..5.
+00000920: 0000 7f11 05ab 3502 0000 b991 05ab 3502  ......5.......5.
+00000930: 0000 c985 05ab 3502 0000 d162 05ab 3502  ......5....b..5.
+00000940: 0000 d7ee 05ab 3502 0000 e107 05ab 3502  ......5.......5.
+00000950: 0000 f37d 05ab 3502 0000 fd64 05ab 3502  ...}..5....d..5.
+00000960: 0001 021e 05ab 3502 0001 08dd 05ab 3502  ......5.......5.
+00000970: 0001 0bba 05ab 3502 0001 1273 05ab 3502  ......5....s..5.
+00000980: 0001 164b 05ab 3502 0001 25cb 05ab 9047  ...K..5...%....G
+00000990: 0000 4577 05ab 9047 0000 7495 05ab 9047  ..Ew...G..t....G
+000009a0: 0000 b70c 05ab 9047 0000 bba3 05ab 9047  .......G.......G
+000009b0: 0000 d347 05ab 9047 0001 1497 05ab 9047  ...G...G.......G
+000009c0: 0001 2387 05af ca82 0001 0bf9 05b0 395c  ..#...........9\
+000009d0: 0000 ffd0 05b0 395c 0001 10cf 05ba 3a34  ......9\......:4
+000009e0: 0000 faf9 05c0 be1c 0000 02ac 05d0 e445  ...............E
+000009f0: 0000 0743 05da a793 0000 ebff 05e2 af74  ...C...........t
+00000a00: 0000 b572 05f1 8ed4 0000 941f 05f8 8384  ...r............
+00000a10: 0000 059b 0619 f9e5 0000 23c6 0627 71cb  ..........#..'q.
+00000a20: 0000 d5b9 0629 6e14 0000 29ac 062a c4c3  .....)n...)..*..
+00000a30: 0000 d2de 0638 cdd2 0000 5653 063f 5e74  .....8....VS.?^t
+00000a40: 0000 91c2 065d ed75 0000 2d28 065f 70d4  .....].u..-(._p.
+00000a50: 0000 330e 066f 3f43 0001 2470 067d da1b  ..3..o?C..$p.}..
+00000a60: 0000 5bd7 067d da1b 0000 6d31 067d da1b  ..[..}....m1.}..
+00000a70: 0000 80a5 067e af18 0000 79ba 0693 cf64  .....~....y....d
+00000a80: 0000 1e48 069c 2827 0000 ab2e 06a0 ab2e  ...H..('........
+00000a90: 0000 78ca 06b6 95a7 0000 8bed 06bd 90c7  ..x.............
+00000aa0: 0000 a160 06c7 0023 0000 c02a 06c8 9002  ...`...#...*....
+00000ab0: 0000 366b 06c8 9002 0000 3b40 06c8 9002  ..6k......;@....
+00000ac0: 0000 3ef1 06c8 9002 0000 4247 06c8 9002  ..>.......BG....
+00000ad0: 0000 5aac 06c8 9002 0000 635d 06c8 9002  ..Z.......c]....
+00000ae0: 0000 6cef 06c8 9002 0000 73b3 06c8 9002  ..l.......s.....
+00000af0: 0000 8066 06c8 9002 0000 b649 06c8 9002  ...f.......I....
+00000b00: 0000 bb25 06c8 9002 0000 beeb 06c8 9002  ...%............
+00000b10: 0000 ca3e 06c8 9002 0000 d244 06c8 9002  ...>.......D....
+00000b20: 0000 d943 06c8 9002 0000 e1ba 06c8 9002  ...C............
+00000b30: 0000 f436 06c8 9002 0000 fea7 06c8 9002  ...6............
+00000b40: 0001 03ec 06c8 9002 0001 0c69 06c8 9002  ...........i....
+00000b50: 0001 1326 06c8 9002 0001 2113 06c8 9002  ...&......!.....
+00000b60: 0001 267e 06d1 bd38 0000 1db1 06d2 e715  ..&~...8........
+00000b70: 0000 cc84 06d4 8784 0000 4113 06e0 e6a7  ..........A.....
+00000b80: 0000 a49f 0707 0e97 0000 ba8d 0708 77d4  ..............w.
+00000b90: 0000 6238 070f a795 0000 0e96 070f ee05  ..b8............
+00000ba0: 0000 0f28 0717 a922 0000 9365 0729 3625  ...(..."...e.)6%
+00000bb0: 0000 0867 0729 7fb5 0000 07b1 072a 7959  ...g.).......*yY
+00000bc0: 0000 616a 0734 fb9b 0000 46b9 0735 9c74  ..aj.4....F..5.t
+00000bd0: 0000 6ac0 0736 7cd4 0001 04ff 0738 b8f4  ..j..6|......8..
+00000be0: 0001 0faa 0740 0f45 0000 2333 0743 abb3  .....@.E..#3.C..
+00000bf0: 0000 ee3a 075f 75e2 0000 9c56 0762 1812  ...:._u....V.b..
+00000c00: 0000 5d2b 0764 2a19 0000 e3ab 0764 2a69  ..]+.d*......d*i
+00000c10: 0000 e2b8 0764 2ac9 0000 e49e 0764 2af9  .....d*......d*.
+00000c20: 0000 e4f4 0769 f814 0000 62e4 076d 903b  .....i....b..m.;
+00000c30: 0000 c119 076e ccf4 0000 ae71 07aa ac92  .....n.....q....
+00000c40: 0001 0004 07aa b6c4 0001 0069 07ab a407  ...........i....
+00000c50: 0000 f897 07ab a477 0000 f84e 07ab a4d7  .......w...N....
+00000c60: 0000 f8e0 07ab a4e7 0000 f929 07ab a677  ...........)...w
+00000c70: 0000 f805 07ae 08d7 0000 73ea 07ae ddc3  ..........s.....
+00000c80: 0000 b0c7 07af 4cc4 0000 5945 07dc 8ca4  ......L...YE....
+00000c90: 0000 951f 07dd c0a9 0000 a51a 07e0 e484  ................
+00000ca0: 0000 81d6 07e6 6bd4 0000 5b71 07f0 d307  ......k...[q....
+00000cb0: 0000 4507 0800 99e4 0000 a7a4 0809 5fa4  ..E..........._.
+00000cc0: 0000 8cf9 081f 07fe 0001 1b2f 0826 40c5  .........../.&@.
+00000cd0: 0000 2445 0826 e5b5 0000 9b31 082a 0f07  ..$E.&.....1.*..
+00000ce0: 0000 9809 082b fc89 0000 dfd6 0833 6794  .....+.......3g.
+00000cf0: 0000 0639 083c 2e14 0000 2663 083f 1a05  ...9.<....&c.?..
+00000d00: 0000 b1eb 0846 6b79 0000 e30e 084b 415c  .....Fky.....KA\
+00000d10: 0000 5dd9 085d 44a3 0000 c227 0869 314b  ..]..]D....'.i1K
+00000d20: 0000 43b8 086a 5832 0000 7cc6 086a bd82  ..C..jX2..|..j..
+00000d30: 0000 1055 086a d9e4 0000 4c5c 086a e832  ...U.j....L\.j.2
+00000d40: 0000 7c71 086f 31a4 0000 25e1 087c d65e  ..|q.o1...%..|.^
+00000d50: 0000 0257 0880 d317 0000 8e81 0883 9bf2  ...W............
+00000d60: 0000 c5de 0883 9c42 0001 094f 0887 e322  .......B...O..."
+00000d70: 0000 7021 0887 e322 0000 b857 0887 e322  ..p!..."...W..."
+00000d80: 0000 d720 088a 6c54 0000 117c 088f 7ee5  ... ..lT...|..~.
+00000d90: 0000 4282 088f 7ee5 0000 4607 088f 7ee5  ..B...~...F...~.
+00000da0: 0000 65a7 088f 7ee5 0000 bfa7 0895 9f04  ..e...~.........
+00000db0: 0000 4e58 0895 b2b4 0000 83b9 08a6 3263  ..NX..........2c
+00000dc0: 0000 d27d 08aa 4ea5 0000 2ef4 08b0 9c32  ...}..N........2
+00000dd0: 0000 ac98 08ba fbc5 0000 391c 08ba fbc5  ..........9.....
+00000de0: 0000 d126 08c0 d214 0000 5429 08d8 2c37  ...&......T)..,7
+00000df0: 0000 502f 08df 6007 0000 ec63 08e5 ad04  ..P/..`....c....
+00000e00: 0000 49cc 08e5 ad04 0000 69d5 08e8 f3e4  ..I.......i.....
+00000e10: 0000 a945 08ec 8907 0000 8514 08f6 17fb  ...E............
+00000e20: 0001 1dcc 08f6 1e32 0000 8d59 08f9 a694  .......2...Y....
+00000e30: 0000 03d0 08fe 4074 0000 7a28 0909 7ed5  ......@t..z(..~.
+00000e40: 0000 0371 090b e857 0000 f554 0926 3027  ...q...W...T.&0'
+00000e50: 0000 36d7 0926 3027 0000 f5f1 0933 f8a4  ..6..&0'.....3..
+00000e60: 0000 1699 093f 33e4 0000 aa38 0940 7c55  .....?3....8.@|U
+00000e70: 0000 ab79 0941 8583 0000 551f 0941 8583  ...y.A....U..A..
+00000e80: 0001 1cbc 0944 519c 0000 eccf 0966 ccc9  .....DQ......f..
+00000e90: 0000 b6cc 096f 94a0 0000 a9b5 098f 2f04  .....o......../.
+00000ea0: 0001 168e 0990 4074 0001 05b1 099e 9e32  ......@t.......2
+00000eb0: 0000 52ce 099e 9e32 0001 17ac 09a8 9fd7  ..R....2........
+00000ec0: 0000 8ee8 09aa 7744 0000 b005 09ac f7f7  ......wD........
+00000ed0: 0000 adf7 09af 0eb2 0000 4164 09b1 5ef7  ..........Ad..^.
+00000ee0: 0000 a0df 09b2 b917 0000 5ae5 09b4 01d7  ..........Z.....
+00000ef0: 0000 341c 09b4 01d7 0000 39ae 09b4 01d7  ..4.......9.....
+00000f00: 0000 3d2c 09b4 01d7 0000 4887 09b4 01d7  ..=,......H.....
+00000f10: 0000 60f3 09b4 01d7 0000 68ff 09b4 01d7  ..`.......h.....
+00000f20: 0000 7e36 09b4 01d7 0000 c90b 09b4 01d7  ..~6............
+00000f30: 0000 de69 09b4 01d7 0000 f222 09b4 01d7  ...i......."....
+00000f40: 0000 fb64 09b4 01d7 0001 01a7 09ba b00e  ...d............
+00000f50: 0000 f019 09c3 8dc1 0000 b2e9 09c9 5824  ..............X$
+00000f60: 0000 da7d 09db ed3d 0000 e21f 09f9 d724  ...}...=.......$
+00000f70: 0000 6b2d 0a00 69e4 0000 12b7 0a05 2c45  ..k-..i.......,E
+00000f80: 0000 f9f1 0a06 f357 0000 4425 0a0c cf35  .......W..D%...5
+00000f90: 0000 18f0 0a13 efd4 0000 9e3d 0a18 ea34  ...........=...4
+00000fa0: 0000 9a21 0a1f 3d57 0000 55cd 0a20 9c62  ...!..=W..U.. .b
+00000fb0: 0000 c4dd 0a20 9c82 0000 c429 0a20 9c92  ..... .....). ..
+00000fc0: 0000 c483 0a20 9ca2 0000 c375 0a20 9cb2  ..... .....u. ..
+00000fd0: 0000 c3cf 0a20 9cd2 0000 c31b 0a22 1715  ..... ......."..
+00000fe0: 0000 0b62 0a27 e734 0000 47b0 0a29 ecd7  ...b.'.4..G..)..
+00000ff0: 0000 4f88 0a2a b253 0000 3c7b 0a2a b253  ..O..*.S..<{.*.S
+00001000: 0000 db9f 0a2a b253 0000 f972 0a2b 4f34  .....*.S...r.+O4
+00001010: 0000 eb18 0a30 e882 0000 d796 0a46 599e  .....0.......FY.
+00001020: 0000 74d2 0a49 713e 0000 3f2b 0a53 e6b5  ..t..Iq>..?+.S..
+00001030: 0000 f05a 0a53 e6b5 0000 f9af 0a5a 8c73  ...Z.S.......Z.s
+00001040: 0001 1eaa 0a5a ff55 0000 2fa8 0a5e 17d7  .....Z.U../..^..
+00001050: 0000 56be 0a5e 17d7 0001 1e2d 0a64 3804  ..V..^.....-.d8.
+00001060: 0000 77e5 0a64 3804 0000 c85c 0a64 3804  ..w..d8....\.d8.
+00001070: 0001 07b8 0a64 3804 0001 0ffb 0a64 3c14  .....d8......d<.
+00001080: 0000 3850 0a64 3c14 0000 3cb8 0a64 3c14  ..8P.d<...<..d<.
+00001090: 0000 409d 0a64 3c14 0000 42bd 0a64 3c14  ..@..d<...B..d<.
+000010a0: 0000 6081 0a64 3c14 0000 781a 0a64 3c14  ..`..d<...x..d<.
+000010b0: 0000 7d1b 0a64 3c14 0000 b88f 0a64 3c14  ..}..d<......d<.
+000010c0: 0000 be38 0a64 3c14 0000 c893 0a64 3c14  ...8.d<......d<.
+000010d0: 0000 cae8 0a64 3c14 0000 d06b 0a64 3c14  .....d<....k.d<.
+000010e0: 0000 dc63 0a64 3c14 0000 ead7 0a64 3c14  ...c.d<......d<.
+000010f0: 0000 ef0f 0a64 3c14 0000 f09e 0a64 3c14  .....d<......d<.
+00001100: 0000 fa3f 0a64 3c14 0001 00ec 0a64 3c14  ...?.d<......d<.
+00001110: 0001 07ee 0a64 3c14 0001 0a10 0a64 3c14  .....d<......d<.
+00001120: 0001 116a 0a64 3c14 0001 15d1 0a64 3c14  ...j.d<......d<.
+00001130: 0001 2501 0a64 7f34 0000 46fd 0a66 adf1  ..%..d.4..F..f..
+00001140: 0000 b10c 0a67 9b24 0001 0dd6 0a68 c1d2  .....g.$.....h..
+00001150: 0000 f128 0a6b 9f2c 0000 c630 0a6b 9f2c  ...(.k.,...0.k.,
+00001160: 0001 1099 0a71 6592 0000 8e2a 0a73 280e  .....qe....*.s(.
+00001170: 0000 e966 0a7c 0487 0000 47f6 0a92 e092  ...f.|....G.....
+00001180: 0000 7b3b 0a95 f824 0000 96d2 0a9c b564  ..{;...$.......d
+00001190: 0000 dd1d 0aa1 fa52 0000 6034 0aa9 ec25  .......R..`4...%
+000011a0: 0000 13ea 0ab0 d642 0000 8a4f 0abc 8c74  .......B...O...t
+000011b0: 0000 33e4 0abc 8c74 0000 38e4 0abc 8c74  ..3....t..8....t
+000011c0: 0000 3cf3 0abc 8c74 0000 40d9 0abc 8c74  ..<....t..@....t
+000011d0: 0000 42f9 0abc 8c74 0000 484f 0abc 8c74  ..B....t..HO...t
+000011e0: 0000 60bb 0abc 8c74 0000 68be 0abc 8c74  ..`....t..h....t
+000011f0: 0000 71c2 0abc 8c74 0000 7855 0abc 8c74  ..q....t..xU...t
+00001200: 0000 7aff 0abc 8c74 0000 7da4 0abc 8c74  ..z....t..}....t
+00001210: 0000 af36 0abc 8c74 0000 b410 0abc 8c74  ...6...t.......t
+00001220: 0000 b959 0abc 8c74 0000 be77 0abc 8c74  ...Y...t...w...t
+00001230: 0000 c15b 0abc 8c74 0000 c8d0 0abc 8c74  ...[...t.......t
+00001240: 0000 cb21 0abc 8c74 0000 d0ee 0abc 8c74  ...!...t.......t
+00001250: 0000 d75b 0abc 8c74 0000 dce4 0abc 8c74  ...[...t.......t
+00001260: 0000 ebc0 0abc 8c74 0000 ef50 0abc 8c74  .......t...P...t
+00001270: 0000 f167 0abc 8c74 0000 fac0 0abc 8c74  ...g...t.......t
+00001280: 0001 016f 0abc 8c74 0001 082a 0abc 8c74  ...o...t...*...t
+00001290: 0001 0b21 0abc 8c74 0001 102f 0abc 8c74  ...!...t.../...t
+000012a0: 0001 123a 0abc 8c74 0001 160f 0abc 8c74  ...:...t.......t
+000012b0: 0001 253c 0ac6 ede4 0001 2031 0ad1 7ae4  ..%<...... 1..z.
+000012c0: 0000 9072 0ae8 5a54 0000 9a68 0af3 13a5  ...r..ZT...h....
+000012d0: 0000 1c95 0af3 5a35 0000 1d23 0b02 f807  ......Z5...#....
+000012e0: 0000 ce3e 0b0d 5fb4 0000 9ded 0b0e 3f04  ...>.._.......?.
+000012f0: 0000 996b 0b1a a2b4 0000 cf80 0b22 8f85  ...k........."..
+00001300: 0000 315c 0b24 18e7 0000 f1a2 0b24 9574  ..1\.$.......$.t
+00001310: 0000 d552 0b27 ac64 0000 2cb7 0b28 a084  ...R.'.d..,..(..
+00001320: 0000 a835 0b38 8835 0000 26e7 0b3b 32c8  ...5.8.5..&..;2.
+00001330: 0000 1fee 0b3b 5eb7 0000 8aaa 0b41 be5c  .....;^......A.\
+00001340: 0000 1e8a 0b45 d7c4 0000 a726 0b5f a0d4  .....E.....&._..
+00001350: 0000 210e 0b63 56e5 0000 76d7 0b64 19f3  ..!..cV...v..d..
+00001360: 0000 bbe2 0b64 4ea4 0000 fcb4 0b65 1484  .....dN......e..
+00001370: 0000 acf3 0b70 d343 0000 697f 0b76 5d77  .....p.C..i..v]w
+00001380: 0000 473d 0b76 5d77 0000 679e 0b76 8fb8  ..G=.v]w..g..v..
+00001390: 0000 7669 0b7d 54f4 0000 4b31 0b80 3424  ..vi.}T...K1..4$
+000013a0: 0000 a63f 0b81 f4c9 0000 e63f 0b85 25a4  ...?.......?..%.
+000013b0: 0000 532a 0b8f d415 0000 5f10 0b8f d415  ..S*......_.....
+000013c0: 0000 8fca 0b8f d415 0001 112f 0ba3 dc0c  .........../....
+000013d0: 0001 2920 0ba3 fc0c 0000 2eae 0bac a23b  ..) ...........;
+000013e0: 0001 23ca 0bbf 7902 0000 2053 0bc7 7c12  ..#...y... S..|.
+000013f0: 0000 5817 0bc7 7c12 0000 6bf7 0bc7 7c12  ..X...|...k...|.
+00001400: 0001 02b7 0bca 4275 0000 e91e 0bcf 7a44  ......Bu......zD
+00001410: 0000 156a 0bd3 95e5 0000 d1d0 0bdb 2728  ...j..........'(
+00001420: 0000 7727 0bdc b6f4 0000 24f2 0bdd 4f05  ..w'......$...O.
+00001430: 0000 f29c 0bdd 4f05 0000 fc0f 0be0 af42  ......O........B
+00001440: 0000 3b79 0be5 f563 0000 afb0 0bec c634  ..;y...c.......4
+00001450: 0000 3fbc 0bec c634 0000 e715 0bf1 7f29  ..?....4.......)
+00001460: 0000 e894 0c02 d897 0000 99ba 0c06 e461  ...............a
+00001470: 0000 af6e 0c09 f045 0000 9d96 0c0d 298b  ...n...E......).
+00001480: 0000 f0db 0c0d 298b 0001 0a4a 0c0d 298b  ......)....J..).
+00001490: 0001 11a5 0c0f d674 0000 7be1 0c1a 4642  .......t..{...FB
+000014a0: 0001 13b3 0c1c 0d58 0001 0a94 0c23 01d7  .......X.....#..
+000014b0: 0000 f472 0c3e d602 0000 a090 0c4a ac8e  ...r.>.......J..
+000014c0: 0000 34c6 0c4a ac8e 0000 437d 0c4a ac8e  ..4..J....C}.J..
+000014d0: 0001 08a2 0c4b 8642 0000 7a95 0c57 4c85  .....K.B..z..WL.
+000014e0: 0000 eb65 0c57 f6dc 0000 85ad 0c66 cef2  ...e.W.......f..
+000014f0: 0000 62a2 0c6a dfe3 0000 c198 0c6f 05c2  ..b..j.......o..
+00001500: 0000 3dd7 0c6f 05c2 0000 e0a0 0c6f 05c2  ..=..o.......o..
+00001510: 0000 fcfd 0c97 49a4 0000 3958 0ca7 1d27  ......I...9X...'
+00001520: 0000 9036 0caf 2c14 0000 7164 0cc1 0fc5  ...6..,...qd....
+00001530: 0000 ef8f 0cc8 1b6b 0000 54ac 0cc8 fc25  .......k..T....%
+00001540: 0000 cfde 0cc8 fc25 0001 26b8 0cd0 418e  .......%..&...A.
+00001550: 0000 7f56 0cd0 e6b7 0000 93a4 0cdd 0147  ...V...........G
+00001560: 0000 4aa1 0ce7 2104 0001 199a 0cf1 0414  ..J...!.........
+00001570: 0000 58e1 0cf4 cf72 0001 26f3 0cf7 efc4  ..X....r..&.....
+00001580: 0000 8c97 0cfb 27d7 0000 9aad 0cfb f375  ......'........u
+00001590: 0000 0a9a 0cfe 788e 0000 848f 0d03 1a93  ......x.........
+000015a0: 0000 b231 0d12 0d2e 0000 dc9e 0d12 0d2e  ...1............
+000015b0: 0000 fa7a 0d13 a645 0000 aad3 0d27 b834  ...z...E.....'.4
+000015c0: 0000 2c4c 0d31 9335 0000 bfe5 0d39 3433  ..,L.1.5.....943
+000015d0: 0000 b8c9 0d40 2634 0000 a344 0d40 2a24  .....@&4...D.@*$
+000015e0: 0000 a300 0d44 8cf4 0000 b277 0d5f e113  .....D.....w._..
+000015f0: 0000 b809 0d63 a562 0000 7de2 0d74 7d34  .....c.b..}..t}4
+00001600: 0000 3580 0d74 7d34 0000 72df 0d74 7d34  ..5..t}4..r..t}4
+00001610: 0000 b5cd 0d74 7d34 0000 ba42 0d74 7d34  .....t}4...B.t}4
+00001620: 0000 d8c3 0d74 7d34 0001 2091 0d77 74bc  .....t}4.. ..wt.
+00001630: 0000 5737 0d82 89d4 0000 5883 0d84 5c52  ..W7......X...\R
+00001640: 0000 e019 0d85 04e3 0000 61d4 0d87 97b4  ..........a.....
+00001650: 0001 191d 0d8c 3f44 0000 869a 0d94 b9a2  ......?D........
+00001660: 0000 53d3 0d94 b9a2 0001 1a54 0d9d 4967  ..S........T..Ig
+00001670: 0000 3c1d 0d9d 4967 0000 5d7b 0d9d 4967  ..<...Ig..]{..Ig
+00001680: 0000 6f00 0d9d 4967 0000 751a 0d9d 4967  ..o...Ig..u...Ig
+00001690: 0000 8172 0d9d 4967 0000 b74c 0d9d 4967  ...r..Ig...L..Ig
+000016a0: 0000 bc8e 0d9d 4967 0000 d3fb 0d9d 4967  ......Ig......Ig
+000016b0: 0000 d9ed 0d9d 4967 0000 f7a4 0d9d 4967  ......Ig......Ig
+000016c0: 0001 14d7 0d9d 4967 0001 240e 0da1 0584  ......Ig..$.....
+000016d0: 0000 4a44 0dab e374 0000 57bd 0dab e374  ..JD...t..W....t
+000016e0: 0000 6b94 0dab e374 0001 025d 0dba 7574  ..k....t...]..ut
+000016f0: 0001 0ca2 0dc2 60e5 0000 9d50 0dd7 2e84  ......`....P....
+00001700: 0000 a8ba 0ddc 7d6e 0001 21b6 0ddd 1614  ......}n..!.....
+00001710: 0000 35cb 0de4 87ce 0000 4ef3 0de5 9c12  ..5.......N.....
+00001720: 0000 cd00 0df1 7912 0000 8939 0e02 d357  ......y....9...W
+00001730: 0000 ad9c 0e06 4282 0000 4cd3 0e0d 63f2  ......B...L...c.
+00001740: 0000 09da 0e0f 0be9 0000 64b9 0e27 bbd2  ..........d..'..
+00001750: 0000 121b 0e39 0c85 0000 88a7 0e3d a465  .....9.......=.e
+00001760: 0000 9f18 0e47 3212 0000 7b8d 0e48 1849  .....G2...{..H.I
+00001770: 0000 b513 0e4f a809 0000 dee1 0e56 89c7  .....O.......V..
+00001780: 0000 a20a 0e57 b45c 0000 9896 0e5d 8b67  .....W.\.....].g
+00001790: 0000 8b37 0e65 9654 0000 9296 0e68 7784  ...7.e.T.....hw.
+000017a0: 0000 966e 0e69 e572 0000 a45d 0e6c 1e64  ...n.i.r...].l.d
+000017b0: 0000 8349 0e77 e667 0000 a3d6 0e7b 0fd4  ...I.w.g.....{..
+000017c0: 0000 87b4 0e87 f32d 0000 c7e3 0e90 da43  .......-.......C
+000017d0: 0000 e9a9 0e91 f3e2 0001 0425 0e9b 2634  ...........%..&4
+000017e0: 0000 924c 0ea1 4ea5 0000 19ce 0ea3 08c7  ...L..N.........
+000017f0: 0000 3bb2 0ea3 08c7 0000 4031 0ea3 08c7  ..;.......@1....
+00001800: 0000 5cc0 0ea3 08c7 0000 6424 0ea3 08c7  ..\.......d$....
+00001810: 0000 6e8c 0ea3 08c7 0000 8101 0ea3 08c7  ..n.............
+00001820: 0000 ca7a 0ea3 08c7 0000 d97f 0ea3 08c7  ...z............
+00001830: 0000 e78a 0ea3 08c7 0000 f4e6 0ea3 08c7  ................
+00001840: 0000 ff64 0ea3 08c7 0001 0601 0ea3 f542  ...d...........B
+00001850: 0000 8432 0ea5 5f07 0000 6f67 0ea5 bfb4  ...2.._...og....
+00001860: 0000 8758 0ead 2977 0000 f719 0eb4 0ece  ...X..)w........
+00001870: 0001 180c 0eb8 a434 0001 0b59 0eba 2e2d  .......4...Y...-
+00001880: 0000 aeb4 0ec6 a614 0001 0554 0ec7 6e04  ...........T..n.
+00001890: 0000 1348 0ec8 d9a4 0000 6712 0eca bebe  ...H......g.....
+000018a0: 0000 3802 0eca bfbe 0000 3a84 0ed0 4c84  ..8.......:...L.
+000018b0: 0000 10ee 0ed3 6b43 0000 d386 0ee0 7ca5  ......kC......|.
+000018c0: 0000 04e8 0eeb 6a85 0000 796e 0eec 7334  ......j...yn..s4
+000018d0: 0001 1584 0ef6 0a35 0000 2874 0ef6 b2e5  .......5..(t....
+000018e0: 0000 c2c4 0efe 320e 0000 59c3 0efe 320e  ......2...Y...2.
+000018f0: 0000 9790 0f18 4092 0000 89fe 0f22 0577  ......@......".w
+00001900: 0000 ea7c 0f23 7d77 0000 65e0 0f27 815b  ...|.#}w..e..'.[
+00001910: 0000 d6a0 0f32 a185 0000 631c 0f34 2b34  .....2....c..4+4
+00001920: 0000 2be7 0f38 db34 0000 3262 0f39 3c33  ..+..8.4..2b.9<3
+00001930: 0000 c747 0f46 6b79 0000 e401 0f52 ce92  ...G.Fky.....R..
+00001940: 0000 a04b 0f6d 2577 0001 0d03 0f75 40d4  ...K.m%w.....u@.
+00001950: 0000 376b 0f75 40d4 0000 45b8 0f75 40d4  ..7k.u@...E..u@.
+00001960: 0001 1536 0f84 d524 0000 7107 0f89 3214  ...6...$..q...2.
+00001970: 0000 9bfe 0f90 2974 0000 0429 0fb5 6e45  ......)t...)..nE
+00001980: 0000 2e41 0fc0 9654 0000 a38e 0fc4 9494  ...A...T........
+00001990: 0000 7c27 0fc4 d414 0000 21d9 0fcd c123  ..|'......!....#
+000019a0: 0000 c094 0fdc e525 0000 255f 0fe1 b2c4  .......%..%_....
+000019b0: 0000 eecb 0fe5 3972 0000 b683 0ff9 ac95  ......9r........
+000019c0: 0000 7799 6900 0129 6803 0000 0012 0041  ..w.i..)h......A
+000019d0: 0062 0062 0072 0065 0063 0068 0065 006e  .b.b.r.e.c.h.e.n
+000019e0: 0800 0000 0006 0000 0006 4361 6e63 656c  ..........Cancel
+000019f0: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+00001a00: 0103 0000 0048 0041 0075 0073 0077 0061  .....H.A.u.s.w.a
+00001a10: 0068 006c 0020 0069 006e 0020 004b 006c  .h.l. .i.n. .K.l
+00001a20: 0065 0069 006e 0062 0075 0063 0068 0073  .e.i.n.b.u.c.h.s
+00001a30: 0074 0061 0062 0065 006e 0020 0075 006d  .t.a.b.e.n. .u.m
+00001a40: 0077 0061 006e 0064 0065 006c 006e 0800  .w.a.n.d.e.l.n..
+00001a50: 0000 0006 0000 001f 436f 6e76 6572 7420  ........Convert 
+00001a60: 7365 6c65 6374 696f 6e20 746f 206c 6f77  selection to low
+00001a70: 6572 2063 6173 6507 0000 000b 5173 6369  er case.....Qsci
+00001a80: 436f 6d6d 616e 6401 0300 0000 4600 4100  Command.....F.A.
+00001a90: 7500 7300 7700 6100 6800 6c00 2000 6900  u.s.w.a.h.l. .i.
+00001aa0: 6e00 2000 4700 7200 6f00 df00 6200 7500  n. .G.r.o...b.u.
+00001ab0: 6300 6800 7300 7400 6100 6200 6500 6e00  c.h.s.t.a.b.e.n.
+00001ac0: 2000 7500 6d00 7700 6100 6e00 6400 6500   .u.m.w.a.n.d.e.
+00001ad0: 6c00 6e08 0000 0000 0600 0000 1f43 6f6e  l.n..........Con
+00001ae0: 7665 7274 2073 656c 6563 7469 6f6e 2074  vert selection t
+00001af0: 6f20 7570 7065 7220 6361 7365 0700 0000  o upper case....
+00001b00: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+00001b10: 002e 0041 006b 0074 0075 0065 006c 006c  ...A.k.t.u.e.l.l
+00001b20: 0065 0020 005a 0065 0069 006c 0065 0020  .e. .Z.e.i.l.e. 
+00001b30: 006b 006f 0070 0069 0065 0072 0065 006e  .k.o.p.i.e.r.e.n
+00001b40: 0800 0000 0006 0000 0011 436f 7079 2063  ..........Copy c
+00001b50: 7572 7265 6e74 206c 696e 6507 0000 000b  urrent line.....
+00001b60: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00001b70: 2000 4100 7500 7300 7700 6100 6800 6c00   .A.u.s.w.a.h.l.
+00001b80: 2000 6b00 6f00 7000 6900 6500 7200 6500   .k.o.p.i.e.r.e.
+00001b90: 6e08 0000 0000 0600 0000 0e43 6f70 7920  n..........Copy 
+00001ba0: 7365 6c65 6374 696f 6e07 0000 000b 5173  selection.....Qs
+00001bb0: 6369 436f 6d6d 616e 6401 0300 0000 3600  ciCommand.....6.
+00001bc0: 4100 6b00 7400 7500 6500 6c00 6c00 6500  A.k.t.u.e.l.l.e.
+00001bd0: 2000 5a00 6500 6900 6c00 6500 2000 6100   .Z.e.i.l.e. .a.
+00001be0: 7500 7300 7300 6300 6800 6e00 6500 6900  u.s.s.c.h.n.e.i.
+00001bf0: 6400 6500 6e08 0000 0000 0600 0000 1043  d.e.n..........C
+00001c00: 7574 2063 7572 7265 6e74 206c 696e 6507  ut current line.
+00001c10: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00001c20: 0300 0000 2800 4100 7500 7300 7700 6100  ....(.A.u.s.w.a.
+00001c30: 6800 6c00 2000 6100 7500 7300 7300 6300  h.l. .a.u.s.s.c.
+00001c40: 6800 6e00 6500 6900 6400 6500 6e08 0000  h.n.e.i.d.e.n...
+00001c50: 0000 0600 0000 0d43 7574 2073 656c 6563  .......Cut selec
+00001c60: 7469 6f6e 0700 0000 0b51 7363 6943 6f6d  tion.....QsciCom
+00001c70: 6d61 6e64 0103 0000 0028 0045 0069 006e  mand.....(.E.i.n
+00001c80: 0065 0020 0045 0062 0065 006e 0065 0020  .e. .E.b.e.n.e. 
+00001c90: 0061 0075 0073 0072 00fc 0063 006b 0065  .a.u.s.r...c.k.e
+00001ca0: 006e 0800 0000 0006 0000 0013 4465 2d69  .n..........De-i
+00001cb0: 6e64 656e 7420 6f6e 6520 6c65 7665 6c07  ndent one level.
+00001cc0: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00001cd0: 0300 0000 3200 4100 6b00 7400 7500 6500  ....2.A.k.t.u.e.
+00001ce0: 6c00 6c00 6500 7300 2000 5a00 6500 6900  l.l.e.s. .Z.e.i.
+00001cf0: 6300 6800 6500 6e00 2000 6c00 f600 7300  c.h.e.n. .l...s.
+00001d00: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+00001d10: 1844 656c 6574 6520 6375 7272 656e 7420  .Delete current 
+00001d20: 6368 6172 6163 7465 7207 0000 000b 5173  character.....Qs
+00001d30: 6369 436f 6d6d 616e 6401 0300 0000 2c00  ciCommand.....,.
+00001d40: 4100 6b00 7400 7500 6500 6c00 6c00 6500  A.k.t.u.e.l.l.e.
+00001d50: 2000 5a00 6500 6900 6c00 6500 2000 6c00   .Z.e.i.l.e. .l.
+00001d60: f600 7300 6300 6800 6500 6e08 0000 0000  ..s.c.h.e.n.....
+00001d70: 0600 0000 1344 656c 6574 6520 6375 7272  .....Delete curr
+00001d80: 656e 7420 6c69 6e65 0700 0000 0b51 7363  ent line.....Qsc
+00001d90: 6943 6f6d 6d61 6e64 0103 0000 0026 005a  iCommand.....&.Z
+00001da0: 0065 0069 006c 0065 0020 006c 0069 006e  .e.i.l.e. .l.i.n
+00001db0: 006b 0073 0020 006c 00f6 0073 0063 0068  .k.s. .l...s.c.h
+00001dc0: 0065 006e 0800 0000 0006 0000 0013 4465  .e.n..........De
+00001dd0: 6c65 7465 206c 696e 6520 746f 206c 6566  lete line to lef
+00001de0: 7407 0000 000b 5173 6369 436f 6d6d 616e  t.....QsciComman
+00001df0: 6401 0300 0000 2800 5a00 6500 6900 6c00  d.....(.Z.e.i.l.
+00001e00: 6500 2000 7200 6500 6300 6800 7400 7300  e. .r.e.c.h.t.s.
+00001e10: 2000 6c00 f600 7300 6300 6800 6500 6e08   .l...s.c.h.e.n.
+00001e20: 0000 0000 0600 0000 1444 656c 6574 6520  .........Delete 
+00001e30: 6c69 6e65 2074 6f20 7269 6768 7407 0000  line to right...
+00001e40: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
+00001e50: 0000 2a00 5a00 6500 6900 6300 6800 6500  ..*.Z.e.i.c.h.e.
+00001e60: 6e00 2000 6c00 6900 6e00 6b00 7300 2000  n. .l.i.n.k.s. .
+00001e70: 6c00 f600 7300 6300 6800 6500 6e08 0000  l...s.c.h.e.n...
+00001e80: 0000 0600 0000 1944 656c 6574 6520 7072  .......Delete pr
+00001e90: 6576 696f 7573 2063 6861 7261 6374 6572  evious character
+00001ea0: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+00001eb0: 0103 0000 0062 005a 0065 0069 0063 0068  .....b.Z.e.i.c.h
+00001ec0: 0065 006e 0020 006c 0069 006e 006b 0073  .e.n. .l.i.n.k.s
+00001ed0: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
+00001ee0: 002c 0020 0077 0065 006e 006e 0020 006e  .,. .w.e.n.n. .n
+00001ef0: 0069 0063 0068 0074 0020 0061 006d 0020  .i.c.h.t. .a.m. 
+00001f00: 005a 0065 0069 006c 0065 006e 0061 006e  .Z.e.i.l.e.n.a.n
+00001f10: 0066 0061 006e 0067 0800 0000 0006 0000  .f.a.n.g........
+00001f20: 0031 4465 6c65 7465 2070 7265 7669 6f75  .1Delete previou
+00001f30: 7320 6368 6172 6163 7465 7220 6966 206e  s character if n
+00001f40: 6f74 2061 7420 7374 6172 7420 6f66 206c  ot at start of l
+00001f50: 696e 6507 0000 000b 5173 6369 436f 6d6d  ine.....QsciComm
+00001f60: 616e 6401 0300 0000 5e00 5200 6500 6300  and.....^.R.e.c.
+00001f70: 6800 7400 7300 2000 6200 6900 7300 2000  h.t.s. .b.i.s. .
+00001f80: 7a00 7500 6d00 2000 4500 6e00 6400 6500  z.u.m. .E.n.d.e.
+00001f90: 2000 6400 6500 7300 2000 6e00 e400 6300   .d.e.s. .n...c.
+00001fa0: 6800 7300 7400 6500 6e00 2000 5700 6f00  h.s.t.e.n. .W.o.
+00001fb0: 7200 7400 6500 7300 2000 6c00 f600 7300  r.t.e.s. .l...s.
+00001fc0: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+00001fd0: 2044 656c 6574 6520 7269 6768 7420 746f   Delete right to
+00001fe0: 2065 6e64 206f 6620 6e65 7874 2077 6f72   end of next wor
+00001ff0: 6407 0000 000b 5173 6369 436f 6d6d 616e  d.....QsciComman
+00002000: 6401 0300 0000 2400 5700 6f00 7200 7400  d.....$.W.o.r.t.
+00002010: 2000 6c00 6900 6e00 6b00 7300 2000 6c00   .l.i.n.k.s. .l.
+00002020: f600 7300 6300 6800 6500 6e08 0000 0000  ..s.c.h.e.n.....
+00002030: 0600 0000 1344 656c 6574 6520 776f 7264  .....Delete word
+00002040: 2074 6f20 6c65 6674 0700 0000 0b51 7363   to left.....Qsc
+00002050: 6943 6f6d 6d61 6e64 0103 0000 0026 0057  iCommand.....&.W
+00002060: 006f 0072 0074 0020 0072 0065 0063 0068  .o.r.t. .r.e.c.h
+00002070: 0074 0073 0020 006c 00f6 0073 0063 0068  .t.s. .l...s.c.h
+00002080: 0065 006e 0800 0000 0006 0000 0014 4465  .e.n..........De
+00002090: 6c65 7465 2077 6f72 6420 746f 2072 6967  lete word to rig
+000020a0: 6874 0700 0000 0b51 7363 6943 6f6d 6d61  ht.....QsciComma
+000020b0: 6e64 0103 0000 0026 0041 0075 0073 0077  nd.....&.A.u.s.w
+000020c0: 0061 0068 006c 0020 0064 0075 0070 006c  .a.h.l. .d.u.p.l
+000020d0: 0069 007a 0069 0065 0072 0065 006e 0800  .i.z.i.e.r.e.n..
+000020e0: 0000 0006 0000 0013 4475 706c 6963 6174  ........Duplicat
+000020f0: 6520 7365 6c65 6374 696f 6e07 0000 000b  e selection.....
+00002100: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00002110: 3400 4100 6b00 7400 7500 6500 6c00 6c00  4.A.k.t.u.e.l.l.
+00002120: 6500 2000 5a00 6500 6900 6c00 6500 2000  e. .Z.e.i.l.e. .
+00002130: 6400 7500 7000 6c00 6900 7a00 6900 6500  d.u.p.l.i.z.i.e.
+00002140: 7200 6500 6e08 0000 0000 0600 0000 1a44  r.e.n..........D
+00002150: 7570 6c69 6361 7465 2074 6865 2063 7572  uplicate the cur
+00002160: 7265 6e74 206c 696e 6507 0000 000b 5173  rent line.....Qs
+00002170: 6369 436f 6d6d 616e 6401 0300 0000 6c00  ciCommand.....l.
+00002180: 5200 6500 6300 6800 7400 6500 6300 6b00  R.e.c.h.t.e.c.k.
+00002190: 6900 6700 6500 2000 4100 7500 7300 7700  i.g.e. .A.u.s.w.
+000021a0: 6100 6800 6c00 2000 7500 6d00 2000 6500  a.h.l. .u.m. .e.
+000021b0: 6900 6e00 6500 2000 5a00 6500 6900 6c00  i.n.e. .Z.e.i.l.
+000021c0: 6500 2000 6e00 6100 6300 6800 2000 7500  e. .n.a.c.h. .u.
+000021d0: 6e00 7400 6500 6e00 2000 6500 7200 7700  n.t.e.n. .e.r.w.
+000021e0: 6500 6900 7400 6500 7200 6e08 0000 0000  e.i.t.e.r.n.....
+000021f0: 0600 0000 2a45 7874 656e 6420 7265 6374  ....*Extend rect
+00002200: 616e 6775 6c61 7220 7365 6c65 6374 696f  angular selectio
+00002210: 6e20 646f 776e 206f 6e65 206c 696e 6507  n down one line.
+00002220: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00002230: 0300 0000 6c00 5200 6500 6300 6800 7400  ....l.R.e.c.h.t.
+00002240: 6500 6300 6b00 6900 6700 6500 2000 4100  e.c.k.i.g.e. .A.
+00002250: 7500 7300 7700 6100 6800 6c00 2000 7500  u.s.w.a.h.l. .u.
+00002260: 6d00 2000 6500 6900 6e00 6500 2000 5300  m. .e.i.n.e. .S.
+00002270: 6500 6900 7400 6500 2000 6e00 6100 6300  e.i.t.e. .n.a.c.
+00002280: 6800 2000 7500 6e00 7400 6500 6e00 2000  h. .u.n.t.e.n. .
+00002290: 6500 7200 7700 6500 6900 7400 6500 7200  e.r.w.e.i.t.e.r.
+000022a0: 6e08 0000 0000 0600 0000 2a45 7874 656e  n.........*Exten
+000022b0: 6420 7265 6374 616e 6775 6c61 7220 7365  d rectangular se
+000022c0: 6c65 6374 696f 6e20 646f 776e 206f 6e65  lection down one
+000022d0: 2070 6167 6507 0000 000b 5173 6369 436f   page.....QsciCo
+000022e0: 6d6d 616e 6401 0300 0000 6e00 5200 6500  mmand.....n.R.e.
+000022f0: 6300 6800 7400 6500 6300 6b00 6900 6700  c.h.t.e.c.k.i.g.
+00002300: 6500 2000 4100 7500 7300 7700 6100 6800  e. .A.u.s.w.a.h.
+00002310: 6c00 2000 7500 6d00 2000 6500 6900 6e00  l. .u.m. .e.i.n.
+00002320: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
+00002330: 2000 6e00 6100 6300 6800 2000 6c00 6900   .n.a.c.h. .l.i.
+00002340: 6e00 6b00 7300 2000 6500 7200 7700 6500  n.k.s. .e.r.w.e.
+00002350: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
+00002360: 0000 2f45 7874 656e 6420 7265 6374 616e  ../Extend rectan
+00002370: 6775 6c61 7220 7365 6c65 6374 696f 6e20  gular selection 
+00002380: 6c65 6674 206f 6e65 2063 6861 7261 6374  left one charact
+00002390: 6572 0700 0000 0b51 7363 6943 6f6d 6d61  er.....QsciComma
+000023a0: 6e64 0103 0000 0070 0052 0065 0063 0068  nd.....p.R.e.c.h
+000023b0: 0074 0065 0063 006b 0069 0067 0065 0020  .t.e.c.k.i.g.e. 
+000023c0: 0041 0075 0073 0077 0061 0068 006c 0020  .A.u.s.w.a.h.l. 
+000023d0: 0075 006d 0020 0065 0069 006e 0020 005a  .u.m. .e.i.n. .Z
+000023e0: 0065 0069 0063 0068 0065 006e 0020 006e  .e.i.c.h.e.n. .n
+000023f0: 0061 0063 0068 0020 0072 0065 0063 0068  .a.c.h. .r.e.c.h
+00002400: 0074 0073 0020 0065 0072 0077 0065 0069  .t.s. .e.r.w.e.i
+00002410: 0074 0065 0072 006e 0800 0000 0006 0000  .t.e.r.n........
+00002420: 0030 4578 7465 6e64 2072 6563 7461 6e67  .0Extend rectang
+00002430: 756c 6172 2073 656c 6563 7469 6f6e 2072  ular selection r
+00002440: 6967 6874 206f 6e65 2063 6861 7261 6374  ight one charact
+00002450: 6572 0700 0000 0b51 7363 6943 6f6d 6d61  er.....QsciComma
+00002460: 6e64 0103 0000 0074 0052 0065 0063 0068  nd.....t.R.e.c.h
+00002470: 0074 0065 0063 006b 0069 0067 0065 0020  .t.e.c.k.i.g.e. 
+00002480: 0041 0075 0073 0077 0061 0068 006c 0020  .A.u.s.w.a.h.l. 
+00002490: 007a 0075 006d 0020 0045 006e 0064 0065  .z.u.m. .E.n.d.e
+000024a0: 0020 0064 0065 0072 0020 0044 006f 006b  . .d.e.r. .D.o.k
+000024b0: 0075 006d 0065 006e 0074 0065 006e 007a  .u.m.e.n.t.e.n.z
+000024c0: 0065 0069 006c 0065 0020 0065 0072 0077  .e.i.l.e. .e.r.w
+000024d0: 0065 0069 0074 0065 0072 006e 0800 0000  .e.i.t.e.r.n....
+000024e0: 0006 0000 0034 4578 7465 6e64 2072 6563  .....4Extend rec
+000024f0: 7461 6e67 756c 6172 2073 656c 6563 7469  tangular selecti
+00002500: 6f6e 2074 6f20 656e 6420 6f66 2064 6f63  on to end of doc
+00002510: 756d 656e 7420 6c69 6e65 0700 0000 0b51  ument line.....Q
+00002520: 7363 6943 6f6d 6d61 6e64 0103 0000 009a  sciCommand......
+00002530: 0052 0065 0063 0068 0074 0065 0063 006b  .R.e.c.h.t.e.c.k
+00002540: 0069 0067 0065 0020 0041 0075 0073 0077  .i.g.e. .A.u.s.w
+00002550: 0061 0068 006c 0020 007a 0075 006d 0020  .a.h.l. .z.u.m. 
+00002560: 0065 0072 0073 0074 0065 006e 0020 0073  .e.r.s.t.e.n. .s
+00002570: 0069 0063 0068 0074 0062 0061 0072 0065  .i.c.h.t.b.a.r.e
+00002580: 006e 0020 005a 0065 0069 0063 0068 0065  .n. .Z.e.i.c.h.e
+00002590: 006e 0020 0064 0065 0072 0020 0044 006f  .n. .d.e.r. .D.o
+000025a0: 006b 0075 006d 0065 006e 0074 007a 0065  .k.u.m.e.n.t.z.e
+000025b0: 0069 006c 0065 0020 0065 0072 0077 0065  .i.l.e. .e.r.w.e
+000025c0: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
+000025d0: 0000 0048 4578 7465 6e64 2072 6563 7461  ...HExtend recta
+000025e0: 6e67 756c 6172 2073 656c 6563 7469 6f6e  ngular selection
+000025f0: 2074 6f20 6669 7273 7420 7669 7369 626c   to first visibl
+00002600: 6520 6368 6172 6163 7465 7220 696e 2064  e character in d
+00002610: 6f63 756d 656e 7420 6c69 6e65 0700 0000  ocument line....
+00002620: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+00002630: 0078 0052 0065 0063 0068 0074 0065 0063  .x.R.e.c.h.t.e.c
+00002640: 006b 0069 0067 0065 0020 0041 0075 0073  .k.i.g.e. .A.u.s
+00002650: 0077 0061 0068 006c 0020 007a 0075 006d  .w.a.h.l. .z.u.m
+00002660: 0020 0042 0065 0067 0069 006e 006e 0020  . .B.e.g.i.n.n. 
+00002670: 0064 0065 0072 0020 0044 006f 006b 0075  .d.e.r. .D.o.k.u
+00002680: 006d 0065 006e 0074 0065 006e 007a 0065  .m.e.n.t.e.n.z.e
+00002690: 0069 006c 0065 0020 0065 0072 0077 0065  .i.l.e. .e.r.w.e
+000026a0: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
+000026b0: 0000 0036 4578 7465 6e64 2072 6563 7461  ...6Extend recta
+000026c0: 6e67 756c 6172 2073 656c 6563 7469 6f6e  ngular selection
+000026d0: 2074 6f20 7374 6172 7420 6f66 2064 6f63   to start of doc
+000026e0: 756d 656e 7420 6c69 6e65 0700 0000 0b51  ument line.....Q
+000026f0: 7363 6943 6f6d 6d61 6e64 0103 0000 006a  sciCommand.....j
+00002700: 0052 0065 0063 0068 0074 0065 0063 006b  .R.e.c.h.t.e.c.k
+00002710: 0069 0067 0065 0020 0041 0075 0073 0077  .i.g.e. .A.u.s.w
+00002720: 0061 0068 006c 0020 0075 006d 0020 0065  .a.h.l. .u.m. .e
+00002730: 0069 006e 0065 0020 005a 0065 0069 006c  .i.n.e. .Z.e.i.l
+00002740: 0065 0020 006e 0061 0063 0068 0020 006f  .e. .n.a.c.h. .o
+00002750: 0062 0065 006e 0020 0065 0072 0077 0065  .b.e.n. .e.r.w.e
+00002760: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
+00002770: 0000 0028 4578 7465 6e64 2072 6563 7461  ...(Extend recta
+00002780: 6e67 756c 6172 2073 656c 6563 7469 6f6e  ngular selection
+00002790: 2075 7020 6f6e 6520 6c69 6e65 0700 0000   up one line....
+000027a0: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+000027b0: 006a 0052 0065 0063 0068 0074 0065 0063  .j.R.e.c.h.t.e.c
+000027c0: 006b 0069 0067 0065 0020 0041 0075 0073  .k.i.g.e. .A.u.s
+000027d0: 0077 0061 0068 006c 0020 0075 006d 0020  .w.a.h.l. .u.m. 
+000027e0: 0065 0069 006e 0065 0020 0053 0065 0069  .e.i.n.e. .S.e.i
+000027f0: 0074 0065 0020 006e 0061 0063 0068 0020  .t.e. .n.a.c.h. 
+00002800: 006f 0062 0065 006e 0020 0065 0072 0077  .o.b.e.n. .e.r.w
+00002810: 0065 0069 0074 0065 0072 006e 0800 0000  .e.i.t.e.r.n....
+00002820: 0006 0000 0028 4578 7465 6e64 2072 6563  .....(Extend rec
+00002830: 7461 6e67 756c 6172 2073 656c 6563 7469  tangular selecti
+00002840: 6f6e 2075 7020 6f6e 6520 7061 6765 0700  on up one page..
+00002850: 0000 0b51 7363 6943 6f6d 6d61 6e64 0103  ...QsciCommand..
+00002860: 0000 0054 0041 0075 0073 0077 0061 0068  ...T.A.u.s.w.a.h
+00002870: 006c 0020 0075 006d 0020 0065 0069 006e  .l. .u.m. .e.i.n
+00002880: 0065 0020 005a 0065 0069 006c 0065 0020  .e. .Z.e.i.l.e. 
+00002890: 006e 0061 0063 0068 0020 0075 006e 0074  .n.a.c.h. .u.n.t
+000028a0: 0065 006e 0020 0065 0072 0077 0065 0069  .e.n. .e.r.w.e.i
+000028b0: 0074 0065 0072 006e 0800 0000 0006 0000  .t.e.r.n........
+000028c0: 001e 4578 7465 6e64 2073 656c 6563 7469  ..Extend selecti
+000028d0: 6f6e 2064 6f77 6e20 6f6e 6520 6c69 6e65  on down one line
+000028e0: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+000028f0: 0103 0000 0054 0041 0075 0073 0077 0061  .....T.A.u.s.w.a
+00002900: 0068 006c 0020 0075 006d 0020 0065 0069  .h.l. .u.m. .e.i
+00002910: 006e 0065 0020 0053 0065 0069 0074 0065  .n.e. .S.e.i.t.e
+00002920: 0020 006e 0061 0063 0068 0020 0075 006e  . .n.a.c.h. .u.n
+00002930: 0074 0065 006e 0020 0065 0072 0077 0065  .t.e.n. .e.r.w.e
+00002940: 0069 0074 0065 0072 006e 0800 0000 0006  .i.t.e.r.n......
+00002950: 0000 001e 4578 7465 6e64 2073 656c 6563  ....Extend selec
+00002960: 7469 6f6e 2064 6f77 6e20 6f6e 6520 7061  tion down one pa
+00002970: 6765 0700 0000 0b51 7363 6943 6f6d 6d61  ge.....QsciComma
+00002980: 6e64 0103 0000 0058 0041 0075 0073 0077  nd.....X.A.u.s.w
+00002990: 0061 0068 006c 0020 0075 006d 0020 0065  .a.h.l. .u.m. .e
+000029a0: 0069 006e 0065 006e 0020 0041 0062 0073  .i.n.e.n. .A.b.s
+000029b0: 0061 0074 007a 0020 006e 0061 0063 0068  .a.t.z. .n.a.c.h
+000029c0: 0020 0075 006e 0074 0065 006e 0020 0065  . .u.n.t.e.n. .e
+000029d0: 0072 0077 0065 0069 0074 0065 0072 006e  .r.w.e.i.t.e.r.n
+000029e0: 0800 0000 0006 0000 0023 4578 7465 6e64  .........#Extend
+000029f0: 2073 656c 6563 7469 6f6e 2064 6f77 6e20   selection down 
+00002a00: 6f6e 6520 7061 7261 6772 6170 6807 0000  one paragraph...
+00002a10: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
+00002a20: 0000 5600 4100 7500 7300 7700 6100 6800  ..V.A.u.s.w.a.h.
+00002a30: 6c00 2000 7500 6d00 2000 6500 6900 6e00  l. .u.m. .e.i.n.
+00002a40: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
+00002a50: 2000 6e00 6100 6300 6800 2000 6c00 6900   .n.a.c.h. .l.i.
+00002a60: 6e00 6b00 7300 2000 6500 7200 7700 6500  n.k.s. .e.r.w.e.
+00002a70: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
+00002a80: 0000 2345 7874 656e 6420 7365 6c65 6374  ..#Extend select
+00002a90: 696f 6e20 6c65 6674 206f 6e65 2063 6861  ion left one cha
+00002aa0: 7261 6374 6572 0700 0000 0b51 7363 6943  racter.....QsciC
+00002ab0: 6f6d 6d61 6e64 0103 0000 0050 0041 0075  ommand.....P.A.u
+00002ac0: 0073 0077 0061 0068 006c 0020 0075 006d  .s.w.a.h.l. .u.m
+00002ad0: 0020 0065 0069 006e 0020 0057 006f 0072  . .e.i.n. .W.o.r
+00002ae0: 0074 0020 006e 0061 0063 0068 0020 006c  .t. .n.a.c.h. .l
+00002af0: 0069 006e 006b 0073 0020 0065 0072 0077  .i.n.k.s. .e.r.w
+00002b00: 0065 0069 0074 0065 0072 006e 0800 0000  .e.i.t.e.r.n....
+00002b10: 0006 0000 001e 4578 7465 6e64 2073 656c  ......Extend sel
+00002b20: 6563 7469 6f6e 206c 6566 7420 6f6e 6520  ection left one 
+00002b30: 776f 7264 0700 0000 0b51 7363 6943 6f6d  word.....QsciCom
+00002b40: 6d61 6e64 0103 0000 005c 0041 0075 0073  mand.....\.A.u.s
+00002b50: 0077 0061 0068 006c 0020 0075 006d 0020  .w.a.h.l. .u.m. 
+00002b60: 0065 0069 006e 0065 006e 0020 0057 006f  .e.i.n.e.n. .W.o
+00002b70: 0072 0074 0074 0065 0069 006c 0020 006e  .r.t.t.e.i.l. .n
+00002b80: 0061 0063 0068 0020 006c 0069 006e 006b  .a.c.h. .l.i.n.k
+00002b90: 0073 0020 0065 0072 0077 0065 0069 0074  .s. .e.r.w.e.i.t
+00002ba0: 0065 0072 006e 0800 0000 0006 0000 0023  .e.r.n.........#
+00002bb0: 4578 7465 6e64 2073 656c 6563 7469 6f6e  Extend selection
+00002bc0: 206c 6566 7420 6f6e 6520 776f 7264 2070   left one word p
+00002bd0: 6172 7407 0000 000b 5173 6369 436f 6d6d  art.....QsciComm
+00002be0: 616e 6401 0300 0000 5800 4100 7500 7300  and.....X.A.u.s.
+00002bf0: 7700 6100 6800 6c00 2000 7500 6d00 2000  w.a.h.l. .u.m. .
+00002c00: 6500 6900 6e00 2000 5a00 6500 6900 6300  e.i.n. .Z.e.i.c.
+00002c10: 6800 6500 6e00 2000 6e00 6100 6300 6800  h.e.n. .n.a.c.h.
+00002c20: 2000 7200 6500 6300 6800 7400 7300 2000   .r.e.c.h.t.s. .
+00002c30: 6500 7200 7700 6500 6900 7400 6500 7200  e.r.w.e.i.t.e.r.
+00002c40: 6e08 0000 0000 0600 0000 2445 7874 656e  n.........$Exten
+00002c50: 6420 7365 6c65 6374 696f 6e20 7269 6768  d selection righ
+00002c60: 7420 6f6e 6520 6368 6172 6163 7465 7207  t one character.
+00002c70: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00002c80: 0300 0000 5200 4100 7500 7300 7700 6100  ....R.A.u.s.w.a.
+00002c90: 6800 6c00 2000 7500 6d00 2000 6500 6900  h.l. .u.m. .e.i.
+00002ca0: 6e00 2000 5700 6f00 7200 7400 2000 6e00  n. .W.o.r.t. .n.
+00002cb0: 6100 6300 6800 2000 7200 6500 6300 6800  a.c.h. .r.e.c.h.
+00002cc0: 7400 7300 2000 6500 7200 7700 6500 6900  t.s. .e.r.w.e.i.
+00002cd0: 7400 6500 7200 6e08 0000 0000 0600 0000  t.e.r.n.........
+00002ce0: 1f45 7874 656e 6420 7365 6c65 6374 696f  .Extend selectio
+00002cf0: 6e20 7269 6768 7420 6f6e 6520 776f 7264  n right one word
+00002d00: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+00002d10: 0103 0000 005e 0041 0075 0073 0077 0061  .....^.A.u.s.w.a
+00002d20: 0068 006c 0020 0075 006d 0020 0065 0069  .h.l. .u.m. .e.i
+00002d30: 006e 0065 006e 0020 0057 006f 0072 0074  .n.e.n. .W.o.r.t
+00002d40: 0074 0065 0069 006c 0020 006e 0061 0063  .t.e.i.l. .n.a.c
+00002d50: 0068 0020 0072 0065 0063 0068 0074 0073  .h. .r.e.c.h.t.s
+00002d60: 0020 0065 0072 0077 0065 0069 0074 0065  . .e.r.w.e.i.t.e
+00002d70: 0072 006e 0800 0000 0006 0000 0024 4578  .r.n.........$Ex
+00002d80: 7465 6e64 2073 656c 6563 7469 6f6e 2072  tend selection r
+00002d90: 6967 6874 206f 6e65 2077 6f72 6420 7061  ight one word pa
+00002da0: 7274 0700 0000 0b51 7363 6943 6f6d 6d61  rt.....QsciComma
+00002db0: 6e64 0103 0000 0056 0041 0075 0073 0077  nd.....V.A.u.s.w
+00002dc0: 0061 0068 006c 0020 007a 0075 006d 0020  .a.h.l. .z.u.m. 
+00002dd0: 0045 006e 0064 0065 0020 0064 0065 0072  .E.n.d.e. .d.e.r
+00002de0: 0020 0041 006e 007a 0065 0069 0067 0065  . .A.n.z.e.i.g.e
+00002df0: 007a 0065 0069 006c 0065 0020 0065 0072  .z.e.i.l.e. .e.r
+00002e00: 0077 0065 0069 0074 0065 0072 006e 0800  .w.e.i.t.e.r.n..
+00002e10: 0000 0006 0000 0027 4578 7465 6e64 2073  .......'Extend s
+00002e20: 656c 6563 7469 6f6e 2074 6f20 656e 6420  election to end 
+00002e30: 6f66 2064 6973 706c 6179 206c 696e 6507  of display line.
+00002e40: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00002e50: 0300 0000 9000 5200 6500 6300 6800 7400  ......R.e.c.h.t.
+00002e60: 6500 6300 6b00 6900 6700 6500 2000 4100  e.c.k.i.g.e. .A.
+00002e70: 7500 7300 7700 6100 6800 6c00 2000 7a00  u.s.w.a.h.l. .z.
+00002e80: 7500 6d00 2000 4500 6e00 6400 6500 2000  u.m. .E.n.d.e. .
+00002e90: 6400 6500 7200 2000 4400 6f00 6b00 7500  d.e.r. .D.o.k.u.
+00002ea0: 6d00 6500 6e00 7400 6500 6e00 2d00 2000  m.e.n.t.e.n.-. .
+00002eb0: 6f00 6400 6500 7200 2000 4100 6e00 7a00  o.d.e.r. .A.n.z.
+00002ec0: 6500 6900 6700 6500 7a00 6500 6900 6c00  e.i.g.e.z.e.i.l.
+00002ed0: 6500 2000 6500 7200 7700 6500 6900 7400  e. .e.r.w.e.i.t.
+00002ee0: 6500 7200 6e08 0000 0000 0600 0000 3345  e.r.n.........3E
+00002ef0: 7874 656e 6420 7365 6c65 6374 696f 6e20  xtend selection 
+00002f00: 746f 2065 6e64 206f 6620 6469 7370 6c61  to end of displa
+00002f10: 7920 6f72 2064 6f63 756d 656e 7420 6c69  y or document li
+00002f20: 6e65 0700 0000 0b51 7363 6943 6f6d 6d61  ne.....QsciComma
+00002f30: 6e64 0103 0000 0048 0041 0075 0073 0077  nd.....H.A.u.s.w
+00002f40: 0061 0068 006c 0020 007a 0075 006d 0020  .a.h.l. .z.u.m. 
+00002f50: 0044 006f 006b 0075 006d 0065 006e 0074  .D.o.k.u.m.e.n.t
+00002f60: 0065 006e 0065 006e 0064 0065 0020 0065  .e.n.e.n.d.e. .e
+00002f70: 0072 0077 0065 0069 0074 0065 0072 006e  .r.w.e.i.t.e.r.n
+00002f80: 0800 0000 0006 0000 0023 4578 7465 6e64  .........#Extend
+00002f90: 2073 656c 6563 7469 6f6e 2074 6f20 656e   selection to en
+00002fa0: 6420 6f66 2064 6f63 756d 656e 7407 0000  d of document...
+00002fb0: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
+00002fc0: 0000 5c00 4100 7500 7300 7700 6100 6800  ..\.A.u.s.w.a.h.
+00002fd0: 6c00 2000 7a00 7500 6d00 2000 4500 6e00  l. .z.u.m. .E.n.
+00002fe0: 6400 6500 2000 6400 6500 7200 2000 4400  d.e. .d.e.r. .D.
+00002ff0: 6f00 6b00 7500 6d00 6500 6e00 7400 6500  o.k.u.m.e.n.t.e.
+00003000: 6e00 7a00 6500 6900 6c00 6500 2000 6500  n.z.e.i.l.e. .e.
+00003010: 7200 7700 6500 6900 7400 6500 7200 6e08  r.w.e.i.t.e.r.n.
+00003020: 0000 0000 0600 0000 2845 7874 656e 6420  ........(Extend 
+00003030: 7365 6c65 6374 696f 6e20 746f 2065 6e64  selection to end
+00003040: 206f 6620 646f 6375 6d65 6e74 206c 696e   of document lin
+00003050: 6507 0000 000b 5173 6369 436f 6d6d 616e  e.....QsciComman
+00003060: 6401 0300 0000 6400 4100 7500 7300 7700  d.....d.A.u.s.w.
+00003070: 6100 6800 6c00 2000 6200 6900 7300 2000  a.h.l. .b.i.s. .
+00003080: 7a00 7500 6d00 2000 4500 6e00 6400 6500  z.u.m. .E.n.d.e.
+00003090: 2000 6400 6500 7300 2000 6e00 e400 6300   .d.e.s. .n...c.
+000030a0: 6800 7300 7400 6500 6e00 2000 5700 6f00  h.s.t.e.n. .W.o.
+000030b0: 7200 7400 6500 7300 2000 6500 7200 7700  r.t.e.s. .e.r.w.
+000030c0: 6500 6900 7400 6500 7200 6e08 0000 0000  e.i.t.e.r.n.....
+000030d0: 0600 0000 2445 7874 656e 6420 7365 6c65  ....$Extend sele
+000030e0: 6374 696f 6e20 746f 2065 6e64 206f 6620  ction to end of 
+000030f0: 6e65 7874 2077 6f72 6407 0000 000b 5173  next word.....Qs
+00003100: 6369 436f 6d6d 616e 6401 0300 0000 6200  ciCommand.....b.
+00003110: 4100 7500 7300 7700 6100 6800 6c00 2000  A.u.s.w.a.h.l. .
+00003120: 6200 6900 7300 2000 7a00 7500 6d00 2000  b.i.s. .z.u.m. .
+00003130: 4500 6e00 6400 6500 2000 6400 6500 7300  E.n.d.e. .d.e.s.
+00003140: 2000 7600 6f00 7200 6900 6700 6500 6e00   .v.o.r.i.g.e.n.
+00003150: 2000 5700 6f00 7200 7400 6500 7300 2000   .W.o.r.t.e.s. .
+00003160: 6500 7200 7700 6500 6900 7400 6500 7200  e.r.w.e.i.t.e.r.
+00003170: 6e08 0000 0000 0600 0000 2845 7874 656e  n.........(Exten
+00003180: 6420 7365 6c65 6374 696f 6e20 746f 2065  d selection to e
+00003190: 6e64 206f 6620 7072 6576 696f 7573 2077  nd of previous w
+000031a0: 6f72 6407 0000 000b 5173 6369 436f 6d6d  ord.....QsciComm
+000031b0: 616e 6401 0300 0000 9e00 4100 7500 7300  and.......A.u.s.
+000031c0: 7700 6100 6800 6c00 2000 7a00 7500 6d00  w.a.h.l. .z.u.m.
+000031d0: 2000 6500 7200 7300 7400 6500 6e00 2000   .e.r.s.t.e.n. .
+000031e0: 7300 6900 6300 6800 7400 6200 6100 7200  s.i.c.h.t.b.a.r.
+000031f0: 6500 6e00 2000 5a00 6500 6900 6300 6800  e.n. .Z.e.i.c.h.
+00003200: 6500 6e00 2000 6400 6500 7200 2000 4400  e.n. .d.e.r. .D.
+00003210: 6f00 6b00 7500 6d00 6500 6e00 7400 2d00  o.k.u.m.e.n.t.-.
+00003220: 2000 6f00 6400 6500 7200 2000 4100 6e00   .o.d.e.r. .A.n.
+00003230: 7a00 6500 6900 6700 6500 7a00 6500 6900  z.e.i.g.e.z.e.i.
+00003240: 6c00 6500 2000 6500 7200 7700 6500 6900  l.e. .e.r.w.e.i.
+00003250: 7400 6500 7200 6e08 0000 0000 0600 0000  t.e.r.n.........
+00003260: 4745 7874 656e 6420 7365 6c65 6374 696f  GExtend selectio
+00003270: 6e20 746f 2066 6972 7374 2076 6973 6962  n to first visib
+00003280: 6c65 2063 6861 7261 6374 6572 2069 6e20  le character in 
+00003290: 6469 7370 6c61 7920 6f72 2064 6f63 756d  display or docum
+000032a0: 656e 7420 6c69 6e65 0700 0000 0b51 7363  ent line.....Qsc
+000032b0: 6943 6f6d 6d61 6e64 0103 0000 0082 0041  iCommand.......A
+000032c0: 0075 0073 0077 0061 0068 006c 0020 007a  .u.s.w.a.h.l. .z
+000032d0: 0075 006d 0020 0065 0072 0073 0074 0065  .u.m. .e.r.s.t.e
+000032e0: 006e 0020 0073 0069 0063 0068 0074 0062  .n. .s.i.c.h.t.b
+000032f0: 0061 0072 0065 006e 0020 005a 0065 0069  .a.r.e.n. .Z.e.i
+00003300: 0063 0068 0065 006e 0020 0064 0065 0072  .c.h.e.n. .d.e.r
+00003310: 0020 0044 006f 006b 0075 006d 0065 006e  . .D.o.k.u.m.e.n
+00003320: 0074 007a 0065 0069 006c 0065 0020 0065  .t.z.e.i.l.e. .e
+00003330: 0072 0077 0065 0069 0074 0065 0072 006e  .r.w.e.i.t.e.r.n
+00003340: 0800 0000 0006 0000 003c 4578 7465 6e64  .........<Extend
+00003350: 2073 656c 6563 7469 6f6e 2074 6f20 6669   selection to fi
+00003360: 7273 7420 7669 7369 626c 6520 6368 6172  rst visible char
+00003370: 6163 7465 7220 696e 2064 6f63 756d 656e  acter in documen
+00003380: 7420 6c69 6e65 0700 0000 0b51 7363 6943  t line.....QsciC
+00003390: 6f6d 6d61 6e64 0103 0000 005a 0041 0075  ommand.....Z.A.u
+000033a0: 0073 0077 0061 0068 006c 0020 007a 0075  .s.w.a.h.l. .z.u
+000033b0: 006d 0020 0042 0065 0067 0069 006e 006e  .m. .B.e.g.i.n.n
+000033c0: 0020 0064 0065 0072 0020 0041 006e 007a  . .d.e.r. .A.n.z
+000033d0: 0065 0069 0067 0065 007a 0065 0069 006c  .e.i.g.e.z.e.i.l
+000033e0: 0065 0020 0065 0072 0077 0065 0069 0074  .e. .e.r.w.e.i.t
+000033f0: 0065 0072 006e 0800 0000 0006 0000 0029  .e.r.n.........)
+00003400: 4578 7465 6e64 2073 656c 6563 7469 6f6e  Extend selection
+00003410: 2074 6f20 7374 6172 7420 6f66 2064 6973   to start of dis
+00003420: 706c 6179 206c 696e 6507 0000 000b 5173  play line.....Qs
+00003430: 6369 436f 6d6d 616e 6401 0300 0000 9400  ciCommand.......
+00003440: 5200 6500 6300 6800 7400 6500 6300 6b00  R.e.c.h.t.e.c.k.
+00003450: 6900 6700 6500 2000 4100 7500 7300 7700  i.g.e. .A.u.s.w.
+00003460: 6100 6800 6c00 2000 7a00 7500 6d00 2000  a.h.l. .z.u.m. .
+00003470: 4200 6500 6700 6900 6e00 6e00 2000 6400  B.e.g.i.n.n. .d.
+00003480: 6500 7200 2000 4400 6f00 6b00 7500 6d00  e.r. .D.o.k.u.m.
+00003490: 6500 6e00 7400 6500 6e00 2d00 2000 6f00  e.n.t.e.n.-. .o.
+000034a0: 6400 6500 7200 2000 4100 6e00 7a00 6500  d.e.r. .A.n.z.e.
+000034b0: 6900 6700 6500 7a00 6500 6900 6c00 6500  i.g.e.z.e.i.l.e.
+000034c0: 2000 6500 7200 7700 6500 6900 7400 6500   .e.r.w.e.i.t.e.
+000034d0: 7200 6e08 0000 0000 0600 0000 3545 7874  r.n.........5Ext
+000034e0: 656e 6420 7365 6c65 6374 696f 6e20 746f  end selection to
+000034f0: 2073 7461 7274 206f 6620 6469 7370 6c61   start of displa
+00003500: 7920 6f72 2064 6f63 756d 656e 7420 6c69  y or document li
+00003510: 6e65 0700 0000 0b51 7363 6943 6f6d 6d61  ne.....QsciComma
+00003520: 6e64 0103 0000 004c 0041 0075 0073 0077  nd.....L.A.u.s.w
+00003530: 0061 0068 006c 0020 007a 0075 006d 0020  .a.h.l. .z.u.m. 
+00003540: 0044 006f 006b 0075 006d 0065 006e 0074  .D.o.k.u.m.e.n.t
+00003550: 0065 006e 0061 006e 0066 0061 006e 0067  .e.n.a.n.f.a.n.g
+00003560: 0020 0065 0072 0077 0065 0069 0074 0065  . .e.r.w.e.i.t.e
+00003570: 0072 006e 0800 0000 0006 0000 0025 4578  .r.n.........%Ex
+00003580: 7465 6e64 2073 656c 6563 7469 6f6e 2074  tend selection t
+00003590: 6f20 7374 6172 7420 6f66 2064 6f63 756d  o start of docum
+000035a0: 656e 7407 0000 000b 5173 6369 436f 6d6d  ent.....QsciComm
+000035b0: 616e 6401 0300 0000 6000 4100 7500 7300  and.....`.A.u.s.
+000035c0: 7700 6100 6800 6c00 2000 7a00 7500 6d00  w.a.h.l. .z.u.m.
+000035d0: 2000 4200 6500 6700 6900 6e00 6e00 2000   .B.e.g.i.n.n. .
+000035e0: 6400 6500 7200 2000 4400 6f00 6b00 7500  d.e.r. .D.o.k.u.
+000035f0: 6d00 6500 6e00 7400 6500 6e00 7a00 6500  m.e.n.t.e.n.z.e.
+00003600: 6900 6c00 6500 2000 6500 7200 7700 6500  i.l.e. .e.r.w.e.
+00003610: 6900 7400 6500 7200 6e08 0000 0000 0600  i.t.e.r.n.......
+00003620: 0000 2a45 7874 656e 6420 7365 6c65 6374  ..*Extend select
+00003630: 696f 6e20 746f 2073 7461 7274 206f 6620  ion to start of 
+00003640: 646f 6375 6d65 6e74 206c 696e 6507 0000  document line...
+00003650: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
+00003660: 0000 5200 4100 7500 7300 7700 6100 6800  ..R.A.u.s.w.a.h.
+00003670: 6c00 2000 7500 6d00 2000 6500 6900 6e00  l. .u.m. .e.i.n.
+00003680: 6500 2000 5a00 6500 6900 6c00 6500 2000  e. .Z.e.i.l.e. .
+00003690: 6e00 6100 6300 6800 2000 6f00 6200 6500  n.a.c.h. .o.b.e.
+000036a0: 6e00 2000 6500 7200 7700 6500 6900 7400  n. .e.r.w.e.i.t.
+000036b0: 6500 7200 6e08 0000 0000 0600 0000 1c45  e.r.n..........E
+000036c0: 7874 656e 6420 7365 6c65 6374 696f 6e20  xtend selection 
+000036d0: 7570 206f 6e65 206c 696e 6507 0000 000b  up one line.....
+000036e0: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+000036f0: 5200 4100 7500 7300 7700 6100 6800 6c00  R.A.u.s.w.a.h.l.
+00003700: 2000 7500 6d00 2000 6500 6900 6e00 6500   .u.m. .e.i.n.e.
+00003710: 2000 5300 6500 6900 7400 6500 2000 6e00   .S.e.i.t.e. .n.
+00003720: 6100 6300 6800 2000 6f00 6200 6500 6e00  a.c.h. .o.b.e.n.
+00003730: 2000 6500 7200 7700 6500 6900 7400 6500   .e.r.w.e.i.t.e.
+00003740: 7200 6e08 0000 0000 0600 0000 1c45 7874  r.n..........Ext
+00003750: 656e 6420 7365 6c65 6374 696f 6e20 7570  end selection up
+00003760: 206f 6e65 2070 6167 6507 0000 000b 5173   one page.....Qs
+00003770: 6369 436f 6d6d 616e 6401 0300 0000 5600  ciCommand.....V.
+00003780: 4100 7500 7300 7700 6100 6800 6c00 2000  A.u.s.w.a.h.l. .
+00003790: 7500 6d00 2000 6500 6900 6e00 6500 6e00  u.m. .e.i.n.e.n.
+000037a0: 2000 4100 6200 7300 6100 7400 7a00 2000   .A.b.s.a.t.z. .
+000037b0: 6e00 6100 6300 6800 2000 6f00 6200 6500  n.a.c.h. .o.b.e.
+000037c0: 6e00 2000 6500 7200 7700 6500 6900 7400  n. .e.r.w.e.i.t.
+000037d0: 6500 7200 6e08 0000 0000 0600 0000 2145  e.r.n.........!E
+000037e0: 7874 656e 6420 7365 6c65 6374 696f 6e20  xtend selection 
+000037f0: 7570 206f 6e65 2070 6172 6167 7261 7068  up one paragraph
+00003800: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+00003810: 0103 0000 001a 0053 0065 0069 0074 0065  .......S.e.i.t.e
+00003820: 006e 0075 006d 0062 0072 0075 0063 0068  .n.u.m.b.r.u.c.h
+00003830: 0800 0000 0006 0000 0008 466f 726d 6665  ..........Formfe
+00003840: 6564 0700 0000 0b51 7363 6943 6f6d 6d61  ed.....QsciComma
+00003850: 6e64 0103 0000 0028 0045 0069 006e 0065  nd.....(.E.i.n.e
+00003860: 0020 0045 0062 0065 006e 0065 0020 0065  . .E.b.e.n.e. .e
+00003870: 0069 006e 0072 00fc 0063 006b 0065 006e  .i.n.r...c.k.e.n
+00003880: 0800 0000 0006 0000 0010 496e 6465 6e74  ..........Indent
+00003890: 206f 6e65 206c 6576 656c 0700 0000 0b51   one level.....Q
+000038a0: 7363 6943 6f6d 6d61 6e64 0103 0000 0026  sciCommand.....&
+000038b0: 004e 0065 0075 0065 0020 005a 0065 0069  .N.e.u.e. .Z.e.i
+000038c0: 006c 0065 0020 0065 0069 006e 0066 00fc  .l.e. .e.i.n.f..
+000038d0: 0067 0065 006e 0800 0000 0006 0000 000e  .g.e.n..........
+000038e0: 496e 7365 7274 206e 6577 6c69 6e65 0700  Insert newline..
+000038f0: 0000 0b51 7363 6943 6f6d 6d61 6e64 0103  ...QsciCommand..
+00003900: 0000 002a 0045 0069 006e 0065 0020 005a  ...*.E.i.n.e. .Z
+00003910: 0065 0069 006c 0065 0020 006e 0061 0063  .e.i.l.e. .n.a.c
+00003920: 0068 0020 0075 006e 0074 0065 006e 0800  .h. .u.n.t.e.n..
+00003930: 0000 0006 0000 0012 4d6f 7665 2064 6f77  ........Move dow
+00003940: 6e20 6f6e 6520 6c69 6e65 0700 0000 0b51  n one line.....Q
+00003950: 7363 6943 6f6d 6d61 6e64 0103 0000 002a  sciCommand.....*
+00003960: 0045 0069 006e 0065 0020 0053 0065 0069  .E.i.n.e. .S.e.i
+00003970: 0074 0065 0020 006e 0061 0063 0068 0020  .t.e. .n.a.c.h. 
+00003980: 0075 006e 0074 0065 006e 0800 0000 0006  .u.n.t.e.n......
+00003990: 0000 0012 4d6f 7665 2064 6f77 6e20 6f6e  ....Move down on
+000039a0: 6520 7061 6765 0700 0000 0b51 7363 6943  e page.....QsciC
+000039b0: 6f6d 6d61 6e64 0103 0000 002e 0045 0069  ommand.......E.i
+000039c0: 006e 0065 006e 0020 0041 0062 0073 0061  .n.e.n. .A.b.s.a
+000039d0: 0074 007a 0020 006e 0061 0063 0068 0020  .t.z. .n.a.c.h. 
+000039e0: 0075 006e 0074 0065 006e 0800 0000 0006  .u.n.t.e.n......
+000039f0: 0000 0017 4d6f 7665 2064 6f77 6e20 6f6e  ....Move down on
+00003a00: 6520 7061 7261 6772 6170 6807 0000 000b  e paragraph.....
+00003a10: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00003a20: 2c00 4500 6900 6e00 2000 5a00 6500 6900  ,.E.i.n. .Z.e.i.
+00003a30: 6300 6800 6500 6e00 2000 6e00 6100 6300  c.h.e.n. .n.a.c.
+00003a40: 6800 2000 6c00 6900 6e00 6b00 7308 0000  h. .l.i.n.k.s...
+00003a50: 0000 0600 0000 174d 6f76 6520 6c65 6674  .......Move left
+00003a60: 206f 6e65 2063 6861 7261 6374 6572 0700   one character..
+00003a70: 0000 0b51 7363 6943 6f6d 6d61 6e64 0103  ...QsciCommand..
+00003a80: 0000 0026 0045 0069 006e 0020 0057 006f  ...&.E.i.n. .W.o
+00003a90: 0072 0074 0020 006e 0061 0063 0068 0020  .r.t. .n.a.c.h. 
+00003aa0: 006c 0069 006e 006b 0073 0800 0000 0006  .l.i.n.k.s......
+00003ab0: 0000 0012 4d6f 7665 206c 6566 7420 6f6e  ....Move left on
+00003ac0: 6520 776f 7264 0700 0000 0b51 7363 6943  e word.....QsciC
+00003ad0: 6f6d 6d61 6e64 0103 0000 002e 0045 0069  ommand.......E.i
+00003ae0: 006e 0020 0057 006f 0072 0074 0074 0065  .n. .W.o.r.t.t.e
+00003af0: 0069 006c 0020 006e 0061 0063 0068 0020  .i.l. .n.a.c.h. 
+00003b00: 006c 0069 006e 006b 0073 0800 0000 0006  .l.i.n.k.s......
+00003b10: 0000 0017 4d6f 7665 206c 6566 7420 6f6e  ....Move left on
+00003b20: 6520 776f 7264 2070 6172 7407 0000 000b  e word part.....
+00003b30: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00003b40: 2e00 4500 6900 6e00 2000 5a00 6500 6900  ..E.i.n. .Z.e.i.
+00003b50: 6300 6800 6500 6e00 2000 6e00 6100 6300  c.h.e.n. .n.a.c.
+00003b60: 6800 2000 7200 6500 6300 6800 7400 7308  h. .r.e.c.h.t.s.
+00003b70: 0000 0000 0600 0000 184d 6f76 6520 7269  .........Move ri
+00003b80: 6768 7420 6f6e 6520 6368 6172 6163 7465  ght one characte
+00003b90: 7207 0000 000b 5173 6369 436f 6d6d 616e  r.....QsciComman
+00003ba0: 6401 0300 0000 2800 4500 6900 6e00 2000  d.....(.E.i.n. .
+00003bb0: 5700 6f00 7200 7400 2000 6e00 6100 6300  W.o.r.t. .n.a.c.
+00003bc0: 6800 2000 7200 6500 6300 6800 7400 7308  h. .r.e.c.h.t.s.
+00003bd0: 0000 0000 0600 0000 134d 6f76 6520 7269  .........Move ri
+00003be0: 6768 7420 6f6e 6520 776f 7264 0700 0000  ght one word....
+00003bf0: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+00003c00: 0030 0045 0069 006e 0020 0057 006f 0072  .0.E.i.n. .W.o.r
+00003c10: 0074 0074 0065 0069 006c 0020 006e 0061  .t.t.e.i.l. .n.a
+00003c20: 0063 0068 0020 0072 0065 0063 0068 0074  .c.h. .r.e.c.h.t
+00003c30: 0073 0800 0000 0006 0000 0018 4d6f 7665  .s..........Move
+00003c40: 2072 6967 6874 206f 6e65 2077 6f72 6420   right one word 
+00003c50: 7061 7274 0700 0000 0b51 7363 6943 6f6d  part.....QsciCom
+00003c60: 6d61 6e64 0103 0000 0056 0041 0075 0073  mand.....V.A.u.s
+00003c70: 0067 0065 0077 00e4 0068 006c 0074 0065  .g.e.w...h.l.t.e
+00003c80: 0020 005a 0065 0069 006c 0065 006e 0020  . .Z.e.i.l.e.n. 
+00003c90: 0075 006d 0020 0065 0069 006e 0065 0020  .u.m. .e.i.n.e. 
+00003ca0: 005a 0065 0069 006c 0065 0020 006e 0061  .Z.e.i.l.e. .n.a
+00003cb0: 0063 0068 0020 0075 006e 0074 0065 006e  .c.h. .u.n.t.e.n
+00003cc0: 0800 0000 0006 0000 0021 4d6f 7665 2073  .........!Move s
+00003cd0: 656c 6563 7465 6420 6c69 6e65 7320 646f  elected lines do
+00003ce0: 776e 206f 6e65 206c 696e 6507 0000 000b  wn one line.....
+00003cf0: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00003d00: 5400 4100 7500 7300 6700 6500 7700 e400  T.A.u.s.g.e.w...
+00003d10: 6800 6c00 7400 6500 2000 5a00 6500 6900  h.l.t.e. .Z.e.i.
+00003d20: 6c00 6500 6e00 2000 7500 6d00 2000 6500  l.e.n. .u.m. .e.
+00003d30: 6900 6e00 6500 2000 5a00 6500 6900 6c00  i.n.e. .Z.e.i.l.
+00003d40: 6500 2000 6e00 6100 6300 6800 2000 6f00  e. .n.a.c.h. .o.
+00003d50: 6200 6500 6e08 0000 0000 0600 0000 1f4d  b.e.n..........M
+00003d60: 6f76 6520 7365 6c65 6374 6564 206c 696e  ove selected lin
+00003d70: 6573 2075 7020 6f6e 6520 6c69 6e65 0700  es up one line..
+00003d80: 0000 0b51 7363 6943 6f6d 6d61 6e64 0103  ...QsciCommand..
+00003d90: 0000 0044 005a 0075 006d 0020 0045 006e  ...D.Z.u.m. .E.n
+00003da0: 0064 0065 0020 0064 0065 0072 0020 0041  .d.e. .d.e.r. .A
+00003db0: 006e 007a 0065 0069 0067 0065 007a 0065  .n.z.e.i.g.e.z.e
+00003dc0: 0069 006c 0065 0020 0073 0070 0072 0069  .i.l.e. .s.p.r.i
+00003dd0: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
+00003de0: 001b 4d6f 7665 2074 6f20 656e 6420 6f66  ..Move to end of
+00003df0: 2064 6973 706c 6179 206c 696e 6507 0000   display line...
+00003e00: 000b 5173 6369 436f 6d6d 616e 6401 0300  ..QsciCommand...
+00003e10: 0000 6600 5a00 7500 6d00 2000 4500 6e00  ..f.Z.u.m. .E.n.
+00003e20: 6400 6500 2000 6400 6500 7200 2000 4400  d.e. .d.e.r. .D.
+00003e30: 6f00 6b00 7500 6d00 6500 6e00 7400 6500  o.k.u.m.e.n.t.e.
+00003e40: 6e00 2d00 2000 6f00 6400 6500 7200 2000  n.-. .o.d.e.r. .
+00003e50: 4100 6e00 7a00 6500 6900 6700 6500 7a00  A.n.z.e.i.g.e.z.
+00003e60: 6500 6900 6c00 6500 2000 7300 7000 7200  e.i.l.e. .s.p.r.
+00003e70: 6900 6e00 6700 6500 6e08 0000 0000 0600  i.n.g.e.n.......
+00003e80: 0000 274d 6f76 6520 746f 2065 6e64 206f  ..'Move to end o
+00003e90: 6620 6469 7370 6c61 7920 6f72 2064 6f63  f display or doc
+00003ea0: 756d 656e 7420 6c69 6e65 0700 0000 0b51  ument line.....Q
+00003eb0: 7363 6943 6f6d 6d61 6e64 0103 0000 0036  sciCommand.....6
+00003ec0: 005a 0075 006d 0020 0044 006f 006b 0075  .Z.u.m. .D.o.k.u
+00003ed0: 006d 0065 006e 0074 0065 006e 0065 006e  .m.e.n.t.e.n.e.n
+00003ee0: 0064 0065 0020 0073 0070 0072 0069 006e  .d.e. .s.p.r.i.n
+00003ef0: 0067 0065 006e 0800 0000 0006 0000 0017  .g.e.n..........
+00003f00: 4d6f 7665 2074 6f20 656e 6420 6f66 2064  Move to end of d
+00003f10: 6f63 756d 656e 7407 0000 000b 5173 6369  ocument.....Qsci
+00003f20: 436f 6d6d 616e 6401 0300 0000 4600 5a00  Command.....F.Z.
+00003f30: 7500 6d00 2000 4500 6e00 6400 6500 2000  u.m. .E.n.d.e. .
+00003f40: 6400 6500 7200 2000 4400 6f00 6b00 7500  d.e.r. .D.o.k.u.
+00003f50: 6d00 6500 6e00 7400 7a00 6500 6900 6c00  m.e.n.t.z.e.i.l.
+00003f60: 6500 2000 7300 7000 7200 6900 6e00 6700  e. .s.p.r.i.n.g.
+00003f70: 6500 6e08 0000 0000 0600 0000 1c4d 6f76  e.n..........Mov
+00003f80: 6520 746f 2065 6e64 206f 6620 646f 6375  e to end of docu
+00003f90: 6d65 6e74 206c 696e 6507 0000 000b 5173  ment line.....Qs
+00003fa0: 6369 436f 6d6d 616e 6401 0300 0000 4a00  ciCommand.....J.
+00003fb0: 5a00 7500 6d00 2000 4500 6e00 6400 6500  Z.u.m. .E.n.d.e.
+00003fc0: 2000 6400 6500 7300 2000 6e00 e400 6300   .d.e.s. .n...c.
+00003fd0: 6800 7300 7400 6500 6e00 2000 5700 6f00  h.s.t.e.n. .W.o.
+00003fe0: 7200 7400 6500 7300 2000 7300 7000 7200  r.t.e.s. .s.p.r.
+00003ff0: 6900 6e00 6700 6500 6e08 0000 0000 0600  i.n.g.e.n.......
+00004000: 0000 184d 6f76 6520 746f 2065 6e64 206f  ...Move to end o
+00004010: 6620 6e65 7874 2077 6f72 6407 0000 000b  f next word.....
+00004020: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00004030: 4800 5a00 7500 6d00 2000 4500 6e00 6400  H.Z.u.m. .E.n.d.
+00004040: 6500 2000 6400 6500 7300 2000 7600 6f00  e. .d.e.s. .v.o.
+00004050: 7200 6900 6700 6500 6e00 2000 5700 6f00  r.i.g.e.n. .W.o.
+00004060: 7200 7400 6500 7300 2000 7300 7000 7200  r.t.e.s. .s.p.r.
+00004070: 6900 6e00 6700 6500 6e08 0000 0000 0600  i.n.g.e.n.......
+00004080: 0000 1c4d 6f76 6520 746f 2065 6e64 206f  ...Move to end o
+00004090: 6620 7072 6576 696f 7573 2077 6f72 6407  f previous word.
+000040a0: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+000040b0: 0300 0000 7000 5a00 7500 6d00 2000 6500  ....p.Z.u.m. .e.
+000040c0: 7200 7300 7400 6500 6e00 2000 7300 6900  r.s.t.e.n. .s.i.
+000040d0: 6300 6800 7400 6200 6100 7200 6500 6e00  c.h.t.b.a.r.e.n.
+000040e0: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
+000040f0: 2000 6400 6500 7200 2000 4400 6f00 6b00   .d.e.r. .D.o.k.
+00004100: 7500 6d00 6500 6e00 7400 7a00 6500 6900  u.m.e.n.t.z.e.i.
+00004110: 6c00 6500 2000 7300 7000 7200 6900 6e00  l.e. .s.p.r.i.n.
+00004120: 6700 6500 6e08 0000 0000 0600 0000 304d  g.e.n.........0M
+00004130: 6f76 6520 746f 2066 6972 7374 2076 6973  ove to first vis
+00004140: 6962 6c65 2063 6861 7261 6374 6572 2069  ible character i
+00004150: 6e20 646f 6375 6d65 6e74 206c 696e 6507  n document line.
+00004160: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00004170: 0300 0000 7200 5a00 7500 6d00 2000 6500  ....r.Z.u.m. .e.
+00004180: 7200 7300 7400 6500 6e00 2000 6100 6e00  r.s.t.e.n. .a.n.
+00004190: 6700 6500 7a00 6500 6900 6700 7400 6500  g.e.z.e.i.g.t.e.
+000041a0: 6e00 2000 5a00 6500 6900 6300 6800 6500  n. .Z.e.i.c.h.e.
+000041b0: 6e00 2000 6400 6500 7200 2000 4400 6f00  n. .d.e.r. .D.o.
+000041c0: 6b00 7500 6d00 6500 6e00 7400 7a00 6500  k.u.m.e.n.t.z.e.
+000041d0: 6900 6c00 6500 2000 7300 7000 7200 6900  i.l.e. .s.p.r.i.
+000041e0: 6e00 6700 6500 6e08 0000 0000 0600 0000  n.g.e.n.........
+000041f0: 3b4d 6f76 6520 746f 2066 6972 7374 2076  ;Move to first v
+00004200: 6973 6962 6c65 2063 6861 7261 6374 6572  isible character
+00004210: 206f 6620 6469 7370 6c61 7920 696e 2064   of display in d
+00004220: 6f63 756d 656e 7420 6c69 6e65 0700 0000  ocument line....
+00004230: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+00004240: 0048 005a 0075 006d 0020 0042 0065 0067  .H.Z.u.m. .B.e.g
+00004250: 0069 006e 006e 0020 0064 0065 0072 0020  .i.n.n. .d.e.r. 
+00004260: 0041 006e 007a 0065 0069 0067 0065 007a  .A.n.z.e.i.g.e.z
+00004270: 0065 0069 006c 0065 0020 0073 0070 0072  .e.i.l.e. .s.p.r
+00004280: 0069 006e 0067 0065 006e 0800 0000 0006  .i.n.g.e.n......
+00004290: 0000 001d 4d6f 7665 2074 6f20 7374 6172  ....Move to star
+000042a0: 7420 6f66 2064 6973 706c 6179 206c 696e  t of display lin
+000042b0: 6507 0000 000b 5173 6369 436f 6d6d 616e  e.....QsciComman
+000042c0: 6401 0300 0000 6a00 5a00 7500 6d00 2000  d.....j.Z.u.m. .
+000042d0: 4200 6500 6700 6900 6e00 6e00 2000 6400  B.e.g.i.n.n. .d.
+000042e0: 6500 7200 2000 4400 6f00 6b00 7500 6d00  e.r. .D.o.k.u.m.
+000042f0: 6500 6e00 7400 6500 6e00 2d00 2000 6f00  e.n.t.e.n.-. .o.
+00004300: 6400 6500 7200 2000 4100 6e00 7a00 6500  d.e.r. .A.n.z.e.
+00004310: 6900 6700 6500 7a00 6500 6900 6c00 6500  i.g.e.z.e.i.l.e.
+00004320: 2000 7300 7000 7200 6900 6e00 6700 6500   .s.p.r.i.n.g.e.
+00004330: 6e08 0000 0000 0600 0000 294d 6f76 6520  n.........)Move 
+00004340: 746f 2073 7461 7274 206f 6620 6469 7370  to start of disp
+00004350: 6c61 7920 6f72 2064 6f63 756d 656e 7420  lay or document 
+00004360: 6c69 6e65 0700 0000 0b51 7363 6943 6f6d  line.....QsciCom
+00004370: 6d61 6e64 0103 0000 003a 005a 0075 006d  mand.....:.Z.u.m
+00004380: 0020 0044 006f 006b 0075 006d 0065 006e  . .D.o.k.u.m.e.n
+00004390: 0074 0065 006e 0061 006e 0066 0061 006e  .t.e.n.a.n.f.a.n
+000043a0: 0067 0020 0073 0070 0072 0069 006e 0067  .g. .s.p.r.i.n.g
+000043b0: 0065 006e 0800 0000 0006 0000 0019 4d6f  .e.n..........Mo
+000043c0: 7665 2074 6f20 7374 6172 7420 6f66 2064  ve to start of d
+000043d0: 6f63 756d 656e 7407 0000 000b 5173 6369  ocument.....Qsci
+000043e0: 436f 6d6d 616e 6401 0300 0000 4e00 5a00  Command.....N.Z.
+000043f0: 7500 6d00 2000 4200 6500 6700 6900 6e00  u.m. .B.e.g.i.n.
+00004400: 6e00 2000 6400 6500 7200 2000 4400 6f00  n. .d.e.r. .D.o.
+00004410: 6b00 7500 6d00 6500 6e00 7400 6500 6e00  k.u.m.e.n.t.e.n.
+00004420: 7a00 6500 6900 6c00 6500 2000 7300 7000  z.e.i.l.e. .s.p.
+00004430: 7200 6900 6e00 6700 6500 6e08 0000 0000  r.i.n.g.e.n.....
+00004440: 0600 0000 1e4d 6f76 6520 746f 2073 7461  .....Move to sta
+00004450: 7274 206f 6620 646f 6375 6d65 6e74 206c  rt of document l
+00004460: 696e 6507 0000 000b 5173 6369 436f 6d6d  ine.....QsciComm
+00004470: 616e 6401 0300 0000 2800 4500 6900 6e00  and.....(.E.i.n.
+00004480: 6500 2000 5a00 6500 6900 6c00 6500 2000  e. .Z.e.i.l.e. .
+00004490: 6e00 6100 6300 6800 2000 6f00 6200 6500  n.a.c.h. .o.b.e.
+000044a0: 6e08 0000 0000 0600 0000 104d 6f76 6520  n..........Move 
+000044b0: 7570 206f 6e65 206c 696e 6507 0000 000b  up one line.....
+000044c0: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+000044d0: 1e00 4500 6900 6e00 6500 2000 5300 6500  ..E.i.n.e. .S.e.
+000044e0: 6900 7400 6500 2000 6800 6f00 6300 6808  i.t.e. .h.o.c.h.
+000044f0: 0000 0000 0600 0000 104d 6f76 6520 7570  .........Move up
+00004500: 206f 6e65 2070 6167 6507 0000 000b 5173   one page.....Qs
+00004510: 6369 436f 6d6d 616e 6401 0300 0000 2c00  ciCommand.....,.
+00004520: 4500 6900 6e00 6500 6e00 2000 4100 6200  E.i.n.e.n. .A.b.
+00004530: 7300 6100 7400 7a00 2000 6e00 6100 6300  s.a.t.z. .n.a.c.
+00004540: 6800 2000 6f00 6200 6500 6e08 0000 0000  h. .o.b.e.n.....
+00004550: 0600 0000 154d 6f76 6520 7570 206f 6e65  .....Move up one
+00004560: 2070 6172 6167 7261 7068 0700 0000 0b51   paragraph.....Q
+00004570: 7363 6943 6f6d 6d61 6e64 0103 0000 0010  sciCommand......
+00004580: 0045 0069 006e 0066 00fc 0067 0065 006e  .E.i.n.f...g.e.n
+00004590: 0800 0000 0006 0000 0005 5061 7374 6507  ..........Paste.
+000045a0: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+000045b0: 0300 0000 3400 4c00 6500 7400 7a00 7400  ....4.L.e.t.z.t.
+000045c0: 6500 6e00 2000 4200 6500 6600 6500 6800  e.n. .B.e.f.e.h.
+000045d0: 6c00 2000 7700 6900 6500 6400 6500 7200  l. .w.i.e.d.e.r.
+000045e0: 6800 6f00 6c00 6500 6e08 0000 0000 0600  h.o.l.e.n.......
+000045f0: 0000 1152 6564 6f20 6c61 7374 2063 6f6d  ...Redo last com
+00004600: 6d61 6e64 0700 0000 0b51 7363 6943 6f6d  mand.....QsciCom
+00004610: 6d61 6e64 0103 0000 0032 005a 0075 006d  mand.....2.Z.u.m
+00004620: 0020 0044 006f 006b 0075 006d 0065 006e  . .D.o.k.u.m.e.n
+00004630: 0074 0065 006e 0065 006e 0064 0065 0020  .t.e.n.e.n.d.e. 
+00004640: 0072 006f 006c 006c 0065 006e 0800 0000  .r.o.l.l.e.n....
+00004650: 0006 0000 0019 5363 726f 6c6c 2074 6f20  ......Scroll to 
+00004660: 656e 6420 6f66 2064 6f63 756d 656e 7407  end of document.
+00004670: 0000 000b 5173 6369 436f 6d6d 616e 6401  ....QsciCommand.
+00004680: 0300 0000 3600 5a00 7500 6d00 2000 4400  ....6.Z.u.m. .D.
+00004690: 6f00 6b00 7500 6d00 6500 6e00 7400 6500  o.k.u.m.e.n.t.e.
+000046a0: 6e00 6100 6e00 6600 6100 6e00 6700 2000  n.a.n.f.a.n.g. .
+000046b0: 7200 6f00 6c00 6c00 6500 6e08 0000 0000  r.o.l.l.e.n.....
+000046c0: 0600 0000 1b53 6372 6f6c 6c20 746f 2073  .....Scroll to s
+000046d0: 7461 7274 206f 6620 646f 6375 6d65 6e74  tart of document
+000046e0: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+000046f0: 0103 0000 0060 0056 0065 0072 0074 0069  .....`.V.e.r.t.i
+00004700: 0063 0061 006c 0020 0072 006f 006c 006c  .c.a.l. .r.o.l.l
+00004710: 0065 006e 002c 0020 0075 006d 0020 0061  .e.n.,. .u.m. .a
+00004720: 006b 0074 0075 0065 006c 006c 0065 0020  .k.t.u.e.l.l.e. 
+00004730: 005a 0065 0069 006c 0065 0020 007a 0075  .Z.e.i.l.e. .z.u
+00004740: 0020 007a 0065 006e 0074 0072 0069 0065  . .z.e.n.t.r.i.e
+00004750: 0072 0065 006e 0800 0000 0006 0000 0028  .r.e.n.........(
+00004760: 5363 726f 6c6c 2076 6572 7469 6361 6c6c  Scroll verticall
+00004770: 7920 746f 2063 656e 7472 6520 6375 7272  y to centre curr
+00004780: 656e 7420 6c69 6e65 0700 0000 0b51 7363  ent line.....Qsc
+00004790: 6943 6f6d 6d61 6e64 0103 0000 0038 0045  iCommand.....8.E
+000047a0: 0069 006e 0065 0020 005a 0065 0069 006c  .i.n.e. .Z.e.i.l
+000047b0: 0065 0020 006e 0061 0063 0068 0020 0075  .e. .n.a.c.h. .u
+000047c0: 006e 0074 0065 006e 0020 0072 006f 006c  .n.t.e.n. .r.o.l
+000047d0: 006c 0065 006e 0800 0000 0006 0000 0019  .l.e.n..........
+000047e0: 5363 726f 6c6c 2076 6965 7720 646f 776e  Scroll view down
+000047f0: 206f 6e65 206c 696e 6507 0000 000b 5173   one line.....Qs
+00004800: 6369 436f 6d6d 616e 6401 0300 0000 3600  ciCommand.....6.
+00004810: 4500 6900 6e00 6500 2000 5a00 6500 6900  E.i.n.e. .Z.e.i.
+00004820: 6c00 6500 2000 6e00 6100 6300 6800 2000  l.e. .n.a.c.h. .
+00004830: 6f00 6200 6500 6e00 2000 7200 6f00 6c00  o.b.e.n. .r.o.l.
+00004840: 6c00 6500 6e08 0000 0000 0600 0000 1753  l.e.n..........S
+00004850: 6372 6f6c 6c20 7669 6577 2075 7020 6f6e  croll view up on
+00004860: 6520 6c69 6e65 0700 0000 0b51 7363 6943  e line.....QsciC
+00004870: 6f6d 6d61 6e64 0103 0000 001c 0041 006c  ommand.......A.l
+00004880: 006c 0065 0020 0061 0075 0073 0077 00e4  .l.e. .a.u.s.w..
+00004890: 0068 006c 0065 006e 0800 0000 0006 0000  .h.l.e.n........
+000048a0: 000a 5365 6c65 6374 2061 6c6c 0700 0000  ..Select all....
+000048b0: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+000048c0: 006c 0041 0075 0073 0077 0061 0068 006c  .l.A.u.s.w.a.h.l
+000048d0: 0020 0022 0073 0074 006f 0074 0074 0065  . .".s.t.o.t.t.e
+000048e0: 0072 006e 0064 0022 0020 0075 006d 0020  .r.n.d.". .u.m. 
+000048f0: 0065 0069 006e 0065 0020 0053 0065 0069  .e.i.n.e. .S.e.i
+00004900: 0074 0065 0020 006e 0061 0063 0068 0020  .t.e. .n.a.c.h. 
+00004910: 0075 006e 0074 0065 006e 0020 0065 0072  .u.n.t.e.n. .e.r
+00004920: 0077 0065 0069 0074 0065 0072 006e 0800  .w.e.i.t.e.r.n..
+00004930: 0000 0006 0000 0028 5374 7574 7465 7265  .......(Stuttere
+00004940: 6420 6578 7465 6e64 2073 656c 6563 7469  d extend selecti
+00004950: 6f6e 2064 6f77 6e20 6f6e 6520 7061 6765  on down one page
+00004960: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+00004970: 0103 0000 006a 0041 0075 0073 0077 0061  .....j.A.u.s.w.a
+00004980: 0068 006c 0020 0022 0073 0074 006f 0074  .h.l. .".s.t.o.t
+00004990: 0074 0065 0072 006e 0064 0022 0020 0075  .t.e.r.n.d.". .u
+000049a0: 006d 0020 0065 0069 006e 0065 0020 0053  .m. .e.i.n.e. .S
+000049b0: 0065 0069 0074 0065 0020 006e 0061 0063  .e.i.t.e. .n.a.c
+000049c0: 0068 0020 006f 0062 0065 006e 0020 0065  .h. .o.b.e.n. .e
+000049d0: 0072 0077 0065 0069 0074 0065 0072 006e  .r.w.e.i.t.e.r.n
+000049e0: 0800 0000 0006 0000 0026 5374 7574 7465  .........&Stutte
+000049f0: 7265 6420 6578 7465 6e64 2073 656c 6563  red extend selec
+00004a00: 7469 6f6e 2075 7020 6f6e 6520 7061 6765  tion up one page
+00004a10: 0700 0000 0b51 7363 6943 6f6d 6d61 6e64  .....QsciCommand
+00004a20: 0103 0000 0048 0022 0053 0074 006f 0074  .....H.".S.t.o.t
+00004a30: 0074 0065 0072 006e 0064 0022 0020 0075  .t.e.r.n.d.". .u
+00004a40: 006d 0020 0065 0069 006e 0065 0020 0053  .m. .e.i.n.e. .S
+00004a50: 0065 0069 0074 0065 0020 006e 0061 0063  .e.i.t.e. .n.a.c
+00004a60: 0068 0020 0075 006e 0074 0065 006e 0800  .h. .u.n.t.e.n..
+00004a70: 0000 0006 0000 001c 5374 7574 7465 7265  ........Stuttere
+00004a80: 6420 6d6f 7665 2064 6f77 6e20 6f6e 6520  d move down one 
+00004a90: 7061 6765 0700 0000 0b51 7363 6943 6f6d  page.....QsciCom
+00004aa0: 6d61 6e64 0103 0000 0046 0022 0053 0074  mand.....F.".S.t
+00004ab0: 006f 0074 0074 0065 0072 006e 0064 0022  .o.t.t.e.r.n.d."
+00004ac0: 0020 0075 006d 0020 0065 0069 006e 0065  . .u.m. .e.i.n.e
+00004ad0: 0020 0053 0065 0069 0074 0065 0020 006e  . .S.e.i.t.e. .n
+00004ae0: 0061 0063 0068 0020 006f 0062 0065 006e  .a.c.h. .o.b.e.n
+00004af0: 0800 0000 0006 0000 001a 5374 7574 7465  ..........Stutte
+00004b00: 7265 6420 6d6f 7665 2075 7020 6f6e 6520  red move up one 
+00004b10: 7061 6765 0700 0000 0b51 7363 6943 6f6d  page.....QsciCom
+00004b20: 6d61 6e64 0103 0000 0042 0045 0069 006e  mand.....B.E.i.n
+00004b30: 0066 00fc 0067 0065 006e 002f 00dc 0062  .f...g.e.n./...b
+00004b40: 0065 0072 0073 0063 0068 0072 0065 0069  .e.r.s.c.h.r.e.i
+00004b50: 0062 0065 006e 0020 0075 006d 0073 0063  .b.e.n. .u.m.s.c
+00004b60: 0068 0061 006c 0074 0065 006e 0800 0000  .h.a.l.t.e.n....
+00004b70: 0006 0000 0016 546f 6767 6c65 2069 6e73  ......Toggle ins
+00004b80: 6572 742f 6f76 6572 7479 7065 0700 0000  ert/overtype....
+00004b90: 0b51 7363 6943 6f6d 6d61 6e64 0103 0000  .QsciCommand....
+00004ba0: 004a 0041 006b 0074 0075 0065 006c 006c  .J.A.k.t.u.e.l.l
+00004bb0: 0065 0020 0075 006e 0064 0020 0076 006f  .e. .u.n.d. .v.o
+00004bc0: 0072 0068 0065 0072 0069 0067 0065 0020  .r.h.e.r.i.g.e. 
+00004bd0: 005a 0065 0069 006c 0065 0020 0074 0061  .Z.e.i.l.e. .t.a
+00004be0: 0075 0073 0063 0068 0065 006e 0800 0000  .u.s.c.h.e.n....
+00004bf0: 0006 0000 0024 5472 616e 7370 6f73 6520  .....$Transpose 
+00004c00: 6375 7272 656e 7420 616e 6420 7072 6576  current and prev
+00004c10: 696f 7573 206c 696e 6573 0700 0000 0b51  ious lines.....Q
+00004c20: 7363 6943 6f6d 6d61 6e64 0103 0000 0040  sciCommand.....@
+00004c30: 004c 0065 0074 007a 0074 0065 006e 0020  .L.e.t.z.t.e.n. 
+00004c40: 0042 0065 0066 0065 0068 006c 0020 0072  .B.e.f.e.h.l. .r
+00004c50: 00fc 0063 006b 0067 00e4 006e 0067 0069  ...c.k.g...n.g.i
+00004c60: 0067 0020 006d 0061 0063 0068 0065 006e  .g. .m.a.c.h.e.n
+00004c70: 0800 0000 0006 0000 0011 556e 646f 206c  ..........Undo l
+00004c80: 6173 7420 636f 6d6d 616e 6407 0000 000b  ast command.....
+00004c90: 5173 6369 436f 6d6d 616e 6401 0300 0000  QsciCommand.....
+00004ca0: 1400 5600 6500 7200 6700 7200 f600 df00  ..V.e.r.g.r.....
+00004cb0: 6500 7200 6e08 0000 0000 0600 0000 075a  e.r.n..........Z
+00004cc0: 6f6f 6d20 696e 0700 0000 0b51 7363 6943  oom in.....QsciC
+00004cd0: 6f6d 6d61 6e64 0103 0000 0016 0056 0065  ommand.......V.e
+00004ce0: 0072 006b 006c 0065 0069 006e 0065 0072  .r.k.l.e.i.n.e.r
+00004cf0: 006e 0800 0000 0006 0000 0008 5a6f 6f6d  .n..........Zoom
+00004d00: 206f 7574 0700 0000 0b51 7363 6943 6f6d   out.....QsciCom
+00004d10: 6d61 6e64 0103 0000 001c 0042 006c 006f  mand.......B.l.o
+00004d20: 0063 006b 006b 006f 006d 006d 0065 006e  .c.k.k.o.m.m.e.n
+00004d30: 0074 0061 0072 0800 0000 0006 0000 000d  .t.a.r..........
+00004d40: 426c 6f63 6b20 636f 6d6d 656e 7407 0000  Block comment...
+00004d50: 000c 5173 6369 4c65 7865 7241 5653 0103  ..QsciLexerAVS..
+00004d60: 0000 0020 0043 006c 0069 0070 0020 0045  ... .C.l.i.p. .E
+00004d70: 0069 0067 0065 006e 0073 0063 0068 0061  .i.g.e.n.s.c.h.a
+00004d80: 0066 0074 0800 0000 0006 0000 000d 436c  .f.t..........Cl
+00004d90: 6970 2070 726f 7065 7274 7907 0000 000c  ip property.....
+00004da0: 5173 6369 4c65 7865 7241 5653 0103 0000  QsciLexerAVS....
+00004db0: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
+00004dc0: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
+00004dd0: 756c 7407 0000 000c 5173 6369 4c65 7865  ult.....QsciLexe
+00004de0: 7241 5653 0103 0000 0042 005a 0065 0069  rAVS.....B.Z.e.i
+00004df0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
+00004e00: 0065 0020 0069 006e 0020 0041 006e 0066  .e. .i.n. .A.n.f
+00004e10: 00fc 0068 0072 0075 006e 0067 0073 007a  ...h.r.u.n.g.s.z
+00004e20: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
+00004e30: 0006 0000 0014 446f 7562 6c65 2d71 756f  ......Double-quo
+00004e40: 7465 6420 7374 7269 6e67 0700 0000 0c51  ted string.....Q
+00004e50: 7363 694c 6578 6572 4156 5301 0300 0000  sciLexerAVS.....
+00004e60: 0c00 4600 6900 6c00 7400 6500 7208 0000  ..F.i.l.t.e.r...
+00004e70: 0000 0600 0000 0646 696c 7465 7207 0000  .......Filter...
+00004e80: 000c 5173 6369 4c65 7865 7241 5653 0103  ..QsciLexerAVS..
+00004e90: 0000 0010 0046 0075 006e 006b 0074 0069  .....F.u.n.k.t.i
+00004ea0: 006f 006e 0800 0000 0006 0000 0008 4675  .o.n..........Fu
+00004eb0: 6e63 7469 6f6e 0700 0000 0c51 7363 694c  nction.....QsciL
+00004ec0: 6578 6572 4156 5301 0300 0000 1400 4200  exerAVS.......B.
+00004ed0: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
+00004ee0: 7208 0000 0000 0600 0000 0a49 6465 6e74  r..........Ident
+00004ef0: 6966 6965 7207 0000 000c 5173 6369 4c65  ifier.....QsciLe
+00004f00: 7865 7241 5653 0103 0000 001a 0053 0063  xerAVS.......S.c
+00004f10: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
+00004f20: 006f 0072 0074 0800 0000 0006 0000 0007  .o.r.t..........
+00004f30: 4b65 7977 6f72 6407 0000 000c 5173 6369  Keyword.....Qsci
+00004f40: 4c65 7865 7241 5653 0103 0000 001e 005a  LexerAVS.......Z
+00004f50: 0065 0069 006c 0065 006e 006b 006f 006d  .e.i.l.e.n.k.o.m
+00004f60: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
+00004f70: 0006 0000 000c 4c69 6e65 2063 6f6d 6d65  ......Line comme
+00004f80: 6e74 0700 0000 0c51 7363 694c 6578 6572  nt.....QsciLexer
+00004f90: 4156 5301 0300 0000 3c00 5600 6500 7200  AVS.....<.V.e.r.
+00004fa0: 7300 6300 6800 6100 6300 6800 7400 6500  s.c.h.a.c.h.t.e.
+00004fb0: 6c00 7400 6500 7200 2000 4200 6c00 6f00  l.t.e.r. .B.l.o.
+00004fc0: 6300 6b00 6b00 6f00 6d00 6d00 6500 6e00  c.k.k.o.m.m.e.n.
+00004fd0: 7400 6100 7208 0000 0000 0600 0000 144e  t.a.r..........N
+00004fe0: 6573 7465 6420 626c 6f63 6b20 636f 6d6d  ested block comm
+00004ff0: 656e 7407 0000 000c 5173 6369 4c65 7865  ent.....QsciLexe
+00005000: 7241 5653 0103 0000 0008 005a 0061 0068  rAVS.......Z.a.h
+00005010: 006c 0800 0000 0006 0000 0006 4e75 6d62  .l..........Numb
+00005020: 6572 0700 0000 0c51 7363 694c 6578 6572  er.....QsciLexer
+00005030: 4156 5301 0300 0000 1000 4f00 7000 6500  AVS.......O.p.e.
+00005040: 7200 6100 7400 6f00 7208 0000 0000 0600  r.a.t.o.r.......
+00005050: 0000 084f 7065 7261 746f 7207 0000 000c  ...Operator.....
+00005060: 5173 6369 4c65 7865 7241 5653 0103 0000  QsciLexerAVS....
+00005070: 000c 0050 006c 0075 0067 0069 006e 0800  ...P.l.u.g.i.n..
+00005080: 0000 0006 0000 0006 506c 7567 696e 0700  ........Plugin..
+00005090: 0000 0c51 7363 694c 6578 6572 4156 5301  ...QsciLexerAVS.
+000050a0: 0300 0000 5800 5a00 6500 6900 6300 6800  ....X.Z.e.i.c.h.
+000050b0: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
+000050c0: 6900 6e00 2000 6400 7200 6500 6900 6600  i.n. .d.r.e.i.f.
+000050d0: 6100 6300 6800 6500 6e00 2000 4100 6e00  a.c.h.e.n. .A.n.
+000050e0: 6600 fc00 6800 7200 7500 6e00 6700 7300  f...h.r.u.n.g.s.
+000050f0: 7a00 6500 6900 6300 6800 6500 6e08 0000  z.e.i.c.h.e.n...
+00005100: 0000 0600 0000 1b54 7269 706c 6520 646f  .......Triple do
+00005110: 7562 6c65 2d71 756f 7465 6420 7374 7269  uble-quoted stri
+00005120: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
+00005130: 4156 5301 0300 0000 2000 4e00 7500 7400  AVS..... .N.u.t.
+00005140: 7a00 6500 7200 2000 6400 6500 6600 6900  z.e.r. .d.e.f.i.
+00005150: 6e00 6900 6500 7200 7408 0000 0000 0600  n.i.e.r.t.......
+00005160: 0000 0c55 7365 7220 6465 6669 6e65 6407  ...User defined.
+00005170: 0000 000c 5173 6369 4c65 7865 7241 5653  ....QsciLexerAVS
+00005180: 0103 0000 001c 0042 006c 006f 0063 006b  .......B.l.o.c.k
+00005190: 006b 006f 006d 006d 0065 006e 0074 0061  .k.o.m.m.e.n.t.a
+000051a0: 0072 0800 0000 0006 0000 000d 426c 6f63  .r..........Bloc
+000051b0: 6b20 636f 6d6d 656e 7407 0000 000c 5173  k comment.....Qs
+000051c0: 6369 4c65 7865 7241 736d 0103 0000 001e  ciLexerAsm......
+000051d0: 0043 0050 0055 0020 0049 006e 0073 0074  .C.P.U. .I.n.s.t
+000051e0: 0072 0075 006b 0074 0069 006f 006e 0800  .r.u.k.t.i.o.n..
+000051f0: 0000 0006 0000 000f 4350 5520 696e 7374  ........CPU inst
+00005200: 7275 6374 696f 6e07 0000 000c 5173 6369  ruction.....Qsci
+00005210: 4c65 7865 7241 736d 0103 0000 0012 004b  LexerAsm.......K
+00005220: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
+00005230: 0800 0000 0006 0000 0007 436f 6d6d 656e  ..........Commen
+00005240: 7407 0000 000c 5173 6369 4c65 7865 7241  t.....QsciLexerA
+00005250: 736d 0103 0000 0028 0052 0069 0063 0068  sm.....(.R.i.c.h
+00005260: 0074 006c 0069 006e 0069 0065 006e 006b  .t.l.i.n.i.e.n.k
+00005270: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
+00005280: 0800 0000 0006 0000 0011 436f 6d6d 656e  ..........Commen
+00005290: 7420 6469 7265 6374 6976 6507 0000 000c  t directive.....
+000052a0: 5173 6369 4c65 7865 7241 736d 0103 0000  QsciLexerAsm....
+000052b0: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
+000052c0: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
+000052d0: 756c 7407 0000 000c 5173 6369 4c65 7865  ult.....QsciLexe
+000052e0: 7241 736d 0103 0000 0012 0044 0069 0072  rAsm.......D.i.r
+000052f0: 0065 006b 0074 0069 0076 0065 0800 0000  .e.k.t.i.v.e....
+00005300: 0006 0000 0009 4469 7265 6374 6976 6507  ......Directive.
+00005310: 0000 000c 5173 6369 4c65 7865 7241 736d  ....QsciLexerAsm
+00005320: 0103 0000 0024 0052 0069 0063 0068 0074  .....$.R.i.c.h.t
+00005330: 006c 0069 006e 0069 0065 006e 006f 0070  .l.i.n.i.e.n.o.p
+00005340: 0065 0072 0061 006e 0064 0800 0000 0006  .e.r.a.n.d......
+00005350: 0000 0011 4469 7265 6374 6976 6520 6f70  ....Directive op
+00005360: 6572 616e 6407 0000 000c 5173 6369 4c65  erand.....QsciLe
+00005370: 7865 7241 736d 0103 0000 0042 005a 0065  xerAsm.....B.Z.e
+00005380: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+00005390: 0074 0065 0020 0069 006e 0020 0041 006e  .t.e. .i.n. .A.n
+000053a0: 0066 00fc 0068 0072 0075 006e 0067 0073  .f...h.r.u.n.g.s
+000053b0: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+000053c0: 0000 0006 0000 0014 446f 7562 6c65 2d71  ........Double-q
+000053d0: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
+000053e0: 0c51 7363 694c 6578 6572 4173 6d01 0300  .QsciLexerAsm...
+000053f0: 0000 2a00 4500 7200 7700 6500 6900 7400  ..*.E.r.w.e.i.t.
+00005400: 6500 7200 6500 2000 4900 6e00 7300 7400  e.r.e. .I.n.s.t.
+00005410: 7200 7500 6b00 7400 6900 6f00 6e08 0000  r.u.k.t.i.o.n...
+00005420: 0000 0600 0000 1445 7874 656e 6465 6420  .......Extended 
+00005430: 696e 7374 7275 6374 696f 6e07 0000 000c  instruction.....
+00005440: 5173 6369 4c65 7865 7241 736d 0103 0000  QsciLexerAsm....
+00005450: 001e 0046 0050 0055 0020 0049 006e 0073  ...F.P.U. .I.n.s
+00005460: 0074 0072 0075 006b 0074 0069 006f 006e  .t.r.u.k.t.i.o.n
+00005470: 0800 0000 0006 0000 000f 4650 5520 696e  ..........FPU in
+00005480: 7374 7275 6374 696f 6e07 0000 000c 5173  struction.....Qs
+00005490: 6369 4c65 7865 7241 736d 0103 0000 0014  ciLexerAsm......
+000054a0: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
+000054b0: 0065 0072 0800 0000 0006 0000 000a 4964  .e.r..........Id
+000054c0: 656e 7469 6669 6572 0700 0000 0c51 7363  entifier.....Qsc
+000054d0: 694c 6578 6572 4173 6d01 0300 0000 0800  iLexerAsm.......
+000054e0: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
+000054f0: 064e 756d 6265 7207 0000 000c 5173 6369  .Number.....Qsci
+00005500: 4c65 7865 7241 736d 0103 0000 0010 004f  LexerAsm.......O
+00005510: 0070 0065 0072 0061 0074 006f 0072 0800  .p.e.r.a.t.o.r..
+00005520: 0000 0006 0000 0008 4f70 6572 6174 6f72  ........Operator
+00005530: 0700 0000 0c51 7363 694c 6578 6572 4173  .....QsciLexerAs
+00005540: 6d01 0300 0000 1000 5200 6500 6700 6900  m.......R.e.g.i.
+00005550: 7300 7400 6500 7208 0000 0000 0600 0000  s.t.e.r.........
+00005560: 0852 6567 6973 7465 7207 0000 000c 5173  .Register.....Qs
+00005570: 6369 4c65 7865 7241 736d 0103 0000 0036  ciLexerAsm.....6
+00005580: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+00005590: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
+000055a0: 0048 006f 0063 0068 006b 006f 006d 006d  .H.o.c.h.k.o.m.m
+000055b0: 0061 0074 0061 0800 0000 0006 0000 0014  .a.t.a..........
+000055c0: 5369 6e67 6c65 2d71 756f 7465 6420 7374  Single-quoted st
+000055d0: 7269 6e67 0700 0000 0c51 7363 694c 6578  ring.....QsciLex
+000055e0: 6572 4173 6d01 0300 0000 2e00 5500 6e00  erAsm.......U.n.
+000055f0: 6200 6500 6500 6e00 6400 6500 7400 6500  b.e.e.n.d.e.t.e.
+00005600: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
+00005610: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
+00005620: 0000 0f55 6e63 6c6f 7365 6420 7374 7269  ...Unclosed stri
+00005630: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
+00005640: 4173 6d01 0300 0000 1200 4200 6100 6300  Asm.......B.a.c.
+00005650: 6b00 7400 6900 6300 6b00 7308 0000 0000  k.t.i.c.k.s.....
+00005660: 0600 0000 0942 6163 6b74 6963 6b73 0700  .....Backticks..
+00005670: 0000 0d51 7363 694c 6578 6572 4261 7368  ...QsciLexerBash
+00005680: 0103 0000 0012 004b 006f 006d 006d 0065  .......K.o.m.m.e
+00005690: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
+000056a0: 0007 436f 6d6d 656e 7407 0000 000d 5173  ..Comment.....Qs
+000056b0: 6369 4c65 7865 7242 6173 6801 0300 0000  ciLexerBash.....
+000056c0: 1000 5300 7400 6100 6e00 6400 6100 7200  ..S.t.a.n.d.a.r.
+000056d0: 6408 0000 0000 0600 0000 0744 6566 6175  d..........Defau
+000056e0: 6c74 0700 0000 0d51 7363 694c 6578 6572  lt.....QsciLexer
+000056f0: 4261 7368 0103 0000 0042 005a 0065 0069  Bash.....B.Z.e.i
+00005700: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
+00005710: 0065 0020 0069 006e 0020 0041 006e 0066  .e. .i.n. .A.n.f
+00005720: 00fc 0068 0072 0075 006e 0067 0073 007a  ...h.r.u.n.g.s.z
+00005730: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
+00005740: 0006 0000 0014 446f 7562 6c65 2d71 756f  ......Double-quo
+00005750: 7465 6420 7374 7269 6e67 0700 0000 0d51  ted string.....Q
+00005760: 7363 694c 6578 6572 4261 7368 0103 0000  sciLexerBash....
+00005770: 000c 0046 0065 0068 006c 0065 0072 0800  ...F.e.h.l.e.r..
+00005780: 0000 0006 0000 0005 4572 726f 7207 0000  ........Error...
+00005790: 000d 5173 6369 4c65 7865 7242 6173 6801  ..QsciLexerBash.
+000057a0: 0300 0000 2e00 4800 6500 7200 6500 2000  ......H.e.r.e. .
+000057b0: 4400 6f00 6b00 7500 6d00 6500 6e00 7400  D.o.k.u.m.e.n.t.
+000057c0: 2d00 4200 6500 6700 7200 6500 6e00 7a00  -.B.e.g.r.e.n.z.
+000057d0: 6500 7208 0000 0000 0600 0000 1748 6572  e.r..........Her
+000057e0: 6520 646f 6375 6d65 6e74 2064 656c 696d  e document delim
+000057f0: 6974 6572 0700 0000 0d51 7363 694c 6578  iter.....QsciLex
+00005800: 6572 4261 7368 0103 0000 0014 0042 0065  erBash.......B.e
+00005810: 007a 0065 0069 0063 0068 006e 0065 0072  .z.e.i.c.h.n.e.r
+00005820: 0800 0000 0006 0000 000a 4964 656e 7469  ..........Identi
+00005830: 6669 6572 0700 0000 0d51 7363 694c 6578  fier.....QsciLex
+00005840: 6572 4261 7368 0103 0000 001a 0053 0063  erBash.......S.c
+00005850: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
+00005860: 006f 0072 0074 0800 0000 0006 0000 0007  .o.r.t..........
+00005870: 4b65 7977 6f72 6407 0000 000d 5173 6369  Keyword.....Qsci
+00005880: 4c65 7865 7242 6173 6801 0300 0000 0800  LexerBash.......
+00005890: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
+000058a0: 064e 756d 6265 7207 0000 000d 5173 6369  .Number.....Qsci
+000058b0: 4c65 7865 7242 6173 6801 0300 0000 1000  LexerBash.......
+000058c0: 4f00 7000 6500 7200 6100 7400 6f00 7208  O.p.e.r.a.t.o.r.
+000058d0: 0000 0000 0600 0000 084f 7065 7261 746f  .........Operato
+000058e0: 7207 0000 000d 5173 6369 4c65 7865 7242  r.....QsciLexerB
+000058f0: 6173 6801 0300 0000 2800 5000 6100 7200  ash.....(.P.a.r.
+00005900: 6100 6d00 6500 7400 6500 7200 6500 7200  a.m.e.t.e.r.e.r.
+00005910: 7700 6500 6900 7400 6500 7200 7500 6e00  w.e.i.t.e.r.u.n.
+00005920: 6708 0000 0000 0600 0000 1350 6172 616d  g..........Param
+00005930: 6574 6572 2065 7870 616e 7369 6f6e 0700  eter expansion..
+00005940: 0000 0d51 7363 694c 6578 6572 4261 7368  ...QsciLexerBash
+00005950: 0103 0000 000c 0053 006b 0061 006c 0061  .......S.k.a.l.a
+00005960: 0072 0800 0000 0006 0000 0006 5363 616c  .r..........Scal
+00005970: 6172 0700 0000 0d51 7363 694c 6578 6572  ar.....QsciLexer
+00005980: 4261 7368 0103 0000 0038 0048 0065 0072  Bash.....8.H.e.r
+00005990: 0065 0020 0044 006f 006b 0075 006d 0065  .e. .D.o.k.u.m.e
+000059a0: 006e 0074 0020 0069 006e 0020 0048 006f  .n.t. .i.n. .H.o
+000059b0: 0063 0068 006b 006f 006d 006d 0061 0074  .c.h.k.o.m.m.a.t
+000059c0: 0061 0800 0000 0006 0000 001b 5369 6e67  .a..........Sing
+000059d0: 6c65 2d71 756f 7465 6420 6865 7265 2064  le-quoted here d
+000059e0: 6f63 756d 656e 7407 0000 000d 5173 6369  ocument.....Qsci
+000059f0: 4c65 7865 7242 6173 6801 0300 0000 3600  LexerBash.....6.
+00005a00: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+00005a10: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
+00005a20: 4800 6f00 6300 6800 6b00 6f00 6d00 6d00  H.o.c.h.k.o.m.m.
+00005a30: 6100 7400 6108 0000 0000 0600 0000 1453  a.t.a..........S
+00005a40: 696e 676c 652d 7175 6f74 6564 2073 7472  ingle-quoted str
+00005a50: 696e 6707 0000 000d 5173 6369 4c65 7865  ing.....QsciLexe
+00005a60: 7242 6173 6801 0300 0000 1200 4b00 6f00  rBash.......K.o.
+00005a70: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+00005a80: 0000 0600 0000 0743 6f6d 6d65 6e74 0700  .......Comment..
+00005a90: 0000 0e51 7363 694c 6578 6572 4261 7463  ...QsciLexerBatc
+00005aa0: 6801 0300 0000 1000 5300 7400 6100 6e00  h.......S.t.a.n.
+00005ab0: 6400 6100 7200 6408 0000 0000 0600 0000  d.a.r.d.........
+00005ac0: 0744 6566 6175 6c74 0700 0000 0e51 7363  .Default.....Qsc
+00005ad0: 694c 6578 6572 4261 7463 6801 0300 0000  iLexerBatch.....
+00005ae0: 1e00 4500 7800 7400 6500 7200 6e00 6500  ..E.x.t.e.r.n.e.
+00005af0: 7200 2000 4200 6500 6600 6500 6800 6c08  r. .B.e.f.e.h.l.
+00005b00: 0000 0000 0600 0000 1045 7874 6572 6e61  .........Externa
+00005b10: 6c20 636f 6d6d 616e 6407 0000 000e 5173  l command.....Qs
+00005b20: 6369 4c65 7865 7242 6174 6368 0103 0000  ciLexerBatch....
+00005b30: 0034 0022 0042 0065 0066 0065 0068 006c  .4.".B.e.f.e.h.l
+00005b40: 0020 0076 0065 0072 0062 0065 0072 0067  . .v.e.r.b.e.r.g
+00005b50: 0065 006e 0022 0020 005a 0065 0069 0063  .e.n.". .Z.e.i.c
+00005b60: 0068 0065 006e 0800 0000 0006 0000 0016  .h.e.n..........
+00005b70: 4869 6465 2063 6f6d 6d61 6e64 2063 6861  Hide command cha
+00005b80: 7261 6374 6572 0700 0000 0e51 7363 694c  racter.....QsciL
+00005b90: 6578 6572 4261 7463 6801 0300 0000 1a00  exerBatch.......
+00005ba0: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
+00005bb0: 6c00 7700 6f00 7200 7408 0000 0000 0600  l.w.o.r.t.......
+00005bc0: 0000 074b 6579 776f 7264 0700 0000 0e51  ...Keyword.....Q
+00005bd0: 7363 694c 6578 6572 4261 7463 6801 0300  sciLexerBatch...
+00005be0: 0000 0a00 4d00 6100 7200 6b00 6508 0000  ....M.a.r.k.e...
+00005bf0: 0000 0600 0000 054c 6162 656c 0700 0000  .......Label....
+00005c00: 0e51 7363 694c 6578 6572 4261 7463 6801  .QsciLexerBatch.
+00005c10: 0300 0000 1000 4f00 7000 6500 7200 6100  ......O.p.e.r.a.
+00005c20: 7400 6f00 7208 0000 0000 0600 0000 084f  t.o.r..........O
+00005c30: 7065 7261 746f 7207 0000 000e 5173 6369  perator.....Qsci
+00005c40: 4c65 7865 7242 6174 6368 0103 0000 0010  LexerBatch......
+00005c50: 0056 0061 0072 0069 0061 0062 006c 0065  .V.a.r.i.a.b.l.e
+00005c60: 0800 0000 0006 0000 0008 5661 7269 6162  ..........Variab
+00005c70: 6c65 0700 0000 0e51 7363 694c 6578 6572  le.....QsciLexer
+00005c80: 4261 7463 6801 0300 0000 1200 4b00 6f00  Batch.......K.o.
+00005c90: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+00005ca0: 0000 0600 0000 0743 6f6d 6d65 6e74 0700  .......Comment..
+00005cb0: 0000 0e51 7363 694c 6578 6572 434d 616b  ...QsciLexerCMak
+00005cc0: 6501 0300 0000 1000 5300 7400 6100 6e00  e.......S.t.a.n.
+00005cd0: 6400 6100 7200 6408 0000 0000 0600 0000  d.a.r.d.........
+00005ce0: 0744 6566 6175 6c74 0700 0000 0e51 7363  .Default.....Qsc
+00005cf0: 694c 6578 6572 434d 616b 6501 0300 0000  iLexerCMake.....
+00005d00: 1a00 4600 4f00 5200 4500 4100 4300 4800  ..F.O.R.E.A.C.H.
+00005d10: 2000 4200 6c00 6f00 6300 6b08 0000 0000   .B.l.o.c.k.....
+00005d20: 0600 0000 0d46 4f52 4541 4348 2062 6c6f  .....FOREACH blo
+00005d30: 636b 0700 0000 0e51 7363 694c 6578 6572  ck.....QsciLexer
+00005d40: 434d 616b 6501 0300 0000 1000 4600 7500  CMake.......F.u.
+00005d50: 6e00 6b00 7400 6900 6f00 6e08 0000 0000  n.k.t.i.o.n.....
+00005d60: 0600 0000 0846 756e 6374 696f 6e07 0000  .....Function...
+00005d70: 000e 5173 6369 4c65 7865 7243 4d61 6b65  ..QsciLexerCMake
+00005d80: 0103 0000 0010 0049 0046 0020 0042 006c  .......I.F. .B.l
+00005d90: 006f 0063 006b 0800 0000 0006 0000 0008  .o.c.k..........
+00005da0: 4946 2062 6c6f 636b 0700 0000 0e51 7363  IF block.....Qsc
+00005db0: 694c 6578 6572 434d 616b 6501 0300 0000  iLexerCMake.....
+00005dc0: 0a00 4d00 6100 7200 6b00 6508 0000 0000  ..M.a.r.k.e.....
+00005dd0: 0600 0000 054c 6162 656c 0700 0000 0e51  .....Label.....Q
+00005de0: 7363 694c 6578 6572 434d 616b 6501 0300  sciLexerCMake...
+00005df0: 0000 3800 4c00 6900 6e00 6b00 7300 2000  ..8.L.i.n.k.s. .
+00005e00: 7100 7500 6f00 7400 6900 6500 7200 7400  q.u.o.t.i.e.r.t.
+00005e10: 6500 2000 5a00 6500 6900 6300 6800 6500  e. .Z.e.i.c.h.e.
+00005e20: 6e00 6b00 6500 7400 7400 6508 0000 0000  n.k.e.t.t.e.....
+00005e30: 0600 0000 124c 6566 7420 7175 6f74 6564  .....Left quoted
+00005e40: 2073 7472 696e 6707 0000 000e 5173 6369   string.....Qsci
+00005e50: 4c65 7865 7243 4d61 6b65 0103 0000 0016  LexerCMake......
+00005e60: 004d 0041 0043 0052 004f 0020 0042 006c  .M.A.C.R.O. .B.l
+00005e70: 006f 0063 006b 0800 0000 0006 0000 000b  .o.c.k..........
+00005e80: 4d41 4352 4f20 626c 6f63 6b07 0000 000e  MACRO block.....
+00005e90: 5173 6369 4c65 7865 7243 4d61 6b65 0103  QsciLexerCMake..
+00005ea0: 0000 0008 005a 0061 0068 006c 0800 0000  .....Z.a.h.l....
+00005eb0: 0006 0000 0006 4e75 6d62 6572 0700 0000  ......Number....
+00005ec0: 0e51 7363 694c 6578 6572 434d 616b 6501  .QsciLexerCMake.
+00005ed0: 0300 0000 3a00 5200 6500 6300 6800 7400  ....:.R.e.c.h.t.
+00005ee0: 7300 2000 7100 7500 6f00 7400 6900 6500  s. .q.u.o.t.i.e.
+00005ef0: 7200 7400 6500 2000 5a00 6500 6900 6300  r.t.e. .Z.e.i.c.
+00005f00: 6800 6500 6e00 6b00 6500 7400 7400 6508  h.e.n.k.e.t.t.e.
+00005f10: 0000 0000 0600 0000 1352 6967 6874 2071  .........Right q
+00005f20: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
+00005f30: 0e51 7363 694c 6578 6572 434d 616b 6501  .QsciLexerCMake.
+00005f40: 0300 0000 1800 5a00 6500 6900 6300 6800  ......Z.e.i.c.h.
+00005f50: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
+00005f60: 0000 0600 0000 0653 7472 696e 6707 0000  .......String...
+00005f70: 000e 5173 6369 4c65 7865 7243 4d61 6b65  ..QsciLexerCMake
+00005f80: 0103 0000 0020 004e 0075 0074 007a 0065  ..... .N.u.t.z.e
+00005f90: 0072 0020 0064 0065 0066 0069 006e 0069  .r. .d.e.f.i.n.i
+00005fa0: 0065 0072 0074 0800 0000 0006 0000 000c  .e.r.t..........
+00005fb0: 5573 6572 2064 6566 696e 6564 0700 0000  User defined....
+00005fc0: 0e51 7363 694c 6578 6572 434d 616b 6501  .QsciLexerCMake.
+00005fd0: 0300 0000 1000 5600 6100 7200 6900 6100  ......V.a.r.i.a.
+00005fe0: 6200 6c00 6508 0000 0000 0600 0000 0856  b.l.e..........V
+00005ff0: 6172 6961 626c 6507 0000 000e 5173 6369  ariable.....Qsci
+00006000: 4c65 7865 7243 4d61 6b65 0103 0000 003c  LexerCMake.....<
+00006010: 0056 0061 0072 0069 0061 0062 006c 0065  .V.a.r.i.a.b.l.e
+00006020: 0020 0069 006e 0020 0065 0069 006e 0065  . .i.n. .e.i.n.e
+00006030: 0072 0020 005a 0065 0069 0063 0068 0065  .r. .Z.e.i.c.h.e
+00006040: 006e 006b 0065 0074 0074 0065 0800 0000  .n.k.e.t.t.e....
+00006050: 0006 0000 0018 5661 7269 6162 6c65 2077  ......Variable w
+00006060: 6974 6869 6e20 6120 7374 7269 6e67 0700  ithin a string..
+00006070: 0000 0e51 7363 694c 6578 6572 434d 616b  ...QsciLexerCMak
+00006080: 6501 0300 0000 1600 5700 4800 4900 4c00  e.......W.H.I.L.
+00006090: 4500 2000 4200 6c00 6f00 6300 6b08 0000  E. .B.l.o.c.k...
+000060a0: 0000 0600 0000 0b57 4849 4c45 2062 6c6f  .......WHILE blo
+000060b0: 636b 0700 0000 0e51 7363 694c 6578 6572  ck.....QsciLexer
+000060c0: 434d 616b 6501 0300 0000 1600 4300 2000  CMake.......C. .
+000060d0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+000060e0: 7208 0000 0000 0600 0000 0943 2063 6f6d  r..........C com
+000060f0: 6d65 6e74 0700 0000 0c51 7363 694c 6578  ment.....QsciLex
+00006100: 6572 4350 5001 0300 0000 4000 5500 6e00  erCPP.....@.U.n.
+00006110: 6900 6e00 7400 6500 7200 7000 7200 6500  i.n.t.e.r.p.r.e.
+00006120: 7400 6900 6500 7200 7400 6500 2000 4300  t.i.e.r.t.e. .C.
+00006130: 2300 2000 5a00 6500 6900 6300 6800 6500  #. .Z.e.i.c.h.e.
+00006140: 6e00 6b00 6500 7400 7400 6508 0000 0000  n.k.e.t.t.e.....
+00006150: 0600 0000 1243 2320 7665 7262 6174 696d  .....C# verbatim
+00006160: 2073 7472 696e 6707 0000 000c 5173 6369   string.....Qsci
+00006170: 4c65 7865 7243 5050 0103 0000 001a 0043  LexerCPP.......C
+00006180: 002b 002b 0020 004b 006f 006d 006d 0065  .+.+. .K.o.m.m.e
+00006190: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
+000061a0: 000b 432b 2b20 636f 6d6d 656e 7407 0000  ..C++ comment...
+000061b0: 000c 5173 6369 4c65 7865 7243 5050 0103  ..QsciLexerCPP..
+000061c0: 0000 002a 0052 006f 0068 0065 0020 0043  ...*.R.o.h.e. .C
+000061d0: 002b 002b 0020 005a 0065 0069 0063 0068  .+.+. .Z.e.i.c.h
+000061e0: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
+000061f0: 0000 0006 0000 000e 432b 2b20 7261 7720  ........C++ raw 
+00006200: 7374 7269 6e67 0700 0000 0c51 7363 694c  string.....QsciL
+00006210: 6578 6572 4350 5001 0300 0000 1000 5300  exerCPP.......S.
+00006220: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
+00006230: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
+00006240: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
+00006250: 0300 0000 4200 5a00 6500 6900 6300 6800  ....B.Z.e.i.c.h.
+00006260: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
+00006270: 6900 6e00 2000 4100 6e00 6600 fc00 6800  i.n. .A.n.f...h.
+00006280: 7200 7500 6e00 6700 7300 7a00 6500 6900  r.u.n.g.s.z.e.i.
+00006290: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+000062a0: 1444 6f75 626c 652d 7175 6f74 6564 2073  .Double-quoted s
+000062b0: 7472 696e 6707 0000 000c 5173 6369 4c65  tring.....QsciLe
+000062c0: 7865 7243 5050 0103 0000 001c 0045 0073  xerCPP.......E.s
+000062d0: 0063 0061 0070 0065 002d 0053 0065 0071  .c.a.p.e.-.S.e.q
+000062e0: 0075 0065 006e 007a 0800 0000 0006 0000  .u.e.n.z........
+000062f0: 000f 4573 6361 7065 2073 6571 7565 6e63  ..Escape sequenc
+00006300: 6507 0000 000c 5173 6369 4c65 7865 7243  e.....QsciLexerC
+00006310: 5050 0103 0000 0046 0047 006c 006f 0062  PP.....F.G.l.o.b
+00006320: 0061 006c 0065 0020 004b 006c 0061 0073  .a.l.e. .K.l.a.s
+00006330: 0073 0065 006e 0020 0075 006e 0064 0020  .s.e.n. .u.n.d. 
+00006340: 0054 0079 0070 0064 0065 0066 0069 006e  .T.y.p.d.e.f.i.n
+00006350: 0069 0074 0069 006f 006e 0065 006e 0800  .i.t.i.o.n.e.n..
+00006360: 0000 0006 0000 001b 476c 6f62 616c 2063  ........Global c
+00006370: 6c61 7373 6573 2061 6e64 2074 7970 6564  lasses and typed
+00006380: 6566 7307 0000 000c 5173 6369 4c65 7865  efs.....QsciLexe
+00006390: 7243 5050 0103 0000 0010 0049 0044 004c  rCPP.......I.D.L
+000063a0: 0020 0055 0055 0049 0044 0800 0000 0006  . .U.U.I.D......
+000063b0: 0000 0008 4944 4c20 5555 4944 0700 0000  ....IDL UUID....
+000063c0: 0c51 7363 694c 6578 6572 4350 5001 0300  .QsciLexerCPP...
+000063d0: 0000 1400 4200 6500 7a00 6500 6900 6300  ....B.e.z.e.i.c.
+000063e0: 6800 6e00 6500 7208 0000 0000 0600 0000  h.n.e.r.........
+000063f0: 0a49 6465 6e74 6966 6965 7207 0000 000c  .Identifier.....
+00006400: 5173 6369 4c65 7865 7243 5050 0103 0000  QsciLexerCPP....
+00006410: 002a 0049 006e 0061 006b 0074 0069 0076  .*.I.n.a.k.t.i.v
+00006420: 0065 0072 0020 0043 0020 004b 006f 006d  .e.r. .C. .K.o.m
+00006430: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
+00006440: 0006 0000 0012 496e 6163 7469 7665 2043  ......Inactive C
+00006450: 2063 6f6d 6d65 6e74 0700 0000 0c51 7363   comment.....Qsc
+00006460: 694c 6578 6572 4350 5001 0300 0000 5400  iLexerCPP.....T.
+00006470: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
+00006480: 2c00 2000 5500 6e00 6900 6e00 7400 6500  ,. .U.n.i.n.t.e.
+00006490: 7200 7000 7200 6500 7400 6900 6500 7200  r.p.r.e.t.i.e.r.
+000064a0: 7400 6500 2000 4300 2300 2000 5a00 6500  t.e. .C.#. .Z.e.
+000064b0: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
+000064c0: 7400 6508 0000 0000 0600 0000 1b49 6e61  t.e..........Ina
+000064d0: 6374 6976 6520 4323 2076 6572 6261 7469  ctive C# verbati
+000064e0: 6d20 7374 7269 6e67 0700 0000 0c51 7363  m string.....Qsc
+000064f0: 694c 6578 6572 4350 5001 0300 0000 2e00  iLexerCPP.......
+00006500: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
+00006510: 7200 2000 4300 2b00 2b00 2000 4b00 6f00  r. .C.+.+. .K.o.
+00006520: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+00006530: 0000 0600 0000 1449 6e61 6374 6976 6520  .......Inactive 
+00006540: 432b 2b20 636f 6d6d 656e 7407 0000 000c  C++ comment.....
+00006550: 5173 6369 4c65 7865 7243 5050 0103 0000  QsciLexerCPP....
+00006560: 003c 0049 006e 0061 006b 0074 0069 0076  .<.I.n.a.k.t.i.v
+00006570: 0065 0020 0072 006f 0068 0065 0020 0043  .e. .r.o.h.e. .C
+00006580: 002b 002b 0020 005a 0065 0069 0063 0068  .+.+. .Z.e.i.c.h
+00006590: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
+000065a0: 0000 0006 0000 0017 496e 6163 7469 7665  ........Inactive
+000065b0: 2043 2b2b 2072 6177 2073 7472 696e 6707   C++ raw string.
+000065c0: 0000 000c 5173 6369 4c65 7865 7243 5050  ....QsciLexerCPP
+000065d0: 0103 0000 0022 0049 006e 0061 006b 0074  .....".I.n.a.k.t
+000065e0: 0069 0076 0065 0020 0049 0044 004c 0020  .i.v.e. .I.D.L. 
+000065f0: 0055 0055 0049 0044 0800 0000 0006 0000  .U.U.I.D........
+00006600: 0011 496e 6163 7469 7665 2049 444c 2055  ..Inactive IDL U
+00006610: 5549 4407 0000 000c 5173 6369 4c65 7865  UID.....QsciLexe
+00006620: 7243 5050 0103 0000 003e 0049 006e 0061  rCPP.....>.I.n.a
+00006630: 006b 0074 0069 0076 0065 0073 0020 004a  .k.t.i.v.e.s. .J
+00006640: 0061 0076 0061 0044 006f 0063 0020 0053  .a.v.a.D.o.c. .S
+00006650: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
+00006660: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
+00006670: 0018 496e 6163 7469 7665 204a 6176 6144  ..Inactive JavaD
+00006680: 6f63 206b 6579 776f 7264 0700 0000 0c51  oc keyword.....Q
+00006690: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
+000066a0: 4a00 4900 6e00 6100 6b00 7400 6900 7600  J.I.n.a.k.t.i.v.
+000066b0: 6500 7200 2000 4a00 6100 7600 6100 4400  e.r. .J.a.v.a.D.
+000066c0: 6f00 6300 2000 5300 6300 6800 6c00 fc00  o.c. .S.c.h.l...
+000066d0: 7300 7300 6500 6c00 7700 6f00 7200 7400  s.s.e.l.w.o.r.t.
+000066e0: 6600 6500 6800 6c00 6500 7208 0000 0000  f.e.h.l.e.r.....
+000066f0: 0600 0000 1e49 6e61 6374 6976 6520 4a61  .....Inactive Ja
+00006700: 7661 446f 6320 6b65 7977 6f72 6420 6572  vaDoc keyword er
+00006710: 726f 7207 0000 000c 5173 6369 4c65 7865  ror.....QsciLexe
+00006720: 7243 5050 0103 0000 003a 0049 006e 0061  rCPP.....:.I.n.a
+00006730: 006b 0074 0069 0076 0065 0072 0020 004a  .k.t.i.v.e.r. .J
+00006740: 0061 0076 0061 0044 006f 0063 0020 0043  .a.v.a.D.o.c. .C
+00006750: 0020 004b 006f 006d 006d 0065 006e 0074  . .K.o.m.m.e.n.t
+00006760: 0061 0072 0800 0000 0006 0000 0020 496e  .a.r......... In
+00006770: 6163 7469 7665 204a 6176 6144 6f63 2073  active JavaDoc s
+00006780: 7479 6c65 2043 2063 6f6d 6d65 6e74 0700  tyle C comment..
+00006790: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
+000067a0: 0300 0000 3e00 4900 6e00 6100 6b00 7400  ....>.I.n.a.k.t.
+000067b0: 6900 7600 6500 7200 2000 4a00 6100 7600  i.v.e.r. .J.a.v.
+000067c0: 6100 4400 6f00 6300 2000 4300 2b00 2b00  a.D.o.c. .C.+.+.
+000067d0: 2000 4b00 6f00 6d00 6d00 6500 6e00 7400   .K.o.m.m.e.n.t.
+000067e0: 6100 7208 0000 0000 0600 0000 2249 6e61  a.r........."Ina
+000067f0: 6374 6976 6520 4a61 7661 446f 6320 7374  ctive JavaDoc st
+00006800: 796c 6520 432b 2b20 636f 6d6d 656e 7407  yle C++ comment.
+00006810: 0000 000c 5173 6369 4c65 7865 7243 5050  ....QsciLexerCPP
+00006820: 0103 0000 004e 0049 006e 0061 006b 0074  .....N.I.n.a.k.t
+00006830: 0069 0076 0065 0072 0020 004a 0061 0076  .i.v.e.r. .J.a.v
+00006840: 0061 0044 006f 0063 0020 0050 0072 00e4  .a.D.o.c. .P.r..
+00006850: 0070 0072 006f 007a 0065 0073 0073 006f  .p.r.o.z.e.s.s.o
+00006860: 0072 006b 006f 006d 006d 0065 006e 0074  .r.k.o.m.m.e.n.t
+00006870: 0061 0072 0800 0000 0006 0000 002c 496e  .a.r.........,In
+00006880: 6163 7469 7665 204a 6176 6144 6f63 2073  active JavaDoc s
+00006890: 7479 6c65 2070 7265 2d70 726f 6365 7373  tyle pre-process
+000068a0: 6f72 2063 6f6d 6d65 6e74 0700 0000 0c51  or comment.....Q
+000068b0: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
+000068c0: 4e00 4a00 6100 7600 6100 5300 6300 7200  N.J.a.v.a.S.c.r.
+000068d0: 6900 7000 7400 2000 4900 6e00 6100 6b00  i.p.t. .I.n.a.k.
+000068e0: 7400 6900 7600 6500 7200 2000 5200 6500  t.i.v.e.r. .R.e.
+000068f0: 6700 7500 6c00 e400 7200 6500 7200 2000  g.u.l...r.e.r. .
+00006900: 4100 7500 7300 6400 7200 7500 6300 6b08  A.u.s.d.r.u.c.k.
+00006910: 0000 0000 0600 0000 2649 6e61 6374 6976  ........&Inactiv
+00006920: 6520 4a61 7661 5363 7269 7074 2072 6567  e JavaScript reg
+00006930: 756c 6172 2065 7870 7265 7373 696f 6e07  ular expression.
+00006940: 0000 000c 5173 6369 4c65 7865 7243 5050  ....QsciLexerCPP
+00006950: 0103 0000 0066 0049 006e 0061 006b 0074  .....f.I.n.a.k.t
+00006960: 0069 0076 0065 0020 0050 0069 006b 0065  .i.v.e. .P.i.k.e
+00006970: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
+00006980: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
+00006990: 0020 0027 0023 002d 0041 006e 0066 00fc  . .'.#.-.A.n.f..
+000069a0: 0068 0072 0075 006e 0067 0073 007a 0065  .h.r.u.n.g.s.z.e
+000069b0: 0069 0063 0068 0065 006e 0027 0800 0000  .i.c.h.e.n.'....
+000069c0: 0006 0000 0020 496e 6163 7469 7665 2050  ..... Inactive P
+000069d0: 696b 6520 6861 7368 2d71 756f 7465 6420  ike hash-quoted 
+000069e0: 7374 7269 6e67 0700 0000 0c51 7363 694c  string.....QsciL
+000069f0: 6578 6572 4350 5001 0300 0000 6800 4900  exerCPP.....h.I.
+00006a00: 6e00 6100 6b00 7400 6900 7600 6500 2000  n.a.k.t.i.v.e. .
+00006a10: 5600 6100 6c00 6100 2000 5a00 6500 6900  V.a.l.a. .Z.e.i.
+00006a20: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
+00006a30: 6500 2000 6900 6e00 2000 6400 7200 6500  e. .i.n. .d.r.e.
+00006a40: 6900 6600 6100 6300 6800 6500 6e00 2000  i.f.a.c.h.e.n. .
+00006a50: 4800 6f00 6300 6800 6b00 6f00 6d00 6d00  H.o.c.h.k.o.m.m.
+00006a60: 6100 7400 6108 0000 0000 0600 0000 2b49  a.t.a.........+I
+00006a70: 6e61 6374 6976 6520 5661 6c61 2074 7269  nactive Vala tri
+00006a80: 706c 652d 7175 6f74 6564 2076 6572 6261  ple-quoted verba
+00006a90: 7469 6d20 7374 7269 6e67 0700 0000 0c51  tim string.....Q
+00006aa0: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
+00006ab0: 2400 4900 6e00 6100 6b00 7400 6900 7600  $.I.n.a.k.t.i.v.
+00006ac0: 6500 7200 2000 5300 7400 6100 6e00 6400  e.r. .S.t.a.n.d.
+00006ad0: 6100 7200 6408 0000 0000 0600 0000 1049  a.r.d..........I
+00006ae0: 6e61 6374 6976 6520 6465 6661 756c 7407  nactive default.
+00006af0: 0000 000c 5173 6369 4c65 7865 7243 5050  ....QsciLexerCPP
+00006b00: 0103 0000 0054 0049 006e 0061 006b 0074  .....T.I.n.a.k.t
+00006b10: 0069 0076 0065 0020 005a 0065 0069 0063  .i.v.e. .Z.e.i.c
+00006b20: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
+00006b30: 0020 0069 006e 0020 0041 006e 0066 00fc  . .i.n. .A.n.f..
+00006b40: 0068 0072 0075 006e 0067 0073 007a 0065  .h.r.u.n.g.s.z.e
+00006b50: 0069 0063 0068 0065 006e 0800 0000 0006  .i.c.h.e.n......
+00006b60: 0000 001d 496e 6163 7469 7665 2064 6f75  ....Inactive dou
+00006b70: 626c 652d 7175 6f74 6564 2073 7472 696e  ble-quoted strin
+00006b80: 6707 0000 000c 5173 6369 4c65 7865 7243  g.....QsciLexerC
+00006b90: 5050 0103 0000 002e 0049 006e 0061 006b  PP.......I.n.a.k
+00006ba0: 0074 0069 0076 0065 0020 0045 0073 0063  .t.i.v.e. .E.s.c
+00006bb0: 0061 0070 0065 002d 0053 0065 0071 0075  .a.p.e.-.S.e.q.u
+00006bc0: 0065 006e 007a 0800 0000 0006 0000 0018  .e.n.z..........
+00006bd0: 496e 6163 7469 7665 2065 7363 6170 6520  Inactive escape 
+00006be0: 7365 7175 656e 6365 0700 0000 0c51 7363  sequence.....Qsc
+00006bf0: 694c 6578 6572 4350 5001 0300 0000 5800  iLexerCPP.....X.
+00006c00: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
+00006c10: 2000 6700 6c00 6f00 6200 6100 6c00 6500   .g.l.o.b.a.l.e.
+00006c20: 2000 4b00 6c00 6100 7300 7300 6500 6e00   .K.l.a.s.s.e.n.
+00006c30: 2000 7500 6e00 6400 2000 5400 7900 7000   .u.n.d. .T.y.p.
+00006c40: 6400 6500 6600 6900 6e00 6900 7400 6900  d.e.f.i.n.i.t.i.
+00006c50: 6f00 6e00 6500 6e08 0000 0000 0600 0000  o.n.e.n.........
+00006c60: 2449 6e61 6374 6976 6520 676c 6f62 616c  $Inactive global
+00006c70: 2063 6c61 7373 6573 2061 6e64 2074 7970   classes and typ
+00006c80: 6564 6566 7307 0000 000c 5173 6369 4c65  edefs.....QsciLe
+00006c90: 7865 7243 5050 0103 0000 0028 0049 006e  xerCPP.....(.I.n
+00006ca0: 0061 006b 0074 0069 0076 0065 0072 0020  .a.k.t.i.v.e.r. 
+00006cb0: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
+00006cc0: 0065 0072 0800 0000 0006 0000 0013 496e  .e.r..........In
+00006cd0: 6163 7469 7665 2069 6465 6e74 6966 6965  active identifie
+00006ce0: 7207 0000 000c 5173 6369 4c65 7865 7243  r.....QsciLexerC
+00006cf0: 5050 0103 0000 002e 0049 006e 0061 006b  PP.......I.n.a.k
+00006d00: 0074 0069 0076 0065 0073 0020 0053 0063  .t.i.v.e.s. .S.c
+00006d10: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
+00006d20: 006f 0072 0074 0800 0000 0006 0000 0010  .o.r.t..........
+00006d30: 496e 6163 7469 7665 206b 6579 776f 7264  Inactive keyword
+00006d40: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
+00006d50: 5001 0300 0000 1a00 4900 6e00 6100 6b00  P.......I.n.a.k.
+00006d60: 7400 6900 7600 6500 2000 5a00 6100 6800  t.i.v.e. .Z.a.h.
+00006d70: 6c08 0000 0000 0600 0000 0f49 6e61 6374  l..........Inact
+00006d80: 6976 6520 6e75 6d62 6572 0700 0000 0c51  ive number.....Q
+00006d90: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
+00006da0: 2400 4900 6e00 6100 6b00 7400 6900 7600  $.I.n.a.k.t.i.v.
+00006db0: 6500 7200 2000 4f00 7000 6500 7200 6100  e.r. .O.p.e.r.a.
+00006dc0: 7400 6f00 7208 0000 0000 0600 0000 1149  t.o.r..........I
+00006dd0: 6e61 6374 6976 6520 6f70 6572 6174 6f72  nactive operator
+00006de0: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
+00006df0: 5001 0300 0000 4200 4900 6e00 6100 6b00  P.....B.I.n.a.k.
+00006e00: 7400 6900 7600 6500 7200 2000 4300 2000  t.i.v.e.r. .C. .
+00006e10: 5000 7200 e400 7000 7200 6f00 7a00 6500  P.r...p.r.o.z.e.
+00006e20: 7300 7300 6f00 7200 6b00 6f00 6d00 6d00  s.s.o.r.k.o.m.m.
+00006e30: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
+00006e40: 0000 2049 6e61 6374 6976 6520 7072 652d  .. Inactive pre-
+00006e50: 7072 6f63 6573 736f 7220 4320 636f 6d6d  processor C comm
+00006e60: 656e 7407 0000 000c 5173 6369 4c65 7865  ent.....QsciLexe
+00006e70: 7243 5050 0103 0000 0036 0049 006e 0061  rCPP.....6.I.n.a
+00006e80: 006b 0074 0069 0076 0065 0072 0020 0050  .k.t.i.v.e.r. .P
+00006e90: 0072 00e4 0070 0072 006f 007a 0065 0073  .r...p.r.o.z.e.s
+00006ea0: 0073 006f 0072 0062 006c 006f 0063 006b  .s.o.r.b.l.o.c.k
+00006eb0: 0800 0000 0006 0000 001c 496e 6163 7469  ..........Inacti
+00006ec0: 7665 2070 7265 2d70 726f 6365 7373 6f72  ve pre-processor
+00006ed0: 2062 6c6f 636b 0700 0000 0c51 7363 694c   block.....QsciL
+00006ee0: 6578 6572 4350 5001 0300 0000 6200 4900  exerCPP.....b.I.
+00006ef0: 6e00 6100 6b00 7400 6900 7600 6500 2000  n.a.k.t.i.v.e. .
+00006f00: 7300 6500 6b00 7500 6e00 6400 e400 7200  s.e.k.u.n.d...r.
+00006f10: 6500 2000 5300 6300 6800 6c00 7500 7300  e. .S.c.h.l.u.s.
+00006f20: 7300 6500 6c00 7700 f600 7200 7400 6500  s.e.l.w...r.t.e.
+00006f30: 7200 2000 7500 6e00 6400 2000 4200 6500  r. .u.n.d. .B.e.
+00006f40: 7a00 6500 6900 6300 6800 6e00 6500 7208  z.e.i.c.h.n.e.r.
+00006f50: 0000 0000 0600 0000 2b49 6e61 6374 6976  ........+Inactiv
+00006f60: 6520 7365 636f 6e64 6172 7920 6b65 7977  e secondary keyw
+00006f70: 6f72 6473 2061 6e64 2069 6465 6e74 6966  ords and identif
+00006f80: 6965 7273 0700 0000 0c51 7363 694c 6578  iers.....QsciLex
+00006f90: 6572 4350 5001 0300 0000 4800 4900 6e00  erCPP.....H.I.n.
+00006fa0: 6100 6b00 7400 6900 7600 6500 2000 5a00  a.k.t.i.v.e. .Z.
+00006fb0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+00006fc0: 7400 7400 6500 2000 6900 6e00 2000 4800  t.t.e. .i.n. .H.
+00006fd0: 6f00 6300 6800 6b00 6f00 6d00 6d00 6100  o.c.h.k.o.m.m.a.
+00006fe0: 7400 6108 0000 0000 0600 0000 1d49 6e61  t.a..........Ina
+00006ff0: 6374 6976 6520 7369 6e67 6c65 2d71 756f  ctive single-quo
+00007000: 7465 6420 7374 7269 6e67 0700 0000 0c51  ted string.....Q
 00007010: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
-00007020: 5000 5300 6500 6b00 7500 6e00 6400 e400  P.S.e.k.u.n.d...
-00007030: 7200 6500 2000 5300 6300 6800 6c00 7500  r.e. .S.c.h.l.u.
-00007040: 7300 7300 6500 6c00 7700 f600 7200 7400  s.s.e.l.w...r.t.
-00007050: 6500 7200 2000 7500 6e00 6400 2000 4200  e.r. .u.n.d. .B.
-00007060: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
-00007070: 7208 0000 0000 0600 0000 2253 6563 6f6e  r........."Secon
-00007080: 6461 7279 206b 6579 776f 7264 7320 616e  dary keywords an
-00007090: 6420 6964 656e 7469 6669 6572 7307 0000  d identifiers...
-000070a0: 000c 5173 6369 4c65 7865 7243 5050 0103  ..QsciLexerCPP..
-000070b0: 0000 0036 005a 0065 0069 0063 0068 0065  ...6.Z.e.i.c.h.e
-000070c0: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
-000070d0: 006e 0020 0048 006f 0063 0068 006b 006f  .n. .H.o.c.h.k.o
-000070e0: 006d 006d 0061 0074 0061 0800 0000 0006  .m.m.a.t.a......
-000070f0: 0000 0014 5369 6e67 6c65 2d71 756f 7465  ....Single-quote
-00007100: 6420 7374 7269 6e67 0700 0000 0c51 7363  d string.....Qsc
-00007110: 694c 6578 6572 4350 5001 0300 0000 2400  iLexerCPP.....$.
-00007120: 4100 7500 6600 6700 6100 6200 6500 6e00  A.u.f.g.a.b.e.n.
-00007130: 6d00 6100 7200 6b00 6900 6500 7200 7500  m.a.r.k.i.e.r.u.
-00007140: 6e00 6708 0000 0000 0600 0000 0b54 6173  n.g..........Tas
-00007150: 6b20 6d61 726b 6572 0700 0000 0c51 7363  k marker.....Qsc
-00007160: 694c 6578 6572 4350 5001 0300 0000 2e00  iLexerCPP.......
-00007170: 5500 6e00 6200 6500 6500 6e00 6400 6500  U.n.b.e.e.n.d.e.
-00007180: 7400 6500 2000 5a00 6500 6900 6300 6800  t.e. .Z.e.i.c.h.
-00007190: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
-000071a0: 0000 0600 0000 0f55 6e63 6c6f 7365 6420  .......Unclosed 
-000071b0: 7374 7269 6e67 0700 0000 0c51 7363 694c  string.....QsciL
-000071c0: 6578 6572 4350 5001 0300 0000 3400 4e00  exerCPP.....4.N.
-000071d0: 7500 7400 7a00 6500 7200 2000 6400 6500  u.t.z.e.r. .d.e.
-000071e0: 6600 6900 6e00 6900 6500 7200 7400 6500  f.i.n.i.e.r.t.e.
-000071f0: 7300 2000 4c00 6900 7400 6500 7200 6100  s. .L.i.t.e.r.a.
-00007200: 6c08 0000 0000 0600 0000 1455 7365 722d  l..........User-
-00007210: 6465 6669 6e65 6420 6c69 7465 7261 6c07  defined literal.
-00007220: 0000 000c 5173 6369 4c65 7865 7243 5050  ....QsciLexerCPP
-00007230: 0103 0000 0056 0056 0061 006c 0061 0020  .....V.V.a.l.a. 
-00007240: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-00007250: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
-00007260: 0064 0072 0065 0069 0066 0061 0063 0068  .d.r.e.i.f.a.c.h
-00007270: 0065 006e 0020 0048 006f 0063 0068 006b  .e.n. .H.o.c.h.k
-00007280: 006f 006d 006d 0061 0074 0061 0800 0000  .o.m.m.a.t.a....
-00007290: 0006 0000 0022 5661 6c61 2074 7269 706c  ....."Vala tripl
-000072a0: 652d 7175 6f74 6564 2076 6572 6261 7469  e-quoted verbati
-000072b0: 6d20 7374 7269 6e67 0700 0000 0c51 7363  m string.....Qsc
-000072c0: 694c 6578 6572 4350 5001 0300 0000 0e00  iLexerCPP.......
-000072d0: 4000 2d00 5200 6500 6700 6500 6c08 0000  @.-.R.e.g.e.l...
-000072e0: 0000 0600 0000 0640 2d72 756c 6507 0000  .......@-rule...
-000072f0: 000c 5173 6369 4c65 7865 7243 5353 0103  ..QsciLexerCSS..
-00007300: 0000 0010 0041 0074 0074 0072 0069 0062  .....A.t.t.r.i.b
-00007310: 0075 0074 0800 0000 0006 0000 0009 4174  .u.t..........At
-00007320: 7472 6962 7574 6507 0000 000c 5173 6369  tribute.....Qsci
-00007330: 4c65 7865 7243 5353 0103 0000 0020 0043  LexerCSS..... .C
-00007340: 0053 0053 0031 0020 0045 0069 0067 0065  .S.S.1. .E.i.g.e
-00007350: 006e 0073 0063 0068 0061 0066 0074 0800  .n.s.c.h.a.f.t..
-00007360: 0000 0006 0000 000d 4353 5331 2070 726f  ........CSS1 pro
-00007370: 7065 7274 7907 0000 000c 5173 6369 4c65  perty.....QsciLe
-00007380: 7865 7243 5353 0103 0000 0020 0043 0053  xerCSS..... .C.S
-00007390: 0053 0032 0020 0045 0069 0067 0065 006e  .S.2. .E.i.g.e.n
-000073a0: 0073 0063 0068 0061 0066 0074 0800 0000  .s.c.h.a.f.t....
-000073b0: 0006 0000 000d 4353 5332 2070 726f 7065  ......CSS2 prope
-000073c0: 7274 7907 0000 000c 5173 6369 4c65 7865  rty.....QsciLexe
-000073d0: 7243 5353 0103 0000 0020 0043 0053 0053  rCSS..... .C.S.S
-000073e0: 0033 0020 0045 0069 0067 0065 006e 0073  .3. .E.i.g.e.n.s
-000073f0: 0063 0068 0061 0066 0074 0800 0000 0006  .c.h.a.f.t......
-00007400: 0000 000d 4353 5333 2070 726f 7065 7274  ....CSS3 propert
-00007410: 7907 0000 000c 5173 6369 4c65 7865 7243  y.....QsciLexerC
-00007420: 5353 0103 0000 001e 004b 006c 0061 0073  SS.......K.l.a.s
-00007430: 0073 0065 006e 0073 0065 006c 0065 006b  .s.e.n.s.e.l.e.k
-00007440: 0074 006f 0072 0800 0000 0006 0000 000e  .t.o.r..........
-00007450: 436c 6173 7320 7365 6c65 6374 6f72 0700  Class selector..
-00007460: 0000 0c51 7363 694c 6578 6572 4353 5301  ...QsciLexerCSS.
-00007470: 0300 0000 1000 5300 7400 6100 6e00 6400  ......S.t.a.n.d.
-00007480: 6100 7200 6408 0000 0000 0600 0000 0744  a.r.d..........D
-00007490: 6566 6175 6c74 0700 0000 0c51 7363 694c  efault.....QsciL
-000074a0: 6578 6572 4353 5301 0300 0000 4200 5a00  exerCSS.....B.Z.
-000074b0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-000074c0: 7400 7400 6500 2000 6900 6e00 2000 4100  t.t.e. .i.n. .A.
-000074d0: 6e00 6600 fc00 6800 7200 7500 6e00 6700  n.f...h.r.u.n.g.
-000074e0: 7300 7a00 6500 6900 6300 6800 6500 6e08  s.z.e.i.c.h.e.n.
-000074f0: 0000 0000 0600 0000 1444 6f75 626c 652d  .........Double-
-00007500: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
-00007510: 000c 5173 6369 4c65 7865 7243 5353 0103  ..QsciLexerCSS..
-00007520: 0000 0034 0045 0072 0077 0065 0069 0074  ...4.E.r.w.e.i.t
-00007530: 0065 0072 0074 0065 0020 0043 0053 0053  .e.r.t.e. .C.S.S
-00007540: 0020 0045 0069 0067 0065 006e 0073 0063  . .E.i.g.e.n.s.c
-00007550: 0068 0061 0066 0074 0800 0000 0006 0000  .h.a.f.t........
-00007560: 0015 4578 7465 6e64 6564 2043 5353 2070  ..Extended CSS p
-00007570: 726f 7065 7274 7907 0000 000c 5173 6369  roperty.....Qsci
-00007580: 4c65 7865 7243 5353 0103 0000 002e 0045  LexerCSS.......E
-00007590: 0072 0077 0065 0069 0074 0065 0072 0074  .r.w.e.i.t.e.r.t
-000075a0: 0065 0020 0050 0073 0065 0075 0064 006f  .e. .P.s.e.u.d.o
-000075b0: 006b 006c 0061 0073 0073 0065 0800 0000  .k.l.a.s.s.e....
-000075c0: 0006 0000 0015 4578 7465 6e64 6564 2070  ......Extended p
-000075d0: 7365 7564 6f2d 636c 6173 7307 0000 000c  seudo-class.....
-000075e0: 5173 6369 4c65 7865 7243 5353 0103 0000  QsciLexerCSS....
-000075f0: 0032 0045 0072 0077 0065 0069 0074 0065  .2.E.r.w.e.i.t.e
-00007600: 0072 0074 0065 0073 0020 0050 0073 0065  .r.t.e.s. .P.s.e
-00007610: 0075 0064 006f 0065 006c 0065 006d 0065  .u.d.o.e.l.e.m.e
-00007620: 006e 0074 0800 0000 0006 0000 0017 4578  .n.t..........Ex
-00007630: 7465 6e64 6564 2070 7365 7564 6f2d 656c  tended pseudo-el
-00007640: 656d 656e 7407 0000 000c 5173 6369 4c65  ement.....QsciLe
-00007650: 7865 7243 5353 0103 0000 0016 0049 0044  xerCSS.......I.D
-00007660: 002d 0053 0065 006c 0065 006b 0074 006f  .-.S.e.l.e.k.t.o
-00007670: 0072 0800 0000 0006 0000 000b 4944 2073  .r..........ID s
-00007680: 656c 6563 746f 7207 0000 000c 5173 6369  elector.....Qsci
-00007690: 4c65 7865 7243 5353 0103 0000 000e 0057  LexerCSS.......W
-000076a0: 0069 0063 0068 0074 0069 0067 0800 0000  .i.c.h.t.i.g....
-000076b0: 0006 0000 0009 496d 706f 7274 616e 7407  ......Important.
-000076c0: 0000 000c 5173 6369 4c65 7865 7243 5353  ....QsciLexerCSS
-000076d0: 0103 0000 0016 004d 0065 0064 0069 0065  .......M.e.d.i.e
-000076e0: 006e 0072 0065 0067 0065 006c 0800 0000  .n.r.e.g.e.l....
-000076f0: 0006 0000 000a 4d65 6469 6120 7275 6c65  ......Media rule
-00007700: 0700 0000 0c51 7363 694c 6578 6572 4353  .....QsciLexerCS
-00007710: 5301 0300 0000 1000 4f00 7000 6500 7200  S.......O.p.e.r.
-00007720: 6100 7400 6f00 7208 0000 0000 0600 0000  a.t.o.r.........
-00007730: 084f 7065 7261 746f 7207 0000 000c 5173  .Operator.....Qs
-00007740: 6369 4c65 7865 7243 5353 0103 0000 0018  ciLexerCSS......
-00007750: 0050 0073 0065 0075 0064 006f 006b 006c  .P.s.e.u.d.o.k.l
-00007760: 0061 0073 0073 0065 0800 0000 0006 0000  .a.s.s.e........
-00007770: 000c 5073 6575 646f 2d63 6c61 7373 0700  ..Pseudo-class..
-00007780: 0000 0c51 7363 694c 6578 6572 4353 5301  ...QsciLexerCSS.
-00007790: 0300 0000 1a00 5000 7300 6500 7500 6400  ......P.s.e.u.d.
-000077a0: 6f00 6500 6c00 6500 6d00 6500 6e00 7408  o.e.l.e.m.e.n.t.
-000077b0: 0000 0000 0600 0000 0e50 7365 7564 6f2d  .........Pseudo-
-000077c0: 656c 656d 656e 7407 0000 000c 5173 6369  element.....Qsci
-000077d0: 4c65 7865 7243 5353 0103 0000 0036 005a  LexerCSS.....6.Z
-000077e0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-000077f0: 0074 0074 0065 0020 0069 006e 0020 0048  .t.t.e. .i.n. .H
-00007800: 006f 0063 0068 006b 006f 006d 006d 0061  .o.c.h.k.o.m.m.a
-00007810: 0074 0061 0800 0000 0006 0000 0014 5369  .t.a..........Si
-00007820: 6e67 6c65 2d71 756f 7465 6420 7374 7269  ngle-quoted stri
-00007830: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
-00007840: 4353 5301 0300 0000 0600 5400 6100 6708  CSS.......T.a.g.
-00007850: 0000 0000 0600 0000 0354 6167 0700 0000  .........Tag....
-00007860: 0c51 7363 694c 6578 6572 4353 5301 0300  .QsciLexerCSS...
-00007870: 0000 2c00 5500 6e00 6200 6500 6b00 6100  ..,.U.n.b.e.k.a.
-00007880: 6e00 6e00 7400 6500 2000 4500 6900 6700  n.n.t.e. .E.i.g.
-00007890: 6500 6e00 7300 6300 6800 6100 6600 7408  e.n.s.c.h.a.f.t.
-000078a0: 0000 0000 0600 0000 1055 6e6b 6e6f 776e  .........Unknown
-000078b0: 2070 726f 7065 7274 7907 0000 000c 5173   property.....Qs
-000078c0: 6369 4c65 7865 7243 5353 0103 0000 002e  ciLexerCSS......
-000078d0: 0055 006e 0062 0065 006b 0061 006e 006e  .U.n.b.e.k.a.n.n
-000078e0: 0074 0065 0020 0050 0073 0065 0075 0064  .t.e. .P.s.e.u.d
-000078f0: 006f 006b 006c 0061 0073 0073 0065 0800  .o.k.l.a.s.s.e..
-00007900: 0000 0006 0000 0014 556e 6b6e 6f77 6e20  ........Unknown 
-00007910: 7073 6575 646f 2d63 6c61 7373 0700 0000  pseudo-class....
-00007920: 0c51 7363 694c 6578 6572 4353 5301 0300  .QsciLexerCSS...
-00007930: 0000 0800 5700 6500 7200 7408 0000 0000  ....W.e.r.t.....
-00007940: 0600 0000 0556 616c 7565 0700 0000 0c51  .....Value.....Q
-00007950: 7363 694c 6578 6572 4353 5301 0300 0000  sciLexerCSS.....
-00007960: 1000 5600 6100 7200 6900 6100 6200 6c00  ..V.a.r.i.a.b.l.
-00007970: 6508 0000 0000 0600 0000 0856 6172 6961  e..........Varia
-00007980: 626c 6507 0000 000c 5173 6369 4c65 7865  ble.....QsciLexe
-00007990: 7243 5353 0103 0000 003a 0055 006e 0069  rCSS.....:.U.n.i
-000079a0: 006e 0074 0065 0072 0070 0072 0065 0074  .n.t.e.r.p.r.e.t
-000079b0: 0069 0065 0072 0074 0065 0020 005a 0065  .i.e.r.t.e. .Z.e
-000079c0: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-000079d0: 0074 0065 0800 0000 0006 0000 000f 5665  .t.e..........Ve
-000079e0: 7262 6174 696d 2073 7472 696e 6707 0000  rbatim string...
-000079f0: 000f 5173 6369 4c65 7865 7243 5368 6172  ..QsciLexerCShar
-00007a00: 7001 0300 0000 1c00 4200 6c00 6f00 6300  p.......B.l.o.c.
-00007a10: 6b00 6b00 6f00 6d00 6d00 6500 6e00 7400  k.k.o.m.m.e.n.t.
-00007a20: 6100 7208 0000 0000 0600 0000 0d42 6c6f  a.r..........Blo
-00007a30: 636b 2063 6f6d 6d65 6e74 0700 0000 1551  ck comment.....Q
-00007a40: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
-00007a50: 7269 7074 0103 0000 0030 0052 0065 0067  ript.....0.R.e.g
-00007a60: 0075 006c 00e4 0072 0065 0072 0020 0041  .u.l...r.e.r. .A
-00007a70: 0075 0073 0064 0072 0075 0063 006b 0073  .u.s.d.r.u.c.k.s
-00007a80: 0062 006c 006f 0063 006b 0800 0000 0006  .b.l.o.c.k......
-00007a90: 0000 0018 426c 6f63 6b20 7265 6775 6c61  ....Block regula
-00007aa0: 7220 6578 7072 6573 7369 6f6e 0700 0000  r expression....
-00007ab0: 1551 7363 694c 6578 6572 436f 6666 6565  .QsciLexerCoffee
-00007ac0: 5363 7269 7074 0103 0000 0042 0052 0065  Script.....B.R.e
-00007ad0: 0067 0075 006c 00e4 0072 0065 0072 0020  .g.u.l...r.e.r. 
-00007ae0: 0041 0075 0073 0064 0072 0075 0063 006b  .A.u.s.d.r.u.c.k
-00007af0: 0073 0062 006c 006f 0063 006b 006b 006f  .s.b.l.o.c.k.k.o
-00007b00: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-00007b10: 0000 0006 0000 0020 426c 6f63 6b20 7265  ....... Block re
-00007b20: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
-00007b30: 2063 6f6d 6d65 6e74 0700 0000 1551 7363   comment.....Qsc
-00007b40: 694c 6578 6572 436f 6666 6565 5363 7269  iLexerCoffeeScri
-00007b50: 7074 0103 0000 0040 0055 006e 0069 006e  pt.....@.U.n.i.n
-00007b60: 0074 0065 0072 0070 0072 0065 0074 0069  .t.e.r.p.r.e.t.i
-00007b70: 0065 0072 0074 0065 0020 0043 0023 0020  .e.r.t.e. .C.#. 
-00007b80: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-00007b90: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
-00007ba0: 0012 4323 2076 6572 6261 7469 6d20 7374  ..C# verbatim st
-00007bb0: 7269 6e67 0700 0000 1551 7363 694c 6578  ring.....QsciLex
-00007bc0: 6572 436f 6666 6565 5363 7269 7074 0103  erCoffeeScript..
-00007bd0: 0000 001a 0043 002b 002b 0020 004b 006f  .....C.+.+. .K.o
-00007be0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-00007bf0: 0000 0006 0000 0011 432b 2b2d 7374 796c  ........C++-styl
-00007c00: 6520 636f 6d6d 656e 7407 0000 0015 5173  e comment.....Qs
-00007c10: 6369 4c65 7865 7243 6f66 6665 6553 6372  ciLexerCoffeeScr
-00007c20: 6970 7401 0300 0000 1600 4300 2000 4b00  ipt.......C. .K.
-00007c30: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-00007c40: 0000 0000 0600 0000 0f43 2d73 7479 6c65  .........C-style
-00007c50: 2063 6f6d 6d65 6e74 0700 0000 1551 7363   comment.....Qsc
-00007c60: 694c 6578 6572 436f 6666 6565 5363 7269  iLexerCoffeeScri
-00007c70: 7074 0103 0000 0010 0053 0074 0061 006e  pt.......S.t.a.n
-00007c80: 0064 0061 0072 0064 0800 0000 0006 0000  .d.a.r.d........
-00007c90: 0007 4465 6661 756c 7407 0000 0015 5173  ..Default.....Qs
-00007ca0: 6369 4c65 7865 7243 6f66 6665 6553 6372  ciLexerCoffeeScr
-00007cb0: 6970 7401 0300 0000 4200 5a00 6500 6900  ipt.....B.Z.e.i.
-00007cc0: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00007cd0: 6500 2000 6900 6e00 2000 4100 6e00 6600  e. .i.n. .A.n.f.
-00007ce0: fc00 6800 7200 7500 6e00 6700 7300 7a00  ..h.r.u.n.g.s.z.
-00007cf0: 6500 6900 6300 6800 6500 6e08 0000 0000  e.i.c.h.e.n.....
-00007d00: 0600 0000 1444 6f75 626c 652d 7175 6f74  .....Double-quot
-00007d10: 6564 2073 7472 696e 6707 0000 0015 5173  ed string.....Qs
-00007d20: 6369 4c65 7865 7243 6f66 6665 6553 6372  ciLexerCoffeeScr
-00007d30: 6970 7401 0300 0000 1e00 4700 6c00 6f00  ipt.......G.l.o.
-00007d40: 6200 6100 6c00 6500 2000 4b00 6c00 6100  b.a.l.e. .K.l.a.
-00007d50: 7300 7300 6500 6e08 0000 0000 0600 0000  s.s.e.n.........
-00007d60: 0e47 6c6f 6261 6c20 636c 6173 7365 7307  .Global classes.
-00007d70: 0000 0015 5173 6369 4c65 7865 7243 6f66  ....QsciLexerCof
-00007d80: 6665 6553 6372 6970 7401 0300 0000 1000  feeScript.......
-00007d90: 4900 4400 4c00 2000 5500 5500 4900 4408  I.D.L. .U.U.I.D.
-00007da0: 0000 0000 0600 0000 0849 444c 2055 5549  .........IDL UUI
-00007db0: 4407 0000 0015 5173 6369 4c65 7865 7243  D.....QsciLexerC
-00007dc0: 6f66 6665 6553 6372 6970 7401 0300 0000  offeeScript.....
-00007dd0: 1400 4200 6500 7a00 6500 6900 6300 6800  ..B.e.z.e.i.c.h.
-00007de0: 6e00 6500 7208 0000 0000 0600 0000 0a49  n.e.r..........I
-00007df0: 6465 6e74 6966 6965 7207 0000 0015 5173  dentifier.....Qs
-00007e00: 6369 4c65 7865 7243 6f66 6665 6553 6372  ciLexerCoffeeScr
-00007e10: 6970 7401 0300 0000 2600 4900 6e00 7300  ipt.....&.I.n.s.
-00007e20: 7400 6100 6e00 7a00 2d00 4500 6900 6700  t.a.n.z.-.E.i.g.
-00007e30: 6500 6e00 7300 6300 6800 6100 6600 7408  e.n.s.c.h.a.f.t.
-00007e40: 0000 0000 0600 0000 1149 6e73 7461 6e63  .........Instanc
-00007e50: 6520 7072 6f70 6572 7479 0700 0000 1551  e property.....Q
-00007e60: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
-00007e70: 7269 7074 0103 0000 002a 004a 0061 0076  ript.....*.J.a.v
-00007e80: 0061 0044 006f 0063 0020 0043 002b 002b  .a.D.o.c. .C.+.+
-00007e90: 0020 004b 006f 006d 006d 0065 006e 0074  . .K.o.m.m.e.n.t
-00007ea0: 0061 0072 0800 0000 0006 0000 0019 4a61  .a.r..........Ja
-00007eb0: 7661 446f 6320 432b 2b2d 7374 796c 6520  vaDoc C++-style 
-00007ec0: 636f 6d6d 656e 7407 0000 0015 5173 6369  comment.....Qsci
-00007ed0: 4c65 7865 7243 6f66 6665 6553 6372 6970  LexerCoffeeScrip
-00007ee0: 7401 0300 0000 2600 4a00 6100 7600 6100  t.....&.J.a.v.a.
-00007ef0: 4400 6f00 6300 2000 4300 2000 4b00 6f00  D.o.c. .C. .K.o.
-00007f00: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
-00007f10: 0000 0600 0000 174a 6176 6144 6f63 2043  .......JavaDoc C
-00007f20: 2d73 7479 6c65 2063 6f6d 6d65 6e74 0700  -style comment..
-00007f30: 0000 1551 7363 694c 6578 6572 436f 6666  ...QsciLexerCoff
-00007f40: 6565 5363 7269 7074 0103 0000 002a 004a  eeScript.....*.J
-00007f50: 0061 0076 0061 0044 006f 0063 0020 0053  .a.v.a.D.o.c. .S
-00007f60: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
-00007f70: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
-00007f80: 000f 4a61 7661 446f 6320 6b65 7977 6f72  ..JavaDoc keywor
-00007f90: 6407 0000 0015 5173 6369 4c65 7865 7243  d.....QsciLexerC
-00007fa0: 6f66 6665 6553 6372 6970 7401 0300 0000  offeeScript.....
-00007fb0: 3600 4a00 6100 7600 6100 4400 6f00 6300  6.J.a.v.a.D.o.c.
-00007fc0: 2000 5300 6300 6800 6c00 fc00 7300 7300   .S.c.h.l...s.s.
-00007fd0: 6500 6c00 7700 6f00 7200 7400 6600 6500  e.l.w.o.r.t.f.e.
-00007fe0: 6800 6c00 6500 7208 0000 0000 0600 0000  h.l.e.r.........
-00007ff0: 154a 6176 6144 6f63 206b 6579 776f 7264  .JavaDoc keyword
-00008000: 2065 7272 6f72 0700 0000 1551 7363 694c   error.....QsciL
-00008010: 6578 6572 436f 6666 6565 5363 7269 7074  exerCoffeeScript
-00008020: 0103 0000 001a 0053 0063 0068 006c 00fc  .......S.c.h.l..
-00008030: 0073 0073 0065 006c 0077 006f 0072 0074  .s.s.e.l.w.o.r.t
-00008040: 0800 0000 0006 0000 0007 4b65 7977 6f72  ..........Keywor
-00008050: 6407 0000 0015 5173 6369 4c65 7865 7243  d.....QsciLexerC
-00008060: 6f66 6665 6553 6372 6970 7401 0300 0000  offeeScript.....
-00008070: 0800 5a00 6100 6800 6c08 0000 0000 0600  ..Z.a.h.l.......
-00008080: 0000 064e 756d 6265 7207 0000 0015 5173  ...Number.....Qs
-00008090: 6369 4c65 7865 7243 6f66 6665 6553 6372  ciLexerCoffeeScr
-000080a0: 6970 7401 0300 0000 1000 4f00 7000 6500  ipt.......O.p.e.
-000080b0: 7200 6100 7400 6f00 7208 0000 0000 0600  r.a.t.o.r.......
-000080c0: 0000 084f 7065 7261 746f 7207 0000 0015  ...Operator.....
-000080d0: 5173 6369 4c65 7865 7243 6f66 6665 6553  QsciLexerCoffeeS
-000080e0: 6372 6970 7401 0300 0000 2200 5000 7200  cript.....".P.r.
-000080f0: e400 7000 7200 6f00 7a00 6500 7300 7300  ..p.r.o.z.e.s.s.
-00008100: 6f00 7200 6200 6c00 6f00 6300 6b08 0000  o.r.b.l.o.c.k...
-00008110: 0000 0600 0000 1350 7265 2d70 726f 6365  .......Pre-proce
-00008120: 7373 6f72 2062 6c6f 636b 0700 0000 1551  ssor block.....Q
-00008130: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
-00008140: 7269 7074 0103 0000 0024 0052 0065 0067  ript.....$.R.e.g
-00008150: 0075 006c 00e4 0072 0065 0072 0020 0041  .u.l...r.e.r. .A
-00008160: 0075 0073 0064 0072 0075 0063 006b 0800  .u.s.d.r.u.c.k..
-00008170: 0000 0006 0000 0012 5265 6775 6c61 7220  ........Regular 
-00008180: 6578 7072 6573 7369 6f6e 0700 0000 1551  expression.....Q
-00008190: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
-000081a0: 7269 7074 0103 0000 0050 0053 0065 006b  ript.....P.S.e.k
-000081b0: 0075 006e 0064 00e4 0072 0065 0020 0053  .u.n.d...r.e. .S
-000081c0: 0063 0068 006c 0075 0073 0073 0065 006c  .c.h.l.u.s.s.e.l
-000081d0: 0077 00f6 0072 0074 0065 0072 0020 0075  .w...r.t.e.r. .u
-000081e0: 006e 0064 0020 0042 0065 007a 0065 0069  .n.d. .B.e.z.e.i
-000081f0: 0063 0068 006e 0065 0072 0800 0000 0006  .c.h.n.e.r......
-00008200: 0000 0022 5365 636f 6e64 6172 7920 6b65  ..."Secondary ke
-00008210: 7977 6f72 6473 2061 6e64 2069 6465 6e74  ywords and ident
-00008220: 6966 6965 7273 0700 0000 1551 7363 694c  ifiers.....QsciL
-00008230: 6578 6572 436f 6666 6565 5363 7269 7074  exerCoffeeScript
-00008240: 0103 0000 0036 005a 0065 0069 0063 0068  .....6.Z.e.i.c.h
-00008250: 0065 006e 006b 0065 0074 0074 0065 0020  .e.n.k.e.t.t.e. 
-00008260: 0069 006e 0020 0048 006f 0063 0068 006b  .i.n. .H.o.c.h.k
-00008270: 006f 006d 006d 0061 0074 0061 0800 0000  .o.m.m.a.t.a....
-00008280: 0006 0000 0014 5369 6e67 6c65 2d71 756f  ......Single-quo
-00008290: 7465 6420 7374 7269 6e67 0700 0000 1551  ted string.....Q
-000082a0: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
-000082b0: 7269 7074 0103 0000 002e 0055 006e 0062  ript.......U.n.b
-000082c0: 0065 0065 006e 0064 0065 0074 0065 0020  .e.e.n.d.e.t.e. 
-000082d0: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-000082e0: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
-000082f0: 000f 556e 636c 6f73 6564 2073 7472 696e  ..Unclosed strin
-00008300: 6707 0000 0015 5173 6369 4c65 7865 7243  g.....QsciLexerC
-00008310: 6f66 6665 6553 6372 6970 7401 0300 0000  offeeScript.....
-00008320: 4200 5a00 6500 6900 6300 6800 6500 6e00  B.Z.e.i.c.h.e.n.
-00008330: 6b00 6500 7400 7400 6500 2000 6900 6e00  k.e.t.t.e. .i.n.
-00008340: 2000 5200 fc00 6300 6b00 7700 e400 7200   .R...c.k.w...r.
-00008350: 7400 7300 7300 7400 7200 6900 6300 6800  t.s.s.t.r.i.c.h.
-00008360: 6500 6e08 0000 0000 0600 0000 1142 6163  e.n..........Bac
-00008370: 6b71 756f 7465 6420 7374 7269 6e67 0700  kquoted string..
-00008380: 0000 0a51 7363 694c 6578 6572 4401 0300  ...QsciLexerD...
-00008390: 0000 1c00 4200 6c00 6f00 6300 6b00 6b00  ....B.l.o.c.k.k.
-000083a0: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-000083b0: 0000 0000 0600 0000 0d42 6c6f 636b 2063  .........Block c
-000083c0: 6f6d 6d65 6e74 0700 0000 0a51 7363 694c  omment.....QsciL
-000083d0: 6578 6572 4401 0300 0000 0e00 5a00 6500  exerD.......Z.e.
-000083e0: 6900 6300 6800 6500 6e08 0000 0000 0600  i.c.h.e.n.......
-000083f0: 0000 0943 6861 7261 6374 6572 0700 0000  ...Character....
-00008400: 0a51 7363 694c 6578 6572 4401 0300 0000  .QsciLexerD.....
-00008410: 2400 4400 4400 6f00 6300 2000 5300 6300  $.D.D.o.c. .S.c.
-00008420: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
-00008430: 6f00 7200 7408 0000 0000 0600 0000 0c44  o.r.t..........D
-00008440: 446f 6320 6b65 7977 6f72 6407 0000 000a  Doc keyword.....
-00008450: 5173 6369 4c65 7865 7244 0103 0000 0030  QsciLexerD.....0
-00008460: 0044 0044 006f 0063 0020 0053 0063 0068  .D.D.o.c. .S.c.h
-00008470: 006c 00fc 0073 0073 0065 006c 0077 006f  .l...s.s.e.l.w.o
-00008480: 0072 0074 0066 0065 0068 006c 0065 0072  .r.t.f.e.h.l.e.r
-00008490: 0800 0000 0006 0000 0012 4444 6f63 206b  ..........DDoc k
-000084a0: 6579 776f 7264 2065 7272 6f72 0700 0000  eyword error....
-000084b0: 0a51 7363 694c 6578 6572 4401 0300 0000  .QsciLexerD.....
-000084c0: 2600 4400 4400 6f00 6300 2000 4200 6c00  &.D.D.o.c. .B.l.
-000084d0: 6f00 6300 6b00 6b00 6f00 6d00 6d00 6500  o.c.k.k.o.m.m.e.
-000084e0: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
-000084f0: 1844 446f 6320 7374 796c 6520 626c 6f63  .DDoc style bloc
-00008500: 6b20 636f 6d6d 656e 7407 0000 000a 5173  k comment.....Qs
-00008510: 6369 4c65 7865 7244 0103 0000 0028 0044  ciLexerD.....(.D
-00008520: 0044 006f 0063 0020 005a 0065 0069 006c  .D.o.c. .Z.e.i.l
-00008530: 0065 006e 006b 006f 006d 006d 0065 006e  .e.n.k.o.m.m.e.n
-00008540: 0074 0061 0072 0800 0000 0006 0000 0017  .t.a.r..........
-00008550: 4444 6f63 2073 7479 6c65 206c 696e 6520  DDoc style line 
-00008560: 636f 6d6d 656e 7407 0000 000a 5173 6369  comment.....Qsci
-00008570: 4c65 7865 7244 0103 0000 0010 0053 0074  LexerD.......S.t
-00008580: 0061 006e 0064 0061 0072 0064 0800 0000  .a.n.d.a.r.d....
-00008590: 0006 0000 0007 4465 6661 756c 7407 0000  ......Default...
-000085a0: 000a 5173 6369 4c65 7865 7244 0103 0000  ..QsciLexerD....
-000085b0: 0036 0044 006f 006b 0075 006d 0065 006e  .6.D.o.k.u.m.e.n
-000085c0: 0074 0061 0074 0069 006f 006e 0073 0073  .t.a.t.i.o.n.s.s
-000085d0: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
-000085e0: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
-000085f0: 0015 446f 6375 6d65 6e74 6174 696f 6e20  ..Documentation 
-00008600: 6b65 7977 6f72 6407 0000 000a 5173 6369  keyword.....Qsci
-00008610: 4c65 7865 7244 0103 0000 0014 0042 0065  LexerD.......B.e
-00008620: 007a 0065 0069 0063 0068 006e 0065 0072  .z.e.i.c.h.n.e.r
-00008630: 0800 0000 0006 0000 000a 4964 656e 7469  ..........Identi
-00008640: 6669 6572 0700 0000 0a51 7363 694c 6578  fier.....QsciLex
-00008650: 6572 4401 0300 0000 1a00 5300 6300 6800  erD.......S.c.h.
-00008660: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
-00008670: 7200 7408 0000 0000 0600 0000 074b 6579  r.t..........Key
-00008680: 776f 7264 0700 0000 0a51 7363 694c 6578  word.....QsciLex
-00008690: 6572 4401 0300 0000 1e00 5a00 6500 6900  erD.......Z.e.i.
-000086a0: 6c00 6500 6e00 6b00 6f00 6d00 6d00 6500  l.e.n.k.o.m.m.e.
-000086b0: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
-000086c0: 0c4c 696e 6520 636f 6d6d 656e 7407 0000  .Line comment...
-000086d0: 000a 5173 6369 4c65 7865 7244 0103 0000  ..QsciLexerD....
-000086e0: 0030 0073 0063 0068 0061 0063 0068 0074  .0.s.c.h.a.c.h.t
-000086f0: 0065 006c 0062 0061 0072 0065 0072 0020  .e.l.b.a.r.e.r. 
-00008700: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
-00008710: 0072 0800 0000 0006 0000 000f 4e65 7374  .r..........Nest
-00008720: 696e 6720 636f 6d6d 656e 7407 0000 000a  ing comment.....
-00008730: 5173 6369 4c65 7865 7244 0103 0000 0008  QsciLexerD......
-00008740: 005a 0061 0068 006c 0800 0000 0006 0000  .Z.a.h.l........
-00008750: 0006 4e75 6d62 6572 0700 0000 0a51 7363  ..Number.....Qsc
-00008760: 694c 6578 6572 4401 0300 0000 1000 4f00  iLexerD.......O.
-00008770: 7000 6500 7200 6100 7400 6f00 7208 0000  p.e.r.a.t.o.r...
-00008780: 0000 0600 0000 084f 7065 7261 746f 7207  .......Operator.
-00008790: 0000 000a 5173 6369 4c65 7865 7244 0103  ....QsciLexerD..
-000087a0: 0000 0022 0052 006f 0068 0065 0020 005a  ...".R.o.h.e. .Z
-000087b0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-000087c0: 0074 0074 0065 0800 0000 0006 0000 000a  .t.t.e..........
-000087d0: 5261 7720 7374 7269 6e67 0700 0000 0a51  Raw string.....Q
-000087e0: 7363 694c 6578 6572 4401 0300 0000 3000  sciLexerD.....0.
-000087f0: 5300 6500 6b00 7500 6e00 6400 e400 7200  S.e.k.u.n.d...r.
-00008800: 6500 7300 2000 5300 6300 6800 6c00 fc00  e.s. .S.c.h.l...
-00008810: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
-00008820: 0000 0000 0600 0000 1153 6563 6f6e 6461  .........Seconda
-00008830: 7279 206b 6579 776f 7264 0700 0000 0a51  ry keyword.....Q
-00008840: 7363 694c 6578 6572 4401 0300 0000 1800  sciLexerD.......
-00008850: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
-00008860: 6500 7400 7400 6508 0000 0000 0600 0000  e.t.t.e.........
-00008870: 0653 7472 696e 6707 0000 000a 5173 6369  .String.....Qsci
-00008880: 4c65 7865 7244 0103 0000 001a 0054 0079  LexerD.......T.y
-00008890: 0070 0064 0065 0066 0069 006e 0069 0074  .p.d.e.f.i.n.i.t
-000088a0: 0069 006f 006e 0800 0000 0006 0000 000f  .i.o.n..........
-000088b0: 5479 7065 2064 6566 696e 6974 696f 6e07  Type definition.
-000088c0: 0000 000a 5173 6369 4c65 7865 7244 0103  ....QsciLexerD..
-000088d0: 0000 002e 0055 006e 0062 0065 0065 006e  .....U.n.b.e.e.n
-000088e0: 0064 0065 0074 0065 0020 005a 0065 0069  .d.e.t.e. .Z.e.i
-000088f0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00008900: 0065 0800 0000 0006 0000 000f 556e 636c  .e..........Uncl
-00008910: 6f73 6564 2073 7472 696e 6707 0000 000a  osed string.....
-00008920: 5173 6369 4c65 7865 7244 0103 0000 0024  QsciLexerD.....$
-00008930: 004e 0075 0074 007a 0065 0072 0020 0064  .N.u.t.z.e.r. .d
-00008940: 0065 0066 0069 006e 0069 0065 0072 0074  .e.f.i.n.i.e.r.t
-00008950: 0020 0031 0800 0000 0006 0000 000e 5573  . .1..........Us
-00008960: 6572 2064 6566 696e 6564 2031 0700 0000  er defined 1....
-00008970: 0a51 7363 694c 6578 6572 4401 0300 0000  .QsciLexerD.....
-00008980: 2400 4e00 7500 7400 7a00 6500 7200 2000  $.N.u.t.z.e.r. .
-00008990: 6400 6500 6600 6900 6e00 6900 6500 7200  d.e.f.i.n.i.e.r.
-000089a0: 7400 2000 3208 0000 0000 0600 0000 0e55  t. .2..........U
-000089b0: 7365 7220 6465 6669 6e65 6420 3207 0000  ser defined 2...
-000089c0: 000a 5173 6369 4c65 7865 7244 0103 0000  ..QsciLexerD....
-000089d0: 0024 004e 0075 0074 007a 0065 0072 0020  .$.N.u.t.z.e.r. 
-000089e0: 0064 0065 0066 0069 006e 0069 0065 0072  .d.e.f.i.n.i.e.r
-000089f0: 0074 0020 0033 0800 0000 0006 0000 000e  .t. .3..........
-00008a00: 5573 6572 2064 6566 696e 6564 2033 0700  User defined 3..
-00008a10: 0000 0a51 7363 694c 6578 6572 4401 0300  ...QsciLexerD...
-00008a20: 0000 3a00 4800 6900 6e00 7a00 7500 6700  ..:.H.i.n.z.u.g.
-00008a30: 6500 6600 fc00 6700 7400 6500 7200 2000  e.f...g.t.e.r. .
-00008a40: 4500 7200 6700 e400 6e00 7a00 7500 6e00  E.r.g...n.z.u.n.
-00008a50: 6700 7300 7000 6100 7400 6300 6808 0000  g.s.p.a.t.c.h...
-00008a60: 0000 0600 0000 1241 6464 6564 2061 6464  .......Added add
-00008a70: 696e 6720 7061 7463 6807 0000 000d 5173  ing patch.....Qs
-00008a80: 6369 4c65 7865 7244 6966 6601 0300 0000  ciLexerDiff.....
-00008a90: 2400 4800 6900 6e00 7a00 7500 6700 6500  $.H.i.n.z.u.g.e.
-00008aa0: 6600 fc00 6700 7400 6500 2000 5a00 6500  f...g.t.e. .Z.e.
-00008ab0: 6900 6c00 6508 0000 0000 0600 0000 0a41  i.l.e..........A
-00008ac0: 6464 6564 206c 696e 6507 0000 000d 5173  dded line.....Qs
-00008ad0: 6369 4c65 7865 7244 6966 6601 0300 0000  ciLexerDiff.....
-00008ae0: 3c00 4800 6900 6e00 7a00 7500 6700 6500  <.H.i.n.z.u.g.e.
-00008af0: 6600 fc00 6700 7400 6500 7200 2000 4500  f...g.t.e.r. .E.
-00008b00: 6e00 7400 6600 6500 7200 6e00 7500 6e00  n.t.f.e.r.n.u.n.
-00008b10: 6700 7300 7000 6100 7400 6300 6808 0000  g.s.p.a.t.c.h...
-00008b20: 0000 0600 0000 1441 6464 6564 2072 656d  .......Added rem
-00008b30: 6f76 696e 6720 7061 7463 6807 0000 000d  oving patch.....
-00008b40: 5173 6369 4c65 7865 7244 6966 6601 0300  QsciLexerDiff...
-00008b50: 0000 1e00 4700 6500 e400 6e00 6400 6500  ....G.e...n.d.e.
-00008b60: 7200 7400 6500 2000 5a00 6500 6900 6c00  r.t.e. .Z.e.i.l.
-00008b70: 6508 0000 0000 0600 0000 0c43 6861 6e67  e..........Chang
-00008b80: 6564 206c 696e 6507 0000 000d 5173 6369  ed line.....Qsci
-00008b90: 4c65 7865 7244 6966 6601 0300 0000 0c00  LexerDiff.......
-00008ba0: 4200 6500 6600 6500 6800 6c08 0000 0000  B.e.f.e.h.l.....
-00008bb0: 0600 0000 0743 6f6d 6d61 6e64 0700 0000  .....Command....
-00008bc0: 0d51 7363 694c 6578 6572 4469 6666 0103  .QsciLexerDiff..
-00008bd0: 0000 0012 004b 006f 006d 006d 0065 006e  .....K.o.m.m.e.n
-00008be0: 0074 0061 0072 0800 0000 0006 0000 0007  .t.a.r..........
-00008bf0: 436f 6d6d 656e 7407 0000 000d 5173 6369  Comment.....Qsci
-00008c00: 4c65 7865 7244 6966 6601 0300 0000 1000  LexerDiff.......
-00008c10: 5300 7400 6100 6e00 6400 6100 7200 6408  S.t.a.n.d.a.r.d.
-00008c20: 0000 0000 0600 0000 0744 6566 6175 6c74  .........Default
-00008c30: 0700 0000 0d51 7363 694c 6578 6572 4469  .....QsciLexerDi
-00008c40: 6666 0103 0000 0014 004b 006f 0070 0066  ff.......K.o.p.f
-00008c50: 007a 0065 0069 006c 0065 006e 0800 0000  .z.e.i.l.e.n....
-00008c60: 0006 0000 0006 4865 6164 6572 0700 0000  ......Header....
-00008c70: 0d51 7363 694c 6578 6572 4469 6666 0103  .QsciLexerDiff..
-00008c80: 0000 0010 0050 006f 0073 0069 0074 0069  .....P.o.s.i.t.i
-00008c90: 006f 006e 0800 0000 0006 0000 0008 506f  .o.n..........Po
-00008ca0: 7369 7469 6f6e 0700 0000 0d51 7363 694c  sition.....QsciL
-00008cb0: 6578 6572 4469 6666 0103 0000 0034 0045  exerDiff.....4.E
-00008cc0: 006e 0074 0066 0065 0072 006e 0074 0065  .n.t.f.e.r.n.t.e
-00008cd0: 0072 0020 0045 0072 0067 00e4 006e 007a  .r. .E.r.g...n.z
-00008ce0: 0075 006e 0067 0073 0070 0061 0074 0063  .u.n.g.s.p.a.t.c
-00008cf0: 0068 0800 0000 0006 0000 0014 5265 6d6f  .h..........Remo
-00008d00: 7665 6420 6164 6469 6e67 2070 6174 6368  ved adding patch
-00008d10: 0700 0000 0d51 7363 694c 6578 6572 4469  .....QsciLexerDi
-00008d20: 6666 0103 0000 001e 0045 006e 0074 0066  ff.......E.n.t.f
-00008d30: 0065 0072 006e 0074 0065 0020 005a 0065  .e.r.n.t.e. .Z.e
-00008d40: 0069 006c 0065 0800 0000 0006 0000 000c  .i.l.e..........
-00008d50: 5265 6d6f 7665 6420 6c69 6e65 0700 0000  Removed line....
-00008d60: 0d51 7363 694c 6578 6572 4469 6666 0103  .QsciLexerDiff..
-00008d70: 0000 0036 0045 006e 0074 0066 0065 0072  ...6.E.n.t.f.e.r
-00008d80: 006e 0074 0065 0072 0020 0045 006e 0074  .n.t.e.r. .E.n.t
-00008d90: 0066 0065 0072 006e 0075 006e 0067 0073  .f.e.r.n.u.n.g.s
-00008da0: 0070 0061 0074 0063 0068 0800 0000 0006  .p.a.t.c.h......
-00008db0: 0000 0016 5265 6d6f 7665 6420 7265 6d6f  ....Removed remo
-00008dc0: 7669 6e67 2070 6174 6368 0700 0000 0d51  ving patch.....Q
-00008dd0: 7363 694c 6578 6572 4469 6666 0103 0000  sciLexerDiff....
-00008de0: 0034 0053 0063 0068 006c 0065 0063 0068  .4.S.c.h.l.e.c.h
-00008df0: 0074 0020 0067 0065 0066 006f 0072 006d  .t. .g.e.f.o.r.m
-00008e00: 0074 0065 0073 0020 0053 0065 0067 006d  .t.e.s. .S.e.g.m
-00008e10: 0065 006e 0074 0800 0000 0006 0000 0014  .e.n.t..........
-00008e20: 4261 646c 7920 666f 726d 6564 2073 6567  Badly formed seg
-00008e30: 6d65 6e74 0700 0000 1051 7363 694c 6578  ment.....QsciLex
-00008e40: 6572 4544 4946 4143 5401 0300 0000 3200  erEDIFACT.....2.
-00008e50: 5a00 7500 7300 6100 6d00 6d00 6500 6e00  Z.u.s.a.m.m.e.n.
-00008e60: 6700 6500 7300 6500 7400 7a00 7400 6500  g.e.s.e.t.z.t.e.
-00008e70: 7200 2000 5400 7200 6500 6e00 6e00 6500  r. .T.r.e.n.n.e.
-00008e80: 7208 0000 0000 0600 0000 1343 6f6d 706f  r..........Compo
-00008e90: 7369 7465 2073 6570 6172 6174 6f72 0700  site separator..
-00008ea0: 0000 1051 7363 694c 6578 6572 4544 4946  ...QsciLexerEDIF
-00008eb0: 4143 5401 0300 0000 1000 5300 7400 6100  ACT.......S.t.a.
-00008ec0: 6e00 6400 6100 7200 6408 0000 0000 0600  n.d.a.r.d.......
-00008ed0: 0000 0744 6566 6175 6c74 0700 0000 1051  ...Default.....Q
-00008ee0: 7363 694c 6578 6572 4544 4946 4143 5401  sciLexerEDIFACT.
-00008ef0: 0300 0000 1c00 4500 6c00 6500 6d00 6500  ......E.l.e.m.e.
-00008f00: 6e00 7400 7400 7200 6500 6e00 6e00 6500  n.t.t.r.e.n.n.e.
-00008f10: 7208 0000 0000 0600 0000 1145 6c65 6d65  r..........Eleme
-00008f20: 6e74 2073 6570 6172 6174 6f72 0700 0000  nt separator....
-00008f30: 1051 7363 694c 6578 6572 4544 4946 4143  .QsciLexerEDIFAC
-00008f40: 5401 0300 0000 1e00 4600 7200 6500 6900  T.......F.r.e.i.
-00008f50: 6700 6100 6200 6500 7400 7200 6500 6e00  g.a.b.e.t.r.e.n.
-00008f60: 6e00 6500 7208 0000 0000 0600 0000 1152  n.e.r..........R
-00008f70: 656c 6561 7365 2073 6570 6172 6174 6f72  elease separator
-00008f80: 0700 0000 1051 7363 694c 6578 6572 4544  .....QsciLexerED
-00008f90: 4946 4143 5401 0300 0000 1600 5300 6500  IFACT.......S.e.
-00008fa0: 6700 6d00 6500 6e00 7400 6500 6e00 6400  g.m.e.n.t.e.n.d.
-00008fb0: 6508 0000 0000 0600 0000 0b53 6567 6d65  e..........Segme
-00008fc0: 6e74 2065 6e64 0700 0000 1051 7363 694c  nt end.....QsciL
-00008fd0: 6578 6572 4544 4946 4143 5401 0300 0000  exerEDIFACT.....
-00008fe0: 1800 5300 6500 6700 6d00 6500 6e00 7400  ..S.e.g.m.e.n.t.
-00008ff0: 7300 7400 6100 7200 7408 0000 0000 0600  s.t.a.r.t.......
-00009000: 0000 0d53 6567 6d65 6e74 2073 7461 7274  ...Segment start
-00009010: 0700 0000 1051 7363 694c 6578 6572 4544  .....QsciLexerED
-00009020: 4946 4143 5401 0300 0000 1e00 5500 4e00  IFACT.......U.N.
-00009030: 4100 2000 5300 6500 6700 6d00 6500 6e00  A. .S.e.g.m.e.n.
-00009040: 7400 6b00 6f00 7000 6608 0000 0000 0600  t.k.o.p.f.......
-00009050: 0000 1255 4e41 2073 6567 6d65 6e74 2068  ...UNA segment h
-00009060: 6561 6465 7207 0000 0010 5173 6369 4c65  eader.....QsciLe
-00009070: 7865 7245 4449 4641 4354 0103 0000 001e  xerEDIFACT......
-00009080: 0055 004e 0048 0020 0053 0065 0067 006d  .U.N.H. .S.e.g.m
-00009090: 0065 006e 0074 006b 006f 0070 0066 0800  .e.n.t.k.o.p.f..
-000090a0: 0000 0006 0000 0012 554e 4820 7365 676d  ........UNH segm
-000090b0: 656e 7420 6865 6164 6572 0700 0000 1051  ent header.....Q
-000090c0: 7363 694c 6578 6572 4544 4946 4143 5401  sciLexerEDIFACT.
-000090d0: 0300 0000 1200 4b00 6f00 6d00 6d00 6500  ......K.o.m.m.e.
-000090e0: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
-000090f0: 0743 6f6d 6d65 6e74 0700 0000 1251 7363  .Comment.....Qsc
-00009100: 694c 6578 6572 466f 7274 7261 6e37 3701  iLexerFortran77.
-00009110: 0300 0000 1600 4600 6f00 7200 7400 7300  ......F.o.r.t.s.
-00009120: 6500 7400 7a00 7500 6e00 6708 0000 0000  e.t.z.u.n.g.....
-00009130: 0600 0000 0c43 6f6e 7469 6e75 6174 696f  .....Continuatio
-00009140: 6e07 0000 0012 5173 6369 4c65 7865 7246  n.....QsciLexerF
-00009150: 6f72 7472 616e 3737 0103 0000 0010 0053  ortran77.......S
-00009160: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
-00009170: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
-00009180: 0000 0012 5173 6369 4c65 7865 7246 6f72  ....QsciLexerFor
-00009190: 7472 616e 3737 0103 0000 001e 0044 006f  tran77.......D.o
-000091a0: 0074 0074 0065 0064 0020 004f 0070 0065  .t.t.e.d. .O.p.e
-000091b0: 0072 0061 0074 006f 0072 0800 0000 0006  .r.a.t.o.r......
-000091c0: 0000 000f 446f 7474 6564 206f 7065 7261  ....Dotted opera
-000091d0: 746f 7207 0000 0012 5173 6369 4c65 7865  tor.....QsciLexe
-000091e0: 7246 6f72 7472 616e 3737 0103 0000 0042  rFortran77.....B
-000091f0: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-00009200: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
-00009210: 0041 006e 0066 00fc 0068 0072 0075 006e  .A.n.f...h.r.u.n
-00009220: 0067 0073 007a 0065 0069 0063 0068 0065  .g.s.z.e.i.c.h.e
-00009230: 006e 0800 0000 0006 0000 0014 446f 7562  .n..........Doub
-00009240: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
-00009250: 0700 0000 1251 7363 694c 6578 6572 466f  .....QsciLexerFo
-00009260: 7274 7261 6e37 3701 0300 0000 2600 4500  rtran77.....&.E.
-00009270: 7200 7700 6500 6900 7400 6500 7200 7400  r.w.e.i.t.e.r.t.
-00009280: 6500 2000 4600 7500 6e00 6b00 7400 6900  e. .F.u.n.k.t.i.
-00009290: 6f00 6e08 0000 0000 0600 0000 1145 7874  o.n..........Ext
-000092a0: 656e 6465 6420 6675 6e63 7469 6f6e 0700  ended function..
-000092b0: 0000 1251 7363 694c 6578 6572 466f 7274  ...QsciLexerFort
-000092c0: 7261 6e37 3701 0300 0000 1400 4200 6500  ran77.......B.e.
-000092d0: 7a00 6500 6900 6300 6800 6e00 6500 7208  z.e.i.c.h.n.e.r.
-000092e0: 0000 0000 0600 0000 0a49 6465 6e74 6966  .........Identif
-000092f0: 6965 7207 0000 0012 5173 6369 4c65 7865  ier.....QsciLexe
-00009300: 7246 6f72 7472 616e 3737 0103 0000 0024  rFortran77.....$
-00009310: 0049 006e 0074 0072 0069 006e 0073 0069  .I.n.t.r.i.n.s.i
-00009320: 0063 002d 0046 0075 006e 006b 0074 0069  .c.-.F.u.n.k.t.i
-00009330: 006f 006e 0800 0000 0006 0000 0012 496e  .o.n..........In
-00009340: 7472 696e 7369 6320 6675 6e63 7469 6f6e  trinsic function
-00009350: 0700 0000 1251 7363 694c 6578 6572 466f  .....QsciLexerFo
-00009360: 7274 7261 6e37 3701 0300 0000 1a00 5300  rtran77.......S.
-00009370: 6300 6800 6c00 fc00 7300 7300 6500 6c00  c.h.l...s.s.e.l.
-00009380: 7700 6f00 7200 7408 0000 0000 0600 0000  w.o.r.t.........
-00009390: 074b 6579 776f 7264 0700 0000 1251 7363  .Keyword.....Qsc
-000093a0: 694c 6578 6572 466f 7274 7261 6e37 3701  iLexerFortran77.
-000093b0: 0300 0000 0a00 4d00 6100 7200 6b00 6508  ......M.a.r.k.e.
-000093c0: 0000 0000 0600 0000 054c 6162 656c 0700  .........Label..
-000093d0: 0000 1251 7363 694c 6578 6572 466f 7274  ...QsciLexerFort
-000093e0: 7261 6e37 3701 0300 0000 0800 5a00 6100  ran77.......Z.a.
-000093f0: 6800 6c08 0000 0000 0600 0000 064e 756d  h.l..........Num
-00009400: 6265 7207 0000 0012 5173 6369 4c65 7865  ber.....QsciLexe
-00009410: 7246 6f72 7472 616e 3737 0103 0000 0010  rFortran77......
-00009420: 004f 0070 0065 0072 0061 0074 006f 0072  .O.p.e.r.a.t.o.r
-00009430: 0800 0000 0006 0000 0008 4f70 6572 6174  ..........Operat
-00009440: 6f72 0700 0000 1251 7363 694c 6578 6572  or.....QsciLexer
-00009450: 466f 7274 7261 6e37 3701 0300 0000 2200  Fortran77.....".
-00009460: 5000 7200 e400 7000 7200 6f00 7a00 6500  P.r...p.r.o.z.e.
-00009470: 7300 7300 6f00 7200 6200 6c00 6f00 6300  s.s.o.r.b.l.o.c.
-00009480: 6b08 0000 0000 0600 0000 1350 7265 2d70  k..........Pre-p
-00009490: 726f 6365 7373 6f72 2062 6c6f 636b 0700  rocessor block..
-000094a0: 0000 1251 7363 694c 6578 6572 466f 7274  ...QsciLexerFort
-000094b0: 7261 6e37 3701 0300 0000 3600 5a00 6500  ran77.....6.Z.e.
-000094c0: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
-000094d0: 7400 6500 2000 6900 6e00 2000 4800 6f00  t.e. .i.n. .H.o.
-000094e0: 6300 6800 6b00 6f00 6d00 6d00 6100 7400  c.h.k.o.m.m.a.t.
-000094f0: 6108 0000 0000 0600 0000 1453 696e 676c  a..........Singl
-00009500: 652d 7175 6f74 6564 2073 7472 696e 6707  e-quoted string.
-00009510: 0000 0012 5173 6369 4c65 7865 7246 6f72  ....QsciLexerFor
-00009520: 7472 616e 3737 0103 0000 002e 0055 006e  tran77.......U.n
-00009530: 0062 0065 0065 006e 0064 0065 0074 0065  .b.e.e.n.d.e.t.e
-00009540: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-00009550: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
-00009560: 0000 000f 556e 636c 6f73 6564 2073 7472  ....Unclosed str
-00009570: 696e 6707 0000 0012 5173 6369 4c65 7865  ing.....QsciLexe
-00009580: 7246 6f72 7472 616e 3737 0103 0000 0030  rFortran77.....0
-00009590: 0041 0053 0050 0020 004a 0061 0076 0061  .A.S.P. .J.a.v.a
-000095a0: 0053 0063 0072 0069 0070 0074 0020 004b  .S.c.r.i.p.t. .K
-000095b0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-000095c0: 0800 0000 0006 0000 0016 4153 5020 4a61  ..........ASP Ja
-000095d0: 7661 5363 7269 7074 2063 6f6d 6d65 6e74  vaScript comment
-000095e0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-000095f0: 4d4c 0103 0000 002e 0041 0053 0050 0020  ML.......A.S.P. 
-00009600: 004a 0061 0076 0061 0053 0063 0072 0069  .J.a.v.a.S.c.r.i
-00009610: 0070 0074 0020 0053 0074 0061 006e 0064  .p.t. .S.t.a.n.d
-00009620: 0061 0072 0064 0800 0000 0006 0000 0016  .a.r.d..........
-00009630: 4153 5020 4a61 7661 5363 7269 7074 2064  ASP JavaScript d
-00009640: 6566 6175 6c74 0700 0000 0d51 7363 694c  efault.....QsciL
-00009650: 6578 6572 4854 4d4c 0103 0000 0060 0041  exerHTML.....`.A
-00009660: 0053 0050 0020 004a 0061 0076 0061 0053  .S.P. .J.a.v.a.S
-00009670: 0063 0072 0069 0070 0074 0020 005a 0065  .c.r.i.p.t. .Z.e
-00009680: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-00009690: 0074 0065 0020 0069 006e 0020 0041 006e  .t.e. .i.n. .A.n
-000096a0: 0066 00fc 0068 0072 0075 006e 0067 0073  .f...h.r.u.n.g.s
-000096b0: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
-000096c0: 0000 0006 0000 0023 4153 5020 4a61 7661  .......#ASP Java
-000096d0: 5363 7269 7074 2064 6f75 626c 652d 7175  Script double-qu
-000096e0: 6f74 6564 2073 7472 696e 6707 0000 000d  oted string.....
-000096f0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-00009700: 0000 3800 4100 5300 5000 2000 4a00 6100  ..8.A.S.P. .J.a.
-00009710: 7600 6100 5300 6300 7200 6900 7000 7400  v.a.S.c.r.i.p.t.
-00009720: 2000 5300 6300 6800 6c00 fc00 7300 7300   .S.c.h.l...s.s.
-00009730: 6500 6c00 7700 6f00 7200 7408 0000 0000  e.l.w.o.r.t.....
-00009740: 0600 0000 1641 5350 204a 6176 6153 6372  .....ASP JavaScr
-00009750: 6970 7420 6b65 7977 6f72 6407 0000 000d  ipt keyword.....
-00009760: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-00009770: 0000 3c00 4100 5300 5000 2000 4a00 6100  ..<.A.S.P. .J.a.
-00009780: 7600 6100 5300 6300 7200 6900 7000 7400  v.a.S.c.r.i.p.t.
-00009790: 2000 5a00 6500 6900 6c00 6500 6e00 6b00   .Z.e.i.l.e.n.k.
-000097a0: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-000097b0: 0000 0000 0600 0000 1b41 5350 204a 6176  .........ASP Jav
-000097c0: 6153 6372 6970 7420 6c69 6e65 2063 6f6d  aScript line com
-000097d0: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
-000097e0: 6572 4854 4d4c 0103 0000 0026 0041 0053  erHTML.....&.A.S
-000097f0: 0050 0020 004a 0061 0076 0061 0053 0063  .P. .J.a.v.a.S.c
-00009800: 0072 0069 0070 0074 0020 005a 0061 0068  .r.i.p.t. .Z.a.h
-00009810: 006c 0800 0000 0006 0000 0015 4153 5020  .l..........ASP 
-00009820: 4a61 7661 5363 7269 7074 206e 756d 6265  JavaScript numbe
-00009830: 7207 0000 000d 5173 6369 4c65 7865 7248  r.....QsciLexerH
-00009840: 544d 4c01 0300 0000 4200 4100 5300 5000  TML.....B.A.S.P.
-00009850: 2000 4a00 6100 7600 6100 5300 6300 7200   .J.a.v.a.S.c.r.
-00009860: 6900 7000 7400 2000 5200 6500 6700 7500  i.p.t. .R.e.g.u.
-00009870: 6c00 e400 7200 6500 7200 2000 4100 7500  l...r.e.r. .A.u.
-00009880: 7300 6400 7200 7500 6300 6b08 0000 0000  s.d.r.u.c.k.....
-00009890: 0600 0000 2141 5350 204a 6176 6153 6372  ....!ASP JavaScr
-000098a0: 6970 7420 7265 6775 6c61 7220 6578 7072  ipt regular expr
-000098b0: 6573 7369 6f6e 0700 0000 0d51 7363 694c  ession.....QsciL
-000098c0: 6578 6572 4854 4d4c 0103 0000 0054 0041  exerHTML.....T.A
-000098d0: 0053 0050 0020 004a 0061 0076 0061 0053  .S.P. .J.a.v.a.S
-000098e0: 0063 0072 0069 0070 0074 0020 005a 0065  .c.r.i.p.t. .Z.e
-000098f0: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-00009900: 0074 0065 0020 0069 006e 0020 0048 006f  .t.e. .i.n. .H.o
-00009910: 0063 0068 006b 006f 006d 006d 0061 0074  .c.h.k.o.m.m.a.t
-00009920: 0061 0800 0000 0006 0000 0023 4153 5020  .a.........#ASP 
-00009930: 4a61 7661 5363 7269 7074 2073 696e 676c  JavaScript singl
-00009940: 652d 7175 6f74 6564 2073 7472 696e 6707  e-quoted string.
-00009950: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
-00009960: 4c01 0300 0000 2a00 4100 5300 5000 2000  L.....*.A.S.P. .
-00009970: 4a00 6100 7600 6100 5300 6300 7200 6900  J.a.v.a.S.c.r.i.
-00009980: 7000 7400 2000 5300 7900 6d00 6200 6f00  p.t. .S.y.m.b.o.
-00009990: 6c08 0000 0000 0600 0000 1541 5350 204a  l..........ASP J
-000099a0: 6176 6153 6372 6970 7420 7379 6d62 6f6c  avaScript symbol
-000099b0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-000099c0: 4d4c 0103 0000 004c 0041 0053 0050 0020  ML.....L.A.S.P. 
-000099d0: 004a 0061 0076 0061 0053 0063 0072 0069  .J.a.v.a.S.c.r.i
-000099e0: 0070 0074 0020 0055 006e 0062 0065 0065  .p.t. .U.n.b.e.e
-000099f0: 006e 0064 0065 0074 0065 0020 005a 0065  .n.d.e.t.e. .Z.e
-00009a00: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-00009a10: 0074 0065 0800 0000 0006 0000 001e 4153  .t.e..........AS
-00009a20: 5020 4a61 7661 5363 7269 7074 2075 6e63  P JavaScript unc
-00009a30: 6c6f 7365 6420 7374 7269 6e67 0700 0000  losed string....
-00009a40: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-00009a50: 0000 0026 0041 0053 0050 0020 004a 0061  ...&.A.S.P. .J.a
-00009a60: 0076 0061 0053 0063 0072 0069 0070 0074  .v.a.S.c.r.i.p.t
-00009a70: 0020 0057 006f 0072 0074 0800 0000 0006  . .W.o.r.t......
-00009a80: 0000 0013 4153 5020 4a61 7661 5363 7269  ....ASP JavaScri
-00009a90: 7074 2077 6f72 6407 0000 000d 5173 6369  pt word.....Qsci
-00009aa0: 4c65 7865 7248 544d 4c01 0300 0000 2c00  LexerHTML.....,.
-00009ab0: 4100 5300 5000 2000 5000 7900 7400 6800  A.S.P. .P.y.t.h.
-00009ac0: 6f00 6e00 2000 4b00 6c00 6100 7300 7300  o.n. .K.l.a.s.s.
-00009ad0: 6500 6e00 6e00 6100 6d00 6508 0000 0000  e.n.n.a.m.e.....
-00009ae0: 0600 0000 1541 5350 2050 7974 686f 6e20  .....ASP Python 
-00009af0: 636c 6173 7320 6e61 6d65 0700 0000 0d51  class name.....Q
-00009b00: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-00009b10: 0028 0041 0053 0050 0020 0050 0079 0074  .(.A.S.P. .P.y.t
-00009b20: 0068 006f 006e 0020 004b 006f 006d 006d  .h.o.n. .K.o.m.m
-00009b30: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
-00009b40: 0000 0012 4153 5020 5079 7468 6f6e 2063  ....ASP Python c
-00009b50: 6f6d 6d65 6e74 0700 0000 0d51 7363 694c  omment.....QsciL
-00009b60: 6578 6572 4854 4d4c 0103 0000 0026 0041  exerHTML.....&.A
-00009b70: 0053 0050 0020 0050 0079 0074 0068 006f  .S.P. .P.y.t.h.o
-00009b80: 006e 0020 0053 0074 0061 006e 0064 0061  .n. .S.t.a.n.d.a
-00009b90: 0072 0064 0800 0000 0006 0000 0012 4153  .r.d..........AS
-00009ba0: 5020 5079 7468 6f6e 2064 6566 6175 6c74  P Python default
-00009bb0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-00009bc0: 4d4c 0103 0000 0058 0041 0053 0050 0020  ML.....X.A.S.P. 
-00009bd0: 0050 0079 0074 0068 006f 006e 0020 005a  .P.y.t.h.o.n. .Z
-00009be0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-00009bf0: 0074 0074 0065 0020 0069 006e 0020 0041  .t.t.e. .i.n. .A
-00009c00: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
-00009c10: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
-00009c20: 0800 0000 0006 0000 001f 4153 5020 5079  ..........ASP Py
-00009c30: 7468 6f6e 2064 6f75 626c 652d 7175 6f74  thon double-quot
-00009c40: 6564 2073 7472 696e 6707 0000 000d 5173  ed string.....Qs
-00009c50: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
-00009c60: 4e00 4100 5300 5000 2000 5000 7900 7400  N.A.S.P. .P.y.t.
-00009c70: 6800 6f00 6e00 2000 4600 7500 6e00 6b00  h.o.n. .F.u.n.k.
-00009c80: 7400 6900 6f00 6e00 7300 2d00 2000 6f00  t.i.o.n.s.-. .o.
-00009c90: 6400 6500 7200 2000 4d00 6500 7400 6800  d.e.r. .M.e.t.h.
-00009ca0: 6f00 6400 6500 6e00 6e00 6100 6d00 6508  o.d.e.n.n.a.m.e.
-00009cb0: 0000 0000 0600 0000 2241 5350 2050 7974  ........"ASP Pyt
-00009cc0: 686f 6e20 6675 6e63 7469 6f6e 206f 7220  hon function or 
-00009cd0: 6d65 7468 6f64 206e 616d 6507 0000 000d  method name.....
-00009ce0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-00009cf0: 0000 2a00 4100 5300 5000 2000 5000 7900  ..*.A.S.P. .P.y.
-00009d00: 7400 6800 6f00 6e00 2000 4200 6500 7a00  t.h.o.n. .B.e.z.
-00009d10: 6500 6900 6300 6800 6e00 6500 7208 0000  e.i.c.h.n.e.r...
-00009d20: 0000 0600 0000 1541 5350 2050 7974 686f  .......ASP Pytho
-00009d30: 6e20 6964 656e 7469 6669 6572 0700 0000  n identifier....
-00009d40: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-00009d50: 0000 0030 0041 0053 0050 0020 0050 0079  ...0.A.S.P. .P.y
-00009d60: 0074 0068 006f 006e 0020 0053 0063 0068  .t.h.o.n. .S.c.h
-00009d70: 006c 00fc 0073 0073 0065 006c 0077 006f  .l...s.s.e.l.w.o
-00009d80: 0072 0074 0800 0000 0006 0000 0012 4153  .r.t..........AS
-00009d90: 5020 5079 7468 6f6e 206b 6579 776f 7264  P Python keyword
-00009da0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-00009db0: 4d4c 0103 0000 001e 0041 0053 0050 0020  ML.......A.S.P. 
-00009dc0: 0050 0079 0074 0068 006f 006e 0020 005a  .P.y.t.h.o.n. .Z
-00009dd0: 0061 0068 006c 0800 0000 0006 0000 0011  .a.h.l..........
-00009de0: 4153 5020 5079 7468 6f6e 206e 756d 6265  ASP Python numbe
-00009df0: 7207 0000 000d 5173 6369 4c65 7865 7248  r.....QsciLexerH
-00009e00: 544d 4c01 0300 0000 2600 4100 5300 5000  TML.....&.A.S.P.
-00009e10: 2000 5000 7900 7400 6800 6f00 6e00 2000   .P.y.t.h.o.n. .
-00009e20: 4f00 7000 6500 7200 6100 7400 6f00 7208  O.p.e.r.a.t.o.r.
-00009e30: 0000 0000 0600 0000 1341 5350 2050 7974  .........ASP Pyt
-00009e40: 686f 6e20 6f70 6572 6174 6f72 0700 0000  hon operator....
-00009e50: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-00009e60: 0000 004c 0041 0053 0050 0020 0050 0079  ...L.A.S.P. .P.y
-00009e70: 0074 0068 006f 006e 0020 005a 0065 0069  .t.h.o.n. .Z.e.i
-00009e80: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00009e90: 0065 0020 0069 006e 0020 0048 006f 0063  .e. .i.n. .H.o.c
-00009ea0: 0068 006b 006f 006d 006d 0061 0074 0061  .h.k.o.m.m.a.t.a
-00009eb0: 0800 0000 0006 0000 001f 4153 5020 5079  ..........ASP Py
-00009ec0: 7468 6f6e 2073 696e 676c 652d 7175 6f74  thon single-quot
-00009ed0: 6564 2073 7472 696e 6707 0000 000d 5173  ed string.....Qs
-00009ee0: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
-00009ef0: 6e00 4100 5300 5000 2000 5000 7900 7400  n.A.S.P. .P.y.t.
-00009f00: 6800 6f00 6e00 2000 5a00 6500 6900 6300  h.o.n. .Z.e.i.c.
-00009f10: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
-00009f20: 2000 6900 6e00 2000 6400 7200 6500 6900   .i.n. .d.r.e.i.
-00009f30: 6600 6100 6300 6800 6500 6e00 2000 4100  f.a.c.h.e.n. .A.
-00009f40: 6e00 6600 fc00 6800 7200 7500 6e00 6700  n.f...h.r.u.n.g.
-00009f50: 7300 7a00 6500 6900 6300 6800 6500 6e08  s.z.e.i.c.h.e.n.
-00009f60: 0000 0000 0600 0000 2641 5350 2050 7974  ........&ASP Pyt
-00009f70: 686f 6e20 7472 6970 6c65 2064 6f75 626c  hon triple doubl
-00009f80: 652d 7175 6f74 6564 2073 7472 696e 6707  e-quoted string.
-00009f90: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
-00009fa0: 4c01 0300 0000 6200 4100 5300 5000 2000  L.....b.A.S.P. .
-00009fb0: 5000 7900 7400 6800 6f00 6e00 2000 5a00  P.y.t.h.o.n. .Z.
-00009fc0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-00009fd0: 7400 7400 6500 2000 6900 6e00 2000 6400  t.t.e. .i.n. .d.
-00009fe0: 7200 6500 6900 6600 6100 6300 6800 6500  r.e.i.f.a.c.h.e.
-00009ff0: 6e00 2000 4800 6f00 6300 6800 6b00 6f00  n. .H.o.c.h.k.o.
-0000a000: 6d00 6d00 6100 7400 6108 0000 0000 0600  m.m.a.t.a.......
-0000a010: 0000 2641 5350 2050 7974 686f 6e20 7472  ..&ASP Python tr
-0000a020: 6970 6c65 2073 696e 676c 652d 7175 6f74  iple single-quot
-0000a030: 6564 2073 7472 696e 6707 0000 000d 5173  ed string.....Qs
-0000a040: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
-0000a050: 2c00 4100 5300 5000 2000 5600 4200 5300  ,.A.S.P. .V.B.S.
-0000a060: 6300 7200 6900 7000 7400 2000 4b00 6f00  c.r.i.p.t. .K.o.
-0000a070: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
-0000a080: 0000 0600 0000 1441 5350 2056 4253 6372  .......ASP VBScr
-0000a090: 6970 7420 636f 6d6d 656e 7407 0000 000d  ipt comment.....
-0000a0a0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-0000a0b0: 0000 2a00 4100 5300 5000 2000 5600 4200  ..*.A.S.P. .V.B.
-0000a0c0: 5300 6300 7200 6900 7000 7400 2000 5300  S.c.r.i.p.t. .S.
-0000a0d0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
-0000a0e0: 0000 0600 0000 1441 5350 2056 4253 6372  .......ASP VBScr
-0000a0f0: 6970 7420 6465 6661 756c 7407 0000 000d  ipt default.....
-0000a100: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-0000a110: 0000 2e00 4100 5300 5000 2000 5600 4200  ....A.S.P. .V.B.
-0000a120: 5300 6300 7200 6900 7000 7400 2000 4200  S.c.r.i.p.t. .B.
-0000a130: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
-0000a140: 7208 0000 0000 0600 0000 1741 5350 2056  r..........ASP V
-0000a150: 4253 6372 6970 7420 6964 656e 7469 6669  BScript identifi
-0000a160: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
-0000a170: 4854 4d4c 0103 0000 0034 0041 0053 0050  HTML.....4.A.S.P
-0000a180: 0020 0056 0042 0053 0063 0072 0069 0070  . .V.B.S.c.r.i.p
-0000a190: 0074 0020 0053 0063 0068 006c 00fc 0073  .t. .S.c.h.l...s
-0000a1a0: 0073 0065 006c 0077 006f 0072 0074 0800  .s.e.l.w.o.r.t..
-0000a1b0: 0000 0006 0000 0014 4153 5020 5642 5363  ........ASP VBSc
-0000a1c0: 7269 7074 206b 6579 776f 7264 0700 0000  ript keyword....
-0000a1d0: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-0000a1e0: 0000 0022 0041 0053 0050 0020 0056 0042  ...".A.S.P. .V.B
-0000a1f0: 0053 0063 0072 0069 0070 0074 0020 005a  .S.c.r.i.p.t. .Z
-0000a200: 0061 0068 006c 0800 0000 0006 0000 0013  .a.h.l..........
-0000a210: 4153 5020 5642 5363 7269 7074 206e 756d  ASP VBScript num
-0000a220: 6265 7207 0000 000d 5173 6369 4c65 7865  ber.....QsciLexe
-0000a230: 7248 544d 4c01 0300 0000 3200 4100 5300  rHTML.....2.A.S.
-0000a240: 5000 2000 5600 4200 5300 6300 7200 6900  P. .V.B.S.c.r.i.
-0000a250: 7000 7400 2000 5a00 6500 6900 6300 6800  p.t. .Z.e.i.c.h.
-0000a260: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
-0000a270: 0000 0600 0000 1341 5350 2056 4253 6372  .......ASP VBScr
-0000a280: 6970 7420 7374 7269 6e67 0700 0000 0d51  ipt string.....Q
-0000a290: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000a2a0: 0048 0041 0053 0050 0020 0056 0042 0053  .H.A.S.P. .V.B.S
-0000a2b0: 0063 0072 0069 0070 0074 0020 0055 006e  .c.r.i.p.t. .U.n
-0000a2c0: 0062 0065 0065 006e 0064 0065 0074 0065  .b.e.e.n.d.e.t.e
-0000a2d0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-0000a2e0: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
-0000a2f0: 0000 001c 4153 5020 5642 5363 7269 7074  ....ASP VBScript
-0000a300: 2075 6e63 6c6f 7365 6420 7374 7269 6e67   unclosed string
-0000a310: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000a320: 4d4c 0103 0000 0028 0041 0053 0050 0020  ML.....(.A.S.P. 
-0000a330: 0058 002d 0043 006f 0064 0065 0020 004b  .X.-.C.o.d.e. .K
-0000a340: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-0000a350: 0800 0000 0006 0000 0012 4153 5020 582d  ..........ASP X-
-0000a360: 436f 6465 2063 6f6d 6d65 6e74 0700 0000  Code comment....
-0000a370: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-0000a380: 0000 0010 0041 0074 0074 0072 0069 0062  .....A.t.t.r.i.b
-0000a390: 0075 0074 0800 0000 0006 0000 0009 4174  .u.t..........At
-0000a3a0: 7472 6962 7574 6507 0000 000d 5173 6369  tribute.....Qsci
-0000a3b0: 4c65 7865 7248 544d 4c01 0300 0000 0a00  LexerHTML.......
-0000a3c0: 4300 4400 4100 5400 4108 0000 0000 0600  C.D.A.T.A.......
-0000a3d0: 0000 0543 4441 5441 0700 0000 0d51 7363  ...CDATA.....Qsc
-0000a3e0: 694c 6578 6572 4854 4d4c 0103 0000 000e  iLexerHTML......
-0000a3f0: 0054 0061 0067 0065 006e 0064 0065 0800  .T.a.g.e.n.d.e..
-0000a400: 0000 0006 0000 000c 456e 6420 6f66 2061  ........End of a
-0000a410: 2074 6167 0700 0000 0d51 7363 694c 6578   tag.....QsciLex
-0000a420: 6572 4854 4d4c 0103 0000 0032 0045 006e  erHTML.....2.E.n
-0000a430: 0064 0065 0020 0065 0069 006e 0065 0073  .d.e. .e.i.n.e.s
-0000a440: 0020 0058 004d 004c 0020 0046 0072 0061  . .X.M.L. .F.r.a
-0000a450: 0067 006d 0065 006e 0074 0065 0073 0800  .g.m.e.n.t.e.s..
-0000a460: 0000 0006 0000 0016 456e 6420 6f66 2061  ........End of a
-0000a470: 6e20 584d 4c20 6672 6167 6d65 6e74 0700  n XML fragment..
-0000a480: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
-0000a490: 0103 0000 000e 0045 006e 0074 0069 0074  .......E.n.t.i.t
-0000a4a0: 00e4 0074 0800 0000 0006 0000 0006 456e  ...t..........En
-0000a4b0: 7469 7479 0700 0000 0d51 7363 694c 6578  tity.....QsciLex
-0000a4c0: 6572 4854 4d4c 0103 0000 0064 004b 006f  erHTML.....d.K.o
-0000a4d0: 006d 006d 0065 006e 0074 0061 0072 0020  .m.m.e.n.t.a.r. 
-0000a4e0: 0064 0065 0073 0020 0065 0072 0073 0074  .d.e.s. .e.r.s.t
-0000a4f0: 0065 006e 0020 0050 0061 0072 0061 006d  .e.n. .P.a.r.a.m
-0000a500: 0065 0074 0065 0072 0073 0020 0065 0069  .e.t.e.r.s. .e.i
-0000a510: 006e 0065 0073 0020 0053 0047 004d 004c  .n.e.s. .S.G.M.L
-0000a520: 0020 0042 0065 0066 0065 0068 006c 0073  . .B.e.f.e.h.l.s
-0000a530: 0800 0000 0006 0000 002a 4669 7273 7420  .........*First 
-0000a540: 7061 7261 6d65 7465 7220 636f 6d6d 656e  parameter commen
-0000a550: 7420 6f66 2061 6e20 5347 4d4c 2063 6f6d  t of an SGML com
-0000a560: 6d61 6e64 0700 0000 0d51 7363 694c 6578  mand.....QsciLex
-0000a570: 6572 4854 4d4c 0103 0000 0046 0045 0072  erHTML.....F.E.r
-0000a580: 0073 0074 0065 0072 0020 0050 0061 0072  .s.t.e.r. .P.a.r
-0000a590: 0061 006d 0065 0074 0065 0072 0020 0065  .a.m.e.t.e.r. .e
-0000a5a0: 0069 006e 0065 0073 0020 0053 0047 004d  .i.n.e.s. .S.G.M
-0000a5b0: 004c 0020 0042 0065 0066 0065 0068 006c  .L. .B.e.f.e.h.l
-0000a5c0: 0073 0800 0000 0006 0000 0022 4669 7273  .s........."Firs
-0000a5d0: 7420 7061 7261 6d65 7465 7220 6f66 2061  t parameter of a
-0000a5e0: 6e20 5347 4d4c 2063 6f6d 6d61 6e64 0700  n SGML command..
-0000a5f0: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
-0000a600: 0103 0000 001c 0048 0054 004d 004c 0020  .......H.T.M.L. 
-0000a610: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
-0000a620: 0072 0800 0000 0006 0000 000c 4854 4d4c  .r..........HTML
-0000a630: 2063 6f6d 6d65 6e74 0700 0000 0d51 7363   comment.....Qsc
-0000a640: 694c 6578 6572 4854 4d4c 0103 0000 001a  iLexerHTML......
-0000a650: 0048 0054 004d 004c 0020 0053 0074 0061  .H.T.M.L. .S.t.a
-0000a660: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
-0000a670: 0000 000c 4854 4d4c 2064 6566 6175 6c74  ....HTML default
-0000a680: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000a690: 4d4c 0103 0000 004c 0048 0054 004d 004c  ML.....L.H.T.M.L
-0000a6a0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-0000a6b0: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
-0000a6c0: 0020 0041 006e 0066 00fc 0068 0072 0075  . .A.n.f...h.r.u
-0000a6d0: 006e 0067 0073 007a 0065 0069 0063 0068  .n.g.s.z.e.i.c.h
-0000a6e0: 0065 006e 0800 0000 0006 0000 0019 4854  .e.n..........HT
-0000a6f0: 4d4c 2064 6f75 626c 652d 7175 6f74 6564  ML double-quoted
-0000a700: 2073 7472 696e 6707 0000 000d 5173 6369   string.....Qsci
-0000a710: 4c65 7865 7248 544d 4c01 0300 0000 1200  LexerHTML.......
-0000a720: 4800 5400 4d00 4c00 2000 5a00 6100 6800  H.T.M.L. .Z.a.h.
-0000a730: 6c08 0000 0000 0600 0000 0b48 544d 4c20  l..........HTML 
-0000a740: 6e75 6d62 6572 0700 0000 0d51 7363 694c  number.....QsciL
-0000a750: 6578 6572 4854 4d4c 0103 0000 0040 0048  exerHTML.....@.H
-0000a760: 0054 004d 004c 0020 005a 0065 0069 0063  .T.M.L. .Z.e.i.c
-0000a770: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
-0000a780: 0020 0069 006e 0020 0048 006f 0063 0068  . .i.n. .H.o.c.h
-0000a790: 006b 006f 006d 006d 0061 0074 0061 0800  .k.o.m.m.a.t.a..
-0000a7a0: 0000 0006 0000 0019 4854 4d4c 2073 696e  ........HTML sin
-0000a7b0: 676c 652d 7175 6f74 6564 2073 7472 696e  gle-quoted strin
-0000a7c0: 6707 0000 000d 5173 6369 4c65 7865 7248  g.....QsciLexerH
-0000a7d0: 544d 4c01 0300 0000 4000 4a00 6100 7600  TML.....@.J.a.v.
-0000a7e0: 6100 4400 6f00 6300 2000 4100 5300 5000  a.D.o.c. .A.S.P.
-0000a7f0: 2000 4a00 6100 7600 6100 5300 6300 7200   .J.a.v.a.S.c.r.
-0000a800: 6900 7000 7400 2000 4b00 6f00 6d00 6d00  i.p.t. .K.o.m.m.
-0000a810: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
-0000a820: 0000 244a 6176 6144 6f63 2073 7479 6c65  ..$JavaDoc style
-0000a830: 2041 5350 204a 6176 6153 6372 6970 7420   ASP JavaScript 
-0000a840: 636f 6d6d 656e 7407 0000 000d 5173 6369  comment.....Qsci
-0000a850: 4c65 7865 7248 544d 4c01 0300 0000 3800  LexerHTML.....8.
-0000a860: 4a00 6100 7600 6100 4400 6f00 6300 2000  J.a.v.a.D.o.c. .
-0000a870: 4a00 6100 7600 6100 5300 6300 7200 6900  J.a.v.a.S.c.r.i.
-0000a880: 7000 7400 2000 4b00 6f00 6d00 6d00 6500  p.t. .K.o.m.m.e.
-0000a890: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
-0000a8a0: 204a 6176 6144 6f63 2073 7479 6c65 204a   JavaDoc style J
-0000a8b0: 6176 6153 6372 6970 7420 636f 6d6d 656e  avaScript commen
-0000a8c0: 7407 0000 000d 5173 6369 4c65 7865 7248  t.....QsciLexerH
-0000a8d0: 544d 4c01 0300 0000 2800 4a00 6100 7600  TML.....(.J.a.v.
-0000a8e0: 6100 5300 6300 7200 6900 7000 7400 2000  a.S.c.r.i.p.t. .
-0000a8f0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
-0000a900: 7208 0000 0000 0600 0000 124a 6176 6153  r..........JavaS
-0000a910: 6372 6970 7420 636f 6d6d 656e 7407 0000  cript comment...
-0000a920: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000a930: 0300 0000 2600 4a00 6100 7600 6100 5300  ....&.J.a.v.a.S.
-0000a940: 6300 7200 6900 7000 7400 2000 5300 7400  c.r.i.p.t. .S.t.
-0000a950: 6100 6e00 6400 6100 7200 6408 0000 0000  a.n.d.a.r.d.....
-0000a960: 0600 0000 124a 6176 6153 6372 6970 7420  .....JavaScript 
-0000a970: 6465 6661 756c 7407 0000 000d 5173 6369  default.....Qsci
-0000a980: 4c65 7865 7248 544d 4c01 0300 0000 5800  LexerHTML.....X.
-0000a990: 4a00 6100 7600 6100 5300 6300 7200 6900  J.a.v.a.S.c.r.i.
-0000a9a0: 7000 7400 2000 5a00 6500 6900 6300 6800  p.t. .Z.e.i.c.h.
-0000a9b0: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
-0000a9c0: 6900 6e00 2000 4100 6e00 6600 fc00 6800  i.n. .A.n.f...h.
-0000a9d0: 7200 7500 6e00 6700 7300 7a00 6500 6900  r.u.n.g.s.z.e.i.
-0000a9e0: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
-0000a9f0: 1f4a 6176 6153 6372 6970 7420 646f 7562  .JavaScript doub
-0000aa00: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
-0000aa10: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000aa20: 4d4c 0103 0000 0030 004a 0061 0076 0061  ML.....0.J.a.v.a
-0000aa30: 0053 0063 0072 0069 0070 0074 0020 0053  .S.c.r.i.p.t. .S
-0000aa40: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
-0000aa50: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
-0000aa60: 0012 4a61 7661 5363 7269 7074 206b 6579  ..JavaScript key
-0000aa70: 776f 7264 0700 0000 0d51 7363 694c 6578  word.....QsciLex
-0000aa80: 6572 4854 4d4c 0103 0000 0034 004a 0061  erHTML.....4.J.a
-0000aa90: 0076 0061 0053 0063 0072 0069 0070 0074  .v.a.S.c.r.i.p.t
-0000aaa0: 0020 005a 0065 0069 006c 0065 006e 006b  . .Z.e.i.l.e.n.k
-0000aab0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-0000aac0: 0800 0000 0006 0000 0017 4a61 7661 5363  ..........JavaSc
-0000aad0: 7269 7074 206c 696e 6520 636f 6d6d 656e  ript line commen
-0000aae0: 7407 0000 000d 5173 6369 4c65 7865 7248  t.....QsciLexerH
-0000aaf0: 544d 4c01 0300 0000 1e00 4a00 6100 7600  TML.......J.a.v.
-0000ab00: 6100 5300 6300 7200 6900 7000 7400 2000  a.S.c.r.i.p.t. .
-0000ab10: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
-0000ab20: 114a 6176 6153 6372 6970 7420 6e75 6d62  .JavaScript numb
-0000ab30: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
-0000ab40: 4854 4d4c 0103 0000 003a 004a 0061 0076  HTML.....:.J.a.v
-0000ab50: 0061 0053 0063 0072 0069 0070 0074 0020  .a.S.c.r.i.p.t. 
-0000ab60: 0052 0065 0067 0075 006c 00e4 0072 0065  .R.e.g.u.l...r.e
-0000ab70: 0072 0020 0041 0075 0073 0064 0072 0075  .r. .A.u.s.d.r.u
-0000ab80: 0063 006b 0800 0000 0006 0000 001d 4a61  .c.k..........Ja
-0000ab90: 7661 5363 7269 7074 2072 6567 756c 6172  vaScript regular
-0000aba0: 2065 7870 7265 7373 696f 6e07 0000 000d   expression.....
-0000abb0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-0000abc0: 0000 4c00 4a00 6100 7600 6100 5300 6300  ..L.J.a.v.a.S.c.
-0000abd0: 7200 6900 7000 7400 2000 5a00 6500 6900  r.i.p.t. .Z.e.i.
-0000abe0: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-0000abf0: 6500 2000 6900 6e00 2000 4800 6f00 6300  e. .i.n. .H.o.c.
-0000ac00: 6800 6b00 6f00 6d00 6d00 6100 7400 6108  h.k.o.m.m.a.t.a.
-0000ac10: 0000 0000 0600 0000 1f4a 6176 6153 6372  .........JavaScr
-0000ac20: 6970 7420 7369 6e67 6c65 2d71 756f 7465  ipt single-quote
-0000ac30: 6420 7374 7269 6e67 0700 0000 0d51 7363  d string.....Qsc
-0000ac40: 694c 6578 6572 4854 4d4c 0103 0000 0022  iLexerHTML....."
-0000ac50: 004a 0061 0076 0061 0053 0063 0072 0069  .J.a.v.a.S.c.r.i
-0000ac60: 0070 0074 0020 0053 0079 006d 0062 006f  .p.t. .S.y.m.b.o
-0000ac70: 006c 0800 0000 0006 0000 0011 4a61 7661  .l..........Java
-0000ac80: 5363 7269 7074 2073 796d 626f 6c07 0000  Script symbol...
-0000ac90: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000aca0: 0300 0000 4400 4a00 6100 7600 6100 5300  ....D.J.a.v.a.S.
-0000acb0: 6300 7200 6900 7000 7400 2000 5500 6e00  c.r.i.p.t. .U.n.
-0000acc0: 6200 6500 6500 6e00 6400 6500 7400 6500  b.e.e.n.d.e.t.e.
-0000acd0: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
-0000ace0: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
-0000acf0: 0000 1a4a 6176 6153 6372 6970 7420 756e  ...JavaScript un
-0000ad00: 636c 6f73 6564 2073 7472 696e 6707 0000  closed string...
-0000ad10: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000ad20: 0300 0000 1e00 4a00 6100 7600 6100 5300  ......J.a.v.a.S.
-0000ad30: 6300 7200 6900 7000 7400 2000 5700 6f00  c.r.i.p.t. .W.o.
-0000ad40: 7200 7408 0000 0000 0600 0000 0f4a 6176  r.t..........Jav
-0000ad50: 6153 6372 6970 7420 776f 7264 0700 0000  aScript word....
-0000ad60: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-0000ad70: 0000 0032 0041 006e 0064 0065 0072 0065  ...2.A.n.d.e.r.e
-0000ad80: 0072 0020 0054 0065 0078 0074 0020 0069  .r. .T.e.x.t. .i
-0000ad90: 006e 0020 0065 0069 006e 0065 006d 0020  .n. .e.i.n.e.m. 
-0000ada0: 0054 0061 0067 0800 0000 0006 0000 0013  .T.a.g..........
-0000adb0: 4f74 6865 7220 7465 7874 2069 6e20 6120  Other text in a 
-0000adc0: 7461 6707 0000 000d 5173 6369 4c65 7865  tag.....QsciLexe
-0000add0: 7248 544d 4c01 0300 0000 1a00 5000 4800  rHTML.......P.H.
-0000ade0: 5000 2000 4b00 6f00 6d00 6d00 6500 6e00  P. .K.o.m.m.e.n.
-0000adf0: 7400 6100 7208 0000 0000 0600 0000 0b50  t.a.r..........P
-0000ae00: 4850 2063 6f6d 6d65 6e74 0700 0000 0d51  HP comment.....Q
-0000ae10: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000ae20: 0018 0050 0048 0050 0020 0053 0074 0061  ...P.H.P. .S.t.a
-0000ae30: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
-0000ae40: 0000 000b 5048 5020 6465 6661 756c 7407  ....PHP default.
-0000ae50: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
-0000ae60: 4c01 0300 0000 4a00 5000 4800 5000 2000  L.....J.P.H.P. .
-0000ae70: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
-0000ae80: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
-0000ae90: 4100 6e00 6600 fc00 6800 7200 7500 6e00  A.n.f...h.r.u.n.
-0000aea0: 6700 7300 7a00 6500 6900 6300 6800 6500  g.s.z.e.i.c.h.e.
-0000aeb0: 6e08 0000 0000 0600 0000 1850 4850 2064  n..........PHP d
-0000aec0: 6f75 626c 652d 7175 6f74 6564 2073 7472  ouble-quoted str
-0000aed0: 696e 6707 0000 000d 5173 6369 4c65 7865  ing.....QsciLexe
-0000aee0: 7248 544d 4c01 0300 0000 4200 5000 4800  rHTML.....B.P.H.
-0000aef0: 5000 2000 5600 6100 7200 6900 6100 6200  P. .V.a.r.i.a.b.
-0000af00: 6c00 6500 2000 6900 6e00 2000 4100 6e00  l.e. .i.n. .A.n.
-0000af10: 6600 fc00 6800 7200 7500 6e00 6700 7300  f...h.r.u.n.g.s.
-0000af20: 7a00 6500 6900 6300 6800 6500 6e08 0000  z.e.i.c.h.e.n...
-0000af30: 0000 0600 0000 1a50 4850 2064 6f75 626c  .......PHP doubl
-0000af40: 652d 7175 6f74 6564 2076 6172 6961 626c  e-quoted variabl
-0000af50: 6507 0000 000d 5173 6369 4c65 7865 7248  e.....QsciLexerH
-0000af60: 544d 4c01 0300 0000 2200 5000 4800 5000  TML.....".P.H.P.
-0000af70: 2000 5300 6300 6800 6c00 fc00 7300 7300   .S.c.h.l...s.s.
-0000af80: 6500 6c00 7700 6f00 7200 7408 0000 0000  e.l.w.o.r.t.....
-0000af90: 0600 0000 0b50 4850 206b 6579 776f 7264  .....PHP keyword
-0000afa0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000afb0: 4d4c 0103 0000 0026 0050 0048 0050 0020  ML.....&.P.H.P. 
-0000afc0: 005a 0065 0069 006c 0065 006e 006b 006f  .Z.e.i.l.e.n.k.o
-0000afd0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-0000afe0: 0000 0006 0000 0010 5048 5020 6c69 6e65  ........PHP line
-0000aff0: 2063 6f6d 6d65 6e74 0700 0000 0d51 7363   comment.....Qsc
-0000b000: 694c 6578 6572 4854 4d4c 0103 0000 0010  iLexerHTML......
-0000b010: 0050 0048 0050 0020 005a 0061 0068 006c  .P.H.P. .Z.a.h.l
-0000b020: 0800 0000 0006 0000 000a 5048 5020 6e75  ..........PHP nu
-0000b030: 6d62 6572 0700 0000 0d51 7363 694c 6578  mber.....QsciLex
-0000b040: 6572 4854 4d4c 0103 0000 0018 0050 0048  erHTML.......P.H
-0000b050: 0050 0020 004f 0070 0065 0072 0061 0074  .P. .O.p.e.r.a.t
-0000b060: 006f 0072 0800 0000 0006 0000 000c 5048  .o.r..........PH
-0000b070: 5020 6f70 6572 6174 6f72 0700 0000 0d51  P operator.....Q
-0000b080: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000b090: 003e 0050 0048 0050 0020 005a 0065 0069  .>.P.H.P. .Z.e.i
-0000b0a0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-0000b0b0: 0065 0020 0069 006e 0020 0048 006f 0063  .e. .i.n. .H.o.c
-0000b0c0: 0068 006b 006f 006d 006d 0061 0074 0061  .h.k.o.m.m.a.t.a
-0000b0d0: 0800 0000 0006 0000 0018 5048 5020 7369  ..........PHP si
-0000b0e0: 6e67 6c65 2d71 756f 7465 6420 7374 7269  ngle-quoted stri
-0000b0f0: 6e67 0700 0000 0d51 7363 694c 6578 6572  ng.....QsciLexer
-0000b100: 4854 4d4c 0103 0000 0018 0050 0048 0050  HTML.......P.H.P
-0000b110: 0020 0056 0061 0072 0069 0061 0062 006c  . .V.a.r.i.a.b.l
-0000b120: 0065 0800 0000 0006 0000 000c 5048 5020  .e..........PHP 
-0000b130: 7661 7269 6162 6c65 0700 0000 0d51 7363  variable.....Qsc
-0000b140: 694c 6578 6572 4854 4d4c 0103 0000 0024  iLexerHTML.....$
-0000b150: 0050 0079 0074 0068 006f 006e 0020 004b  .P.y.t.h.o.n. .K
-0000b160: 006c 0061 0073 0073 0065 006e 006e 0061  .l.a.s.s.e.n.n.a
-0000b170: 006d 0065 0800 0000 0006 0000 0011 5079  .m.e..........Py
-0000b180: 7468 6f6e 2063 6c61 7373 206e 616d 6507  thon class name.
-0000b190: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
-0000b1a0: 4c01 0300 0000 2000 5000 7900 7400 6800  L..... .P.y.t.h.
-0000b1b0: 6f00 6e00 2000 4b00 6f00 6d00 6d00 6500  o.n. .K.o.m.m.e.
-0000b1c0: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
-0000b1d0: 0e50 7974 686f 6e20 636f 6d6d 656e 7407  .Python comment.
-0000b1e0: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
-0000b1f0: 4c01 0300 0000 1e00 5000 7900 7400 6800  L.......P.y.t.h.
-0000b200: 6f00 6e00 2000 5300 7400 6100 6e00 6400  o.n. .S.t.a.n.d.
-0000b210: 6100 7200 6408 0000 0000 0600 0000 0e50  a.r.d..........P
-0000b220: 7974 686f 6e20 6465 6661 756c 7407 0000  ython default...
-0000b230: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000b240: 0300 0000 5000 5000 7900 7400 6800 6f00  ....P.P.y.t.h.o.
-0000b250: 6e00 2000 5a00 6500 6900 6300 6800 6500  n. .Z.e.i.c.h.e.
-0000b260: 6e00 6b00 6500 7400 7400 6500 2000 6900  n.k.e.t.t.e. .i.
-0000b270: 6e00 2000 4100 6e00 6600 fc00 6800 7200  n. .A.n.f...h.r.
-0000b280: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
-0000b290: 6800 6500 6e08 0000 0000 0600 0000 1b50  h.e.n..........P
-0000b2a0: 7974 686f 6e20 646f 7562 6c65 2d71 756f  ython double-quo
-0000b2b0: 7465 6420 7374 7269 6e67 0700 0000 0d51  ted string.....Q
-0000b2c0: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000b2d0: 0046 0050 0079 0074 0068 006f 006e 0020  .F.P.y.t.h.o.n. 
-0000b2e0: 0046 0075 006e 006b 0074 0069 006f 006e  .F.u.n.k.t.i.o.n
-0000b2f0: 0073 002d 0020 006f 0064 0065 0072 0020  .s.-. .o.d.e.r. 
-0000b300: 004d 0065 0074 0068 006f 0064 0065 006e  .M.e.t.h.o.d.e.n
-0000b310: 006e 0061 006d 0065 0800 0000 0006 0000  .n.a.m.e........
-0000b320: 001e 5079 7468 6f6e 2066 756e 6374 696f  ..Python functio
-0000b330: 6e20 6f72 206d 6574 686f 6420 6e61 6d65  n or method name
-0000b340: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000b350: 4d4c 0103 0000 0022 0050 0079 0074 0068  ML.....".P.y.t.h
-0000b360: 006f 006e 0020 0042 0065 007a 0065 0069  .o.n. .B.e.z.e.i
-0000b370: 0063 0068 006e 0065 0072 0800 0000 0006  .c.h.n.e.r......
-0000b380: 0000 0011 5079 7468 6f6e 2069 6465 6e74  ....Python ident
-0000b390: 6966 6965 7207 0000 000d 5173 6369 4c65  ifier.....QsciLe
-0000b3a0: 7865 7248 544d 4c01 0300 0000 2800 5000  xerHTML.....(.P.
-0000b3b0: 7900 7400 6800 6f00 6e00 2000 5300 6300  y.t.h.o.n. .S.c.
-0000b3c0: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
-0000b3d0: 6f00 7200 7408 0000 0000 0600 0000 0e50  o.r.t..........P
-0000b3e0: 7974 686f 6e20 6b65 7977 6f72 6407 0000  ython keyword...
-0000b3f0: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000b400: 0300 0000 1600 5000 7900 7400 6800 6f00  ......P.y.t.h.o.
-0000b410: 6e00 2000 5a00 6100 6800 6c08 0000 0000  n. .Z.a.h.l.....
-0000b420: 0600 0000 0d50 7974 686f 6e20 6e75 6d62  .....Python numb
-0000b430: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
-0000b440: 4854 4d4c 0103 0000 001e 0050 0079 0074  HTML.......P.y.t
-0000b450: 0068 006f 006e 0020 004f 0070 0065 0072  .h.o.n. .O.p.e.r
-0000b460: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
-0000b470: 000f 5079 7468 6f6e 206f 7065 7261 746f  ..Python operato
-0000b480: 7207 0000 000d 5173 6369 4c65 7865 7248  r.....QsciLexerH
-0000b490: 544d 4c01 0300 0000 4400 5000 7900 7400  TML.....D.P.y.t.
-0000b4a0: 6800 6f00 6e00 2000 5a00 6500 6900 6300  h.o.n. .Z.e.i.c.
-0000b4b0: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
-0000b4c0: 2000 6900 6e00 2000 4800 6f00 6300 6800   .i.n. .H.o.c.h.
-0000b4d0: 6b00 6f00 6d00 6d00 6100 7400 6108 0000  k.o.m.m.a.t.a...
-0000b4e0: 0000 0600 0000 1b50 7974 686f 6e20 7369  .......Python si
-0000b4f0: 6e67 6c65 2d71 756f 7465 6420 7374 7269  ngle-quoted stri
-0000b500: 6e67 0700 0000 0d51 7363 694c 6578 6572  ng.....QsciLexer
-0000b510: 4854 4d4c 0103 0000 0066 0050 0079 0074  HTML.....f.P.y.t
-0000b520: 0068 006f 006e 0020 005a 0065 0069 0063  .h.o.n. .Z.e.i.c
-0000b530: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
-0000b540: 0020 0069 006e 0020 0064 0072 0065 0069  . .i.n. .d.r.e.i
-0000b550: 0066 0061 0063 0068 0065 006e 0020 0041  .f.a.c.h.e.n. .A
-0000b560: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
-0000b570: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
-0000b580: 0800 0000 0006 0000 0022 5079 7468 6f6e  ........."Python
-0000b590: 2074 7269 706c 6520 646f 7562 6c65 2d71   triple double-q
-0000b5a0: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
-0000b5b0: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-0000b5c0: 0000 005a 0050 0079 0074 0068 006f 006e  ...Z.P.y.t.h.o.n
-0000b5d0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-0000b5e0: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
-0000b5f0: 0020 0064 0072 0065 0069 0066 0061 0063  . .d.r.e.i.f.a.c
-0000b600: 0068 0065 006e 0020 0048 006f 0063 0068  .h.e.n. .H.o.c.h
-0000b610: 006b 006f 006d 006d 0061 0074 0061 0800  .k.o.m.m.a.t.a..
-0000b620: 0000 0006 0000 0022 5079 7468 6f6e 2074  ......."Python t
-0000b630: 7269 706c 6520 7369 6e67 6c65 2d71 756f  riple single-quo
-0000b640: 7465 6420 7374 7269 6e67 0700 0000 0d51  ted string.....Q
-0000b650: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000b660: 0024 0053 0047 004d 004c 0020 0053 0074  .$.S.G.M.L. .S.t
-0000b670: 0061 006e 0064 0061 0072 0064 0062 006c  .a.n.d.a.r.d.b.l
-0000b680: 006f 0063 006b 0800 0000 0006 0000 0012  .o.c.k..........
-0000b690: 5347 4d4c 2062 6c6f 636b 2064 6566 6175  SGML block defau
-0000b6a0: 6c74 0700 0000 0d51 7363 694c 6578 6572  lt.....QsciLexer
-0000b6b0: 4854 4d4c 0103 0000 0016 0053 0047 004d  HTML.......S.G.M
-0000b6c0: 004c 0020 0042 0065 0066 0065 0068 006c  .L. .B.e.f.e.h.l
-0000b6d0: 0800 0000 0006 0000 000c 5347 4d4c 2063  ..........SGML c
-0000b6e0: 6f6d 6d61 6e64 0700 0000 0d51 7363 694c  ommand.....QsciL
-0000b6f0: 6578 6572 4854 4d4c 0103 0000 001c 0053  exerHTML.......S
-0000b700: 0047 004d 004c 0020 004b 006f 006d 006d  .G.M.L. .K.o.m.m
-0000b710: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
-0000b720: 0000 000c 5347 4d4c 2063 6f6d 6d65 6e74  ....SGML comment
-0000b730: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000b740: 4d4c 0103 0000 001a 0053 0047 004d 004c  ML.......S.G.M.L
-0000b750: 0020 0053 0074 0061 006e 0064 0061 0072  . .S.t.a.n.d.a.r
-0000b760: 0064 0800 0000 0006 0000 000c 5347 4d4c  .d..........SGML
-0000b770: 2064 6566 6175 6c74 0700 0000 0d51 7363   default.....Qsc
-0000b780: 694c 6578 6572 4854 4d4c 0103 0000 004c  iLexerHTML.....L
-0000b790: 0053 0047 004d 004c 0020 005a 0065 0069  .S.G.M.L. .Z.e.i
-0000b7a0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-0000b7b0: 0065 0020 0069 006e 0020 0041 006e 0066  .e. .i.n. .A.n.f
-0000b7c0: 00fc 0068 0072 0075 006e 0067 0073 007a  ...h.r.u.n.g.s.z
-0000b7d0: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
-0000b7e0: 0006 0000 0019 5347 4d4c 2064 6f75 626c  ......SGML doubl
-0000b7f0: 652d 7175 6f74 6564 2073 7472 696e 6707  e-quoted string.
-0000b800: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
-0000b810: 4c01 0300 0000 1600 5300 4700 4d00 4c00  L.......S.G.M.L.
-0000b820: 2000 4600 6500 6800 6c00 6500 7208 0000   .F.e.h.l.e.r...
-0000b830: 0000 0600 0000 0a53 474d 4c20 6572 726f  .......SGML erro
-0000b840: 7207 0000 000d 5173 6369 4c65 7865 7248  r.....QsciLexerH
-0000b850: 544d 4c01 0300 0000 4000 5300 4700 4d00  TML.....@.S.G.M.
-0000b860: 4c00 2000 5a00 6500 6900 6300 6800 6500  L. .Z.e.i.c.h.e.
-0000b870: 6e00 6b00 6500 7400 7400 6500 2000 6900  n.k.e.t.t.e. .i.
-0000b880: 6e00 2000 4800 6f00 6300 6800 6b00 6f00  n. .H.o.c.h.k.o.
-0000b890: 6d00 6d00 6100 7400 6108 0000 0000 0600  m.m.a.t.a.......
-0000b8a0: 0000 1953 474d 4c20 7369 6e67 6c65 2d71  ...SGML single-q
-0000b8b0: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
-0000b8c0: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-0000b8d0: 0000 002c 0053 0047 004d 004c 0020 0053  ...,.S.G.M.L. .S
-0000b8e0: 0070 0065 007a 0069 0065 006c 006c 0065  .p.e.z.i.e.l.l.e
-0000b8f0: 0020 0045 006e 0074 0069 0074 00e4 0074  . .E.n.t.i.t...t
-0000b900: 0800 0000 0006 0000 0013 5347 4d4c 2073  ..........SGML s
-0000b910: 7065 6369 616c 2065 6e74 6974 7907 0000  pecial entity...
-0000b920: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000b930: 0300 0000 1400 5300 6b00 7200 6900 7000  ......S.k.r.i.p.
-0000b940: 7400 2000 5400 6100 6708 0000 0000 0600  t. .T.a.g.......
-0000b950: 0000 0a53 6372 6970 7420 7461 6707 0000  ...Script tag...
-0000b960: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
-0000b970: 0300 0000 4400 4200 6500 6700 6900 6e00  ....D.B.e.g.i.n.
-0000b980: 6e00 2000 6500 6900 6e00 6500 7300 2000  n. .e.i.n.e.s. .
-0000b990: 4a00 6100 7600 6100 5300 6300 7200 6900  J.a.v.a.S.c.r.i.
-0000b9a0: 7000 7400 2000 4600 7200 6100 6700 6d00  p.t. .F.r.a.g.m.
-0000b9b0: 6500 6e00 7400 6500 7308 0000 0000 0600  e.n.t.e.s.......
-0000b9c0: 0000 1e53 7461 7274 206f 6620 6120 4a61  ...Start of a Ja
-0000b9d0: 7661 5363 7269 7074 2066 7261 676d 656e  vaScript fragmen
-0000b9e0: 7407 0000 000d 5173 6369 4c65 7865 7248  t.....QsciLexerH
-0000b9f0: 544d 4c01 0300 0000 3600 4200 6500 6700  TML.....6.B.e.g.
-0000ba00: 6900 6e00 6e00 2000 6500 6900 6e00 6500  i.n.n. .e.i.n.e.
-0000ba10: 7300 2000 5000 4800 5000 2000 4600 7200  s. .P.H.P. .F.r.
-0000ba20: 6100 6700 6d00 6500 6e00 7400 6500 7308  a.g.m.e.n.t.e.s.
-0000ba30: 0000 0000 0600 0000 1753 7461 7274 206f  .........Start o
-0000ba40: 6620 6120 5048 5020 6672 6167 6d65 6e74  f a PHP fragment
-0000ba50: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000ba60: 4d4c 0103 0000 003c 0042 0065 0067 0069  ML.....<.B.e.g.i
-0000ba70: 006e 006e 0020 0065 0069 006e 0065 0073  .n.n. .e.i.n.e.s
-0000ba80: 0020 0050 0079 0074 0068 006f 006e 0020  . .P.y.t.h.o.n. 
-0000ba90: 0046 0072 0061 0067 006d 0065 006e 0074  .F.r.a.g.m.e.n.t
-0000baa0: 0065 0073 0800 0000 0006 0000 001a 5374  .e.s..........St
-0000bab0: 6172 7420 6f66 2061 2050 7974 686f 6e20  art of a Python 
-0000bac0: 6672 6167 6d65 6e74 0700 0000 0d51 7363  fragment.....Qsc
-0000bad0: 694c 6578 6572 4854 4d4c 0103 0000 0040  iLexerHTML.....@
-0000bae0: 0042 0065 0067 0069 006e 006e 0020 0065  .B.e.g.i.n.n. .e
-0000baf0: 0069 006e 0065 0073 0020 0056 0042 0053  .i.n.e.s. .V.B.S
-0000bb00: 0063 0072 0069 0070 0074 0020 0046 0072  .c.r.i.p.t. .F.r
-0000bb10: 0061 0067 006d 0065 006e 0074 0065 0073  .a.g.m.e.n.t.e.s
-0000bb20: 0800 0000 0006 0000 001c 5374 6172 7420  ..........Start 
-0000bb30: 6f66 2061 2056 4253 6372 6970 7420 6672  of a VBScript fr
-0000bb40: 6167 6d65 6e74 0700 0000 0d51 7363 694c  agment.....QsciL
-0000bb50: 6578 6572 4854 4d4c 0103 0000 004c 0042  exerHTML.....L.B
-0000bb60: 0065 0067 0069 006e 006e 0020 0065 0069  .e.g.i.n.n. .e.i
-0000bb70: 006e 0065 0073 0020 0041 0053 0050 0020  .n.e.s. .A.S.P. 
-0000bb80: 004a 0061 0076 0061 0053 0063 0072 0069  .J.a.v.a.S.c.r.i
-0000bb90: 0070 0074 0020 0046 0072 0061 0067 006d  .p.t. .F.r.a.g.m
-0000bba0: 0065 006e 0074 0065 0073 0800 0000 0006  .e.n.t.e.s......
-0000bbb0: 0000 0023 5374 6172 7420 6f66 2061 6e20  ...#Start of an 
-0000bbc0: 4153 5020 4a61 7661 5363 7269 7074 2066  ASP JavaScript f
-0000bbd0: 7261 676d 656e 7407 0000 000d 5173 6369  ragment.....Qsci
-0000bbe0: 4c65 7865 7248 544d 4c01 0300 0000 4400  LexerHTML.....D.
-0000bbf0: 4200 6500 6700 6900 6e00 6e00 2000 6500  B.e.g.i.n.n. .e.
-0000bc00: 6900 6e00 6500 7300 2000 4100 5300 5000  i.n.e.s. .A.S.P.
-0000bc10: 2000 5000 7900 7400 6800 6f00 6e00 2000   .P.y.t.h.o.n. .
-0000bc20: 4600 7200 6100 6700 6d00 6500 6e00 7400  F.r.a.g.m.e.n.t.
-0000bc30: 6500 7308 0000 0000 0600 0000 1f53 7461  e.s..........Sta
-0000bc40: 7274 206f 6620 616e 2041 5350 2050 7974  rt of an ASP Pyt
-0000bc50: 686f 6e20 6672 6167 6d65 6e74 0700 0000  hon fragment....
-0000bc60: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
-0000bc70: 0000 0048 0042 0065 0067 0069 006e 006e  ...H.B.e.g.i.n.n
-0000bc80: 0020 0065 0069 006e 0065 0073 0020 0041  . .e.i.n.e.s. .A
-0000bc90: 0053 0050 0020 0056 0042 0053 0063 0072  .S.P. .V.B.S.c.r
-0000bca0: 0069 0070 0074 0020 0046 0072 0061 0067  .i.p.t. .F.r.a.g
-0000bcb0: 006d 0065 006e 0074 0065 0073 0800 0000  .m.e.n.t.e.s....
-0000bcc0: 0006 0000 0021 5374 6172 7420 6f66 2061  .....!Start of a
-0000bcd0: 6e20 4153 5020 5642 5363 7269 7074 2066  n ASP VBScript f
-0000bce0: 7261 676d 656e 7407 0000 000d 5173 6369  ragment.....Qsci
-0000bcf0: 4c65 7865 7248 544d 4c01 0300 0000 3600  LexerHTML.....6.
-0000bd00: 4200 6500 6700 6900 6e00 6e00 2000 6500  B.e.g.i.n.n. .e.
-0000bd10: 6900 6e00 6500 7300 2000 4100 5300 5000  i.n.e.s. .A.S.P.
-0000bd20: 2000 4600 7200 6100 6700 6d00 6500 6e00   .F.r.a.g.m.e.n.
-0000bd30: 7400 6500 7308 0000 0000 0600 0000 1853  t.e.s..........S
-0000bd40: 7461 7274 206f 6620 616e 2041 5350 2066  tart of an ASP f
-0000bd50: 7261 676d 656e 7407 0000 000d 5173 6369  ragment.....Qsci
-0000bd60: 4c65 7865 7248 544d 4c01 0300 0000 4200  LexerHTML.....B.
-0000bd70: 4200 6500 6700 6900 6e00 6e00 2000 6500  B.e.g.i.n.n. .e.
-0000bd80: 6900 6e00 6500 7300 2000 4100 5300 5000  i.n.e.s. .A.S.P.
-0000bd90: 2000 4600 7200 6100 6700 6d00 6500 6e00   .F.r.a.g.m.e.n.
-0000bda0: 7400 6500 7300 2000 6d00 6900 7400 2000  t.e.s. .m.i.t. .
-0000bdb0: 4008 0000 0000 0600 0000 1f53 7461 7274  @..........Start
-0000bdc0: 206f 6620 616e 2041 5350 2066 7261 676d   of an ASP fragm
-0000bdd0: 656e 7420 7769 7468 2040 0700 0000 0d51  ent with @.....Q
-0000bde0: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000bdf0: 0036 0042 0065 0067 0069 006e 006e 0020  .6.B.e.g.i.n.n. 
-0000be00: 0065 0069 006e 0065 0073 0020 0058 004d  .e.i.n.e.s. .X.M
-0000be10: 004c 0020 0046 0072 0061 0067 006d 0065  .L. .F.r.a.g.m.e
-0000be20: 006e 0074 0065 0073 0800 0000 0006 0000  .n.t.e.s........
-0000be30: 0018 5374 6172 7420 6f66 2061 6e20 584d  ..Start of an XM
-0000be40: 4c20 6672 6167 6d65 6e74 0700 0000 0d51  L fragment.....Q
-0000be50: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000be60: 0006 0054 0061 0067 0800 0000 0006 0000  ...T.a.g........
-0000be70: 0003 5461 6707 0000 000d 5173 6369 4c65  ..Tag.....QsciLe
-0000be80: 7865 7248 544d 4c01 0300 0000 2800 5500  xerHTML.....(.U.
-0000be90: 6e00 6200 6500 6b00 6100 6e00 6e00 7400  n.b.e.k.a.n.n.t.
-0000bea0: 6500 7300 2000 4100 7400 7400 7200 6900  e.s. .A.t.t.r.i.
-0000beb0: 6200 7500 7408 0000 0000 0600 0000 1155  b.u.t..........U
-0000bec0: 6e6b 6e6f 776e 2061 7474 7269 6275 7465  nknown attribute
+00007020: 3600 4900 6e00 6100 6b00 7400 6900 7600  6.I.n.a.k.t.i.v.
+00007030: 6500 2000 4100 7500 6600 6700 6100 6200  e. .A.u.f.g.a.b.
+00007040: 6500 6e00 6d00 6100 7200 6b00 6900 6500  e.n.m.a.r.k.i.e.
+00007050: 7200 7500 6e00 6708 0000 0000 0600 0000  r.u.n.g.........
+00007060: 1449 6e61 6374 6976 6520 7461 736b 206d  .Inactive task m
+00007070: 6172 6b65 7207 0000 000c 5173 6369 4c65  arker.....QsciLe
+00007080: 7865 7243 5050 0103 0000 0040 0049 006e  xerCPP.....@.I.n
+00007090: 0061 006b 0074 0069 0076 0065 0020 0075  .a.k.t.i.v.e. .u
+000070a0: 006e 0062 0065 0065 006e 0064 0065 0074  .n.b.e.e.n.d.e.t
+000070b0: 0065 0020 005a 0065 0069 0063 0068 0065  .e. .Z.e.i.c.h.e
+000070c0: 006e 006b 0065 0074 0074 0065 0800 0000  .n.k.e.t.t.e....
+000070d0: 0006 0000 0018 496e 6163 7469 7665 2075  ......Inactive u
+000070e0: 6e63 6c6f 7365 6420 7374 7269 6e67 0700  nclosed string..
+000070f0: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
+00007100: 0300 0000 4800 4900 6e00 6100 6b00 7400  ....H.I.n.a.k.t.
+00007110: 6900 7600 6500 7300 2000 4e00 7500 7400  i.v.e.s. .N.u.t.
+00007120: 7a00 6500 7200 2000 6400 6500 6600 6900  z.e.r. .d.e.f.i.
+00007130: 6e00 6900 6500 7200 7400 6500 7300 2000  n.i.e.r.t.e.s. .
+00007140: 4c00 6900 7400 6500 7200 6100 6c08 0000  L.i.t.e.r.a.l...
+00007150: 0000 0600 0000 1d49 6e61 6374 6976 6520  .......Inactive 
+00007160: 7573 6572 2d64 6566 696e 6564 206c 6974  user-defined lit
+00007170: 6572 616c 0700 0000 0c51 7363 694c 6578  eral.....QsciLex
+00007180: 6572 4350 5001 0300 0000 2a00 4a00 6100  erCPP.....*.J.a.
+00007190: 7600 6100 4400 6f00 6300 2000 5300 6300  v.a.D.o.c. .S.c.
+000071a0: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
+000071b0: 6f00 7200 7408 0000 0000 0600 0000 0f4a  o.r.t..........J
+000071c0: 6176 6144 6f63 206b 6579 776f 7264 0700  avaDoc keyword..
+000071d0: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
+000071e0: 0300 0000 3600 4a00 6100 7600 6100 4400  ....6.J.a.v.a.D.
+000071f0: 6f00 6300 2000 5300 6300 6800 6c00 fc00  o.c. .S.c.h.l...
+00007200: 7300 7300 6500 6c00 7700 6f00 7200 7400  s.s.e.l.w.o.r.t.
+00007210: 6600 6500 6800 6c00 6500 7208 0000 0000  f.e.h.l.e.r.....
+00007220: 0600 0000 154a 6176 6144 6f63 206b 6579  .....JavaDoc key
+00007230: 776f 7264 2065 7272 6f72 0700 0000 0c51  word error.....Q
+00007240: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
+00007250: 2600 4a00 6100 7600 6100 4400 6f00 6300  &.J.a.v.a.D.o.c.
+00007260: 2000 4300 2000 4b00 6f00 6d00 6d00 6500   .C. .K.o.m.m.e.
+00007270: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
+00007280: 174a 6176 6144 6f63 2073 7479 6c65 2043  .JavaDoc style C
+00007290: 2063 6f6d 6d65 6e74 0700 0000 0c51 7363   comment.....Qsc
+000072a0: 694c 6578 6572 4350 5001 0300 0000 2a00  iLexerCPP.....*.
+000072b0: 4a00 6100 7600 6100 4400 6f00 6300 2000  J.a.v.a.D.o.c. .
+000072c0: 4300 2b00 2b00 2000 4b00 6f00 6d00 6d00  C.+.+. .K.o.m.m.
+000072d0: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
+000072e0: 0000 194a 6176 6144 6f63 2073 7479 6c65  ...JavaDoc style
+000072f0: 2043 2b2b 2063 6f6d 6d65 6e74 0700 0000   C++ comment....
+00007300: 0c51 7363 694c 6578 6572 4350 5001 0300  .QsciLexerCPP...
+00007310: 0000 3a00 4a00 6100 7600 6100 4400 6f00  ..:.J.a.v.a.D.o.
+00007320: 6300 2000 5000 7200 e400 7000 7200 6f00  c. .P.r...p.r.o.
+00007330: 7a00 6500 7300 7300 6f00 7200 6b00 6f00  z.e.s.s.o.r.k.o.
+00007340: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+00007350: 0000 0600 0000 234a 6176 6144 6f63 2073  ......#JavaDoc s
+00007360: 7479 6c65 2070 7265 2d70 726f 6365 7373  tyle pre-process
+00007370: 6f72 2063 6f6d 6d65 6e74 0700 0000 0c51  or comment.....Q
+00007380: 7363 694c 6578 6572 4350 5001 0300 0000  sciLexerCPP.....
+00007390: 3a00 4a00 6100 7600 6100 5300 6300 7200  :.J.a.v.a.S.c.r.
+000073a0: 6900 7000 7400 2000 5200 6500 6700 7500  i.p.t. .R.e.g.u.
+000073b0: 6c00 e400 7200 6500 7200 2000 4100 7500  l...r.e.r. .A.u.
+000073c0: 7300 6400 7200 7500 6300 6b08 0000 0000  s.d.r.u.c.k.....
+000073d0: 0600 0000 1d4a 6176 6153 6372 6970 7420  .....JavaScript 
+000073e0: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+000073f0: 6f6e 0700 0000 0c51 7363 694c 6578 6572  on.....QsciLexer
+00007400: 4350 5001 0300 0000 1a00 5300 6300 6800  CPP.......S.c.h.
+00007410: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
+00007420: 7200 7408 0000 0000 0600 0000 074b 6579  r.t..........Key
+00007430: 776f 7264 0700 0000 0c51 7363 694c 6578  word.....QsciLex
+00007440: 6572 4350 5001 0300 0000 0800 5a00 6100  erCPP.......Z.a.
+00007450: 6800 6c08 0000 0000 0600 0000 064e 756d  h.l..........Num
+00007460: 6265 7207 0000 000c 5173 6369 4c65 7865  ber.....QsciLexe
+00007470: 7243 5050 0103 0000 0010 004f 0070 0065  rCPP.......O.p.e
+00007480: 0072 0061 0074 006f 0072 0800 0000 0006  .r.a.t.o.r......
+00007490: 0000 0008 4f70 6572 6174 6f72 0700 0000  ....Operator....
+000074a0: 0c51 7363 694c 6578 6572 4350 5001 0300  .QsciLexerCPP...
+000074b0: 0000 5400 5000 6900 6b00 6500 2000 5a00  ..T.P.i.k.e. .Z.
+000074c0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+000074d0: 7400 7400 6500 2000 6900 6e00 2000 2700  t.t.e. .i.n. .'.
+000074e0: 2300 2d00 4100 6e00 6600 fc00 6800 7200  #.-.A.n.f...h.r.
+000074f0: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
+00007500: 6800 6500 6e00 2708 0000 0000 0600 0000  h.e.n.'.........
+00007510: 1750 696b 6520 6861 7368 2d71 756f 7465  .Pike hash-quote
+00007520: 6420 7374 7269 6e67 0700 0000 0c51 7363  d string.....Qsc
+00007530: 694c 6578 6572 4350 5001 0300 0000 2e00  iLexerCPP.......
+00007540: 4300 2000 5000 7200 e400 7000 7200 6f00  C. .P.r...p.r.o.
+00007550: 7a00 6500 7300 7300 6f00 7200 6b00 6f00  z.e.s.s.o.r.k.o.
+00007560: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+00007570: 0000 0600 0000 1750 7265 2d70 726f 6365  .......Pre-proce
+00007580: 7373 6f72 2043 2063 6f6d 6d65 6e74 0700  ssor C comment..
+00007590: 0000 0c51 7363 694c 6578 6572 4350 5001  ...QsciLexerCPP.
+000075a0: 0300 0000 2200 5000 7200 e400 7000 7200  ....".P.r...p.r.
+000075b0: 6f00 7a00 6500 7300 7300 6f00 7200 6200  o.z.e.s.s.o.r.b.
+000075c0: 6c00 6f00 6300 6b08 0000 0000 0600 0000  l.o.c.k.........
+000075d0: 1350 7265 2d70 726f 6365 7373 6f72 2062  .Pre-processor b
+000075e0: 6c6f 636b 0700 0000 0c51 7363 694c 6578  lock.....QsciLex
+000075f0: 6572 4350 5001 0300 0000 5000 5300 6500  erCPP.....P.S.e.
+00007600: 6b00 7500 6e00 6400 e400 7200 6500 2000  k.u.n.d...r.e. .
+00007610: 5300 6300 6800 6c00 7500 7300 7300 6500  S.c.h.l.u.s.s.e.
+00007620: 6c00 7700 f600 7200 7400 6500 7200 2000  l.w...r.t.e.r. .
+00007630: 7500 6e00 6400 2000 4200 6500 7a00 6500  u.n.d. .B.e.z.e.
+00007640: 6900 6300 6800 6e00 6500 7208 0000 0000  i.c.h.n.e.r.....
+00007650: 0600 0000 2253 6563 6f6e 6461 7279 206b  ...."Secondary k
+00007660: 6579 776f 7264 7320 616e 6420 6964 656e  eywords and iden
+00007670: 7469 6669 6572 7307 0000 000c 5173 6369  tifiers.....Qsci
+00007680: 4c65 7865 7243 5050 0103 0000 0036 005a  LexerCPP.....6.Z
+00007690: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
+000076a0: 0074 0074 0065 0020 0069 006e 0020 0048  .t.t.e. .i.n. .H
+000076b0: 006f 0063 0068 006b 006f 006d 006d 0061  .o.c.h.k.o.m.m.a
+000076c0: 0074 0061 0800 0000 0006 0000 0014 5369  .t.a..........Si
+000076d0: 6e67 6c65 2d71 756f 7465 6420 7374 7269  ngle-quoted stri
+000076e0: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
+000076f0: 4350 5001 0300 0000 2400 4100 7500 6600  CPP.....$.A.u.f.
+00007700: 6700 6100 6200 6500 6e00 6d00 6100 7200  g.a.b.e.n.m.a.r.
+00007710: 6b00 6900 6500 7200 7500 6e00 6708 0000  k.i.e.r.u.n.g...
+00007720: 0000 0600 0000 0b54 6173 6b20 6d61 726b  .......Task mark
+00007730: 6572 0700 0000 0c51 7363 694c 6578 6572  er.....QsciLexer
+00007740: 4350 5001 0300 0000 2e00 5500 6e00 6200  CPP.......U.n.b.
+00007750: 6500 6500 6e00 6400 6500 7400 6500 2000  e.e.n.d.e.t.e. .
+00007760: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+00007770: 6500 7400 7400 6508 0000 0000 0600 0000  e.t.t.e.........
+00007780: 0f55 6e63 6c6f 7365 6420 7374 7269 6e67  .Unclosed string
+00007790: 0700 0000 0c51 7363 694c 6578 6572 4350  .....QsciLexerCP
+000077a0: 5001 0300 0000 3400 4e00 7500 7400 7a00  P.....4.N.u.t.z.
+000077b0: 6500 7200 2000 6400 6500 6600 6900 6e00  e.r. .d.e.f.i.n.
+000077c0: 6900 6500 7200 7400 6500 7300 2000 4c00  i.e.r.t.e.s. .L.
+000077d0: 6900 7400 6500 7200 6100 6c08 0000 0000  i.t.e.r.a.l.....
+000077e0: 0600 0000 1455 7365 722d 6465 6669 6e65  .....User-define
+000077f0: 6420 6c69 7465 7261 6c07 0000 000c 5173  d literal.....Qs
+00007800: 6369 4c65 7865 7243 5050 0103 0000 0056  ciLexerCPP.....V
+00007810: 0056 0061 006c 0061 0020 005a 0065 0069  .V.a.l.a. .Z.e.i
+00007820: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
+00007830: 0065 0020 0069 006e 0020 0064 0072 0065  .e. .i.n. .d.r.e
+00007840: 0069 0066 0061 0063 0068 0065 006e 0020  .i.f.a.c.h.e.n. 
+00007850: 0048 006f 0063 0068 006b 006f 006d 006d  .H.o.c.h.k.o.m.m
+00007860: 0061 0074 0061 0800 0000 0006 0000 0022  .a.t.a........."
+00007870: 5661 6c61 2074 7269 706c 652d 7175 6f74  Vala triple-quot
+00007880: 6564 2076 6572 6261 7469 6d20 7374 7269  ed verbatim stri
+00007890: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
+000078a0: 4350 5001 0300 0000 0e00 4000 2d00 5200  CPP.......@.-.R.
+000078b0: 6500 6700 6500 6c08 0000 0000 0600 0000  e.g.e.l.........
+000078c0: 0640 2d72 756c 6507 0000 000c 5173 6369  .@-rule.....Qsci
+000078d0: 4c65 7865 7243 5353 0103 0000 0010 0041  LexerCSS.......A
+000078e0: 0074 0074 0072 0069 0062 0075 0074 0800  .t.t.r.i.b.u.t..
+000078f0: 0000 0006 0000 0009 4174 7472 6962 7574  ........Attribut
+00007900: 6507 0000 000c 5173 6369 4c65 7865 7243  e.....QsciLexerC
+00007910: 5353 0103 0000 0020 0043 0053 0053 0031  SS..... .C.S.S.1
+00007920: 0020 0045 0069 0067 0065 006e 0073 0063  . .E.i.g.e.n.s.c
+00007930: 0068 0061 0066 0074 0800 0000 0006 0000  .h.a.f.t........
+00007940: 000d 4353 5331 2070 726f 7065 7274 7907  ..CSS1 property.
+00007950: 0000 000c 5173 6369 4c65 7865 7243 5353  ....QsciLexerCSS
+00007960: 0103 0000 0020 0043 0053 0053 0032 0020  ..... .C.S.S.2. 
+00007970: 0045 0069 0067 0065 006e 0073 0063 0068  .E.i.g.e.n.s.c.h
+00007980: 0061 0066 0074 0800 0000 0006 0000 000d  .a.f.t..........
+00007990: 4353 5332 2070 726f 7065 7274 7907 0000  CSS2 property...
+000079a0: 000c 5173 6369 4c65 7865 7243 5353 0103  ..QsciLexerCSS..
+000079b0: 0000 0020 0043 0053 0053 0033 0020 0045  ... .C.S.S.3. .E
+000079c0: 0069 0067 0065 006e 0073 0063 0068 0061  .i.g.e.n.s.c.h.a
+000079d0: 0066 0074 0800 0000 0006 0000 000d 4353  .f.t..........CS
+000079e0: 5333 2070 726f 7065 7274 7907 0000 000c  S3 property.....
+000079f0: 5173 6369 4c65 7865 7243 5353 0103 0000  QsciLexerCSS....
+00007a00: 001e 004b 006c 0061 0073 0073 0065 006e  ...K.l.a.s.s.e.n
+00007a10: 0073 0065 006c 0065 006b 0074 006f 0072  .s.e.l.e.k.t.o.r
+00007a20: 0800 0000 0006 0000 000e 436c 6173 7320  ..........Class 
+00007a30: 7365 6c65 6374 6f72 0700 0000 0c51 7363  selector.....Qsc
+00007a40: 694c 6578 6572 4353 5301 0300 0000 1200  iLexerCSS.......
+00007a50: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00007a60: 7208 0000 0000 0600 0000 0743 6f6d 6d65  r..........Comme
+00007a70: 6e74 0700 0000 0c51 7363 694c 6578 6572  nt.....QsciLexer
+00007a80: 4353 5301 0300 0000 1000 5300 7400 6100  CSS.......S.t.a.
+00007a90: 6e00 6400 6100 7200 6408 0000 0000 0600  n.d.a.r.d.......
+00007aa0: 0000 0744 6566 6175 6c74 0700 0000 0c51  ...Default.....Q
+00007ab0: 7363 694c 6578 6572 4353 5301 0300 0000  sciLexerCSS.....
+00007ac0: 4200 5a00 6500 6900 6300 6800 6500 6e00  B.Z.e.i.c.h.e.n.
+00007ad0: 6b00 6500 7400 7400 6500 2000 6900 6e00  k.e.t.t.e. .i.n.
+00007ae0: 2000 4100 6e00 6600 fc00 6800 7200 7500   .A.n.f...h.r.u.
+00007af0: 6e00 6700 7300 7a00 6500 6900 6300 6800  n.g.s.z.e.i.c.h.
+00007b00: 6500 6e08 0000 0000 0600 0000 1444 6f75  e.n..........Dou
+00007b10: 626c 652d 7175 6f74 6564 2073 7472 696e  ble-quoted strin
+00007b20: 6707 0000 000c 5173 6369 4c65 7865 7243  g.....QsciLexerC
+00007b30: 5353 0103 0000 0034 0045 0072 0077 0065  SS.....4.E.r.w.e
+00007b40: 0069 0074 0065 0072 0074 0065 0020 0043  .i.t.e.r.t.e. .C
+00007b50: 0053 0053 0020 0045 0069 0067 0065 006e  .S.S. .E.i.g.e.n
+00007b60: 0073 0063 0068 0061 0066 0074 0800 0000  .s.c.h.a.f.t....
+00007b70: 0006 0000 0015 4578 7465 6e64 6564 2043  ......Extended C
+00007b80: 5353 2070 726f 7065 7274 7907 0000 000c  SS property.....
+00007b90: 5173 6369 4c65 7865 7243 5353 0103 0000  QsciLexerCSS....
+00007ba0: 002e 0045 0072 0077 0065 0069 0074 0065  ...E.r.w.e.i.t.e
+00007bb0: 0072 0074 0065 0020 0050 0073 0065 0075  .r.t.e. .P.s.e.u
+00007bc0: 0064 006f 006b 006c 0061 0073 0073 0065  .d.o.k.l.a.s.s.e
+00007bd0: 0800 0000 0006 0000 0015 4578 7465 6e64  ..........Extend
+00007be0: 6564 2070 7365 7564 6f2d 636c 6173 7307  ed pseudo-class.
+00007bf0: 0000 000c 5173 6369 4c65 7865 7243 5353  ....QsciLexerCSS
+00007c00: 0103 0000 0032 0045 0072 0077 0065 0069  .....2.E.r.w.e.i
+00007c10: 0074 0065 0072 0074 0065 0073 0020 0050  .t.e.r.t.e.s. .P
+00007c20: 0073 0065 0075 0064 006f 0065 006c 0065  .s.e.u.d.o.e.l.e
+00007c30: 006d 0065 006e 0074 0800 0000 0006 0000  .m.e.n.t........
+00007c40: 0017 4578 7465 6e64 6564 2070 7365 7564  ..Extended pseud
+00007c50: 6f2d 656c 656d 656e 7407 0000 000c 5173  o-element.....Qs
+00007c60: 6369 4c65 7865 7243 5353 0103 0000 0016  ciLexerCSS......
+00007c70: 0049 0044 002d 0053 0065 006c 0065 006b  .I.D.-.S.e.l.e.k
+00007c80: 0074 006f 0072 0800 0000 0006 0000 000b  .t.o.r..........
+00007c90: 4944 2073 656c 6563 746f 7207 0000 000c  ID selector.....
+00007ca0: 5173 6369 4c65 7865 7243 5353 0103 0000  QsciLexerCSS....
+00007cb0: 000e 0057 0069 0063 0068 0074 0069 0067  ...W.i.c.h.t.i.g
+00007cc0: 0800 0000 0006 0000 0009 496d 706f 7274  ..........Import
+00007cd0: 616e 7407 0000 000c 5173 6369 4c65 7865  ant.....QsciLexe
+00007ce0: 7243 5353 0103 0000 0016 004d 0065 0064  rCSS.......M.e.d
+00007cf0: 0069 0065 006e 0072 0065 0067 0065 006c  .i.e.n.r.e.g.e.l
+00007d00: 0800 0000 0006 0000 000a 4d65 6469 6120  ..........Media 
+00007d10: 7275 6c65 0700 0000 0c51 7363 694c 6578  rule.....QsciLex
+00007d20: 6572 4353 5301 0300 0000 1000 4f00 7000  erCSS.......O.p.
+00007d30: 6500 7200 6100 7400 6f00 7208 0000 0000  e.r.a.t.o.r.....
+00007d40: 0600 0000 084f 7065 7261 746f 7207 0000  .....Operator...
+00007d50: 000c 5173 6369 4c65 7865 7243 5353 0103  ..QsciLexerCSS..
+00007d60: 0000 0018 0050 0073 0065 0075 0064 006f  .....P.s.e.u.d.o
+00007d70: 006b 006c 0061 0073 0073 0065 0800 0000  .k.l.a.s.s.e....
+00007d80: 0006 0000 000c 5073 6575 646f 2d63 6c61  ......Pseudo-cla
+00007d90: 7373 0700 0000 0c51 7363 694c 6578 6572  ss.....QsciLexer
+00007da0: 4353 5301 0300 0000 1a00 5000 7300 6500  CSS.......P.s.e.
+00007db0: 7500 6400 6f00 6500 6c00 6500 6d00 6500  u.d.o.e.l.e.m.e.
+00007dc0: 6e00 7408 0000 0000 0600 0000 0e50 7365  n.t..........Pse
+00007dd0: 7564 6f2d 656c 656d 656e 7407 0000 000c  udo-element.....
+00007de0: 5173 6369 4c65 7865 7243 5353 0103 0000  QsciLexerCSS....
+00007df0: 0036 005a 0065 0069 0063 0068 0065 006e  .6.Z.e.i.c.h.e.n
+00007e00: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
+00007e10: 0020 0048 006f 0063 0068 006b 006f 006d  . .H.o.c.h.k.o.m
+00007e20: 006d 0061 0074 0061 0800 0000 0006 0000  .m.a.t.a........
+00007e30: 0014 5369 6e67 6c65 2d71 756f 7465 6420  ..Single-quoted 
+00007e40: 7374 7269 6e67 0700 0000 0c51 7363 694c  string.....QsciL
+00007e50: 6578 6572 4353 5301 0300 0000 0600 5400  exerCSS.......T.
+00007e60: 6100 6708 0000 0000 0600 0000 0354 6167  a.g..........Tag
+00007e70: 0700 0000 0c51 7363 694c 6578 6572 4353  .....QsciLexerCS
+00007e80: 5301 0300 0000 2c00 5500 6e00 6200 6500  S.....,.U.n.b.e.
+00007e90: 6b00 6100 6e00 6e00 7400 6500 2000 4500  k.a.n.n.t.e. .E.
+00007ea0: 6900 6700 6500 6e00 7300 6300 6800 6100  i.g.e.n.s.c.h.a.
+00007eb0: 6600 7408 0000 0000 0600 0000 1055 6e6b  f.t..........Unk
+00007ec0: 6e6f 776e 2070 726f 7065 7274 7907 0000  nown property...
+00007ed0: 000c 5173 6369 4c65 7865 7243 5353 0103  ..QsciLexerCSS..
+00007ee0: 0000 002e 0055 006e 0062 0065 006b 0061  .....U.n.b.e.k.a
+00007ef0: 006e 006e 0074 0065 0020 0050 0073 0065  .n.n.t.e. .P.s.e
+00007f00: 0075 0064 006f 006b 006c 0061 0073 0073  .u.d.o.k.l.a.s.s
+00007f10: 0065 0800 0000 0006 0000 0014 556e 6b6e  .e..........Unkn
+00007f20: 6f77 6e20 7073 6575 646f 2d63 6c61 7373  own pseudo-class
+00007f30: 0700 0000 0c51 7363 694c 6578 6572 4353  .....QsciLexerCS
+00007f40: 5301 0300 0000 0800 5700 6500 7200 7408  S.......W.e.r.t.
+00007f50: 0000 0000 0600 0000 0556 616c 7565 0700  .........Value..
+00007f60: 0000 0c51 7363 694c 6578 6572 4353 5301  ...QsciLexerCSS.
+00007f70: 0300 0000 1000 5600 6100 7200 6900 6100  ......V.a.r.i.a.
+00007f80: 6200 6c00 6508 0000 0000 0600 0000 0856  b.l.e..........V
+00007f90: 6172 6961 626c 6507 0000 000c 5173 6369  ariable.....Qsci
+00007fa0: 4c65 7865 7243 5353 0103 0000 003a 0055  LexerCSS.....:.U
+00007fb0: 006e 0069 006e 0074 0065 0072 0070 0072  .n.i.n.t.e.r.p.r
+00007fc0: 0065 0074 0069 0065 0072 0074 0065 0020  .e.t.i.e.r.t.e. 
+00007fd0: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+00007fe0: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
+00007ff0: 000f 5665 7262 6174 696d 2073 7472 696e  ..Verbatim strin
+00008000: 6707 0000 000f 5173 6369 4c65 7865 7243  g.....QsciLexerC
+00008010: 5368 6172 7001 0300 0000 1c00 4200 6c00  Sharp.......B.l.
+00008020: 6f00 6300 6b00 6b00 6f00 6d00 6d00 6500  o.c.k.k.o.m.m.e.
+00008030: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
+00008040: 0d42 6c6f 636b 2063 6f6d 6d65 6e74 0700  .Block comment..
+00008050: 0000 1551 7363 694c 6578 6572 436f 6666  ...QsciLexerCoff
+00008060: 6565 5363 7269 7074 0103 0000 0030 0052  eeScript.....0.R
+00008070: 0065 0067 0075 006c 00e4 0072 0065 0072  .e.g.u.l...r.e.r
+00008080: 0020 0041 0075 0073 0064 0072 0075 0063  . .A.u.s.d.r.u.c
+00008090: 006b 0073 0062 006c 006f 0063 006b 0800  .k.s.b.l.o.c.k..
+000080a0: 0000 0006 0000 0018 426c 6f63 6b20 7265  ........Block re
+000080b0: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+000080c0: 0700 0000 1551 7363 694c 6578 6572 436f  .....QsciLexerCo
+000080d0: 6666 6565 5363 7269 7074 0103 0000 0042  ffeeScript.....B
+000080e0: 0052 0065 0067 0075 006c 00e4 0072 0065  .R.e.g.u.l...r.e
+000080f0: 0072 0020 0041 0075 0073 0064 0072 0075  .r. .A.u.s.d.r.u
+00008100: 0063 006b 0073 0062 006c 006f 0063 006b  .c.k.s.b.l.o.c.k
+00008110: 006b 006f 006d 006d 0065 006e 0074 0061  .k.o.m.m.e.n.t.a
+00008120: 0072 0800 0000 0006 0000 0020 426c 6f63  .r......... Bloc
+00008130: 6b20 7265 6775 6c61 7220 6578 7072 6573  k regular expres
+00008140: 7369 6f6e 2063 6f6d 6d65 6e74 0700 0000  sion comment....
+00008150: 1551 7363 694c 6578 6572 436f 6666 6565  .QsciLexerCoffee
+00008160: 5363 7269 7074 0103 0000 0040 0055 006e  Script.....@.U.n
+00008170: 0069 006e 0074 0065 0072 0070 0072 0065  .i.n.t.e.r.p.r.e
+00008180: 0074 0069 0065 0072 0074 0065 0020 0043  .t.i.e.r.t.e. .C
+00008190: 0023 0020 005a 0065 0069 0063 0068 0065  .#. .Z.e.i.c.h.e
+000081a0: 006e 006b 0065 0074 0074 0065 0800 0000  .n.k.e.t.t.e....
+000081b0: 0006 0000 0012 4323 2076 6572 6261 7469  ......C# verbati
+000081c0: 6d20 7374 7269 6e67 0700 0000 1551 7363  m string.....Qsc
+000081d0: 694c 6578 6572 436f 6666 6565 5363 7269  iLexerCoffeeScri
+000081e0: 7074 0103 0000 001a 0043 002b 002b 0020  pt.......C.+.+. 
+000081f0: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
+00008200: 0072 0800 0000 0006 0000 0011 432b 2b2d  .r..........C++-
+00008210: 7374 796c 6520 636f 6d6d 656e 7407 0000  style comment...
+00008220: 0015 5173 6369 4c65 7865 7243 6f66 6665  ..QsciLexerCoffe
+00008230: 6553 6372 6970 7401 0300 0000 1600 4300  eScript.......C.
+00008240: 2000 4b00 6f00 6d00 6d00 6500 6e00 7400   .K.o.m.m.e.n.t.
+00008250: 6100 7208 0000 0000 0600 0000 0f43 2d73  a.r..........C-s
+00008260: 7479 6c65 2063 6f6d 6d65 6e74 0700 0000  tyle comment....
+00008270: 1551 7363 694c 6578 6572 436f 6666 6565  .QsciLexerCoffee
+00008280: 5363 7269 7074 0103 0000 0010 0053 0074  Script.......S.t
+00008290: 0061 006e 0064 0061 0072 0064 0800 0000  .a.n.d.a.r.d....
+000082a0: 0006 0000 0007 4465 6661 756c 7407 0000  ......Default...
+000082b0: 0015 5173 6369 4c65 7865 7243 6f66 6665  ..QsciLexerCoffe
+000082c0: 6553 6372 6970 7401 0300 0000 4200 5a00  eScript.....B.Z.
+000082d0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+000082e0: 7400 7400 6500 2000 6900 6e00 2000 4100  t.t.e. .i.n. .A.
+000082f0: 6e00 6600 fc00 6800 7200 7500 6e00 6700  n.f...h.r.u.n.g.
+00008300: 7300 7a00 6500 6900 6300 6800 6500 6e08  s.z.e.i.c.h.e.n.
+00008310: 0000 0000 0600 0000 1444 6f75 626c 652d  .........Double-
+00008320: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
+00008330: 0015 5173 6369 4c65 7865 7243 6f66 6665  ..QsciLexerCoffe
+00008340: 6553 6372 6970 7401 0300 0000 1e00 4700  eScript.......G.
+00008350: 6c00 6f00 6200 6100 6c00 6500 2000 4b00  l.o.b.a.l.e. .K.
+00008360: 6c00 6100 7300 7300 6500 6e08 0000 0000  l.a.s.s.e.n.....
+00008370: 0600 0000 0e47 6c6f 6261 6c20 636c 6173  .....Global clas
+00008380: 7365 7307 0000 0015 5173 6369 4c65 7865  ses.....QsciLexe
+00008390: 7243 6f66 6665 6553 6372 6970 7401 0300  rCoffeeScript...
+000083a0: 0000 1000 4900 4400 4c00 2000 5500 5500  ....I.D.L. .U.U.
+000083b0: 4900 4408 0000 0000 0600 0000 0849 444c  I.D..........IDL
+000083c0: 2055 5549 4407 0000 0015 5173 6369 4c65   UUID.....QsciLe
+000083d0: 7865 7243 6f66 6665 6553 6372 6970 7401  xerCoffeeScript.
+000083e0: 0300 0000 1400 4200 6500 7a00 6500 6900  ......B.e.z.e.i.
+000083f0: 6300 6800 6e00 6500 7208 0000 0000 0600  c.h.n.e.r.......
+00008400: 0000 0a49 6465 6e74 6966 6965 7207 0000  ...Identifier...
+00008410: 0015 5173 6369 4c65 7865 7243 6f66 6665  ..QsciLexerCoffe
+00008420: 6553 6372 6970 7401 0300 0000 2600 4900  eScript.....&.I.
+00008430: 6e00 7300 7400 6100 6e00 7a00 2d00 4500  n.s.t.a.n.z.-.E.
+00008440: 6900 6700 6500 6e00 7300 6300 6800 6100  i.g.e.n.s.c.h.a.
+00008450: 6600 7408 0000 0000 0600 0000 1149 6e73  f.t..........Ins
+00008460: 7461 6e63 6520 7072 6f70 6572 7479 0700  tance property..
+00008470: 0000 1551 7363 694c 6578 6572 436f 6666  ...QsciLexerCoff
+00008480: 6565 5363 7269 7074 0103 0000 002a 004a  eeScript.....*.J
+00008490: 0061 0076 0061 0044 006f 0063 0020 0043  .a.v.a.D.o.c. .C
+000084a0: 002b 002b 0020 004b 006f 006d 006d 0065  .+.+. .K.o.m.m.e
+000084b0: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
+000084c0: 0019 4a61 7661 446f 6320 432b 2b2d 7374  ..JavaDoc C++-st
+000084d0: 796c 6520 636f 6d6d 656e 7407 0000 0015  yle comment.....
+000084e0: 5173 6369 4c65 7865 7243 6f66 6665 6553  QsciLexerCoffeeS
+000084f0: 6372 6970 7401 0300 0000 2600 4a00 6100  cript.....&.J.a.
+00008500: 7600 6100 4400 6f00 6300 2000 4300 2000  v.a.D.o.c. .C. .
+00008510: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00008520: 7208 0000 0000 0600 0000 174a 6176 6144  r..........JavaD
+00008530: 6f63 2043 2d73 7479 6c65 2063 6f6d 6d65  oc C-style comme
+00008540: 6e74 0700 0000 1551 7363 694c 6578 6572  nt.....QsciLexer
+00008550: 436f 6666 6565 5363 7269 7074 0103 0000  CoffeeScript....
+00008560: 002a 004a 0061 0076 0061 0044 006f 0063  .*.J.a.v.a.D.o.c
+00008570: 0020 0053 0063 0068 006c 00fc 0073 0073  . .S.c.h.l...s.s
+00008580: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
+00008590: 0006 0000 000f 4a61 7661 446f 6320 6b65  ......JavaDoc ke
+000085a0: 7977 6f72 6407 0000 0015 5173 6369 4c65  yword.....QsciLe
+000085b0: 7865 7243 6f66 6665 6553 6372 6970 7401  xerCoffeeScript.
+000085c0: 0300 0000 3600 4a00 6100 7600 6100 4400  ....6.J.a.v.a.D.
+000085d0: 6f00 6300 2000 5300 6300 6800 6c00 fc00  o.c. .S.c.h.l...
+000085e0: 7300 7300 6500 6c00 7700 6f00 7200 7400  s.s.e.l.w.o.r.t.
+000085f0: 6600 6500 6800 6c00 6500 7208 0000 0000  f.e.h.l.e.r.....
+00008600: 0600 0000 154a 6176 6144 6f63 206b 6579  .....JavaDoc key
+00008610: 776f 7264 2065 7272 6f72 0700 0000 1551  word error.....Q
+00008620: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
+00008630: 7269 7074 0103 0000 001a 0053 0063 0068  ript.......S.c.h
+00008640: 006c 00fc 0073 0073 0065 006c 0077 006f  .l...s.s.e.l.w.o
+00008650: 0072 0074 0800 0000 0006 0000 0007 4b65  .r.t..........Ke
+00008660: 7977 6f72 6407 0000 0015 5173 6369 4c65  yword.....QsciLe
+00008670: 7865 7243 6f66 6665 6553 6372 6970 7401  xerCoffeeScript.
+00008680: 0300 0000 0800 5a00 6100 6800 6c08 0000  ......Z.a.h.l...
+00008690: 0000 0600 0000 064e 756d 6265 7207 0000  .......Number...
+000086a0: 0015 5173 6369 4c65 7865 7243 6f66 6665  ..QsciLexerCoffe
+000086b0: 6553 6372 6970 7401 0300 0000 1000 4f00  eScript.......O.
+000086c0: 7000 6500 7200 6100 7400 6f00 7208 0000  p.e.r.a.t.o.r...
+000086d0: 0000 0600 0000 084f 7065 7261 746f 7207  .......Operator.
+000086e0: 0000 0015 5173 6369 4c65 7865 7243 6f66  ....QsciLexerCof
+000086f0: 6665 6553 6372 6970 7401 0300 0000 2200  feeScript.....".
+00008700: 5000 7200 e400 7000 7200 6f00 7a00 6500  P.r...p.r.o.z.e.
+00008710: 7300 7300 6f00 7200 6200 6c00 6f00 6300  s.s.o.r.b.l.o.c.
+00008720: 6b08 0000 0000 0600 0000 1350 7265 2d70  k..........Pre-p
+00008730: 726f 6365 7373 6f72 2062 6c6f 636b 0700  rocessor block..
+00008740: 0000 1551 7363 694c 6578 6572 436f 6666  ...QsciLexerCoff
+00008750: 6565 5363 7269 7074 0103 0000 0024 0052  eeScript.....$.R
+00008760: 0065 0067 0075 006c 00e4 0072 0065 0072  .e.g.u.l...r.e.r
+00008770: 0020 0041 0075 0073 0064 0072 0075 0063  . .A.u.s.d.r.u.c
+00008780: 006b 0800 0000 0006 0000 0012 5265 6775  .k..........Regu
+00008790: 6c61 7220 6578 7072 6573 7369 6f6e 0700  lar expression..
+000087a0: 0000 1551 7363 694c 6578 6572 436f 6666  ...QsciLexerCoff
+000087b0: 6565 5363 7269 7074 0103 0000 0050 0053  eeScript.....P.S
+000087c0: 0065 006b 0075 006e 0064 00e4 0072 0065  .e.k.u.n.d...r.e
+000087d0: 0020 0053 0063 0068 006c 0075 0073 0073  . .S.c.h.l.u.s.s
+000087e0: 0065 006c 0077 00f6 0072 0074 0065 0072  .e.l.w...r.t.e.r
+000087f0: 0020 0075 006e 0064 0020 0042 0065 007a  . .u.n.d. .B.e.z
+00008800: 0065 0069 0063 0068 006e 0065 0072 0800  .e.i.c.h.n.e.r..
+00008810: 0000 0006 0000 0022 5365 636f 6e64 6172  ......."Secondar
+00008820: 7920 6b65 7977 6f72 6473 2061 6e64 2069  y keywords and i
+00008830: 6465 6e74 6966 6965 7273 0700 0000 1551  dentifiers.....Q
+00008840: 7363 694c 6578 6572 436f 6666 6565 5363  sciLexerCoffeeSc
+00008850: 7269 7074 0103 0000 0036 005a 0065 0069  ript.....6.Z.e.i
+00008860: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
+00008870: 0065 0020 0069 006e 0020 0048 006f 0063  .e. .i.n. .H.o.c
+00008880: 0068 006b 006f 006d 006d 0061 0074 0061  .h.k.o.m.m.a.t.a
+00008890: 0800 0000 0006 0000 0014 5369 6e67 6c65  ..........Single
+000088a0: 2d71 756f 7465 6420 7374 7269 6e67 0700  -quoted string..
+000088b0: 0000 1551 7363 694c 6578 6572 436f 6666  ...QsciLexerCoff
+000088c0: 6565 5363 7269 7074 0103 0000 002e 0055  eeScript.......U
+000088d0: 006e 0062 0065 0065 006e 0064 0065 0074  .n.b.e.e.n.d.e.t
+000088e0: 0065 0020 005a 0065 0069 0063 0068 0065  .e. .Z.e.i.c.h.e
+000088f0: 006e 006b 0065 0074 0074 0065 0800 0000  .n.k.e.t.t.e....
+00008900: 0006 0000 000f 556e 636c 6f73 6564 2073  ......Unclosed s
+00008910: 7472 696e 6707 0000 0015 5173 6369 4c65  tring.....QsciLe
+00008920: 7865 7243 6f66 6665 6553 6372 6970 7401  xerCoffeeScript.
+00008930: 0300 0000 4200 5a00 6500 6900 6300 6800  ....B.Z.e.i.c.h.
+00008940: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
+00008950: 6900 6e00 2000 5200 fc00 6300 6b00 7700  i.n. .R...c.k.w.
+00008960: e400 7200 7400 7300 7300 7400 7200 6900  ..r.t.s.s.t.r.i.
+00008970: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+00008980: 1142 6163 6b71 756f 7465 6420 7374 7269  .Backquoted stri
+00008990: 6e67 0700 0000 0a51 7363 694c 6578 6572  ng.....QsciLexer
+000089a0: 4401 0300 0000 1c00 4200 6c00 6f00 6300  D.......B.l.o.c.
+000089b0: 6b00 6b00 6f00 6d00 6d00 6500 6e00 7400  k.k.o.m.m.e.n.t.
+000089c0: 6100 7208 0000 0000 0600 0000 0d42 6c6f  a.r..........Blo
+000089d0: 636b 2063 6f6d 6d65 6e74 0700 0000 0a51  ck comment.....Q
+000089e0: 7363 694c 6578 6572 4401 0300 0000 0e00  sciLexerD.......
+000089f0: 5a00 6500 6900 6300 6800 6500 6e08 0000  Z.e.i.c.h.e.n...
+00008a00: 0000 0600 0000 0943 6861 7261 6374 6572  .......Character
+00008a10: 0700 0000 0a51 7363 694c 6578 6572 4401  .....QsciLexerD.
+00008a20: 0300 0000 2400 4400 4400 6f00 6300 2000  ....$.D.D.o.c. .
+00008a30: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
+00008a40: 6c00 7700 6f00 7200 7408 0000 0000 0600  l.w.o.r.t.......
+00008a50: 0000 0c44 446f 6320 6b65 7977 6f72 6407  ...DDoc keyword.
+00008a60: 0000 000a 5173 6369 4c65 7865 7244 0103  ....QsciLexerD..
+00008a70: 0000 0030 0044 0044 006f 0063 0020 0053  ...0.D.D.o.c. .S
+00008a80: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
+00008a90: 0077 006f 0072 0074 0066 0065 0068 006c  .w.o.r.t.f.e.h.l
+00008aa0: 0065 0072 0800 0000 0006 0000 0012 4444  .e.r..........DD
+00008ab0: 6f63 206b 6579 776f 7264 2065 7272 6f72  oc keyword error
+00008ac0: 0700 0000 0a51 7363 694c 6578 6572 4401  .....QsciLexerD.
+00008ad0: 0300 0000 2600 4400 4400 6f00 6300 2000  ....&.D.D.o.c. .
+00008ae0: 4200 6c00 6f00 6300 6b00 6b00 6f00 6d00  B.l.o.c.k.k.o.m.
+00008af0: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+00008b00: 0600 0000 1844 446f 6320 7374 796c 6520  .....DDoc style 
+00008b10: 626c 6f63 6b20 636f 6d6d 656e 7407 0000  block comment...
+00008b20: 000a 5173 6369 4c65 7865 7244 0103 0000  ..QsciLexerD....
+00008b30: 0028 0044 0044 006f 0063 0020 005a 0065  .(.D.D.o.c. .Z.e
+00008b40: 0069 006c 0065 006e 006b 006f 006d 006d  .i.l.e.n.k.o.m.m
+00008b50: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+00008b60: 0000 0017 4444 6f63 2073 7479 6c65 206c  ....DDoc style l
+00008b70: 696e 6520 636f 6d6d 656e 7407 0000 000a  ine comment.....
+00008b80: 5173 6369 4c65 7865 7244 0103 0000 0010  QsciLexerD......
+00008b90: 0053 0074 0061 006e 0064 0061 0072 0064  .S.t.a.n.d.a.r.d
+00008ba0: 0800 0000 0006 0000 0007 4465 6661 756c  ..........Defaul
+00008bb0: 7407 0000 000a 5173 6369 4c65 7865 7244  t.....QsciLexerD
+00008bc0: 0103 0000 0036 0044 006f 006b 0075 006d  .....6.D.o.k.u.m
+00008bd0: 0065 006e 0074 0061 0074 0069 006f 006e  .e.n.t.a.t.i.o.n
+00008be0: 0073 0073 0063 0068 006c 00fc 0073 0073  .s.s.c.h.l...s.s
+00008bf0: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
+00008c00: 0006 0000 0015 446f 6375 6d65 6e74 6174  ......Documentat
+00008c10: 696f 6e20 6b65 7977 6f72 6407 0000 000a  ion keyword.....
+00008c20: 5173 6369 4c65 7865 7244 0103 0000 0014  QsciLexerD......
+00008c30: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
+00008c40: 0065 0072 0800 0000 0006 0000 000a 4964  .e.r..........Id
+00008c50: 656e 7469 6669 6572 0700 0000 0a51 7363  entifier.....Qsc
+00008c60: 694c 6578 6572 4401 0300 0000 1a00 5300  iLexerD.......S.
+00008c70: 6300 6800 6c00 fc00 7300 7300 6500 6c00  c.h.l...s.s.e.l.
+00008c80: 7700 6f00 7200 7408 0000 0000 0600 0000  w.o.r.t.........
+00008c90: 074b 6579 776f 7264 0700 0000 0a51 7363  .Keyword.....Qsc
+00008ca0: 694c 6578 6572 4401 0300 0000 1e00 5a00  iLexerD.......Z.
+00008cb0: 6500 6900 6c00 6500 6e00 6b00 6f00 6d00  e.i.l.e.n.k.o.m.
+00008cc0: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+00008cd0: 0600 0000 0c4c 696e 6520 636f 6d6d 656e  .....Line commen
+00008ce0: 7407 0000 000a 5173 6369 4c65 7865 7244  t.....QsciLexerD
+00008cf0: 0103 0000 0030 0073 0063 0068 0061 0063  .....0.s.c.h.a.c
+00008d00: 0068 0074 0065 006c 0062 0061 0072 0065  .h.t.e.l.b.a.r.e
+00008d10: 0072 0020 004b 006f 006d 006d 0065 006e  .r. .K.o.m.m.e.n
+00008d20: 0074 0061 0072 0800 0000 0006 0000 000f  .t.a.r..........
+00008d30: 4e65 7374 696e 6720 636f 6d6d 656e 7407  Nesting comment.
+00008d40: 0000 000a 5173 6369 4c65 7865 7244 0103  ....QsciLexerD..
+00008d50: 0000 0008 005a 0061 0068 006c 0800 0000  .....Z.a.h.l....
+00008d60: 0006 0000 0006 4e75 6d62 6572 0700 0000  ......Number....
+00008d70: 0a51 7363 694c 6578 6572 4401 0300 0000  .QsciLexerD.....
+00008d80: 1000 4f00 7000 6500 7200 6100 7400 6f00  ..O.p.e.r.a.t.o.
+00008d90: 7208 0000 0000 0600 0000 084f 7065 7261  r..........Opera
+00008da0: 746f 7207 0000 000a 5173 6369 4c65 7865  tor.....QsciLexe
+00008db0: 7244 0103 0000 0022 0052 006f 0068 0065  rD.....".R.o.h.e
+00008dc0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
+00008dd0: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
+00008de0: 0000 000a 5261 7720 7374 7269 6e67 0700  ....Raw string..
+00008df0: 0000 0a51 7363 694c 6578 6572 4401 0300  ...QsciLexerD...
+00008e00: 0000 3000 5300 6500 6b00 7500 6e00 6400  ..0.S.e.k.u.n.d.
+00008e10: e400 7200 6500 7300 2000 5300 6300 6800  ..r.e.s. .S.c.h.
+00008e20: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
+00008e30: 7200 7408 0000 0000 0600 0000 1153 6563  r.t..........Sec
+00008e40: 6f6e 6461 7279 206b 6579 776f 7264 0700  ondary keyword..
+00008e50: 0000 0a51 7363 694c 6578 6572 4401 0300  ...QsciLexerD...
+00008e60: 0000 1800 5a00 6500 6900 6300 6800 6500  ....Z.e.i.c.h.e.
+00008e70: 6e00 6b00 6500 7400 7400 6508 0000 0000  n.k.e.t.t.e.....
+00008e80: 0600 0000 0653 7472 696e 6707 0000 000a  .....String.....
+00008e90: 5173 6369 4c65 7865 7244 0103 0000 001a  QsciLexerD......
+00008ea0: 0054 0079 0070 0064 0065 0066 0069 006e  .T.y.p.d.e.f.i.n
+00008eb0: 0069 0074 0069 006f 006e 0800 0000 0006  .i.t.i.o.n......
+00008ec0: 0000 000f 5479 7065 2064 6566 696e 6974  ....Type definit
+00008ed0: 696f 6e07 0000 000a 5173 6369 4c65 7865  ion.....QsciLexe
+00008ee0: 7244 0103 0000 002e 0055 006e 0062 0065  rD.......U.n.b.e
+00008ef0: 0065 006e 0064 0065 0074 0065 0020 005a  .e.n.d.e.t.e. .Z
+00008f00: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
+00008f10: 0074 0074 0065 0800 0000 0006 0000 000f  .t.t.e..........
+00008f20: 556e 636c 6f73 6564 2073 7472 696e 6707  Unclosed string.
+00008f30: 0000 000a 5173 6369 4c65 7865 7244 0103  ....QsciLexerD..
+00008f40: 0000 0024 004e 0075 0074 007a 0065 0072  ...$.N.u.t.z.e.r
+00008f50: 0020 0064 0065 0066 0069 006e 0069 0065  . .d.e.f.i.n.i.e
+00008f60: 0072 0074 0020 0031 0800 0000 0006 0000  .r.t. .1........
+00008f70: 000e 5573 6572 2064 6566 696e 6564 2031  ..User defined 1
+00008f80: 0700 0000 0a51 7363 694c 6578 6572 4401  .....QsciLexerD.
+00008f90: 0300 0000 2400 4e00 7500 7400 7a00 6500  ....$.N.u.t.z.e.
+00008fa0: 7200 2000 6400 6500 6600 6900 6e00 6900  r. .d.e.f.i.n.i.
+00008fb0: 6500 7200 7400 2000 3208 0000 0000 0600  e.r.t. .2.......
+00008fc0: 0000 0e55 7365 7220 6465 6669 6e65 6420  ...User defined 
+00008fd0: 3207 0000 000a 5173 6369 4c65 7865 7244  2.....QsciLexerD
+00008fe0: 0103 0000 0024 004e 0075 0074 007a 0065  .....$.N.u.t.z.e
+00008ff0: 0072 0020 0064 0065 0066 0069 006e 0069  .r. .d.e.f.i.n.i
+00009000: 0065 0072 0074 0020 0033 0800 0000 0006  .e.r.t. .3......
+00009010: 0000 000e 5573 6572 2064 6566 696e 6564  ....User defined
+00009020: 2033 0700 0000 0a51 7363 694c 6578 6572   3.....QsciLexer
+00009030: 4401 0300 0000 3a00 4800 6900 6e00 7a00  D.....:.H.i.n.z.
+00009040: 7500 6700 6500 6600 fc00 6700 7400 6500  u.g.e.f...g.t.e.
+00009050: 7200 2000 4500 7200 6700 e400 6e00 7a00  r. .E.r.g...n.z.
+00009060: 7500 6e00 6700 7300 7000 6100 7400 6300  u.n.g.s.p.a.t.c.
+00009070: 6808 0000 0000 0600 0000 1241 6464 6564  h..........Added
+00009080: 2061 6464 696e 6720 7061 7463 6807 0000   adding patch...
+00009090: 000d 5173 6369 4c65 7865 7244 6966 6601  ..QsciLexerDiff.
+000090a0: 0300 0000 2400 4800 6900 6e00 7a00 7500  ....$.H.i.n.z.u.
+000090b0: 6700 6500 6600 fc00 6700 7400 6500 2000  g.e.f...g.t.e. .
+000090c0: 5a00 6500 6900 6c00 6508 0000 0000 0600  Z.e.i.l.e.......
+000090d0: 0000 0a41 6464 6564 206c 696e 6507 0000  ...Added line...
+000090e0: 000d 5173 6369 4c65 7865 7244 6966 6601  ..QsciLexerDiff.
+000090f0: 0300 0000 3c00 4800 6900 6e00 7a00 7500  ....<.H.i.n.z.u.
+00009100: 6700 6500 6600 fc00 6700 7400 6500 7200  g.e.f...g.t.e.r.
+00009110: 2000 4500 6e00 7400 6600 6500 7200 6e00   .E.n.t.f.e.r.n.
+00009120: 7500 6e00 6700 7300 7000 6100 7400 6300  u.n.g.s.p.a.t.c.
+00009130: 6808 0000 0000 0600 0000 1441 6464 6564  h..........Added
+00009140: 2072 656d 6f76 696e 6720 7061 7463 6807   removing patch.
+00009150: 0000 000d 5173 6369 4c65 7865 7244 6966  ....QsciLexerDif
+00009160: 6601 0300 0000 1e00 4700 6500 e400 6e00  f.......G.e...n.
+00009170: 6400 6500 7200 7400 6500 2000 5a00 6500  d.e.r.t.e. .Z.e.
+00009180: 6900 6c00 6508 0000 0000 0600 0000 0c43  i.l.e..........C
+00009190: 6861 6e67 6564 206c 696e 6507 0000 000d  hanged line.....
+000091a0: 5173 6369 4c65 7865 7244 6966 6601 0300  QsciLexerDiff...
+000091b0: 0000 0c00 4200 6500 6600 6500 6800 6c08  ....B.e.f.e.h.l.
+000091c0: 0000 0000 0600 0000 0743 6f6d 6d61 6e64  .........Command
+000091d0: 0700 0000 0d51 7363 694c 6578 6572 4469  .....QsciLexerDi
+000091e0: 6666 0103 0000 0012 004b 006f 006d 006d  ff.......K.o.m.m
+000091f0: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+00009200: 0000 0007 436f 6d6d 656e 7407 0000 000d  ....Comment.....
+00009210: 5173 6369 4c65 7865 7244 6966 6601 0300  QsciLexerDiff...
+00009220: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
+00009230: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
+00009240: 6175 6c74 0700 0000 0d51 7363 694c 6578  ault.....QsciLex
+00009250: 6572 4469 6666 0103 0000 0014 004b 006f  erDiff.......K.o
+00009260: 0070 0066 007a 0065 0069 006c 0065 006e  .p.f.z.e.i.l.e.n
+00009270: 0800 0000 0006 0000 0006 4865 6164 6572  ..........Header
+00009280: 0700 0000 0d51 7363 694c 6578 6572 4469  .....QsciLexerDi
+00009290: 6666 0103 0000 0010 0050 006f 0073 0069  ff.......P.o.s.i
+000092a0: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
+000092b0: 0008 506f 7369 7469 6f6e 0700 0000 0d51  ..Position.....Q
+000092c0: 7363 694c 6578 6572 4469 6666 0103 0000  sciLexerDiff....
+000092d0: 0034 0045 006e 0074 0066 0065 0072 006e  .4.E.n.t.f.e.r.n
+000092e0: 0074 0065 0072 0020 0045 0072 0067 00e4  .t.e.r. .E.r.g..
+000092f0: 006e 007a 0075 006e 0067 0073 0070 0061  .n.z.u.n.g.s.p.a
+00009300: 0074 0063 0068 0800 0000 0006 0000 0014  .t.c.h..........
+00009310: 5265 6d6f 7665 6420 6164 6469 6e67 2070  Removed adding p
+00009320: 6174 6368 0700 0000 0d51 7363 694c 6578  atch.....QsciLex
+00009330: 6572 4469 6666 0103 0000 001e 0045 006e  erDiff.......E.n
+00009340: 0074 0066 0065 0072 006e 0074 0065 0020  .t.f.e.r.n.t.e. 
+00009350: 005a 0065 0069 006c 0065 0800 0000 0006  .Z.e.i.l.e......
+00009360: 0000 000c 5265 6d6f 7665 6420 6c69 6e65  ....Removed line
+00009370: 0700 0000 0d51 7363 694c 6578 6572 4469  .....QsciLexerDi
+00009380: 6666 0103 0000 0036 0045 006e 0074 0066  ff.....6.E.n.t.f
+00009390: 0065 0072 006e 0074 0065 0072 0020 0045  .e.r.n.t.e.r. .E
+000093a0: 006e 0074 0066 0065 0072 006e 0075 006e  .n.t.f.e.r.n.u.n
+000093b0: 0067 0073 0070 0061 0074 0063 0068 0800  .g.s.p.a.t.c.h..
+000093c0: 0000 0006 0000 0016 5265 6d6f 7665 6420  ........Removed 
+000093d0: 7265 6d6f 7669 6e67 2070 6174 6368 0700  removing patch..
+000093e0: 0000 0d51 7363 694c 6578 6572 4469 6666  ...QsciLexerDiff
+000093f0: 0103 0000 0034 0053 0063 0068 006c 0065  .....4.S.c.h.l.e
+00009400: 0063 0068 0074 0020 0067 0065 0066 006f  .c.h.t. .g.e.f.o
+00009410: 0072 006d 0074 0065 0073 0020 0053 0065  .r.m.t.e.s. .S.e
+00009420: 0067 006d 0065 006e 0074 0800 0000 0006  .g.m.e.n.t......
+00009430: 0000 0014 4261 646c 7920 666f 726d 6564  ....Badly formed
+00009440: 2073 6567 6d65 6e74 0700 0000 1051 7363   segment.....Qsc
+00009450: 694c 6578 6572 4544 4946 4143 5401 0300  iLexerEDIFACT...
+00009460: 0000 3200 5a00 7500 7300 6100 6d00 6d00  ..2.Z.u.s.a.m.m.
+00009470: 6500 6e00 6700 6500 7300 6500 7400 7a00  e.n.g.e.s.e.t.z.
+00009480: 7400 6500 7200 2000 5400 7200 6500 6e00  t.e.r. .T.r.e.n.
+00009490: 6e00 6500 7208 0000 0000 0600 0000 1343  n.e.r..........C
+000094a0: 6f6d 706f 7369 7465 2073 6570 6172 6174  omposite separat
+000094b0: 6f72 0700 0000 1051 7363 694c 6578 6572  or.....QsciLexer
+000094c0: 4544 4946 4143 5401 0300 0000 1000 5300  EDIFACT.......S.
+000094d0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
+000094e0: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
+000094f0: 0000 1051 7363 694c 6578 6572 4544 4946  ...QsciLexerEDIF
+00009500: 4143 5401 0300 0000 1c00 4500 6c00 6500  ACT.......E.l.e.
+00009510: 6d00 6500 6e00 7400 7400 7200 6500 6e00  m.e.n.t.t.r.e.n.
+00009520: 6e00 6500 7208 0000 0000 0600 0000 1145  n.e.r..........E
+00009530: 6c65 6d65 6e74 2073 6570 6172 6174 6f72  lement separator
+00009540: 0700 0000 1051 7363 694c 6578 6572 4544  .....QsciLexerED
+00009550: 4946 4143 5401 0300 0000 1e00 4600 7200  IFACT.......F.r.
+00009560: 6500 6900 6700 6100 6200 6500 7400 7200  e.i.g.a.b.e.t.r.
+00009570: 6500 6e00 6e00 6500 7208 0000 0000 0600  e.n.n.e.r.......
+00009580: 0000 1152 656c 6561 7365 2073 6570 6172  ...Release separ
+00009590: 6174 6f72 0700 0000 1051 7363 694c 6578  ator.....QsciLex
+000095a0: 6572 4544 4946 4143 5401 0300 0000 1600  erEDIFACT.......
+000095b0: 5300 6500 6700 6d00 6500 6e00 7400 6500  S.e.g.m.e.n.t.e.
+000095c0: 6e00 6400 6508 0000 0000 0600 0000 0b53  n.d.e..........S
+000095d0: 6567 6d65 6e74 2065 6e64 0700 0000 1051  egment end.....Q
+000095e0: 7363 694c 6578 6572 4544 4946 4143 5401  sciLexerEDIFACT.
+000095f0: 0300 0000 1800 5300 6500 6700 6d00 6500  ......S.e.g.m.e.
+00009600: 6e00 7400 7300 7400 6100 7200 7408 0000  n.t.s.t.a.r.t...
+00009610: 0000 0600 0000 0d53 6567 6d65 6e74 2073  .......Segment s
+00009620: 7461 7274 0700 0000 1051 7363 694c 6578  tart.....QsciLex
+00009630: 6572 4544 4946 4143 5401 0300 0000 1e00  erEDIFACT.......
+00009640: 5500 4e00 4100 2000 5300 6500 6700 6d00  U.N.A. .S.e.g.m.
+00009650: 6500 6e00 7400 6b00 6f00 7000 6608 0000  e.n.t.k.o.p.f...
+00009660: 0000 0600 0000 1255 4e41 2073 6567 6d65  .......UNA segme
+00009670: 6e74 2068 6561 6465 7207 0000 0010 5173  nt header.....Qs
+00009680: 6369 4c65 7865 7245 4449 4641 4354 0103  ciLexerEDIFACT..
+00009690: 0000 001e 0055 004e 0048 0020 0053 0065  .....U.N.H. .S.e
+000096a0: 0067 006d 0065 006e 0074 006b 006f 0070  .g.m.e.n.t.k.o.p
+000096b0: 0066 0800 0000 0006 0000 0012 554e 4820  .f..........UNH 
+000096c0: 7365 676d 656e 7420 6865 6164 6572 0700  segment header..
+000096d0: 0000 1051 7363 694c 6578 6572 4544 4946  ...QsciLexerEDIF
+000096e0: 4143 5401 0300 0000 1200 4b00 6f00 6d00  ACT.......K.o.m.
+000096f0: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+00009700: 0600 0000 0743 6f6d 6d65 6e74 0700 0000  .....Comment....
+00009710: 1251 7363 694c 6578 6572 466f 7274 7261  .QsciLexerFortra
+00009720: 6e37 3701 0300 0000 1600 4600 6f00 7200  n77.......F.o.r.
+00009730: 7400 7300 6500 7400 7a00 7500 6e00 6708  t.s.e.t.z.u.n.g.
+00009740: 0000 0000 0600 0000 0c43 6f6e 7469 6e75  .........Continu
+00009750: 6174 696f 6e07 0000 0012 5173 6369 4c65  ation.....QsciLe
+00009760: 7865 7246 6f72 7472 616e 3737 0103 0000  xerFortran77....
+00009770: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
+00009780: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
+00009790: 756c 7407 0000 0012 5173 6369 4c65 7865  ult.....QsciLexe
+000097a0: 7246 6f72 7472 616e 3737 0103 0000 001e  rFortran77......
+000097b0: 0044 006f 0074 0074 0065 0064 0020 004f  .D.o.t.t.e.d. .O
+000097c0: 0070 0065 0072 0061 0074 006f 0072 0800  .p.e.r.a.t.o.r..
+000097d0: 0000 0006 0000 000f 446f 7474 6564 206f  ........Dotted o
+000097e0: 7065 7261 746f 7207 0000 0012 5173 6369  perator.....Qsci
+000097f0: 4c65 7865 7246 6f72 7472 616e 3737 0103  LexerFortran77..
+00009800: 0000 0042 005a 0065 0069 0063 0068 0065  ...B.Z.e.i.c.h.e
+00009810: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
+00009820: 006e 0020 0041 006e 0066 00fc 0068 0072  .n. .A.n.f...h.r
+00009830: 0075 006e 0067 0073 007a 0065 0069 0063  .u.n.g.s.z.e.i.c
+00009840: 0068 0065 006e 0800 0000 0006 0000 0014  .h.e.n..........
+00009850: 446f 7562 6c65 2d71 756f 7465 6420 7374  Double-quoted st
+00009860: 7269 6e67 0700 0000 1251 7363 694c 6578  ring.....QsciLex
+00009870: 6572 466f 7274 7261 6e37 3701 0300 0000  erFortran77.....
+00009880: 2600 4500 7200 7700 6500 6900 7400 6500  &.E.r.w.e.i.t.e.
+00009890: 7200 7400 6500 2000 4600 7500 6e00 6b00  r.t.e. .F.u.n.k.
+000098a0: 7400 6900 6f00 6e08 0000 0000 0600 0000  t.i.o.n.........
+000098b0: 1145 7874 656e 6465 6420 6675 6e63 7469  .Extended functi
+000098c0: 6f6e 0700 0000 1251 7363 694c 6578 6572  on.....QsciLexer
+000098d0: 466f 7274 7261 6e37 3701 0300 0000 1400  Fortran77.......
+000098e0: 4200 6500 7a00 6500 6900 6300 6800 6e00  B.e.z.e.i.c.h.n.
+000098f0: 6500 7208 0000 0000 0600 0000 0a49 6465  e.r..........Ide
+00009900: 6e74 6966 6965 7207 0000 0012 5173 6369  ntifier.....Qsci
+00009910: 4c65 7865 7246 6f72 7472 616e 3737 0103  LexerFortran77..
+00009920: 0000 0024 0049 006e 0074 0072 0069 006e  ...$.I.n.t.r.i.n
+00009930: 0073 0069 0063 002d 0046 0075 006e 006b  .s.i.c.-.F.u.n.k
+00009940: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
+00009950: 0012 496e 7472 696e 7369 6320 6675 6e63  ..Intrinsic func
+00009960: 7469 6f6e 0700 0000 1251 7363 694c 6578  tion.....QsciLex
+00009970: 6572 466f 7274 7261 6e37 3701 0300 0000  erFortran77.....
+00009980: 1a00 5300 6300 6800 6c00 fc00 7300 7300  ..S.c.h.l...s.s.
+00009990: 6500 6c00 7700 6f00 7200 7408 0000 0000  e.l.w.o.r.t.....
+000099a0: 0600 0000 074b 6579 776f 7264 0700 0000  .....Keyword....
+000099b0: 1251 7363 694c 6578 6572 466f 7274 7261  .QsciLexerFortra
+000099c0: 6e37 3701 0300 0000 0a00 4d00 6100 7200  n77.......M.a.r.
+000099d0: 6b00 6508 0000 0000 0600 0000 054c 6162  k.e..........Lab
+000099e0: 656c 0700 0000 1251 7363 694c 6578 6572  el.....QsciLexer
+000099f0: 466f 7274 7261 6e37 3701 0300 0000 0800  Fortran77.......
+00009a00: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
+00009a10: 064e 756d 6265 7207 0000 0012 5173 6369  .Number.....Qsci
+00009a20: 4c65 7865 7246 6f72 7472 616e 3737 0103  LexerFortran77..
+00009a30: 0000 0010 004f 0070 0065 0072 0061 0074  .....O.p.e.r.a.t
+00009a40: 006f 0072 0800 0000 0006 0000 0008 4f70  .o.r..........Op
+00009a50: 6572 6174 6f72 0700 0000 1251 7363 694c  erator.....QsciL
+00009a60: 6578 6572 466f 7274 7261 6e37 3701 0300  exerFortran77...
+00009a70: 0000 2200 5000 7200 e400 7000 7200 6f00  ..".P.r...p.r.o.
+00009a80: 7a00 6500 7300 7300 6f00 7200 6200 6c00  z.e.s.s.o.r.b.l.
+00009a90: 6f00 6300 6b08 0000 0000 0600 0000 1350  o.c.k..........P
+00009aa0: 7265 2d70 726f 6365 7373 6f72 2062 6c6f  re-processor blo
+00009ab0: 636b 0700 0000 1251 7363 694c 6578 6572  ck.....QsciLexer
+00009ac0: 466f 7274 7261 6e37 3701 0300 0000 3600  Fortran77.....6.
+00009ad0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+00009ae0: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
+00009af0: 4800 6f00 6300 6800 6b00 6f00 6d00 6d00  H.o.c.h.k.o.m.m.
+00009b00: 6100 7400 6108 0000 0000 0600 0000 1453  a.t.a..........S
+00009b10: 696e 676c 652d 7175 6f74 6564 2073 7472  ingle-quoted str
+00009b20: 696e 6707 0000 0012 5173 6369 4c65 7865  ing.....QsciLexe
+00009b30: 7246 6f72 7472 616e 3737 0103 0000 002e  rFortran77......
+00009b40: 0055 006e 0062 0065 0065 006e 0064 0065  .U.n.b.e.e.n.d.e
+00009b50: 0074 0065 0020 005a 0065 0069 0063 0068  .t.e. .Z.e.i.c.h
+00009b60: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
+00009b70: 0000 0006 0000 000f 556e 636c 6f73 6564  ........Unclosed
+00009b80: 2073 7472 696e 6707 0000 0012 5173 6369   string.....Qsci
+00009b90: 4c65 7865 7246 6f72 7472 616e 3737 0103  LexerFortran77..
+00009ba0: 0000 0030 0041 0053 0050 0020 004a 0061  ...0.A.S.P. .J.a
+00009bb0: 0076 0061 0053 0063 0072 0069 0070 0074  .v.a.S.c.r.i.p.t
+00009bc0: 0020 004b 006f 006d 006d 0065 006e 0074  . .K.o.m.m.e.n.t
+00009bd0: 0061 0072 0800 0000 0006 0000 0016 4153  .a.r..........AS
+00009be0: 5020 4a61 7661 5363 7269 7074 2063 6f6d  P JavaScript com
+00009bf0: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
+00009c00: 6572 4854 4d4c 0103 0000 002e 0041 0053  erHTML.......A.S
+00009c10: 0050 0020 004a 0061 0076 0061 0053 0063  .P. .J.a.v.a.S.c
+00009c20: 0072 0069 0070 0074 0020 0053 0074 0061  .r.i.p.t. .S.t.a
+00009c30: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
+00009c40: 0000 0016 4153 5020 4a61 7661 5363 7269  ....ASP JavaScri
+00009c50: 7074 2064 6566 6175 6c74 0700 0000 0d51  pt default.....Q
+00009c60: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+00009c70: 0060 0041 0053 0050 0020 004a 0061 0076  .`.A.S.P. .J.a.v
+00009c80: 0061 0053 0063 0072 0069 0070 0074 0020  .a.S.c.r.i.p.t. 
+00009c90: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+00009ca0: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
+00009cb0: 0041 006e 0066 00fc 0068 0072 0075 006e  .A.n.f...h.r.u.n
+00009cc0: 0067 0073 007a 0065 0069 0063 0068 0065  .g.s.z.e.i.c.h.e
+00009cd0: 006e 0800 0000 0006 0000 0023 4153 5020  .n.........#ASP 
+00009ce0: 4a61 7661 5363 7269 7074 2064 6f75 626c  JavaScript doubl
+00009cf0: 652d 7175 6f74 6564 2073 7472 696e 6707  e-quoted string.
+00009d00: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+00009d10: 4c01 0300 0000 3800 4100 5300 5000 2000  L.....8.A.S.P. .
+00009d20: 4a00 6100 7600 6100 5300 6300 7200 6900  J.a.v.a.S.c.r.i.
+00009d30: 7000 7400 2000 5300 6300 6800 6c00 fc00  p.t. .S.c.h.l...
+00009d40: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
+00009d50: 0000 0000 0600 0000 1641 5350 204a 6176  .........ASP Jav
+00009d60: 6153 6372 6970 7420 6b65 7977 6f72 6407  aScript keyword.
+00009d70: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+00009d80: 4c01 0300 0000 3c00 4100 5300 5000 2000  L.....<.A.S.P. .
+00009d90: 4a00 6100 7600 6100 5300 6300 7200 6900  J.a.v.a.S.c.r.i.
+00009da0: 7000 7400 2000 5a00 6500 6900 6c00 6500  p.t. .Z.e.i.l.e.
+00009db0: 6e00 6b00 6f00 6d00 6d00 6500 6e00 7400  n.k.o.m.m.e.n.t.
+00009dc0: 6100 7208 0000 0000 0600 0000 1b41 5350  a.r..........ASP
+00009dd0: 204a 6176 6153 6372 6970 7420 6c69 6e65   JavaScript line
+00009de0: 2063 6f6d 6d65 6e74 0700 0000 0d51 7363   comment.....Qsc
+00009df0: 694c 6578 6572 4854 4d4c 0103 0000 0026  iLexerHTML.....&
+00009e00: 0041 0053 0050 0020 004a 0061 0076 0061  .A.S.P. .J.a.v.a
+00009e10: 0053 0063 0072 0069 0070 0074 0020 005a  .S.c.r.i.p.t. .Z
+00009e20: 0061 0068 006c 0800 0000 0006 0000 0015  .a.h.l..........
+00009e30: 4153 5020 4a61 7661 5363 7269 7074 206e  ASP JavaScript n
+00009e40: 756d 6265 7207 0000 000d 5173 6369 4c65  umber.....QsciLe
+00009e50: 7865 7248 544d 4c01 0300 0000 4200 4100  xerHTML.....B.A.
+00009e60: 5300 5000 2000 4a00 6100 7600 6100 5300  S.P. .J.a.v.a.S.
+00009e70: 6300 7200 6900 7000 7400 2000 5200 6500  c.r.i.p.t. .R.e.
+00009e80: 6700 7500 6c00 e400 7200 6500 7200 2000  g.u.l...r.e.r. .
+00009e90: 4100 7500 7300 6400 7200 7500 6300 6b08  A.u.s.d.r.u.c.k.
+00009ea0: 0000 0000 0600 0000 2141 5350 204a 6176  ........!ASP Jav
+00009eb0: 6153 6372 6970 7420 7265 6775 6c61 7220  aScript regular 
+00009ec0: 6578 7072 6573 7369 6f6e 0700 0000 0d51  expression.....Q
+00009ed0: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+00009ee0: 0054 0041 0053 0050 0020 004a 0061 0076  .T.A.S.P. .J.a.v
+00009ef0: 0061 0053 0063 0072 0069 0070 0074 0020  .a.S.c.r.i.p.t. 
+00009f00: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+00009f10: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
+00009f20: 0048 006f 0063 0068 006b 006f 006d 006d  .H.o.c.h.k.o.m.m
+00009f30: 0061 0074 0061 0800 0000 0006 0000 0023  .a.t.a.........#
+00009f40: 4153 5020 4a61 7661 5363 7269 7074 2073  ASP JavaScript s
+00009f50: 696e 676c 652d 7175 6f74 6564 2073 7472  ingle-quoted str
+00009f60: 696e 6707 0000 000d 5173 6369 4c65 7865  ing.....QsciLexe
+00009f70: 7248 544d 4c01 0300 0000 2a00 4100 5300  rHTML.....*.A.S.
+00009f80: 5000 2000 4a00 6100 7600 6100 5300 6300  P. .J.a.v.a.S.c.
+00009f90: 7200 6900 7000 7400 2000 5300 7900 6d00  r.i.p.t. .S.y.m.
+00009fa0: 6200 6f00 6c08 0000 0000 0600 0000 1541  b.o.l..........A
+00009fb0: 5350 204a 6176 6153 6372 6970 7420 7379  SP JavaScript sy
+00009fc0: 6d62 6f6c 0700 0000 0d51 7363 694c 6578  mbol.....QsciLex
+00009fd0: 6572 4854 4d4c 0103 0000 004c 0041 0053  erHTML.....L.A.S
+00009fe0: 0050 0020 004a 0061 0076 0061 0053 0063  .P. .J.a.v.a.S.c
+00009ff0: 0072 0069 0070 0074 0020 0055 006e 0062  .r.i.p.t. .U.n.b
+0000a000: 0065 0065 006e 0064 0065 0074 0065 0020  .e.e.n.d.e.t.e. 
+0000a010: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+0000a020: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
+0000a030: 001e 4153 5020 4a61 7661 5363 7269 7074  ..ASP JavaScript
+0000a040: 2075 6e63 6c6f 7365 6420 7374 7269 6e67   unclosed string
+0000a050: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000a060: 4d4c 0103 0000 0026 0041 0053 0050 0020  ML.....&.A.S.P. 
+0000a070: 004a 0061 0076 0061 0053 0063 0072 0069  .J.a.v.a.S.c.r.i
+0000a080: 0070 0074 0020 0057 006f 0072 0074 0800  .p.t. .W.o.r.t..
+0000a090: 0000 0006 0000 0013 4153 5020 4a61 7661  ........ASP Java
+0000a0a0: 5363 7269 7074 2077 6f72 6407 0000 000d  Script word.....
+0000a0b0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000a0c0: 0000 2c00 4100 5300 5000 2000 5000 7900  ..,.A.S.P. .P.y.
+0000a0d0: 7400 6800 6f00 6e00 2000 4b00 6c00 6100  t.h.o.n. .K.l.a.
+0000a0e0: 7300 7300 6500 6e00 6e00 6100 6d00 6508  s.s.e.n.n.a.m.e.
+0000a0f0: 0000 0000 0600 0000 1541 5350 2050 7974  .........ASP Pyt
+0000a100: 686f 6e20 636c 6173 7320 6e61 6d65 0700  hon class name..
+0000a110: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000a120: 0103 0000 0028 0041 0053 0050 0020 0050  .....(.A.S.P. .P
+0000a130: 0079 0074 0068 006f 006e 0020 004b 006f  .y.t.h.o.n. .K.o
+0000a140: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+0000a150: 0000 0006 0000 0012 4153 5020 5079 7468  ........ASP Pyth
+0000a160: 6f6e 2063 6f6d 6d65 6e74 0700 0000 0d51  on comment.....Q
+0000a170: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+0000a180: 0026 0041 0053 0050 0020 0050 0079 0074  .&.A.S.P. .P.y.t
+0000a190: 0068 006f 006e 0020 0053 0074 0061 006e  .h.o.n. .S.t.a.n
+0000a1a0: 0064 0061 0072 0064 0800 0000 0006 0000  .d.a.r.d........
+0000a1b0: 0012 4153 5020 5079 7468 6f6e 2064 6566  ..ASP Python def
+0000a1c0: 6175 6c74 0700 0000 0d51 7363 694c 6578  ault.....QsciLex
+0000a1d0: 6572 4854 4d4c 0103 0000 0058 0041 0053  erHTML.....X.A.S
+0000a1e0: 0050 0020 0050 0079 0074 0068 006f 006e  .P. .P.y.t.h.o.n
+0000a1f0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
+0000a200: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
+0000a210: 0020 0041 006e 0066 00fc 0068 0072 0075  . .A.n.f...h.r.u
+0000a220: 006e 0067 0073 007a 0065 0069 0063 0068  .n.g.s.z.e.i.c.h
+0000a230: 0065 006e 0800 0000 0006 0000 001f 4153  .e.n..........AS
+0000a240: 5020 5079 7468 6f6e 2064 6f75 626c 652d  P Python double-
+0000a250: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
+0000a260: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
+0000a270: 0300 0000 4e00 4100 5300 5000 2000 5000  ....N.A.S.P. .P.
+0000a280: 7900 7400 6800 6f00 6e00 2000 4600 7500  y.t.h.o.n. .F.u.
+0000a290: 6e00 6b00 7400 6900 6f00 6e00 7300 2d00  n.k.t.i.o.n.s.-.
+0000a2a0: 2000 6f00 6400 6500 7200 2000 4d00 6500   .o.d.e.r. .M.e.
+0000a2b0: 7400 6800 6f00 6400 6500 6e00 6e00 6100  t.h.o.d.e.n.n.a.
+0000a2c0: 6d00 6508 0000 0000 0600 0000 2241 5350  m.e........."ASP
+0000a2d0: 2050 7974 686f 6e20 6675 6e63 7469 6f6e   Python function
+0000a2e0: 206f 7220 6d65 7468 6f64 206e 616d 6507   or method name.
+0000a2f0: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+0000a300: 4c01 0300 0000 2a00 4100 5300 5000 2000  L.....*.A.S.P. .
+0000a310: 5000 7900 7400 6800 6f00 6e00 2000 4200  P.y.t.h.o.n. .B.
+0000a320: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
+0000a330: 7208 0000 0000 0600 0000 1541 5350 2050  r..........ASP P
+0000a340: 7974 686f 6e20 6964 656e 7469 6669 6572  ython identifier
+0000a350: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000a360: 4d4c 0103 0000 0030 0041 0053 0050 0020  ML.....0.A.S.P. 
+0000a370: 0050 0079 0074 0068 006f 006e 0020 0053  .P.y.t.h.o.n. .S
+0000a380: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
+0000a390: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
+0000a3a0: 0012 4153 5020 5079 7468 6f6e 206b 6579  ..ASP Python key
+0000a3b0: 776f 7264 0700 0000 0d51 7363 694c 6578  word.....QsciLex
+0000a3c0: 6572 4854 4d4c 0103 0000 001e 0041 0053  erHTML.......A.S
+0000a3d0: 0050 0020 0050 0079 0074 0068 006f 006e  .P. .P.y.t.h.o.n
+0000a3e0: 0020 005a 0061 0068 006c 0800 0000 0006  . .Z.a.h.l......
+0000a3f0: 0000 0011 4153 5020 5079 7468 6f6e 206e  ....ASP Python n
+0000a400: 756d 6265 7207 0000 000d 5173 6369 4c65  umber.....QsciLe
+0000a410: 7865 7248 544d 4c01 0300 0000 2600 4100  xerHTML.....&.A.
+0000a420: 5300 5000 2000 5000 7900 7400 6800 6f00  S.P. .P.y.t.h.o.
+0000a430: 6e00 2000 4f00 7000 6500 7200 6100 7400  n. .O.p.e.r.a.t.
+0000a440: 6f00 7208 0000 0000 0600 0000 1341 5350  o.r..........ASP
+0000a450: 2050 7974 686f 6e20 6f70 6572 6174 6f72   Python operator
+0000a460: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000a470: 4d4c 0103 0000 004c 0041 0053 0050 0020  ML.....L.A.S.P. 
+0000a480: 0050 0079 0074 0068 006f 006e 0020 005a  .P.y.t.h.o.n. .Z
+0000a490: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
+0000a4a0: 0074 0074 0065 0020 0069 006e 0020 0048  .t.t.e. .i.n. .H
+0000a4b0: 006f 0063 0068 006b 006f 006d 006d 0061  .o.c.h.k.o.m.m.a
+0000a4c0: 0074 0061 0800 0000 0006 0000 001f 4153  .t.a..........AS
+0000a4d0: 5020 5079 7468 6f6e 2073 696e 676c 652d  P Python single-
+0000a4e0: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
+0000a4f0: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
+0000a500: 0300 0000 6e00 4100 5300 5000 2000 5000  ....n.A.S.P. .P.
+0000a510: 7900 7400 6800 6f00 6e00 2000 5a00 6500  y.t.h.o.n. .Z.e.
+0000a520: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
+0000a530: 7400 6500 2000 6900 6e00 2000 6400 7200  t.e. .i.n. .d.r.
+0000a540: 6500 6900 6600 6100 6300 6800 6500 6e00  e.i.f.a.c.h.e.n.
+0000a550: 2000 4100 6e00 6600 fc00 6800 7200 7500   .A.n.f...h.r.u.
+0000a560: 6e00 6700 7300 7a00 6500 6900 6300 6800  n.g.s.z.e.i.c.h.
+0000a570: 6500 6e08 0000 0000 0600 0000 2641 5350  e.n.........&ASP
+0000a580: 2050 7974 686f 6e20 7472 6970 6c65 2064   Python triple d
+0000a590: 6f75 626c 652d 7175 6f74 6564 2073 7472  ouble-quoted str
+0000a5a0: 696e 6707 0000 000d 5173 6369 4c65 7865  ing.....QsciLexe
+0000a5b0: 7248 544d 4c01 0300 0000 6200 4100 5300  rHTML.....b.A.S.
+0000a5c0: 5000 2000 5000 7900 7400 6800 6f00 6e00  P. .P.y.t.h.o.n.
+0000a5d0: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
+0000a5e0: 6b00 6500 7400 7400 6500 2000 6900 6e00  k.e.t.t.e. .i.n.
+0000a5f0: 2000 6400 7200 6500 6900 6600 6100 6300   .d.r.e.i.f.a.c.
+0000a600: 6800 6500 6e00 2000 4800 6f00 6300 6800  h.e.n. .H.o.c.h.
+0000a610: 6b00 6f00 6d00 6d00 6100 7400 6108 0000  k.o.m.m.a.t.a...
+0000a620: 0000 0600 0000 2641 5350 2050 7974 686f  ......&ASP Pytho
+0000a630: 6e20 7472 6970 6c65 2073 696e 676c 652d  n triple single-
+0000a640: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
+0000a650: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
+0000a660: 0300 0000 2c00 4100 5300 5000 2000 5600  ....,.A.S.P. .V.
+0000a670: 4200 5300 6300 7200 6900 7000 7400 2000  B.S.c.r.i.p.t. .
+0000a680: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+0000a690: 7208 0000 0000 0600 0000 1441 5350 2056  r..........ASP V
+0000a6a0: 4253 6372 6970 7420 636f 6d6d 656e 7407  BScript comment.
+0000a6b0: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+0000a6c0: 4c01 0300 0000 2a00 4100 5300 5000 2000  L.....*.A.S.P. .
+0000a6d0: 5600 4200 5300 6300 7200 6900 7000 7400  V.B.S.c.r.i.p.t.
+0000a6e0: 2000 5300 7400 6100 6e00 6400 6100 7200   .S.t.a.n.d.a.r.
+0000a6f0: 6408 0000 0000 0600 0000 1441 5350 2056  d..........ASP V
+0000a700: 4253 6372 6970 7420 6465 6661 756c 7407  BScript default.
+0000a710: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+0000a720: 4c01 0300 0000 2e00 4100 5300 5000 2000  L.......A.S.P. .
+0000a730: 5600 4200 5300 6300 7200 6900 7000 7400  V.B.S.c.r.i.p.t.
+0000a740: 2000 4200 6500 7a00 6500 6900 6300 6800   .B.e.z.e.i.c.h.
+0000a750: 6e00 6500 7208 0000 0000 0600 0000 1741  n.e.r..........A
+0000a760: 5350 2056 4253 6372 6970 7420 6964 656e  SP VBScript iden
+0000a770: 7469 6669 6572 0700 0000 0d51 7363 694c  tifier.....QsciL
+0000a780: 6578 6572 4854 4d4c 0103 0000 0034 0041  exerHTML.....4.A
+0000a790: 0053 0050 0020 0056 0042 0053 0063 0072  .S.P. .V.B.S.c.r
+0000a7a0: 0069 0070 0074 0020 0053 0063 0068 006c  .i.p.t. .S.c.h.l
+0000a7b0: 00fc 0073 0073 0065 006c 0077 006f 0072  ...s.s.e.l.w.o.r
+0000a7c0: 0074 0800 0000 0006 0000 0014 4153 5020  .t..........ASP 
+0000a7d0: 5642 5363 7269 7074 206b 6579 776f 7264  VBScript keyword
+0000a7e0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000a7f0: 4d4c 0103 0000 0022 0041 0053 0050 0020  ML.....".A.S.P. 
+0000a800: 0056 0042 0053 0063 0072 0069 0070 0074  .V.B.S.c.r.i.p.t
+0000a810: 0020 005a 0061 0068 006c 0800 0000 0006  . .Z.a.h.l......
+0000a820: 0000 0013 4153 5020 5642 5363 7269 7074  ....ASP VBScript
+0000a830: 206e 756d 6265 7207 0000 000d 5173 6369   number.....Qsci
+0000a840: 4c65 7865 7248 544d 4c01 0300 0000 3200  LexerHTML.....2.
+0000a850: 4100 5300 5000 2000 5600 4200 5300 6300  A.S.P. .V.B.S.c.
+0000a860: 7200 6900 7000 7400 2000 5a00 6500 6900  r.i.p.t. .Z.e.i.
+0000a870: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
+0000a880: 6508 0000 0000 0600 0000 1341 5350 2056  e..........ASP V
+0000a890: 4253 6372 6970 7420 7374 7269 6e67 0700  BScript string..
+0000a8a0: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000a8b0: 0103 0000 0048 0041 0053 0050 0020 0056  .....H.A.S.P. .V
+0000a8c0: 0042 0053 0063 0072 0069 0070 0074 0020  .B.S.c.r.i.p.t. 
+0000a8d0: 0055 006e 0062 0065 0065 006e 0064 0065  .U.n.b.e.e.n.d.e
+0000a8e0: 0074 0065 0020 005a 0065 0069 0063 0068  .t.e. .Z.e.i.c.h
+0000a8f0: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
+0000a900: 0000 0006 0000 001c 4153 5020 5642 5363  ........ASP VBSc
+0000a910: 7269 7074 2075 6e63 6c6f 7365 6420 7374  ript unclosed st
+0000a920: 7269 6e67 0700 0000 0d51 7363 694c 6578  ring.....QsciLex
+0000a930: 6572 4854 4d4c 0103 0000 0028 0041 0053  erHTML.....(.A.S
+0000a940: 0050 0020 0058 002d 0043 006f 0064 0065  .P. .X.-.C.o.d.e
+0000a950: 0020 004b 006f 006d 006d 0065 006e 0074  . .K.o.m.m.e.n.t
+0000a960: 0061 0072 0800 0000 0006 0000 0012 4153  .a.r..........AS
+0000a970: 5020 582d 436f 6465 2063 6f6d 6d65 6e74  P X-Code comment
+0000a980: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000a990: 4d4c 0103 0000 0010 0041 0074 0074 0072  ML.......A.t.t.r
+0000a9a0: 0069 0062 0075 0074 0800 0000 0006 0000  .i.b.u.t........
+0000a9b0: 0009 4174 7472 6962 7574 6507 0000 000d  ..Attribute.....
+0000a9c0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000a9d0: 0000 0a00 4300 4400 4100 5400 4108 0000  ....C.D.A.T.A...
+0000a9e0: 0000 0600 0000 0543 4441 5441 0700 0000  .......CDATA....
+0000a9f0: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000aa00: 0000 000e 0054 0061 0067 0065 006e 0064  .....T.a.g.e.n.d
+0000aa10: 0065 0800 0000 0006 0000 000c 456e 6420  .e..........End 
+0000aa20: 6f66 2061 2074 6167 0700 0000 0d51 7363  of a tag.....Qsc
+0000aa30: 694c 6578 6572 4854 4d4c 0103 0000 0032  iLexerHTML.....2
+0000aa40: 0045 006e 0064 0065 0020 0065 0069 006e  .E.n.d.e. .e.i.n
+0000aa50: 0065 0073 0020 0058 004d 004c 0020 0046  .e.s. .X.M.L. .F
+0000aa60: 0072 0061 0067 006d 0065 006e 0074 0065  .r.a.g.m.e.n.t.e
+0000aa70: 0073 0800 0000 0006 0000 0016 456e 6420  .s..........End 
+0000aa80: 6f66 2061 6e20 584d 4c20 6672 6167 6d65  of an XML fragme
+0000aa90: 6e74 0700 0000 0d51 7363 694c 6578 6572  nt.....QsciLexer
+0000aaa0: 4854 4d4c 0103 0000 000e 0045 006e 0074  HTML.......E.n.t
+0000aab0: 0069 0074 00e4 0074 0800 0000 0006 0000  .i.t...t........
+0000aac0: 0006 456e 7469 7479 0700 0000 0d51 7363  ..Entity.....Qsc
+0000aad0: 694c 6578 6572 4854 4d4c 0103 0000 0064  iLexerHTML.....d
+0000aae0: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
+0000aaf0: 0072 0020 0064 0065 0073 0020 0065 0072  .r. .d.e.s. .e.r
+0000ab00: 0073 0074 0065 006e 0020 0050 0061 0072  .s.t.e.n. .P.a.r
+0000ab10: 0061 006d 0065 0074 0065 0072 0073 0020  .a.m.e.t.e.r.s. 
+0000ab20: 0065 0069 006e 0065 0073 0020 0053 0047  .e.i.n.e.s. .S.G
+0000ab30: 004d 004c 0020 0042 0065 0066 0065 0068  .M.L. .B.e.f.e.h
+0000ab40: 006c 0073 0800 0000 0006 0000 002a 4669  .l.s.........*Fi
+0000ab50: 7273 7420 7061 7261 6d65 7465 7220 636f  rst parameter co
+0000ab60: 6d6d 656e 7420 6f66 2061 6e20 5347 4d4c  mment of an SGML
+0000ab70: 2063 6f6d 6d61 6e64 0700 0000 0d51 7363   command.....Qsc
+0000ab80: 694c 6578 6572 4854 4d4c 0103 0000 0046  iLexerHTML.....F
+0000ab90: 0045 0072 0073 0074 0065 0072 0020 0050  .E.r.s.t.e.r. .P
+0000aba0: 0061 0072 0061 006d 0065 0074 0065 0072  .a.r.a.m.e.t.e.r
+0000abb0: 0020 0065 0069 006e 0065 0073 0020 0053  . .e.i.n.e.s. .S
+0000abc0: 0047 004d 004c 0020 0042 0065 0066 0065  .G.M.L. .B.e.f.e
+0000abd0: 0068 006c 0073 0800 0000 0006 0000 0022  .h.l.s........."
+0000abe0: 4669 7273 7420 7061 7261 6d65 7465 7220  First parameter 
+0000abf0: 6f66 2061 6e20 5347 4d4c 2063 6f6d 6d61  of an SGML comma
+0000ac00: 6e64 0700 0000 0d51 7363 694c 6578 6572  nd.....QsciLexer
+0000ac10: 4854 4d4c 0103 0000 001c 0048 0054 004d  HTML.......H.T.M
+0000ac20: 004c 0020 004b 006f 006d 006d 0065 006e  .L. .K.o.m.m.e.n
+0000ac30: 0074 0061 0072 0800 0000 0006 0000 000c  .t.a.r..........
+0000ac40: 4854 4d4c 2063 6f6d 6d65 6e74 0700 0000  HTML comment....
+0000ac50: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000ac60: 0000 001a 0048 0054 004d 004c 0020 0053  .....H.T.M.L. .S
+0000ac70: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+0000ac80: 0000 0006 0000 000c 4854 4d4c 2064 6566  ........HTML def
+0000ac90: 6175 6c74 0700 0000 0d51 7363 694c 6578  ault.....QsciLex
+0000aca0: 6572 4854 4d4c 0103 0000 004c 0048 0054  erHTML.....L.H.T
+0000acb0: 004d 004c 0020 005a 0065 0069 0063 0068  .M.L. .Z.e.i.c.h
+0000acc0: 0065 006e 006b 0065 0074 0074 0065 0020  .e.n.k.e.t.t.e. 
+0000acd0: 0069 006e 0020 0041 006e 0066 00fc 0068  .i.n. .A.n.f...h
+0000ace0: 0072 0075 006e 0067 0073 007a 0065 0069  .r.u.n.g.s.z.e.i
+0000acf0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
+0000ad00: 0019 4854 4d4c 2064 6f75 626c 652d 7175  ..HTML double-qu
+0000ad10: 6f74 6564 2073 7472 696e 6707 0000 000d  oted string.....
+0000ad20: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000ad30: 0000 1200 4800 5400 4d00 4c00 2000 5a00  ....H.T.M.L. .Z.
+0000ad40: 6100 6800 6c08 0000 0000 0600 0000 0b48  a.h.l..........H
+0000ad50: 544d 4c20 6e75 6d62 6572 0700 0000 0d51  TML number.....Q
+0000ad60: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+0000ad70: 0040 0048 0054 004d 004c 0020 005a 0065  .@.H.T.M.L. .Z.e
+0000ad80: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+0000ad90: 0074 0065 0020 0069 006e 0020 0048 006f  .t.e. .i.n. .H.o
+0000ada0: 0063 0068 006b 006f 006d 006d 0061 0074  .c.h.k.o.m.m.a.t
+0000adb0: 0061 0800 0000 0006 0000 0019 4854 4d4c  .a..........HTML
+0000adc0: 2073 696e 676c 652d 7175 6f74 6564 2073   single-quoted s
+0000add0: 7472 696e 6707 0000 000d 5173 6369 4c65  tring.....QsciLe
+0000ade0: 7865 7248 544d 4c01 0300 0000 4000 4a00  xerHTML.....@.J.
+0000adf0: 6100 7600 6100 4400 6f00 6300 2000 4100  a.v.a.D.o.c. .A.
+0000ae00: 5300 5000 2000 4a00 6100 7600 6100 5300  S.P. .J.a.v.a.S.
+0000ae10: 6300 7200 6900 7000 7400 2000 4b00 6f00  c.r.i.p.t. .K.o.
+0000ae20: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+0000ae30: 0000 0600 0000 244a 6176 6144 6f63 2073  ......$JavaDoc s
+0000ae40: 7479 6c65 2041 5350 204a 6176 6153 6372  tyle ASP JavaScr
+0000ae50: 6970 7420 636f 6d6d 656e 7407 0000 000d  ipt comment.....
+0000ae60: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000ae70: 0000 3800 4a00 6100 7600 6100 4400 6f00  ..8.J.a.v.a.D.o.
+0000ae80: 6300 2000 4a00 6100 7600 6100 5300 6300  c. .J.a.v.a.S.c.
+0000ae90: 7200 6900 7000 7400 2000 4b00 6f00 6d00  r.i.p.t. .K.o.m.
+0000aea0: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+0000aeb0: 0600 0000 204a 6176 6144 6f63 2073 7479  .... JavaDoc sty
+0000aec0: 6c65 204a 6176 6153 6372 6970 7420 636f  le JavaScript co
+0000aed0: 6d6d 656e 7407 0000 000d 5173 6369 4c65  mment.....QsciLe
+0000aee0: 7865 7248 544d 4c01 0300 0000 2800 4a00  xerHTML.....(.J.
+0000aef0: 6100 7600 6100 5300 6300 7200 6900 7000  a.v.a.S.c.r.i.p.
+0000af00: 7400 2000 4b00 6f00 6d00 6d00 6500 6e00  t. .K.o.m.m.e.n.
+0000af10: 7400 6100 7208 0000 0000 0600 0000 124a  t.a.r..........J
+0000af20: 6176 6153 6372 6970 7420 636f 6d6d 656e  avaScript commen
+0000af30: 7407 0000 000d 5173 6369 4c65 7865 7248  t.....QsciLexerH
+0000af40: 544d 4c01 0300 0000 2600 4a00 6100 7600  TML.....&.J.a.v.
+0000af50: 6100 5300 6300 7200 6900 7000 7400 2000  a.S.c.r.i.p.t. .
+0000af60: 5300 7400 6100 6e00 6400 6100 7200 6408  S.t.a.n.d.a.r.d.
+0000af70: 0000 0000 0600 0000 124a 6176 6153 6372  .........JavaScr
+0000af80: 6970 7420 6465 6661 756c 7407 0000 000d  ipt default.....
+0000af90: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000afa0: 0000 5800 4a00 6100 7600 6100 5300 6300  ..X.J.a.v.a.S.c.
+0000afb0: 7200 6900 7000 7400 2000 5a00 6500 6900  r.i.p.t. .Z.e.i.
+0000afc0: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
+0000afd0: 6500 2000 6900 6e00 2000 4100 6e00 6600  e. .i.n. .A.n.f.
+0000afe0: fc00 6800 7200 7500 6e00 6700 7300 7a00  ..h.r.u.n.g.s.z.
+0000aff0: 6500 6900 6300 6800 6500 6e08 0000 0000  e.i.c.h.e.n.....
+0000b000: 0600 0000 1f4a 6176 6153 6372 6970 7420  .....JavaScript 
+0000b010: 646f 7562 6c65 2d71 756f 7465 6420 7374  double-quoted st
+0000b020: 7269 6e67 0700 0000 0d51 7363 694c 6578  ring.....QsciLex
+0000b030: 6572 4854 4d4c 0103 0000 0030 004a 0061  erHTML.....0.J.a
+0000b040: 0076 0061 0053 0063 0072 0069 0070 0074  .v.a.S.c.r.i.p.t
+0000b050: 0020 0053 0063 0068 006c 00fc 0073 0073  . .S.c.h.l...s.s
+0000b060: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
+0000b070: 0006 0000 0012 4a61 7661 5363 7269 7074  ......JavaScript
+0000b080: 206b 6579 776f 7264 0700 0000 0d51 7363   keyword.....Qsc
+0000b090: 694c 6578 6572 4854 4d4c 0103 0000 0034  iLexerHTML.....4
+0000b0a0: 004a 0061 0076 0061 0053 0063 0072 0069  .J.a.v.a.S.c.r.i
+0000b0b0: 0070 0074 0020 005a 0065 0069 006c 0065  .p.t. .Z.e.i.l.e
+0000b0c0: 006e 006b 006f 006d 006d 0065 006e 0074  .n.k.o.m.m.e.n.t
+0000b0d0: 0061 0072 0800 0000 0006 0000 0017 4a61  .a.r..........Ja
+0000b0e0: 7661 5363 7269 7074 206c 696e 6520 636f  vaScript line co
+0000b0f0: 6d6d 656e 7407 0000 000d 5173 6369 4c65  mment.....QsciLe
+0000b100: 7865 7248 544d 4c01 0300 0000 1e00 4a00  xerHTML.......J.
+0000b110: 6100 7600 6100 5300 6300 7200 6900 7000  a.v.a.S.c.r.i.p.
+0000b120: 7400 2000 5a00 6100 6800 6c08 0000 0000  t. .Z.a.h.l.....
+0000b130: 0600 0000 114a 6176 6153 6372 6970 7420  .....JavaScript 
+0000b140: 6e75 6d62 6572 0700 0000 0d51 7363 694c  number.....QsciL
+0000b150: 6578 6572 4854 4d4c 0103 0000 003a 004a  exerHTML.....:.J
+0000b160: 0061 0076 0061 0053 0063 0072 0069 0070  .a.v.a.S.c.r.i.p
+0000b170: 0074 0020 0052 0065 0067 0075 006c 00e4  .t. .R.e.g.u.l..
+0000b180: 0072 0065 0072 0020 0041 0075 0073 0064  .r.e.r. .A.u.s.d
+0000b190: 0072 0075 0063 006b 0800 0000 0006 0000  .r.u.c.k........
+0000b1a0: 001d 4a61 7661 5363 7269 7074 2072 6567  ..JavaScript reg
+0000b1b0: 756c 6172 2065 7870 7265 7373 696f 6e07  ular expression.
+0000b1c0: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+0000b1d0: 4c01 0300 0000 4c00 4a00 6100 7600 6100  L.....L.J.a.v.a.
+0000b1e0: 5300 6300 7200 6900 7000 7400 2000 5a00  S.c.r.i.p.t. .Z.
+0000b1f0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+0000b200: 7400 7400 6500 2000 6900 6e00 2000 4800  t.t.e. .i.n. .H.
+0000b210: 6f00 6300 6800 6b00 6f00 6d00 6d00 6100  o.c.h.k.o.m.m.a.
+0000b220: 7400 6108 0000 0000 0600 0000 1f4a 6176  t.a..........Jav
+0000b230: 6153 6372 6970 7420 7369 6e67 6c65 2d71  aScript single-q
+0000b240: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
+0000b250: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000b260: 0000 0022 004a 0061 0076 0061 0053 0063  ...".J.a.v.a.S.c
+0000b270: 0072 0069 0070 0074 0020 0053 0079 006d  .r.i.p.t. .S.y.m
+0000b280: 0062 006f 006c 0800 0000 0006 0000 0011  .b.o.l..........
+0000b290: 4a61 7661 5363 7269 7074 2073 796d 626f  JavaScript symbo
+0000b2a0: 6c07 0000 000d 5173 6369 4c65 7865 7248  l.....QsciLexerH
+0000b2b0: 544d 4c01 0300 0000 4400 4a00 6100 7600  TML.....D.J.a.v.
+0000b2c0: 6100 5300 6300 7200 6900 7000 7400 2000  a.S.c.r.i.p.t. .
+0000b2d0: 5500 6e00 6200 6500 6500 6e00 6400 6500  U.n.b.e.e.n.d.e.
+0000b2e0: 7400 6500 2000 5a00 6500 6900 6300 6800  t.e. .Z.e.i.c.h.
+0000b2f0: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
+0000b300: 0000 0600 0000 1a4a 6176 6153 6372 6970  .......JavaScrip
+0000b310: 7420 756e 636c 6f73 6564 2073 7472 696e  t unclosed strin
+0000b320: 6707 0000 000d 5173 6369 4c65 7865 7248  g.....QsciLexerH
+0000b330: 544d 4c01 0300 0000 1e00 4a00 6100 7600  TML.......J.a.v.
+0000b340: 6100 5300 6300 7200 6900 7000 7400 2000  a.S.c.r.i.p.t. .
+0000b350: 5700 6f00 7200 7408 0000 0000 0600 0000  W.o.r.t.........
+0000b360: 0f4a 6176 6153 6372 6970 7420 776f 7264  .JavaScript word
+0000b370: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000b380: 4d4c 0103 0000 0032 0041 006e 0064 0065  ML.....2.A.n.d.e
+0000b390: 0072 0065 0072 0020 0054 0065 0078 0074  .r.e.r. .T.e.x.t
+0000b3a0: 0020 0069 006e 0020 0065 0069 006e 0065  . .i.n. .e.i.n.e
+0000b3b0: 006d 0020 0054 0061 0067 0800 0000 0006  .m. .T.a.g......
+0000b3c0: 0000 0013 4f74 6865 7220 7465 7874 2069  ....Other text i
+0000b3d0: 6e20 6120 7461 6707 0000 000d 5173 6369  n a tag.....Qsci
+0000b3e0: 4c65 7865 7248 544d 4c01 0300 0000 1a00  LexerHTML.......
+0000b3f0: 5000 4800 5000 2000 4b00 6f00 6d00 6d00  P.H.P. .K.o.m.m.
+0000b400: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
+0000b410: 0000 0b50 4850 2063 6f6d 6d65 6e74 0700  ...PHP comment..
+0000b420: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000b430: 0103 0000 0018 0050 0048 0050 0020 0053  .......P.H.P. .S
+0000b440: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+0000b450: 0000 0006 0000 000b 5048 5020 6465 6661  ........PHP defa
+0000b460: 756c 7407 0000 000d 5173 6369 4c65 7865  ult.....QsciLexe
+0000b470: 7248 544d 4c01 0300 0000 4a00 5000 4800  rHTML.....J.P.H.
+0000b480: 5000 2000 5a00 6500 6900 6300 6800 6500  P. .Z.e.i.c.h.e.
+0000b490: 6e00 6b00 6500 7400 7400 6500 2000 6900  n.k.e.t.t.e. .i.
+0000b4a0: 6e00 2000 4100 6e00 6600 fc00 6800 7200  n. .A.n.f...h.r.
+0000b4b0: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
+0000b4c0: 6800 6500 6e08 0000 0000 0600 0000 1850  h.e.n..........P
+0000b4d0: 4850 2064 6f75 626c 652d 7175 6f74 6564  HP double-quoted
+0000b4e0: 2073 7472 696e 6707 0000 000d 5173 6369   string.....Qsci
+0000b4f0: 4c65 7865 7248 544d 4c01 0300 0000 4200  LexerHTML.....B.
+0000b500: 5000 4800 5000 2000 5600 6100 7200 6900  P.H.P. .V.a.r.i.
+0000b510: 6100 6200 6c00 6500 2000 6900 6e00 2000  a.b.l.e. .i.n. .
+0000b520: 4100 6e00 6600 fc00 6800 7200 7500 6e00  A.n.f...h.r.u.n.
+0000b530: 6700 7300 7a00 6500 6900 6300 6800 6500  g.s.z.e.i.c.h.e.
+0000b540: 6e08 0000 0000 0600 0000 1a50 4850 2064  n..........PHP d
+0000b550: 6f75 626c 652d 7175 6f74 6564 2076 6172  ouble-quoted var
+0000b560: 6961 626c 6507 0000 000d 5173 6369 4c65  iable.....QsciLe
+0000b570: 7865 7248 544d 4c01 0300 0000 2200 5000  xerHTML.....".P.
+0000b580: 4800 5000 2000 5300 6300 6800 6c00 fc00  H.P. .S.c.h.l...
+0000b590: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
+0000b5a0: 0000 0000 0600 0000 0b50 4850 206b 6579  .........PHP key
+0000b5b0: 776f 7264 0700 0000 0d51 7363 694c 6578  word.....QsciLex
+0000b5c0: 6572 4854 4d4c 0103 0000 0026 0050 0048  erHTML.....&.P.H
+0000b5d0: 0050 0020 005a 0065 0069 006c 0065 006e  .P. .Z.e.i.l.e.n
+0000b5e0: 006b 006f 006d 006d 0065 006e 0074 0061  .k.o.m.m.e.n.t.a
+0000b5f0: 0072 0800 0000 0006 0000 0010 5048 5020  .r..........PHP 
+0000b600: 6c69 6e65 2063 6f6d 6d65 6e74 0700 0000  line comment....
+0000b610: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000b620: 0000 0010 0050 0048 0050 0020 005a 0061  .....P.H.P. .Z.a
+0000b630: 0068 006c 0800 0000 0006 0000 000a 5048  .h.l..........PH
+0000b640: 5020 6e75 6d62 6572 0700 0000 0d51 7363  P number.....Qsc
+0000b650: 694c 6578 6572 4854 4d4c 0103 0000 0018  iLexerHTML......
+0000b660: 0050 0048 0050 0020 004f 0070 0065 0072  .P.H.P. .O.p.e.r
+0000b670: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+0000b680: 000c 5048 5020 6f70 6572 6174 6f72 0700  ..PHP operator..
+0000b690: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000b6a0: 0103 0000 003e 0050 0048 0050 0020 005a  .....>.P.H.P. .Z
+0000b6b0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
+0000b6c0: 0074 0074 0065 0020 0069 006e 0020 0048  .t.t.e. .i.n. .H
+0000b6d0: 006f 0063 0068 006b 006f 006d 006d 0061  .o.c.h.k.o.m.m.a
+0000b6e0: 0074 0061 0800 0000 0006 0000 0018 5048  .t.a..........PH
+0000b6f0: 5020 7369 6e67 6c65 2d71 756f 7465 6420  P single-quoted 
+0000b700: 7374 7269 6e67 0700 0000 0d51 7363 694c  string.....QsciL
+0000b710: 6578 6572 4854 4d4c 0103 0000 0018 0050  exerHTML.......P
+0000b720: 0048 0050 0020 0056 0061 0072 0069 0061  .H.P. .V.a.r.i.a
+0000b730: 0062 006c 0065 0800 0000 0006 0000 000c  .b.l.e..........
+0000b740: 5048 5020 7661 7269 6162 6c65 0700 0000  PHP variable....
+0000b750: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000b760: 0000 0024 0050 0079 0074 0068 006f 006e  ...$.P.y.t.h.o.n
+0000b770: 0020 004b 006c 0061 0073 0073 0065 006e  . .K.l.a.s.s.e.n
+0000b780: 006e 0061 006d 0065 0800 0000 0006 0000  .n.a.m.e........
+0000b790: 0011 5079 7468 6f6e 2063 6c61 7373 206e  ..Python class n
+0000b7a0: 616d 6507 0000 000d 5173 6369 4c65 7865  ame.....QsciLexe
+0000b7b0: 7248 544d 4c01 0300 0000 2000 5000 7900  rHTML..... .P.y.
+0000b7c0: 7400 6800 6f00 6e00 2000 4b00 6f00 6d00  t.h.o.n. .K.o.m.
+0000b7d0: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+0000b7e0: 0600 0000 0e50 7974 686f 6e20 636f 6d6d  .....Python comm
+0000b7f0: 656e 7407 0000 000d 5173 6369 4c65 7865  ent.....QsciLexe
+0000b800: 7248 544d 4c01 0300 0000 1e00 5000 7900  rHTML.......P.y.
+0000b810: 7400 6800 6f00 6e00 2000 5300 7400 6100  t.h.o.n. .S.t.a.
+0000b820: 6e00 6400 6100 7200 6408 0000 0000 0600  n.d.a.r.d.......
+0000b830: 0000 0e50 7974 686f 6e20 6465 6661 756c  ...Python defaul
+0000b840: 7407 0000 000d 5173 6369 4c65 7865 7248  t.....QsciLexerH
+0000b850: 544d 4c01 0300 0000 5000 5000 7900 7400  TML.....P.P.y.t.
+0000b860: 6800 6f00 6e00 2000 5a00 6500 6900 6300  h.o.n. .Z.e.i.c.
+0000b870: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
+0000b880: 2000 6900 6e00 2000 4100 6e00 6600 fc00   .i.n. .A.n.f...
+0000b890: 6800 7200 7500 6e00 6700 7300 7a00 6500  h.r.u.n.g.s.z.e.
+0000b8a0: 6900 6300 6800 6500 6e08 0000 0000 0600  i.c.h.e.n.......
+0000b8b0: 0000 1b50 7974 686f 6e20 646f 7562 6c65  ...Python double
+0000b8c0: 2d71 756f 7465 6420 7374 7269 6e67 0700  -quoted string..
+0000b8d0: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000b8e0: 0103 0000 0046 0050 0079 0074 0068 006f  .....F.P.y.t.h.o
+0000b8f0: 006e 0020 0046 0075 006e 006b 0074 0069  .n. .F.u.n.k.t.i
+0000b900: 006f 006e 0073 002d 0020 006f 0064 0065  .o.n.s.-. .o.d.e
+0000b910: 0072 0020 004d 0065 0074 0068 006f 0064  .r. .M.e.t.h.o.d
+0000b920: 0065 006e 006e 0061 006d 0065 0800 0000  .e.n.n.a.m.e....
+0000b930: 0006 0000 001e 5079 7468 6f6e 2066 756e  ......Python fun
+0000b940: 6374 696f 6e20 6f72 206d 6574 686f 6420  ction or method 
+0000b950: 6e61 6d65 0700 0000 0d51 7363 694c 6578  name.....QsciLex
+0000b960: 6572 4854 4d4c 0103 0000 0022 0050 0079  erHTML.....".P.y
+0000b970: 0074 0068 006f 006e 0020 0042 0065 007a  .t.h.o.n. .B.e.z
+0000b980: 0065 0069 0063 0068 006e 0065 0072 0800  .e.i.c.h.n.e.r..
+0000b990: 0000 0006 0000 0011 5079 7468 6f6e 2069  ........Python i
+0000b9a0: 6465 6e74 6966 6965 7207 0000 000d 5173  dentifier.....Qs
+0000b9b0: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
+0000b9c0: 2800 5000 7900 7400 6800 6f00 6e00 2000  (.P.y.t.h.o.n. .
+0000b9d0: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
+0000b9e0: 6c00 7700 6f00 7200 7408 0000 0000 0600  l.w.o.r.t.......
+0000b9f0: 0000 0e50 7974 686f 6e20 6b65 7977 6f72  ...Python keywor
+0000ba00: 6407 0000 000d 5173 6369 4c65 7865 7248  d.....QsciLexerH
+0000ba10: 544d 4c01 0300 0000 1600 5000 7900 7400  TML.......P.y.t.
+0000ba20: 6800 6f00 6e00 2000 5a00 6100 6800 6c08  h.o.n. .Z.a.h.l.
+0000ba30: 0000 0000 0600 0000 0d50 7974 686f 6e20  .........Python 
+0000ba40: 6e75 6d62 6572 0700 0000 0d51 7363 694c  number.....QsciL
+0000ba50: 6578 6572 4854 4d4c 0103 0000 001e 0050  exerHTML.......P
+0000ba60: 0079 0074 0068 006f 006e 0020 004f 0070  .y.t.h.o.n. .O.p
+0000ba70: 0065 0072 0061 0074 006f 0072 0800 0000  .e.r.a.t.o.r....
+0000ba80: 0006 0000 000f 5079 7468 6f6e 206f 7065  ......Python ope
+0000ba90: 7261 746f 7207 0000 000d 5173 6369 4c65  rator.....QsciLe
+0000baa0: 7865 7248 544d 4c01 0300 0000 4400 5000  xerHTML.....D.P.
+0000bab0: 7900 7400 6800 6f00 6e00 2000 5a00 6500  y.t.h.o.n. .Z.e.
+0000bac0: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
+0000bad0: 7400 6500 2000 6900 6e00 2000 4800 6f00  t.e. .i.n. .H.o.
+0000bae0: 6300 6800 6b00 6f00 6d00 6d00 6100 7400  c.h.k.o.m.m.a.t.
+0000baf0: 6108 0000 0000 0600 0000 1b50 7974 686f  a..........Pytho
+0000bb00: 6e20 7369 6e67 6c65 2d71 756f 7465 6420  n single-quoted 
+0000bb10: 7374 7269 6e67 0700 0000 0d51 7363 694c  string.....QsciL
+0000bb20: 6578 6572 4854 4d4c 0103 0000 0066 0050  exerHTML.....f.P
+0000bb30: 0079 0074 0068 006f 006e 0020 005a 0065  .y.t.h.o.n. .Z.e
+0000bb40: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+0000bb50: 0074 0065 0020 0069 006e 0020 0064 0072  .t.e. .i.n. .d.r
+0000bb60: 0065 0069 0066 0061 0063 0068 0065 006e  .e.i.f.a.c.h.e.n
+0000bb70: 0020 0041 006e 0066 00fc 0068 0072 0075  . .A.n.f...h.r.u
+0000bb80: 006e 0067 0073 007a 0065 0069 0063 0068  .n.g.s.z.e.i.c.h
+0000bb90: 0065 006e 0800 0000 0006 0000 0022 5079  .e.n........."Py
+0000bba0: 7468 6f6e 2074 7269 706c 6520 646f 7562  thon triple doub
+0000bbb0: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
+0000bbc0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000bbd0: 4d4c 0103 0000 005a 0050 0079 0074 0068  ML.....Z.P.y.t.h
+0000bbe0: 006f 006e 0020 005a 0065 0069 0063 0068  .o.n. .Z.e.i.c.h
+0000bbf0: 0065 006e 006b 0065 0074 0074 0065 0020  .e.n.k.e.t.t.e. 
+0000bc00: 0069 006e 0020 0064 0072 0065 0069 0066  .i.n. .d.r.e.i.f
+0000bc10: 0061 0063 0068 0065 006e 0020 0048 006f  .a.c.h.e.n. .H.o
+0000bc20: 0063 0068 006b 006f 006d 006d 0061 0074  .c.h.k.o.m.m.a.t
+0000bc30: 0061 0800 0000 0006 0000 0022 5079 7468  .a........."Pyth
+0000bc40: 6f6e 2074 7269 706c 6520 7369 6e67 6c65  on triple single
+0000bc50: 2d71 756f 7465 6420 7374 7269 6e67 0700  -quoted string..
+0000bc60: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000bc70: 0103 0000 0024 0053 0047 004d 004c 0020  .....$.S.G.M.L. 
+0000bc80: 0053 0074 0061 006e 0064 0061 0072 0064  .S.t.a.n.d.a.r.d
+0000bc90: 0062 006c 006f 0063 006b 0800 0000 0006  .b.l.o.c.k......
+0000bca0: 0000 0012 5347 4d4c 2062 6c6f 636b 2064  ....SGML block d
+0000bcb0: 6566 6175 6c74 0700 0000 0d51 7363 694c  efault.....QsciL
+0000bcc0: 6578 6572 4854 4d4c 0103 0000 0016 0053  exerHTML.......S
+0000bcd0: 0047 004d 004c 0020 0042 0065 0066 0065  .G.M.L. .B.e.f.e
+0000bce0: 0068 006c 0800 0000 0006 0000 000c 5347  .h.l..........SG
+0000bcf0: 4d4c 2063 6f6d 6d61 6e64 0700 0000 0d51  ML command.....Q
+0000bd00: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+0000bd10: 001c 0053 0047 004d 004c 0020 004b 006f  ...S.G.M.L. .K.o
+0000bd20: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+0000bd30: 0000 0006 0000 000c 5347 4d4c 2063 6f6d  ........SGML com
+0000bd40: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
+0000bd50: 6572 4854 4d4c 0103 0000 001a 0053 0047  erHTML.......S.G
+0000bd60: 004d 004c 0020 0053 0074 0061 006e 0064  .M.L. .S.t.a.n.d
+0000bd70: 0061 0072 0064 0800 0000 0006 0000 000c  .a.r.d..........
+0000bd80: 5347 4d4c 2064 6566 6175 6c74 0700 0000  SGML default....
+0000bd90: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000bda0: 0000 004c 0053 0047 004d 004c 0020 005a  ...L.S.G.M.L. .Z
+0000bdb0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
+0000bdc0: 0074 0074 0065 0020 0069 006e 0020 0041  .t.t.e. .i.n. .A
+0000bdd0: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
+0000bde0: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
+0000bdf0: 0800 0000 0006 0000 0019 5347 4d4c 2064  ..........SGML d
+0000be00: 6f75 626c 652d 7175 6f74 6564 2073 7472  ouble-quoted str
+0000be10: 696e 6707 0000 000d 5173 6369 4c65 7865  ing.....QsciLexe
+0000be20: 7248 544d 4c01 0300 0000 1600 5300 4700  rHTML.......S.G.
+0000be30: 4d00 4c00 2000 4600 6500 6800 6c00 6500  M.L. .F.e.h.l.e.
+0000be40: 7208 0000 0000 0600 0000 0a53 474d 4c20  r..........SGML 
+0000be50: 6572 726f 7207 0000 000d 5173 6369 4c65  error.....QsciLe
+0000be60: 7865 7248 544d 4c01 0300 0000 4000 5300  xerHTML.....@.S.
+0000be70: 4700 4d00 4c00 2000 5a00 6500 6900 6300  G.M.L. .Z.e.i.c.
+0000be80: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
+0000be90: 2000 6900 6e00 2000 4800 6f00 6300 6800   .i.n. .H.o.c.h.
+0000bea0: 6b00 6f00 6d00 6d00 6100 7400 6108 0000  k.o.m.m.a.t.a...
+0000beb0: 0000 0600 0000 1953 474d 4c20 7369 6e67  .......SGML sing
+0000bec0: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
 0000bed0: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000bee0: 4d4c 0103 0000 001e 0055 006e 0062 0065  ML.......U.n.b.e
-0000bef0: 006b 0061 006e 006e 0074 0065 0073 0020  .k.a.n.n.t.e.s. 
-0000bf00: 0054 0061 0067 0800 0000 0006 0000 000b  .T.a.g..........
-0000bf10: 556e 6b6e 6f77 6e20 7461 6707 0000 000d  Unknown tag.....
-0000bf20: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
-0000bf30: 0000 4000 4800 5400 4d00 4c00 2000 5700  ..@.H.T.M.L. .W.
-0000bf40: 6500 7200 7400 2000 6f00 6800 6e00 6500  e.r.t. .o.h.n.e.
-0000bf50: 2000 4100 6e00 6600 fc00 6800 7200 7500   .A.n.f...h.r.u.
-0000bf60: 6e00 6700 7300 7a00 6500 6900 6300 6800  n.g.s.z.e.i.c.h.
-0000bf70: 6500 6e08 0000 0000 0600 0000 1355 6e71  e.n..........Unq
-0000bf80: 756f 7465 6420 4854 4d4c 2076 616c 7565  uoted HTML value
-0000bf90: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
-0000bfa0: 4d4c 0103 0000 0024 0056 0042 0053 0063  ML.....$.V.B.S.c
-0000bfb0: 0072 0069 0070 0074 0020 004b 006f 006d  .r.i.p.t. .K.o.m
-0000bfc0: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
-0000bfd0: 0006 0000 0010 5642 5363 7269 7074 2063  ......VBScript c
-0000bfe0: 6f6d 6d65 6e74 0700 0000 0d51 7363 694c  omment.....QsciL
-0000bff0: 6578 6572 4854 4d4c 0103 0000 0022 0056  exerHTML.....".V
-0000c000: 0042 0053 0063 0072 0069 0070 0074 0020  .B.S.c.r.i.p.t. 
-0000c010: 0053 0074 0061 006e 0064 0061 0072 0064  .S.t.a.n.d.a.r.d
-0000c020: 0800 0000 0006 0000 0010 5642 5363 7269  ..........VBScri
-0000c030: 7074 2064 6566 6175 6c74 0700 0000 0d51  pt default.....Q
-0000c040: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
-0000c050: 0026 0056 0042 0053 0063 0072 0069 0070  .&.V.B.S.c.r.i.p
-0000c060: 0074 0020 0042 0065 007a 0065 0069 0063  .t. .B.e.z.e.i.c
-0000c070: 0068 006e 0065 0072 0800 0000 0006 0000  .h.n.e.r........
-0000c080: 0013 5642 5363 7269 7074 2069 6465 6e74  ..VBScript ident
-0000c090: 6966 6965 7207 0000 000d 5173 6369 4c65  ifier.....QsciLe
-0000c0a0: 7865 7248 544d 4c01 0300 0000 2c00 5600  xerHTML.....,.V.
-0000c0b0: 4200 5300 6300 7200 6900 7000 7400 2000  B.S.c.r.i.p.t. .
-0000c0c0: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
-0000c0d0: 6c00 7700 6f00 7200 7408 0000 0000 0600  l.w.o.r.t.......
-0000c0e0: 0000 1056 4253 6372 6970 7420 6b65 7977  ...VBScript keyw
-0000c0f0: 6f72 6407 0000 000d 5173 6369 4c65 7865  ord.....QsciLexe
-0000c100: 7248 544d 4c01 0300 0000 1a00 5600 4200  rHTML.......V.B.
-0000c110: 5300 6300 7200 6900 7000 7400 2000 5a00  S.c.r.i.p.t. .Z.
-0000c120: 6100 6800 6c08 0000 0000 0600 0000 0f56  a.h.l..........V
-0000c130: 4253 6372 6970 7420 6e75 6d62 6572 0700  BScript number..
-0000c140: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
-0000c150: 0103 0000 002a 0056 0042 0053 0063 0072  .....*.V.B.S.c.r
-0000c160: 0069 0070 0074 0020 005a 0065 0069 0063  .i.p.t. .Z.e.i.c
-0000c170: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
-0000c180: 0800 0000 0006 0000 000f 5642 5363 7269  ..........VBScri
-0000c190: 7074 2073 7472 696e 6707 0000 000d 5173  pt string.....Qs
-0000c1a0: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
-0000c1b0: 4000 5600 4200 5300 6300 7200 6900 7000  @.V.B.S.c.r.i.p.
-0000c1c0: 7400 2000 5500 6e00 6200 6500 6500 6e00  t. .U.n.b.e.e.n.
-0000c1d0: 6400 6500 7400 6500 2000 5a00 6500 6900  d.e.t.e. .Z.e.i.
-0000c1e0: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-0000c1f0: 6508 0000 0000 0600 0000 1856 4253 6372  e..........VBScr
-0000c200: 6970 7420 756e 636c 6f73 6564 2073 7472  ipt unclosed str
-0000c210: 696e 6707 0000 000d 5173 6369 4c65 7865  ing.....QsciLexe
-0000c220: 7248 544d 4c01 0300 0000 0800 5500 5500  rHTML.......U.U.
-0000c230: 4900 4408 0000 0000 0600 0000 0455 5549  I.D..........UUI
-0000c240: 4407 0000 000c 5173 6369 4c65 7865 7249  D.....QsciLexerI
-0000c250: 444c 0103 0000 001c 0042 006c 006f 0063  DL.......B.l.o.c
-0000c260: 006b 006b 006f 006d 006d 0065 006e 0074  .k.k.o.m.m.e.n.t
-0000c270: 0061 0072 0800 0000 0006 0000 000d 426c  .a.r..........Bl
-0000c280: 6f63 6b20 636f 6d6d 656e 7407 0000 000d  ock comment.....
-0000c290: 5173 6369 4c65 7865 724a 534f 4e01 0300  QsciLexerJSON...
-0000c2a0: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
-0000c2b0: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
-0000c2c0: 6175 6c74 0700 0000 0d51 7363 694c 6578  ault.....QsciLex
-0000c2d0: 6572 4a53 4f4e 0103 0000 001c 0045 0073  erJSON.......E.s
-0000c2e0: 0063 0061 0070 0065 002d 0053 0065 0071  .c.a.p.e.-.S.e.q
-0000c2f0: 0075 0065 006e 007a 0800 0000 0006 0000  .u.e.n.z........
-0000c300: 000f 4573 6361 7065 2073 6571 7565 6e63  ..Escape sequenc
-0000c310: 6507 0000 000d 5173 6369 4c65 7865 724a  e.....QsciLexerJ
-0000c320: 534f 4e01 0300 0000 0600 4900 5200 4908  SON.......I.R.I.
-0000c330: 0000 0000 0600 0000 0349 5249 0700 0000  .........IRI....
-0000c340: 0d51 7363 694c 6578 6572 4a53 4f4e 0103  .QsciLexerJSON..
-0000c350: 0000 0024 004a 0053 004f 004e 0020 0053  ...$.J.S.O.N. .S
-0000c360: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
-0000c370: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
-0000c380: 000c 4a53 4f4e 206b 6579 776f 7264 0700  ..JSON keyword..
-0000c390: 0000 0d51 7363 694c 6578 6572 4a53 4f4e  ...QsciLexerJSON
-0000c3a0: 0103 0000 002a 004a 0053 004f 004e 002d  .....*.J.S.O.N.-
-0000c3b0: 004c 0044 0020 006b 006f 006d 0070 0061  .L.D. .k.o.m.p.a
-0000c3c0: 006b 0074 0065 0073 0020 0049 0052 0049  .k.t.e.s. .I.R.I
-0000c3d0: 0800 0000 0006 0000 0013 4a53 4f4e 2d4c  ..........JSON-L
-0000c3e0: 4420 636f 6d70 6163 7420 4952 4907 0000  D compact IRI...
-0000c3f0: 000d 5173 6369 4c65 7865 724a 534f 4e01  ..QsciLexerJSON.
-0000c400: 0300 0000 2a00 4a00 5300 4f00 4e00 2d00  ....*.J.S.O.N.-.
-0000c410: 4c00 4400 2000 5300 6300 6800 6c00 fc00  L.D. .S.c.h.l...
-0000c420: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
-0000c430: 0000 0000 0600 0000 0f4a 534f 4e2d 4c44  .........JSON-LD
-0000c440: 206b 6579 776f 7264 0700 0000 0d51 7363   keyword.....Qsc
-0000c450: 694c 6578 6572 4a53 4f4e 0103 0000 001e  iLexerJSON......
-0000c460: 005a 0065 0069 006c 0065 006e 006b 006f  .Z.e.i.l.e.n.k.o
-0000c470: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-0000c480: 0000 0006 0000 000c 4c69 6e65 2063 6f6d  ........Line com
-0000c490: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
-0000c4a0: 6572 4a53 4f4e 0103 0000 0008 005a 0061  erJSON.......Z.a
-0000c4b0: 0068 006c 0800 0000 0006 0000 0006 4e75  .h.l..........Nu
-0000c4c0: 6d62 6572 0700 0000 0d51 7363 694c 6578  mber.....QsciLex
-0000c4d0: 6572 4a53 4f4e 0103 0000 0010 004f 0070  erJSON.......O.p
-0000c4e0: 0065 0072 0061 0074 006f 0072 0800 0000  .e.r.a.t.o.r....
-0000c4f0: 0006 0000 0008 4f70 6572 6174 6f72 0700  ......Operator..
-0000c500: 0000 0d51 7363 694c 6578 6572 4a53 4f4e  ...QsciLexerJSON
-0000c510: 0103 0000 001a 0041 006e 0061 006c 0079  .......A.n.a.l.y
-0000c520: 0073 0065 0066 0065 0068 006c 0065 0072  .s.e.f.e.h.l.e.r
-0000c530: 0800 0000 0006 0000 000d 5061 7273 696e  ..........Parsin
-0000c540: 6720 6572 726f 7207 0000 000d 5173 6369  g error.....Qsci
-0000c550: 4c65 7865 724a 534f 4e01 0300 0000 1600  LexerJSON.......
-0000c560: 4500 6900 6700 6500 6e00 7300 6300 6800  E.i.g.e.n.s.c.h.
-0000c570: 6100 6600 7408 0000 0000 0600 0000 0850  a.f.t..........P
-0000c580: 726f 7065 7274 7907 0000 000d 5173 6369  roperty.....Qsci
-0000c590: 4c65 7865 724a 534f 4e01 0300 0000 1800  LexerJSON.......
-0000c5a0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
-0000c5b0: 6500 7400 7400 6508 0000 0000 0600 0000  e.t.t.e.........
-0000c5c0: 0653 7472 696e 6707 0000 000d 5173 6369  .String.....Qsci
-0000c5d0: 4c65 7865 724a 534f 4e01 0300 0000 2e00  LexerJSON.......
-0000c5e0: 5500 6e00 6200 6500 6500 6e00 6400 6500  U.n.b.e.e.n.d.e.
-0000c5f0: 7400 6500 2000 5a00 6500 6900 6300 6800  t.e. .Z.e.i.c.h.
-0000c600: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
-0000c610: 0000 0600 0000 0f55 6e63 6c6f 7365 6420  .......Unclosed 
-0000c620: 7374 7269 6e67 0700 0000 0d51 7363 694c  string.....QsciL
-0000c630: 6578 6572 4a53 4f4e 0103 0000 0024 0052  exerJSON.....$.R
-0000c640: 0065 0067 0075 006c 00e4 0072 0065 0072  .e.g.u.l...r.e.r
-0000c650: 0020 0041 0075 0073 0064 0072 0075 0063  . .A.u.s.d.r.u.c
-0000c660: 006b 0800 0000 0006 0000 0012 5265 6775  .k..........Regu
-0000c670: 6c61 7220 6578 7072 6573 7369 6f6e 0700  lar expression..
-0000c680: 0000 1351 7363 694c 6578 6572 4a61 7661  ...QsciLexerJava
-0000c690: 5363 7269 7074 0103 0000 001e 0042 0061  Script.......B.a
-0000c6a0: 0073 0069 0073 0066 0075 006e 006b 0074  .s.i.s.f.u.n.k.t
-0000c6b0: 0069 006f 006e 0065 006e 0800 0000 0006  .i.o.n.e.n......
-0000c6c0: 0000 000f 4261 7369 6320 6675 6e63 7469  ....Basic functi
-0000c6d0: 6f6e 7307 0000 000c 5173 6369 4c65 7865  ons.....QsciLexe
-0000c6e0: 724c 7561 0103 0000 000e 005a 0065 0069  rLua.......Z.e.i
-0000c6f0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-0000c700: 0009 4368 6172 6163 7465 7207 0000 000c  ..Character.....
-0000c710: 5173 6369 4c65 7865 724c 7561 0103 0000  QsciLexerLua....
-0000c720: 0012 004b 006f 006d 006d 0065 006e 0074  ...K.o.m.m.e.n.t
-0000c730: 0061 0072 0800 0000 0006 0000 0007 436f  .a.r..........Co
-0000c740: 6d6d 656e 7407 0000 000c 5173 6369 4c65  mment.....QsciLe
-0000c750: 7865 724c 7561 0103 0000 004a 004b 006f  xerLua.....J.K.o
-0000c760: 0072 006f 0075 0074 0069 006e 0065 006e  .r.o.u.t.i.n.e.n
-0000c770: 002c 0020 0049 002f 004f 002d 0020 0075  .,. .I./.O.-. .u
-0000c780: 006e 0064 0020 0053 0079 0073 0074 0065  .n.d. .S.y.s.t.e
-0000c790: 006d 0066 0075 006e 006b 0074 0069 006f  .m.f.u.n.k.t.i.o
-0000c7a0: 006e 0065 006e 0800 0000 0006 0000 0025  .n.e.n.........%
-0000c7b0: 436f 726f 7574 696e 6573 2c20 692f 6f20  Coroutines, i/o 
-0000c7c0: 616e 6420 7379 7374 656d 2066 6163 696c  and system facil
-0000c7d0: 6974 6965 7307 0000 000c 5173 6369 4c65  ities.....QsciLe
-0000c7e0: 7865 724c 7561 0103 0000 0010 0053 0074  xerLua.......S.t
-0000c7f0: 0061 006e 0064 0061 0072 0064 0800 0000  .a.n.d.a.r.d....
-0000c800: 0006 0000 0007 4465 6661 756c 7407 0000  ......Default...
-0000c810: 000c 5173 6369 4c65 7865 724c 7561 0103  ..QsciLexerLua..
-0000c820: 0000 0014 0042 0065 007a 0065 0069 0063  .....B.e.z.e.i.c
-0000c830: 0068 006e 0065 0072 0800 0000 0006 0000  .h.n.e.r........
-0000c840: 000a 4964 656e 7469 6669 6572 0700 0000  ..Identifier....
-0000c850: 0c51 7363 694c 6578 6572 4c75 6101 0300  .QsciLexerLua...
-0000c860: 0000 1a00 5300 6300 6800 6c00 fc00 7300  ....S.c.h.l...s.
-0000c870: 7300 6500 6c00 7700 6f00 7200 7408 0000  s.e.l.w.o.r.t...
-0000c880: 0000 0600 0000 074b 6579 776f 7264 0700  .......Keyword..
-0000c890: 0000 0c51 7363 694c 6578 6572 4c75 6101  ...QsciLexerLua.
-0000c8a0: 0300 0000 0a00 4d00 6100 7200 6b00 6508  ......M.a.r.k.e.
-0000c8b0: 0000 0000 0600 0000 054c 6162 656c 0700  .........Label..
-0000c8c0: 0000 0c51 7363 694c 6578 6572 4c75 6101  ...QsciLexerLua.
-0000c8d0: 0300 0000 1e00 5a00 6500 6900 6c00 6500  ......Z.e.i.l.e.
-0000c8e0: 6e00 6b00 6f00 6d00 6d00 6500 6e00 7400  n.k.o.m.m.e.n.t.
-0000c8f0: 6100 7208 0000 0000 0600 0000 0c4c 696e  a.r..........Lin
-0000c900: 6520 636f 6d6d 656e 7407 0000 000c 5173  e comment.....Qs
-0000c910: 6369 4c65 7865 724c 7561 0103 0000 003a  ciLexerLua.....:
-0000c920: 0055 006e 0069 006e 0074 0065 0072 0070  .U.n.i.n.t.e.r.p
-0000c930: 0072 0065 0074 0069 0065 0072 0074 0065  .r.e.t.i.e.r.t.e
-0000c940: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-0000c950: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
-0000c960: 0000 000e 4c69 7465 7261 6c20 7374 7269  ....Literal stri
-0000c970: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
-0000c980: 4c75 6101 0300 0000 0800 5a00 6100 6800  Lua.......Z.a.h.
-0000c990: 6c08 0000 0000 0600 0000 064e 756d 6265  l..........Numbe
-0000c9a0: 7207 0000 000c 5173 6369 4c65 7865 724c  r.....QsciLexerL
-0000c9b0: 7561 0103 0000 0010 004f 0070 0065 0072  ua.......O.p.e.r
-0000c9c0: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
-0000c9d0: 0008 4f70 6572 6174 6f72 0700 0000 0c51  ..Operator.....Q
-0000c9e0: 7363 694c 6578 6572 4c75 6101 0300 0000  sciLexerLua.....
-0000c9f0: 1800 5000 7200 e400 7000 7200 6f00 7a00  ..P.r...p.r.o.z.
-0000ca00: 6500 7300 7300 6f00 7208 0000 0000 0600  e.s.s.o.r.......
-0000ca10: 0000 0c50 7265 7072 6f63 6573 736f 7207  ...Preprocessor.
-0000ca20: 0000 000c 5173 6369 4c65 7865 724c 7561  ....QsciLexerLua
-0000ca30: 0103 0000 0018 005a 0065 0069 0063 0068  .......Z.e.i.c.h
-0000ca40: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
-0000ca50: 0000 0006 0000 0006 5374 7269 6e67 0700  ........String..
-0000ca60: 0000 0c51 7363 694c 6578 6572 4c75 6101  ...QsciLexerLua.
-0000ca70: 0300 0000 6a00 5a00 6500 6900 6300 6800  ....j.Z.e.i.c.h.
-0000ca80: 6500 6e00 6b00 6500 7400 7400 6500 6e00  e.n.k.e.t.t.e.n.
-0000ca90: 2d00 2c00 2000 5400 6100 6200 6500 6c00  -.,. .T.a.b.e.l.
-0000caa0: 6c00 6500 2d00 2000 7500 6e00 6400 2000  l.e.-. .u.n.d. .
-0000cab0: 6d00 6100 7400 6800 6500 6d00 6100 7400  m.a.t.h.e.m.a.t.
-0000cac0: 6900 7300 6300 6800 6500 2000 4600 7500  i.s.c.h.e. .F.u.
-0000cad0: 6e00 6b00 7400 6900 6f00 6e00 6500 6e08  n.k.t.i.o.n.e.n.
-0000cae0: 0000 0000 0600 0000 2153 7472 696e 672c  ........!String,
-0000caf0: 2074 6162 6c65 2061 6e64 206d 6174 6873   table and maths
-0000cb00: 2066 756e 6374 696f 6e73 0700 0000 0c51   functions.....Q
-0000cb10: 7363 694c 6578 6572 4c75 6101 0300 0000  sciLexerLua.....
-0000cb20: 2e00 5500 6e00 6200 6500 6500 6e00 6400  ..U.n.b.e.e.n.d.
-0000cb30: 6500 7400 6500 2000 5a00 6500 6900 6300  e.t.e. .Z.e.i.c.
-0000cb40: 6800 6500 6e00 6b00 6500 7400 7400 6508  h.e.n.k.e.t.t.e.
-0000cb50: 0000 0000 0600 0000 0f55 6e63 6c6f 7365  .........Unclose
-0000cb60: 6420 7374 7269 6e67 0700 0000 0c51 7363  d string.....Qsc
-0000cb70: 694c 6578 6572 4c75 6101 0300 0000 2400  iLexerLua.....$.
-0000cb80: 4e00 7500 7400 7a00 6500 7200 2000 6400  N.u.t.z.e.r. .d.
-0000cb90: 6500 6600 6900 6e00 6900 6500 7200 7400  e.f.i.n.i.e.r.t.
-0000cba0: 2000 3108 0000 0000 0600 0000 0e55 7365   .1..........Use
-0000cbb0: 7220 6465 6669 6e65 6420 3107 0000 000c  r defined 1.....
-0000cbc0: 5173 6369 4c65 7865 724c 7561 0103 0000  QsciLexerLua....
-0000cbd0: 0024 004e 0075 0074 007a 0065 0072 0020  .$.N.u.t.z.e.r. 
-0000cbe0: 0064 0065 0066 0069 006e 0069 0065 0072  .d.e.f.i.n.i.e.r
-0000cbf0: 0074 0020 0032 0800 0000 0006 0000 000e  .t. .2..........
-0000cc00: 5573 6572 2064 6566 696e 6564 2032 0700  User defined 2..
-0000cc10: 0000 0c51 7363 694c 6578 6572 4c75 6101  ...QsciLexerLua.
-0000cc20: 0300 0000 2400 4e00 7500 7400 7a00 6500  ....$.N.u.t.z.e.
-0000cc30: 7200 2000 6400 6500 6600 6900 6e00 6900  r. .d.e.f.i.n.i.
-0000cc40: 6500 7200 7400 2000 3308 0000 0000 0600  e.r.t. .3.......
-0000cc50: 0000 0e55 7365 7220 6465 6669 6e65 6420  ...User defined 
-0000cc60: 3307 0000 000c 5173 6369 4c65 7865 724c  3.....QsciLexerL
-0000cc70: 7561 0103 0000 0024 004e 0075 0074 007a  ua.....$.N.u.t.z
-0000cc80: 0065 0072 0020 0064 0065 0066 0069 006e  .e.r. .d.e.f.i.n
-0000cc90: 0069 0065 0072 0074 0020 0034 0800 0000  .i.e.r.t. .4....
-0000cca0: 0006 0000 000e 5573 6572 2064 6566 696e  ......User defin
-0000ccb0: 6564 2034 0700 0000 0c51 7363 694c 6578  ed 4.....QsciLex
-0000ccc0: 6572 4c75 6101 0300 0000 1200 4b00 6f00  erLua.......K.o.
-0000ccd0: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
-0000cce0: 0000 0600 0000 0743 6f6d 6d65 6e74 0700  .......Comment..
-0000ccf0: 0000 1151 7363 694c 6578 6572 4d61 6b65  ...QsciLexerMake
-0000cd00: 6669 6c65 0103 0000 0010 0053 0074 0061  file.......S.t.a
-0000cd10: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
-0000cd20: 0000 0007 4465 6661 756c 7407 0000 0011  ....Default.....
-0000cd30: 5173 6369 4c65 7865 724d 616b 6566 696c  QsciLexerMakefil
-0000cd40: 6501 0300 0000 0c00 4600 6500 6800 6c00  e.......F.e.h.l.
-0000cd50: 6500 7208 0000 0000 0600 0000 0545 7272  e.r..........Err
-0000cd60: 6f72 0700 0000 1151 7363 694c 6578 6572  or.....QsciLexer
-0000cd70: 4d61 6b65 6669 6c65 0103 0000 0010 004f  Makefile.......O
-0000cd80: 0070 0065 0072 0061 0074 006f 0072 0800  .p.e.r.a.t.o.r..
-0000cd90: 0000 0006 0000 0008 4f70 6572 6174 6f72  ........Operator
-0000cda0: 0700 0000 1151 7363 694c 6578 6572 4d61  .....QsciLexerMa
-0000cdb0: 6b65 6669 6c65 0103 0000 0018 0050 0072  kefile.......P.r
-0000cdc0: 00e4 0070 0072 006f 007a 0065 0073 0073  ...p.r.o.z.e.s.s
-0000cdd0: 006f 0072 0800 0000 0006 0000 000c 5072  .o.r..........Pr
-0000cde0: 6570 726f 6365 7373 6f72 0700 0000 1151  eprocessor.....Q
-0000cdf0: 7363 694c 6578 6572 4d61 6b65 6669 6c65  sciLexerMakefile
-0000ce00: 0103 0000 0008 005a 0069 0065 006c 0800  .......Z.i.e.l..
-0000ce10: 0000 0006 0000 0006 5461 7267 6574 0700  ........Target..
-0000ce20: 0000 1151 7363 694c 6578 6572 4d61 6b65  ...QsciLexerMake
-0000ce30: 6669 6c65 0103 0000 0010 0056 0061 0072  file.......V.a.r
-0000ce40: 0069 0061 0062 006c 0065 0800 0000 0006  .i.a.b.l.e......
-0000ce50: 0000 0008 5661 7269 6162 6c65 0700 0000  ....Variable....
-0000ce60: 1151 7363 694c 6578 6572 4d61 6b65 6669  .QsciLexerMakefi
-0000ce70: 6c65 0103 0000 0014 0042 006c 006f 0063  le.......B.l.o.c
-0000ce80: 006b 007a 0069 0074 0061 0074 0800 0000  .k.z.i.t.a.t....
-0000ce90: 0006 0000 000b 426c 6f63 6b20 7175 6f74  ......Block quot
-0000cea0: 6507 0000 0011 5173 6369 4c65 7865 724d  e.....QsciLexerM
-0000ceb0: 6172 6b64 6f77 6e01 0300 0000 2e00 4300  arkdown.......C.
-0000cec0: 6f00 6400 6500 2000 7a00 7700 6900 7300  o.d.e. .z.w.i.s.
-0000ced0: 6300 6800 6500 6e00 2000 4200 6100 6300  c.h.e.n. .B.a.c.
-0000cee0: 6b00 7400 6900 6300 6b00 7308 0000 0000  k.t.i.c.k.s.....
-0000cef0: 0600 0000 1643 6f64 6520 6265 7477 6565  .....Code betwee
-0000cf00: 6e20 6261 636b 7469 636b 7307 0000 0011  n backticks.....
-0000cf10: 5173 6369 4c65 7865 724d 6172 6b64 6f77  QsciLexerMarkdow
-0000cf20: 6e01 0300 0000 4200 4300 6f00 6400 6500  n.....B.C.o.d.e.
-0000cf30: 2000 7a00 7700 6900 7300 6300 6800 6500   .z.w.i.s.c.h.e.
-0000cf40: 6e00 2000 6400 6f00 7000 7000 6500 6c00  n. .d.o.p.p.e.l.
-0000cf50: 7400 6500 6e00 2000 4200 6100 6300 6b00  t.e.n. .B.a.c.k.
-0000cf60: 7400 6900 6300 6b00 7308 0000 0000 0600  t.i.c.k.s.......
-0000cf70: 0000 1d43 6f64 6520 6265 7477 6565 6e20  ...Code between 
-0000cf80: 646f 7562 6c65 2062 6163 6b74 6963 6b73  double backticks
-0000cf90: 0700 0000 1151 7363 694c 6578 6572 4d61  .....QsciLexerMa
-0000cfa0: 726b 646f 776e 0103 0000 0012 0043 006f  rkdown.......C.o
-0000cfb0: 0064 0065 0062 006c 006f 0063 006b 0800  .d.e.b.l.o.c.k..
-0000cfc0: 0000 0006 0000 000a 436f 6465 2062 6c6f  ........Code blo
-0000cfd0: 636b 0700 0000 1151 7363 694c 6578 6572  ck.....QsciLexer
-0000cfe0: 4d61 726b 646f 776e 0103 0000 0010 0053  Markdown.......S
-0000cff0: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
-0000d000: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
-0000d010: 0000 0011 5173 6369 4c65 7865 724d 6172  ....QsciLexerMar
-0000d020: 6b64 6f77 6e01 0300 0000 4a00 4b00 7500  kdown.....J.K.u.
-0000d030: 7200 7300 6900 7600 6500 2000 5300 6300  r.s.i.v.e. .S.c.
-0000d040: 6800 7200 6900 6600 7400 2000 6d00 6900  h.r.i.f.t. .m.i.
-0000d050: 7400 2000 6500 6900 6e00 6600 6100 6300  t. .e.i.n.f.a.c.
-0000d060: 6800 6500 6e00 2000 5300 7400 6500 7200  h.e.n. .S.t.e.r.
-0000d070: 6e00 6500 6e08 0000 0000 0600 0000 1f45  n.e.n..........E
-0000d080: 6d70 6861 7369 7320 7573 696e 6720 7369  mphasis using si
-0000d090: 6e67 6c65 2061 7374 6572 6973 6b73 0700  ngle asterisks..
-0000d0a0: 0000 1151 7363 694c 6578 6572 4d61 726b  ...QsciLexerMark
-0000d0b0: 646f 776e 0103 0000 0056 004b 0075 0072  down.....V.K.u.r
-0000d0c0: 0073 0069 0076 0065 0020 0053 0063 0068  .s.i.v.e. .S.c.h
-0000d0d0: 0072 0069 0066 0074 0020 006d 0069 0074  .r.i.f.t. .m.i.t
-0000d0e0: 0020 0065 0069 006e 0066 0061 0063 0068  . .e.i.n.f.a.c.h
-0000d0f0: 0065 006e 0020 0055 006e 0074 0065 0072  .e.n. .U.n.t.e.r
-0000d100: 0073 0074 0072 0069 0063 0068 0065 006e  .s.t.r.i.c.h.e.n
-0000d110: 0800 0000 0006 0000 0021 456d 7068 6173  .........!Emphas
-0000d120: 6973 2075 7369 6e67 2073 696e 676c 6520  is using single 
-0000d130: 756e 6465 7273 636f 7265 7307 0000 0011  underscores.....
-0000d140: 5173 6369 4c65 7865 724d 6172 6b64 6f77  QsciLexerMarkdow
-0000d150: 6e01 0300 0000 2200 4800 6f00 7200 6900  n.....".H.o.r.i.
-0000d160: 7a00 6f00 6e00 7400 6100 6c00 6500 2000  z.o.n.t.a.l.e. .
-0000d170: 4c00 6900 6e00 6900 6508 0000 0000 0600  L.i.n.i.e.......
-0000d180: 0000 0f48 6f72 697a 6f6e 7461 6c20 7275  ...Horizontal ru
-0000d190: 6c65 0700 0000 1151 7363 694c 6578 6572  le.....QsciLexer
-0000d1a0: 4d61 726b 646f 776e 0103 0000 0026 00dc  Markdown.....&..
-0000d1b0: 0062 0065 0072 0073 0063 0068 0072 0069  .b.e.r.s.c.h.r.i
-0000d1c0: 0066 0074 0020 0045 0062 0065 006e 0065  .f.t. .E.b.e.n.e
-0000d1d0: 0020 0031 0800 0000 0006 0000 000e 4c65  . .1..........Le
-0000d1e0: 7665 6c20 3120 6865 6164 6572 0700 0000  vel 1 header....
-0000d1f0: 1151 7363 694c 6578 6572 4d61 726b 646f  .QsciLexerMarkdo
-0000d200: 776e 0103 0000 0026 00dc 0062 0065 0072  wn.....&...b.e.r
-0000d210: 0073 0063 0068 0072 0069 0066 0074 0020  .s.c.h.r.i.f.t. 
-0000d220: 0045 0062 0065 006e 0065 0020 0032 0800  .E.b.e.n.e. .2..
-0000d230: 0000 0006 0000 000e 4c65 7665 6c20 3220  ........Level 2 
-0000d240: 6865 6164 6572 0700 0000 1151 7363 694c  header.....QsciL
-0000d250: 6578 6572 4d61 726b 646f 776e 0103 0000  exerMarkdown....
-0000d260: 0026 00dc 0062 0065 0072 0073 0063 0068  .&...b.e.r.s.c.h
-0000d270: 0072 0069 0066 0074 0020 0045 0062 0065  .r.i.f.t. .E.b.e
-0000d280: 006e 0065 0020 0033 0800 0000 0006 0000  .n.e. .3........
-0000d290: 000e 4c65 7665 6c20 3320 6865 6164 6572  ..Level 3 header
-0000d2a0: 0700 0000 1151 7363 694c 6578 6572 4d61  .....QsciLexerMa
-0000d2b0: 726b 646f 776e 0103 0000 0026 00dc 0062  rkdown.....&...b
-0000d2c0: 0065 0072 0073 0063 0068 0072 0069 0066  .e.r.s.c.h.r.i.f
-0000d2d0: 0074 0020 0045 0062 0065 006e 0065 0020  .t. .E.b.e.n.e. 
-0000d2e0: 0034 0800 0000 0006 0000 000e 4c65 7665  .4..........Leve
-0000d2f0: 6c20 3420 6865 6164 6572 0700 0000 1151  l 4 header.....Q
-0000d300: 7363 694c 6578 6572 4d61 726b 646f 776e  sciLexerMarkdown
-0000d310: 0103 0000 0026 00dc 0062 0065 0072 0073  .....&...b.e.r.s
-0000d320: 0063 0068 0072 0069 0066 0074 0020 0045  .c.h.r.i.f.t. .E
-0000d330: 0062 0065 006e 0065 0020 0035 0800 0000  .b.e.n.e. .5....
-0000d340: 0006 0000 000e 4c65 7665 6c20 3520 6865  ......Level 5 he
-0000d350: 6164 6572 0700 0000 1151 7363 694c 6578  ader.....QsciLex
-0000d360: 6572 4d61 726b 646f 776e 0103 0000 0026  erMarkdown.....&
-0000d370: 00dc 0062 0065 0072 0073 0063 0068 0072  ...b.e.r.s.c.h.r
-0000d380: 0069 0066 0074 0020 0045 0062 0065 006e  .i.f.t. .E.b.e.n
-0000d390: 0065 0020 0036 0800 0000 0006 0000 000e  .e. .6..........
-0000d3a0: 4c65 7665 6c20 3620 6865 6164 6572 0700  Level 6 header..
-0000d3b0: 0000 1151 7363 694c 6578 6572 4d61 726b  ...QsciLexerMark
-0000d3c0: 646f 776e 0103 0000 0012 0048 0079 0070  down.......H.y.p
-0000d3d0: 0065 0072 006c 0069 006e 006b 0800 0000  .e.r.l.i.n.k....
-0000d3e0: 0006 0000 0004 4c69 6e6b 0700 0000 1151  ......Link.....Q
-0000d3f0: 7363 694c 6578 6572 4d61 726b 646f 776e  sciLexerMarkdown
-0000d400: 0103 0000 0034 004e 0075 006d 006d 0065  .....4.N.u.m.m.e
-0000d410: 0072 0069 0065 0072 0074 0065 0073 0020  .r.i.e.r.t.e.s. 
-0000d420: 004c 0069 0073 0074 0065 006e 0065 006c  .L.i.s.t.e.n.e.l
-0000d430: 0065 006d 0065 006e 0074 0800 0000 0006  .e.m.e.n.t......
-0000d440: 0000 0011 4f72 6465 7265 6420 6c69 7374  ....Ordered list
-0000d450: 2069 7465 6d07 0000 0011 5173 6369 4c65   item.....QsciLe
-0000d460: 7865 724d 6172 6b64 6f77 6e01 0300 0000  xerMarkdown.....
-0000d470: 2400 4500 6900 6e00 6c00 6500 6900 7400  $.E.i.n.l.e.i.t.
-0000d480: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
-0000d490: 6800 6500 6e08 0000 0000 0600 0000 0850  h.e.n..........P
-0000d4a0: 7265 2d63 6861 7207 0000 0011 5173 6369  re-char.....Qsci
-0000d4b0: 4c65 7865 724d 6172 6b64 6f77 6e01 0300  LexerMarkdown...
-0000d4c0: 0000 0e00 5300 7000 6500 7a00 6900 6100  ....S.p.e.z.i.a.
-0000d4d0: 6c08 0000 0000 0600 0000 0753 7065 6369  l..........Speci
-0000d4e0: 616c 0700 0000 1151 7363 694c 6578 6572  al.....QsciLexer
-0000d4f0: 4d61 726b 646f 776e 0103 0000 001e 0044  Markdown.......D
-0000d500: 0075 0072 0063 0068 0067 0065 0073 0074  .u.r.c.h.g.e.s.t
-0000d510: 0072 0069 0063 0068 0065 006e 0800 0000  .r.i.c.h.e.n....
-0000d520: 0006 0000 000a 5374 7269 6b65 206f 7574  ......Strike out
-0000d530: 0700 0000 1151 7363 694c 6578 6572 4d61  .....QsciLexerMa
-0000d540: 726b 646f 776e 0103 0000 0042 0046 0065  rkdown.....B.F.e
-0000d550: 0074 0074 0073 0063 0068 0072 0069 0066  .t.t.s.c.h.r.i.f
-0000d560: 0074 0020 006d 0069 0074 0020 0064 006f  .t. .m.i.t. .d.o
-0000d570: 0070 0070 0065 006c 0074 0065 006e 0020  .p.p.e.l.t.e.n. 
-0000d580: 0053 0074 0065 0072 006e 0065 006e 0800  .S.t.e.r.n.e.n..
-0000d590: 0000 0006 0000 0026 5374 726f 6e67 2065  .......&Strong e
-0000d5a0: 6d70 6861 7369 7320 7573 696e 6720 646f  mphasis using do
-0000d5b0: 7562 6c65 2061 7374 6572 6973 6b73 0700  uble asterisks..
-0000d5c0: 0000 1151 7363 694c 6578 6572 4d61 726b  ...QsciLexerMark
-0000d5d0: 646f 776e 0103 0000 004e 0046 0065 0074  down.....N.F.e.t
-0000d5e0: 0074 0073 0063 0068 0072 0069 0066 0074  .t.s.c.h.r.i.f.t
-0000d5f0: 0020 006d 0069 0074 0020 0064 006f 0070  . .m.i.t. .d.o.p
-0000d600: 0070 0065 006c 0074 0065 006e 0020 0055  .p.e.l.t.e.n. .U
-0000d610: 006e 0074 0065 0072 0073 0074 0072 0069  .n.t.e.r.s.t.r.i
-0000d620: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
-0000d630: 0028 5374 726f 6e67 2065 6d70 6861 7369  .(Strong emphasi
-0000d640: 7320 7573 696e 6720 646f 7562 6c65 2075  s using double u
-0000d650: 6e64 6572 7363 6f72 6573 0700 0000 1151  nderscores.....Q
-0000d660: 7363 694c 6578 6572 4d61 726b 646f 776e  sciLexerMarkdown
-0000d670: 0103 0000 0040 004e 0069 0063 0068 0074  .....@.N.i.c.h.t
-0000d680: 0020 006e 0075 006d 006d 0065 0072 0069  . .n.u.m.m.e.r.i
-0000d690: 0065 0072 0074 0065 0073 0020 004c 0069  .e.r.t.e.s. .L.i
-0000d6a0: 0073 0074 0065 006e 0065 006c 0065 006d  .s.t.e.n.e.l.e.m
-0000d6b0: 0065 006e 0074 0800 0000 0006 0000 0013  .e.n.t..........
-0000d6c0: 556e 6f72 6465 7265 6420 6c69 7374 2069  Unordered list i
-0000d6d0: 7465 6d07 0000 0011 5173 6369 4c65 7865  tem.....QsciLexe
-0000d6e0: 724d 6172 6b64 6f77 6e01 0300 0000 0c00  rMarkdown.......
-0000d6f0: 4200 6500 6600 6500 6800 6c08 0000 0000  B.e.f.e.h.l.....
-0000d700: 0600 0000 0743 6f6d 6d61 6e64 0700 0000  .....Command....
-0000d710: 0f51 7363 694c 6578 6572 4d61 746c 6162  .QsciLexerMatlab
-0000d720: 0103 0000 0012 004b 006f 006d 006d 0065  .......K.o.m.m.e
-0000d730: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
-0000d740: 0007 436f 6d6d 656e 7407 0000 000f 5173  ..Comment.....Qs
-0000d750: 6369 4c65 7865 724d 6174 6c61 6201 0300  ciLexerMatlab...
-0000d760: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
-0000d770: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
-0000d780: 6175 6c74 0700 0000 0f51 7363 694c 6578  ault.....QsciLex
-0000d790: 6572 4d61 746c 6162 0103 0000 0042 005a  erMatlab.....B.Z
-0000d7a0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-0000d7b0: 0074 0074 0065 0020 0069 006e 0020 0041  .t.t.e. .i.n. .A
-0000d7c0: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
-0000d7d0: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
-0000d7e0: 0800 0000 0006 0000 0014 446f 7562 6c65  ..........Double
-0000d7f0: 2d71 756f 7465 6420 7374 7269 6e67 0700  -quoted string..
-0000d800: 0000 0f51 7363 694c 6578 6572 4d61 746c  ...QsciLexerMatl
-0000d810: 6162 0103 0000 0014 0042 0065 007a 0065  ab.......B.e.z.e
-0000d820: 0069 0063 0068 006e 0065 0072 0800 0000  .i.c.h.n.e.r....
-0000d830: 0006 0000 000a 4964 656e 7469 6669 6572  ......Identifier
-0000d840: 0700 0000 0f51 7363 694c 6578 6572 4d61  .....QsciLexerMa
-0000d850: 746c 6162 0103 0000 001a 0053 0063 0068  tlab.......S.c.h
-0000d860: 006c 00fc 0073 0073 0065 006c 0077 006f  .l...s.s.e.l.w.o
-0000d870: 0072 0074 0800 0000 0006 0000 0007 4b65  .r.t..........Ke
-0000d880: 7977 6f72 6407 0000 000f 5173 6369 4c65  yword.....QsciLe
-0000d890: 7865 724d 6174 6c61 6201 0300 0000 0800  xerMatlab.......
-0000d8a0: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
-0000d8b0: 064e 756d 6265 7207 0000 000f 5173 6369  .Number.....Qsci
-0000d8c0: 4c65 7865 724d 6174 6c61 6201 0300 0000  LexerMatlab.....
-0000d8d0: 1000 4f00 7000 6500 7200 6100 7400 6f00  ..O.p.e.r.a.t.o.
-0000d8e0: 7208 0000 0000 0600 0000 084f 7065 7261  r..........Opera
-0000d8f0: 746f 7207 0000 000f 5173 6369 4c65 7865  tor.....QsciLexe
-0000d900: 724d 6174 6c61 6201 0300 0000 3600 5a00  rMatlab.....6.Z.
-0000d910: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-0000d920: 7400 7400 6500 2000 6900 6e00 2000 4800  t.t.e. .i.n. .H.
-0000d930: 6f00 6300 6800 6b00 6f00 6d00 6d00 6100  o.c.h.k.o.m.m.a.
-0000d940: 7400 6108 0000 0000 0600 0000 1453 696e  t.a..........Sin
-0000d950: 676c 652d 7175 6f74 6564 2073 7472 696e  gle-quoted strin
-0000d960: 6707 0000 000f 5173 6369 4c65 7865 724d  g.....QsciLexerM
-0000d970: 6174 6c61 6201 0300 0000 1200 4b00 6f00  atlab.......K.o.
-0000d980: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
-0000d990: 0000 0600 0000 0743 6f6d 6d65 6e74 0700  .......Comment..
-0000d9a0: 0000 0b51 7363 694c 6578 6572 504f 0103  ...QsciLexerPO..
-0000d9b0: 0000 0010 0053 0074 0061 006e 0064 0061  .....S.t.a.n.d.a
-0000d9c0: 0072 0064 0800 0000 0006 0000 0007 4465  .r.d..........De
-0000d9d0: 6661 756c 7407 0000 000b 5173 6369 4c65  fault.....QsciLe
-0000d9e0: 7865 7250 4f01 0300 0000 1400 4d00 6100  xerPO.......M.a.
-0000d9f0: 7200 6b00 6900 6500 7200 7500 6e00 6708  r.k.i.e.r.u.n.g.
-0000da00: 0000 0000 0600 0000 0546 6c61 6773 0700  .........Flags..
-0000da10: 0000 0b51 7363 694c 6578 6572 504f 0103  ...QsciLexerPO..
-0000da20: 0000 0022 0055 006e 0073 0063 0068 0072  ...".U.n.s.c.h.r
-0000da30: 0066 006d 0061 0072 006b 0069 0065 0072  .f.m.a.r.k.i.e.r
-0000da40: 0075 006e 0067 0800 0000 0006 0000 000a  .u.n.g..........
-0000da50: 4675 7a7a 7920 666c 6167 0700 0000 0b51  Fuzzy flag.....Q
-0000da60: 7363 694c 6578 6572 504f 0103 0000 001e  sciLexerPO......
-0000da70: 004d 0065 006c 0064 0075 006e 0067 0073  .M.e.l.d.u.n.g.s
-0000da80: 006b 006f 006e 0074 0065 0078 0074 0800  .k.o.n.t.e.x.t..
-0000da90: 0000 0006 0000 000f 4d65 7373 6167 6520  ........Message 
-0000daa0: 636f 6e74 6578 7407 0000 000b 5173 6369  context.....Qsci
-0000dab0: 4c65 7865 7250 4f01 0300 0000 2600 4d00  LexerPO.....&.M.
-0000dac0: 6500 6c00 6400 7500 6e00 6700 7300 6b00  e.l.d.u.n.g.s.k.
-0000dad0: 6f00 6e00 7400 6500 7800 7400 7400 6500  o.n.t.e.x.t.t.e.
-0000dae0: 7800 7408 0000 0000 0600 0000 144d 6573  x.t..........Mes
-0000daf0: 7361 6765 2063 6f6e 7465 7874 2074 6578  sage context tex
-0000db00: 7407 0000 000b 5173 6369 4c65 7865 7250  t.....QsciLexerP
-0000db10: 4f01 0300 0000 3c00 4d00 6500 6c00 6400  O.....<.M.e.l.d.
-0000db20: 7500 6e00 6700 7300 6b00 6f00 6e00 7400  u.n.g.s.k.o.n.t.
-0000db30: 6500 7800 7400 7400 6500 7800 7400 2000  e.x.t.t.e.x.t. .
-0000db40: 5a00 6500 6900 6c00 6500 6e00 6500 6e00  Z.e.i.l.e.n.e.n.
-0000db50: 6400 6508 0000 0000 0600 0000 204d 6573  d.e......... Mes
-0000db60: 7361 6765 2063 6f6e 7465 7874 2074 6578  sage context tex
-0000db70: 7420 656e 642d 6f66 2d6c 696e 6507 0000  t end-of-line...
-0000db80: 000b 5173 6369 4c65 7865 7250 4f01 0300  ..QsciLexerPO...
-0000db90: 0000 2400 4d00 6500 6c00 6400 7500 6e00  ..$.M.e.l.d.u.n.
-0000dba0: 6700 7300 6200 6500 7a00 6500 6900 6300  g.s.b.e.z.e.i.c.
-0000dbb0: 6800 6e00 6500 7208 0000 0000 0600 0000  h.n.e.r.........
-0000dbc0: 124d 6573 7361 6765 2069 6465 6e74 6966  .Message identif
-0000dbd0: 6965 7207 0000 000b 5173 6369 4c65 7865  ier.....QsciLexe
-0000dbe0: 7250 4f01 0300 0000 2c00 4d00 6500 6c00  rPO.....,.M.e.l.
-0000dbf0: 6400 7500 6e00 6700 7300 6200 6500 7a00  d.u.n.g.s.b.e.z.
-0000dc00: 6500 6900 6300 6800 6e00 6500 7200 7400  e.i.c.h.n.e.r.t.
-0000dc10: 6500 7800 7408 0000 0000 0600 0000 174d  e.x.t..........M
-0000dc20: 6573 7361 6765 2069 6465 6e74 6966 6965  essage identifie
-0000dc30: 7220 7465 7874 0700 0000 0b51 7363 694c  r text.....QsciL
-0000dc40: 6578 6572 504f 0103 0000 0042 004d 0065  exerPO.....B.M.e
-0000dc50: 006c 0064 0075 006e 0067 0073 0062 0065  .l.d.u.n.g.s.b.e
-0000dc60: 007a 0065 0069 0063 0068 006e 0065 0072  .z.e.i.c.h.n.e.r
-0000dc70: 0074 0065 0078 0074 0020 005a 0065 0069  .t.e.x.t. .Z.e.i
-0000dc80: 006c 0065 006e 0065 006e 0064 0065 0800  .l.e.n.e.n.d.e..
-0000dc90: 0000 0006 0000 0023 4d65 7373 6167 6520  .......#Message 
-0000dca0: 6964 656e 7469 6669 6572 2074 6578 7420  identifier text 
-0000dcb0: 656e 642d 6f66 2d6c 696e 6507 0000 000b  end-of-line.....
-0000dcc0: 5173 6369 4c65 7865 7250 4f01 0300 0000  QsciLexerPO.....
-0000dcd0: 2800 4d00 6500 6c00 6400 7500 6e00 6700  (.M.e.l.d.u.n.g.
-0000dce0: 7300 7a00 6500 6900 6300 6800 6500 6e00  s.z.e.i.c.h.e.n.
-0000dcf0: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
-0000dd00: 0000 0e4d 6573 7361 6765 2073 7472 696e  ...Message strin
-0000dd10: 6707 0000 000b 5173 6369 4c65 7865 7250  g.....QsciLexerP
-0000dd20: 4f01 0300 0000 3200 4d00 6500 6c00 6400  O.....2.M.e.l.d.
-0000dd30: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
-0000dd40: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
-0000dd50: 6e00 7400 6500 7800 7408 0000 0000 0600  n.t.e.x.t.......
-0000dd60: 0000 134d 6573 7361 6765 2073 7472 696e  ...Message strin
-0000dd70: 6720 7465 7874 0700 0000 0b51 7363 694c  g text.....QsciL
-0000dd80: 6578 6572 504f 0103 0000 0048 004d 0065  exerPO.....H.M.e
-0000dd90: 006c 0064 0075 006e 0067 0073 007a 0065  .l.d.u.n.g.s.z.e
-0000dda0: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-0000ddb0: 0074 0065 006e 0074 0065 0078 0074 0020  .t.e.n.t.e.x.t. 
-0000ddc0: 005a 0065 0069 006c 0065 006e 0065 006e  .Z.e.i.l.e.n.e.n
-0000ddd0: 0064 0065 0800 0000 0006 0000 001f 4d65  .d.e..........Me
-0000dde0: 7373 6167 6520 7374 7269 6e67 2074 6578  ssage string tex
-0000ddf0: 7420 656e 642d 6f66 2d6c 696e 6507 0000  t end-of-line...
-0000de00: 000b 5173 6369 4c65 7865 7250 4f01 0300  ..QsciLexerPO...
-0000de10: 0000 2c00 5000 7200 6f00 6700 7200 6100  ..,.P.r.o.g.r.a.
-0000de20: 6d00 6d00 6900 6500 7200 6500 7200 6b00  m.m.i.e.r.e.r.k.
-0000de30: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-0000de40: 0000 0000 0600 0000 1250 726f 6772 616d  .........Program
-0000de50: 6d65 7220 636f 6d6d 656e 7407 0000 000b  mer comment.....
-0000de60: 5173 6369 4c65 7865 7250 4f01 0300 0000  QsciLexerPO.....
-0000de70: 1000 5200 6500 6600 6500 7200 6500 6e00  ..R.e.f.e.r.e.n.
-0000de80: 7a08 0000 0000 0600 0000 0952 6566 6572  z..........Refer
-0000de90: 656e 6365 0700 0000 0b51 7363 694c 6578  ence.....QsciLex
-0000dea0: 6572 504f 0103 0000 0026 0055 006e 0067  erPO.....&.U.n.g
-0000deb0: 00fc 006c 0074 0069 0067 0065 0020 0044  ...l.t.i.g.e. .D
-0000dec0: 0069 0072 0065 006b 0074 0069 0076 0065  .i.r.e.k.t.i.v.e
-0000ded0: 0800 0000 0006 0000 000d 4261 6420 6469  ..........Bad di
-0000dee0: 7265 6374 6976 6507 0000 000c 5173 6369  rective.....Qsci
-0000def0: 4c65 7865 7250 4f56 0103 0000 0012 004b  LexerPOV.......K
-0000df00: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-0000df10: 0800 0000 0006 0000 0007 436f 6d6d 656e  ..........Commen
-0000df20: 7407 0000 000c 5173 6369 4c65 7865 7250  t.....QsciLexerP
-0000df30: 4f56 0103 0000 001c 004b 006f 006d 006d  OV.......K.o.m.m
-0000df40: 0065 006e 0074 0061 0072 007a 0065 0069  .e.n.t.a.r.z.e.i
-0000df50: 006c 0065 0800 0000 0006 0000 000c 436f  .l.e..........Co
-0000df60: 6d6d 656e 7420 6c69 6e65 0700 0000 0c51  mment line.....Q
-0000df70: 7363 694c 6578 6572 504f 5601 0300 0000  sciLexerPOV.....
-0000df80: 1000 5300 7400 6100 6e00 6400 6100 7200  ..S.t.a.n.d.a.r.
-0000df90: 6408 0000 0000 0600 0000 0744 6566 6175  d..........Defau
-0000dfa0: 6c74 0700 0000 0c51 7363 694c 6578 6572  lt.....QsciLexer
-0000dfb0: 504f 5601 0300 0000 1200 4400 6900 7200  POV.......D.i.r.
-0000dfc0: 6500 6b00 7400 6900 7600 6508 0000 0000  e.k.t.i.v.e.....
-0000dfd0: 0600 0000 0944 6972 6563 7469 7665 0700  .....Directive..
-0000dfe0: 0000 0c51 7363 694c 6578 6572 504f 5601  ...QsciLexerPOV.
-0000dff0: 0300 0000 1400 4200 6500 7a00 6500 6900  ......B.e.z.e.i.
-0000e000: 6300 6800 6e00 6500 7208 0000 0000 0600  c.h.n.e.r.......
-0000e010: 0000 0a49 6465 6e74 6966 6965 7207 0000  ...Identifier...
-0000e020: 000c 5173 6369 4c65 7865 7250 4f56 0103  ..QsciLexerPOV..
-0000e030: 0000 0008 005a 0061 0068 006c 0800 0000  .....Z.a.h.l....
-0000e040: 0006 0000 0006 4e75 6d62 6572 0700 0000  ......Number....
-0000e050: 0c51 7363 694c 6578 6572 504f 5601 0300  .QsciLexerPOV...
-0000e060: 0000 3800 4f00 6200 6a00 6500 6b00 7400  ..8.O.b.j.e.k.t.
-0000e070: 6500 2c00 2000 4300 5300 4700 2000 7500  e.,. .C.S.G. .u.
-0000e080: 6e00 6400 2000 4500 7200 7300 6300 6800  n.d. .E.r.s.c.h.
-0000e090: 6500 6900 6e00 7500 6e00 6708 0000 0000  e.i.n.u.n.g.....
-0000e0a0: 0600 0000 1b4f 626a 6563 7473 2c20 4353  .....Objects, CS
-0000e0b0: 4720 616e 6420 6170 7065 6172 616e 6365  G and appearance
-0000e0c0: 0700 0000 0c51 7363 694c 6578 6572 504f  .....QsciLexerPO
-0000e0d0: 5601 0300 0000 1000 4f00 7000 6500 7200  V.......O.p.e.r.
-0000e0e0: 6100 7400 6f00 7208 0000 0000 0600 0000  a.t.o.r.........
-0000e0f0: 084f 7065 7261 746f 7207 0000 000c 5173  .Operator.....Qs
-0000e100: 6369 4c65 7865 7250 4f56 0103 0000 002c  ciLexerPOV.....,
-0000e110: 0056 006f 0072 0064 0065 0066 0069 006e  .V.o.r.d.e.f.i.n
-0000e120: 0069 0065 0072 0074 0065 0020 0046 0075  .i.e.r.t.e. .F.u
-0000e130: 006e 006b 0074 0069 006f 006e 0800 0000  .n.k.t.i.o.n....
-0000e140: 0006 0000 0014 5072 6564 6566 696e 6564  ......Predefined
-0000e150: 2066 756e 6374 696f 6e73 0700 0000 0c51   functions.....Q
-0000e160: 7363 694c 6578 6572 504f 5601 0300 0000  sciLexerPOV.....
-0000e170: 3200 5600 6f00 7200 6400 6500 6600 6900  2.V.o.r.d.e.f.i.
-0000e180: 6e00 6900 6500 7200 7400 6500 7200 2000  n.i.e.r.t.e.r. .
-0000e190: 4200 6500 7a00 6500 6900 6300 6800 6e00  B.e.z.e.i.c.h.n.
-0000e1a0: 6500 7208 0000 0000 0600 0000 1650 7265  e.r..........Pre
-0000e1b0: 6465 6669 6e65 6420 6964 656e 7469 6669  defined identifi
-0000e1c0: 6572 7307 0000 000c 5173 6369 4c65 7865  ers.....QsciLexe
-0000e1d0: 7250 4f56 0103 0000 0018 005a 0065 0069  rPOV.......Z.e.i
-0000e1e0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-0000e1f0: 0065 0800 0000 0006 0000 0006 5374 7269  .e..........Stri
-0000e200: 6e67 0700 0000 0c51 7363 694c 6578 6572  ng.....QsciLexer
-0000e210: 504f 5601 0300 0000 3a00 5400 7900 7000  POV.....:.T.y.p.
-0000e220: 6500 6e00 2c00 2000 4d00 6f00 6400 6900  e.n.,. .M.o.d.i.
-0000e230: 6600 6900 7a00 6900 6500 7200 6500 7200  f.i.z.i.e.r.e.r.
-0000e240: 2000 7500 6e00 6400 2000 4900 7400 6500   .u.n.d. .I.t.e.
-0000e250: 6d00 7308 0000 0000 0600 0000 1a54 7970  m.s..........Typ
-0000e260: 6573 2c20 6d6f 6469 6669 6572 7320 616e  es, modifiers an
-0000e270: 6420 6974 656d 7307 0000 000c 5173 6369  d items.....Qsci
-0000e280: 4c65 7865 7250 4f56 0103 0000 002e 0055  LexerPOV.......U
-0000e290: 006e 0062 0065 0065 006e 0064 0065 0074  .n.b.e.e.n.d.e.t
-0000e2a0: 0065 0020 005a 0065 0069 0063 0068 0065  .e. .Z.e.i.c.h.e
-0000e2b0: 006e 006b 0065 0074 0074 0065 0800 0000  .n.k.e.t.t.e....
-0000e2c0: 0006 0000 000f 556e 636c 6f73 6564 2073  ......Unclosed s
-0000e2d0: 7472 696e 6707 0000 000c 5173 6369 4c65  tring.....QsciLe
-0000e2e0: 7865 7250 4f56 0103 0000 0024 004e 0075  xerPOV.....$.N.u
-0000e2f0: 0074 007a 0065 0072 0020 0064 0065 0066  .t.z.e.r. .d.e.f
-0000e300: 0069 006e 0069 0065 0072 0074 0020 0031  .i.n.i.e.r.t. .1
-0000e310: 0800 0000 0006 0000 000e 5573 6572 2064  ..........User d
-0000e320: 6566 696e 6564 2031 0700 0000 0c51 7363  efined 1.....Qsc
-0000e330: 694c 6578 6572 504f 5601 0300 0000 2400  iLexerPOV.....$.
-0000e340: 4e00 7500 7400 7a00 6500 7200 2000 6400  N.u.t.z.e.r. .d.
-0000e350: 6500 6600 6900 6e00 6900 6500 7200 7400  e.f.i.n.i.e.r.t.
-0000e360: 2000 3208 0000 0000 0600 0000 0e55 7365   .2..........Use
-0000e370: 7220 6465 6669 6e65 6420 3207 0000 000c  r defined 2.....
-0000e380: 5173 6369 4c65 7865 7250 4f56 0103 0000  QsciLexerPOV....
-0000e390: 0024 004e 0075 0074 007a 0065 0072 0020  .$.N.u.t.z.e.r. 
-0000e3a0: 0064 0065 0066 0069 006e 0069 0065 0072  .d.e.f.i.n.i.e.r
-0000e3b0: 0074 0020 0033 0800 0000 0006 0000 000e  .t. .3..........
-0000e3c0: 5573 6572 2064 6566 696e 6564 2033 0700  User defined 3..
-0000e3d0: 0000 0c51 7363 694c 6578 6572 504f 5601  ...QsciLexerPOV.
-0000e3e0: 0300 0000 2a00 2700 2800 2a00 2000 2e00  ....*.'.(.*. ...
-0000e3f0: 2e00 2e00 2000 2a00 2900 2700 2000 4b00  .... .*.).'. .K.
-0000e400: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-0000e410: 0000 0000 0600 0000 1927 282a 202e 2e2e  .........'(* ...
-0000e420: 202a 2927 2073 7479 6c65 2063 6f6d 6d65   *)' style comme
-0000e430: 6e74 0700 0000 0f51 7363 694c 6578 6572  nt.....QsciLexer
-0000e440: 5061 7363 616c 0103 0000 003c 0027 0028  Pascal.....<.'.(
-0000e450: 002a 0024 0020 002e 002e 002e 0020 002a  .*.$. ....... .*
-0000e460: 0029 0027 0020 0050 0072 00e4 0070 0072  .).'. .P.r...p.r
-0000e470: 006f 007a 0065 0073 0073 006f 0072 0062  .o.z.e.s.s.o.r.b
-0000e480: 006c 006f 0063 006b 0800 0000 0006 0000  .l.o.c.k........
-0000e490: 0026 2728 2a24 202e 2e2e 202a 2927 2073  .&'(*$ ... *)' s
-0000e4a0: 7479 6c65 2070 7265 2d70 726f 6365 7373  tyle pre-process
-0000e4b0: 6f72 2062 6c6f 636b 0700 0000 0f51 7363  or block.....Qsc
-0000e4c0: 694c 6578 6572 5061 7363 616c 0103 0000  iLexerPascal....
-0000e4d0: 0026 0027 007b 0020 002e 002e 002e 0020  .&.'.{. ....... 
-0000e4e0: 007d 0027 0020 004b 006f 006d 006d 0065  .}.'. .K.o.m.m.e
-0000e4f0: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
-0000e500: 0017 277b 202e 2e2e 207d 2720 7374 796c  ..'{ ... }' styl
-0000e510: 6520 636f 6d6d 656e 7407 0000 000f 5173  e comment.....Qs
-0000e520: 6369 4c65 7865 7250 6173 6361 6c01 0300  ciLexerPascal...
-0000e530: 0000 3800 2700 7b00 2400 2000 2e00 2e00  ..8.'.{.$. .....
-0000e540: 2e00 2000 7d00 2700 2000 5000 7200 e400  .. .}.'. .P.r...
-0000e550: 7000 7200 6f00 7a00 6500 7300 7300 6f00  p.r.o.z.e.s.s.o.
-0000e560: 7200 6200 6c00 6f00 6300 6b08 0000 0000  r.b.l.o.c.k.....
-0000e570: 0600 0000 2427 7b24 202e 2e2e 207d 2720  ....$'{$ ... }' 
-0000e580: 7374 796c 6520 7072 652d 7072 6f63 6573  style pre-proces
-0000e590: 736f 7220 626c 6f63 6b07 0000 000f 5173  sor block.....Qs
-0000e5a0: 6369 4c65 7865 7250 6173 6361 6c01 0300  ciLexerPascal...
-0000e5b0: 0000 0e00 5a00 6500 6900 6300 6800 6500  ....Z.e.i.c.h.e.
-0000e5c0: 6e08 0000 0000 0600 0000 0943 6861 7261  n..........Chara
-0000e5d0: 6374 6572 0700 0000 0f51 7363 694c 6578  cter.....QsciLex
-0000e5e0: 6572 5061 7363 616c 0103 0000 0010 0053  erPascal.......S
-0000e5f0: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
-0000e600: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
-0000e610: 0000 000f 5173 6369 4c65 7865 7250 6173  ....QsciLexerPas
-0000e620: 6361 6c01 0300 0000 2200 4800 6500 7800  cal.....".H.e.x.
-0000e630: 6100 6400 6500 7a00 6900 6d00 6100 6c00  a.d.e.z.i.m.a.l.
-0000e640: 6500 2000 5a00 6100 6800 6c08 0000 0000  e. .Z.a.h.l.....
-0000e650: 0600 0000 1248 6578 6164 6563 696d 616c  .....Hexadecimal
-0000e660: 206e 756d 6265 7207 0000 000f 5173 6369   number.....Qsci
-0000e670: 4c65 7865 7250 6173 6361 6c01 0300 0000  LexerPascal.....
-0000e680: 1400 4200 6500 7a00 6500 6900 6300 6800  ..B.e.z.e.i.c.h.
-0000e690: 6e00 6500 7208 0000 0000 0600 0000 0a49  n.e.r..........I
-0000e6a0: 6465 6e74 6966 6965 7207 0000 000f 5173  dentifier.....Qs
-0000e6b0: 6369 4c65 7865 7250 6173 6361 6c01 0300  ciLexerPascal...
-0000e6c0: 0000 2000 4900 6e00 6c00 6900 6e00 6500  .. .I.n.l.i.n.e.
-0000e6d0: 2000 4100 7300 7300 6500 6d00 6200 6c00   .A.s.s.e.m.b.l.
-0000e6e0: 6500 7208 0000 0000 0600 0000 0a49 6e6c  e.r..........Inl
-0000e6f0: 696e 6520 6173 6d07 0000 000f 5173 6369  ine asm.....Qsci
-0000e700: 4c65 7865 7250 6173 6361 6c01 0300 0000  LexerPascal.....
-0000e710: 1a00 5300 6300 6800 6c00 fc00 7300 7300  ..S.c.h.l...s.s.
-0000e720: 6500 6c00 7700 6f00 7200 7408 0000 0000  e.l.w.o.r.t.....
-0000e730: 0600 0000 074b 6579 776f 7264 0700 0000  .....Keyword....
-0000e740: 0f51 7363 694c 6578 6572 5061 7363 616c  .QsciLexerPascal
-0000e750: 0103 0000 001e 005a 0065 0069 006c 0065  .......Z.e.i.l.e
-0000e760: 006e 006b 006f 006d 006d 0065 006e 0074  .n.k.o.m.m.e.n.t
-0000e770: 0061 0072 0800 0000 0006 0000 000c 4c69  .a.r..........Li
-0000e780: 6e65 2063 6f6d 6d65 6e74 0700 0000 0f51  ne comment.....Q
-0000e790: 7363 694c 6578 6572 5061 7363 616c 0103  sciLexerPascal..
-0000e7a0: 0000 0008 005a 0061 0068 006c 0800 0000  .....Z.a.h.l....
-0000e7b0: 0006 0000 0006 4e75 6d62 6572 0700 0000  ......Number....
-0000e7c0: 0f51 7363 694c 6578 6572 5061 7363 616c  .QsciLexerPascal
-0000e7d0: 0103 0000 0010 004f 0070 0065 0072 0061  .......O.p.e.r.a
-0000e7e0: 0074 006f 0072 0800 0000 0006 0000 0008  .t.o.r..........
-0000e7f0: 4f70 6572 6174 6f72 0700 0000 0f51 7363  Operator.....Qsc
-0000e800: 694c 6578 6572 5061 7363 616c 0103 0000  iLexerPascal....
-0000e810: 0036 005a 0065 0069 0063 0068 0065 006e  .6.Z.e.i.c.h.e.n
-0000e820: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
-0000e830: 0020 0048 006f 0063 0068 006b 006f 006d  . .H.o.c.h.k.o.m
-0000e840: 006d 0061 0074 0061 0800 0000 0006 0000  .m.a.t.a........
-0000e850: 0014 5369 6e67 6c65 2d71 756f 7465 6420  ..Single-quoted 
-0000e860: 7374 7269 6e67 0700 0000 0f51 7363 694c  string.....QsciL
-0000e870: 6578 6572 5061 7363 616c 0103 0000 002e  exerPascal......
-0000e880: 0055 006e 0062 0065 0065 006e 0064 0065  .U.n.b.e.e.n.d.e
-0000e890: 0074 0065 0020 005a 0065 0069 0063 0068  .t.e. .Z.e.i.c.h
-0000e8a0: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
-0000e8b0: 0000 0006 0000 000f 556e 636c 6f73 6564  ........Unclosed
-0000e8c0: 2073 7472 696e 6707 0000 000f 5173 6369   string.....Qsci
-0000e8d0: 4c65 7865 7250 6173 6361 6c01 0300 0000  LexerPascal.....
-0000e8e0: 0800 4600 6500 6c00 6408 0000 0000 0600  ..F.e.l.d.......
-0000e8f0: 0000 0541 7272 6179 0700 0000 0d51 7363  ...Array.....Qsc
-0000e900: 694c 6578 6572 5065 726c 0103 0000 0034  iLexerPerl.....4
-0000e910: 0048 0065 0072 0065 0020 0044 006f 006b  .H.e.r.e. .D.o.k
-0000e920: 0075 006d 0065 006e 0074 0020 0069 006e  .u.m.e.n.t. .i.n
-0000e930: 0020 0042 0061 0063 006b 0074 0069 0063  . .B.a.c.k.t.i.c
-0000e940: 006b 0073 0800 0000 0006 0000 0016 4261  .k.s..........Ba
-0000e950: 636b 7469 636b 2068 6572 6520 646f 6375  cktick here docu
-0000e960: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
-0000e970: 6572 5065 726c 0103 0000 0066 0048 0065  erPerl.....f.H.e
-0000e980: 0072 0065 0020 0044 006f 006b 0075 006d  .r.e. .D.o.k.u.m
-0000e990: 0065 006e 0074 0020 0069 006e 0020 0042  .e.n.t. .i.n. .B
-0000e9a0: 0061 0063 006b 0074 0069 0063 006b 0073  .a.c.k.t.i.c.k.s
-0000e9b0: 0020 0028 0069 006e 0074 0065 0072 0070  . .(.i.n.t.e.r.p
-0000e9c0: 006f 006c 0069 0065 0072 0074 0065 0020  .o.l.i.e.r.t.e. 
-0000e9d0: 0056 0061 0072 0069 0061 0062 006c 0065  .V.a.r.i.a.b.l.e
-0000e9e0: 0029 0800 0000 0006 0000 002e 4261 636b  .)..........Back
-0000e9f0: 7469 636b 2068 6572 6520 646f 6375 6d65  tick here docume
-0000ea00: 6e74 2028 696e 7465 7270 6f6c 6174 6564  nt (interpolated
-0000ea10: 2076 6172 6961 626c 6529 0700 0000 0d51   variable).....Q
-0000ea20: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
-0000ea30: 0012 0042 0061 0063 006b 0074 0069 0063  ...B.a.c.k.t.i.c
-0000ea40: 006b 0073 0800 0000 0006 0000 0009 4261  .k.s..........Ba
-0000ea50: 636b 7469 636b 7307 0000 000d 5173 6369  ckticks.....Qsci
-0000ea60: 4c65 7865 7250 6572 6c01 0300 0000 4400  LexerPerl.....D.
-0000ea70: 4200 6100 6300 6b00 7400 6900 6300 6b00  B.a.c.k.t.i.c.k.
-0000ea80: 7300 2000 2800 6900 6e00 7400 6500 7200  s. .(.i.n.t.e.r.
-0000ea90: 7000 6f00 6c00 6900 6500 7200 7400 6500  p.o.l.i.e.r.t.e.
-0000eaa0: 2000 5600 6100 7200 6900 6100 6200 6c00   .V.a.r.i.a.b.l.
-0000eab0: 6500 2908 0000 0000 0600 0000 2142 6163  e.).........!Bac
-0000eac0: 6b74 6963 6b73 2028 696e 7465 7270 6f6c  kticks (interpol
-0000ead0: 6174 6564 2076 6172 6961 626c 6529 0700  ated variable)..
-0000eae0: 0000 0d51 7363 694c 6578 6572 5065 726c  ...QsciLexerPerl
-0000eaf0: 0103 0000 0012 004b 006f 006d 006d 0065  .......K.o.m.m.e
-0000eb00: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
-0000eb10: 0007 436f 6d6d 656e 7407 0000 000d 5173  ..Comment.....Qs
-0000eb20: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
-0000eb30: 1800 4400 6100 7400 6500 6e00 7300 6500  ..D.a.t.e.n.s.e.
-0000eb40: 6b00 7400 6900 6f00 6e08 0000 0000 0600  k.t.i.o.n.......
-0000eb50: 0000 0c44 6174 6120 7365 6374 696f 6e07  ...Data section.
-0000eb60: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
-0000eb70: 6c01 0300 0000 1000 5300 7400 6100 6e00  l.......S.t.a.n.
-0000eb80: 6400 6100 7200 6408 0000 0000 0600 0000  d.a.r.d.........
-0000eb90: 0744 6566 6175 6c74 0700 0000 0d51 7363  .Default.....Qsc
-0000eba0: 694c 6578 6572 5065 726c 0103 0000 0044  iLexerPerl.....D
-0000ebb0: 0048 0065 0072 0065 0020 0044 006f 006b  .H.e.r.e. .D.o.k
-0000ebc0: 0075 006d 0065 006e 0074 0020 0069 006e  .u.m.e.n.t. .i.n
-0000ebd0: 0020 0041 006e 0066 00fc 0068 0072 0075  . .A.n.f...h.r.u
-0000ebe0: 006e 0067 0073 007a 0065 0069 0063 0068  .n.g.s.z.e.i.c.h
-0000ebf0: 0065 006e 0800 0000 0006 0000 001b 446f  .e.n..........Do
-0000ec00: 7562 6c65 2d71 756f 7465 6420 6865 7265  uble-quoted here
-0000ec10: 2064 6f63 756d 656e 7407 0000 000d 5173   document.....Qs
-0000ec20: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
-0000ec30: 7600 4800 6500 7200 6500 2000 4400 6f00  v.H.e.r.e. .D.o.
-0000ec40: 6b00 7500 6d00 6500 6e00 7400 2000 6900  k.u.m.e.n.t. .i.
-0000ec50: 6e00 2000 4100 6e00 6600 fc00 6800 7200  n. .A.n.f...h.r.
-0000ec60: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
-0000ec70: 6800 6500 6e00 2000 2800 6900 6e00 7400  h.e.n. .(.i.n.t.
-0000ec80: 6500 7200 7000 6f00 6c00 6900 6500 7200  e.r.p.o.l.i.e.r.
-0000ec90: 7400 6500 2000 5600 6100 7200 6900 6100  t.e. .V.a.r.i.a.
-0000eca0: 6200 6c00 6500 2908 0000 0000 0600 0000  b.l.e.).........
-0000ecb0: 3344 6f75 626c 652d 7175 6f74 6564 2068  3Double-quoted h
-0000ecc0: 6572 6520 646f 6375 6d65 6e74 2028 696e  ere document (in
-0000ecd0: 7465 7270 6f6c 6174 6564 2076 6172 6961  terpolated varia
-0000ece0: 626c 6529 0700 0000 0d51 7363 694c 6578  ble).....QsciLex
-0000ecf0: 6572 5065 726c 0103 0000 0042 005a 0065  erPerl.....B.Z.e
-0000ed00: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-0000ed10: 0074 0065 0020 0069 006e 0020 0041 006e  .t.e. .i.n. .A.n
-0000ed20: 0066 00fc 0068 0072 0075 006e 0067 0073  .f...h.r.u.n.g.s
-0000ed30: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
-0000ed40: 0000 0006 0000 0014 446f 7562 6c65 2d71  ........Double-q
-0000ed50: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
-0000ed60: 0d51 7363 694c 6578 6572 5065 726c 0103  .QsciLexerPerl..
-0000ed70: 0000 0074 005a 0065 0069 0063 0068 0065  ...t.Z.e.i.c.h.e
-0000ed80: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
-0000ed90: 006e 0020 0041 006e 0066 00fc 0068 0072  .n. .A.n.f...h.r
-0000eda0: 0075 006e 0067 0073 007a 0065 0069 0063  .u.n.g.s.z.e.i.c
-0000edb0: 0068 0065 006e 0020 0028 0069 006e 0074  .h.e.n. .(.i.n.t
-0000edc0: 0065 0072 0070 006f 006c 0069 0065 0072  .e.r.p.o.l.i.e.r
-0000edd0: 0074 0065 0020 0056 0061 0072 0069 0061  .t.e. .V.a.r.i.a
-0000ede0: 0062 006c 0065 0029 0800 0000 0006 0000  .b.l.e.)........
-0000edf0: 002c 446f 7562 6c65 2d71 756f 7465 6420  .,Double-quoted 
-0000ee00: 7374 7269 6e67 2028 696e 7465 7270 6f6c  string (interpol
-0000ee10: 6174 6564 2076 6172 6961 626c 6529 0700  ated variable)..
-0000ee20: 0000 0d51 7363 694c 6578 6572 5065 726c  ...QsciLexerPerl
-0000ee30: 0103 0000 000c 0046 0065 0068 006c 0065  .......F.e.h.l.e
-0000ee40: 0072 0800 0000 0006 0000 0005 4572 726f  .r..........Erro
-0000ee50: 7207 0000 000d 5173 6369 4c65 7865 7250  r.....QsciLexerP
-0000ee60: 6572 6c01 0300 0000 1600 4600 6f00 7200  erl.......F.o.r.
-0000ee70: 6d00 6100 7400 7a00 7700 6500 6900 6708  m.a.t.z.w.e.i.g.
-0000ee80: 0000 0000 0600 0000 0b46 6f72 6d61 7420  .........Format 
-0000ee90: 626f 6479 0700 0000 0d51 7363 694c 6578  body.....QsciLex
-0000eea0: 6572 5065 726c 0103 0000 0026 0046 006f  erPerl.....&.F.o
-0000eeb0: 0072 006d 0061 0074 0069 0064 0065 006e  .r.m.a.t.i.d.e.n
-0000eec0: 0074 0069 0066 0069 006b 0061 0074 006f  .t.i.f.i.k.a.t.o
-0000eed0: 0072 0800 0000 0006 0000 0011 466f 726d  .r..........Form
-0000eee0: 6174 2069 6465 6e74 6966 6965 7207 0000  at identifier...
-0000eef0: 000d 5173 6369 4c65 7865 7250 6572 6c01  ..QsciLexerPerl.
-0000ef00: 0300 0000 0800 4800 6100 7300 6808 0000  ......H.a.s.h...
-0000ef10: 0000 0600 0000 0448 6173 6807 0000 000d  .......Hash.....
-0000ef20: 5173 6369 4c65 7865 7250 6572 6c01 0300  QsciLexerPerl...
-0000ef30: 0000 2e00 4800 6500 7200 6500 2000 4400  ....H.e.r.e. .D.
-0000ef40: 6f00 6b00 7500 6d00 6500 6e00 7400 2d00  o.k.u.m.e.n.t.-.
-0000ef50: 4200 6500 6700 7200 6500 6e00 7a00 6500  B.e.g.r.e.n.z.e.
-0000ef60: 7208 0000 0000 0600 0000 1748 6572 6520  r..........Here 
-0000ef70: 646f 6375 6d65 6e74 2064 656c 696d 6974  document delimit
-0000ef80: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
-0000ef90: 5065 726c 0103 0000 0014 0042 0065 007a  Perl.......B.e.z
-0000efa0: 0065 0069 0063 0068 006e 0065 0072 0800  .e.i.c.h.n.e.r..
-0000efb0: 0000 0006 0000 000a 4964 656e 7469 6669  ........Identifi
-0000efc0: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
-0000efd0: 5065 726c 0103 0000 001a 0053 0063 0068  Perl.......S.c.h
-0000efe0: 006c 00fc 0073 0073 0065 006c 0077 006f  .l...s.s.e.l.w.o
-0000eff0: 0072 0074 0800 0000 0006 0000 0007 4b65  .r.t..........Ke
-0000f000: 7977 6f72 6407 0000 000d 5173 6369 4c65  yword.....QsciLe
-0000f010: 7865 7250 6572 6c01 0300 0000 0800 5a00  xerPerl.......Z.
-0000f020: 6100 6800 6c08 0000 0000 0600 0000 064e  a.h.l..........N
-0000f030: 756d 6265 7207 0000 000d 5173 6369 4c65  umber.....QsciLe
-0000f040: 7865 7250 6572 6c01 0300 0000 1000 4f00  xerPerl.......O.
-0000f050: 7000 6500 7200 6100 7400 6f00 7208 0000  p.e.r.a.t.o.r...
-0000f060: 0000 0600 0000 084f 7065 7261 746f 7207  .......Operator.
-0000f070: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
-0000f080: 6c01 0300 0000 0600 5000 4f00 4408 0000  l.......P.O.D...
-0000f090: 0000 0600 0000 0350 4f44 0700 0000 0d51  .......POD.....Q
-0000f0a0: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
-0000f0b0: 0018 0050 004f 0044 0020 0077 00f6 0072  ...P.O.D. .w...r
-0000f0c0: 0074 006c 0069 0063 0068 0800 0000 0006  .t.l.i.c.h......
-0000f0d0: 0000 000c 504f 4420 7665 7262 6174 696d  ....POD verbatim
-0000f0e0: 0700 0000 0d51 7363 694c 6578 6572 5065  .....QsciLexerPe
-0000f0f0: 726c 0103 0000 0020 005a 0065 0069 0063  rl..... .Z.e.i.c
-0000f100: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
-0000f110: 0020 0028 0071 0029 0800 0000 0006 0000  . .(.q.)........
-0000f120: 0011 5175 6f74 6564 2073 7472 696e 6720  ..Quoted string 
-0000f130: 2871 2907 0000 000d 5173 6369 4c65 7865  (q).....QsciLexe
-0000f140: 7250 6572 6c01 0300 0000 2200 5a00 6500  rPerl.....".Z.e.
-0000f150: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
-0000f160: 7400 6500 2000 2800 7100 7100 2908 0000  t.e. .(.q.q.)...
-0000f170: 0000 0600 0000 1251 756f 7465 6420 7374  .......Quoted st
-0000f180: 7269 6e67 2028 7171 2907 0000 000d 5173  ring (qq).....Qs
-0000f190: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
-0000f1a0: 5200 5a00 6500 6900 6300 6800 6500 6e00  R.Z.e.i.c.h.e.n.
-0000f1b0: 6b00 6500 7400 7400 6500 2000 2800 7100  k.e.t.t.e. .(.q.
-0000f1c0: 7100 2c00 2000 6900 6e00 7400 6500 7200  q.,. .i.n.t.e.r.
-0000f1d0: 7000 6f00 6c00 6900 6500 7200 7400 6500  p.o.l.i.e.r.t.e.
-0000f1e0: 2000 5600 6100 7200 6900 6100 6200 6c00   .V.a.r.i.a.b.l.
-0000f1f0: 6500 2908 0000 0000 0600 0000 2951 756f  e.).........)Quo
-0000f200: 7465 6420 7374 7269 6e67 2028 7171 2c20  ted string (qq, 
-0000f210: 696e 7465 7270 6f6c 6174 6564 2076 6172  interpolated var
-0000f220: 6961 626c 6529 0700 0000 0d51 7363 694c  iable).....QsciL
-0000f230: 6578 6572 5065 726c 0103 0000 0022 005a  exerPerl.....".Z
-0000f240: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-0000f250: 0074 0074 0065 0020 0028 0071 0072 0029  .t.t.e. .(.q.r.)
-0000f260: 0800 0000 0006 0000 0012 5175 6f74 6564  ..........Quoted
-0000f270: 2073 7472 696e 6720 2871 7229 0700 0000   string (qr)....
-0000f280: 0d51 7363 694c 6578 6572 5065 726c 0103  .QsciLexerPerl..
-0000f290: 0000 0052 005a 0065 0069 0063 0068 0065  ...R.Z.e.i.c.h.e
-0000f2a0: 006e 006b 0065 0074 0074 0065 0020 0028  .n.k.e.t.t.e. .(
-0000f2b0: 0071 0072 002c 0020 0069 006e 0074 0065  .q.r.,. .i.n.t.e
-0000f2c0: 0072 0070 006f 006c 0069 0065 0072 0074  .r.p.o.l.i.e.r.t
-0000f2d0: 0065 0020 0056 0061 0072 0069 0061 0062  .e. .V.a.r.i.a.b
-0000f2e0: 006c 0065 0029 0800 0000 0006 0000 0029  .l.e.).........)
-0000f2f0: 5175 6f74 6564 2073 7472 696e 6720 2871  Quoted string (q
-0000f300: 722c 2069 6e74 6572 706f 6c61 7465 6420  r, interpolated 
-0000f310: 7661 7269 6162 6c65 2907 0000 000d 5173  variable).....Qs
-0000f320: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
-0000f330: 2200 5a00 6500 6900 6300 6800 6500 6e00  ".Z.e.i.c.h.e.n.
-0000f340: 6b00 6500 7400 7400 6500 2000 2800 7100  k.e.t.t.e. .(.q.
-0000f350: 7700 2908 0000 0000 0600 0000 1251 756f  w.)..........Quo
-0000f360: 7465 6420 7374 7269 6e67 2028 7177 2907  ted string (qw).
-0000f370: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
-0000f380: 6c01 0300 0000 2200 5a00 6500 6900 6300  l.....".Z.e.i.c.
-0000f390: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
-0000f3a0: 2000 2800 7100 7800 2908 0000 0000 0600   .(.q.x.).......
-0000f3b0: 0000 1251 756f 7465 6420 7374 7269 6e67  ...Quoted string
-0000f3c0: 2028 7178 2907 0000 000d 5173 6369 4c65   (qx).....QsciLe
-0000f3d0: 7865 7250 6572 6c01 0300 0000 5200 5a00  xerPerl.....R.Z.
-0000f3e0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-0000f3f0: 7400 7400 6500 2000 2800 7100 7800 2c00  t.t.e. .(.q.x.,.
-0000f400: 2000 6900 6e00 7400 6500 7200 7000 6f00   .i.n.t.e.r.p.o.
-0000f410: 6c00 6900 6500 7200 7400 6500 2000 5600  l.i.e.r.t.e. .V.
-0000f420: 6100 7200 6900 6100 6200 6c00 6500 2908  a.r.i.a.b.l.e.).
-0000f430: 0000 0000 0600 0000 2951 756f 7465 6420  ........)Quoted 
-0000f440: 7374 7269 6e67 2028 7178 2c20 696e 7465  string (qx, inte
-0000f450: 7270 6f6c 6174 6564 2076 6172 6961 626c  rpolated variabl
-0000f460: 6529 0700 0000 0d51 7363 694c 6578 6572  e).....QsciLexer
-0000f470: 5065 726c 0103 0000 0024 0052 0065 0067  Perl.....$.R.e.g
-0000f480: 0075 006c 00e4 0072 0065 0072 0020 0041  .u.l...r.e.r. .A
-0000f490: 0075 0073 0064 0072 0075 0063 006b 0800  .u.s.d.r.u.c.k..
-0000f4a0: 0000 0006 0000 0012 5265 6775 6c61 7220  ........Regular 
-0000f4b0: 6578 7072 6573 7369 6f6e 0700 0000 0d51  expression.....Q
-0000f4c0: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
-0000f4d0: 0056 0052 0065 0067 0075 006c 00e4 0072  .V.R.e.g.u.l...r
-0000f4e0: 0065 0072 0020 0041 0075 0073 0064 0072  .e.r. .A.u.s.d.r
-0000f4f0: 0075 0063 006b 0020 0028 0069 006e 0074  .u.c.k. .(.i.n.t
-0000f500: 0065 0072 0070 006f 006c 0069 0065 0072  .e.r.p.o.l.i.e.r
-0000f510: 0074 0065 0020 0056 0061 0072 0069 0061  .t.e. .V.a.r.i.a
-0000f520: 0062 006c 0065 0029 0800 0000 0006 0000  .b.l.e.)........
-0000f530: 002a 5265 6775 6c61 7220 6578 7072 6573  .*Regular expres
-0000f540: 7369 6f6e 2028 696e 7465 7270 6f6c 6174  sion (interpolat
-0000f550: 6564 2076 6172 6961 626c 6529 0700 0000  ed variable)....
-0000f560: 0d51 7363 694c 6578 6572 5065 726c 0103  .QsciLexerPerl..
-0000f570: 0000 000c 0053 006b 0061 006c 0061 0072  .....S.k.a.l.a.r
-0000f580: 0800 0000 0006 0000 0006 5363 616c 6172  ..........Scalar
-0000f590: 0700 0000 0d51 7363 694c 6578 6572 5065  .....QsciLexerPe
-0000f5a0: 726c 0103 0000 0038 0048 0065 0072 0065  rl.....8.H.e.r.e
-0000f5b0: 0020 0044 006f 006b 0075 006d 0065 006e  . .D.o.k.u.m.e.n
-0000f5c0: 0074 0020 0069 006e 0020 0048 006f 0063  .t. .i.n. .H.o.c
-0000f5d0: 0068 006b 006f 006d 006d 0061 0074 0061  .h.k.o.m.m.a.t.a
-0000f5e0: 0800 0000 0006 0000 001b 5369 6e67 6c65  ..........Single
-0000f5f0: 2d71 756f 7465 6420 6865 7265 2064 6f63  -quoted here doc
-0000f600: 756d 656e 7407 0000 000d 5173 6369 4c65  ument.....QsciLe
-0000f610: 7865 7250 6572 6c01 0300 0000 3600 5a00  xerPerl.....6.Z.
-0000f620: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-0000f630: 7400 7400 6500 2000 6900 6e00 2000 4800  t.t.e. .i.n. .H.
-0000f640: 6f00 6300 6800 6b00 6f00 6d00 6d00 6100  o.c.h.k.o.m.m.a.
-0000f650: 7400 6108 0000 0000 0600 0000 1453 696e  t.a..........Sin
-0000f660: 676c 652d 7175 6f74 6564 2073 7472 696e  gle-quoted strin
-0000f670: 6707 0000 000d 5173 6369 4c65 7865 7250  g.....QsciLexerP
-0000f680: 6572 6c01 0300 0000 2800 5300 7500 6200  erl.....(.S.u.b.
-0000f690: 7200 6f00 7500 7400 6900 6e00 6500 6e00  r.o.u.t.i.n.e.n.
-0000f6a0: 2000 5000 7200 6f00 7400 6f00 7400 7900   .P.r.o.t.o.t.y.
-0000f6b0: 7008 0000 0000 0600 0000 1453 7562 726f  p..........Subro
-0000f6c0: 7574 696e 6520 7072 6f74 6f74 7970 6507  utine prototype.
-0000f6d0: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
-0000f6e0: 6c01 0300 0000 1200 4500 7200 7300 6500  l.......E.r.s.e.
-0000f6f0: 7400 7a00 7500 6e00 6708 0000 0000 0600  t.z.u.n.g.......
-0000f700: 0000 0c53 7562 7374 6974 7574 696f 6e07  ...Substitution.
-0000f710: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
-0000f720: 6c01 0300 0000 4400 4500 7200 7300 6500  l.....D.E.r.s.e.
-0000f730: 7400 7a00 7500 6e00 6700 2000 2800 6900  t.z.u.n.g. .(.i.
-0000f740: 6e00 7400 6500 7200 7000 6f00 6c00 6900  n.t.e.r.p.o.l.i.
-0000f750: 6500 7200 7400 6500 2000 5600 6100 7200  e.r.t.e. .V.a.r.
-0000f760: 6900 6100 6200 6c00 6500 2908 0000 0000  i.a.b.l.e.).....
-0000f770: 0600 0000 2453 7562 7374 6974 7574 696f  ....$Substitutio
-0000f780: 6e20 2869 6e74 6572 706f 6c61 7465 6420  n (interpolated 
-0000f790: 7661 7269 6162 6c65 2907 0000 000d 5173  variable).....Qs
-0000f7a0: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
-0000f7b0: 1a00 5300 7900 6d00 6200 6f00 6c00 7400  ..S.y.m.b.o.l.t.
-0000f7c0: 6100 6200 6500 6c00 6c00 6508 0000 0000  a.b.e.l.l.e.....
-0000f7d0: 0600 0000 0c53 796d 626f 6c20 7461 626c  .....Symbol tabl
-0000f7e0: 6507 0000 000d 5173 6369 4c65 7865 7250  e.....QsciLexerP
-0000f7f0: 6572 6c01 0300 0000 1600 dc00 6200 6500  erl.........b.e.
-0000f800: 7200 7300 6500 7400 7a00 7500 6e00 6708  r.s.e.t.z.u.n.g.
-0000f810: 0000 0000 0600 0000 0b54 7261 6e73 6c61  .........Transla
-0000f820: 7469 6f6e 0700 0000 0d51 7363 694c 6578  tion.....QsciLex
-0000f830: 6572 5065 726c 0103 0000 0018 0046 0065  erPerl.......F.e
-0000f840: 006c 0064 006b 006c 0061 006d 006d 0065  .l.d.k.l.a.m.m.e
-0000f850: 0072 006e 0800 0000 0006 0000 0011 4172  .r.n..........Ar
-0000f860: 7261 7920 7061 7265 6e74 6865 7369 7307  ray parenthesis.
-0000f870: 0000 0013 5173 6369 4c65 7865 7250 6f73  ....QsciLexerPos
-0000f880: 7453 6372 6970 7401 0300 0000 4600 5500  tScript.....F.U.
-0000f890: 6e00 6700 fc00 6c00 7400 6900 6700 6500  n.g...l.t.i.g.e.
-0000f8a0: 7300 2000 5a00 6500 6900 6300 6800 6500  s. .Z.e.i.c.h.e.
-0000f8b0: 6e00 2000 6600 fc00 7200 2000 5a00 6500  n. .f...r. .Z.e.
-0000f8c0: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
-0000f8d0: 7400 6508 0000 0000 0600 0000 1442 6164  t.e..........Bad
-0000f8e0: 2073 7472 696e 6720 6368 6172 6163 7465   string characte
-0000f8f0: 7207 0000 0013 5173 6369 4c65 7865 7250  r.....QsciLexerP
-0000f900: 6f73 7453 6372 6970 7401 0300 0000 2600  ostScript.....&.
-0000f910: 4200 6100 7300 6500 3800 3500 2000 5a00  B.a.s.e.8.5. .Z.
-0000f920: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-0000f930: 7400 7400 6508 0000 0000 0600 0000 0d42  t.t.e..........B
-0000f940: 6173 6538 3520 7374 7269 6e67 0700 0000  ase85 string....
-0000f950: 1351 7363 694c 6578 6572 506f 7374 5363  .QsciLexerPostSc
-0000f960: 7269 7074 0103 0000 0012 004b 006f 006d  ript.......K.o.m
-0000f970: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
-0000f980: 0006 0000 0007 436f 6d6d 656e 7407 0000  ......Comment...
-0000f990: 0013 5173 6369 4c65 7865 7250 6f73 7453  ..QsciLexerPostS
-0000f9a0: 6372 6970 7401 0300 0000 1a00 4400 5300  cript.......D.S.
-0000f9b0: 4300 2000 4b00 6f00 6d00 6d00 6500 6e00  C. .K.o.m.m.e.n.
-0000f9c0: 7400 6100 7208 0000 0000 0600 0000 0b44  t.a.r..........D
-0000f9d0: 5343 2063 6f6d 6d65 6e74 0700 0000 1351  SC comment.....Q
-0000f9e0: 7363 694c 6578 6572 506f 7374 5363 7269  sciLexerPostScri
-0000f9f0: 7074 0103 0000 0022 0044 0053 0043 0020  pt.....".D.S.C. 
-0000fa00: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
-0000fa10: 0072 0077 0065 0072 0074 0800 0000 0006  .r.w.e.r.t......
-0000fa20: 0000 0011 4453 4320 636f 6d6d 656e 7420  ....DSC comment 
-0000fa30: 7661 6c75 6507 0000 0013 5173 6369 4c65  value.....QsciLe
-0000fa40: 7865 7250 6f73 7453 6372 6970 7401 0300  xerPostScript...
-0000fa50: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
-0000fa60: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
-0000fa70: 6175 6c74 0700 0000 1351 7363 694c 6578  ault.....QsciLex
-0000fa80: 6572 506f 7374 5363 7269 7074 0103 0000  erPostScript....
-0000fa90: 0026 0044 0069 0063 0074 0069 006f 006e  .&.D.i.c.t.i.o.n
-0000faa0: 0061 0072 0079 002d 004b 006c 0061 006d  .a.r.y.-.K.l.a.m
-0000fab0: 006d 0065 0072 006e 0800 0000 0006 0000  .m.e.r.n........
-0000fac0: 0016 4469 6374 696f 6e61 7279 2070 6172  ..Dictionary par
-0000fad0: 656e 7468 6573 6973 0700 0000 1351 7363  enthesis.....Qsc
-0000fae0: 694c 6578 6572 506f 7374 5363 7269 7074  iLexerPostScript
-0000faf0: 0103 0000 0032 0048 0065 0078 0061 0064  .....2.H.e.x.a.d
-0000fb00: 0065 007a 0069 006d 0061 006c 0065 0020  .e.z.i.m.a.l.e. 
-0000fb10: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-0000fb20: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
-0000fb30: 0012 4865 7861 6465 6369 6d61 6c20 7374  ..Hexadecimal st
-0000fb40: 7269 6e67 0700 0000 1351 7363 694c 6578  ring.....QsciLex
-0000fb50: 6572 506f 7374 5363 7269 7074 0103 0000  erPostScript....
-0000fb60: 0036 0044 0069 0072 0065 006b 0074 0020  .6.D.i.r.e.k.t. 
-0000fb70: 0061 0075 0073 0067 0065 0066 00fc 0068  .a.u.s.g.e.f...h
-0000fb80: 0072 0074 0065 0073 0020 004c 0069 0074  .r.t.e.s. .L.i.t
-0000fb90: 0065 0072 0061 006c 0800 0000 0006 0000  .e.r.a.l........
-0000fba0: 001d 496d 6d65 6469 6174 656c 7920 6576  ..Immediately ev
-0000fbb0: 616c 7561 7465 6420 6c69 7465 7261 6c07  aluated literal.
-0000fbc0: 0000 0013 5173 6369 4c65 7865 7250 6f73  ....QsciLexerPos
-0000fbd0: 7453 6372 6970 7401 0300 0000 1a00 5300  tScript.......S.
-0000fbe0: 6300 6800 6c00 fc00 7300 7300 6500 6c00  c.h.l...s.s.e.l.
-0000fbf0: 7700 6f00 7200 7408 0000 0000 0600 0000  w.o.r.t.........
-0000fc00: 074b 6579 776f 7264 0700 0000 1351 7363  .Keyword.....Qsc
-0000fc10: 694c 6578 6572 506f 7374 5363 7269 7074  iLexerPostScript
-0000fc20: 0103 0000 000e 004c 0069 0074 0065 0072  .......L.i.t.e.r
-0000fc30: 0061 006c 0800 0000 0006 0000 0007 4c69  .a.l..........Li
-0000fc40: 7465 7261 6c07 0000 0013 5173 6369 4c65  teral.....QsciLe
-0000fc50: 7865 7250 6f73 7453 6372 6970 7401 0300  xerPostScript...
-0000fc60: 0000 0800 4e00 6100 6d00 6508 0000 0000  ....N.a.m.e.....
-0000fc70: 0600 0000 044e 616d 6507 0000 0013 5173  .....Name.....Qs
-0000fc80: 6369 4c65 7865 7250 6f73 7453 6372 6970  ciLexerPostScrip
-0000fc90: 7401 0300 0000 0800 5a00 6100 6800 6c08  t.......Z.a.h.l.
-0000fca0: 0000 0000 0600 0000 064e 756d 6265 7207  .........Number.
-0000fcb0: 0000 0013 5173 6369 4c65 7865 7250 6f73  ....QsciLexerPos
-0000fcc0: 7453 6372 6970 7401 0300 0000 2000 5000  tScript..... .P.
-0000fcd0: 7200 6f00 7a00 6500 6400 7500 7200 6b00  r.o.z.e.d.u.r.k.
-0000fce0: 6c00 6100 6d00 6d00 6500 7200 6e08 0000  l.a.m.m.e.r.n...
-0000fcf0: 0000 0600 0000 1550 726f 6365 6475 7265  .......Procedure
-0000fd00: 2070 6172 656e 7468 6573 6973 0700 0000   parenthesis....
-0000fd10: 1351 7363 694c 6578 6572 506f 7374 5363  .QsciLexerPostSc
-0000fd20: 7269 7074 0103 0000 0008 0054 0065 0078  ript.......T.e.x
-0000fd30: 0074 0800 0000 0006 0000 0004 5465 7874  .t..........Text
-0000fd40: 0700 0000 1351 7363 694c 6578 6572 506f  .....QsciLexerPo
-0000fd50: 7374 5363 7269 7074 0103 0000 0012 005a  stScript.......Z
-0000fd60: 0075 0077 0065 0069 0073 0075 006e 0067  .u.w.e.i.s.u.n.g
-0000fd70: 0800 0000 0006 0000 000a 4173 7369 676e  ..........Assign
-0000fd80: 6d65 6e74 0700 0000 1351 7363 694c 6578  ment.....QsciLex
-0000fd90: 6572 5072 6f70 6572 7469 6573 0103 0000  erProperties....
-0000fda0: 0012 004b 006f 006d 006d 0065 006e 0074  ...K.o.m.m.e.n.t
-0000fdb0: 0061 0072 0800 0000 0006 0000 0007 436f  .a.r..........Co
-0000fdc0: 6d6d 656e 7407 0000 0013 5173 6369 4c65  mment.....QsciLe
-0000fdd0: 7865 7250 726f 7065 7274 6965 7301 0300  xerProperties...
-0000fde0: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
-0000fdf0: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
-0000fe00: 6175 6c74 0700 0000 1351 7363 694c 6578  ault.....QsciLex
-0000fe10: 6572 5072 6f70 6572 7469 6573 0103 0000  erProperties....
-0000fe20: 0018 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
-0000fe30: 0064 0077 0065 0072 0074 0800 0000 0006  .d.w.e.r.t......
-0000fe40: 0000 000d 4465 6661 756c 7420 7661 6c75  ....Default valu
-0000fe50: 6507 0000 0013 5173 6369 4c65 7865 7250  e.....QsciLexerP
-0000fe60: 726f 7065 7274 6965 7301 0300 0000 1200  roperties.......
-0000fe70: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
-0000fe80: 6c08 0000 0000 0600 0000 034b 6579 0700  l..........Key..
-0000fe90: 0000 1351 7363 694c 6578 6572 5072 6f70  ...QsciLexerProp
-0000fea0: 6572 7469 6573 0103 0000 0012 0041 0062  erties.......A.b
-0000feb0: 0073 0063 0068 006e 0069 0074 0074 0800  .s.c.h.n.i.t.t..
-0000fec0: 0000 0006 0000 0007 5365 6374 696f 6e07  ........Section.
-0000fed0: 0000 0013 5173 6369 4c65 7865 7250 726f  ....QsciLexerPro
-0000fee0: 7065 7274 6965 7301 0300 0000 1600 4b00  perties.......K.
-0000fef0: 6c00 6100 7300 7300 6500 6e00 6e00 6100  l.a.s.s.e.n.n.a.
-0000ff00: 6d00 6508 0000 0000 0600 0000 0a43 6c61  m.e..........Cla
-0000ff10: 7373 206e 616d 6507 0000 000f 5173 6369  ss name.....Qsci
-0000ff20: 4c65 7865 7250 7974 686f 6e01 0300 0000  LexerPython.....
-0000ff30: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
-0000ff40: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
-0000ff50: 6d65 6e74 0700 0000 0f51 7363 694c 6578  ment.....QsciLex
-0000ff60: 6572 5079 7468 6f6e 0103 0000 001c 004b  erPython.......K
-0000ff70: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-0000ff80: 0062 006c 006f 0063 006b 0800 0000 0006  .b.l.o.c.k......
-0000ff90: 0000 000d 436f 6d6d 656e 7420 626c 6f63  ....Comment bloc
-0000ffa0: 6b07 0000 000f 5173 6369 4c65 7865 7250  k.....QsciLexerP
-0000ffb0: 7974 686f 6e01 0300 0000 1200 4400 6500  ython.......D.e.
-0000ffc0: 6b00 6f00 7200 6100 7400 6f00 7208 0000  k.o.r.a.t.o.r...
-0000ffd0: 0000 0600 0000 0944 6563 6f72 6174 6f72  .......Decorator
-0000ffe0: 0700 0000 0f51 7363 694c 6578 6572 5079  .....QsciLexerPy
-0000fff0: 7468 6f6e 0103 0000 0010 0053 0074 0061  thon.......S.t.a
-00010000: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
-00010010: 0000 0007 4465 6661 756c 7407 0000 000f  ....Default.....
-00010020: 5173 6369 4c65 7865 7250 7974 686f 6e01  QsciLexerPython.
-00010030: 0300 0000 4600 4600 2d00 5a00 6500 6900  ....F.F.-.Z.e.i.
-00010040: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00010050: 6500 2000 6900 6e00 2000 4100 6e00 6600  e. .i.n. .A.n.f.
-00010060: fc00 6800 7200 7500 6e00 6700 7300 7a00  ..h.r.u.n.g.s.z.
-00010070: 6500 6900 6300 6800 6500 6e08 0000 0000  e.i.c.h.e.n.....
-00010080: 0600 0000 1644 6f75 626c 652d 7175 6f74  .....Double-quot
-00010090: 6564 2066 2d73 7472 696e 6707 0000 000f  ed f-string.....
-000100a0: 5173 6369 4c65 7865 7250 7974 686f 6e01  QsciLexerPython.
-000100b0: 0300 0000 4200 5a00 6500 6900 6300 6800  ....B.Z.e.i.c.h.
-000100c0: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
-000100d0: 6900 6e00 2000 4100 6e00 6600 fc00 6800  i.n. .A.n.f...h.
-000100e0: 7200 7500 6e00 6700 7300 7a00 6500 6900  r.u.n.g.s.z.e.i.
-000100f0: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
-00010100: 1444 6f75 626c 652d 7175 6f74 6564 2073  .Double-quoted s
-00010110: 7472 696e 6707 0000 000f 5173 6369 4c65  tring.....QsciLe
-00010120: 7865 7250 7974 686f 6e01 0300 0000 3800  xerPython.....8.
-00010130: 4600 7500 6e00 6b00 7400 6900 6f00 6e00  F.u.n.k.t.i.o.n.
-00010140: 7300 2d00 2000 6f00 6400 6500 7200 2000  s.-. .o.d.e.r. .
-00010150: 4d00 6500 7400 6800 6f00 6400 6500 6e00  M.e.t.h.o.d.e.n.
-00010160: 6e00 6100 6d00 6508 0000 0000 0600 0000  n.a.m.e.........
-00010170: 1746 756e 6374 696f 6e20 6f72 206d 6574  .Function or met
-00010180: 686f 6420 6e61 6d65 0700 0000 0f51 7363  hod name.....Qsc
-00010190: 694c 6578 6572 5079 7468 6f6e 0103 0000  iLexerPython....
-000101a0: 0034 0048 0065 0072 0076 006f 0072 0067  .4.H.e.r.v.o.r.g
-000101b0: 0065 0068 006f 0062 0065 006e 0065 0072  .e.h.o.b.e.n.e.r
-000101c0: 0020 0042 0065 007a 0065 0069 0063 0068  . .B.e.z.e.i.c.h
-000101d0: 006e 0065 0072 0800 0000 0006 0000 0016  .n.e.r..........
-000101e0: 4869 6768 6c69 6768 7465 6420 6964 656e  Highlighted iden
-000101f0: 7469 6669 6572 0700 0000 0f51 7363 694c  tifier.....QsciL
-00010200: 6578 6572 5079 7468 6f6e 0103 0000 0014  exerPython......
-00010210: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
-00010220: 0065 0072 0800 0000 0006 0000 000a 4964  .e.r..........Id
-00010230: 656e 7469 6669 6572 0700 0000 0f51 7363  entifier.....Qsc
-00010240: 694c 6578 6572 5079 7468 6f6e 0103 0000  iLexerPython....
-00010250: 001a 0053 0063 0068 006c 00fc 0073 0073  ...S.c.h.l...s.s
-00010260: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
-00010270: 0006 0000 0007 4b65 7977 6f72 6407 0000  ......Keyword...
-00010280: 000f 5173 6369 4c65 7865 7250 7974 686f  ..QsciLexerPytho
-00010290: 6e01 0300 0000 0800 5a00 6100 6800 6c08  n.......Z.a.h.l.
-000102a0: 0000 0000 0600 0000 064e 756d 6265 7207  .........Number.
-000102b0: 0000 000f 5173 6369 4c65 7865 7250 7974  ....QsciLexerPyt
-000102c0: 686f 6e01 0300 0000 1000 4f00 7000 6500  hon.......O.p.e.
-000102d0: 7200 6100 7400 6f00 7208 0000 0000 0600  r.a.t.o.r.......
-000102e0: 0000 084f 7065 7261 746f 7207 0000 000f  ...Operator.....
-000102f0: 5173 6369 4c65 7865 7250 7974 686f 6e01  QsciLexerPython.
-00010300: 0300 0000 3a00 4600 2d00 5a00 6500 6900  ....:.F.-.Z.e.i.
-00010310: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00010320: 6500 2000 6900 6e00 2000 4800 6f00 6300  e. .i.n. .H.o.c.
-00010330: 6800 6b00 6f00 6d00 6d00 6100 7400 6108  h.k.o.m.m.a.t.a.
-00010340: 0000 0000 0600 0000 1653 696e 676c 652d  .........Single-
-00010350: 7175 6f74 6564 2066 2d73 7472 696e 6707  quoted f-string.
-00010360: 0000 000f 5173 6369 4c65 7865 7250 7974  ....QsciLexerPyt
-00010370: 686f 6e01 0300 0000 3600 5a00 6500 6900  hon.....6.Z.e.i.
-00010380: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00010390: 6500 2000 6900 6e00 2000 4800 6f00 6300  e. .i.n. .H.o.c.
-000103a0: 6800 6b00 6f00 6d00 6d00 6100 7400 6108  h.k.o.m.m.a.t.a.
-000103b0: 0000 0000 0600 0000 1453 696e 676c 652d  .........Single-
-000103c0: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
-000103d0: 000f 5173 6369 4c65 7865 7250 7974 686f  ..QsciLexerPytho
-000103e0: 6e01 0300 0000 5c00 4600 2d00 5a00 6500  n.....\.F.-.Z.e.
-000103f0: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
-00010400: 7400 6500 2000 6900 6e00 2000 6400 7200  t.e. .i.n. .d.r.
-00010410: 6500 6900 6600 6100 6300 6800 6500 6e00  e.i.f.a.c.h.e.n.
-00010420: 2000 4100 6e00 6600 fc00 6800 7200 7500   .A.n.f...h.r.u.
-00010430: 6e00 6700 7300 7a00 6500 6900 6300 6800  n.g.s.z.e.i.c.h.
-00010440: 6500 6e08 0000 0000 0600 0000 1d54 7269  e.n..........Tri
-00010450: 706c 6520 646f 7562 6c65 2d71 756f 7465  ple double-quote
-00010460: 6420 662d 7374 7269 6e67 0700 0000 0f51  d f-string.....Q
-00010470: 7363 694c 6578 6572 5079 7468 6f6e 0103  sciLexerPython..
-00010480: 0000 0058 005a 0065 0069 0063 0068 0065  ...X.Z.e.i.c.h.e
-00010490: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
-000104a0: 006e 0020 0064 0072 0065 0069 0066 0061  .n. .d.r.e.i.f.a
-000104b0: 0063 0068 0065 006e 0020 0041 006e 0066  .c.h.e.n. .A.n.f
-000104c0: 00fc 0068 0072 0075 006e 0067 0073 007a  ...h.r.u.n.g.s.z
-000104d0: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
-000104e0: 0006 0000 001b 5472 6970 6c65 2064 6f75  ......Triple dou
-000104f0: 626c 652d 7175 6f74 6564 2073 7472 696e  ble-quoted strin
-00010500: 6707 0000 000f 5173 6369 4c65 7865 7250  g.....QsciLexerP
-00010510: 7974 686f 6e01 0300 0000 5000 4600 2d00  ython.....P.F.-.
-00010520: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
-00010530: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
-00010540: 6400 7200 6500 6900 6600 6100 6300 6800  d.r.e.i.f.a.c.h.
-00010550: 6500 6e00 2000 4800 6f00 6300 6800 6b00  e.n. .H.o.c.h.k.
-00010560: 6f00 6d00 6d00 6100 7400 6108 0000 0000  o.m.m.a.t.a.....
-00010570: 0600 0000 1d54 7269 706c 6520 7369 6e67  .....Triple sing
-00010580: 6c65 2d71 756f 7465 6420 662d 7374 7269  le-quoted f-stri
-00010590: 6e67 0700 0000 0f51 7363 694c 6578 6572  ng.....QsciLexer
-000105a0: 5079 7468 6f6e 0103 0000 004c 005a 0065  Python.....L.Z.e
-000105b0: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
-000105c0: 0074 0065 0020 0069 006e 0020 0064 0072  .t.e. .i.n. .d.r
-000105d0: 0065 0069 0066 0061 0063 0068 0065 006e  .e.i.f.a.c.h.e.n
-000105e0: 0020 0048 006f 0063 0068 006b 006f 006d  . .H.o.c.h.k.o.m
-000105f0: 006d 0061 0074 0061 0800 0000 0006 0000  .m.a.t.a........
-00010600: 001b 5472 6970 6c65 2073 696e 676c 652d  ..Triple single-
-00010610: 7175 6f74 6564 2073 7472 696e 6707 0000  quoted string...
-00010620: 000f 5173 6369 4c65 7865 7250 7974 686f  ..QsciLexerPytho
-00010630: 6e01 0300 0000 2e00 5500 6e00 6200 6500  n.......U.n.b.e.
-00010640: 6500 6e00 6400 6500 7400 6500 2000 5a00  e.n.d.e.t.e. .Z.
-00010650: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
-00010660: 7400 7400 6508 0000 0000 0600 0000 0f55  t.t.e..........U
-00010670: 6e63 6c6f 7365 6420 7374 7269 6e67 0700  nclosed string..
-00010680: 0000 0f51 7363 694c 6578 6572 5079 7468  ...QsciLexerPyth
-00010690: 6f6e 0103 0000 001e 0025 0051 0020 005a  on.......%.Q. .Z
-000106a0: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
-000106b0: 0074 0074 0065 0800 0000 0006 0000 0009  .t.t.e..........
-000106c0: 2551 2073 7472 696e 6707 0000 000d 5173  %Q string.....Qs
-000106d0: 6369 4c65 7865 7252 7562 7901 0300 0000  ciLexerRuby.....
-000106e0: 1e00 2500 7100 2000 5a00 6500 6900 6300  ..%.q. .Z.e.i.c.
-000106f0: 6800 6500 6e00 6b00 6500 7400 7400 6508  h.e.n.k.e.t.t.e.
-00010700: 0000 0000 0600 0000 0925 7120 7374 7269  .........%q stri
-00010710: 6e67 0700 0000 0d51 7363 694c 6578 6572  ng.....QsciLexer
-00010720: 5275 6279 0103 0000 001e 0025 0072 0020  Ruby.......%.r. 
-00010730: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-00010740: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
-00010750: 0009 2572 2073 7472 696e 6707 0000 000d  ..%r string.....
-00010760: 5173 6369 4c65 7865 7252 7562 7901 0300  QsciLexerRuby...
-00010770: 0000 1e00 2500 7700 2000 5a00 6500 6900  ....%.w. .Z.e.i.
-00010780: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
-00010790: 6508 0000 0000 0600 0000 0925 7720 7374  e..........%w st
-000107a0: 7269 6e67 0700 0000 0d51 7363 694c 6578  ring.....QsciLex
-000107b0: 6572 5275 6279 0103 0000 001e 0025 0078  erRuby.......%.x
-000107c0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
-000107d0: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
-000107e0: 0000 0009 2578 2073 7472 696e 6707 0000  ....%x string...
-000107f0: 000d 5173 6369 4c65 7865 7252 7562 7901  ..QsciLexerRuby.
-00010800: 0300 0000 1200 4200 6100 6300 6b00 7400  ......B.a.c.k.t.
-00010810: 6900 6300 6b00 7308 0000 0000 0600 0000  i.c.k.s.........
-00010820: 0942 6163 6b74 6963 6b73 0700 0000 0d51  .Backticks.....Q
-00010830: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
-00010840: 0016 004b 006c 0061 0073 0073 0065 006e  ...K.l.a.s.s.e.n
-00010850: 006e 0061 006d 0065 0800 0000 0006 0000  .n.a.m.e........
-00010860: 000a 436c 6173 7320 6e61 6d65 0700 0000  ..Class name....
-00010870: 0d51 7363 694c 6578 6572 5275 6279 0103  .QsciLexerRuby..
-00010880: 0000 001e 004b 006c 0061 0073 0073 0065  .....K.l.a.s.s.e
-00010890: 006e 0076 0061 0072 0069 0061 0062 006c  .n.v.a.r.i.a.b.l
-000108a0: 0065 0800 0000 0006 0000 000e 436c 6173  .e..........Clas
-000108b0: 7320 7661 7269 6162 6c65 0700 0000 0d51  s variable.....Q
-000108c0: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
-000108d0: 0012 004b 006f 006d 006d 0065 006e 0074  ...K.o.m.m.e.n.t
-000108e0: 0061 0072 0800 0000 0006 0000 0007 436f  .a.r..........Co
-000108f0: 6d6d 656e 7407 0000 000d 5173 6369 4c65  mment.....QsciLe
-00010900: 7865 7252 7562 7901 0300 0000 1800 4400  xerRuby.......D.
-00010910: 6100 7400 6500 6e00 7300 6500 6b00 7400  a.t.e.n.s.e.k.t.
-00010920: 6900 6f00 6e08 0000 0000 0600 0000 0c44  i.o.n..........D
-00010930: 6174 6120 7365 6374 696f 6e07 0000 000d  ata section.....
-00010940: 5173 6369 4c65 7865 7252 7562 7901 0300  QsciLexerRuby...
-00010950: 0000 1000 5300 7400 6100 6e00 6400 6100  ....S.t.a.n.d.a.
-00010960: 7200 6408 0000 0000 0600 0000 0744 6566  r.d..........Def
-00010970: 6175 6c74 0700 0000 0d51 7363 694c 6578  ault.....QsciLex
-00010980: 6572 5275 6279 0103 0000 003a 007a 0075  erRuby.....:.z.u
-00010990: 0072 00fc 0063 006b 0067 0065 0073 0074  .r...c.k.g.e.s.t
-000109a0: 0075 0066 0074 0065 0073 0020 0053 0063  .u.f.t.e.s. .S.c
-000109b0: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
-000109c0: 006f 0072 0074 0800 0000 0006 0000 000f  .o.r.t..........
-000109d0: 4465 6d6f 7465 6420 6b65 7977 6f72 6407  Demoted keyword.
-000109e0: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
-000109f0: 7901 0300 0000 4200 5a00 6500 6900 6300  y.....B.Z.e.i.c.
-00010a00: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
-00010a10: 2000 6900 6e00 2000 4100 6e00 6600 fc00   .i.n. .A.n.f...
-00010a20: 6800 7200 7500 6e00 6700 7300 7a00 6500  h.r.u.n.g.s.z.e.
-00010a30: 6900 6300 6800 6500 6e08 0000 0000 0600  i.c.h.e.n.......
-00010a40: 0000 1444 6f75 626c 652d 7175 6f74 6564  ...Double-quoted
-00010a50: 2073 7472 696e 6707 0000 000d 5173 6369   string.....Qsci
-00010a60: 4c65 7865 7252 7562 7901 0300 0000 0c00  LexerRuby.......
-00010a70: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
-00010a80: 0600 0000 0545 7272 6f72 0700 0000 0d51  .....Error.....Q
-00010a90: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
-00010aa0: 0038 0046 0075 006e 006b 0074 0069 006f  .8.F.u.n.k.t.i.o
-00010ab0: 006e 0073 002d 0020 006f 0064 0065 0072  .n.s.-. .o.d.e.r
-00010ac0: 0020 004d 0065 0074 0068 006f 0064 0065  . .M.e.t.h.o.d.e
-00010ad0: 006e 006e 0061 006d 0065 0800 0000 0006  .n.n.a.m.e......
-00010ae0: 0000 0017 4675 6e63 7469 6f6e 206f 7220  ....Function or 
-00010af0: 6d65 7468 6f64 206e 616d 6507 0000 000d  method name.....
-00010b00: 5173 6369 4c65 7865 7252 7562 7901 0300  QsciLexerRuby...
-00010b10: 0000 0c00 4700 6c00 6f00 6200 6100 6c08  ....G.l.o.b.a.l.
-00010b20: 0000 0000 0600 0000 0647 6c6f 6261 6c07  .........Global.
-00010b30: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
-00010b40: 7901 0300 0000 1a00 4800 6500 7200 6500  y.......H.e.r.e.
-00010b50: 2000 4400 6f00 6b00 7500 6d00 6500 6e00   .D.o.k.u.m.e.n.
-00010b60: 7408 0000 0000 0600 0000 0d48 6572 6520  t..........Here 
-00010b70: 646f 6375 6d65 6e74 0700 0000 0d51 7363  document.....Qsc
-00010b80: 694c 6578 6572 5275 6279 0103 0000 002e  iLexerRuby......
-00010b90: 0048 0065 0072 0065 0020 0044 006f 006b  .H.e.r.e. .D.o.k
-00010ba0: 0075 006d 0065 006e 0074 002d 0042 0065  .u.m.e.n.t.-.B.e
-00010bb0: 0067 0072 0065 006e 007a 0065 0072 0800  .g.r.e.n.z.e.r..
-00010bc0: 0000 0006 0000 0017 4865 7265 2064 6f63  ........Here doc
-00010bd0: 756d 656e 7420 6465 6c69 6d69 7465 7207  ument delimiter.
-00010be0: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
-00010bf0: 7901 0300 0000 1400 4200 6500 7a00 6500  y.......B.e.z.e.
-00010c00: 6900 6300 6800 6e00 6500 7208 0000 0000  i.c.h.n.e.r.....
-00010c10: 0600 0000 0a49 6465 6e74 6966 6965 7207  .....Identifier.
-00010c20: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
-00010c30: 7901 0300 0000 1e00 4900 6e00 7300 7400  y.......I.n.s.t.
-00010c40: 6100 6e00 7a00 7600 6100 7200 6900 6100  a.n.z.v.a.r.i.a.
-00010c50: 6200 6c00 6508 0000 0000 0600 0000 1149  b.l.e..........I
-00010c60: 6e73 7461 6e63 6520 7661 7269 6162 6c65  nstance variable
-00010c70: 0700 0000 0d51 7363 694c 6578 6572 5275  .....QsciLexerRu
-00010c80: 6279 0103 0000 001a 0053 0063 0068 006c  by.......S.c.h.l
-00010c90: 00fc 0073 0073 0065 006c 0077 006f 0072  ...s.s.e.l.w.o.r
-00010ca0: 0074 0800 0000 0006 0000 0007 4b65 7977  .t..........Keyw
-00010cb0: 6f72 6407 0000 000d 5173 6369 4c65 7865  ord.....QsciLexe
-00010cc0: 7252 7562 7901 0300 0000 1200 4d00 6f00  rRuby.......M.o.
-00010cd0: 6400 7500 6c00 6e00 6100 6d00 6508 0000  d.u.l.n.a.m.e...
-00010ce0: 0000 0600 0000 0b4d 6f64 756c 6520 6e61  .......Module na
-00010cf0: 6d65 0700 0000 0d51 7363 694c 6578 6572  me.....QsciLexer
-00010d00: 5275 6279 0103 0000 0008 005a 0061 0068  Ruby.......Z.a.h
-00010d10: 006c 0800 0000 0006 0000 0006 4e75 6d62  .l..........Numb
-00010d20: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
-00010d30: 5275 6279 0103 0000 0010 004f 0070 0065  Ruby.......O.p.e
-00010d40: 0072 0061 0074 006f 0072 0800 0000 0006  .r.a.t.o.r......
-00010d50: 0000 0008 4f70 6572 6174 6f72 0700 0000  ....Operator....
-00010d60: 0d51 7363 694c 6578 6572 5275 6279 0103  .QsciLexerRuby..
-00010d70: 0000 0006 0050 004f 0044 0800 0000 0006  .....P.O.D......
-00010d80: 0000 0003 504f 4407 0000 000d 5173 6369  ....POD.....Qsci
-00010d90: 4c65 7865 7252 7562 7901 0300 0000 2400  LexerRuby.....$.
-00010da0: 5200 6500 6700 7500 6c00 e400 7200 6500  R.e.g.u.l...r.e.
-00010db0: 7200 2000 4100 7500 7300 6400 7200 7500  r. .A.u.s.d.r.u.
-00010dc0: 6300 6b08 0000 0000 0600 0000 1252 6567  c.k..........Reg
-00010dd0: 756c 6172 2065 7870 7265 7373 696f 6e07  ular expression.
-00010de0: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
-00010df0: 7901 0300 0000 3600 5a00 6500 6900 6300  y.....6.Z.e.i.c.
-00010e00: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
-00010e10: 2000 6900 6e00 2000 4800 6f00 6300 6800   .i.n. .H.o.c.h.
-00010e20: 6b00 6f00 6d00 6d00 6100 7400 6108 0000  k.o.m.m.a.t.a...
-00010e30: 0000 0600 0000 1453 696e 676c 652d 7175  .......Single-qu
-00010e40: 6f74 6564 2073 7472 696e 6707 0000 000d  oted string.....
-00010e50: 5173 6369 4c65 7865 7252 7562 7901 0300  QsciLexerRuby...
-00010e60: 0000 0c00 5300 7900 6d00 6200 6f00 6c08  ....S.y.m.b.o.l.
-00010e70: 0000 0000 0600 0000 0653 796d 626f 6c07  .........Symbol.
-00010e80: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
-00010e90: 7901 0300 0000 0c00 5300 7400 6400 6500  y.......S.t.d.e.
-00010ea0: 7200 7208 0000 0000 0600 0000 0673 7464  r.r..........std
-00010eb0: 6572 7207 0000 000d 5173 6369 4c65 7865  err.....QsciLexe
-00010ec0: 7252 7562 7901 0300 0000 0a00 5300 7400  rRuby.......S.t.
-00010ed0: 6400 6900 6e08 0000 0000 0600 0000 0573  d.i.n..........s
-00010ee0: 7464 696e 0700 0000 0d51 7363 694c 6578  tdin.....QsciLex
-00010ef0: 6572 5275 6279 0103 0000 000c 0053 0074  erRuby.......S.t
-00010f00: 0064 006f 0075 0074 0800 0000 0006 0000  .d.o.u.t........
-00010f10: 0006 7374 646f 7574 0700 0000 0d51 7363  ..stdout.....Qsc
-00010f20: 694c 6578 6572 5275 6279 0103 0000 0020  iLexerRuby..... 
-00010f30: 0023 0020 004b 006f 006d 006d 0065 006e  .#. .K.o.m.m.e.n
-00010f40: 0074 0061 0072 007a 0065 0069 006c 0065  .t.a.r.z.e.i.l.e
-00010f50: 0800 0000 0006 0000 000e 2320 636f 6d6d  ..........# comm
-00010f60: 656e 7420 6c69 6e65 0700 0000 0c51 7363  ent line.....Qsc
-00010f70: 694c 6578 6572 5351 4c01 0300 0000 1200  iLexerSQL.......
-00010f80: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
-00010f90: 7208 0000 0000 0600 0000 0743 6f6d 6d65  r..........Comme
-00010fa0: 6e74 0700 0000 0c51 7363 694c 6578 6572  nt.....QsciLexer
-00010fb0: 5351 4c01 0300 0000 1c00 4b00 6f00 6d00  SQL.......K.o.m.
-00010fc0: 6d00 6500 6e00 7400 6100 7200 7a00 6500  m.e.n.t.a.r.z.e.
-00010fd0: 6900 6c00 6508 0000 0000 0600 0000 0c43  i.l.e..........C
-00010fe0: 6f6d 6d65 6e74 206c 696e 6507 0000 000c  omment line.....
-00010ff0: 5173 6369 4c65 7865 7253 514c 0103 0000  QsciLexerSQL....
-00011000: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
-00011010: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
-00011020: 756c 7407 0000 000c 5173 6369 4c65 7865  ult.....QsciLexe
-00011030: 7253 514c 0103 0000 0042 005a 0065 0069  rSQL.....B.Z.e.i
-00011040: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00011050: 0065 0020 0069 006e 0020 0041 006e 0066  .e. .i.n. .A.n.f
-00011060: 00fc 0068 0072 0075 006e 0067 0073 007a  ...h.r.u.n.g.s.z
-00011070: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
-00011080: 0006 0000 0014 446f 7562 6c65 2d71 756f  ......Double-quo
-00011090: 7465 6420 7374 7269 6e67 0700 0000 0c51  ted string.....Q
-000110a0: 7363 694c 6578 6572 5351 4c01 0300 0000  sciLexerSQL.....
-000110b0: 1400 4200 6500 7a00 6500 6900 6300 6800  ..B.e.z.e.i.c.h.
-000110c0: 6e00 6500 7208 0000 0000 0600 0000 0a49  n.e.r..........I
-000110d0: 6465 6e74 6966 6965 7207 0000 000c 5173  dentifier.....Qs
-000110e0: 6369 4c65 7865 7253 514c 0103 0000 002a  ciLexerSQL.....*
-000110f0: 004a 0061 0076 0061 0044 006f 0063 0020  .J.a.v.a.D.o.c. 
-00011100: 0053 0063 0068 006c 00fc 0073 0073 0065  .S.c.h.l...s.s.e
-00011110: 006c 0077 006f 0072 0074 0800 0000 0006  .l.w.o.r.t......
-00011120: 0000 000f 4a61 7661 446f 6320 6b65 7977  ....JavaDoc keyw
-00011130: 6f72 6407 0000 000c 5173 6369 4c65 7865  ord.....QsciLexe
-00011140: 7253 514c 0103 0000 0036 004a 0061 0076  rSQL.....6.J.a.v
-00011150: 0061 0044 006f 0063 0020 0053 0063 0068  .a.D.o.c. .S.c.h
-00011160: 006c 00fc 0073 0073 0065 006c 0077 006f  .l...s.s.e.l.w.o
-00011170: 0072 0074 0066 0065 0068 006c 0065 0072  .r.t.f.e.h.l.e.r
-00011180: 0800 0000 0006 0000 0015 4a61 7661 446f  ..........JavaDo
-00011190: 6320 6b65 7977 6f72 6420 6572 726f 7207  c keyword error.
-000111a0: 0000 000c 5173 6369 4c65 7865 7253 514c  ....QsciLexerSQL
-000111b0: 0103 0000 0022 004a 0061 0076 0061 0044  .....".J.a.v.a.D
-000111c0: 006f 0063 0020 004b 006f 006d 006d 0065  .o.c. .K.o.m.m.e
-000111d0: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
-000111e0: 0015 4a61 7661 446f 6320 7374 796c 6520  ..JavaDoc style 
-000111f0: 636f 6d6d 656e 7407 0000 000c 5173 6369  comment.....Qsci
-00011200: 4c65 7865 7253 514c 0103 0000 001a 0053  LexerSQL.......S
-00011210: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
-00011220: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
-00011230: 0007 4b65 7977 6f72 6407 0000 000c 5173  ..Keyword.....Qs
-00011240: 6369 4c65 7865 7253 514c 0103 0000 0008  ciLexerSQL......
-00011250: 005a 0061 0068 006c 0800 0000 0006 0000  .Z.a.h.l........
-00011260: 0006 4e75 6d62 6572 0700 0000 0c51 7363  ..Number.....Qsc
-00011270: 694c 6578 6572 5351 4c01 0300 0000 1000  iLexerSQL.......
-00011280: 4f00 7000 6500 7200 6100 7400 6f00 7208  O.p.e.r.a.t.o.r.
-00011290: 0000 0000 0600 0000 084f 7065 7261 746f  .........Operato
-000112a0: 7207 0000 000c 5173 6369 4c65 7865 7253  r.....QsciLexerS
-000112b0: 514c 0103 0000 003e 0042 0065 007a 0065  QL.....>.B.e.z.e
-000112c0: 0069 0063 0068 006e 0065 0072 0020 0069  .i.c.h.n.e.r. .i
-000112d0: 006e 0020 0041 006e 0066 00fc 0068 0072  .n. .A.n.f...h.r
-000112e0: 0075 006e 0067 0073 007a 0065 0069 0063  .u.n.g.s.z.e.i.c
-000112f0: 0068 0065 006e 0800 0000 0006 0000 0011  .h.e.n..........
-00011300: 5175 6f74 6564 2069 6465 6e74 6966 6965  Quoted identifie
-00011310: 7207 0000 000c 5173 6369 4c65 7865 7253  r.....QsciLexerS
-00011320: 514c 0103 0000 003a 004f 0070 0065 0072  QL.....:.O.p.e.r
-00011330: 0061 0074 006f 0072 0020 0069 006e 0020  .a.t.o.r. .i.n. 
-00011340: 0041 006e 0066 00fc 0068 0072 0075 006e  .A.n.f...h.r.u.n
-00011350: 0067 0073 007a 0065 0069 0063 0068 0065  .g.s.z.e.i.c.h.e
-00011360: 006e 0800 0000 0006 0000 000f 5175 6f74  .n..........Quot
-00011370: 6564 206f 7065 7261 746f 7207 0000 000c  ed operator.....
-00011380: 5173 6369 4c65 7865 7253 514c 0103 0000  QsciLexerSQL....
-00011390: 0024 0053 0051 004c 002a 0050 006c 0075  .$.S.Q.L.*.P.l.u
-000113a0: 0073 0020 004b 006f 006d 006d 0065 006e  .s. .K.o.m.m.e.n
-000113b0: 0074 0061 0072 0800 0000 0006 0000 0010  .t.a.r..........
-000113c0: 5351 4c2a 506c 7573 2063 6f6d 6d65 6e74  SQL*Plus comment
-000113d0: 0700 0000 0c51 7363 694c 6578 6572 5351  .....QsciLexerSQ
-000113e0: 4c01 0300 0000 2c00 5300 5100 4c00 2a00  L.....,.S.Q.L.*.
-000113f0: 5000 6c00 7500 7300 2000 5300 6300 6800  P.l.u.s. .S.c.h.
-00011400: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
-00011410: 7200 7408 0000 0000 0600 0000 1053 514c  r.t..........SQL
-00011420: 2a50 6c75 7320 6b65 7977 6f72 6407 0000  *Plus keyword...
-00011430: 000c 5173 6369 4c65 7865 7253 514c 0103  ..QsciLexerSQL..
-00011440: 0000 0020 0053 0051 004c 002a 0050 006c  ... .S.Q.L.*.P.l
-00011450: 0075 0073 0020 0045 0069 006e 0067 0061  .u.s. .E.i.n.g.a
-00011460: 0062 0065 0800 0000 0006 0000 000f 5351  .b.e..........SQ
-00011470: 4c2a 506c 7573 2070 726f 6d70 7407 0000  L*Plus prompt...
-00011480: 000c 5173 6369 4c65 7865 7253 514c 0103  ..QsciLexerSQL..
-00011490: 0000 0036 005a 0065 0069 0063 0068 0065  ...6.Z.e.i.c.h.e
-000114a0: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
-000114b0: 006e 0020 0048 006f 0063 0068 006b 006f  .n. .H.o.c.h.k.o
-000114c0: 006d 006d 0061 0074 0061 0800 0000 0006  .m.m.a.t.a......
-000114d0: 0000 0014 5369 6e67 6c65 2d71 756f 7465  ....Single-quote
-000114e0: 6420 7374 7269 6e67 0700 0000 0c51 7363  d string.....Qsc
-000114f0: 694c 6578 6572 5351 4c01 0300 0000 2400  iLexerSQL.....$.
-00011500: 4e00 7500 7400 7a00 6500 7200 2000 6400  N.u.t.z.e.r. .d.
-00011510: 6500 6600 6900 6e00 6900 6500 7200 7400  e.f.i.n.i.e.r.t.
-00011520: 2000 3108 0000 0000 0600 0000 0e55 7365   .1..........Use
-00011530: 7220 6465 6669 6e65 6420 3107 0000 000c  r defined 1.....
-00011540: 5173 6369 4c65 7865 7253 514c 0103 0000  QsciLexerSQL....
-00011550: 0024 004e 0075 0074 007a 0065 0072 0020  .$.N.u.t.z.e.r. 
-00011560: 0064 0065 0066 0069 006e 0069 0065 0072  .d.e.f.i.n.i.e.r
-00011570: 0074 0020 0032 0800 0000 0006 0000 000e  .t. .2..........
-00011580: 5573 6572 2064 6566 696e 6564 2032 0700  User defined 2..
-00011590: 0000 0c51 7363 694c 6578 6572 5351 4c01  ...QsciLexerSQL.
-000115a0: 0300 0000 2400 4e00 7500 7400 7a00 6500  ....$.N.u.t.z.e.
-000115b0: 7200 2000 6400 6500 6600 6900 6e00 6900  r. .d.e.f.i.n.i.
-000115c0: 6500 7200 7400 2000 3308 0000 0000 0600  e.r.t. .3.......
-000115d0: 0000 0e55 7365 7220 6465 6669 6e65 6420  ...User defined 
-000115e0: 3307 0000 000c 5173 6369 4c65 7865 7253  3.....QsciLexerS
-000115f0: 514c 0103 0000 0024 004e 0075 0074 007a  QL.....$.N.u.t.z
-00011600: 0065 0072 0020 0064 0065 0066 0069 006e  .e.r. .d.e.f.i.n
-00011610: 0069 0065 0072 0074 0020 0034 0800 0000  .i.e.r.t. .4....
-00011620: 0006 0000 000e 5573 6572 2064 6566 696e  ......User defin
-00011630: 6564 2034 0700 0000 0c51 7363 694c 6578  ed 4.....QsciLex
-00011640: 6572 5351 4c01 0300 0000 0c00 4200 6500  erSQL.......B.e.
-00011650: 6600 6500 6800 6c08 0000 0000 0600 0000  f.e.h.l.........
-00011660: 0743 6f6d 6d61 6e64 0700 0000 0e51 7363  .Command.....Qsc
-00011670: 694c 6578 6572 5370 6963 6501 0300 0000  iLexerSpice.....
-00011680: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
-00011690: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
-000116a0: 6d65 6e74 0700 0000 0e51 7363 694c 6578  ment.....QsciLex
-000116b0: 6572 5370 6963 6501 0300 0000 1000 5300  erSpice.......S.
-000116c0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
-000116d0: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
-000116e0: 0000 0e51 7363 694c 6578 6572 5370 6963  ...QsciLexerSpic
-000116f0: 6501 0300 0000 1200 4400 6500 6c00 6900  e.......D.e.l.i.
-00011700: 6d00 6900 7400 6500 7208 0000 0000 0600  m.i.t.e.r.......
-00011710: 0000 0944 656c 696d 6974 6572 0700 0000  ...Delimiter....
-00011720: 0e51 7363 694c 6578 6572 5370 6963 6501  .QsciLexerSpice.
-00011730: 0300 0000 1000 4600 7500 6e00 6b00 7400  ......F.u.n.k.t.
-00011740: 6900 6f00 6e08 0000 0000 0600 0000 0846  i.o.n..........F
-00011750: 756e 6374 696f 6e07 0000 000e 5173 6369  unction.....Qsci
-00011760: 4c65 7865 7253 7069 6365 0103 0000 0014  LexerSpice......
-00011770: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
-00011780: 0065 0072 0800 0000 0006 0000 000a 4964  .e.r..........Id
-00011790: 656e 7469 6669 6572 0700 0000 0e51 7363  entifier.....Qsc
-000117a0: 694c 6578 6572 5370 6963 6501 0300 0000  iLexerSpice.....
-000117b0: 0800 5a00 6100 6800 6c08 0000 0000 0600  ..Z.a.h.l.......
-000117c0: 0000 064e 756d 6265 7207 0000 000e 5173  ...Number.....Qs
-000117d0: 6369 4c65 7865 7253 7069 6365 0103 0000  ciLexerSpice....
-000117e0: 0012 0050 0061 0072 0061 006d 0065 0074  ...P.a.r.a.m.e.t
-000117f0: 0065 0072 0800 0000 0006 0000 0009 5061  .e.r..........Pa
-00011800: 7261 6d65 7465 7207 0000 000e 5173 6369  rameter.....Qsci
-00011810: 4c65 7865 7253 7069 6365 0103 0000 0008  LexerSpice......
-00011820: 0057 0065 0072 0074 0800 0000 0006 0000  .W.e.r.t........
-00011830: 0005 5661 6c75 6507 0000 000e 5173 6369  ..Value.....Qsci
-00011840: 4c65 7865 7253 7069 6365 0103 0000 0020  LexerSpice..... 
-00011850: 004b 006c 0061 006d 006d 0065 0072 0065  .K.l.a.m.m.e.r.e
-00011860: 0072 0073 0065 0074 007a 0075 006e 0067  .r.s.e.t.z.u.n.g
-00011870: 0800 0000 0006 0000 0012 4272 6163 6520  ..........Brace 
-00011880: 7375 6273 7469 7475 7469 6f6e 0700 0000  substitution....
-00011890: 0c51 7363 694c 6578 6572 5443 4c01 0300  .QsciLexerTCL...
-000118a0: 0000 1200 4b00 6f00 6d00 6d00 6500 6e00  ....K.o.m.m.e.n.
-000118b0: 7400 6100 7208 0000 0000 0600 0000 0743  t.a.r..........C
-000118c0: 6f6d 6d65 6e74 0700 0000 0c51 7363 694c  omment.....QsciL
-000118d0: 6578 6572 5443 4c01 0300 0000 1c00 4b00  exerTCL.......K.
-000118e0: 6f00 6d00 6d00 6500 6e00 7400 6100 7200  o.m.m.e.n.t.a.r.
-000118f0: 6200 6c00 6f00 6300 6b08 0000 0000 0600  b.l.o.c.k.......
-00011900: 0000 0d43 6f6d 6d65 6e74 2062 6c6f 636b  ...Comment block
-00011910: 0700 0000 0c51 7363 694c 6578 6572 5443  .....QsciLexerTC
-00011920: 4c01 0300 0000 1800 4b00 6f00 6d00 6d00  L.......K.o.m.m.
-00011930: 6500 6e00 7400 6100 7200 6200 6f00 7808  e.n.t.a.r.b.o.x.
-00011940: 0000 0000 0600 0000 0b43 6f6d 6d65 6e74  .........Comment
-00011950: 2062 6f78 0700 0000 0c51 7363 694c 6578   box.....QsciLex
-00011960: 6572 5443 4c01 0300 0000 1c00 4b00 6f00  erTCL.......K.o.
-00011970: 6d00 6d00 6500 6e00 7400 6100 7200 7a00  m.m.e.n.t.a.r.z.
-00011980: 6500 6900 6c00 6508 0000 0000 0600 0000  e.i.l.e.........
-00011990: 0c43 6f6d 6d65 6e74 206c 696e 6507 0000  .Comment line...
-000119a0: 000c 5173 6369 4c65 7865 7254 434c 0103  ..QsciLexerTCL..
-000119b0: 0000 0010 0053 0074 0061 006e 0064 0061  .....S.t.a.n.d.a
-000119c0: 0072 0064 0800 0000 0006 0000 0007 4465  .r.d..........De
-000119d0: 6661 756c 7407 0000 000c 5173 6369 4c65  fault.....QsciLe
-000119e0: 7865 7254 434c 0103 0000 0032 0045 0072  xerTCL.....2.E.r
-000119f0: 0077 0065 0069 0074 0065 0072 0075 006e  .w.e.i.t.e.r.u.n
-00011a00: 0067 0073 0073 0063 0068 006c 00fc 0073  .g.s.s.c.h.l...s
-00011a10: 0073 0065 006c 0077 006f 0072 0074 0800  .s.e.l.w.o.r.t..
-00011a20: 0000 0006 0000 000e 4578 7061 6e64 206b  ........Expand k
-00011a30: 6579 776f 7264 0700 0000 0c51 7363 694c  eyword.....QsciL
-00011a40: 6578 6572 5443 4c01 0300 0000 1400 4200  exerTCL.......B.
-00011a50: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
-00011a60: 7208 0000 0000 0600 0000 0a49 6465 6e74  r..........Ident
-00011a70: 6966 6965 7207 0000 000c 5173 6369 4c65  ifier.....QsciLe
-00011a80: 7865 7254 434c 0103 0000 0018 004d 006f  xerTCL.......M.o
-00011a90: 0064 0069 0066 0069 007a 0069 0065 0072  .d.i.f.i.z.i.e.r
-00011aa0: 0065 0072 0800 0000 0006 0000 0008 4d6f  .e.r..........Mo
-00011ab0: 6469 6669 6572 0700 0000 0c51 7363 694c  difier.....QsciL
-00011ac0: 6578 6572 5443 4c01 0300 0000 0800 5a00  exerTCL.......Z.
-00011ad0: 6100 6800 6c08 0000 0000 0600 0000 064e  a.h.l..........N
-00011ae0: 756d 6265 7207 0000 000c 5173 6369 4c65  umber.....QsciLe
-00011af0: 7865 7254 434c 0103 0000 0010 004f 0070  xerTCL.......O.p
-00011b00: 0065 0072 0061 0074 006f 0072 0800 0000  .e.r.a.t.o.r....
-00011b10: 0006 0000 0008 4f70 6572 6174 6f72 0700  ......Operator..
-00011b20: 0000 0c51 7363 694c 6578 6572 5443 4c01  ...QsciLexerTCL.
-00011b30: 0300 0000 3200 6100 6e00 6700 6500 6600  ....2.a.n.g.e.f.
-00011b40: fc00 6800 7200 7400 6500 7300 2000 5300  ..h.r.t.e.s. .S.
-00011b50: 6300 6800 6c00 fc00 7300 7300 6500 6c00  c.h.l...s.s.e.l.
-00011b60: 7700 6f00 7200 7408 0000 0000 0600 0000  w.o.r.t.........
-00011b70: 0e51 756f 7465 6420 6b65 7977 6f72 6407  .Quoted keyword.
-00011b80: 0000 000c 5173 6369 4c65 7865 7254 434c  ....QsciLexerTCL
-00011b90: 0103 0000 0018 005a 0065 0069 0063 0068  .......Z.e.i.c.h
-00011ba0: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
-00011bb0: 0000 0006 0000 000d 5175 6f74 6564 2073  ........Quoted s
-00011bc0: 7472 696e 6707 0000 000c 5173 6369 4c65  tring.....QsciLe
-00011bd0: 7865 7254 434c 0103 0000 0012 0045 0072  xerTCL.......E.r
-00011be0: 0073 0065 0074 007a 0075 006e 0067 0800  .s.e.t.z.u.n.g..
-00011bf0: 0000 0006 0000 000c 5375 6273 7469 7475  ........Substitu
-00011c00: 7469 6f6e 0700 0000 0c51 7363 694c 6578  tion.....QsciLex
-00011c10: 6572 5443 4c01 0300 0000 2200 5400 4300  erTCL.....".T.C.
-00011c20: 4c00 2000 5300 6300 6800 6c00 fc00 7300  L. .S.c.h.l...s.
-00011c30: 7300 6500 6c00 7700 6f00 7200 7408 0000  s.e.l.w.o.r.t...
-00011c40: 0000 0600 0000 0b54 434c 206b 6579 776f  .......TCL keywo
-00011c50: 7264 0700 0000 0c51 7363 694c 6578 6572  rd.....QsciLexer
-00011c60: 5443 4c01 0300 0000 1200 5400 6b00 2000  TCL.......T.k. .
-00011c70: 4200 6500 6600 6500 6800 6c08 0000 0000  B.e.f.e.h.l.....
-00011c80: 0600 0000 0a54 6b20 636f 6d6d 616e 6407  .....Tk command.
-00011c90: 0000 000c 5173 6369 4c65 7865 7254 434c  ....QsciLexerTCL
-00011ca0: 0103 0000 0020 0054 006b 0020 0053 0063  ..... .T.k. .S.c
-00011cb0: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
-00011cc0: 006f 0072 0074 0800 0000 0006 0000 000a  .o.r.t..........
-00011cd0: 546b 206b 6579 776f 7264 0700 0000 0c51  Tk keyword.....Q
-00011ce0: 7363 694c 6578 6572 5443 4c01 0300 0000  sciLexerTCL.....
-00011cf0: 2400 4e00 7500 7400 7a00 6500 7200 2000  $.N.u.t.z.e.r. .
-00011d00: 6400 6500 6600 6900 6e00 6900 6500 7200  d.e.f.i.n.i.e.r.
-00011d10: 7400 2000 3108 0000 0000 0600 0000 0e55  t. .1..........U
-00011d20: 7365 7220 6465 6669 6e65 6420 3107 0000  ser defined 1...
-00011d30: 000c 5173 6369 4c65 7865 7254 434c 0103  ..QsciLexerTCL..
-00011d40: 0000 0024 004e 0075 0074 007a 0065 0072  ...$.N.u.t.z.e.r
-00011d50: 0020 0064 0065 0066 0069 006e 0069 0065  . .d.e.f.i.n.i.e
-00011d60: 0072 0074 0020 0032 0800 0000 0006 0000  .r.t. .2........
-00011d70: 000e 5573 6572 2064 6566 696e 6564 2032  ..User defined 2
-00011d80: 0700 0000 0c51 7363 694c 6578 6572 5443  .....QsciLexerTC
-00011d90: 4c01 0300 0000 2400 4e00 7500 7400 7a00  L.....$.N.u.t.z.
-00011da0: 6500 7200 2000 6400 6500 6600 6900 6e00  e.r. .d.e.f.i.n.
-00011db0: 6900 6500 7200 7400 2000 3308 0000 0000  i.e.r.t. .3.....
-00011dc0: 0600 0000 0e55 7365 7220 6465 6669 6e65  .....User define
-00011dd0: 6420 3307 0000 000c 5173 6369 4c65 7865  d 3.....QsciLexe
-00011de0: 7254 434c 0103 0000 0024 004e 0075 0074  rTCL.....$.N.u.t
-00011df0: 007a 0065 0072 0020 0064 0065 0066 0069  .z.e.r. .d.e.f.i
-00011e00: 006e 0069 0065 0072 0074 0020 0034 0800  .n.i.e.r.t. .4..
-00011e10: 0000 0006 0000 000e 5573 6572 2064 6566  ........User def
-00011e20: 696e 6564 2034 0700 0000 0c51 7363 694c  ined 4.....QsciL
-00011e30: 6578 6572 5443 4c01 0300 0000 2400 6900  exerTCL.....$.i.
-00011e40: 5400 4300 4c00 2000 5300 6300 6800 6c00  T.C.L. .S.c.h.l.
-00011e50: fc00 7300 7300 6500 6c00 7700 6f00 7200  ..s.s.e.l.w.o.r.
-00011e60: 7408 0000 0000 0600 0000 0c69 5443 4c20  t..........iTCL 
-00011e70: 6b65 7977 6f72 6407 0000 000c 5173 6369  keyword.....Qsci
-00011e80: 4c65 7865 7254 434c 0103 0000 000c 0042  LexerTCL.......B
-00011e90: 0065 0066 0065 0068 006c 0800 0000 0006  .e.f.e.h.l......
-00011ea0: 0000 0007 436f 6d6d 616e 6407 0000 000c  ....Command.....
-00011eb0: 5173 6369 4c65 7865 7254 6558 0103 0000  QsciLexerTeX....
-00011ec0: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
-00011ed0: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
-00011ee0: 756c 7407 0000 000c 5173 6369 4c65 7865  ult.....QsciLexe
-00011ef0: 7254 6558 0103 0000 000c 0047 0072 0075  rTeX.......G.r.u
-00011f00: 0070 0070 0065 0800 0000 0006 0000 0005  .p.p.e..........
-00011f10: 4772 6f75 7007 0000 000c 5173 6369 4c65  Group.....QsciLe
-00011f20: 7865 7254 6558 0103 0000 000e 0053 0070  xerTeX.......S.p
-00011f30: 0065 007a 0069 0061 006c 0800 0000 0006  .e.z.i.a.l......
-00011f40: 0000 0007 5370 6563 6961 6c07 0000 000c  ....Special.....
-00011f50: 5173 6369 4c65 7865 7254 6558 0103 0000  QsciLexerTeX....
-00011f60: 000c 0053 0079 006d 0062 006f 006c 0800  ...S.y.m.b.o.l..
-00011f70: 0000 0006 0000 0006 5379 6d62 6f6c 0700  ........Symbol..
-00011f80: 0000 0c51 7363 694c 6578 6572 5465 5801  ...QsciLexerTeX.
-00011f90: 0300 0000 0800 5400 6500 7800 7408 0000  ......T.e.x.t...
-00011fa0: 0000 0600 0000 0454 6578 7407 0000 000c  .......Text.....
-00011fb0: 5173 6369 4c65 7865 7254 6558 0103 0000  QsciLexerTeX....
-00011fc0: 0010 0041 0074 0074 0072 0069 0062 0075  ...A.t.t.r.i.b.u
-00011fd0: 0074 0800 0000 0006 0000 0009 4174 7472  .t..........Attr
-00011fe0: 6962 7574 6507 0000 000d 5173 6369 4c65  ibute.....QsciLe
-00011ff0: 7865 7256 4844 4c01 0300 0000 1200 4b00  xerVHDL.......K.
-00012000: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-00012010: 0000 0000 0600 0000 0743 6f6d 6d65 6e74  .........Comment
-00012020: 0700 0000 0d51 7363 694c 6578 6572 5648  .....QsciLexerVH
-00012030: 444c 0103 0000 001c 004b 006f 006d 006d  DL.......K.o.m.m
-00012040: 0065 006e 0074 0061 0072 0062 006c 006f  .e.n.t.a.r.b.l.o
-00012050: 0063 006b 0800 0000 0006 0000 000d 436f  .c.k..........Co
-00012060: 6d6d 656e 7420 626c 6f63 6b07 0000 000d  mment block.....
-00012070: 5173 6369 4c65 7865 7256 4844 4c01 0300  QsciLexerVHDL...
-00012080: 0000 1c00 4b00 6f00 6d00 6d00 6500 6e00  ....K.o.m.m.e.n.
-00012090: 7400 6100 7200 7a00 6500 6900 6c00 6508  t.a.r.z.e.i.l.e.
-000120a0: 0000 0000 0600 0000 0c43 6f6d 6d65 6e74  .........Comment
-000120b0: 206c 696e 6507 0000 000d 5173 6369 4c65   line.....QsciLe
-000120c0: 7865 7256 4844 4c01 0300 0000 1000 5300  xerVHDL.......S.
-000120d0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
-000120e0: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
-000120f0: 0000 0d51 7363 694c 6578 6572 5648 444c  ...QsciLexerVHDL
-00012100: 0103 0000 0014 0042 0065 007a 0065 0069  .......B.e.z.e.i
-00012110: 0063 0068 006e 0065 0072 0800 0000 0006  .c.h.n.e.r......
-00012120: 0000 000a 4964 656e 7469 6669 6572 0700  ....Identifier..
-00012130: 0000 0d51 7363 694c 6578 6572 5648 444c  ...QsciLexerVHDL
-00012140: 0103 0000 001a 0053 0063 0068 006c 00fc  .......S.c.h.l..
-00012150: 0073 0073 0065 006c 0077 006f 0072 0074  .s.s.e.l.w.o.r.t
-00012160: 0800 0000 0006 0000 0007 4b65 7977 6f72  ..........Keywor
-00012170: 6407 0000 000d 5173 6369 4c65 7865 7256  d.....QsciLexerV
-00012180: 4844 4c01 0300 0000 0800 5a00 6100 6800  HDL.......Z.a.h.
-00012190: 6c08 0000 0000 0600 0000 064e 756d 6265  l..........Numbe
-000121a0: 7207 0000 000d 5173 6369 4c65 7865 7256  r.....QsciLexerV
-000121b0: 4844 4c01 0300 0000 1000 4f00 7000 6500  HDL.......O.p.e.
-000121c0: 7200 6100 7400 6f00 7208 0000 0000 0600  r.a.t.o.r.......
-000121d0: 0000 084f 7065 7261 746f 7207 0000 000d  ...Operator.....
-000121e0: 5173 6369 4c65 7865 7256 4844 4c01 0300  QsciLexerVHDL...
-000121f0: 0000 2000 5300 7400 6100 6e00 6400 6100  .. .S.t.a.n.d.a.
-00012200: 7200 6400 6600 7500 6e00 6b00 7400 6900  r.d.f.u.n.k.t.i.
-00012210: 6f00 6e08 0000 0000 0600 0000 1153 7461  o.n..........Sta
-00012220: 6e64 6172 6420 6675 6e63 7469 6f6e 0700  ndard function..
-00012230: 0000 0d51 7363 694c 6578 6572 5648 444c  ...QsciLexerVHDL
-00012240: 0103 0000 0020 0053 0074 0061 006e 0064  ..... .S.t.a.n.d
-00012250: 0061 0072 0064 006f 0070 0065 0072 0061  .a.r.d.o.p.e.r.a
-00012260: 0074 006f 0072 0800 0000 0006 0000 0011  .t.o.r..........
-00012270: 5374 616e 6461 7264 206f 7065 7261 746f  Standard operato
-00012280: 7207 0000 000d 5173 6369 4c65 7865 7256  r.....QsciLexerV
-00012290: 4844 4c01 0300 0000 1a00 5300 7400 6100  HDL.......S.t.a.
-000122a0: 6e00 6400 6100 7200 6400 7000 6100 6b00  n.d.a.r.d.p.a.k.
-000122b0: 6500 7408 0000 0000 0600 0000 1053 7461  e.t..........Sta
-000122c0: 6e64 6172 6420 7061 636b 6167 6507 0000  ndard package...
-000122d0: 000d 5173 6369 4c65 7865 7256 4844 4c01  ..QsciLexerVHDL.
-000122e0: 0300 0000 1600 5300 7400 6100 6e00 6400  ......S.t.a.n.d.
-000122f0: 6100 7200 6400 7400 7900 7008 0000 0000  a.r.d.t.y.p.....
-00012300: 0600 0000 0d53 7461 6e64 6172 6420 7479  .....Standard ty
-00012310: 7065 0700 0000 0d51 7363 694c 6578 6572  pe.....QsciLexer
-00012320: 5648 444c 0103 0000 0018 005a 0065 0069  VHDL.......Z.e.i
-00012330: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00012340: 0065 0800 0000 0006 0000 0006 5374 7269  .e..........Stri
-00012350: 6e67 0700 0000 0d51 7363 694c 6578 6572  ng.....QsciLexer
-00012360: 5648 444c 0103 0000 002e 0055 006e 0062  VHDL.......U.n.b
-00012370: 0065 0065 006e 0064 0065 0074 0065 0020  .e.e.n.d.e.t.e. 
-00012380: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
-00012390: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
-000123a0: 000f 556e 636c 6f73 6564 2073 7472 696e  ..Unclosed strin
-000123b0: 6707 0000 000d 5173 6369 4c65 7865 7256  g.....QsciLexerV
-000123c0: 4844 4c01 0300 0000 2000 4e00 7500 7400  HDL..... .N.u.t.
-000123d0: 7a00 6500 7200 2000 6400 6500 6600 6900  z.e.r. .d.e.f.i.
-000123e0: 6e00 6900 6500 7200 7408 0000 0000 0600  n.i.e.r.t.......
-000123f0: 0000 0c55 7365 7220 6465 6669 6e65 6407  ...User defined.
-00012400: 0000 000d 5173 6369 4c65 7865 7256 4844  ....QsciLexerVHD
-00012410: 4c01 0300 0000 1c00 4200 6100 6e00 6700  L.......B.a.n.g.
-00012420: 2000 4b00 6f00 6d00 6d00 6500 6e00 7400   .K.o.m.m.e.n.t.
-00012430: 6100 7208 0000 0000 0600 0000 0c42 616e  a.r..........Ban
-00012440: 6720 636f 6d6d 656e 7407 0000 0010 5173  g comment.....Qs
-00012450: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
-00012460: 0000 0012 004b 006f 006d 006d 0065 006e  .....K.o.m.m.e.n
-00012470: 0074 0061 0072 0800 0000 0006 0000 0007  .t.a.r..........
-00012480: 436f 6d6d 656e 7407 0000 0010 5173 6369  Comment.....Qsci
-00012490: 4c65 7865 7256 6572 696c 6f67 0103 0000  LexerVerilog....
-000124a0: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
-000124b0: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
-000124c0: 756c 7407 0000 0010 5173 6369 4c65 7865  ult.....QsciLexe
-000124d0: 7256 6572 696c 6f67 0103 0000 0014 0042  rVerilog.......B
-000124e0: 0065 007a 0065 0069 0063 0068 006e 0065  .e.z.e.i.c.h.n.e
-000124f0: 0072 0800 0000 0006 0000 000a 4964 656e  .r..........Iden
-00012500: 7469 6669 6572 0700 0000 1051 7363 694c  tifier.....QsciL
-00012510: 6578 6572 5665 7269 6c6f 6701 0300 0000  exerVerilog.....
-00012520: 3000 4900 6e00 6100 6b00 7400 6900 7600  0.I.n.a.k.t.i.v.
-00012530: 6500 7200 2000 4200 6100 6e00 6700 2000  e.r. .B.a.n.g. .
-00012540: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
-00012550: 7208 0000 0000 0600 0000 1549 6e61 6374  r..........Inact
-00012560: 6976 6520 6261 6e67 2063 6f6d 6d65 6e74  ive bang comment
-00012570: 0700 0000 1051 7363 694c 6578 6572 5665  .....QsciLexerVe
-00012580: 7269 6c6f 6701 0300 0000 2600 4900 6e00  rilog.....&.I.n.
-00012590: 6100 6b00 7400 6900 7600 6500 7200 2000  a.k.t.i.v.e.r. .
-000125a0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
-000125b0: 7208 0000 0000 0600 0000 1049 6e61 6374  r..........Inact
-000125c0: 6976 6520 636f 6d6d 656e 7407 0000 0010  ive comment.....
-000125d0: 5173 6369 4c65 7865 7256 6572 696c 6f67  QsciLexerVerilog
-000125e0: 0103 0000 0024 0049 006e 0061 006b 0074  .....$.I.n.a.k.t
-000125f0: 0069 0076 0065 0072 0020 0053 0074 0061  .i.v.e.r. .S.t.a
-00012600: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
-00012610: 0000 0010 496e 6163 7469 7665 2064 6566  ....Inactive def
-00012620: 6175 6c74 0700 0000 1051 7363 694c 6578  ault.....QsciLex
-00012630: 6572 5665 7269 6c6f 6701 0300 0000 2800  erVerilog.....(.
-00012640: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
-00012650: 7200 2000 4200 6500 7a00 6500 6900 6300  r. .B.e.z.e.i.c.
-00012660: 6800 6e00 6500 7208 0000 0000 0600 0000  h.n.e.r.........
-00012670: 1349 6e61 6374 6976 6520 6964 656e 7469  .Inactive identi
-00012680: 6669 6572 0700 0000 1051 7363 694c 6578  fier.....QsciLex
-00012690: 6572 5665 7269 6c6f 6701 0300 0000 3c00  erVerilog.....<.
-000126a0: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
-000126b0: 2000 4500 6900 6e00 6700 6100 6200 6500   .E.i.n.g.a.b.e.
-000126c0: 7000 6f00 7200 7400 6400 6500 6600 6900  p.o.r.t.d.e.f.i.
-000126d0: 6e00 6900 7400 6900 6f00 6e08 0000 0000  n.i.t.i.o.n.....
-000126e0: 0600 0000 1f49 6e61 6374 6976 6520 696e  .....Inactive in
-000126f0: 7075 7420 706f 7274 2064 6563 6c61 7261  put port declara
-00012700: 7469 6f6e 0700 0000 1051 7363 694c 6578  tion.....QsciLex
-00012710: 6572 5665 7269 6c6f 6701 0300 0000 4600  erVerilog.....F.
-00012720: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
-00012730: 2000 4500 6900 6e00 2d00 2f00 4100 7500   .E.i.n.-./.A.u.
-00012740: 7300 6700 6100 6200 6500 7000 6f00 7200  s.g.a.b.e.p.o.r.
-00012750: 7400 6400 6500 6600 6900 6e00 6900 7400  t.d.e.f.i.n.i.t.
-00012760: 6900 6f00 6e08 0000 0000 0600 0000 2649  i.o.n.........&I
-00012770: 6e61 6374 6976 6520 696e 7075 742f 6f75  nactive input/ou
-00012780: 7470 7574 2070 6f72 7420 6465 636c 6172  tput port declar
-00012790: 6174 696f 6e07 0000 0010 5173 6369 4c65  ation.....QsciLe
-000127a0: 7865 7256 6572 696c 6f67 0103 0000 0040  xerVerilog.....@
-000127b0: 0049 006e 0061 006b 0074 0069 0076 0065  .I.n.a.k.t.i.v.e
-000127c0: 0072 0020 0053 0063 0068 006c 00fc 0073  .r. .S.c.h.l...s
-000127d0: 0073 0065 006c 0077 006f 0072 0074 006b  .s.e.l.w.o.r.t.k
-000127e0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-000127f0: 0800 0000 0006 0000 0018 496e 6163 7469  ..........Inacti
-00012800: 7665 206b 6579 776f 7264 2063 6f6d 6d65  ve keyword comme
-00012810: 6e74 0700 0000 1051 7363 694c 6578 6572  nt.....QsciLexer
-00012820: 5665 7269 6c6f 6701 0300 0000 3200 4900  Verilog.....2.I.
-00012830: 6e00 6100 6b00 7400 6900 7600 6500 7200  n.a.k.t.i.v.e.r.
-00012840: 2000 5a00 6500 6900 6c00 6500 6e00 6b00   .Z.e.i.l.e.n.k.
-00012850: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
-00012860: 0000 0000 0600 0000 1549 6e61 6374 6976  .........Inactiv
-00012870: 6520 6c69 6e65 2063 6f6d 6d65 6e74 0700  e line comment..
-00012880: 0000 1051 7363 694c 6578 6572 5665 7269  ...QsciLexerVeri
-00012890: 6c6f 6701 0300 0000 1a00 4900 6e00 6100  log.......I.n.a.
-000128a0: 6b00 7400 6900 7600 6500 2000 5a00 6100  k.t.i.v.e. .Z.a.
-000128b0: 6800 6c08 0000 0000 0600 0000 0f49 6e61  h.l..........Ina
-000128c0: 6374 6976 6520 6e75 6d62 6572 0700 0000  ctive number....
-000128d0: 1051 7363 694c 6578 6572 5665 7269 6c6f  .QsciLexerVerilo
-000128e0: 6701 0300 0000 2400 4900 6e00 6100 6b00  g.....$.I.n.a.k.
-000128f0: 7400 6900 7600 6500 7200 2000 4f00 7000  t.i.v.e.r. .O.p.
-00012900: 6500 7200 6100 7400 6f00 7208 0000 0000  e.r.a.t.o.r.....
-00012910: 0600 0000 1149 6e61 6374 6976 6520 6f70  .....Inactive op
-00012920: 6572 6174 6f72 0700 0000 1051 7363 694c  erator.....QsciL
-00012930: 6578 6572 5665 7269 6c6f 6701 0300 0000  exerVerilog.....
-00012940: 3c00 4900 6e00 6100 6b00 7400 6900 7600  <.I.n.a.k.t.i.v.
-00012950: 6500 2000 4100 7500 7300 6700 6100 6200  e. .A.u.s.g.a.b.
-00012960: 6500 7000 6f00 7200 7400 6400 6500 6600  e.p.o.r.t.d.e.f.
-00012970: 6900 6e00 6900 7400 6900 6f00 6e08 0000  i.n.i.t.i.o.n...
-00012980: 0000 0600 0000 2049 6e61 6374 6976 6520  ...... Inactive 
-00012990: 6f75 7470 7574 2070 6f72 7420 6465 636c  output port decl
-000129a0: 6172 6174 696f 6e07 0000 0010 5173 6369  aration.....Qsci
-000129b0: 4c65 7865 7256 6572 696c 6f67 0103 0000  LexerVerilog....
-000129c0: 002e 0049 006e 0061 006b 0074 0069 0076  ...I.n.a.k.t.i.v
-000129d0: 0065 0020 0050 006f 0072 0074 0076 0065  .e. .P.o.r.t.v.e
-000129e0: 0072 0062 0069 006e 0064 0075 006e 0067  .r.b.i.n.d.u.n.g
-000129f0: 0800 0000 0006 0000 0018 496e 6163 7469  ..........Inacti
-00012a00: 7665 2070 6f72 7420 636f 6e6e 6563 7469  ve port connecti
-00012a10: 6f6e 0700 0000 1051 7363 694c 6578 6572  on.....QsciLexer
-00012a20: 5665 7269 6c6f 6701 0300 0000 3600 4900  Verilog.....6.I.
-00012a30: 6e00 6100 6b00 7400 6900 7600 6500 7200  n.a.k.t.i.v.e.r.
-00012a40: 2000 5000 7200 e400 7000 7200 6f00 7a00   .P.r...p.r.o.z.
-00012a50: 6500 7300 7300 6f00 7200 6200 6c00 6f00  e.s.s.o.r.b.l.o.
-00012a60: 6300 6b08 0000 0000 0600 0000 1b49 6e61  c.k..........Ina
-00012a70: 6374 6976 6520 7072 6570 726f 6365 7373  ctive preprocess
-00012a80: 6f72 2062 6c6f 636b 0700 0000 1051 7363  or block.....Qsc
-00012a90: 694c 6578 6572 5665 7269 6c6f 6701 0300  iLexerVerilog...
-00012aa0: 0000 5e00 4900 6e00 6100 6b00 7400 6900  ..^.I.n.a.k.t.i.
-00012ab0: 7600 6500 2000 7000 7200 6900 6d00 e400  v.e. .p.r.i.m...
-00012ac0: 7200 6500 2000 5300 6300 6800 6c00 7500  r.e. .S.c.h.l.u.
-00012ad0: 7300 7300 6500 6c00 7700 f600 7200 7400  s.s.e.l.w...r.t.
-00012ae0: 6500 7200 2000 7500 6e00 6400 2000 4200  e.r. .u.n.d. .B.
-00012af0: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
-00012b00: 7208 0000 0000 0600 0000 2949 6e61 6374  r.........)Inact
-00012b10: 6976 6520 7072 696d 6172 7920 6b65 7977  ive primary keyw
-00012b20: 6f72 6473 2061 6e64 2069 6465 6e74 6966  ords and identif
-00012b30: 6965 7273 0700 0000 1051 7363 694c 6578  iers.....QsciLex
-00012b40: 6572 5665 7269 6c6f 6701 0300 0000 6200  erVerilog.....b.
-00012b50: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
-00012b60: 2000 7300 6500 6b00 7500 6e00 6400 e400   .s.e.k.u.n.d...
-00012b70: 7200 6500 2000 5300 6300 6800 6c00 7500  r.e. .S.c.h.l.u.
-00012b80: 7300 7300 6500 6c00 7700 f600 7200 7400  s.s.e.l.w...r.t.
-00012b90: 6500 7200 2000 7500 6e00 6400 2000 4200  e.r. .u.n.d. .B.
-00012ba0: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
-00012bb0: 7208 0000 0000 0600 0000 2b49 6e61 6374  r.........+Inact
-00012bc0: 6976 6520 7365 636f 6e64 6172 7920 6b65  ive secondary ke
-00012bd0: 7977 6f72 6473 2061 6e64 2069 6465 6e74  ywords and ident
-00012be0: 6966 6965 7273 0700 0000 1051 7363 694c  ifiers.....QsciL
-00012bf0: 6578 6572 5665 7269 6c6f 6701 0300 0000  exerVerilog.....
-00012c00: 2a00 4900 6e00 6100 6b00 7400 6900 7600  *.I.n.a.k.t.i.v.
-00012c10: 6500 2000 5a00 6500 6900 6300 6800 6500  e. .Z.e.i.c.h.e.
-00012c20: 6e00 6b00 6500 7400 7400 6508 0000 0000  n.k.e.t.t.e.....
-00012c30: 0600 0000 0f49 6e61 6374 6976 6520 7374  .....Inactive st
-00012c40: 7269 6e67 0700 0000 1051 7363 694c 6578  ring.....QsciLex
-00012c50: 6572 5665 7269 6c6f 6701 0300 0000 2800  erVerilog.....(.
-00012c60: 4900 6e00 6100 6b00 7400 6900 7600 6500  I.n.a.k.t.i.v.e.
-00012c70: 7200 2000 5300 7900 7300 7400 6500 6d00  r. .S.y.s.t.e.m.
-00012c80: 7400 6100 7300 6b08 0000 0000 0600 0000  t.a.s.k.........
-00012c90: 1449 6e61 6374 6976 6520 7379 7374 656d  .Inactive system
-00012ca0: 2074 6173 6b07 0000 0010 5173 6369 4c65   task.....QsciLe
-00012cb0: 7865 7256 6572 696c 6f67 0103 0000 0040  xerVerilog.....@
-00012cc0: 0049 006e 0061 006b 0074 0069 0076 0065  .I.n.a.k.t.i.v.e
-00012cd0: 0020 0075 006e 0062 0065 0065 006e 0064  . .u.n.b.e.e.n.d
-00012ce0: 0065 0074 0065 0020 005a 0065 0069 0063  .e.t.e. .Z.e.i.c
-00012cf0: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
-00012d00: 0800 0000 0006 0000 0018 496e 6163 7469  ..........Inacti
-00012d10: 7665 2075 6e63 6c6f 7365 6420 7374 7269  ve unclosed stri
-00012d20: 6e67 0700 0000 1051 7363 694c 6578 6572  ng.....QsciLexer
-00012d30: 5665 7269 6c6f 6701 0300 0000 5c00 4900  Verilog.....\.I.
-00012d40: 6e00 6100 6b00 7400 6900 7600 6500 2000  n.a.k.t.i.v.e. .
-00012d50: 6e00 7500 7400 7a00 6500 7200 6400 6500  n.u.t.z.e.r.d.e.
-00012d60: 6600 6900 6e00 6900 6500 7200 7400 6500  f.i.n.i.e.r.t.e.
-00012d70: 2000 5400 6100 7300 6b00 7300 2000 7500   .T.a.s.k.s. .u.
-00012d80: 6e00 6400 2000 4200 6500 7a00 6500 6900  n.d. .B.e.z.e.i.
-00012d90: 6300 6800 6e00 6500 7208 0000 0000 0600  c.h.n.e.r.......
-00012da0: 0000 2b49 6e61 6374 6976 6520 7573 6572  ..+Inactive user
-00012db0: 2064 6566 696e 6564 2074 6173 6b73 2061   defined tasks a
-00012dc0: 6e64 2069 6465 6e74 6966 6965 7273 0700  nd identifiers..
-00012dd0: 0000 1051 7363 694c 6578 6572 5665 7269  ...QsciLexerVeri
-00012de0: 6c6f 6701 0300 0000 2a00 4500 6900 6e00  log.....*.E.i.n.
-00012df0: 6700 6100 6200 6500 7000 6f00 7200 7400  g.a.b.e.p.o.r.t.
-00012e00: 6400 6500 6600 6900 6e00 6900 7400 6900  d.e.f.i.n.i.t.i.
-00012e10: 6f00 6e08 0000 0000 0600 0000 1649 6e70  o.n..........Inp
-00012e20: 7574 2070 6f72 7420 6465 636c 6172 6174  ut port declarat
-00012e30: 696f 6e07 0000 0010 5173 6369 4c65 7865  ion.....QsciLexe
-00012e40: 7256 6572 696c 6f67 0103 0000 0034 0045  rVerilog.....4.E
-00012e50: 0069 006e 002d 002f 0041 0075 0073 0067  .i.n.-./.A.u.s.g
-00012e60: 0061 0062 0065 0070 006f 0072 0074 0064  .a.b.e.p.o.r.t.d
-00012e70: 0065 0066 0069 006e 0069 0074 0069 006f  .e.f.i.n.i.t.i.o
-00012e80: 006e 0800 0000 0006 0000 001d 496e 7075  .n..........Inpu
-00012e90: 742f 6f75 7470 7574 2070 6f72 7420 6465  t/output port de
-00012ea0: 636c 6172 6174 696f 6e07 0000 0010 5173  claration.....Qs
-00012eb0: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
-00012ec0: 0000 002c 0053 0063 0068 006c 00fc 0073  ...,.S.c.h.l...s
-00012ed0: 0073 0065 006c 0077 006f 0072 0074 006b  .s.e.l.w.o.r.t.k
-00012ee0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-00012ef0: 0800 0000 0006 0000 000f 4b65 7977 6f72  ..........Keywor
-00012f00: 6420 636f 6d6d 656e 7407 0000 0010 5173  d comment.....Qs
-00012f10: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
-00012f20: 0000 001e 005a 0065 0069 006c 0065 006e  .....Z.e.i.l.e.n
-00012f30: 006b 006f 006d 006d 0065 006e 0074 0061  .k.o.m.m.e.n.t.a
-00012f40: 0072 0800 0000 0006 0000 000c 4c69 6e65  .r..........Line
-00012f50: 2063 6f6d 6d65 6e74 0700 0000 1051 7363   comment.....Qsc
-00012f60: 694c 6578 6572 5665 7269 6c6f 6701 0300  iLexerVerilog...
-00012f70: 0000 0800 5a00 6100 6800 6c08 0000 0000  ....Z.a.h.l.....
-00012f80: 0600 0000 064e 756d 6265 7207 0000 0010  .....Number.....
-00012f90: 5173 6369 4c65 7865 7256 6572 696c 6f67  QsciLexerVerilog
-00012fa0: 0103 0000 0010 004f 0070 0065 0072 0061  .......O.p.e.r.a
-00012fb0: 0074 006f 0072 0800 0000 0006 0000 0008  .t.o.r..........
-00012fc0: 4f70 6572 6174 6f72 0700 0000 1051 7363  Operator.....Qsc
-00012fd0: 694c 6578 6572 5665 7269 6c6f 6701 0300  iLexerVerilog...
-00012fe0: 0000 2a00 4100 7500 7300 6700 6100 6200  ..*.A.u.s.g.a.b.
-00012ff0: 6500 7000 6f00 7200 7400 6400 6500 6600  e.p.o.r.t.d.e.f.
-00013000: 6900 6e00 6900 7400 6900 6f00 6e08 0000  i.n.i.t.i.o.n...
-00013010: 0000 0600 0000 174f 7574 7075 7420 706f  .......Output po
-00013020: 7274 2064 6563 6c61 7261 7469 6f6e 0700  rt declaration..
-00013030: 0000 1051 7363 694c 6578 6572 5665 7269  ...QsciLexerVeri
-00013040: 6c6f 6701 0300 0000 1c00 5000 6f00 7200  log.......P.o.r.
-00013050: 7400 7600 6500 7200 6200 6900 6e00 6400  t.v.e.r.b.i.n.d.
-00013060: 7500 6e00 6708 0000 0000 0600 0000 0f50  u.n.g..........P
-00013070: 6f72 7420 636f 6e6e 6563 7469 6f6e 0700  ort connection..
-00013080: 0000 1051 7363 694c 6578 6572 5665 7269  ...QsciLexerVeri
-00013090: 6c6f 6701 0300 0000 2200 5000 7200 e400  log.....".P.r...
-000130a0: 7000 7200 6f00 7a00 6500 7300 7300 6f00  p.r.o.z.e.s.s.o.
-000130b0: 7200 6200 6c00 6f00 6300 6b08 0000 0000  r.b.l.o.c.k.....
-000130c0: 0600 0000 1250 7265 7072 6f63 6573 736f  .....Preprocesso
-000130d0: 7220 626c 6f63 6b07 0000 0010 5173 6369  r block.....Qsci
-000130e0: 4c65 7865 7256 6572 696c 6f67 0103 0000  LexerVerilog....
-000130f0: 004c 0050 0072 0069 006d 00e4 0072 0065  .L.P.r.i.m...r.e
-00013100: 0020 0053 0063 0068 006c 0075 0073 0073  . .S.c.h.l.u.s.s
-00013110: 0065 006c 0077 00f6 0072 0074 0065 0072  .e.l.w...r.t.e.r
-00013120: 0020 0075 006e 0064 0020 0042 0065 007a  . .u.n.d. .B.e.z
-00013130: 0065 0069 0063 0068 006e 0065 0072 0800  .e.i.c.h.n.e.r..
-00013140: 0000 0006 0000 0020 5072 696d 6172 7920  ....... Primary 
-00013150: 6b65 7977 6f72 6473 2061 6e64 2069 6465  keywords and ide
-00013160: 6e74 6966 6965 7273 0700 0000 1051 7363  ntifiers.....Qsc
-00013170: 694c 6578 6572 5665 7269 6c6f 6701 0300  iLexerVerilog...
-00013180: 0000 5000 5300 6500 6b00 7500 6e00 6400  ..P.S.e.k.u.n.d.
-00013190: e400 7200 6500 2000 5300 6300 6800 6c00  ..r.e. .S.c.h.l.
-000131a0: 7500 7300 7300 6500 6c00 7700 f600 7200  u.s.s.e.l.w...r.
-000131b0: 7400 6500 7200 2000 7500 6e00 6400 2000  t.e.r. .u.n.d. .
-000131c0: 4200 6500 7a00 6500 6900 6300 6800 6e00  B.e.z.e.i.c.h.n.
-000131d0: 6500 7208 0000 0000 0600 0000 2253 6563  e.r........."Sec
-000131e0: 6f6e 6461 7279 206b 6579 776f 7264 7320  ondary keywords 
-000131f0: 616e 6420 6964 656e 7469 6669 6572 7307  and identifiers.
-00013200: 0000 0010 5173 6369 4c65 7865 7256 6572  ....QsciLexerVer
-00013210: 696c 6f67 0103 0000 0018 005a 0065 0069  ilog.......Z.e.i
-00013220: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
-00013230: 0065 0800 0000 0006 0000 0006 5374 7269  .e..........Stri
-00013240: 6e67 0700 0000 1051 7363 694c 6578 6572  ng.....QsciLexer
-00013250: 5665 7269 6c6f 6701 0300 0000 1400 5300  Verilog.......S.
-00013260: 7900 7300 7400 6500 6d00 7400 6100 7300  y.s.t.e.m.t.a.s.
-00013270: 6b08 0000 0000 0600 0000 0b53 7973 7465  k..........Syste
-00013280: 6d20 7461 736b 0700 0000 1051 7363 694c  m task.....QsciL
-00013290: 6578 6572 5665 7269 6c6f 6701 0300 0000  exerVerilog.....
-000132a0: 2e00 5500 6e00 6200 6500 6500 6e00 6400  ..U.n.b.e.e.n.d.
-000132b0: 6500 7400 6500 2000 5a00 6500 6900 6300  e.t.e. .Z.e.i.c.
-000132c0: 6800 6500 6e00 6b00 6500 7400 7400 6508  h.e.n.k.e.t.t.e.
-000132d0: 0000 0000 0600 0000 0f55 6e63 6c6f 7365  .........Unclose
-000132e0: 6420 7374 7269 6e67 0700 0000 1051 7363  d string.....Qsc
-000132f0: 694c 6578 6572 5665 7269 6c6f 6701 0300  iLexerVerilog...
-00013300: 0000 4a00 4e00 7500 7400 7a00 6500 7200  ..J.N.u.t.z.e.r.
-00013310: 6400 6500 6600 6900 6e00 6900 6500 7200  d.e.f.i.n.i.e.r.
-00013320: 7400 6500 2000 5400 6100 7300 6b00 7300  t.e. .T.a.s.k.s.
-00013330: 2000 7500 6e00 6400 2000 4200 6500 7a00   .u.n.d. .B.e.z.
-00013340: 6500 6900 6300 6800 6e00 6500 7208 0000  e.i.c.h.n.e.r...
-00013350: 0000 0600 0000 2255 7365 7220 6465 6669  ......"User defi
-00013360: 6e65 6420 7461 736b 7320 616e 6420 6964  ned tasks and id
-00013370: 656e 7469 6669 6572 7307 0000 0010 5173  entifiers.....Qs
-00013380: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
-00013390: 0000 0012 004b 006f 006d 006d 0065 006e  .....K.o.m.m.e.n
-000133a0: 0074 0061 0072 0800 0000 0006 0000 0007  .t.a.r..........
-000133b0: 436f 6d6d 656e 7407 0000 000d 5173 6369  Comment.....Qsci
-000133c0: 4c65 7865 7259 414d 4c01 0300 0000 1000  LexerYAML.......
-000133d0: 5300 7400 6100 6e00 6400 6100 7200 6408  S.t.a.n.d.a.r.d.
-000133e0: 0000 0000 0600 0000 0744 6566 6175 6c74  .........Default
-000133f0: 0700 0000 0d51 7363 694c 6578 6572 5941  .....QsciLexerYA
-00013400: 4d4c 0103 0000 0022 0044 006f 006b 0075  ML.....".D.o.k.u
-00013410: 006d 0065 006e 0074 0062 0065 0067 0072  .m.e.n.t.b.e.g.r
-00013420: 0065 006e 007a 0065 0072 0800 0000 0006  .e.n.z.e.r......
-00013430: 0000 0012 446f 6375 6d65 6e74 2064 656c  ....Document del
-00013440: 696d 6974 6572 0700 0000 0d51 7363 694c  imiter.....QsciL
-00013450: 6578 6572 5941 4d4c 0103 0000 0014 0042  exerYAML.......B
-00013460: 0065 007a 0065 0069 0063 0068 006e 0065  .e.z.e.i.c.h.n.e
-00013470: 0072 0800 0000 0006 0000 000a 4964 656e  .r..........Iden
-00013480: 7469 6669 6572 0700 0000 0d51 7363 694c  tifier.....QsciL
-00013490: 6578 6572 5941 4d4c 0103 0000 001a 0053  exerYAML.......S
-000134a0: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
-000134b0: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
-000134c0: 0007 4b65 7977 6f72 6407 0000 000d 5173  ..Keyword.....Qs
-000134d0: 6369 4c65 7865 7259 414d 4c01 0300 0000  ciLexerYAML.....
-000134e0: 0800 5a00 6100 6800 6c08 0000 0000 0600  ..Z.a.h.l.......
-000134f0: 0000 064e 756d 6265 7207 0000 000d 5173  ...Number.....Qs
-00013500: 6369 4c65 7865 7259 414d 4c01 0300 0000  ciLexerYAML.....
-00013510: 1000 4f00 7000 6500 7200 6100 7400 6f00  ..O.p.e.r.a.t.o.
-00013520: 7208 0000 0000 0600 0000 084f 7065 7261  r..........Opera
-00013530: 746f 7207 0000 000d 5173 6369 4c65 7865  tor.....QsciLexe
-00013540: 7259 414d 4c01 0300 0000 1000 5200 6500  rYAML.......R.e.
-00013550: 6600 6500 7200 6500 6e00 7a08 0000 0000  f.e.r.e.n.z.....
-00013560: 0600 0000 0952 6566 6572 656e 6365 0700  .....Reference..
-00013570: 0000 0d51 7363 694c 6578 6572 5941 4d4c  ...QsciLexerYAML
-00013580: 0103 0000 002e 0053 0079 006e 0074 0061  .......S.y.n.t.a
-00013590: 0078 0066 0065 0068 006c 0065 0072 0020  .x.f.e.h.l.e.r. 
-000135a0: 004d 0061 0072 006b 0069 0065 0072 0075  .M.a.r.k.i.e.r.u
-000135b0: 006e 0067 0800 0000 0006 0000 0013 5379  .n.g..........Sy
-000135c0: 6e74 6178 2065 7272 6f72 206d 6172 6b65  ntax error marke
-000135d0: 7207 0000 000d 5173 6369 4c65 7865 7259  r.....QsciLexerY
-000135e0: 414d 4c01 0300 0000 2800 5400 6500 7800  AML.....(.T.e.x.
-000135f0: 7400 6200 6c00 6f00 6300 6b00 2000 4d00  t.b.l.o.c.k. .M.
-00013600: 6100 7200 6b00 6900 6500 7200 7500 6e00  a.r.k.i.e.r.u.n.
-00013610: 6708 0000 0000 0600 0000 1154 6578 7420  g..........Text 
-00013620: 626c 6f63 6b20 6d61 726b 6572 0700 0000  block marker....
-00013630: 0d51 7363 694c 6578 6572 5941 4d4c 0103  .QsciLexerYAML..
-00013640: 0000 0012 0026 004b 006f 0070 0069 0065  .....&.K.o.p.i.e
-00013650: 0072 0065 006e 0800 0000 0006 0000 0005  .r.e.n..........
-00013660: 2643 6f70 7907 0000 000d 5173 6369 5363  &Copy.....QsciSc
-00013670: 696e 7469 6c6c 6101 0300 0000 1200 4500  intilla.......E.
-00013680: 6900 6e00 2600 6600 fc00 6700 6500 6e08  i.n.&.f...g.e.n.
-00013690: 0000 0000 0600 0000 0626 5061 7374 6507  .........&Paste.
-000136a0: 0000 000d 5173 6369 5363 696e 7469 6c6c  ....QsciScintill
-000136b0: 6101 0300 0000 2200 5700 6900 6500 6400  a.....".W.i.e.d.
-000136c0: 6500 7200 2600 6800 6500 7200 7300 7400  e.r.&.h.e.r.s.t.
-000136d0: 6500 6c00 6c00 6500 6e08 0000 0000 0600  e.l.l.e.n.......
-000136e0: 0000 0526 5265 646f 0700 0000 0d51 7363  ...&Redo.....Qsc
-000136f0: 6953 6369 6e74 696c 6c61 0103 0000 0016  iScintilla......
-00013700: 0026 0052 00fc 0063 006b 0067 00e4 006e  .&.R...c.k.g...n
-00013710: 0067 0069 0067 0800 0000 0006 0000 0005  .g.i.g..........
-00013720: 2655 6e64 6f07 0000 000d 5173 6369 5363  &Undo.....QsciSc
-00013730: 696e 7469 6c6c 6101 0300 0000 1a00 2600  intilla.......&.
-00013740: 4100 7500 7300 7300 6300 6800 6e00 6500  A.u.s.s.c.h.n.e.
-00013750: 6900 6400 6500 6e08 0000 0000 0600 0000  i.d.e.n.........
-00013760: 0443 7526 7407 0000 000d 5173 6369 5363  .Cu&t.....QsciSc
-00013770: 696e 7469 6c6c 6101 0300 0000 0e00 4c00  intilla.......L.
-00013780: f600 7300 6300 6800 6500 6e08 0000 0000  ..s.c.h.e.n.....
-00013790: 0600 0000 0644 656c 6574 6507 0000 000d  .....Delete.....
-000137a0: 5173 6369 5363 696e 7469 6c6c 6101 0300  QsciScintilla...
-000137b0: 0000 1c00 4100 6c00 6c00 6500 2000 6100  ....A.l.l.e. .a.
-000137c0: 7500 7300 7700 e400 6800 6c00 6500 6e08  u.s.w...h.l.e.n.
-000137d0: 0000 0000 0600 0000 0a53 656c 6563 7420  .........Select 
-000137e0: 416c 6c07 0000 000d 5173 6369 5363 696e  All.....QsciScin
-000137f0: 7469 6c6c 6101 8800 0000 0201 01         tilla........
+0000bee0: 4d4c 0103 0000 002c 0053 0047 004d 004c  ML.....,.S.G.M.L
+0000bef0: 0020 0053 0070 0065 007a 0069 0065 006c  . .S.p.e.z.i.e.l
+0000bf00: 006c 0065 0020 0045 006e 0074 0069 0074  .l.e. .E.n.t.i.t
+0000bf10: 00e4 0074 0800 0000 0006 0000 0013 5347  ...t..........SG
+0000bf20: 4d4c 2073 7065 6369 616c 2065 6e74 6974  ML special entit
+0000bf30: 7907 0000 000d 5173 6369 4c65 7865 7248  y.....QsciLexerH
+0000bf40: 544d 4c01 0300 0000 1400 5300 6b00 7200  TML.......S.k.r.
+0000bf50: 6900 7000 7400 2000 5400 6100 6708 0000  i.p.t. .T.a.g...
+0000bf60: 0000 0600 0000 0a53 6372 6970 7420 7461  .......Script ta
+0000bf70: 6707 0000 000d 5173 6369 4c65 7865 7248  g.....QsciLexerH
+0000bf80: 544d 4c01 0300 0000 4400 4200 6500 6700  TML.....D.B.e.g.
+0000bf90: 6900 6e00 6e00 2000 6500 6900 6e00 6500  i.n.n. .e.i.n.e.
+0000bfa0: 7300 2000 4a00 6100 7600 6100 5300 6300  s. .J.a.v.a.S.c.
+0000bfb0: 7200 6900 7000 7400 2000 4600 7200 6100  r.i.p.t. .F.r.a.
+0000bfc0: 6700 6d00 6500 6e00 7400 6500 7308 0000  g.m.e.n.t.e.s...
+0000bfd0: 0000 0600 0000 1e53 7461 7274 206f 6620  .......Start of 
+0000bfe0: 6120 4a61 7661 5363 7269 7074 2066 7261  a JavaScript fra
+0000bff0: 676d 656e 7407 0000 000d 5173 6369 4c65  gment.....QsciLe
+0000c000: 7865 7248 544d 4c01 0300 0000 3600 4200  xerHTML.....6.B.
+0000c010: 6500 6700 6900 6e00 6e00 2000 6500 6900  e.g.i.n.n. .e.i.
+0000c020: 6e00 6500 7300 2000 5000 4800 5000 2000  n.e.s. .P.H.P. .
+0000c030: 4600 7200 6100 6700 6d00 6500 6e00 7400  F.r.a.g.m.e.n.t.
+0000c040: 6500 7308 0000 0000 0600 0000 1753 7461  e.s..........Sta
+0000c050: 7274 206f 6620 6120 5048 5020 6672 6167  rt of a PHP frag
+0000c060: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
+0000c070: 6572 4854 4d4c 0103 0000 003c 0042 0065  erHTML.....<.B.e
+0000c080: 0067 0069 006e 006e 0020 0065 0069 006e  .g.i.n.n. .e.i.n
+0000c090: 0065 0073 0020 0050 0079 0074 0068 006f  .e.s. .P.y.t.h.o
+0000c0a0: 006e 0020 0046 0072 0061 0067 006d 0065  .n. .F.r.a.g.m.e
+0000c0b0: 006e 0074 0065 0073 0800 0000 0006 0000  .n.t.e.s........
+0000c0c0: 001a 5374 6172 7420 6f66 2061 2050 7974  ..Start of a Pyt
+0000c0d0: 686f 6e20 6672 6167 6d65 6e74 0700 0000  hon fragment....
+0000c0e0: 0d51 7363 694c 6578 6572 4854 4d4c 0103  .QsciLexerHTML..
+0000c0f0: 0000 0040 0042 0065 0067 0069 006e 006e  ...@.B.e.g.i.n.n
+0000c100: 0020 0065 0069 006e 0065 0073 0020 0056  . .e.i.n.e.s. .V
+0000c110: 0042 0053 0063 0072 0069 0070 0074 0020  .B.S.c.r.i.p.t. 
+0000c120: 0046 0072 0061 0067 006d 0065 006e 0074  .F.r.a.g.m.e.n.t
+0000c130: 0065 0073 0800 0000 0006 0000 001c 5374  .e.s..........St
+0000c140: 6172 7420 6f66 2061 2056 4253 6372 6970  art of a VBScrip
+0000c150: 7420 6672 6167 6d65 6e74 0700 0000 0d51  t fragment.....Q
+0000c160: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+0000c170: 004c 0042 0065 0067 0069 006e 006e 0020  .L.B.e.g.i.n.n. 
+0000c180: 0065 0069 006e 0065 0073 0020 0041 0053  .e.i.n.e.s. .A.S
+0000c190: 0050 0020 004a 0061 0076 0061 0053 0063  .P. .J.a.v.a.S.c
+0000c1a0: 0072 0069 0070 0074 0020 0046 0072 0061  .r.i.p.t. .F.r.a
+0000c1b0: 0067 006d 0065 006e 0074 0065 0073 0800  .g.m.e.n.t.e.s..
+0000c1c0: 0000 0006 0000 0023 5374 6172 7420 6f66  .......#Start of
+0000c1d0: 2061 6e20 4153 5020 4a61 7661 5363 7269   an ASP JavaScri
+0000c1e0: 7074 2066 7261 676d 656e 7407 0000 000d  pt fragment.....
+0000c1f0: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000c200: 0000 4400 4200 6500 6700 6900 6e00 6e00  ..D.B.e.g.i.n.n.
+0000c210: 2000 6500 6900 6e00 6500 7300 2000 4100   .e.i.n.e.s. .A.
+0000c220: 5300 5000 2000 5000 7900 7400 6800 6f00  S.P. .P.y.t.h.o.
+0000c230: 6e00 2000 4600 7200 6100 6700 6d00 6500  n. .F.r.a.g.m.e.
+0000c240: 6e00 7400 6500 7308 0000 0000 0600 0000  n.t.e.s.........
+0000c250: 1f53 7461 7274 206f 6620 616e 2041 5350  .Start of an ASP
+0000c260: 2050 7974 686f 6e20 6672 6167 6d65 6e74   Python fragment
+0000c270: 0700 0000 0d51 7363 694c 6578 6572 4854  .....QsciLexerHT
+0000c280: 4d4c 0103 0000 0048 0042 0065 0067 0069  ML.....H.B.e.g.i
+0000c290: 006e 006e 0020 0065 0069 006e 0065 0073  .n.n. .e.i.n.e.s
+0000c2a0: 0020 0041 0053 0050 0020 0056 0042 0053  . .A.S.P. .V.B.S
+0000c2b0: 0063 0072 0069 0070 0074 0020 0046 0072  .c.r.i.p.t. .F.r
+0000c2c0: 0061 0067 006d 0065 006e 0074 0065 0073  .a.g.m.e.n.t.e.s
+0000c2d0: 0800 0000 0006 0000 0021 5374 6172 7420  .........!Start 
+0000c2e0: 6f66 2061 6e20 4153 5020 5642 5363 7269  of an ASP VBScri
+0000c2f0: 7074 2066 7261 676d 656e 7407 0000 000d  pt fragment.....
+0000c300: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000c310: 0000 3600 4200 6500 6700 6900 6e00 6e00  ..6.B.e.g.i.n.n.
+0000c320: 2000 6500 6900 6e00 6500 7300 2000 4100   .e.i.n.e.s. .A.
+0000c330: 5300 5000 2000 4600 7200 6100 6700 6d00  S.P. .F.r.a.g.m.
+0000c340: 6500 6e00 7400 6500 7308 0000 0000 0600  e.n.t.e.s.......
+0000c350: 0000 1853 7461 7274 206f 6620 616e 2041  ...Start of an A
+0000c360: 5350 2066 7261 676d 656e 7407 0000 000d  SP fragment.....
+0000c370: 5173 6369 4c65 7865 7248 544d 4c01 0300  QsciLexerHTML...
+0000c380: 0000 4200 4200 6500 6700 6900 6e00 6e00  ..B.B.e.g.i.n.n.
+0000c390: 2000 6500 6900 6e00 6500 7300 2000 4100   .e.i.n.e.s. .A.
+0000c3a0: 5300 5000 2000 4600 7200 6100 6700 6d00  S.P. .F.r.a.g.m.
+0000c3b0: 6500 6e00 7400 6500 7300 2000 6d00 6900  e.n.t.e.s. .m.i.
+0000c3c0: 7400 2000 4008 0000 0000 0600 0000 1f53  t. .@..........S
+0000c3d0: 7461 7274 206f 6620 616e 2041 5350 2066  tart of an ASP f
+0000c3e0: 7261 676d 656e 7420 7769 7468 2040 0700  ragment with @..
+0000c3f0: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000c400: 0103 0000 0036 0042 0065 0067 0069 006e  .....6.B.e.g.i.n
+0000c410: 006e 0020 0065 0069 006e 0065 0073 0020  .n. .e.i.n.e.s. 
+0000c420: 0058 004d 004c 0020 0046 0072 0061 0067  .X.M.L. .F.r.a.g
+0000c430: 006d 0065 006e 0074 0065 0073 0800 0000  .m.e.n.t.e.s....
+0000c440: 0006 0000 0018 5374 6172 7420 6f66 2061  ......Start of a
+0000c450: 6e20 584d 4c20 6672 6167 6d65 6e74 0700  n XML fragment..
+0000c460: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000c470: 0103 0000 0006 0054 0061 0067 0800 0000  .......T.a.g....
+0000c480: 0006 0000 0003 5461 6707 0000 000d 5173  ......Tag.....Qs
+0000c490: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
+0000c4a0: 2800 5500 6e00 6200 6500 6b00 6100 6e00  (.U.n.b.e.k.a.n.
+0000c4b0: 6e00 7400 6500 7300 2000 4100 7400 7400  n.t.e.s. .A.t.t.
+0000c4c0: 7200 6900 6200 7500 7408 0000 0000 0600  r.i.b.u.t.......
+0000c4d0: 0000 1155 6e6b 6e6f 776e 2061 7474 7269  ...Unknown attri
+0000c4e0: 6275 7465 0700 0000 0d51 7363 694c 6578  bute.....QsciLex
+0000c4f0: 6572 4854 4d4c 0103 0000 001e 0055 006e  erHTML.......U.n
+0000c500: 0062 0065 006b 0061 006e 006e 0074 0065  .b.e.k.a.n.n.t.e
+0000c510: 0073 0020 0054 0061 0067 0800 0000 0006  .s. .T.a.g......
+0000c520: 0000 000b 556e 6b6e 6f77 6e20 7461 6707  ....Unknown tag.
+0000c530: 0000 000d 5173 6369 4c65 7865 7248 544d  ....QsciLexerHTM
+0000c540: 4c01 0300 0000 4000 4800 5400 4d00 4c00  L.....@.H.T.M.L.
+0000c550: 2000 5700 6500 7200 7400 2000 6f00 6800   .W.e.r.t. .o.h.
+0000c560: 6e00 6500 2000 4100 6e00 6600 fc00 6800  n.e. .A.n.f...h.
+0000c570: 7200 7500 6e00 6700 7300 7a00 6500 6900  r.u.n.g.s.z.e.i.
+0000c580: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+0000c590: 1355 6e71 756f 7465 6420 4854 4d4c 2076  .Unquoted HTML v
+0000c5a0: 616c 7565 0700 0000 0d51 7363 694c 6578  alue.....QsciLex
+0000c5b0: 6572 4854 4d4c 0103 0000 0024 0056 0042  erHTML.....$.V.B
+0000c5c0: 0053 0063 0072 0069 0070 0074 0020 004b  .S.c.r.i.p.t. .K
+0000c5d0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
+0000c5e0: 0800 0000 0006 0000 0010 5642 5363 7269  ..........VBScri
+0000c5f0: 7074 2063 6f6d 6d65 6e74 0700 0000 0d51  pt comment.....Q
+0000c600: 7363 694c 6578 6572 4854 4d4c 0103 0000  sciLexerHTML....
+0000c610: 0022 0056 0042 0053 0063 0072 0069 0070  .".V.B.S.c.r.i.p
+0000c620: 0074 0020 0053 0074 0061 006e 0064 0061  .t. .S.t.a.n.d.a
+0000c630: 0072 0064 0800 0000 0006 0000 0010 5642  .r.d..........VB
+0000c640: 5363 7269 7074 2064 6566 6175 6c74 0700  Script default..
+0000c650: 0000 0d51 7363 694c 6578 6572 4854 4d4c  ...QsciLexerHTML
+0000c660: 0103 0000 0026 0056 0042 0053 0063 0072  .....&.V.B.S.c.r
+0000c670: 0069 0070 0074 0020 0042 0065 007a 0065  .i.p.t. .B.e.z.e
+0000c680: 0069 0063 0068 006e 0065 0072 0800 0000  .i.c.h.n.e.r....
+0000c690: 0006 0000 0013 5642 5363 7269 7074 2069  ......VBScript i
+0000c6a0: 6465 6e74 6966 6965 7207 0000 000d 5173  dentifier.....Qs
+0000c6b0: 6369 4c65 7865 7248 544d 4c01 0300 0000  ciLexerHTML.....
+0000c6c0: 2c00 5600 4200 5300 6300 7200 6900 7000  ,.V.B.S.c.r.i.p.
+0000c6d0: 7400 2000 5300 6300 6800 6c00 fc00 7300  t. .S.c.h.l...s.
+0000c6e0: 7300 6500 6c00 7700 6f00 7200 7408 0000  s.e.l.w.o.r.t...
+0000c6f0: 0000 0600 0000 1056 4253 6372 6970 7420  .......VBScript 
+0000c700: 6b65 7977 6f72 6407 0000 000d 5173 6369  keyword.....Qsci
+0000c710: 4c65 7865 7248 544d 4c01 0300 0000 1a00  LexerHTML.......
+0000c720: 5600 4200 5300 6300 7200 6900 7000 7400  V.B.S.c.r.i.p.t.
+0000c730: 2000 5a00 6100 6800 6c08 0000 0000 0600   .Z.a.h.l.......
+0000c740: 0000 0f56 4253 6372 6970 7420 6e75 6d62  ...VBScript numb
+0000c750: 6572 0700 0000 0d51 7363 694c 6578 6572  er.....QsciLexer
+0000c760: 4854 4d4c 0103 0000 002a 0056 0042 0053  HTML.....*.V.B.S
+0000c770: 0063 0072 0069 0070 0074 0020 005a 0065  .c.r.i.p.t. .Z.e
+0000c780: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+0000c790: 0074 0065 0800 0000 0006 0000 000f 5642  .t.e..........VB
+0000c7a0: 5363 7269 7074 2073 7472 696e 6707 0000  Script string...
+0000c7b0: 000d 5173 6369 4c65 7865 7248 544d 4c01  ..QsciLexerHTML.
+0000c7c0: 0300 0000 4000 5600 4200 5300 6300 7200  ....@.V.B.S.c.r.
+0000c7d0: 6900 7000 7400 2000 5500 6e00 6200 6500  i.p.t. .U.n.b.e.
+0000c7e0: 6500 6e00 6400 6500 7400 6500 2000 5a00  e.n.d.e.t.e. .Z.
+0000c7f0: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+0000c800: 7400 7400 6508 0000 0000 0600 0000 1856  t.t.e..........V
+0000c810: 4253 6372 6970 7420 756e 636c 6f73 6564  BScript unclosed
+0000c820: 2073 7472 696e 6707 0000 000d 5173 6369   string.....Qsci
+0000c830: 4c65 7865 7248 544d 4c01 0300 0000 1800  LexerHTML.......
+0000c840: 4100 6e00 7a00 6100 6800 6c00 2000 4200  A.n.z.a.h.l. .B.
+0000c850: 7900 7400 6500 7308 0000 0000 0600 0000  y.t.e.s.........
+0000c860: 0a42 7974 6520 636f 756e 7407 0000 000c  .Byte count.....
+0000c870: 5173 6369 4c65 7865 7248 6578 0103 0000  QsciLexerHex....
+0000c880: 0014 0043 0068 0065 0063 006b 0073 0075  ...C.h.e.c.k.s.u
+0000c890: 006d 006d 0065 0800 0000 0006 0000 0008  .m.m.e..........
+0000c8a0: 4368 6563 6b73 756d 0700 0000 0c51 7363  Checksum.....Qsc
+0000c8b0: 694c 6578 6572 4865 7801 0300 0000 1800  iLexerHex.......
+0000c8c0: 4400 6100 7400 6500 6e00 6100 6400 7200  D.a.t.e.n.a.d.r.
+0000c8d0: 6500 7300 7300 6508 0000 0000 0600 0000  e.s.s.e.........
+0000c8e0: 0c44 6174 6120 6164 6472 6573 7307 0000  .Data address...
+0000c8f0: 000c 5173 6369 4c65 7865 7248 6578 0103  ..QsciLexerHex..
+0000c900: 0000 0010 0053 0074 0061 006e 0064 0061  .....S.t.a.n.d.a
+0000c910: 0072 0064 0800 0000 0006 0000 0007 4465  .r.d..........De
+0000c920: 6661 756c 7407 0000 000c 5173 6369 4c65  fault.....QsciLe
+0000c930: 7865 7248 6578 0103 0000 0018 0047 0065  xerHex.......G.e
+0000c940: 0072 0061 0064 0065 0020 0044 0061 0074  .r.a.d.e. .D.a.t
+0000c950: 0065 006e 0800 0000 0006 0000 0009 4576  .e.n..........Ev
+0000c960: 656e 2064 6174 6107 0000 000c 5173 6369  en data.....Qsci
+0000c970: 4c65 7865 7248 6578 0103 0000 0024 0045  LexerHex.....$.E
+0000c980: 0072 0077 0065 0069 0074 0065 0072 0074  .r.w.e.i.t.e.r.t
+0000c990: 0065 0020 0041 0064 0072 0065 0073 0073  .e. .A.d.r.e.s.s
+0000c9a0: 0065 0800 0000 0006 0000 0010 4578 7465  .e..........Exte
+0000c9b0: 6e64 6564 2061 6464 7265 7373 0700 0000  nded address....
+0000c9c0: 0c51 7363 694c 6578 6572 4865 7801 0300  .QsciLexerHex...
+0000c9d0: 0000 3000 4100 6e00 7a00 6100 6800 6c00  ..0.A.n.z.a.h.l.
+0000c9e0: 2000 6900 6e00 6b00 6f00 7200 7200 6500   .i.n.k.o.r.r.e.
+0000c9f0: 6b00 7400 6500 7200 2000 4200 7900 7400  k.t.e.r. .B.y.t.
+0000ca00: 6500 7308 0000 0000 0600 0000 1449 6e63  e.s..........Inc
+0000ca10: 6f72 7265 6374 2062 7974 6520 636f 756e  orrect byte coun
+0000ca20: 7407 0000 000c 5173 6369 4c65 7865 7248  t.....QsciLexerH
+0000ca30: 6578 0103 0000 002a 0049 006e 006b 006f  ex.....*.I.n.k.o
+0000ca40: 0072 0072 0065 006b 0074 0065 0020 0043  .r.r.e.k.t.e. .C
+0000ca50: 0068 0065 0063 006b 0073 0075 006d 006d  .h.e.c.k.s.u.m.m
+0000ca60: 0065 0800 0000 0006 0000 0012 496e 636f  .e..........Inco
+0000ca70: 7272 6563 7420 6368 6563 6b73 756d 0700  rrect checksum..
+0000ca80: 0000 0c51 7363 694c 6578 6572 4865 7801  ...QsciLexerHex.
+0000ca90: 0300 0000 1a00 6b00 6500 6900 6e00 6500  ......k.e.i.n.e.
+0000caa0: 2000 4100 6400 7200 6500 7300 7300 6508   .A.d.r.e.s.s.e.
+0000cab0: 0000 0000 0600 0000 0a4e 6f20 6164 6472  .........No addr
+0000cac0: 6573 7307 0000 000c 5173 6369 4c65 7865  ess.....QsciLexe
+0000cad0: 7248 6578 0103 0000 001c 0055 006e 0067  rHex.......U.n.g
+0000cae0: 0065 0072 0061 0064 0065 0020 0044 0061  .e.r.a.d.e. .D.a
+0000caf0: 0074 0065 006e 0800 0000 0006 0000 0008  .t.e.n..........
+0000cb00: 4f64 6420 6461 7461 0700 0000 0c51 7363  Odd data.....Qsc
+0000cb10: 694c 6578 6572 4865 7801 0300 0000 2200  iLexerHex.....".
+0000cb20: 4100 6e00 7a00 6100 6800 6c00 2000 4400  A.n.z.a.h.l. .D.
+0000cb30: 6100 7400 6500 6e00 7300 e400 7400 7a00  a.t.e.n.s...t.z.
+0000cb40: 6508 0000 0000 0600 0000 0c52 6563 6f72  e..........Recor
+0000cb50: 6420 636f 756e 7407 0000 000c 5173 6369  d count.....Qsci
+0000cb60: 4c65 7865 7248 6578 0103 0000 001e 0044  LexerHex.......D
+0000cb70: 0061 0074 0065 006e 0073 0061 0074 007a  .a.t.e.n.s.a.t.z
+0000cb80: 0061 006e 0066 0061 006e 0067 0800 0000  .a.n.f.a.n.g....
+0000cb90: 0006 0000 000c 5265 636f 7264 2073 7461  ......Record sta
+0000cba0: 7274 0700 0000 0c51 7363 694c 6578 6572  rt.....QsciLexer
+0000cbb0: 4865 7801 0300 0000 1a00 4400 6100 7400  Hex.......D.a.t.
+0000cbc0: 6500 6e00 7300 6100 7400 7a00 6500 6e00  e.n.s.a.t.z.e.n.
+0000cbd0: 6400 6508 0000 0000 0600 0000 0b52 6563  d.e..........Rec
+0000cbe0: 6f72 6420 7479 7065 0700 0000 0c51 7363  ord type.....Qsc
+0000cbf0: 694c 6578 6572 4865 7801 0300 0000 1800  iLexerHex.......
+0000cc00: 5300 7400 6100 7200 7400 6100 6400 7200  S.t.a.r.t.a.d.r.
+0000cc10: 6500 7300 7300 6508 0000 0000 0600 0000  e.s.s.e.........
+0000cc20: 0d53 7461 7274 2061 6464 7265 7373 0700  .Start address..
+0000cc30: 0000 0c51 7363 694c 6578 6572 4865 7801  ...QsciLexerHex.
+0000cc40: 0300 0000 3200 4d00 fc00 6c00 6c00 2000  ....2.M...l.l. .
+0000cc50: 6e00 6100 6300 6800 2000 6500 6900 6e00  n.a.c.h. .e.i.n.
+0000cc60: 6500 6d00 2000 4400 6100 7400 6500 6e00  e.m. .D.a.t.e.n.
+0000cc70: 7300 6100 7400 7a08 0000 0000 0600 0000  s.a.t.z.........
+0000cc80: 1f54 7261 696c 696e 6720 6761 7262 6167  .Trailing garbag
+0000cc90: 6520 6166 7465 7220 6120 7265 636f 7264  e after a record
+0000cca0: 0700 0000 0c51 7363 694c 6578 6572 4865  .....QsciLexerHe
+0000ccb0: 7801 0300 0000 2000 5500 6e00 6200 6500  x..... .U.n.b.e.
+0000ccc0: 6b00 6100 6e00 6e00 7400 6500 2000 4400  k.a.n.n.t.e. .D.
+0000ccd0: 6100 7400 6500 6e08 0000 0000 0600 0000  a.t.e.n.........
+0000cce0: 0c55 6e6b 6e6f 776e 2064 6174 6107 0000  .Unknown data...
+0000ccf0: 000c 5173 6369 4c65 7865 7248 6578 0103  ..QsciLexerHex..
+0000cd00: 0000 002e 0055 006e 0062 0065 006b 0061  .....U.n.b.e.k.a
+0000cd10: 006e 0074 0065 0072 0020 0044 0061 0074  .n.t.e.r. .D.a.t
+0000cd20: 0065 006e 0073 0061 0074 007a 0074 0079  .e.n.s.a.t.z.t.y
+0000cd30: 0070 0800 0000 0006 0000 0013 556e 6b6e  .p..........Unkn
+0000cd40: 6f77 6e20 7265 636f 7264 2074 7970 6507  own record type.
+0000cd50: 0000 000c 5173 6369 4c65 7865 7248 6578  ....QsciLexerHex
+0000cd60: 0103 0000 0008 0055 0055 0049 0044 0800  .......U.U.I.D..
+0000cd70: 0000 0006 0000 0004 5555 4944 0700 0000  ........UUID....
+0000cd80: 0c51 7363 694c 6578 6572 4944 4c01 0300  .QsciLexerIDL...
+0000cd90: 0000 1c00 4200 6c00 6f00 6300 6b00 6b00  ....B.l.o.c.k.k.
+0000cda0: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
+0000cdb0: 0000 0000 0600 0000 0d42 6c6f 636b 2063  .........Block c
+0000cdc0: 6f6d 6d65 6e74 0700 0000 0d51 7363 694c  omment.....QsciL
+0000cdd0: 6578 6572 4a53 4f4e 0103 0000 0010 0053  exerJSON.......S
+0000cde0: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+0000cdf0: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
+0000ce00: 0000 000d 5173 6369 4c65 7865 724a 534f  ....QsciLexerJSO
+0000ce10: 4e01 0300 0000 1c00 4500 7300 6300 6100  N.......E.s.c.a.
+0000ce20: 7000 6500 2d00 5300 6500 7100 7500 6500  p.e.-.S.e.q.u.e.
+0000ce30: 6e00 7a08 0000 0000 0600 0000 0f45 7363  n.z..........Esc
+0000ce40: 6170 6520 7365 7175 656e 6365 0700 0000  ape sequence....
+0000ce50: 0d51 7363 694c 6578 6572 4a53 4f4e 0103  .QsciLexerJSON..
+0000ce60: 0000 0006 0049 0052 0049 0800 0000 0006  .....I.R.I......
+0000ce70: 0000 0003 4952 4907 0000 000d 5173 6369  ....IRI.....Qsci
+0000ce80: 4c65 7865 724a 534f 4e01 0300 0000 2400  LexerJSON.....$.
+0000ce90: 4a00 5300 4f00 4e00 2000 5300 6300 6800  J.S.O.N. .S.c.h.
+0000cea0: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
+0000ceb0: 7200 7408 0000 0000 0600 0000 0c4a 534f  r.t..........JSO
+0000cec0: 4e20 6b65 7977 6f72 6407 0000 000d 5173  N keyword.....Qs
+0000ced0: 6369 4c65 7865 724a 534f 4e01 0300 0000  ciLexerJSON.....
+0000cee0: 2a00 4a00 5300 4f00 4e00 2d00 4c00 4400  *.J.S.O.N.-.L.D.
+0000cef0: 2000 6b00 6f00 6d00 7000 6100 6b00 7400   .k.o.m.p.a.k.t.
+0000cf00: 6500 7300 2000 4900 5200 4908 0000 0000  e.s. .I.R.I.....
+0000cf10: 0600 0000 134a 534f 4e2d 4c44 2063 6f6d  .....JSON-LD com
+0000cf20: 7061 6374 2049 5249 0700 0000 0d51 7363  pact IRI.....Qsc
+0000cf30: 694c 6578 6572 4a53 4f4e 0103 0000 002a  iLexerJSON.....*
+0000cf40: 004a 0053 004f 004e 002d 004c 0044 0020  .J.S.O.N.-.L.D. 
+0000cf50: 0053 0063 0068 006c 00fc 0073 0073 0065  .S.c.h.l...s.s.e
+0000cf60: 006c 0077 006f 0072 0074 0800 0000 0006  .l.w.o.r.t......
+0000cf70: 0000 000f 4a53 4f4e 2d4c 4420 6b65 7977  ....JSON-LD keyw
+0000cf80: 6f72 6407 0000 000d 5173 6369 4c65 7865  ord.....QsciLexe
+0000cf90: 724a 534f 4e01 0300 0000 1e00 5a00 6500  rJSON.......Z.e.
+0000cfa0: 6900 6c00 6500 6e00 6b00 6f00 6d00 6d00  i.l.e.n.k.o.m.m.
+0000cfb0: 6500 6e00 7400 6100 7208 0000 0000 0600  e.n.t.a.r.......
+0000cfc0: 0000 0c4c 696e 6520 636f 6d6d 656e 7407  ...Line comment.
+0000cfd0: 0000 000d 5173 6369 4c65 7865 724a 534f  ....QsciLexerJSO
+0000cfe0: 4e01 0300 0000 0800 5a00 6100 6800 6c08  N.......Z.a.h.l.
+0000cff0: 0000 0000 0600 0000 064e 756d 6265 7207  .........Number.
+0000d000: 0000 000d 5173 6369 4c65 7865 724a 534f  ....QsciLexerJSO
+0000d010: 4e01 0300 0000 1000 4f00 7000 6500 7200  N.......O.p.e.r.
+0000d020: 6100 7400 6f00 7208 0000 0000 0600 0000  a.t.o.r.........
+0000d030: 084f 7065 7261 746f 7207 0000 000d 5173  .Operator.....Qs
+0000d040: 6369 4c65 7865 724a 534f 4e01 0300 0000  ciLexerJSON.....
+0000d050: 1a00 4100 6e00 6100 6c00 7900 7300 6500  ..A.n.a.l.y.s.e.
+0000d060: 6600 6500 6800 6c00 6500 7208 0000 0000  f.e.h.l.e.r.....
+0000d070: 0600 0000 0d50 6172 7369 6e67 2065 7272  .....Parsing err
+0000d080: 6f72 0700 0000 0d51 7363 694c 6578 6572  or.....QsciLexer
+0000d090: 4a53 4f4e 0103 0000 0016 0045 0069 0067  JSON.......E.i.g
+0000d0a0: 0065 006e 0073 0063 0068 0061 0066 0074  .e.n.s.c.h.a.f.t
+0000d0b0: 0800 0000 0006 0000 0008 5072 6f70 6572  ..........Proper
+0000d0c0: 7479 0700 0000 0d51 7363 694c 6578 6572  ty.....QsciLexer
+0000d0d0: 4a53 4f4e 0103 0000 0018 005a 0065 0069  JSON.......Z.e.i
+0000d0e0: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
+0000d0f0: 0065 0800 0000 0006 0000 0006 5374 7269  .e..........Stri
+0000d100: 6e67 0700 0000 0d51 7363 694c 6578 6572  ng.....QsciLexer
+0000d110: 4a53 4f4e 0103 0000 002e 0055 006e 0062  JSON.......U.n.b
+0000d120: 0065 0065 006e 0064 0065 0074 0065 0020  .e.e.n.d.e.t.e. 
+0000d130: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+0000d140: 0065 0074 0074 0065 0800 0000 0006 0000  .e.t.t.e........
+0000d150: 000f 556e 636c 6f73 6564 2073 7472 696e  ..Unclosed strin
+0000d160: 6707 0000 000d 5173 6369 4c65 7865 724a  g.....QsciLexerJ
+0000d170: 534f 4e01 0300 0000 2400 5200 6500 6700  SON.....$.R.e.g.
+0000d180: 7500 6c00 e400 7200 6500 7200 2000 4100  u.l...r.e.r. .A.
+0000d190: 7500 7300 6400 7200 7500 6300 6b08 0000  u.s.d.r.u.c.k...
+0000d1a0: 0000 0600 0000 1252 6567 756c 6172 2065  .......Regular e
+0000d1b0: 7870 7265 7373 696f 6e07 0000 0013 5173  xpression.....Qs
+0000d1c0: 6369 4c65 7865 724a 6176 6153 6372 6970  ciLexerJavaScrip
+0000d1d0: 7401 0300 0000 1e00 4200 6100 7300 6900  t.......B.a.s.i.
+0000d1e0: 7300 6600 7500 6e00 6b00 7400 6900 6f00  s.f.u.n.k.t.i.o.
+0000d1f0: 6e00 6500 6e08 0000 0000 0600 0000 0f42  n.e.n..........B
+0000d200: 6173 6963 2066 756e 6374 696f 6e73 0700  asic functions..
+0000d210: 0000 0c51 7363 694c 6578 6572 4c75 6101  ...QsciLexerLua.
+0000d220: 0300 0000 0e00 5a00 6500 6900 6300 6800  ......Z.e.i.c.h.
+0000d230: 6500 6e08 0000 0000 0600 0000 0943 6861  e.n..........Cha
+0000d240: 7261 6374 6572 0700 0000 0c51 7363 694c  racter.....QsciL
+0000d250: 6578 6572 4c75 6101 0300 0000 1200 4b00  exerLua.......K.
+0000d260: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
+0000d270: 0000 0000 0600 0000 0743 6f6d 6d65 6e74  .........Comment
+0000d280: 0700 0000 0c51 7363 694c 6578 6572 4c75  .....QsciLexerLu
+0000d290: 6101 0300 0000 4a00 4b00 6f00 7200 6f00  a.....J.K.o.r.o.
+0000d2a0: 7500 7400 6900 6e00 6500 6e00 2c00 2000  u.t.i.n.e.n.,. .
+0000d2b0: 4900 2f00 4f00 2d00 2000 7500 6e00 6400  I./.O.-. .u.n.d.
+0000d2c0: 2000 5300 7900 7300 7400 6500 6d00 6600   .S.y.s.t.e.m.f.
+0000d2d0: 7500 6e00 6b00 7400 6900 6f00 6e00 6500  u.n.k.t.i.o.n.e.
+0000d2e0: 6e08 0000 0000 0600 0000 2543 6f72 6f75  n.........%Corou
+0000d2f0: 7469 6e65 732c 2069 2f6f 2061 6e64 2073  tines, i/o and s
+0000d300: 7973 7465 6d20 6661 6369 6c69 7469 6573  ystem facilities
+0000d310: 0700 0000 0c51 7363 694c 6578 6572 4c75  .....QsciLexerLu
+0000d320: 6101 0300 0000 1000 5300 7400 6100 6e00  a.......S.t.a.n.
+0000d330: 6400 6100 7200 6408 0000 0000 0600 0000  d.a.r.d.........
+0000d340: 0744 6566 6175 6c74 0700 0000 0c51 7363  .Default.....Qsc
+0000d350: 694c 6578 6572 4c75 6101 0300 0000 1400  iLexerLua.......
+0000d360: 4200 6500 7a00 6500 6900 6300 6800 6e00  B.e.z.e.i.c.h.n.
+0000d370: 6500 7208 0000 0000 0600 0000 0a49 6465  e.r..........Ide
+0000d380: 6e74 6966 6965 7207 0000 000c 5173 6369  ntifier.....Qsci
+0000d390: 4c65 7865 724c 7561 0103 0000 001a 0053  LexerLua.......S
+0000d3a0: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
+0000d3b0: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
+0000d3c0: 0007 4b65 7977 6f72 6407 0000 000c 5173  ..Keyword.....Qs
+0000d3d0: 6369 4c65 7865 724c 7561 0103 0000 000a  ciLexerLua......
+0000d3e0: 004d 0061 0072 006b 0065 0800 0000 0006  .M.a.r.k.e......
+0000d3f0: 0000 0005 4c61 6265 6c07 0000 000c 5173  ....Label.....Qs
+0000d400: 6369 4c65 7865 724c 7561 0103 0000 001e  ciLexerLua......
+0000d410: 005a 0065 0069 006c 0065 006e 006b 006f  .Z.e.i.l.e.n.k.o
+0000d420: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+0000d430: 0000 0006 0000 000c 4c69 6e65 2063 6f6d  ........Line com
+0000d440: 6d65 6e74 0700 0000 0c51 7363 694c 6578  ment.....QsciLex
+0000d450: 6572 4c75 6101 0300 0000 3a00 5500 6e00  erLua.....:.U.n.
+0000d460: 6900 6e00 7400 6500 7200 7000 7200 6500  i.n.t.e.r.p.r.e.
+0000d470: 7400 6900 6500 7200 7400 6500 2000 5a00  t.i.e.r.t.e. .Z.
+0000d480: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+0000d490: 7400 7400 6508 0000 0000 0600 0000 0e4c  t.t.e..........L
+0000d4a0: 6974 6572 616c 2073 7472 696e 6707 0000  iteral string...
+0000d4b0: 000c 5173 6369 4c65 7865 724c 7561 0103  ..QsciLexerLua..
+0000d4c0: 0000 0008 005a 0061 0068 006c 0800 0000  .....Z.a.h.l....
+0000d4d0: 0006 0000 0006 4e75 6d62 6572 0700 0000  ......Number....
+0000d4e0: 0c51 7363 694c 6578 6572 4c75 6101 0300  .QsciLexerLua...
+0000d4f0: 0000 1000 4f00 7000 6500 7200 6100 7400  ....O.p.e.r.a.t.
+0000d500: 6f00 7208 0000 0000 0600 0000 084f 7065  o.r..........Ope
+0000d510: 7261 746f 7207 0000 000c 5173 6369 4c65  rator.....QsciLe
+0000d520: 7865 724c 7561 0103 0000 0018 0050 0072  xerLua.......P.r
+0000d530: 00e4 0070 0072 006f 007a 0065 0073 0073  ...p.r.o.z.e.s.s
+0000d540: 006f 0072 0800 0000 0006 0000 000c 5072  .o.r..........Pr
+0000d550: 6570 726f 6365 7373 6f72 0700 0000 0c51  eprocessor.....Q
+0000d560: 7363 694c 6578 6572 4c75 6101 0300 0000  sciLexerLua.....
+0000d570: 1800 5a00 6500 6900 6300 6800 6500 6e00  ..Z.e.i.c.h.e.n.
+0000d580: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
+0000d590: 0000 0653 7472 696e 6707 0000 000c 5173  ...String.....Qs
+0000d5a0: 6369 4c65 7865 724c 7561 0103 0000 006a  ciLexerLua.....j
+0000d5b0: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+0000d5c0: 0065 0074 0074 0065 006e 002d 002c 0020  .e.t.t.e.n.-.,. 
+0000d5d0: 0054 0061 0062 0065 006c 006c 0065 002d  .T.a.b.e.l.l.e.-
+0000d5e0: 0020 0075 006e 0064 0020 006d 0061 0074  . .u.n.d. .m.a.t
+0000d5f0: 0068 0065 006d 0061 0074 0069 0073 0063  .h.e.m.a.t.i.s.c
+0000d600: 0068 0065 0020 0046 0075 006e 006b 0074  .h.e. .F.u.n.k.t
+0000d610: 0069 006f 006e 0065 006e 0800 0000 0006  .i.o.n.e.n......
+0000d620: 0000 0021 5374 7269 6e67 2c20 7461 626c  ...!String, tabl
+0000d630: 6520 616e 6420 6d61 7468 7320 6675 6e63  e and maths func
+0000d640: 7469 6f6e 7307 0000 000c 5173 6369 4c65  tions.....QsciLe
+0000d650: 7865 724c 7561 0103 0000 002e 0055 006e  xerLua.......U.n
+0000d660: 0062 0065 0065 006e 0064 0065 0074 0065  .b.e.e.n.d.e.t.e
+0000d670: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
+0000d680: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
+0000d690: 0000 000f 556e 636c 6f73 6564 2073 7472  ....Unclosed str
+0000d6a0: 696e 6707 0000 000c 5173 6369 4c65 7865  ing.....QsciLexe
+0000d6b0: 724c 7561 0103 0000 0024 004e 0075 0074  rLua.....$.N.u.t
+0000d6c0: 007a 0065 0072 0020 0064 0065 0066 0069  .z.e.r. .d.e.f.i
+0000d6d0: 006e 0069 0065 0072 0074 0020 0031 0800  .n.i.e.r.t. .1..
+0000d6e0: 0000 0006 0000 000e 5573 6572 2064 6566  ........User def
+0000d6f0: 696e 6564 2031 0700 0000 0c51 7363 694c  ined 1.....QsciL
+0000d700: 6578 6572 4c75 6101 0300 0000 2400 4e00  exerLua.....$.N.
+0000d710: 7500 7400 7a00 6500 7200 2000 6400 6500  u.t.z.e.r. .d.e.
+0000d720: 6600 6900 6e00 6900 6500 7200 7400 2000  f.i.n.i.e.r.t. .
+0000d730: 3208 0000 0000 0600 0000 0e55 7365 7220  2..........User 
+0000d740: 6465 6669 6e65 6420 3207 0000 000c 5173  defined 2.....Qs
+0000d750: 6369 4c65 7865 724c 7561 0103 0000 0024  ciLexerLua.....$
+0000d760: 004e 0075 0074 007a 0065 0072 0020 0064  .N.u.t.z.e.r. .d
+0000d770: 0065 0066 0069 006e 0069 0065 0072 0074  .e.f.i.n.i.e.r.t
+0000d780: 0020 0033 0800 0000 0006 0000 000e 5573  . .3..........Us
+0000d790: 6572 2064 6566 696e 6564 2033 0700 0000  er defined 3....
+0000d7a0: 0c51 7363 694c 6578 6572 4c75 6101 0300  .QsciLexerLua...
+0000d7b0: 0000 2400 4e00 7500 7400 7a00 6500 7200  ..$.N.u.t.z.e.r.
+0000d7c0: 2000 6400 6500 6600 6900 6e00 6900 6500   .d.e.f.i.n.i.e.
+0000d7d0: 7200 7400 2000 3408 0000 0000 0600 0000  r.t. .4.........
+0000d7e0: 0e55 7365 7220 6465 6669 6e65 6420 3407  .User defined 4.
+0000d7f0: 0000 000c 5173 6369 4c65 7865 724c 7561  ....QsciLexerLua
+0000d800: 0103 0000 0012 004b 006f 006d 006d 0065  .......K.o.m.m.e
+0000d810: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
+0000d820: 0007 436f 6d6d 656e 7407 0000 0011 5173  ..Comment.....Qs
+0000d830: 6369 4c65 7865 724d 616b 6566 696c 6501  ciLexerMakefile.
+0000d840: 0300 0000 1000 5300 7400 6100 6e00 6400  ......S.t.a.n.d.
+0000d850: 6100 7200 6408 0000 0000 0600 0000 0744  a.r.d..........D
+0000d860: 6566 6175 6c74 0700 0000 1151 7363 694c  efault.....QsciL
+0000d870: 6578 6572 4d61 6b65 6669 6c65 0103 0000  exerMakefile....
+0000d880: 000c 0046 0065 0068 006c 0065 0072 0800  ...F.e.h.l.e.r..
+0000d890: 0000 0006 0000 0005 4572 726f 7207 0000  ........Error...
+0000d8a0: 0011 5173 6369 4c65 7865 724d 616b 6566  ..QsciLexerMakef
+0000d8b0: 696c 6501 0300 0000 1000 4f00 7000 6500  ile.......O.p.e.
+0000d8c0: 7200 6100 7400 6f00 7208 0000 0000 0600  r.a.t.o.r.......
+0000d8d0: 0000 084f 7065 7261 746f 7207 0000 0011  ...Operator.....
+0000d8e0: 5173 6369 4c65 7865 724d 616b 6566 696c  QsciLexerMakefil
+0000d8f0: 6501 0300 0000 1800 5000 7200 e400 7000  e.......P.r...p.
+0000d900: 7200 6f00 7a00 6500 7300 7300 6f00 7208  r.o.z.e.s.s.o.r.
+0000d910: 0000 0000 0600 0000 0c50 7265 7072 6f63  .........Preproc
+0000d920: 6573 736f 7207 0000 0011 5173 6369 4c65  essor.....QsciLe
+0000d930: 7865 724d 616b 6566 696c 6501 0300 0000  xerMakefile.....
+0000d940: 0800 5a00 6900 6500 6c08 0000 0000 0600  ..Z.i.e.l.......
+0000d950: 0000 0654 6172 6765 7407 0000 0011 5173  ...Target.....Qs
+0000d960: 6369 4c65 7865 724d 616b 6566 696c 6501  ciLexerMakefile.
+0000d970: 0300 0000 1000 5600 6100 7200 6900 6100  ......V.a.r.i.a.
+0000d980: 6200 6c00 6508 0000 0000 0600 0000 0856  b.l.e..........V
+0000d990: 6172 6961 626c 6507 0000 0011 5173 6369  ariable.....Qsci
+0000d9a0: 4c65 7865 724d 616b 6566 696c 6501 0300  LexerMakefile...
+0000d9b0: 0000 1400 4200 6c00 6f00 6300 6b00 7a00  ....B.l.o.c.k.z.
+0000d9c0: 6900 7400 6100 7408 0000 0000 0600 0000  i.t.a.t.........
+0000d9d0: 0b42 6c6f 636b 2071 756f 7465 0700 0000  .Block quote....
+0000d9e0: 1151 7363 694c 6578 6572 4d61 726b 646f  .QsciLexerMarkdo
+0000d9f0: 776e 0103 0000 002e 0043 006f 0064 0065  wn.......C.o.d.e
+0000da00: 0020 007a 0077 0069 0073 0063 0068 0065  . .z.w.i.s.c.h.e
+0000da10: 006e 0020 0042 0061 0063 006b 0074 0069  .n. .B.a.c.k.t.i
+0000da20: 0063 006b 0073 0800 0000 0006 0000 0016  .c.k.s..........
+0000da30: 436f 6465 2062 6574 7765 656e 2062 6163  Code between bac
+0000da40: 6b74 6963 6b73 0700 0000 1151 7363 694c  kticks.....QsciL
+0000da50: 6578 6572 4d61 726b 646f 776e 0103 0000  exerMarkdown....
+0000da60: 0042 0043 006f 0064 0065 0020 007a 0077  .B.C.o.d.e. .z.w
+0000da70: 0069 0073 0063 0068 0065 006e 0020 0064  .i.s.c.h.e.n. .d
+0000da80: 006f 0070 0070 0065 006c 0074 0065 006e  .o.p.p.e.l.t.e.n
+0000da90: 0020 0042 0061 0063 006b 0074 0069 0063  . .B.a.c.k.t.i.c
+0000daa0: 006b 0073 0800 0000 0006 0000 001d 436f  .k.s..........Co
+0000dab0: 6465 2062 6574 7765 656e 2064 6f75 626c  de between doubl
+0000dac0: 6520 6261 636b 7469 636b 7307 0000 0011  e backticks.....
+0000dad0: 5173 6369 4c65 7865 724d 6172 6b64 6f77  QsciLexerMarkdow
+0000dae0: 6e01 0300 0000 1200 4300 6f00 6400 6500  n.......C.o.d.e.
+0000daf0: 6200 6c00 6f00 6300 6b08 0000 0000 0600  b.l.o.c.k.......
+0000db00: 0000 0a43 6f64 6520 626c 6f63 6b07 0000  ...Code block...
+0000db10: 0011 5173 6369 4c65 7865 724d 6172 6b64  ..QsciLexerMarkd
+0000db20: 6f77 6e01 0300 0000 1000 5300 7400 6100  own.......S.t.a.
+0000db30: 6e00 6400 6100 7200 6408 0000 0000 0600  n.d.a.r.d.......
+0000db40: 0000 0744 6566 6175 6c74 0700 0000 1151  ...Default.....Q
+0000db50: 7363 694c 6578 6572 4d61 726b 646f 776e  sciLexerMarkdown
+0000db60: 0103 0000 004a 004b 0075 0072 0073 0069  .....J.K.u.r.s.i
+0000db70: 0076 0065 0020 0053 0063 0068 0072 0069  .v.e. .S.c.h.r.i
+0000db80: 0066 0074 0020 006d 0069 0074 0020 0065  .f.t. .m.i.t. .e
+0000db90: 0069 006e 0066 0061 0063 0068 0065 006e  .i.n.f.a.c.h.e.n
+0000dba0: 0020 0053 0074 0065 0072 006e 0065 006e  . .S.t.e.r.n.e.n
+0000dbb0: 0800 0000 0006 0000 001f 456d 7068 6173  ..........Emphas
+0000dbc0: 6973 2075 7369 6e67 2073 696e 676c 6520  is using single 
+0000dbd0: 6173 7465 7269 736b 7307 0000 0011 5173  asterisks.....Qs
+0000dbe0: 6369 4c65 7865 724d 6172 6b64 6f77 6e01  ciLexerMarkdown.
+0000dbf0: 0300 0000 5600 4b00 7500 7200 7300 6900  ....V.K.u.r.s.i.
+0000dc00: 7600 6500 2000 5300 6300 6800 7200 6900  v.e. .S.c.h.r.i.
+0000dc10: 6600 7400 2000 6d00 6900 7400 2000 6500  f.t. .m.i.t. .e.
+0000dc20: 6900 6e00 6600 6100 6300 6800 6500 6e00  i.n.f.a.c.h.e.n.
+0000dc30: 2000 5500 6e00 7400 6500 7200 7300 7400   .U.n.t.e.r.s.t.
+0000dc40: 7200 6900 6300 6800 6500 6e08 0000 0000  r.i.c.h.e.n.....
+0000dc50: 0600 0000 2145 6d70 6861 7369 7320 7573  ....!Emphasis us
+0000dc60: 696e 6720 7369 6e67 6c65 2075 6e64 6572  ing single under
+0000dc70: 7363 6f72 6573 0700 0000 1151 7363 694c  scores.....QsciL
+0000dc80: 6578 6572 4d61 726b 646f 776e 0103 0000  exerMarkdown....
+0000dc90: 0022 0048 006f 0072 0069 007a 006f 006e  .".H.o.r.i.z.o.n
+0000dca0: 0074 0061 006c 0065 0020 004c 0069 006e  .t.a.l.e. .L.i.n
+0000dcb0: 0069 0065 0800 0000 0006 0000 000f 486f  .i.e..........Ho
+0000dcc0: 7269 7a6f 6e74 616c 2072 756c 6507 0000  rizontal rule...
+0000dcd0: 0011 5173 6369 4c65 7865 724d 6172 6b64  ..QsciLexerMarkd
+0000dce0: 6f77 6e01 0300 0000 2600 dc00 6200 6500  own.....&...b.e.
+0000dcf0: 7200 7300 6300 6800 7200 6900 6600 7400  r.s.c.h.r.i.f.t.
+0000dd00: 2000 4500 6200 6500 6e00 6500 2000 3108   .E.b.e.n.e. .1.
+0000dd10: 0000 0000 0600 0000 0e4c 6576 656c 2031  .........Level 1
+0000dd20: 2068 6561 6465 7207 0000 0011 5173 6369   header.....Qsci
+0000dd30: 4c65 7865 724d 6172 6b64 6f77 6e01 0300  LexerMarkdown...
+0000dd40: 0000 2600 dc00 6200 6500 7200 7300 6300  ..&...b.e.r.s.c.
+0000dd50: 6800 7200 6900 6600 7400 2000 4500 6200  h.r.i.f.t. .E.b.
+0000dd60: 6500 6e00 6500 2000 3208 0000 0000 0600  e.n.e. .2.......
+0000dd70: 0000 0e4c 6576 656c 2032 2068 6561 6465  ...Level 2 heade
+0000dd80: 7207 0000 0011 5173 6369 4c65 7865 724d  r.....QsciLexerM
+0000dd90: 6172 6b64 6f77 6e01 0300 0000 2600 dc00  arkdown.....&...
+0000dda0: 6200 6500 7200 7300 6300 6800 7200 6900  b.e.r.s.c.h.r.i.
+0000ddb0: 6600 7400 2000 4500 6200 6500 6e00 6500  f.t. .E.b.e.n.e.
+0000ddc0: 2000 3308 0000 0000 0600 0000 0e4c 6576   .3..........Lev
+0000ddd0: 656c 2033 2068 6561 6465 7207 0000 0011  el 3 header.....
+0000dde0: 5173 6369 4c65 7865 724d 6172 6b64 6f77  QsciLexerMarkdow
+0000ddf0: 6e01 0300 0000 2600 dc00 6200 6500 7200  n.....&...b.e.r.
+0000de00: 7300 6300 6800 7200 6900 6600 7400 2000  s.c.h.r.i.f.t. .
+0000de10: 4500 6200 6500 6e00 6500 2000 3408 0000  E.b.e.n.e. .4...
+0000de20: 0000 0600 0000 0e4c 6576 656c 2034 2068  .......Level 4 h
+0000de30: 6561 6465 7207 0000 0011 5173 6369 4c65  eader.....QsciLe
+0000de40: 7865 724d 6172 6b64 6f77 6e01 0300 0000  xerMarkdown.....
+0000de50: 2600 dc00 6200 6500 7200 7300 6300 6800  &...b.e.r.s.c.h.
+0000de60: 7200 6900 6600 7400 2000 4500 6200 6500  r.i.f.t. .E.b.e.
+0000de70: 6e00 6500 2000 3508 0000 0000 0600 0000  n.e. .5.........
+0000de80: 0e4c 6576 656c 2035 2068 6561 6465 7207  .Level 5 header.
+0000de90: 0000 0011 5173 6369 4c65 7865 724d 6172  ....QsciLexerMar
+0000dea0: 6b64 6f77 6e01 0300 0000 2600 dc00 6200  kdown.....&...b.
+0000deb0: 6500 7200 7300 6300 6800 7200 6900 6600  e.r.s.c.h.r.i.f.
+0000dec0: 7400 2000 4500 6200 6500 6e00 6500 2000  t. .E.b.e.n.e. .
+0000ded0: 3608 0000 0000 0600 0000 0e4c 6576 656c  6..........Level
+0000dee0: 2036 2068 6561 6465 7207 0000 0011 5173   6 header.....Qs
+0000def0: 6369 4c65 7865 724d 6172 6b64 6f77 6e01  ciLexerMarkdown.
+0000df00: 0300 0000 1200 4800 7900 7000 6500 7200  ......H.y.p.e.r.
+0000df10: 6c00 6900 6e00 6b08 0000 0000 0600 0000  l.i.n.k.........
+0000df20: 044c 696e 6b07 0000 0011 5173 6369 4c65  .Link.....QsciLe
+0000df30: 7865 724d 6172 6b64 6f77 6e01 0300 0000  xerMarkdown.....
+0000df40: 3400 4e00 7500 6d00 6d00 6500 7200 6900  4.N.u.m.m.e.r.i.
+0000df50: 6500 7200 7400 6500 7300 2000 4c00 6900  e.r.t.e.s. .L.i.
+0000df60: 7300 7400 6500 6e00 6500 6c00 6500 6d00  s.t.e.n.e.l.e.m.
+0000df70: 6500 6e00 7408 0000 0000 0600 0000 114f  e.n.t..........O
+0000df80: 7264 6572 6564 206c 6973 7420 6974 656d  rdered list item
+0000df90: 0700 0000 1151 7363 694c 6578 6572 4d61  .....QsciLexerMa
+0000dfa0: 726b 646f 776e 0103 0000 0024 0045 0069  rkdown.....$.E.i
+0000dfb0: 006e 006c 0065 0069 0074 0075 006e 0067  .n.l.e.i.t.u.n.g
+0000dfc0: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
+0000dfd0: 0800 0000 0006 0000 0008 5072 652d 6368  ..........Pre-ch
+0000dfe0: 6172 0700 0000 1151 7363 694c 6578 6572  ar.....QsciLexer
+0000dff0: 4d61 726b 646f 776e 0103 0000 000e 0053  Markdown.......S
+0000e000: 0070 0065 007a 0069 0061 006c 0800 0000  .p.e.z.i.a.l....
+0000e010: 0006 0000 0007 5370 6563 6961 6c07 0000  ......Special...
+0000e020: 0011 5173 6369 4c65 7865 724d 6172 6b64  ..QsciLexerMarkd
+0000e030: 6f77 6e01 0300 0000 1e00 4400 7500 7200  own.......D.u.r.
+0000e040: 6300 6800 6700 6500 7300 7400 7200 6900  c.h.g.e.s.t.r.i.
+0000e050: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+0000e060: 0a53 7472 696b 6520 6f75 7407 0000 0011  .Strike out.....
+0000e070: 5173 6369 4c65 7865 724d 6172 6b64 6f77  QsciLexerMarkdow
+0000e080: 6e01 0300 0000 4200 4600 6500 7400 7400  n.....B.F.e.t.t.
+0000e090: 7300 6300 6800 7200 6900 6600 7400 2000  s.c.h.r.i.f.t. .
+0000e0a0: 6d00 6900 7400 2000 6400 6f00 7000 7000  m.i.t. .d.o.p.p.
+0000e0b0: 6500 6c00 7400 6500 6e00 2000 5300 7400  e.l.t.e.n. .S.t.
+0000e0c0: 6500 7200 6e00 6500 6e08 0000 0000 0600  e.r.n.e.n.......
+0000e0d0: 0000 2653 7472 6f6e 6720 656d 7068 6173  ..&Strong emphas
+0000e0e0: 6973 2075 7369 6e67 2064 6f75 626c 6520  is using double 
+0000e0f0: 6173 7465 7269 736b 7307 0000 0011 5173  asterisks.....Qs
+0000e100: 6369 4c65 7865 724d 6172 6b64 6f77 6e01  ciLexerMarkdown.
+0000e110: 0300 0000 4e00 4600 6500 7400 7400 7300  ....N.F.e.t.t.s.
+0000e120: 6300 6800 7200 6900 6600 7400 2000 6d00  c.h.r.i.f.t. .m.
+0000e130: 6900 7400 2000 6400 6f00 7000 7000 6500  i.t. .d.o.p.p.e.
+0000e140: 6c00 7400 6500 6e00 2000 5500 6e00 7400  l.t.e.n. .U.n.t.
+0000e150: 6500 7200 7300 7400 7200 6900 6300 6800  e.r.s.t.r.i.c.h.
+0000e160: 6500 6e08 0000 0000 0600 0000 2853 7472  e.n.........(Str
+0000e170: 6f6e 6720 656d 7068 6173 6973 2075 7369  ong emphasis usi
+0000e180: 6e67 2064 6f75 626c 6520 756e 6465 7273  ng double unders
+0000e190: 636f 7265 7307 0000 0011 5173 6369 4c65  cores.....QsciLe
+0000e1a0: 7865 724d 6172 6b64 6f77 6e01 0300 0000  xerMarkdown.....
+0000e1b0: 4000 4e00 6900 6300 6800 7400 2000 6e00  @.N.i.c.h.t. .n.
+0000e1c0: 7500 6d00 6d00 6500 7200 6900 6500 7200  u.m.m.e.r.i.e.r.
+0000e1d0: 7400 6500 7300 2000 4c00 6900 7300 7400  t.e.s. .L.i.s.t.
+0000e1e0: 6500 6e00 6500 6c00 6500 6d00 6500 6e00  e.n.e.l.e.m.e.n.
+0000e1f0: 7408 0000 0000 0600 0000 1355 6e6f 7264  t..........Unord
+0000e200: 6572 6564 206c 6973 7420 6974 656d 0700  ered list item..
+0000e210: 0000 1151 7363 694c 6578 6572 4d61 726b  ...QsciLexerMark
+0000e220: 646f 776e 0103 0000 000c 0042 0065 0066  down.......B.e.f
+0000e230: 0065 0068 006c 0800 0000 0006 0000 0007  .e.h.l..........
+0000e240: 436f 6d6d 616e 6407 0000 000f 5173 6369  Command.....Qsci
+0000e250: 4c65 7865 724d 6174 6c61 6201 0300 0000  LexerMatlab.....
+0000e260: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
+0000e270: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
+0000e280: 6d65 6e74 0700 0000 0f51 7363 694c 6578  ment.....QsciLex
+0000e290: 6572 4d61 746c 6162 0103 0000 0010 0053  erMatlab.......S
+0000e2a0: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+0000e2b0: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
+0000e2c0: 0000 000f 5173 6369 4c65 7865 724d 6174  ....QsciLexerMat
+0000e2d0: 6c61 6201 0300 0000 4200 5a00 6500 6900  lab.....B.Z.e.i.
+0000e2e0: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
+0000e2f0: 6500 2000 6900 6e00 2000 4100 6e00 6600  e. .i.n. .A.n.f.
+0000e300: fc00 6800 7200 7500 6e00 6700 7300 7a00  ..h.r.u.n.g.s.z.
+0000e310: 6500 6900 6300 6800 6500 6e08 0000 0000  e.i.c.h.e.n.....
+0000e320: 0600 0000 1444 6f75 626c 652d 7175 6f74  .....Double-quot
+0000e330: 6564 2073 7472 696e 6707 0000 000f 5173  ed string.....Qs
+0000e340: 6369 4c65 7865 724d 6174 6c61 6201 0300  ciLexerMatlab...
+0000e350: 0000 1400 4200 6500 7a00 6500 6900 6300  ....B.e.z.e.i.c.
+0000e360: 6800 6e00 6500 7208 0000 0000 0600 0000  h.n.e.r.........
+0000e370: 0a49 6465 6e74 6966 6965 7207 0000 000f  .Identifier.....
+0000e380: 5173 6369 4c65 7865 724d 6174 6c61 6201  QsciLexerMatlab.
+0000e390: 0300 0000 1a00 5300 6300 6800 6c00 fc00  ......S.c.h.l...
+0000e3a0: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
+0000e3b0: 0000 0000 0600 0000 074b 6579 776f 7264  .........Keyword
+0000e3c0: 0700 0000 0f51 7363 694c 6578 6572 4d61  .....QsciLexerMa
+0000e3d0: 746c 6162 0103 0000 0008 005a 0061 0068  tlab.......Z.a.h
+0000e3e0: 006c 0800 0000 0006 0000 0006 4e75 6d62  .l..........Numb
+0000e3f0: 6572 0700 0000 0f51 7363 694c 6578 6572  er.....QsciLexer
+0000e400: 4d61 746c 6162 0103 0000 0010 004f 0070  Matlab.......O.p
+0000e410: 0065 0072 0061 0074 006f 0072 0800 0000  .e.r.a.t.o.r....
+0000e420: 0006 0000 0008 4f70 6572 6174 6f72 0700  ......Operator..
+0000e430: 0000 0f51 7363 694c 6578 6572 4d61 746c  ...QsciLexerMatl
+0000e440: 6162 0103 0000 0036 005a 0065 0069 0063  ab.....6.Z.e.i.c
+0000e450: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
+0000e460: 0020 0069 006e 0020 0048 006f 0063 0068  . .i.n. .H.o.c.h
+0000e470: 006b 006f 006d 006d 0061 0074 0061 0800  .k.o.m.m.a.t.a..
+0000e480: 0000 0006 0000 0014 5369 6e67 6c65 2d71  ........Single-q
+0000e490: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
+0000e4a0: 0f51 7363 694c 6578 6572 4d61 746c 6162  .QsciLexerMatlab
+0000e4b0: 0103 0000 0012 004b 006f 006d 006d 0065  .......K.o.m.m.e
+0000e4c0: 006e 0074 0061 0072 0800 0000 0006 0000  .n.t.a.r........
+0000e4d0: 0007 436f 6d6d 656e 7407 0000 000b 5173  ..Comment.....Qs
+0000e4e0: 6369 4c65 7865 7250 4f01 0300 0000 1000  ciLexerPO.......
+0000e4f0: 5300 7400 6100 6e00 6400 6100 7200 6408  S.t.a.n.d.a.r.d.
+0000e500: 0000 0000 0600 0000 0744 6566 6175 6c74  .........Default
+0000e510: 0700 0000 0b51 7363 694c 6578 6572 504f  .....QsciLexerPO
+0000e520: 0103 0000 0014 004d 0061 0072 006b 0069  .......M.a.r.k.i
+0000e530: 0065 0072 0075 006e 0067 0800 0000 0006  .e.r.u.n.g......
+0000e540: 0000 0005 466c 6167 7307 0000 000b 5173  ....Flags.....Qs
+0000e550: 6369 4c65 7865 7250 4f01 0300 0000 2200  ciLexerPO.....".
+0000e560: 5500 6e00 7300 6300 6800 7200 6600 6d00  U.n.s.c.h.r.f.m.
+0000e570: 6100 7200 6b00 6900 6500 7200 7500 6e00  a.r.k.i.e.r.u.n.
+0000e580: 6708 0000 0000 0600 0000 0a46 757a 7a79  g..........Fuzzy
+0000e590: 2066 6c61 6707 0000 000b 5173 6369 4c65   flag.....QsciLe
+0000e5a0: 7865 7250 4f01 0300 0000 1e00 4d00 6500  xerPO.......M.e.
+0000e5b0: 6c00 6400 7500 6e00 6700 7300 6b00 6f00  l.d.u.n.g.s.k.o.
+0000e5c0: 6e00 7400 6500 7800 7408 0000 0000 0600  n.t.e.x.t.......
+0000e5d0: 0000 0f4d 6573 7361 6765 2063 6f6e 7465  ...Message conte
+0000e5e0: 7874 0700 0000 0b51 7363 694c 6578 6572  xt.....QsciLexer
+0000e5f0: 504f 0103 0000 0026 004d 0065 006c 0064  PO.....&.M.e.l.d
+0000e600: 0075 006e 0067 0073 006b 006f 006e 0074  .u.n.g.s.k.o.n.t
+0000e610: 0065 0078 0074 0074 0065 0078 0074 0800  .e.x.t.t.e.x.t..
+0000e620: 0000 0006 0000 0014 4d65 7373 6167 6520  ........Message 
+0000e630: 636f 6e74 6578 7420 7465 7874 0700 0000  context text....
+0000e640: 0b51 7363 694c 6578 6572 504f 0103 0000  .QsciLexerPO....
+0000e650: 003c 004d 0065 006c 0064 0075 006e 0067  .<.M.e.l.d.u.n.g
+0000e660: 0073 006b 006f 006e 0074 0065 0078 0074  .s.k.o.n.t.e.x.t
+0000e670: 0074 0065 0078 0074 0020 005a 0065 0069  .t.e.x.t. .Z.e.i
+0000e680: 006c 0065 006e 0065 006e 0064 0065 0800  .l.e.n.e.n.d.e..
+0000e690: 0000 0006 0000 0020 4d65 7373 6167 6520  ....... Message 
+0000e6a0: 636f 6e74 6578 7420 7465 7874 2065 6e64  context text end
+0000e6b0: 2d6f 662d 6c69 6e65 0700 0000 0b51 7363  -of-line.....Qsc
+0000e6c0: 694c 6578 6572 504f 0103 0000 0024 004d  iLexerPO.....$.M
+0000e6d0: 0065 006c 0064 0075 006e 0067 0073 0062  .e.l.d.u.n.g.s.b
+0000e6e0: 0065 007a 0065 0069 0063 0068 006e 0065  .e.z.e.i.c.h.n.e
+0000e6f0: 0072 0800 0000 0006 0000 0012 4d65 7373  .r..........Mess
+0000e700: 6167 6520 6964 656e 7469 6669 6572 0700  age identifier..
+0000e710: 0000 0b51 7363 694c 6578 6572 504f 0103  ...QsciLexerPO..
+0000e720: 0000 002c 004d 0065 006c 0064 0075 006e  ...,.M.e.l.d.u.n
+0000e730: 0067 0073 0062 0065 007a 0065 0069 0063  .g.s.b.e.z.e.i.c
+0000e740: 0068 006e 0065 0072 0074 0065 0078 0074  .h.n.e.r.t.e.x.t
+0000e750: 0800 0000 0006 0000 0017 4d65 7373 6167  ..........Messag
+0000e760: 6520 6964 656e 7469 6669 6572 2074 6578  e identifier tex
+0000e770: 7407 0000 000b 5173 6369 4c65 7865 7250  t.....QsciLexerP
+0000e780: 4f01 0300 0000 4200 4d00 6500 6c00 6400  O.....B.M.e.l.d.
+0000e790: 7500 6e00 6700 7300 6200 6500 7a00 6500  u.n.g.s.b.e.z.e.
+0000e7a0: 6900 6300 6800 6e00 6500 7200 7400 6500  i.c.h.n.e.r.t.e.
+0000e7b0: 7800 7400 2000 5a00 6500 6900 6c00 6500  x.t. .Z.e.i.l.e.
+0000e7c0: 6e00 6500 6e00 6400 6508 0000 0000 0600  n.e.n.d.e.......
+0000e7d0: 0000 234d 6573 7361 6765 2069 6465 6e74  ..#Message ident
+0000e7e0: 6966 6965 7220 7465 7874 2065 6e64 2d6f  ifier text end-o
+0000e7f0: 662d 6c69 6e65 0700 0000 0b51 7363 694c  f-line.....QsciL
+0000e800: 6578 6572 504f 0103 0000 0028 004d 0065  exerPO.....(.M.e
+0000e810: 006c 0064 0075 006e 0067 0073 007a 0065  .l.d.u.n.g.s.z.e
+0000e820: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+0000e830: 0074 0065 0800 0000 0006 0000 000e 4d65  .t.e..........Me
+0000e840: 7373 6167 6520 7374 7269 6e67 0700 0000  ssage string....
+0000e850: 0b51 7363 694c 6578 6572 504f 0103 0000  .QsciLexerPO....
+0000e860: 0032 004d 0065 006c 0064 0075 006e 0067  .2.M.e.l.d.u.n.g
+0000e870: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
+0000e880: 006b 0065 0074 0074 0065 006e 0074 0065  .k.e.t.t.e.n.t.e
+0000e890: 0078 0074 0800 0000 0006 0000 0013 4d65  .x.t..........Me
+0000e8a0: 7373 6167 6520 7374 7269 6e67 2074 6578  ssage string tex
+0000e8b0: 7407 0000 000b 5173 6369 4c65 7865 7250  t.....QsciLexerP
+0000e8c0: 4f01 0300 0000 4800 4d00 6500 6c00 6400  O.....H.M.e.l.d.
+0000e8d0: 7500 6e00 6700 7300 7a00 6500 6900 6300  u.n.g.s.z.e.i.c.
+0000e8e0: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
+0000e8f0: 6e00 7400 6500 7800 7400 2000 5a00 6500  n.t.e.x.t. .Z.e.
+0000e900: 6900 6c00 6500 6e00 6500 6e00 6400 6508  i.l.e.n.e.n.d.e.
+0000e910: 0000 0000 0600 0000 1f4d 6573 7361 6765  .........Message
+0000e920: 2073 7472 696e 6720 7465 7874 2065 6e64   string text end
+0000e930: 2d6f 662d 6c69 6e65 0700 0000 0b51 7363  -of-line.....Qsc
+0000e940: 694c 6578 6572 504f 0103 0000 002c 0050  iLexerPO.....,.P
+0000e950: 0072 006f 0067 0072 0061 006d 006d 0069  .r.o.g.r.a.m.m.i
+0000e960: 0065 0072 0065 0072 006b 006f 006d 006d  .e.r.e.r.k.o.m.m
+0000e970: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+0000e980: 0000 0012 5072 6f67 7261 6d6d 6572 2063  ....Programmer c
+0000e990: 6f6d 6d65 6e74 0700 0000 0b51 7363 694c  omment.....QsciL
+0000e9a0: 6578 6572 504f 0103 0000 0010 0052 0065  exerPO.......R.e
+0000e9b0: 0066 0065 0072 0065 006e 007a 0800 0000  .f.e.r.e.n.z....
+0000e9c0: 0006 0000 0009 5265 6665 7265 6e63 6507  ......Reference.
+0000e9d0: 0000 000b 5173 6369 4c65 7865 7250 4f01  ....QsciLexerPO.
+0000e9e0: 0300 0000 2600 5500 6e00 6700 fc00 6c00  ....&.U.n.g...l.
+0000e9f0: 7400 6900 6700 6500 2000 4400 6900 7200  t.i.g.e. .D.i.r.
+0000ea00: 6500 6b00 7400 6900 7600 6508 0000 0000  e.k.t.i.v.e.....
+0000ea10: 0600 0000 0d42 6164 2064 6972 6563 7469  .....Bad directi
+0000ea20: 7665 0700 0000 0c51 7363 694c 6578 6572  ve.....QsciLexer
+0000ea30: 504f 5601 0300 0000 1200 4b00 6f00 6d00  POV.......K.o.m.
+0000ea40: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+0000ea50: 0600 0000 0743 6f6d 6d65 6e74 0700 0000  .....Comment....
+0000ea60: 0c51 7363 694c 6578 6572 504f 5601 0300  .QsciLexerPOV...
+0000ea70: 0000 1c00 4b00 6f00 6d00 6d00 6500 6e00  ....K.o.m.m.e.n.
+0000ea80: 7400 6100 7200 7a00 6500 6900 6c00 6508  t.a.r.z.e.i.l.e.
+0000ea90: 0000 0000 0600 0000 0c43 6f6d 6d65 6e74  .........Comment
+0000eaa0: 206c 696e 6507 0000 000c 5173 6369 4c65   line.....QsciLe
+0000eab0: 7865 7250 4f56 0103 0000 0010 0053 0074  xerPOV.......S.t
+0000eac0: 0061 006e 0064 0061 0072 0064 0800 0000  .a.n.d.a.r.d....
+0000ead0: 0006 0000 0007 4465 6661 756c 7407 0000  ......Default...
+0000eae0: 000c 5173 6369 4c65 7865 7250 4f56 0103  ..QsciLexerPOV..
+0000eaf0: 0000 0012 0044 0069 0072 0065 006b 0074  .....D.i.r.e.k.t
+0000eb00: 0069 0076 0065 0800 0000 0006 0000 0009  .i.v.e..........
+0000eb10: 4469 7265 6374 6976 6507 0000 000c 5173  Directive.....Qs
+0000eb20: 6369 4c65 7865 7250 4f56 0103 0000 0014  ciLexerPOV......
+0000eb30: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
+0000eb40: 0065 0072 0800 0000 0006 0000 000a 4964  .e.r..........Id
+0000eb50: 656e 7469 6669 6572 0700 0000 0c51 7363  entifier.....Qsc
+0000eb60: 694c 6578 6572 504f 5601 0300 0000 0800  iLexerPOV.......
+0000eb70: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
+0000eb80: 064e 756d 6265 7207 0000 000c 5173 6369  .Number.....Qsci
+0000eb90: 4c65 7865 7250 4f56 0103 0000 0038 004f  LexerPOV.....8.O
+0000eba0: 0062 006a 0065 006b 0074 0065 002c 0020  .b.j.e.k.t.e.,. 
+0000ebb0: 0043 0053 0047 0020 0075 006e 0064 0020  .C.S.G. .u.n.d. 
+0000ebc0: 0045 0072 0073 0063 0068 0065 0069 006e  .E.r.s.c.h.e.i.n
+0000ebd0: 0075 006e 0067 0800 0000 0006 0000 001b  .u.n.g..........
+0000ebe0: 4f62 6a65 6374 732c 2043 5347 2061 6e64  Objects, CSG and
+0000ebf0: 2061 7070 6561 7261 6e63 6507 0000 000c   appearance.....
+0000ec00: 5173 6369 4c65 7865 7250 4f56 0103 0000  QsciLexerPOV....
+0000ec10: 0010 004f 0070 0065 0072 0061 0074 006f  ...O.p.e.r.a.t.o
+0000ec20: 0072 0800 0000 0006 0000 0008 4f70 6572  .r..........Oper
+0000ec30: 6174 6f72 0700 0000 0c51 7363 694c 6578  ator.....QsciLex
+0000ec40: 6572 504f 5601 0300 0000 2c00 5600 6f00  erPOV.....,.V.o.
+0000ec50: 7200 6400 6500 6600 6900 6e00 6900 6500  r.d.e.f.i.n.i.e.
+0000ec60: 7200 7400 6500 2000 4600 7500 6e00 6b00  r.t.e. .F.u.n.k.
+0000ec70: 7400 6900 6f00 6e08 0000 0000 0600 0000  t.i.o.n.........
+0000ec80: 1450 7265 6465 6669 6e65 6420 6675 6e63  .Predefined func
+0000ec90: 7469 6f6e 7307 0000 000c 5173 6369 4c65  tions.....QsciLe
+0000eca0: 7865 7250 4f56 0103 0000 0032 0056 006f  xerPOV.....2.V.o
+0000ecb0: 0072 0064 0065 0066 0069 006e 0069 0065  .r.d.e.f.i.n.i.e
+0000ecc0: 0072 0074 0065 0072 0020 0042 0065 007a  .r.t.e.r. .B.e.z
+0000ecd0: 0065 0069 0063 0068 006e 0065 0072 0800  .e.i.c.h.n.e.r..
+0000ece0: 0000 0006 0000 0016 5072 6564 6566 696e  ........Predefin
+0000ecf0: 6564 2069 6465 6e74 6966 6965 7273 0700  ed identifiers..
+0000ed00: 0000 0c51 7363 694c 6578 6572 504f 5601  ...QsciLexerPOV.
+0000ed10: 0300 0000 1800 5a00 6500 6900 6300 6800  ......Z.e.i.c.h.
+0000ed20: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
+0000ed30: 0000 0600 0000 0653 7472 696e 6707 0000  .......String...
+0000ed40: 000c 5173 6369 4c65 7865 7250 4f56 0103  ..QsciLexerPOV..
+0000ed50: 0000 003a 0054 0079 0070 0065 006e 002c  ...:.T.y.p.e.n.,
+0000ed60: 0020 004d 006f 0064 0069 0066 0069 007a  . .M.o.d.i.f.i.z
+0000ed70: 0069 0065 0072 0065 0072 0020 0075 006e  .i.e.r.e.r. .u.n
+0000ed80: 0064 0020 0049 0074 0065 006d 0073 0800  .d. .I.t.e.m.s..
+0000ed90: 0000 0006 0000 001a 5479 7065 732c 206d  ........Types, m
+0000eda0: 6f64 6966 6965 7273 2061 6e64 2069 7465  odifiers and ite
+0000edb0: 6d73 0700 0000 0c51 7363 694c 6578 6572  ms.....QsciLexer
+0000edc0: 504f 5601 0300 0000 2e00 5500 6e00 6200  POV.......U.n.b.
+0000edd0: 6500 6500 6e00 6400 6500 7400 6500 2000  e.e.n.d.e.t.e. .
+0000ede0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+0000edf0: 6500 7400 7400 6508 0000 0000 0600 0000  e.t.t.e.........
+0000ee00: 0f55 6e63 6c6f 7365 6420 7374 7269 6e67  .Unclosed string
+0000ee10: 0700 0000 0c51 7363 694c 6578 6572 504f  .....QsciLexerPO
+0000ee20: 5601 0300 0000 2400 4e00 7500 7400 7a00  V.....$.N.u.t.z.
+0000ee30: 6500 7200 2000 6400 6500 6600 6900 6e00  e.r. .d.e.f.i.n.
+0000ee40: 6900 6500 7200 7400 2000 3108 0000 0000  i.e.r.t. .1.....
+0000ee50: 0600 0000 0e55 7365 7220 6465 6669 6e65  .....User define
+0000ee60: 6420 3107 0000 000c 5173 6369 4c65 7865  d 1.....QsciLexe
+0000ee70: 7250 4f56 0103 0000 0024 004e 0075 0074  rPOV.....$.N.u.t
+0000ee80: 007a 0065 0072 0020 0064 0065 0066 0069  .z.e.r. .d.e.f.i
+0000ee90: 006e 0069 0065 0072 0074 0020 0032 0800  .n.i.e.r.t. .2..
+0000eea0: 0000 0006 0000 000e 5573 6572 2064 6566  ........User def
+0000eeb0: 696e 6564 2032 0700 0000 0c51 7363 694c  ined 2.....QsciL
+0000eec0: 6578 6572 504f 5601 0300 0000 2400 4e00  exerPOV.....$.N.
+0000eed0: 7500 7400 7a00 6500 7200 2000 6400 6500  u.t.z.e.r. .d.e.
+0000eee0: 6600 6900 6e00 6900 6500 7200 7400 2000  f.i.n.i.e.r.t. .
+0000eef0: 3308 0000 0000 0600 0000 0e55 7365 7220  3..........User 
+0000ef00: 6465 6669 6e65 6420 3307 0000 000c 5173  defined 3.....Qs
+0000ef10: 6369 4c65 7865 7250 4f56 0103 0000 002a  ciLexerPOV.....*
+0000ef20: 0027 0028 002a 0020 002e 002e 002e 0020  .'.(.*. ....... 
+0000ef30: 002a 0029 0027 0020 004b 006f 006d 006d  .*.).'. .K.o.m.m
+0000ef40: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+0000ef50: 0000 0019 2728 2a20 2e2e 2e20 2a29 2720  ....'(* ... *)' 
+0000ef60: 7374 796c 6520 636f 6d6d 656e 7407 0000  style comment...
+0000ef70: 000f 5173 6369 4c65 7865 7250 6173 6361  ..QsciLexerPasca
+0000ef80: 6c01 0300 0000 3c00 2700 2800 2a00 2400  l.....<.'.(.*.$.
+0000ef90: 2000 2e00 2e00 2e00 2000 2a00 2900 2700   ....... .*.).'.
+0000efa0: 2000 5000 7200 e400 7000 7200 6f00 7a00   .P.r...p.r.o.z.
+0000efb0: 6500 7300 7300 6f00 7200 6200 6c00 6f00  e.s.s.o.r.b.l.o.
+0000efc0: 6300 6b08 0000 0000 0600 0000 2627 282a  c.k.........&'(*
+0000efd0: 2420 2e2e 2e20 2a29 2720 7374 796c 6520  $ ... *)' style 
+0000efe0: 7072 652d 7072 6f63 6573 736f 7220 626c  pre-processor bl
+0000eff0: 6f63 6b07 0000 000f 5173 6369 4c65 7865  ock.....QsciLexe
+0000f000: 7250 6173 6361 6c01 0300 0000 2600 2700  rPascal.....&.'.
+0000f010: 7b00 2000 2e00 2e00 2e00 2000 7d00 2700  {. ....... .}.'.
+0000f020: 2000 4b00 6f00 6d00 6d00 6500 6e00 7400   .K.o.m.m.e.n.t.
+0000f030: 6100 7208 0000 0000 0600 0000 1727 7b20  a.r..........'{ 
+0000f040: 2e2e 2e20 7d27 2073 7479 6c65 2063 6f6d  ... }' style com
+0000f050: 6d65 6e74 0700 0000 0f51 7363 694c 6578  ment.....QsciLex
+0000f060: 6572 5061 7363 616c 0103 0000 0038 0027  erPascal.....8.'
+0000f070: 007b 0024 0020 002e 002e 002e 0020 007d  .{.$. ....... .}
+0000f080: 0027 0020 0050 0072 00e4 0070 0072 006f  .'. .P.r...p.r.o
+0000f090: 007a 0065 0073 0073 006f 0072 0062 006c  .z.e.s.s.o.r.b.l
+0000f0a0: 006f 0063 006b 0800 0000 0006 0000 0024  .o.c.k.........$
+0000f0b0: 277b 2420 2e2e 2e20 7d27 2073 7479 6c65  '{$ ... }' style
+0000f0c0: 2070 7265 2d70 726f 6365 7373 6f72 2062   pre-processor b
+0000f0d0: 6c6f 636b 0700 0000 0f51 7363 694c 6578  lock.....QsciLex
+0000f0e0: 6572 5061 7363 616c 0103 0000 000e 005a  erPascal.......Z
+0000f0f0: 0065 0069 0063 0068 0065 006e 0800 0000  .e.i.c.h.e.n....
+0000f100: 0006 0000 0009 4368 6172 6163 7465 7207  ......Character.
+0000f110: 0000 000f 5173 6369 4c65 7865 7250 6173  ....QsciLexerPas
+0000f120: 6361 6c01 0300 0000 1000 5300 7400 6100  cal.......S.t.a.
+0000f130: 6e00 6400 6100 7200 6408 0000 0000 0600  n.d.a.r.d.......
+0000f140: 0000 0744 6566 6175 6c74 0700 0000 0f51  ...Default.....Q
+0000f150: 7363 694c 6578 6572 5061 7363 616c 0103  sciLexerPascal..
+0000f160: 0000 0022 0048 0065 0078 0061 0064 0065  ...".H.e.x.a.d.e
+0000f170: 007a 0069 006d 0061 006c 0065 0020 005a  .z.i.m.a.l.e. .Z
+0000f180: 0061 0068 006c 0800 0000 0006 0000 0012  .a.h.l..........
+0000f190: 4865 7861 6465 6369 6d61 6c20 6e75 6d62  Hexadecimal numb
+0000f1a0: 6572 0700 0000 0f51 7363 694c 6578 6572  er.....QsciLexer
+0000f1b0: 5061 7363 616c 0103 0000 0014 0042 0065  Pascal.......B.e
+0000f1c0: 007a 0065 0069 0063 0068 006e 0065 0072  .z.e.i.c.h.n.e.r
+0000f1d0: 0800 0000 0006 0000 000a 4964 656e 7469  ..........Identi
+0000f1e0: 6669 6572 0700 0000 0f51 7363 694c 6578  fier.....QsciLex
+0000f1f0: 6572 5061 7363 616c 0103 0000 0020 0049  erPascal..... .I
+0000f200: 006e 006c 0069 006e 0065 0020 0041 0073  .n.l.i.n.e. .A.s
+0000f210: 0073 0065 006d 0062 006c 0065 0072 0800  .s.e.m.b.l.e.r..
+0000f220: 0000 0006 0000 000a 496e 6c69 6e65 2061  ........Inline a
+0000f230: 736d 0700 0000 0f51 7363 694c 6578 6572  sm.....QsciLexer
+0000f240: 5061 7363 616c 0103 0000 001a 0053 0063  Pascal.......S.c
+0000f250: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
+0000f260: 006f 0072 0074 0800 0000 0006 0000 0007  .o.r.t..........
+0000f270: 4b65 7977 6f72 6407 0000 000f 5173 6369  Keyword.....Qsci
+0000f280: 4c65 7865 7250 6173 6361 6c01 0300 0000  LexerPascal.....
+0000f290: 1e00 5a00 6500 6900 6c00 6500 6e00 6b00  ..Z.e.i.l.e.n.k.
+0000f2a0: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
+0000f2b0: 0000 0000 0600 0000 0c4c 696e 6520 636f  .........Line co
+0000f2c0: 6d6d 656e 7407 0000 000f 5173 6369 4c65  mment.....QsciLe
+0000f2d0: 7865 7250 6173 6361 6c01 0300 0000 0800  xerPascal.......
+0000f2e0: 5a00 6100 6800 6c08 0000 0000 0600 0000  Z.a.h.l.........
+0000f2f0: 064e 756d 6265 7207 0000 000f 5173 6369  .Number.....Qsci
+0000f300: 4c65 7865 7250 6173 6361 6c01 0300 0000  LexerPascal.....
+0000f310: 1000 4f00 7000 6500 7200 6100 7400 6f00  ..O.p.e.r.a.t.o.
+0000f320: 7208 0000 0000 0600 0000 084f 7065 7261  r..........Opera
+0000f330: 746f 7207 0000 000f 5173 6369 4c65 7865  tor.....QsciLexe
+0000f340: 7250 6173 6361 6c01 0300 0000 3600 5a00  rPascal.....6.Z.
+0000f350: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+0000f360: 7400 7400 6500 2000 6900 6e00 2000 4800  t.t.e. .i.n. .H.
+0000f370: 6f00 6300 6800 6b00 6f00 6d00 6d00 6100  o.c.h.k.o.m.m.a.
+0000f380: 7400 6108 0000 0000 0600 0000 1453 696e  t.a..........Sin
+0000f390: 676c 652d 7175 6f74 6564 2073 7472 696e  gle-quoted strin
+0000f3a0: 6707 0000 000f 5173 6369 4c65 7865 7250  g.....QsciLexerP
+0000f3b0: 6173 6361 6c01 0300 0000 2e00 5500 6e00  ascal.......U.n.
+0000f3c0: 6200 6500 6500 6e00 6400 6500 7400 6500  b.e.e.n.d.e.t.e.
+0000f3d0: 2000 5a00 6500 6900 6300 6800 6500 6e00   .Z.e.i.c.h.e.n.
+0000f3e0: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
+0000f3f0: 0000 0f55 6e63 6c6f 7365 6420 7374 7269  ...Unclosed stri
+0000f400: 6e67 0700 0000 0f51 7363 694c 6578 6572  ng.....QsciLexer
+0000f410: 5061 7363 616c 0103 0000 0008 0046 0065  Pascal.......F.e
+0000f420: 006c 0064 0800 0000 0006 0000 0005 4172  .l.d..........Ar
+0000f430: 7261 7907 0000 000d 5173 6369 4c65 7865  ray.....QsciLexe
+0000f440: 7250 6572 6c01 0300 0000 3400 4800 6500  rPerl.....4.H.e.
+0000f450: 7200 6500 2000 4400 6f00 6b00 7500 6d00  r.e. .D.o.k.u.m.
+0000f460: 6500 6e00 7400 2000 6900 6e00 2000 4200  e.n.t. .i.n. .B.
+0000f470: 6100 6300 6b00 7400 6900 6300 6b00 7308  a.c.k.t.i.c.k.s.
+0000f480: 0000 0000 0600 0000 1642 6163 6b74 6963  .........Backtic
+0000f490: 6b20 6865 7265 2064 6f63 756d 656e 7407  k here document.
+0000f4a0: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
+0000f4b0: 6c01 0300 0000 6600 4800 6500 7200 6500  l.....f.H.e.r.e.
+0000f4c0: 2000 4400 6f00 6b00 7500 6d00 6500 6e00   .D.o.k.u.m.e.n.
+0000f4d0: 7400 2000 6900 6e00 2000 4200 6100 6300  t. .i.n. .B.a.c.
+0000f4e0: 6b00 7400 6900 6300 6b00 7300 2000 2800  k.t.i.c.k.s. .(.
+0000f4f0: 6900 6e00 7400 6500 7200 7000 6f00 6c00  i.n.t.e.r.p.o.l.
+0000f500: 6900 6500 7200 7400 6500 2000 5600 6100  i.e.r.t.e. .V.a.
+0000f510: 7200 6900 6100 6200 6c00 6500 2908 0000  r.i.a.b.l.e.)...
+0000f520: 0000 0600 0000 2e42 6163 6b74 6963 6b20  .......Backtick 
+0000f530: 6865 7265 2064 6f63 756d 656e 7420 2869  here document (i
+0000f540: 6e74 6572 706f 6c61 7465 6420 7661 7269  nterpolated vari
+0000f550: 6162 6c65 2907 0000 000d 5173 6369 4c65  able).....QsciLe
+0000f560: 7865 7250 6572 6c01 0300 0000 1200 4200  xerPerl.......B.
+0000f570: 6100 6300 6b00 7400 6900 6300 6b00 7308  a.c.k.t.i.c.k.s.
+0000f580: 0000 0000 0600 0000 0942 6163 6b74 6963  .........Backtic
+0000f590: 6b73 0700 0000 0d51 7363 694c 6578 6572  ks.....QsciLexer
+0000f5a0: 5065 726c 0103 0000 0044 0042 0061 0063  Perl.....D.B.a.c
+0000f5b0: 006b 0074 0069 0063 006b 0073 0020 0028  .k.t.i.c.k.s. .(
+0000f5c0: 0069 006e 0074 0065 0072 0070 006f 006c  .i.n.t.e.r.p.o.l
+0000f5d0: 0069 0065 0072 0074 0065 0020 0056 0061  .i.e.r.t.e. .V.a
+0000f5e0: 0072 0069 0061 0062 006c 0065 0029 0800  .r.i.a.b.l.e.)..
+0000f5f0: 0000 0006 0000 0021 4261 636b 7469 636b  .......!Backtick
+0000f600: 7320 2869 6e74 6572 706f 6c61 7465 6420  s (interpolated 
+0000f610: 7661 7269 6162 6c65 2907 0000 000d 5173  variable).....Qs
+0000f620: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
+0000f630: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
+0000f640: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
+0000f650: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
+0000f660: 6572 5065 726c 0103 0000 0018 0044 0061  erPerl.......D.a
+0000f670: 0074 0065 006e 0073 0065 006b 0074 0069  .t.e.n.s.e.k.t.i
+0000f680: 006f 006e 0800 0000 0006 0000 000c 4461  .o.n..........Da
+0000f690: 7461 2073 6563 7469 6f6e 0700 0000 0d51  ta section.....Q
+0000f6a0: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
+0000f6b0: 0010 0053 0074 0061 006e 0064 0061 0072  ...S.t.a.n.d.a.r
+0000f6c0: 0064 0800 0000 0006 0000 0007 4465 6661  .d..........Defa
+0000f6d0: 756c 7407 0000 000d 5173 6369 4c65 7865  ult.....QsciLexe
+0000f6e0: 7250 6572 6c01 0300 0000 4400 4800 6500  rPerl.....D.H.e.
+0000f6f0: 7200 6500 2000 4400 6f00 6b00 7500 6d00  r.e. .D.o.k.u.m.
+0000f700: 6500 6e00 7400 2000 6900 6e00 2000 4100  e.n.t. .i.n. .A.
+0000f710: 6e00 6600 fc00 6800 7200 7500 6e00 6700  n.f...h.r.u.n.g.
+0000f720: 7300 7a00 6500 6900 6300 6800 6500 6e08  s.z.e.i.c.h.e.n.
+0000f730: 0000 0000 0600 0000 1b44 6f75 626c 652d  .........Double-
+0000f740: 7175 6f74 6564 2068 6572 6520 646f 6375  quoted here docu
+0000f750: 6d65 6e74 0700 0000 0d51 7363 694c 6578  ment.....QsciLex
+0000f760: 6572 5065 726c 0103 0000 0076 0048 0065  erPerl.....v.H.e
+0000f770: 0072 0065 0020 0044 006f 006b 0075 006d  .r.e. .D.o.k.u.m
+0000f780: 0065 006e 0074 0020 0069 006e 0020 0041  .e.n.t. .i.n. .A
+0000f790: 006e 0066 00fc 0068 0072 0075 006e 0067  .n.f...h.r.u.n.g
+0000f7a0: 0073 007a 0065 0069 0063 0068 0065 006e  .s.z.e.i.c.h.e.n
+0000f7b0: 0020 0028 0069 006e 0074 0065 0072 0070  . .(.i.n.t.e.r.p
+0000f7c0: 006f 006c 0069 0065 0072 0074 0065 0020  .o.l.i.e.r.t.e. 
+0000f7d0: 0056 0061 0072 0069 0061 0062 006c 0065  .V.a.r.i.a.b.l.e
+0000f7e0: 0029 0800 0000 0006 0000 0033 446f 7562  .).........3Doub
+0000f7f0: 6c65 2d71 756f 7465 6420 6865 7265 2064  le-quoted here d
+0000f800: 6f63 756d 656e 7420 2869 6e74 6572 706f  ocument (interpo
+0000f810: 6c61 7465 6420 7661 7269 6162 6c65 2907  lated variable).
+0000f820: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
+0000f830: 6c01 0300 0000 4200 5a00 6500 6900 6300  l.....B.Z.e.i.c.
+0000f840: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
+0000f850: 2000 6900 6e00 2000 4100 6e00 6600 fc00   .i.n. .A.n.f...
+0000f860: 6800 7200 7500 6e00 6700 7300 7a00 6500  h.r.u.n.g.s.z.e.
+0000f870: 6900 6300 6800 6500 6e08 0000 0000 0600  i.c.h.e.n.......
+0000f880: 0000 1444 6f75 626c 652d 7175 6f74 6564  ...Double-quoted
+0000f890: 2073 7472 696e 6707 0000 000d 5173 6369   string.....Qsci
+0000f8a0: 4c65 7865 7250 6572 6c01 0300 0000 7400  LexerPerl.....t.
+0000f8b0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+0000f8c0: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
+0000f8d0: 4100 6e00 6600 fc00 6800 7200 7500 6e00  A.n.f...h.r.u.n.
+0000f8e0: 6700 7300 7a00 6500 6900 6300 6800 6500  g.s.z.e.i.c.h.e.
+0000f8f0: 6e00 2000 2800 6900 6e00 7400 6500 7200  n. .(.i.n.t.e.r.
+0000f900: 7000 6f00 6c00 6900 6500 7200 7400 6500  p.o.l.i.e.r.t.e.
+0000f910: 2000 5600 6100 7200 6900 6100 6200 6c00   .V.a.r.i.a.b.l.
+0000f920: 6500 2908 0000 0000 0600 0000 2c44 6f75  e.).........,Dou
+0000f930: 626c 652d 7175 6f74 6564 2073 7472 696e  ble-quoted strin
+0000f940: 6720 2869 6e74 6572 706f 6c61 7465 6420  g (interpolated 
+0000f950: 7661 7269 6162 6c65 2907 0000 000d 5173  variable).....Qs
+0000f960: 6369 4c65 7865 7250 6572 6c01 0300 0000  ciLexerPerl.....
+0000f970: 0c00 4600 6500 6800 6c00 6500 7208 0000  ..F.e.h.l.e.r...
+0000f980: 0000 0600 0000 0545 7272 6f72 0700 0000  .......Error....
+0000f990: 0d51 7363 694c 6578 6572 5065 726c 0103  .QsciLexerPerl..
+0000f9a0: 0000 0016 0046 006f 0072 006d 0061 0074  .....F.o.r.m.a.t
+0000f9b0: 007a 0077 0065 0069 0067 0800 0000 0006  .z.w.e.i.g......
+0000f9c0: 0000 000b 466f 726d 6174 2062 6f64 7907  ....Format body.
+0000f9d0: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
+0000f9e0: 6c01 0300 0000 2600 4600 6f00 7200 6d00  l.....&.F.o.r.m.
+0000f9f0: 6100 7400 6900 6400 6500 6e00 7400 6900  a.t.i.d.e.n.t.i.
+0000fa00: 6600 6900 6b00 6100 7400 6f00 7208 0000  f.i.k.a.t.o.r...
+0000fa10: 0000 0600 0000 1146 6f72 6d61 7420 6964  .......Format id
+0000fa20: 656e 7469 6669 6572 0700 0000 0d51 7363  entifier.....Qsc
+0000fa30: 694c 6578 6572 5065 726c 0103 0000 0008  iLexerPerl......
+0000fa40: 0048 0061 0073 0068 0800 0000 0006 0000  .H.a.s.h........
+0000fa50: 0004 4861 7368 0700 0000 0d51 7363 694c  ..Hash.....QsciL
+0000fa60: 6578 6572 5065 726c 0103 0000 002e 0048  exerPerl.......H
+0000fa70: 0065 0072 0065 0020 0044 006f 006b 0075  .e.r.e. .D.o.k.u
+0000fa80: 006d 0065 006e 0074 002d 0042 0065 0067  .m.e.n.t.-.B.e.g
+0000fa90: 0072 0065 006e 007a 0065 0072 0800 0000  .r.e.n.z.e.r....
+0000faa0: 0006 0000 0017 4865 7265 2064 6f63 756d  ......Here docum
+0000fab0: 656e 7420 6465 6c69 6d69 7465 7207 0000  ent delimiter...
+0000fac0: 000d 5173 6369 4c65 7865 7250 6572 6c01  ..QsciLexerPerl.
+0000fad0: 0300 0000 1400 4200 6500 7a00 6500 6900  ......B.e.z.e.i.
+0000fae0: 6300 6800 6e00 6500 7208 0000 0000 0600  c.h.n.e.r.......
+0000faf0: 0000 0a49 6465 6e74 6966 6965 7207 0000  ...Identifier...
+0000fb00: 000d 5173 6369 4c65 7865 7250 6572 6c01  ..QsciLexerPerl.
+0000fb10: 0300 0000 1a00 5300 6300 6800 6c00 fc00  ......S.c.h.l...
+0000fb20: 7300 7300 6500 6c00 7700 6f00 7200 7408  s.s.e.l.w.o.r.t.
+0000fb30: 0000 0000 0600 0000 074b 6579 776f 7264  .........Keyword
+0000fb40: 0700 0000 0d51 7363 694c 6578 6572 5065  .....QsciLexerPe
+0000fb50: 726c 0103 0000 0008 005a 0061 0068 006c  rl.......Z.a.h.l
+0000fb60: 0800 0000 0006 0000 0006 4e75 6d62 6572  ..........Number
+0000fb70: 0700 0000 0d51 7363 694c 6578 6572 5065  .....QsciLexerPe
+0000fb80: 726c 0103 0000 0010 004f 0070 0065 0072  rl.......O.p.e.r
+0000fb90: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+0000fba0: 0008 4f70 6572 6174 6f72 0700 0000 0d51  ..Operator.....Q
+0000fbb0: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
+0000fbc0: 0006 0050 004f 0044 0800 0000 0006 0000  ...P.O.D........
+0000fbd0: 0003 504f 4407 0000 000d 5173 6369 4c65  ..POD.....QsciLe
+0000fbe0: 7865 7250 6572 6c01 0300 0000 1800 5000  xerPerl.......P.
+0000fbf0: 4f00 4400 2000 7700 f600 7200 7400 6c00  O.D. .w...r.t.l.
+0000fc00: 6900 6300 6808 0000 0000 0600 0000 0c50  i.c.h..........P
+0000fc10: 4f44 2076 6572 6261 7469 6d07 0000 000d  OD verbatim.....
+0000fc20: 5173 6369 4c65 7865 7250 6572 6c01 0300  QsciLexerPerl...
+0000fc30: 0000 2000 5a00 6500 6900 6300 6800 6500  .. .Z.e.i.c.h.e.
+0000fc40: 6e00 6b00 6500 7400 7400 6500 2000 2800  n.k.e.t.t.e. .(.
+0000fc50: 7100 2908 0000 0000 0600 0000 1151 756f  q.)..........Quo
+0000fc60: 7465 6420 7374 7269 6e67 2028 7129 0700  ted string (q)..
+0000fc70: 0000 0d51 7363 694c 6578 6572 5065 726c  ...QsciLexerPerl
+0000fc80: 0103 0000 0022 005a 0065 0069 0063 0068  .....".Z.e.i.c.h
+0000fc90: 0065 006e 006b 0065 0074 0074 0065 0020  .e.n.k.e.t.t.e. 
+0000fca0: 0028 0071 0071 0029 0800 0000 0006 0000  .(.q.q.)........
+0000fcb0: 0012 5175 6f74 6564 2073 7472 696e 6720  ..Quoted string 
+0000fcc0: 2871 7129 0700 0000 0d51 7363 694c 6578  (qq).....QsciLex
+0000fcd0: 6572 5065 726c 0103 0000 0052 005a 0065  erPerl.....R.Z.e
+0000fce0: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+0000fcf0: 0074 0065 0020 0028 0071 0071 002c 0020  .t.e. .(.q.q.,. 
+0000fd00: 0069 006e 0074 0065 0072 0070 006f 006c  .i.n.t.e.r.p.o.l
+0000fd10: 0069 0065 0072 0074 0065 0020 0056 0061  .i.e.r.t.e. .V.a
+0000fd20: 0072 0069 0061 0062 006c 0065 0029 0800  .r.i.a.b.l.e.)..
+0000fd30: 0000 0006 0000 0029 5175 6f74 6564 2073  .......)Quoted s
+0000fd40: 7472 696e 6720 2871 712c 2069 6e74 6572  tring (qq, inter
+0000fd50: 706f 6c61 7465 6420 7661 7269 6162 6c65  polated variable
+0000fd60: 2907 0000 000d 5173 6369 4c65 7865 7250  ).....QsciLexerP
+0000fd70: 6572 6c01 0300 0000 2200 5a00 6500 6900  erl.....".Z.e.i.
+0000fd80: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
+0000fd90: 6500 2000 2800 7100 7200 2908 0000 0000  e. .(.q.r.).....
+0000fda0: 0600 0000 1251 756f 7465 6420 7374 7269  .....Quoted stri
+0000fdb0: 6e67 2028 7172 2907 0000 000d 5173 6369  ng (qr).....Qsci
+0000fdc0: 4c65 7865 7250 6572 6c01 0300 0000 5200  LexerPerl.....R.
+0000fdd0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+0000fde0: 6500 7400 7400 6500 2000 2800 7100 7200  e.t.t.e. .(.q.r.
+0000fdf0: 2c00 2000 6900 6e00 7400 6500 7200 7000  ,. .i.n.t.e.r.p.
+0000fe00: 6f00 6c00 6900 6500 7200 7400 6500 2000  o.l.i.e.r.t.e. .
+0000fe10: 5600 6100 7200 6900 6100 6200 6c00 6500  V.a.r.i.a.b.l.e.
+0000fe20: 2908 0000 0000 0600 0000 2951 756f 7465  ).........)Quote
+0000fe30: 6420 7374 7269 6e67 2028 7172 2c20 696e  d string (qr, in
+0000fe40: 7465 7270 6f6c 6174 6564 2076 6172 6961  terpolated varia
+0000fe50: 626c 6529 0700 0000 0d51 7363 694c 6578  ble).....QsciLex
+0000fe60: 6572 5065 726c 0103 0000 0022 005a 0065  erPerl.....".Z.e
+0000fe70: 0069 0063 0068 0065 006e 006b 0065 0074  .i.c.h.e.n.k.e.t
+0000fe80: 0074 0065 0020 0028 0071 0077 0029 0800  .t.e. .(.q.w.)..
+0000fe90: 0000 0006 0000 0012 5175 6f74 6564 2073  ........Quoted s
+0000fea0: 7472 696e 6720 2871 7729 0700 0000 0d51  tring (qw).....Q
+0000feb0: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
+0000fec0: 0022 005a 0065 0069 0063 0068 0065 006e  .".Z.e.i.c.h.e.n
+0000fed0: 006b 0065 0074 0074 0065 0020 0028 0071  .k.e.t.t.e. .(.q
+0000fee0: 0078 0029 0800 0000 0006 0000 0012 5175  .x.)..........Qu
+0000fef0: 6f74 6564 2073 7472 696e 6720 2871 7829  oted string (qx)
+0000ff00: 0700 0000 0d51 7363 694c 6578 6572 5065  .....QsciLexerPe
+0000ff10: 726c 0103 0000 0052 005a 0065 0069 0063  rl.....R.Z.e.i.c
+0000ff20: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
+0000ff30: 0020 0028 0071 0078 002c 0020 0069 006e  . .(.q.x.,. .i.n
+0000ff40: 0074 0065 0072 0070 006f 006c 0069 0065  .t.e.r.p.o.l.i.e
+0000ff50: 0072 0074 0065 0020 0056 0061 0072 0069  .r.t.e. .V.a.r.i
+0000ff60: 0061 0062 006c 0065 0029 0800 0000 0006  .a.b.l.e.)......
+0000ff70: 0000 0029 5175 6f74 6564 2073 7472 696e  ...)Quoted strin
+0000ff80: 6720 2871 782c 2069 6e74 6572 706f 6c61  g (qx, interpola
+0000ff90: 7465 6420 7661 7269 6162 6c65 2907 0000  ted variable)...
+0000ffa0: 000d 5173 6369 4c65 7865 7250 6572 6c01  ..QsciLexerPerl.
+0000ffb0: 0300 0000 2400 5200 6500 6700 7500 6c00  ....$.R.e.g.u.l.
+0000ffc0: e400 7200 6500 7200 2000 4100 7500 7300  ..r.e.r. .A.u.s.
+0000ffd0: 6400 7200 7500 6300 6b08 0000 0000 0600  d.r.u.c.k.......
+0000ffe0: 0000 1252 6567 756c 6172 2065 7870 7265  ...Regular expre
+0000fff0: 7373 696f 6e07 0000 000d 5173 6369 4c65  ssion.....QsciLe
+00010000: 7865 7250 6572 6c01 0300 0000 5600 5200  xerPerl.....V.R.
+00010010: 6500 6700 7500 6c00 e400 7200 6500 7200  e.g.u.l...r.e.r.
+00010020: 2000 4100 7500 7300 6400 7200 7500 6300   .A.u.s.d.r.u.c.
+00010030: 6b00 2000 2800 6900 6e00 7400 6500 7200  k. .(.i.n.t.e.r.
+00010040: 7000 6f00 6c00 6900 6500 7200 7400 6500  p.o.l.i.e.r.t.e.
+00010050: 2000 5600 6100 7200 6900 6100 6200 6c00   .V.a.r.i.a.b.l.
+00010060: 6500 2908 0000 0000 0600 0000 2a52 6567  e.).........*Reg
+00010070: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
+00010080: 2869 6e74 6572 706f 6c61 7465 6420 7661  (interpolated va
+00010090: 7269 6162 6c65 2907 0000 000d 5173 6369  riable).....Qsci
+000100a0: 4c65 7865 7250 6572 6c01 0300 0000 0c00  LexerPerl.......
+000100b0: 5300 6b00 6100 6c00 6100 7208 0000 0000  S.k.a.l.a.r.....
+000100c0: 0600 0000 0653 6361 6c61 7207 0000 000d  .....Scalar.....
+000100d0: 5173 6369 4c65 7865 7250 6572 6c01 0300  QsciLexerPerl...
+000100e0: 0000 3800 4800 6500 7200 6500 2000 4400  ..8.H.e.r.e. .D.
+000100f0: 6f00 6b00 7500 6d00 6500 6e00 7400 2000  o.k.u.m.e.n.t. .
+00010100: 6900 6e00 2000 4800 6f00 6300 6800 6b00  i.n. .H.o.c.h.k.
+00010110: 6f00 6d00 6d00 6100 7400 6108 0000 0000  o.m.m.a.t.a.....
+00010120: 0600 0000 1b53 696e 676c 652d 7175 6f74  .....Single-quot
+00010130: 6564 2068 6572 6520 646f 6375 6d65 6e74  ed here document
+00010140: 0700 0000 0d51 7363 694c 6578 6572 5065  .....QsciLexerPe
+00010150: 726c 0103 0000 0036 005a 0065 0069 0063  rl.....6.Z.e.i.c
+00010160: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
+00010170: 0020 0069 006e 0020 0048 006f 0063 0068  . .i.n. .H.o.c.h
+00010180: 006b 006f 006d 006d 0061 0074 0061 0800  .k.o.m.m.a.t.a..
+00010190: 0000 0006 0000 0014 5369 6e67 6c65 2d71  ........Single-q
+000101a0: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
+000101b0: 0d51 7363 694c 6578 6572 5065 726c 0103  .QsciLexerPerl..
+000101c0: 0000 0028 0053 0075 0062 0072 006f 0075  ...(.S.u.b.r.o.u
+000101d0: 0074 0069 006e 0065 006e 0020 0050 0072  .t.i.n.e.n. .P.r
+000101e0: 006f 0074 006f 0074 0079 0070 0800 0000  .o.t.o.t.y.p....
+000101f0: 0006 0000 0014 5375 6272 6f75 7469 6e65  ......Subroutine
+00010200: 2070 726f 746f 7479 7065 0700 0000 0d51   prototype.....Q
+00010210: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
+00010220: 0012 0045 0072 0073 0065 0074 007a 0075  ...E.r.s.e.t.z.u
+00010230: 006e 0067 0800 0000 0006 0000 000c 5375  .n.g..........Su
+00010240: 6273 7469 7475 7469 6f6e 0700 0000 0d51  bstitution.....Q
+00010250: 7363 694c 6578 6572 5065 726c 0103 0000  sciLexerPerl....
+00010260: 0044 0045 0072 0073 0065 0074 007a 0075  .D.E.r.s.e.t.z.u
+00010270: 006e 0067 0020 0028 0069 006e 0074 0065  .n.g. .(.i.n.t.e
+00010280: 0072 0070 006f 006c 0069 0065 0072 0074  .r.p.o.l.i.e.r.t
+00010290: 0065 0020 0056 0061 0072 0069 0061 0062  .e. .V.a.r.i.a.b
+000102a0: 006c 0065 0029 0800 0000 0006 0000 0024  .l.e.).........$
+000102b0: 5375 6273 7469 7475 7469 6f6e 2028 696e  Substitution (in
+000102c0: 7465 7270 6f6c 6174 6564 2076 6172 6961  terpolated varia
+000102d0: 626c 6529 0700 0000 0d51 7363 694c 6578  ble).....QsciLex
+000102e0: 6572 5065 726c 0103 0000 001a 0053 0079  erPerl.......S.y
+000102f0: 006d 0062 006f 006c 0074 0061 0062 0065  .m.b.o.l.t.a.b.e
+00010300: 006c 006c 0065 0800 0000 0006 0000 000c  .l.l.e..........
+00010310: 5379 6d62 6f6c 2074 6162 6c65 0700 0000  Symbol table....
+00010320: 0d51 7363 694c 6578 6572 5065 726c 0103  .QsciLexerPerl..
+00010330: 0000 0016 00dc 0062 0065 0072 0073 0065  .......b.e.r.s.e
+00010340: 0074 007a 0075 006e 0067 0800 0000 0006  .t.z.u.n.g......
+00010350: 0000 000b 5472 616e 736c 6174 696f 6e07  ....Translation.
+00010360: 0000 000d 5173 6369 4c65 7865 7250 6572  ....QsciLexerPer
+00010370: 6c01 0300 0000 1800 4600 6500 6c00 6400  l.......F.e.l.d.
+00010380: 6b00 6c00 6100 6d00 6d00 6500 7200 6e08  k.l.a.m.m.e.r.n.
+00010390: 0000 0000 0600 0000 1141 7272 6179 2070  .........Array p
+000103a0: 6172 656e 7468 6573 6973 0700 0000 1351  arenthesis.....Q
+000103b0: 7363 694c 6578 6572 506f 7374 5363 7269  sciLexerPostScri
+000103c0: 7074 0103 0000 0046 0055 006e 0067 00fc  pt.....F.U.n.g..
+000103d0: 006c 0074 0069 0067 0065 0073 0020 005a  .l.t.i.g.e.s. .Z
+000103e0: 0065 0069 0063 0068 0065 006e 0020 0066  .e.i.c.h.e.n. .f
+000103f0: 00fc 0072 0020 005a 0065 0069 0063 0068  ...r. .Z.e.i.c.h
+00010400: 0065 006e 006b 0065 0074 0074 0065 0800  .e.n.k.e.t.t.e..
+00010410: 0000 0006 0000 0014 4261 6420 7374 7269  ........Bad stri
+00010420: 6e67 2063 6861 7261 6374 6572 0700 0000  ng character....
+00010430: 1351 7363 694c 6578 6572 506f 7374 5363  .QsciLexerPostSc
+00010440: 7269 7074 0103 0000 0026 0042 0061 0073  ript.....&.B.a.s
+00010450: 0065 0038 0035 0020 005a 0065 0069 0063  .e.8.5. .Z.e.i.c
+00010460: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
+00010470: 0800 0000 0006 0000 000d 4261 7365 3835  ..........Base85
+00010480: 2073 7472 696e 6707 0000 0013 5173 6369   string.....Qsci
+00010490: 4c65 7865 7250 6f73 7453 6372 6970 7401  LexerPostScript.
+000104a0: 0300 0000 1200 4b00 6f00 6d00 6d00 6500  ......K.o.m.m.e.
+000104b0: 6e00 7400 6100 7208 0000 0000 0600 0000  n.t.a.r.........
+000104c0: 0743 6f6d 6d65 6e74 0700 0000 1351 7363  .Comment.....Qsc
+000104d0: 694c 6578 6572 506f 7374 5363 7269 7074  iLexerPostScript
+000104e0: 0103 0000 001a 0044 0053 0043 0020 004b  .......D.S.C. .K
+000104f0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
+00010500: 0800 0000 0006 0000 000b 4453 4320 636f  ..........DSC co
+00010510: 6d6d 656e 7407 0000 0013 5173 6369 4c65  mment.....QsciLe
+00010520: 7865 7250 6f73 7453 6372 6970 7401 0300  xerPostScript...
+00010530: 0000 2200 4400 5300 4300 2000 4b00 6f00  ..".D.S.C. .K.o.
+00010540: 6d00 6d00 6500 6e00 7400 6100 7200 7700  m.m.e.n.t.a.r.w.
+00010550: 6500 7200 7408 0000 0000 0600 0000 1144  e.r.t..........D
+00010560: 5343 2063 6f6d 6d65 6e74 2076 616c 7565  SC comment value
+00010570: 0700 0000 1351 7363 694c 6578 6572 506f  .....QsciLexerPo
+00010580: 7374 5363 7269 7074 0103 0000 0010 0053  stScript.......S
+00010590: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+000105a0: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
+000105b0: 0000 0013 5173 6369 4c65 7865 7250 6f73  ....QsciLexerPos
+000105c0: 7453 6372 6970 7401 0300 0000 2600 4400  tScript.....&.D.
+000105d0: 6900 6300 7400 6900 6f00 6e00 6100 7200  i.c.t.i.o.n.a.r.
+000105e0: 7900 2d00 4b00 6c00 6100 6d00 6d00 6500  y.-.K.l.a.m.m.e.
+000105f0: 7200 6e08 0000 0000 0600 0000 1644 6963  r.n..........Dic
+00010600: 7469 6f6e 6172 7920 7061 7265 6e74 6865  tionary parenthe
+00010610: 7369 7307 0000 0013 5173 6369 4c65 7865  sis.....QsciLexe
+00010620: 7250 6f73 7453 6372 6970 7401 0300 0000  rPostScript.....
+00010630: 3200 4800 6500 7800 6100 6400 6500 7a00  2.H.e.x.a.d.e.z.
+00010640: 6900 6d00 6100 6c00 6500 2000 5a00 6500  i.m.a.l.e. .Z.e.
+00010650: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
+00010660: 7400 6508 0000 0000 0600 0000 1248 6578  t.e..........Hex
+00010670: 6164 6563 696d 616c 2073 7472 696e 6707  adecimal string.
+00010680: 0000 0013 5173 6369 4c65 7865 7250 6f73  ....QsciLexerPos
+00010690: 7453 6372 6970 7401 0300 0000 3600 4400  tScript.....6.D.
+000106a0: 6900 7200 6500 6b00 7400 2000 6100 7500  i.r.e.k.t. .a.u.
+000106b0: 7300 6700 6500 6600 fc00 6800 7200 7400  s.g.e.f...h.r.t.
+000106c0: 6500 7300 2000 4c00 6900 7400 6500 7200  e.s. .L.i.t.e.r.
+000106d0: 6100 6c08 0000 0000 0600 0000 1d49 6d6d  a.l..........Imm
+000106e0: 6564 6961 7465 6c79 2065 7661 6c75 6174  ediately evaluat
+000106f0: 6564 206c 6974 6572 616c 0700 0000 1351  ed literal.....Q
+00010700: 7363 694c 6578 6572 506f 7374 5363 7269  sciLexerPostScri
+00010710: 7074 0103 0000 001a 0053 0063 0068 006c  pt.......S.c.h.l
+00010720: 00fc 0073 0073 0065 006c 0077 006f 0072  ...s.s.e.l.w.o.r
+00010730: 0074 0800 0000 0006 0000 0007 4b65 7977  .t..........Keyw
+00010740: 6f72 6407 0000 0013 5173 6369 4c65 7865  ord.....QsciLexe
+00010750: 7250 6f73 7453 6372 6970 7401 0300 0000  rPostScript.....
+00010760: 0e00 4c00 6900 7400 6500 7200 6100 6c08  ..L.i.t.e.r.a.l.
+00010770: 0000 0000 0600 0000 074c 6974 6572 616c  .........Literal
+00010780: 0700 0000 1351 7363 694c 6578 6572 506f  .....QsciLexerPo
+00010790: 7374 5363 7269 7074 0103 0000 0008 004e  stScript.......N
+000107a0: 0061 006d 0065 0800 0000 0006 0000 0004  .a.m.e..........
+000107b0: 4e61 6d65 0700 0000 1351 7363 694c 6578  Name.....QsciLex
+000107c0: 6572 506f 7374 5363 7269 7074 0103 0000  erPostScript....
+000107d0: 0008 005a 0061 0068 006c 0800 0000 0006  ...Z.a.h.l......
+000107e0: 0000 0006 4e75 6d62 6572 0700 0000 1351  ....Number.....Q
+000107f0: 7363 694c 6578 6572 506f 7374 5363 7269  sciLexerPostScri
+00010800: 7074 0103 0000 0020 0050 0072 006f 007a  pt..... .P.r.o.z
+00010810: 0065 0064 0075 0072 006b 006c 0061 006d  .e.d.u.r.k.l.a.m
+00010820: 006d 0065 0072 006e 0800 0000 0006 0000  .m.e.r.n........
+00010830: 0015 5072 6f63 6564 7572 6520 7061 7265  ..Procedure pare
+00010840: 6e74 6865 7369 7307 0000 0013 5173 6369  nthesis.....Qsci
+00010850: 4c65 7865 7250 6f73 7453 6372 6970 7401  LexerPostScript.
+00010860: 0300 0000 0800 5400 6500 7800 7408 0000  ......T.e.x.t...
+00010870: 0000 0600 0000 0454 6578 7407 0000 0013  .......Text.....
+00010880: 5173 6369 4c65 7865 7250 6f73 7453 6372  QsciLexerPostScr
+00010890: 6970 7401 0300 0000 1200 5a00 7500 7700  ipt.......Z.u.w.
+000108a0: 6500 6900 7300 7500 6e00 6708 0000 0000  e.i.s.u.n.g.....
+000108b0: 0600 0000 0a41 7373 6967 6e6d 656e 7407  .....Assignment.
+000108c0: 0000 0013 5173 6369 4c65 7865 7250 726f  ....QsciLexerPro
+000108d0: 7065 7274 6965 7301 0300 0000 1200 4b00  perties.......K.
+000108e0: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
+000108f0: 0000 0000 0600 0000 0743 6f6d 6d65 6e74  .........Comment
+00010900: 0700 0000 1351 7363 694c 6578 6572 5072  .....QsciLexerPr
+00010910: 6f70 6572 7469 6573 0103 0000 0010 0053  operties.......S
+00010920: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+00010930: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
+00010940: 0000 0013 5173 6369 4c65 7865 7250 726f  ....QsciLexerPro
+00010950: 7065 7274 6965 7301 0300 0000 1800 5300  perties.......S.
+00010960: 7400 6100 6e00 6400 6100 7200 6400 7700  t.a.n.d.a.r.d.w.
+00010970: 6500 7200 7408 0000 0000 0600 0000 0d44  e.r.t..........D
+00010980: 6566 6175 6c74 2076 616c 7565 0700 0000  efault value....
+00010990: 1351 7363 694c 6578 6572 5072 6f70 6572  .QsciLexerProper
+000109a0: 7469 6573 0103 0000 0012 0053 0063 0068  ties.......S.c.h
+000109b0: 006c 00fc 0073 0073 0065 006c 0800 0000  .l...s.s.e.l....
+000109c0: 0006 0000 0003 4b65 7907 0000 0013 5173  ......Key.....Qs
+000109d0: 6369 4c65 7865 7250 726f 7065 7274 6965  ciLexerPropertie
+000109e0: 7301 0300 0000 1200 4100 6200 7300 6300  s.......A.b.s.c.
+000109f0: 6800 6e00 6900 7400 7408 0000 0000 0600  h.n.i.t.t.......
+00010a00: 0000 0753 6563 7469 6f6e 0700 0000 1351  ...Section.....Q
+00010a10: 7363 694c 6578 6572 5072 6f70 6572 7469  sciLexerProperti
+00010a20: 6573 0103 0000 0016 004b 006c 0061 0073  es.......K.l.a.s
+00010a30: 0073 0065 006e 006e 0061 006d 0065 0800  .s.e.n.n.a.m.e..
+00010a40: 0000 0006 0000 000a 436c 6173 7320 6e61  ........Class na
+00010a50: 6d65 0700 0000 0f51 7363 694c 6578 6572  me.....QsciLexer
+00010a60: 5079 7468 6f6e 0103 0000 0012 004b 006f  Python.......K.o
+00010a70: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+00010a80: 0000 0006 0000 0007 436f 6d6d 656e 7407  ........Comment.
+00010a90: 0000 000f 5173 6369 4c65 7865 7250 7974  ....QsciLexerPyt
+00010aa0: 686f 6e01 0300 0000 1c00 4b00 6f00 6d00  hon.......K.o.m.
+00010ab0: 6d00 6500 6e00 7400 6100 7200 6200 6c00  m.e.n.t.a.r.b.l.
+00010ac0: 6f00 6300 6b08 0000 0000 0600 0000 0d43  o.c.k..........C
+00010ad0: 6f6d 6d65 6e74 2062 6c6f 636b 0700 0000  omment block....
+00010ae0: 0f51 7363 694c 6578 6572 5079 7468 6f6e  .QsciLexerPython
+00010af0: 0103 0000 0012 0044 0065 006b 006f 0072  .......D.e.k.o.r
+00010b00: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
+00010b10: 0009 4465 636f 7261 746f 7207 0000 000f  ..Decorator.....
+00010b20: 5173 6369 4c65 7865 7250 7974 686f 6e01  QsciLexerPython.
+00010b30: 0300 0000 1000 5300 7400 6100 6e00 6400  ......S.t.a.n.d.
+00010b40: 6100 7200 6408 0000 0000 0600 0000 0744  a.r.d..........D
+00010b50: 6566 6175 6c74 0700 0000 0f51 7363 694c  efault.....QsciL
+00010b60: 6578 6572 5079 7468 6f6e 0103 0000 0046  exerPython.....F
+00010b70: 0046 002d 005a 0065 0069 0063 0068 0065  .F.-.Z.e.i.c.h.e
+00010b80: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
+00010b90: 006e 0020 0041 006e 0066 00fc 0068 0072  .n. .A.n.f...h.r
+00010ba0: 0075 006e 0067 0073 007a 0065 0069 0063  .u.n.g.s.z.e.i.c
+00010bb0: 0068 0065 006e 0800 0000 0006 0000 0016  .h.e.n..........
+00010bc0: 446f 7562 6c65 2d71 756f 7465 6420 662d  Double-quoted f-
+00010bd0: 7374 7269 6e67 0700 0000 0f51 7363 694c  string.....QsciL
+00010be0: 6578 6572 5079 7468 6f6e 0103 0000 0042  exerPython.....B
+00010bf0: 005a 0065 0069 0063 0068 0065 006e 006b  .Z.e.i.c.h.e.n.k
+00010c00: 0065 0074 0074 0065 0020 0069 006e 0020  .e.t.t.e. .i.n. 
+00010c10: 0041 006e 0066 00fc 0068 0072 0075 006e  .A.n.f...h.r.u.n
+00010c20: 0067 0073 007a 0065 0069 0063 0068 0065  .g.s.z.e.i.c.h.e
+00010c30: 006e 0800 0000 0006 0000 0014 446f 7562  .n..........Doub
+00010c40: 6c65 2d71 756f 7465 6420 7374 7269 6e67  le-quoted string
+00010c50: 0700 0000 0f51 7363 694c 6578 6572 5079  .....QsciLexerPy
+00010c60: 7468 6f6e 0103 0000 0038 0046 0075 006e  thon.....8.F.u.n
+00010c70: 006b 0074 0069 006f 006e 0073 002d 0020  .k.t.i.o.n.s.-. 
+00010c80: 006f 0064 0065 0072 0020 004d 0065 0074  .o.d.e.r. .M.e.t
+00010c90: 0068 006f 0064 0065 006e 006e 0061 006d  .h.o.d.e.n.n.a.m
+00010ca0: 0065 0800 0000 0006 0000 0017 4675 6e63  .e..........Func
+00010cb0: 7469 6f6e 206f 7220 6d65 7468 6f64 206e  tion or method n
+00010cc0: 616d 6507 0000 000f 5173 6369 4c65 7865  ame.....QsciLexe
+00010cd0: 7250 7974 686f 6e01 0300 0000 3400 4800  rPython.....4.H.
+00010ce0: 6500 7200 7600 6f00 7200 6700 6500 6800  e.r.v.o.r.g.e.h.
+00010cf0: 6f00 6200 6500 6e00 6500 7200 2000 4200  o.b.e.n.e.r. .B.
+00010d00: 6500 7a00 6500 6900 6300 6800 6e00 6500  e.z.e.i.c.h.n.e.
+00010d10: 7208 0000 0000 0600 0000 1648 6967 686c  r..........Highl
+00010d20: 6967 6874 6564 2069 6465 6e74 6966 6965  ighted identifie
+00010d30: 7207 0000 000f 5173 6369 4c65 7865 7250  r.....QsciLexerP
+00010d40: 7974 686f 6e01 0300 0000 1400 4200 6500  ython.......B.e.
+00010d50: 7a00 6500 6900 6300 6800 6e00 6500 7208  z.e.i.c.h.n.e.r.
+00010d60: 0000 0000 0600 0000 0a49 6465 6e74 6966  .........Identif
+00010d70: 6965 7207 0000 000f 5173 6369 4c65 7865  ier.....QsciLexe
+00010d80: 7250 7974 686f 6e01 0300 0000 1a00 5300  rPython.......S.
+00010d90: 6300 6800 6c00 fc00 7300 7300 6500 6c00  c.h.l...s.s.e.l.
+00010da0: 7700 6f00 7200 7408 0000 0000 0600 0000  w.o.r.t.........
+00010db0: 074b 6579 776f 7264 0700 0000 0f51 7363  .Keyword.....Qsc
+00010dc0: 694c 6578 6572 5079 7468 6f6e 0103 0000  iLexerPython....
+00010dd0: 0008 005a 0061 0068 006c 0800 0000 0006  ...Z.a.h.l......
+00010de0: 0000 0006 4e75 6d62 6572 0700 0000 0f51  ....Number.....Q
+00010df0: 7363 694c 6578 6572 5079 7468 6f6e 0103  sciLexerPython..
+00010e00: 0000 0010 004f 0070 0065 0072 0061 0074  .....O.p.e.r.a.t
+00010e10: 006f 0072 0800 0000 0006 0000 0008 4f70  .o.r..........Op
+00010e20: 6572 6174 6f72 0700 0000 0f51 7363 694c  erator.....QsciL
+00010e30: 6578 6572 5079 7468 6f6e 0103 0000 003a  exerPython.....:
+00010e40: 0046 002d 005a 0065 0069 0063 0068 0065  .F.-.Z.e.i.c.h.e
+00010e50: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
+00010e60: 006e 0020 0048 006f 0063 0068 006b 006f  .n. .H.o.c.h.k.o
+00010e70: 006d 006d 0061 0074 0061 0800 0000 0006  .m.m.a.t.a......
+00010e80: 0000 0016 5369 6e67 6c65 2d71 756f 7465  ....Single-quote
+00010e90: 6420 662d 7374 7269 6e67 0700 0000 0f51  d f-string.....Q
+00010ea0: 7363 694c 6578 6572 5079 7468 6f6e 0103  sciLexerPython..
+00010eb0: 0000 0036 005a 0065 0069 0063 0068 0065  ...6.Z.e.i.c.h.e
+00010ec0: 006e 006b 0065 0074 0074 0065 0020 0069  .n.k.e.t.t.e. .i
+00010ed0: 006e 0020 0048 006f 0063 0068 006b 006f  .n. .H.o.c.h.k.o
+00010ee0: 006d 006d 0061 0074 0061 0800 0000 0006  .m.m.a.t.a......
+00010ef0: 0000 0014 5369 6e67 6c65 2d71 756f 7465  ....Single-quote
+00010f00: 6420 7374 7269 6e67 0700 0000 0f51 7363  d string.....Qsc
+00010f10: 694c 6578 6572 5079 7468 6f6e 0103 0000  iLexerPython....
+00010f20: 005c 0046 002d 005a 0065 0069 0063 0068  .\.F.-.Z.e.i.c.h
+00010f30: 0065 006e 006b 0065 0074 0074 0065 0020  .e.n.k.e.t.t.e. 
+00010f40: 0069 006e 0020 0064 0072 0065 0069 0066  .i.n. .d.r.e.i.f
+00010f50: 0061 0063 0068 0065 006e 0020 0041 006e  .a.c.h.e.n. .A.n
+00010f60: 0066 00fc 0068 0072 0075 006e 0067 0073  .f...h.r.u.n.g.s
+00010f70: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
+00010f80: 0000 0006 0000 001d 5472 6970 6c65 2064  ........Triple d
+00010f90: 6f75 626c 652d 7175 6f74 6564 2066 2d73  ouble-quoted f-s
+00010fa0: 7472 696e 6707 0000 000f 5173 6369 4c65  tring.....QsciLe
+00010fb0: 7865 7250 7974 686f 6e01 0300 0000 5800  xerPython.....X.
+00010fc0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+00010fd0: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
+00010fe0: 6400 7200 6500 6900 6600 6100 6300 6800  d.r.e.i.f.a.c.h.
+00010ff0: 6500 6e00 2000 4100 6e00 6600 fc00 6800  e.n. .A.n.f...h.
+00011000: 7200 7500 6e00 6700 7300 7a00 6500 6900  r.u.n.g.s.z.e.i.
+00011010: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+00011020: 1b54 7269 706c 6520 646f 7562 6c65 2d71  .Triple double-q
+00011030: 756f 7465 6420 7374 7269 6e67 0700 0000  uoted string....
+00011040: 0f51 7363 694c 6578 6572 5079 7468 6f6e  .QsciLexerPython
+00011050: 0103 0000 0050 0046 002d 005a 0065 0069  .....P.F.-.Z.e.i
+00011060: 0063 0068 0065 006e 006b 0065 0074 0074  .c.h.e.n.k.e.t.t
+00011070: 0065 0020 0069 006e 0020 0064 0072 0065  .e. .i.n. .d.r.e
+00011080: 0069 0066 0061 0063 0068 0065 006e 0020  .i.f.a.c.h.e.n. 
+00011090: 0048 006f 0063 0068 006b 006f 006d 006d  .H.o.c.h.k.o.m.m
+000110a0: 0061 0074 0061 0800 0000 0006 0000 001d  .a.t.a..........
+000110b0: 5472 6970 6c65 2073 696e 676c 652d 7175  Triple single-qu
+000110c0: 6f74 6564 2066 2d73 7472 696e 6707 0000  oted f-string...
+000110d0: 000f 5173 6369 4c65 7865 7250 7974 686f  ..QsciLexerPytho
+000110e0: 6e01 0300 0000 4c00 5a00 6500 6900 6300  n.....L.Z.e.i.c.
+000110f0: 6800 6500 6e00 6b00 6500 7400 7400 6500  h.e.n.k.e.t.t.e.
+00011100: 2000 6900 6e00 2000 6400 7200 6500 6900   .i.n. .d.r.e.i.
+00011110: 6600 6100 6300 6800 6500 6e00 2000 4800  f.a.c.h.e.n. .H.
+00011120: 6f00 6300 6800 6b00 6f00 6d00 6d00 6100  o.c.h.k.o.m.m.a.
+00011130: 7400 6108 0000 0000 0600 0000 1b54 7269  t.a..........Tri
+00011140: 706c 6520 7369 6e67 6c65 2d71 756f 7465  ple single-quote
+00011150: 6420 7374 7269 6e67 0700 0000 0f51 7363  d string.....Qsc
+00011160: 694c 6578 6572 5079 7468 6f6e 0103 0000  iLexerPython....
+00011170: 002e 0055 006e 0062 0065 0065 006e 0064  ...U.n.b.e.e.n.d
+00011180: 0065 0074 0065 0020 005a 0065 0069 0063  .e.t.e. .Z.e.i.c
+00011190: 0068 0065 006e 006b 0065 0074 0074 0065  .h.e.n.k.e.t.t.e
+000111a0: 0800 0000 0006 0000 000f 556e 636c 6f73  ..........Unclos
+000111b0: 6564 2073 7472 696e 6707 0000 000f 5173  ed string.....Qs
+000111c0: 6369 4c65 7865 7250 7974 686f 6e01 0300  ciLexerPython...
+000111d0: 0000 1e00 2500 5100 2000 5a00 6500 6900  ....%.Q. .Z.e.i.
+000111e0: 6300 6800 6500 6e00 6b00 6500 7400 7400  c.h.e.n.k.e.t.t.
+000111f0: 6508 0000 0000 0600 0000 0925 5120 7374  e..........%Q st
+00011200: 7269 6e67 0700 0000 0d51 7363 694c 6578  ring.....QsciLex
+00011210: 6572 5275 6279 0103 0000 001e 0025 0071  erRuby.......%.q
+00011220: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
+00011230: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
+00011240: 0000 0009 2571 2073 7472 696e 6707 0000  ....%q string...
+00011250: 000d 5173 6369 4c65 7865 7252 7562 7901  ..QsciLexerRuby.
+00011260: 0300 0000 1e00 2500 7200 2000 5a00 6500  ......%.r. .Z.e.
+00011270: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
+00011280: 7400 6508 0000 0000 0600 0000 0925 7220  t.e..........%r 
+00011290: 7374 7269 6e67 0700 0000 0d51 7363 694c  string.....QsciL
+000112a0: 6578 6572 5275 6279 0103 0000 001e 0025  exerRuby.......%
+000112b0: 0077 0020 005a 0065 0069 0063 0068 0065  .w. .Z.e.i.c.h.e
+000112c0: 006e 006b 0065 0074 0074 0065 0800 0000  .n.k.e.t.t.e....
+000112d0: 0006 0000 0009 2577 2073 7472 696e 6707  ......%w string.
+000112e0: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
+000112f0: 7901 0300 0000 1e00 2500 7800 2000 5a00  y.......%.x. .Z.
+00011300: 6500 6900 6300 6800 6500 6e00 6b00 6500  e.i.c.h.e.n.k.e.
+00011310: 7400 7400 6508 0000 0000 0600 0000 0925  t.t.e..........%
+00011320: 7820 7374 7269 6e67 0700 0000 0d51 7363  x string.....Qsc
+00011330: 694c 6578 6572 5275 6279 0103 0000 0012  iLexerRuby......
+00011340: 0042 0061 0063 006b 0074 0069 0063 006b  .B.a.c.k.t.i.c.k
+00011350: 0073 0800 0000 0006 0000 0009 4261 636b  .s..........Back
+00011360: 7469 636b 7307 0000 000d 5173 6369 4c65  ticks.....QsciLe
+00011370: 7865 7252 7562 7901 0300 0000 1600 4b00  xerRuby.......K.
+00011380: 6c00 6100 7300 7300 6500 6e00 6e00 6100  l.a.s.s.e.n.n.a.
+00011390: 6d00 6508 0000 0000 0600 0000 0a43 6c61  m.e..........Cla
+000113a0: 7373 206e 616d 6507 0000 000d 5173 6369  ss name.....Qsci
+000113b0: 4c65 7865 7252 7562 7901 0300 0000 1e00  LexerRuby.......
+000113c0: 4b00 6c00 6100 7300 7300 6500 6e00 7600  K.l.a.s.s.e.n.v.
+000113d0: 6100 7200 6900 6100 6200 6c00 6508 0000  a.r.i.a.b.l.e...
+000113e0: 0000 0600 0000 0e43 6c61 7373 2076 6172  .......Class var
+000113f0: 6961 626c 6507 0000 000d 5173 6369 4c65  iable.....QsciLe
+00011400: 7865 7252 7562 7901 0300 0000 1200 4b00  xerRuby.......K.
+00011410: 6f00 6d00 6d00 6500 6e00 7400 6100 7208  o.m.m.e.n.t.a.r.
+00011420: 0000 0000 0600 0000 0743 6f6d 6d65 6e74  .........Comment
+00011430: 0700 0000 0d51 7363 694c 6578 6572 5275  .....QsciLexerRu
+00011440: 6279 0103 0000 0018 0044 0061 0074 0065  by.......D.a.t.e
+00011450: 006e 0073 0065 006b 0074 0069 006f 006e  .n.s.e.k.t.i.o.n
+00011460: 0800 0000 0006 0000 000c 4461 7461 2073  ..........Data s
+00011470: 6563 7469 6f6e 0700 0000 0d51 7363 694c  ection.....QsciL
+00011480: 6578 6572 5275 6279 0103 0000 0010 0053  exerRuby.......S
+00011490: 0074 0061 006e 0064 0061 0072 0064 0800  .t.a.n.d.a.r.d..
+000114a0: 0000 0006 0000 0007 4465 6661 756c 7407  ........Default.
+000114b0: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
+000114c0: 7901 0300 0000 3a00 7a00 7500 7200 fc00  y.....:.z.u.r...
+000114d0: 6300 6b00 6700 6500 7300 7400 7500 6600  c.k.g.e.s.t.u.f.
+000114e0: 7400 6500 7300 2000 5300 6300 6800 6c00  t.e.s. .S.c.h.l.
+000114f0: fc00 7300 7300 6500 6c00 7700 6f00 7200  ..s.s.e.l.w.o.r.
+00011500: 7408 0000 0000 0600 0000 0f44 656d 6f74  t..........Demot
+00011510: 6564 206b 6579 776f 7264 0700 0000 0d51  ed keyword.....Q
+00011520: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
+00011530: 0042 005a 0065 0069 0063 0068 0065 006e  .B.Z.e.i.c.h.e.n
+00011540: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
+00011550: 0020 0041 006e 0066 00fc 0068 0072 0075  . .A.n.f...h.r.u
+00011560: 006e 0067 0073 007a 0065 0069 0063 0068  .n.g.s.z.e.i.c.h
+00011570: 0065 006e 0800 0000 0006 0000 0014 446f  .e.n..........Do
+00011580: 7562 6c65 2d71 756f 7465 6420 7374 7269  uble-quoted stri
+00011590: 6e67 0700 0000 0d51 7363 694c 6578 6572  ng.....QsciLexer
+000115a0: 5275 6279 0103 0000 000c 0046 0065 0068  Ruby.......F.e.h
+000115b0: 006c 0065 0072 0800 0000 0006 0000 0005  .l.e.r..........
+000115c0: 4572 726f 7207 0000 000d 5173 6369 4c65  Error.....QsciLe
+000115d0: 7865 7252 7562 7901 0300 0000 3800 4600  xerRuby.....8.F.
+000115e0: 7500 6e00 6b00 7400 6900 6f00 6e00 7300  u.n.k.t.i.o.n.s.
+000115f0: 2d00 2000 6f00 6400 6500 7200 2000 4d00  -. .o.d.e.r. .M.
+00011600: 6500 7400 6800 6f00 6400 6500 6e00 6e00  e.t.h.o.d.e.n.n.
+00011610: 6100 6d00 6508 0000 0000 0600 0000 1746  a.m.e..........F
+00011620: 756e 6374 696f 6e20 6f72 206d 6574 686f  unction or metho
+00011630: 6420 6e61 6d65 0700 0000 0d51 7363 694c  d name.....QsciL
+00011640: 6578 6572 5275 6279 0103 0000 000c 0047  exerRuby.......G
+00011650: 006c 006f 0062 0061 006c 0800 0000 0006  .l.o.b.a.l......
+00011660: 0000 0006 476c 6f62 616c 0700 0000 0d51  ....Global.....Q
+00011670: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
+00011680: 001a 0048 0065 0072 0065 0020 0044 006f  ...H.e.r.e. .D.o
+00011690: 006b 0075 006d 0065 006e 0074 0800 0000  .k.u.m.e.n.t....
+000116a0: 0006 0000 000d 4865 7265 2064 6f63 756d  ......Here docum
+000116b0: 656e 7407 0000 000d 5173 6369 4c65 7865  ent.....QsciLexe
+000116c0: 7252 7562 7901 0300 0000 2e00 4800 6500  rRuby.......H.e.
+000116d0: 7200 6500 2000 4400 6f00 6b00 7500 6d00  r.e. .D.o.k.u.m.
+000116e0: 6500 6e00 7400 2d00 4200 6500 6700 7200  e.n.t.-.B.e.g.r.
+000116f0: 6500 6e00 7a00 6500 7208 0000 0000 0600  e.n.z.e.r.......
+00011700: 0000 1748 6572 6520 646f 6375 6d65 6e74  ...Here document
+00011710: 2064 656c 696d 6974 6572 0700 0000 0d51   delimiter.....Q
+00011720: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
+00011730: 0014 0042 0065 007a 0065 0069 0063 0068  ...B.e.z.e.i.c.h
+00011740: 006e 0065 0072 0800 0000 0006 0000 000a  .n.e.r..........
+00011750: 4964 656e 7469 6669 6572 0700 0000 0d51  Identifier.....Q
+00011760: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
+00011770: 001e 0049 006e 0073 0074 0061 006e 007a  ...I.n.s.t.a.n.z
+00011780: 0076 0061 0072 0069 0061 0062 006c 0065  .v.a.r.i.a.b.l.e
+00011790: 0800 0000 0006 0000 0011 496e 7374 616e  ..........Instan
+000117a0: 6365 2076 6172 6961 626c 6507 0000 000d  ce variable.....
+000117b0: 5173 6369 4c65 7865 7252 7562 7901 0300  QsciLexerRuby...
+000117c0: 0000 1a00 5300 6300 6800 6c00 fc00 7300  ....S.c.h.l...s.
+000117d0: 7300 6500 6c00 7700 6f00 7200 7408 0000  s.e.l.w.o.r.t...
+000117e0: 0000 0600 0000 074b 6579 776f 7264 0700  .......Keyword..
+000117f0: 0000 0d51 7363 694c 6578 6572 5275 6279  ...QsciLexerRuby
+00011800: 0103 0000 0012 004d 006f 0064 0075 006c  .......M.o.d.u.l
+00011810: 006e 0061 006d 0065 0800 0000 0006 0000  .n.a.m.e........
+00011820: 000b 4d6f 6475 6c65 206e 616d 6507 0000  ..Module name...
+00011830: 000d 5173 6369 4c65 7865 7252 7562 7901  ..QsciLexerRuby.
+00011840: 0300 0000 0800 5a00 6100 6800 6c08 0000  ......Z.a.h.l...
+00011850: 0000 0600 0000 064e 756d 6265 7207 0000  .......Number...
+00011860: 000d 5173 6369 4c65 7865 7252 7562 7901  ..QsciLexerRuby.
+00011870: 0300 0000 1000 4f00 7000 6500 7200 6100  ......O.p.e.r.a.
+00011880: 7400 6f00 7208 0000 0000 0600 0000 084f  t.o.r..........O
+00011890: 7065 7261 746f 7207 0000 000d 5173 6369  perator.....Qsci
+000118a0: 4c65 7865 7252 7562 7901 0300 0000 0600  LexerRuby.......
+000118b0: 5000 4f00 4408 0000 0000 0600 0000 0350  P.O.D..........P
+000118c0: 4f44 0700 0000 0d51 7363 694c 6578 6572  OD.....QsciLexer
+000118d0: 5275 6279 0103 0000 0024 0052 0065 0067  Ruby.....$.R.e.g
+000118e0: 0075 006c 00e4 0072 0065 0072 0020 0041  .u.l...r.e.r. .A
+000118f0: 0075 0073 0064 0072 0075 0063 006b 0800  .u.s.d.r.u.c.k..
+00011900: 0000 0006 0000 0012 5265 6775 6c61 7220  ........Regular 
+00011910: 6578 7072 6573 7369 6f6e 0700 0000 0d51  expression.....Q
+00011920: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
+00011930: 0036 005a 0065 0069 0063 0068 0065 006e  .6.Z.e.i.c.h.e.n
+00011940: 006b 0065 0074 0074 0065 0020 0069 006e  .k.e.t.t.e. .i.n
+00011950: 0020 0048 006f 0063 0068 006b 006f 006d  . .H.o.c.h.k.o.m
+00011960: 006d 0061 0074 0061 0800 0000 0006 0000  .m.a.t.a........
+00011970: 0014 5369 6e67 6c65 2d71 756f 7465 6420  ..Single-quoted 
+00011980: 7374 7269 6e67 0700 0000 0d51 7363 694c  string.....QsciL
+00011990: 6578 6572 5275 6279 0103 0000 000c 0053  exerRuby.......S
+000119a0: 0079 006d 0062 006f 006c 0800 0000 0006  .y.m.b.o.l......
+000119b0: 0000 0006 5379 6d62 6f6c 0700 0000 0d51  ....Symbol.....Q
+000119c0: 7363 694c 6578 6572 5275 6279 0103 0000  sciLexerRuby....
+000119d0: 000c 0053 0074 0064 0065 0072 0072 0800  ...S.t.d.e.r.r..
+000119e0: 0000 0006 0000 0006 7374 6465 7272 0700  ........stderr..
+000119f0: 0000 0d51 7363 694c 6578 6572 5275 6279  ...QsciLexerRuby
+00011a00: 0103 0000 000a 0053 0074 0064 0069 006e  .......S.t.d.i.n
+00011a10: 0800 0000 0006 0000 0005 7374 6469 6e07  ..........stdin.
+00011a20: 0000 000d 5173 6369 4c65 7865 7252 7562  ....QsciLexerRub
+00011a30: 7901 0300 0000 0c00 5300 7400 6400 6f00  y.......S.t.d.o.
+00011a40: 7500 7408 0000 0000 0600 0000 0673 7464  u.t..........std
+00011a50: 6f75 7407 0000 000d 5173 6369 4c65 7865  out.....QsciLexe
+00011a60: 7252 7562 7901 0300 0000 2000 2300 2000  rRuby..... .#. .
+00011a70: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00011a80: 7200 7a00 6500 6900 6c00 6508 0000 0000  r.z.e.i.l.e.....
+00011a90: 0600 0000 0e23 2063 6f6d 6d65 6e74 206c  .....# comment l
+00011aa0: 696e 6507 0000 000c 5173 6369 4c65 7865  ine.....QsciLexe
+00011ab0: 7253 514c 0103 0000 0012 004b 006f 006d  rSQL.......K.o.m
+00011ac0: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
+00011ad0: 0006 0000 0007 436f 6d6d 656e 7407 0000  ......Comment...
+00011ae0: 000c 5173 6369 4c65 7865 7253 514c 0103  ..QsciLexerSQL..
+00011af0: 0000 001c 004b 006f 006d 006d 0065 006e  .....K.o.m.m.e.n
+00011b00: 0074 0061 0072 007a 0065 0069 006c 0065  .t.a.r.z.e.i.l.e
+00011b10: 0800 0000 0006 0000 000c 436f 6d6d 656e  ..........Commen
+00011b20: 7420 6c69 6e65 0700 0000 0c51 7363 694c  t line.....QsciL
+00011b30: 6578 6572 5351 4c01 0300 0000 1000 5300  exerSQL.......S.
+00011b40: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
+00011b50: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
+00011b60: 0000 0c51 7363 694c 6578 6572 5351 4c01  ...QsciLexerSQL.
+00011b70: 0300 0000 4200 5a00 6500 6900 6300 6800  ....B.Z.e.i.c.h.
+00011b80: 6500 6e00 6b00 6500 7400 7400 6500 2000  e.n.k.e.t.t.e. .
+00011b90: 6900 6e00 2000 4100 6e00 6600 fc00 6800  i.n. .A.n.f...h.
+00011ba0: 7200 7500 6e00 6700 7300 7a00 6500 6900  r.u.n.g.s.z.e.i.
+00011bb0: 6300 6800 6500 6e08 0000 0000 0600 0000  c.h.e.n.........
+00011bc0: 1444 6f75 626c 652d 7175 6f74 6564 2073  .Double-quoted s
+00011bd0: 7472 696e 6707 0000 000c 5173 6369 4c65  tring.....QsciLe
+00011be0: 7865 7253 514c 0103 0000 0014 0042 0065  xerSQL.......B.e
+00011bf0: 007a 0065 0069 0063 0068 006e 0065 0072  .z.e.i.c.h.n.e.r
+00011c00: 0800 0000 0006 0000 000a 4964 656e 7469  ..........Identi
+00011c10: 6669 6572 0700 0000 0c51 7363 694c 6578  fier.....QsciLex
+00011c20: 6572 5351 4c01 0300 0000 2a00 4a00 6100  erSQL.....*.J.a.
+00011c30: 7600 6100 4400 6f00 6300 2000 5300 6300  v.a.D.o.c. .S.c.
+00011c40: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
+00011c50: 6f00 7200 7408 0000 0000 0600 0000 0f4a  o.r.t..........J
+00011c60: 6176 6144 6f63 206b 6579 776f 7264 0700  avaDoc keyword..
+00011c70: 0000 0c51 7363 694c 6578 6572 5351 4c01  ...QsciLexerSQL.
+00011c80: 0300 0000 3600 4a00 6100 7600 6100 4400  ....6.J.a.v.a.D.
+00011c90: 6f00 6300 2000 5300 6300 6800 6c00 fc00  o.c. .S.c.h.l...
+00011ca0: 7300 7300 6500 6c00 7700 6f00 7200 7400  s.s.e.l.w.o.r.t.
+00011cb0: 6600 6500 6800 6c00 6500 7208 0000 0000  f.e.h.l.e.r.....
+00011cc0: 0600 0000 154a 6176 6144 6f63 206b 6579  .....JavaDoc key
+00011cd0: 776f 7264 2065 7272 6f72 0700 0000 0c51  word error.....Q
+00011ce0: 7363 694c 6578 6572 5351 4c01 0300 0000  sciLexerSQL.....
+00011cf0: 2200 4a00 6100 7600 6100 4400 6f00 6300  ".J.a.v.a.D.o.c.
+00011d00: 2000 4b00 6f00 6d00 6d00 6500 6e00 7400   .K.o.m.m.e.n.t.
+00011d10: 6100 7208 0000 0000 0600 0000 154a 6176  a.r..........Jav
+00011d20: 6144 6f63 2073 7479 6c65 2063 6f6d 6d65  aDoc style comme
+00011d30: 6e74 0700 0000 0c51 7363 694c 6578 6572  nt.....QsciLexer
+00011d40: 5351 4c01 0300 0000 1a00 5300 6300 6800  SQL.......S.c.h.
+00011d50: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
+00011d60: 7200 7408 0000 0000 0600 0000 074b 6579  r.t..........Key
+00011d70: 776f 7264 0700 0000 0c51 7363 694c 6578  word.....QsciLex
+00011d80: 6572 5351 4c01 0300 0000 0800 5a00 6100  erSQL.......Z.a.
+00011d90: 6800 6c08 0000 0000 0600 0000 064e 756d  h.l..........Num
+00011da0: 6265 7207 0000 000c 5173 6369 4c65 7865  ber.....QsciLexe
+00011db0: 7253 514c 0103 0000 0010 004f 0070 0065  rSQL.......O.p.e
+00011dc0: 0072 0061 0074 006f 0072 0800 0000 0006  .r.a.t.o.r......
+00011dd0: 0000 0008 4f70 6572 6174 6f72 0700 0000  ....Operator....
+00011de0: 0c51 7363 694c 6578 6572 5351 4c01 0300  .QsciLexerSQL...
+00011df0: 0000 3e00 4200 6500 7a00 6500 6900 6300  ..>.B.e.z.e.i.c.
+00011e00: 6800 6e00 6500 7200 2000 6900 6e00 2000  h.n.e.r. .i.n. .
+00011e10: 4100 6e00 6600 fc00 6800 7200 7500 6e00  A.n.f...h.r.u.n.
+00011e20: 6700 7300 7a00 6500 6900 6300 6800 6500  g.s.z.e.i.c.h.e.
+00011e30: 6e08 0000 0000 0600 0000 1151 756f 7465  n..........Quote
+00011e40: 6420 6964 656e 7469 6669 6572 0700 0000  d identifier....
+00011e50: 0c51 7363 694c 6578 6572 5351 4c01 0300  .QsciLexerSQL...
+00011e60: 0000 3a00 4f00 7000 6500 7200 6100 7400  ..:.O.p.e.r.a.t.
+00011e70: 6f00 7200 2000 6900 6e00 2000 4100 6e00  o.r. .i.n. .A.n.
+00011e80: 6600 fc00 6800 7200 7500 6e00 6700 7300  f...h.r.u.n.g.s.
+00011e90: 7a00 6500 6900 6300 6800 6500 6e08 0000  z.e.i.c.h.e.n...
+00011ea0: 0000 0600 0000 0f51 756f 7465 6420 6f70  .......Quoted op
+00011eb0: 6572 6174 6f72 0700 0000 0c51 7363 694c  erator.....QsciL
+00011ec0: 6578 6572 5351 4c01 0300 0000 2400 5300  exerSQL.....$.S.
+00011ed0: 5100 4c00 2a00 5000 6c00 7500 7300 2000  Q.L.*.P.l.u.s. .
+00011ee0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00011ef0: 7208 0000 0000 0600 0000 1053 514c 2a50  r..........SQL*P
+00011f00: 6c75 7320 636f 6d6d 656e 7407 0000 000c  lus comment.....
+00011f10: 5173 6369 4c65 7865 7253 514c 0103 0000  QsciLexerSQL....
+00011f20: 002c 0053 0051 004c 002a 0050 006c 0075  .,.S.Q.L.*.P.l.u
+00011f30: 0073 0020 0053 0063 0068 006c 00fc 0073  .s. .S.c.h.l...s
+00011f40: 0073 0065 006c 0077 006f 0072 0074 0800  .s.e.l.w.o.r.t..
+00011f50: 0000 0006 0000 0010 5351 4c2a 506c 7573  ........SQL*Plus
+00011f60: 206b 6579 776f 7264 0700 0000 0c51 7363   keyword.....Qsc
+00011f70: 694c 6578 6572 5351 4c01 0300 0000 2000  iLexerSQL..... .
+00011f80: 5300 5100 4c00 2a00 5000 6c00 7500 7300  S.Q.L.*.P.l.u.s.
+00011f90: 2000 4500 6900 6e00 6700 6100 6200 6508   .E.i.n.g.a.b.e.
+00011fa0: 0000 0000 0600 0000 0f53 514c 2a50 6c75  .........SQL*Plu
+00011fb0: 7320 7072 6f6d 7074 0700 0000 0c51 7363  s prompt.....Qsc
+00011fc0: 694c 6578 6572 5351 4c01 0300 0000 3600  iLexerSQL.....6.
+00011fd0: 5a00 6500 6900 6300 6800 6500 6e00 6b00  Z.e.i.c.h.e.n.k.
+00011fe0: 6500 7400 7400 6500 2000 6900 6e00 2000  e.t.t.e. .i.n. .
+00011ff0: 4800 6f00 6300 6800 6b00 6f00 6d00 6d00  H.o.c.h.k.o.m.m.
+00012000: 6100 7400 6108 0000 0000 0600 0000 1453  a.t.a..........S
+00012010: 696e 676c 652d 7175 6f74 6564 2073 7472  ingle-quoted str
+00012020: 696e 6707 0000 000c 5173 6369 4c65 7865  ing.....QsciLexe
+00012030: 7253 514c 0103 0000 0024 004e 0075 0074  rSQL.....$.N.u.t
+00012040: 007a 0065 0072 0020 0064 0065 0066 0069  .z.e.r. .d.e.f.i
+00012050: 006e 0069 0065 0072 0074 0020 0031 0800  .n.i.e.r.t. .1..
+00012060: 0000 0006 0000 000e 5573 6572 2064 6566  ........User def
+00012070: 696e 6564 2031 0700 0000 0c51 7363 694c  ined 1.....QsciL
+00012080: 6578 6572 5351 4c01 0300 0000 2400 4e00  exerSQL.....$.N.
+00012090: 7500 7400 7a00 6500 7200 2000 6400 6500  u.t.z.e.r. .d.e.
+000120a0: 6600 6900 6e00 6900 6500 7200 7400 2000  f.i.n.i.e.r.t. .
+000120b0: 3208 0000 0000 0600 0000 0e55 7365 7220  2..........User 
+000120c0: 6465 6669 6e65 6420 3207 0000 000c 5173  defined 2.....Qs
+000120d0: 6369 4c65 7865 7253 514c 0103 0000 0024  ciLexerSQL.....$
+000120e0: 004e 0075 0074 007a 0065 0072 0020 0064  .N.u.t.z.e.r. .d
+000120f0: 0065 0066 0069 006e 0069 0065 0072 0074  .e.f.i.n.i.e.r.t
+00012100: 0020 0033 0800 0000 0006 0000 000e 5573  . .3..........Us
+00012110: 6572 2064 6566 696e 6564 2033 0700 0000  er defined 3....
+00012120: 0c51 7363 694c 6578 6572 5351 4c01 0300  .QsciLexerSQL...
+00012130: 0000 2400 4e00 7500 7400 7a00 6500 7200  ..$.N.u.t.z.e.r.
+00012140: 2000 6400 6500 6600 6900 6e00 6900 6500   .d.e.f.i.n.i.e.
+00012150: 7200 7400 2000 3408 0000 0000 0600 0000  r.t. .4.........
+00012160: 0e55 7365 7220 6465 6669 6e65 6420 3407  .User defined 4.
+00012170: 0000 000c 5173 6369 4c65 7865 7253 514c  ....QsciLexerSQL
+00012180: 0103 0000 000c 0042 0065 0066 0065 0068  .......B.e.f.e.h
+00012190: 006c 0800 0000 0006 0000 0007 436f 6d6d  .l..........Comm
+000121a0: 616e 6407 0000 000e 5173 6369 4c65 7865  and.....QsciLexe
+000121b0: 7253 7069 6365 0103 0000 0012 004b 006f  rSpice.......K.o
+000121c0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+000121d0: 0000 0006 0000 0007 436f 6d6d 656e 7407  ........Comment.
+000121e0: 0000 000e 5173 6369 4c65 7865 7253 7069  ....QsciLexerSpi
+000121f0: 6365 0103 0000 0010 0053 0074 0061 006e  ce.......S.t.a.n
+00012200: 0064 0061 0072 0064 0800 0000 0006 0000  .d.a.r.d........
+00012210: 0007 4465 6661 756c 7407 0000 000e 5173  ..Default.....Qs
+00012220: 6369 4c65 7865 7253 7069 6365 0103 0000  ciLexerSpice....
+00012230: 0012 0044 0065 006c 0069 006d 0069 0074  ...D.e.l.i.m.i.t
+00012240: 0065 0072 0800 0000 0006 0000 0009 4465  .e.r..........De
+00012250: 6c69 6d69 7465 7207 0000 000e 5173 6369  limiter.....Qsci
+00012260: 4c65 7865 7253 7069 6365 0103 0000 0010  LexerSpice......
+00012270: 0046 0075 006e 006b 0074 0069 006f 006e  .F.u.n.k.t.i.o.n
+00012280: 0800 0000 0006 0000 0008 4675 6e63 7469  ..........Functi
+00012290: 6f6e 0700 0000 0e51 7363 694c 6578 6572  on.....QsciLexer
+000122a0: 5370 6963 6501 0300 0000 1400 4200 6500  Spice.......B.e.
+000122b0: 7a00 6500 6900 6300 6800 6e00 6500 7208  z.e.i.c.h.n.e.r.
+000122c0: 0000 0000 0600 0000 0a49 6465 6e74 6966  .........Identif
+000122d0: 6965 7207 0000 000e 5173 6369 4c65 7865  ier.....QsciLexe
+000122e0: 7253 7069 6365 0103 0000 0008 005a 0061  rSpice.......Z.a
+000122f0: 0068 006c 0800 0000 0006 0000 0006 4e75  .h.l..........Nu
+00012300: 6d62 6572 0700 0000 0e51 7363 694c 6578  mber.....QsciLex
+00012310: 6572 5370 6963 6501 0300 0000 1200 5000  erSpice.......P.
+00012320: 6100 7200 6100 6d00 6500 7400 6500 7208  a.r.a.m.e.t.e.r.
+00012330: 0000 0000 0600 0000 0950 6172 616d 6574  .........Paramet
+00012340: 6572 0700 0000 0e51 7363 694c 6578 6572  er.....QsciLexer
+00012350: 5370 6963 6501 0300 0000 0800 5700 6500  Spice.......W.e.
+00012360: 7200 7408 0000 0000 0600 0000 0556 616c  r.t..........Val
+00012370: 7565 0700 0000 0e51 7363 694c 6578 6572  ue.....QsciLexer
+00012380: 5370 6963 6501 0300 0000 2000 4b00 6c00  Spice..... .K.l.
+00012390: 6100 6d00 6d00 6500 7200 6500 7200 7300  a.m.m.e.r.e.r.s.
+000123a0: 6500 7400 7a00 7500 6e00 6708 0000 0000  e.t.z.u.n.g.....
+000123b0: 0600 0000 1242 7261 6365 2073 7562 7374  .....Brace subst
+000123c0: 6974 7574 696f 6e07 0000 000c 5173 6369  itution.....Qsci
+000123d0: 4c65 7865 7254 434c 0103 0000 0012 004b  LexerTCL.......K
+000123e0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
+000123f0: 0800 0000 0006 0000 0007 436f 6d6d 656e  ..........Commen
+00012400: 7407 0000 000c 5173 6369 4c65 7865 7254  t.....QsciLexerT
+00012410: 434c 0103 0000 001c 004b 006f 006d 006d  CL.......K.o.m.m
+00012420: 0065 006e 0074 0061 0072 0062 006c 006f  .e.n.t.a.r.b.l.o
+00012430: 0063 006b 0800 0000 0006 0000 000d 436f  .c.k..........Co
+00012440: 6d6d 656e 7420 626c 6f63 6b07 0000 000c  mment block.....
+00012450: 5173 6369 4c65 7865 7254 434c 0103 0000  QsciLexerTCL....
+00012460: 0018 004b 006f 006d 006d 0065 006e 0074  ...K.o.m.m.e.n.t
+00012470: 0061 0072 0062 006f 0078 0800 0000 0006  .a.r.b.o.x......
+00012480: 0000 000b 436f 6d6d 656e 7420 626f 7807  ....Comment box.
+00012490: 0000 000c 5173 6369 4c65 7865 7254 434c  ....QsciLexerTCL
+000124a0: 0103 0000 001c 004b 006f 006d 006d 0065  .......K.o.m.m.e
+000124b0: 006e 0074 0061 0072 007a 0065 0069 006c  .n.t.a.r.z.e.i.l
+000124c0: 0065 0800 0000 0006 0000 000c 436f 6d6d  .e..........Comm
+000124d0: 656e 7420 6c69 6e65 0700 0000 0c51 7363  ent line.....Qsc
+000124e0: 694c 6578 6572 5443 4c01 0300 0000 1000  iLexerTCL.......
+000124f0: 5300 7400 6100 6e00 6400 6100 7200 6408  S.t.a.n.d.a.r.d.
+00012500: 0000 0000 0600 0000 0744 6566 6175 6c74  .........Default
+00012510: 0700 0000 0c51 7363 694c 6578 6572 5443  .....QsciLexerTC
+00012520: 4c01 0300 0000 3200 4500 7200 7700 6500  L.....2.E.r.w.e.
+00012530: 6900 7400 6500 7200 7500 6e00 6700 7300  i.t.e.r.u.n.g.s.
+00012540: 7300 6300 6800 6c00 fc00 7300 7300 6500  s.c.h.l...s.s.e.
+00012550: 6c00 7700 6f00 7200 7408 0000 0000 0600  l.w.o.r.t.......
+00012560: 0000 0e45 7870 616e 6420 6b65 7977 6f72  ...Expand keywor
+00012570: 6407 0000 000c 5173 6369 4c65 7865 7254  d.....QsciLexerT
+00012580: 434c 0103 0000 0014 0042 0065 007a 0065  CL.......B.e.z.e
+00012590: 0069 0063 0068 006e 0065 0072 0800 0000  .i.c.h.n.e.r....
+000125a0: 0006 0000 000a 4964 656e 7469 6669 6572  ......Identifier
+000125b0: 0700 0000 0c51 7363 694c 6578 6572 5443  .....QsciLexerTC
+000125c0: 4c01 0300 0000 1800 4d00 6f00 6400 6900  L.......M.o.d.i.
+000125d0: 6600 6900 7a00 6900 6500 7200 6500 7208  f.i.z.i.e.r.e.r.
+000125e0: 0000 0000 0600 0000 084d 6f64 6966 6965  .........Modifie
+000125f0: 7207 0000 000c 5173 6369 4c65 7865 7254  r.....QsciLexerT
+00012600: 434c 0103 0000 0008 005a 0061 0068 006c  CL.......Z.a.h.l
+00012610: 0800 0000 0006 0000 0006 4e75 6d62 6572  ..........Number
+00012620: 0700 0000 0c51 7363 694c 6578 6572 5443  .....QsciLexerTC
+00012630: 4c01 0300 0000 1000 4f00 7000 6500 7200  L.......O.p.e.r.
+00012640: 6100 7400 6f00 7208 0000 0000 0600 0000  a.t.o.r.........
+00012650: 084f 7065 7261 746f 7207 0000 000c 5173  .Operator.....Qs
+00012660: 6369 4c65 7865 7254 434c 0103 0000 0032  ciLexerTCL.....2
+00012670: 0061 006e 0067 0065 0066 00fc 0068 0072  .a.n.g.e.f...h.r
+00012680: 0074 0065 0073 0020 0053 0063 0068 006c  .t.e.s. .S.c.h.l
+00012690: 00fc 0073 0073 0065 006c 0077 006f 0072  ...s.s.e.l.w.o.r
+000126a0: 0074 0800 0000 0006 0000 000e 5175 6f74  .t..........Quot
+000126b0: 6564 206b 6579 776f 7264 0700 0000 0c51  ed keyword.....Q
+000126c0: 7363 694c 6578 6572 5443 4c01 0300 0000  sciLexerTCL.....
+000126d0: 1800 5a00 6500 6900 6300 6800 6500 6e00  ..Z.e.i.c.h.e.n.
+000126e0: 6b00 6500 7400 7400 6508 0000 0000 0600  k.e.t.t.e.......
+000126f0: 0000 0d51 756f 7465 6420 7374 7269 6e67  ...Quoted string
+00012700: 0700 0000 0c51 7363 694c 6578 6572 5443  .....QsciLexerTC
+00012710: 4c01 0300 0000 1200 4500 7200 7300 6500  L.......E.r.s.e.
+00012720: 7400 7a00 7500 6e00 6708 0000 0000 0600  t.z.u.n.g.......
+00012730: 0000 0c53 7562 7374 6974 7574 696f 6e07  ...Substitution.
+00012740: 0000 000c 5173 6369 4c65 7865 7254 434c  ....QsciLexerTCL
+00012750: 0103 0000 0022 0054 0043 004c 0020 0053  .....".T.C.L. .S
+00012760: 0063 0068 006c 00fc 0073 0073 0065 006c  .c.h.l...s.s.e.l
+00012770: 0077 006f 0072 0074 0800 0000 0006 0000  .w.o.r.t........
+00012780: 000b 5443 4c20 6b65 7977 6f72 6407 0000  ..TCL keyword...
+00012790: 000c 5173 6369 4c65 7865 7254 434c 0103  ..QsciLexerTCL..
+000127a0: 0000 0012 0054 006b 0020 0042 0065 0066  .....T.k. .B.e.f
+000127b0: 0065 0068 006c 0800 0000 0006 0000 000a  .e.h.l..........
+000127c0: 546b 2063 6f6d 6d61 6e64 0700 0000 0c51  Tk command.....Q
+000127d0: 7363 694c 6578 6572 5443 4c01 0300 0000  sciLexerTCL.....
+000127e0: 2000 5400 6b00 2000 5300 6300 6800 6c00   .T.k. .S.c.h.l.
+000127f0: fc00 7300 7300 6500 6c00 7700 6f00 7200  ..s.s.e.l.w.o.r.
+00012800: 7408 0000 0000 0600 0000 0a54 6b20 6b65  t..........Tk ke
+00012810: 7977 6f72 6407 0000 000c 5173 6369 4c65  yword.....QsciLe
+00012820: 7865 7254 434c 0103 0000 0024 004e 0075  xerTCL.....$.N.u
+00012830: 0074 007a 0065 0072 0020 0064 0065 0066  .t.z.e.r. .d.e.f
+00012840: 0069 006e 0069 0065 0072 0074 0020 0031  .i.n.i.e.r.t. .1
+00012850: 0800 0000 0006 0000 000e 5573 6572 2064  ..........User d
+00012860: 6566 696e 6564 2031 0700 0000 0c51 7363  efined 1.....Qsc
+00012870: 694c 6578 6572 5443 4c01 0300 0000 2400  iLexerTCL.....$.
+00012880: 4e00 7500 7400 7a00 6500 7200 2000 6400  N.u.t.z.e.r. .d.
+00012890: 6500 6600 6900 6e00 6900 6500 7200 7400  e.f.i.n.i.e.r.t.
+000128a0: 2000 3208 0000 0000 0600 0000 0e55 7365   .2..........Use
+000128b0: 7220 6465 6669 6e65 6420 3207 0000 000c  r defined 2.....
+000128c0: 5173 6369 4c65 7865 7254 434c 0103 0000  QsciLexerTCL....
+000128d0: 0024 004e 0075 0074 007a 0065 0072 0020  .$.N.u.t.z.e.r. 
+000128e0: 0064 0065 0066 0069 006e 0069 0065 0072  .d.e.f.i.n.i.e.r
+000128f0: 0074 0020 0033 0800 0000 0006 0000 000e  .t. .3..........
+00012900: 5573 6572 2064 6566 696e 6564 2033 0700  User defined 3..
+00012910: 0000 0c51 7363 694c 6578 6572 5443 4c01  ...QsciLexerTCL.
+00012920: 0300 0000 2400 4e00 7500 7400 7a00 6500  ....$.N.u.t.z.e.
+00012930: 7200 2000 6400 6500 6600 6900 6e00 6900  r. .d.e.f.i.n.i.
+00012940: 6500 7200 7400 2000 3408 0000 0000 0600  e.r.t. .4.......
+00012950: 0000 0e55 7365 7220 6465 6669 6e65 6420  ...User defined 
+00012960: 3407 0000 000c 5173 6369 4c65 7865 7254  4.....QsciLexerT
+00012970: 434c 0103 0000 0024 0069 0054 0043 004c  CL.....$.i.T.C.L
+00012980: 0020 0053 0063 0068 006c 00fc 0073 0073  . .S.c.h.l...s.s
+00012990: 0065 006c 0077 006f 0072 0074 0800 0000  .e.l.w.o.r.t....
+000129a0: 0006 0000 000c 6954 434c 206b 6579 776f  ......iTCL keywo
+000129b0: 7264 0700 0000 0c51 7363 694c 6578 6572  rd.....QsciLexer
+000129c0: 5443 4c01 0300 0000 0c00 4200 6500 6600  TCL.......B.e.f.
+000129d0: 6500 6800 6c08 0000 0000 0600 0000 0743  e.h.l..........C
+000129e0: 6f6d 6d61 6e64 0700 0000 0c51 7363 694c  ommand.....QsciL
+000129f0: 6578 6572 5465 5801 0300 0000 1000 5300  exerTeX.......S.
+00012a00: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
+00012a10: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
+00012a20: 0000 0c51 7363 694c 6578 6572 5465 5801  ...QsciLexerTeX.
+00012a30: 0300 0000 0c00 4700 7200 7500 7000 7000  ......G.r.u.p.p.
+00012a40: 6508 0000 0000 0600 0000 0547 726f 7570  e..........Group
+00012a50: 0700 0000 0c51 7363 694c 6578 6572 5465  .....QsciLexerTe
+00012a60: 5801 0300 0000 0e00 5300 7000 6500 7a00  X.......S.p.e.z.
+00012a70: 6900 6100 6c08 0000 0000 0600 0000 0753  i.a.l..........S
+00012a80: 7065 6369 616c 0700 0000 0c51 7363 694c  pecial.....QsciL
+00012a90: 6578 6572 5465 5801 0300 0000 0c00 5300  exerTeX.......S.
+00012aa0: 7900 6d00 6200 6f00 6c08 0000 0000 0600  y.m.b.o.l.......
+00012ab0: 0000 0653 796d 626f 6c07 0000 000c 5173  ...Symbol.....Qs
+00012ac0: 6369 4c65 7865 7254 6558 0103 0000 0008  ciLexerTeX......
+00012ad0: 0054 0065 0078 0074 0800 0000 0006 0000  .T.e.x.t........
+00012ae0: 0004 5465 7874 0700 0000 0c51 7363 694c  ..Text.....QsciL
+00012af0: 6578 6572 5465 5801 0300 0000 1000 4100  exerTeX.......A.
+00012b00: 7400 7400 7200 6900 6200 7500 7408 0000  t.t.r.i.b.u.t...
+00012b10: 0000 0600 0000 0941 7474 7269 6275 7465  .......Attribute
+00012b20: 0700 0000 0d51 7363 694c 6578 6572 5648  .....QsciLexerVH
+00012b30: 444c 0103 0000 0012 004b 006f 006d 006d  DL.......K.o.m.m
+00012b40: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+00012b50: 0000 0007 436f 6d6d 656e 7407 0000 000d  ....Comment.....
+00012b60: 5173 6369 4c65 7865 7256 4844 4c01 0300  QsciLexerVHDL...
+00012b70: 0000 1c00 4b00 6f00 6d00 6d00 6500 6e00  ....K.o.m.m.e.n.
+00012b80: 7400 6100 7200 6200 6c00 6f00 6300 6b08  t.a.r.b.l.o.c.k.
+00012b90: 0000 0000 0600 0000 0d43 6f6d 6d65 6e74  .........Comment
+00012ba0: 2062 6c6f 636b 0700 0000 0d51 7363 694c   block.....QsciL
+00012bb0: 6578 6572 5648 444c 0103 0000 001c 004b  exerVHDL.......K
+00012bc0: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
+00012bd0: 007a 0065 0069 006c 0065 0800 0000 0006  .z.e.i.l.e......
+00012be0: 0000 000c 436f 6d6d 656e 7420 6c69 6e65  ....Comment line
+00012bf0: 0700 0000 0d51 7363 694c 6578 6572 5648  .....QsciLexerVH
+00012c00: 444c 0103 0000 0010 0053 0074 0061 006e  DL.......S.t.a.n
+00012c10: 0064 0061 0072 0064 0800 0000 0006 0000  .d.a.r.d........
+00012c20: 0007 4465 6661 756c 7407 0000 000d 5173  ..Default.....Qs
+00012c30: 6369 4c65 7865 7256 4844 4c01 0300 0000  ciLexerVHDL.....
+00012c40: 1400 4200 6500 7a00 6500 6900 6300 6800  ..B.e.z.e.i.c.h.
+00012c50: 6e00 6500 7208 0000 0000 0600 0000 0a49  n.e.r..........I
+00012c60: 6465 6e74 6966 6965 7207 0000 000d 5173  dentifier.....Qs
+00012c70: 6369 4c65 7865 7256 4844 4c01 0300 0000  ciLexerVHDL.....
+00012c80: 1a00 5300 6300 6800 6c00 fc00 7300 7300  ..S.c.h.l...s.s.
+00012c90: 6500 6c00 7700 6f00 7200 7408 0000 0000  e.l.w.o.r.t.....
+00012ca0: 0600 0000 074b 6579 776f 7264 0700 0000  .....Keyword....
+00012cb0: 0d51 7363 694c 6578 6572 5648 444c 0103  .QsciLexerVHDL..
+00012cc0: 0000 0008 005a 0061 0068 006c 0800 0000  .....Z.a.h.l....
+00012cd0: 0006 0000 0006 4e75 6d62 6572 0700 0000  ......Number....
+00012ce0: 0d51 7363 694c 6578 6572 5648 444c 0103  .QsciLexerVHDL..
+00012cf0: 0000 0010 004f 0070 0065 0072 0061 0074  .....O.p.e.r.a.t
+00012d00: 006f 0072 0800 0000 0006 0000 0008 4f70  .o.r..........Op
+00012d10: 6572 6174 6f72 0700 0000 0d51 7363 694c  erator.....QsciL
+00012d20: 6578 6572 5648 444c 0103 0000 0020 0053  exerVHDL..... .S
+00012d30: 0074 0061 006e 0064 0061 0072 0064 0066  .t.a.n.d.a.r.d.f
+00012d40: 0075 006e 006b 0074 0069 006f 006e 0800  .u.n.k.t.i.o.n..
+00012d50: 0000 0006 0000 0011 5374 616e 6461 7264  ........Standard
+00012d60: 2066 756e 6374 696f 6e07 0000 000d 5173   function.....Qs
+00012d70: 6369 4c65 7865 7256 4844 4c01 0300 0000  ciLexerVHDL.....
+00012d80: 2000 5300 7400 6100 6e00 6400 6100 7200   .S.t.a.n.d.a.r.
+00012d90: 6400 6f00 7000 6500 7200 6100 7400 6f00  d.o.p.e.r.a.t.o.
+00012da0: 7208 0000 0000 0600 0000 1153 7461 6e64  r..........Stand
+00012db0: 6172 6420 6f70 6572 6174 6f72 0700 0000  ard operator....
+00012dc0: 0d51 7363 694c 6578 6572 5648 444c 0103  .QsciLexerVHDL..
+00012dd0: 0000 001a 0053 0074 0061 006e 0064 0061  .....S.t.a.n.d.a
+00012de0: 0072 0064 0070 0061 006b 0065 0074 0800  .r.d.p.a.k.e.t..
+00012df0: 0000 0006 0000 0010 5374 616e 6461 7264  ........Standard
+00012e00: 2070 6163 6b61 6765 0700 0000 0d51 7363   package.....Qsc
+00012e10: 694c 6578 6572 5648 444c 0103 0000 0016  iLexerVHDL......
+00012e20: 0053 0074 0061 006e 0064 0061 0072 0064  .S.t.a.n.d.a.r.d
+00012e30: 0074 0079 0070 0800 0000 0006 0000 000d  .t.y.p..........
+00012e40: 5374 616e 6461 7264 2074 7970 6507 0000  Standard type...
+00012e50: 000d 5173 6369 4c65 7865 7256 4844 4c01  ..QsciLexerVHDL.
+00012e60: 0300 0000 1800 5a00 6500 6900 6300 6800  ......Z.e.i.c.h.
+00012e70: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
+00012e80: 0000 0600 0000 0653 7472 696e 6707 0000  .......String...
+00012e90: 000d 5173 6369 4c65 7865 7256 4844 4c01  ..QsciLexerVHDL.
+00012ea0: 0300 0000 2e00 5500 6e00 6200 6500 6500  ......U.n.b.e.e.
+00012eb0: 6e00 6400 6500 7400 6500 2000 5a00 6500  n.d.e.t.e. .Z.e.
+00012ec0: 6900 6300 6800 6500 6e00 6b00 6500 7400  i.c.h.e.n.k.e.t.
+00012ed0: 7400 6508 0000 0000 0600 0000 0f55 6e63  t.e..........Unc
+00012ee0: 6c6f 7365 6420 7374 7269 6e67 0700 0000  losed string....
+00012ef0: 0d51 7363 694c 6578 6572 5648 444c 0103  .QsciLexerVHDL..
+00012f00: 0000 0020 004e 0075 0074 007a 0065 0072  ... .N.u.t.z.e.r
+00012f10: 0020 0064 0065 0066 0069 006e 0069 0065  . .d.e.f.i.n.i.e
+00012f20: 0072 0074 0800 0000 0006 0000 000c 5573  .r.t..........Us
+00012f30: 6572 2064 6566 696e 6564 0700 0000 0d51  er defined.....Q
+00012f40: 7363 694c 6578 6572 5648 444c 0103 0000  sciLexerVHDL....
+00012f50: 001c 0042 0061 006e 0067 0020 004b 006f  ...B.a.n.g. .K.o
+00012f60: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
+00012f70: 0000 0006 0000 000c 4261 6e67 2063 6f6d  ........Bang com
+00012f80: 6d65 6e74 0700 0000 1051 7363 694c 6578  ment.....QsciLex
+00012f90: 6572 5665 7269 6c6f 6701 0300 0000 1200  erVerilog.......
+00012fa0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00012fb0: 7208 0000 0000 0600 0000 0743 6f6d 6d65  r..........Comme
+00012fc0: 6e74 0700 0000 1051 7363 694c 6578 6572  nt.....QsciLexer
+00012fd0: 5665 7269 6c6f 6701 0300 0000 1000 5300  Verilog.......S.
+00012fe0: 7400 6100 6e00 6400 6100 7200 6408 0000  t.a.n.d.a.r.d...
+00012ff0: 0000 0600 0000 0744 6566 6175 6c74 0700  .......Default..
+00013000: 0000 1051 7363 694c 6578 6572 5665 7269  ...QsciLexerVeri
+00013010: 6c6f 6701 0300 0000 1400 4200 6500 7a00  log.......B.e.z.
+00013020: 6500 6900 6300 6800 6e00 6500 7208 0000  e.i.c.h.n.e.r...
+00013030: 0000 0600 0000 0a49 6465 6e74 6966 6965  .......Identifie
+00013040: 7207 0000 0010 5173 6369 4c65 7865 7256  r.....QsciLexerV
+00013050: 6572 696c 6f67 0103 0000 0030 0049 006e  erilog.....0.I.n
+00013060: 0061 006b 0074 0069 0076 0065 0072 0020  .a.k.t.i.v.e.r. 
+00013070: 0042 0061 006e 0067 0020 004b 006f 006d  .B.a.n.g. .K.o.m
+00013080: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
+00013090: 0006 0000 0015 496e 6163 7469 7665 2062  ......Inactive b
+000130a0: 616e 6720 636f 6d6d 656e 7407 0000 0010  ang comment.....
+000130b0: 5173 6369 4c65 7865 7256 6572 696c 6f67  QsciLexerVerilog
+000130c0: 0103 0000 0026 0049 006e 0061 006b 0074  .....&.I.n.a.k.t
+000130d0: 0069 0076 0065 0072 0020 004b 006f 006d  .i.v.e.r. .K.o.m
+000130e0: 006d 0065 006e 0074 0061 0072 0800 0000  .m.e.n.t.a.r....
+000130f0: 0006 0000 0010 496e 6163 7469 7665 2063  ......Inactive c
+00013100: 6f6d 6d65 6e74 0700 0000 1051 7363 694c  omment.....QsciL
+00013110: 6578 6572 5665 7269 6c6f 6701 0300 0000  exerVerilog.....
+00013120: 2400 4900 6e00 6100 6b00 7400 6900 7600  $.I.n.a.k.t.i.v.
+00013130: 6500 7200 2000 5300 7400 6100 6e00 6400  e.r. .S.t.a.n.d.
+00013140: 6100 7200 6408 0000 0000 0600 0000 1049  a.r.d..........I
+00013150: 6e61 6374 6976 6520 6465 6661 756c 7407  nactive default.
+00013160: 0000 0010 5173 6369 4c65 7865 7256 6572  ....QsciLexerVer
+00013170: 696c 6f67 0103 0000 0028 0049 006e 0061  ilog.....(.I.n.a
+00013180: 006b 0074 0069 0076 0065 0072 0020 0042  .k.t.i.v.e.r. .B
+00013190: 0065 007a 0065 0069 0063 0068 006e 0065  .e.z.e.i.c.h.n.e
+000131a0: 0072 0800 0000 0006 0000 0013 496e 6163  .r..........Inac
+000131b0: 7469 7665 2069 6465 6e74 6966 6965 7207  tive identifier.
+000131c0: 0000 0010 5173 6369 4c65 7865 7256 6572  ....QsciLexerVer
+000131d0: 696c 6f67 0103 0000 003c 0049 006e 0061  ilog.....<.I.n.a
+000131e0: 006b 0074 0069 0076 0065 0020 0045 0069  .k.t.i.v.e. .E.i
+000131f0: 006e 0067 0061 0062 0065 0070 006f 0072  .n.g.a.b.e.p.o.r
+00013200: 0074 0064 0065 0066 0069 006e 0069 0074  .t.d.e.f.i.n.i.t
+00013210: 0069 006f 006e 0800 0000 0006 0000 001f  .i.o.n..........
+00013220: 496e 6163 7469 7665 2069 6e70 7574 2070  Inactive input p
+00013230: 6f72 7420 6465 636c 6172 6174 696f 6e07  ort declaration.
+00013240: 0000 0010 5173 6369 4c65 7865 7256 6572  ....QsciLexerVer
+00013250: 696c 6f67 0103 0000 0046 0049 006e 0061  ilog.....F.I.n.a
+00013260: 006b 0074 0069 0076 0065 0020 0045 0069  .k.t.i.v.e. .E.i
+00013270: 006e 002d 002f 0041 0075 0073 0067 0061  .n.-./.A.u.s.g.a
+00013280: 0062 0065 0070 006f 0072 0074 0064 0065  .b.e.p.o.r.t.d.e
+00013290: 0066 0069 006e 0069 0074 0069 006f 006e  .f.i.n.i.t.i.o.n
+000132a0: 0800 0000 0006 0000 0026 496e 6163 7469  .........&Inacti
+000132b0: 7665 2069 6e70 7574 2f6f 7574 7075 7420  ve input/output 
+000132c0: 706f 7274 2064 6563 6c61 7261 7469 6f6e  port declaration
+000132d0: 0700 0000 1051 7363 694c 6578 6572 5665  .....QsciLexerVe
+000132e0: 7269 6c6f 6701 0300 0000 4000 4900 6e00  rilog.....@.I.n.
+000132f0: 6100 6b00 7400 6900 7600 6500 7200 2000  a.k.t.i.v.e.r. .
+00013300: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
+00013310: 6c00 7700 6f00 7200 7400 6b00 6f00 6d00  l.w.o.r.t.k.o.m.
+00013320: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+00013330: 0600 0000 1849 6e61 6374 6976 6520 6b65  .....Inactive ke
+00013340: 7977 6f72 6420 636f 6d6d 656e 7407 0000  yword comment...
+00013350: 0010 5173 6369 4c65 7865 7256 6572 696c  ..QsciLexerVeril
+00013360: 6f67 0103 0000 0032 0049 006e 0061 006b  og.....2.I.n.a.k
+00013370: 0074 0069 0076 0065 0072 0020 005a 0065  .t.i.v.e.r. .Z.e
+00013380: 0069 006c 0065 006e 006b 006f 006d 006d  .i.l.e.n.k.o.m.m
+00013390: 0065 006e 0074 0061 0072 0800 0000 0006  .e.n.t.a.r......
+000133a0: 0000 0015 496e 6163 7469 7665 206c 696e  ....Inactive lin
+000133b0: 6520 636f 6d6d 656e 7407 0000 0010 5173  e comment.....Qs
+000133c0: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
+000133d0: 0000 001a 0049 006e 0061 006b 0074 0069  .....I.n.a.k.t.i
+000133e0: 0076 0065 0020 005a 0061 0068 006c 0800  .v.e. .Z.a.h.l..
+000133f0: 0000 0006 0000 000f 496e 6163 7469 7665  ........Inactive
+00013400: 206e 756d 6265 7207 0000 0010 5173 6369   number.....Qsci
+00013410: 4c65 7865 7256 6572 696c 6f67 0103 0000  LexerVerilog....
+00013420: 0024 0049 006e 0061 006b 0074 0069 0076  .$.I.n.a.k.t.i.v
+00013430: 0065 0072 0020 004f 0070 0065 0072 0061  .e.r. .O.p.e.r.a
+00013440: 0074 006f 0072 0800 0000 0006 0000 0011  .t.o.r..........
+00013450: 496e 6163 7469 7665 206f 7065 7261 746f  Inactive operato
+00013460: 7207 0000 0010 5173 6369 4c65 7865 7256  r.....QsciLexerV
+00013470: 6572 696c 6f67 0103 0000 003c 0049 006e  erilog.....<.I.n
+00013480: 0061 006b 0074 0069 0076 0065 0020 0041  .a.k.t.i.v.e. .A
+00013490: 0075 0073 0067 0061 0062 0065 0070 006f  .u.s.g.a.b.e.p.o
+000134a0: 0072 0074 0064 0065 0066 0069 006e 0069  .r.t.d.e.f.i.n.i
+000134b0: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
+000134c0: 0020 496e 6163 7469 7665 206f 7574 7075  . Inactive outpu
+000134d0: 7420 706f 7274 2064 6563 6c61 7261 7469  t port declarati
+000134e0: 6f6e 0700 0000 1051 7363 694c 6578 6572  on.....QsciLexer
+000134f0: 5665 7269 6c6f 6701 0300 0000 2e00 4900  Verilog.......I.
+00013500: 6e00 6100 6b00 7400 6900 7600 6500 2000  n.a.k.t.i.v.e. .
+00013510: 5000 6f00 7200 7400 7600 6500 7200 6200  P.o.r.t.v.e.r.b.
+00013520: 6900 6e00 6400 7500 6e00 6708 0000 0000  i.n.d.u.n.g.....
+00013530: 0600 0000 1849 6e61 6374 6976 6520 706f  .....Inactive po
+00013540: 7274 2063 6f6e 6e65 6374 696f 6e07 0000  rt connection...
+00013550: 0010 5173 6369 4c65 7865 7256 6572 696c  ..QsciLexerVeril
+00013560: 6f67 0103 0000 0036 0049 006e 0061 006b  og.....6.I.n.a.k
+00013570: 0074 0069 0076 0065 0072 0020 0050 0072  .t.i.v.e.r. .P.r
+00013580: 00e4 0070 0072 006f 007a 0065 0073 0073  ...p.r.o.z.e.s.s
+00013590: 006f 0072 0062 006c 006f 0063 006b 0800  .o.r.b.l.o.c.k..
+000135a0: 0000 0006 0000 001b 496e 6163 7469 7665  ........Inactive
+000135b0: 2070 7265 7072 6f63 6573 736f 7220 626c   preprocessor bl
+000135c0: 6f63 6b07 0000 0010 5173 6369 4c65 7865  ock.....QsciLexe
+000135d0: 7256 6572 696c 6f67 0103 0000 005e 0049  rVerilog.....^.I
+000135e0: 006e 0061 006b 0074 0069 0076 0065 0020  .n.a.k.t.i.v.e. 
+000135f0: 0070 0072 0069 006d 00e4 0072 0065 0020  .p.r.i.m...r.e. 
+00013600: 0053 0063 0068 006c 0075 0073 0073 0065  .S.c.h.l.u.s.s.e
+00013610: 006c 0077 00f6 0072 0074 0065 0072 0020  .l.w...r.t.e.r. 
+00013620: 0075 006e 0064 0020 0042 0065 007a 0065  .u.n.d. .B.e.z.e
+00013630: 0069 0063 0068 006e 0065 0072 0800 0000  .i.c.h.n.e.r....
+00013640: 0006 0000 0029 496e 6163 7469 7665 2070  .....)Inactive p
+00013650: 7269 6d61 7279 206b 6579 776f 7264 7320  rimary keywords 
+00013660: 616e 6420 6964 656e 7469 6669 6572 7307  and identifiers.
+00013670: 0000 0010 5173 6369 4c65 7865 7256 6572  ....QsciLexerVer
+00013680: 696c 6f67 0103 0000 0062 0049 006e 0061  ilog.....b.I.n.a
+00013690: 006b 0074 0069 0076 0065 0020 0073 0065  .k.t.i.v.e. .s.e
+000136a0: 006b 0075 006e 0064 00e4 0072 0065 0020  .k.u.n.d...r.e. 
+000136b0: 0053 0063 0068 006c 0075 0073 0073 0065  .S.c.h.l.u.s.s.e
+000136c0: 006c 0077 00f6 0072 0074 0065 0072 0020  .l.w...r.t.e.r. 
+000136d0: 0075 006e 0064 0020 0042 0065 007a 0065  .u.n.d. .B.e.z.e
+000136e0: 0069 0063 0068 006e 0065 0072 0800 0000  .i.c.h.n.e.r....
+000136f0: 0006 0000 002b 496e 6163 7469 7665 2073  .....+Inactive s
+00013700: 6563 6f6e 6461 7279 206b 6579 776f 7264  econdary keyword
+00013710: 7320 616e 6420 6964 656e 7469 6669 6572  s and identifier
+00013720: 7307 0000 0010 5173 6369 4c65 7865 7256  s.....QsciLexerV
+00013730: 6572 696c 6f67 0103 0000 002a 0049 006e  erilog.....*.I.n
+00013740: 0061 006b 0074 0069 0076 0065 0020 005a  .a.k.t.i.v.e. .Z
+00013750: 0065 0069 0063 0068 0065 006e 006b 0065  .e.i.c.h.e.n.k.e
+00013760: 0074 0074 0065 0800 0000 0006 0000 000f  .t.t.e..........
+00013770: 496e 6163 7469 7665 2073 7472 696e 6707  Inactive string.
+00013780: 0000 0010 5173 6369 4c65 7865 7256 6572  ....QsciLexerVer
+00013790: 696c 6f67 0103 0000 0028 0049 006e 0061  ilog.....(.I.n.a
+000137a0: 006b 0074 0069 0076 0065 0072 0020 0053  .k.t.i.v.e.r. .S
+000137b0: 0079 0073 0074 0065 006d 0074 0061 0073  .y.s.t.e.m.t.a.s
+000137c0: 006b 0800 0000 0006 0000 0014 496e 6163  .k..........Inac
+000137d0: 7469 7665 2073 7973 7465 6d20 7461 736b  tive system task
+000137e0: 0700 0000 1051 7363 694c 6578 6572 5665  .....QsciLexerVe
+000137f0: 7269 6c6f 6701 0300 0000 4000 4900 6e00  rilog.....@.I.n.
+00013800: 6100 6b00 7400 6900 7600 6500 2000 7500  a.k.t.i.v.e. .u.
+00013810: 6e00 6200 6500 6500 6e00 6400 6500 7400  n.b.e.e.n.d.e.t.
+00013820: 6500 2000 5a00 6500 6900 6300 6800 6500  e. .Z.e.i.c.h.e.
+00013830: 6e00 6b00 6500 7400 7400 6508 0000 0000  n.k.e.t.t.e.....
+00013840: 0600 0000 1849 6e61 6374 6976 6520 756e  .....Inactive un
+00013850: 636c 6f73 6564 2073 7472 696e 6707 0000  closed string...
+00013860: 0010 5173 6369 4c65 7865 7256 6572 696c  ..QsciLexerVeril
+00013870: 6f67 0103 0000 005c 0049 006e 0061 006b  og.....\.I.n.a.k
+00013880: 0074 0069 0076 0065 0020 006e 0075 0074  .t.i.v.e. .n.u.t
+00013890: 007a 0065 0072 0064 0065 0066 0069 006e  .z.e.r.d.e.f.i.n
+000138a0: 0069 0065 0072 0074 0065 0020 0054 0061  .i.e.r.t.e. .T.a
+000138b0: 0073 006b 0073 0020 0075 006e 0064 0020  .s.k.s. .u.n.d. 
+000138c0: 0042 0065 007a 0065 0069 0063 0068 006e  .B.e.z.e.i.c.h.n
+000138d0: 0065 0072 0800 0000 0006 0000 002b 496e  .e.r.........+In
+000138e0: 6163 7469 7665 2075 7365 7220 6465 6669  active user defi
+000138f0: 6e65 6420 7461 736b 7320 616e 6420 6964  ned tasks and id
+00013900: 656e 7469 6669 6572 7307 0000 0010 5173  entifiers.....Qs
+00013910: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
+00013920: 0000 002a 0045 0069 006e 0067 0061 0062  ...*.E.i.n.g.a.b
+00013930: 0065 0070 006f 0072 0074 0064 0065 0066  .e.p.o.r.t.d.e.f
+00013940: 0069 006e 0069 0074 0069 006f 006e 0800  .i.n.i.t.i.o.n..
+00013950: 0000 0006 0000 0016 496e 7075 7420 706f  ........Input po
+00013960: 7274 2064 6563 6c61 7261 7469 6f6e 0700  rt declaration..
+00013970: 0000 1051 7363 694c 6578 6572 5665 7269  ...QsciLexerVeri
+00013980: 6c6f 6701 0300 0000 3400 4500 6900 6e00  log.....4.E.i.n.
+00013990: 2d00 2f00 4100 7500 7300 6700 6100 6200  -./.A.u.s.g.a.b.
+000139a0: 6500 7000 6f00 7200 7400 6400 6500 6600  e.p.o.r.t.d.e.f.
+000139b0: 6900 6e00 6900 7400 6900 6f00 6e08 0000  i.n.i.t.i.o.n...
+000139c0: 0000 0600 0000 1d49 6e70 7574 2f6f 7574  .......Input/out
+000139d0: 7075 7420 706f 7274 2064 6563 6c61 7261  put port declara
+000139e0: 7469 6f6e 0700 0000 1051 7363 694c 6578  tion.....QsciLex
+000139f0: 6572 5665 7269 6c6f 6701 0300 0000 2c00  erVerilog.....,.
+00013a00: 5300 6300 6800 6c00 fc00 7300 7300 6500  S.c.h.l...s.s.e.
+00013a10: 6c00 7700 6f00 7200 7400 6b00 6f00 6d00  l.w.o.r.t.k.o.m.
+00013a20: 6d00 6500 6e00 7400 6100 7208 0000 0000  m.e.n.t.a.r.....
+00013a30: 0600 0000 0f4b 6579 776f 7264 2063 6f6d  .....Keyword com
+00013a40: 6d65 6e74 0700 0000 1051 7363 694c 6578  ment.....QsciLex
+00013a50: 6572 5665 7269 6c6f 6701 0300 0000 1e00  erVerilog.......
+00013a60: 5a00 6500 6900 6c00 6500 6e00 6b00 6f00  Z.e.i.l.e.n.k.o.
+00013a70: 6d00 6d00 6500 6e00 7400 6100 7208 0000  m.m.e.n.t.a.r...
+00013a80: 0000 0600 0000 0c4c 696e 6520 636f 6d6d  .......Line comm
+00013a90: 656e 7407 0000 0010 5173 6369 4c65 7865  ent.....QsciLexe
+00013aa0: 7256 6572 696c 6f67 0103 0000 0008 005a  rVerilog.......Z
+00013ab0: 0061 0068 006c 0800 0000 0006 0000 0006  .a.h.l..........
+00013ac0: 4e75 6d62 6572 0700 0000 1051 7363 694c  Number.....QsciL
+00013ad0: 6578 6572 5665 7269 6c6f 6701 0300 0000  exerVerilog.....
+00013ae0: 1000 4f00 7000 6500 7200 6100 7400 6f00  ..O.p.e.r.a.t.o.
+00013af0: 7208 0000 0000 0600 0000 084f 7065 7261  r..........Opera
+00013b00: 746f 7207 0000 0010 5173 6369 4c65 7865  tor.....QsciLexe
+00013b10: 7256 6572 696c 6f67 0103 0000 002a 0041  rVerilog.....*.A
+00013b20: 0075 0073 0067 0061 0062 0065 0070 006f  .u.s.g.a.b.e.p.o
+00013b30: 0072 0074 0064 0065 0066 0069 006e 0069  .r.t.d.e.f.i.n.i
+00013b40: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
+00013b50: 0017 4f75 7470 7574 2070 6f72 7420 6465  ..Output port de
+00013b60: 636c 6172 6174 696f 6e07 0000 0010 5173  claration.....Qs
+00013b70: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
+00013b80: 0000 001c 0050 006f 0072 0074 0076 0065  .....P.o.r.t.v.e
+00013b90: 0072 0062 0069 006e 0064 0075 006e 0067  .r.b.i.n.d.u.n.g
+00013ba0: 0800 0000 0006 0000 000f 506f 7274 2063  ..........Port c
+00013bb0: 6f6e 6e65 6374 696f 6e07 0000 0010 5173  onnection.....Qs
+00013bc0: 6369 4c65 7865 7256 6572 696c 6f67 0103  ciLexerVerilog..
+00013bd0: 0000 0022 0050 0072 00e4 0070 0072 006f  ...".P.r...p.r.o
+00013be0: 007a 0065 0073 0073 006f 0072 0062 006c  .z.e.s.s.o.r.b.l
+00013bf0: 006f 0063 006b 0800 0000 0006 0000 0012  .o.c.k..........
+00013c00: 5072 6570 726f 6365 7373 6f72 2062 6c6f  Preprocessor blo
+00013c10: 636b 0700 0000 1051 7363 694c 6578 6572  ck.....QsciLexer
+00013c20: 5665 7269 6c6f 6701 0300 0000 4c00 5000  Verilog.....L.P.
+00013c30: 7200 6900 6d00 e400 7200 6500 2000 5300  r.i.m...r.e. .S.
+00013c40: 6300 6800 6c00 7500 7300 7300 6500 6c00  c.h.l.u.s.s.e.l.
+00013c50: 7700 f600 7200 7400 6500 7200 2000 7500  w...r.t.e.r. .u.
+00013c60: 6e00 6400 2000 4200 6500 7a00 6500 6900  n.d. .B.e.z.e.i.
+00013c70: 6300 6800 6e00 6500 7208 0000 0000 0600  c.h.n.e.r.......
+00013c80: 0000 2050 7269 6d61 7279 206b 6579 776f  .. Primary keywo
+00013c90: 7264 7320 616e 6420 6964 656e 7469 6669  rds and identifi
+00013ca0: 6572 7307 0000 0010 5173 6369 4c65 7865  ers.....QsciLexe
+00013cb0: 7256 6572 696c 6f67 0103 0000 0050 0053  rVerilog.....P.S
+00013cc0: 0065 006b 0075 006e 0064 00e4 0072 0065  .e.k.u.n.d...r.e
+00013cd0: 0020 0053 0063 0068 006c 0075 0073 0073  . .S.c.h.l.u.s.s
+00013ce0: 0065 006c 0077 00f6 0072 0074 0065 0072  .e.l.w...r.t.e.r
+00013cf0: 0020 0075 006e 0064 0020 0042 0065 007a  . .u.n.d. .B.e.z
+00013d00: 0065 0069 0063 0068 006e 0065 0072 0800  .e.i.c.h.n.e.r..
+00013d10: 0000 0006 0000 0022 5365 636f 6e64 6172  ......."Secondar
+00013d20: 7920 6b65 7977 6f72 6473 2061 6e64 2069  y keywords and i
+00013d30: 6465 6e74 6966 6965 7273 0700 0000 1051  dentifiers.....Q
+00013d40: 7363 694c 6578 6572 5665 7269 6c6f 6701  sciLexerVerilog.
+00013d50: 0300 0000 1800 5a00 6500 6900 6300 6800  ......Z.e.i.c.h.
+00013d60: 6500 6e00 6b00 6500 7400 7400 6508 0000  e.n.k.e.t.t.e...
+00013d70: 0000 0600 0000 0653 7472 696e 6707 0000  .......String...
+00013d80: 0010 5173 6369 4c65 7865 7256 6572 696c  ..QsciLexerVeril
+00013d90: 6f67 0103 0000 0014 0053 0079 0073 0074  og.......S.y.s.t
+00013da0: 0065 006d 0074 0061 0073 006b 0800 0000  .e.m.t.a.s.k....
+00013db0: 0006 0000 000b 5379 7374 656d 2074 6173  ......System tas
+00013dc0: 6b07 0000 0010 5173 6369 4c65 7865 7256  k.....QsciLexerV
+00013dd0: 6572 696c 6f67 0103 0000 002e 0055 006e  erilog.......U.n
+00013de0: 0062 0065 0065 006e 0064 0065 0074 0065  .b.e.e.n.d.e.t.e
+00013df0: 0020 005a 0065 0069 0063 0068 0065 006e  . .Z.e.i.c.h.e.n
+00013e00: 006b 0065 0074 0074 0065 0800 0000 0006  .k.e.t.t.e......
+00013e10: 0000 000f 556e 636c 6f73 6564 2073 7472  ....Unclosed str
+00013e20: 696e 6707 0000 0010 5173 6369 4c65 7865  ing.....QsciLexe
+00013e30: 7256 6572 696c 6f67 0103 0000 004a 004e  rVerilog.....J.N
+00013e40: 0075 0074 007a 0065 0072 0064 0065 0066  .u.t.z.e.r.d.e.f
+00013e50: 0069 006e 0069 0065 0072 0074 0065 0020  .i.n.i.e.r.t.e. 
+00013e60: 0054 0061 0073 006b 0073 0020 0075 006e  .T.a.s.k.s. .u.n
+00013e70: 0064 0020 0042 0065 007a 0065 0069 0063  .d. .B.e.z.e.i.c
+00013e80: 0068 006e 0065 0072 0800 0000 0006 0000  .h.n.e.r........
+00013e90: 0022 5573 6572 2064 6566 696e 6564 2074  ."User defined t
+00013ea0: 6173 6b73 2061 6e64 2069 6465 6e74 6966  asks and identif
+00013eb0: 6965 7273 0700 0000 1051 7363 694c 6578  iers.....QsciLex
+00013ec0: 6572 5665 7269 6c6f 6701 0300 0000 1200  erVerilog.......
+00013ed0: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
+00013ee0: 7208 0000 0000 0600 0000 0743 6f6d 6d65  r..........Comme
+00013ef0: 6e74 0700 0000 0d51 7363 694c 6578 6572  nt.....QsciLexer
+00013f00: 5941 4d4c 0103 0000 0010 0053 0074 0061  YAML.......S.t.a
+00013f10: 006e 0064 0061 0072 0064 0800 0000 0006  .n.d.a.r.d......
+00013f20: 0000 0007 4465 6661 756c 7407 0000 000d  ....Default.....
+00013f30: 5173 6369 4c65 7865 7259 414d 4c01 0300  QsciLexerYAML...
+00013f40: 0000 2200 4400 6f00 6b00 7500 6d00 6500  ..".D.o.k.u.m.e.
+00013f50: 6e00 7400 6200 6500 6700 7200 6500 6e00  n.t.b.e.g.r.e.n.
+00013f60: 7a00 6500 7208 0000 0000 0600 0000 1244  z.e.r..........D
+00013f70: 6f63 756d 656e 7420 6465 6c69 6d69 7465  ocument delimite
+00013f80: 7207 0000 000d 5173 6369 4c65 7865 7259  r.....QsciLexerY
+00013f90: 414d 4c01 0300 0000 1400 4200 6500 7a00  AML.......B.e.z.
+00013fa0: 6500 6900 6300 6800 6e00 6500 7208 0000  e.i.c.h.n.e.r...
+00013fb0: 0000 0600 0000 0a49 6465 6e74 6966 6965  .......Identifie
+00013fc0: 7207 0000 000d 5173 6369 4c65 7865 7259  r.....QsciLexerY
+00013fd0: 414d 4c01 0300 0000 1a00 5300 6300 6800  AML.......S.c.h.
+00013fe0: 6c00 fc00 7300 7300 6500 6c00 7700 6f00  l...s.s.e.l.w.o.
+00013ff0: 7200 7408 0000 0000 0600 0000 074b 6579  r.t..........Key
+00014000: 776f 7264 0700 0000 0d51 7363 694c 6578  word.....QsciLex
+00014010: 6572 5941 4d4c 0103 0000 0008 005a 0061  erYAML.......Z.a
+00014020: 0068 006c 0800 0000 0006 0000 0006 4e75  .h.l..........Nu
+00014030: 6d62 6572 0700 0000 0d51 7363 694c 6578  mber.....QsciLex
+00014040: 6572 5941 4d4c 0103 0000 0010 004f 0070  erYAML.......O.p
+00014050: 0065 0072 0061 0074 006f 0072 0800 0000  .e.r.a.t.o.r....
+00014060: 0006 0000 0008 4f70 6572 6174 6f72 0700  ......Operator..
+00014070: 0000 0d51 7363 694c 6578 6572 5941 4d4c  ...QsciLexerYAML
+00014080: 0103 0000 0010 0052 0065 0066 0065 0072  .......R.e.f.e.r
+00014090: 0065 006e 007a 0800 0000 0006 0000 0009  .e.n.z..........
+000140a0: 5265 6665 7265 6e63 6507 0000 000d 5173  Reference.....Qs
+000140b0: 6369 4c65 7865 7259 414d 4c01 0300 0000  ciLexerYAML.....
+000140c0: 2e00 5300 7900 6e00 7400 6100 7800 6600  ..S.y.n.t.a.x.f.
+000140d0: 6500 6800 6c00 6500 7200 2000 4d00 6100  e.h.l.e.r. .M.a.
+000140e0: 7200 6b00 6900 6500 7200 7500 6e00 6708  r.k.i.e.r.u.n.g.
+000140f0: 0000 0000 0600 0000 1353 796e 7461 7820  .........Syntax 
+00014100: 6572 726f 7220 6d61 726b 6572 0700 0000  error marker....
+00014110: 0d51 7363 694c 6578 6572 5941 4d4c 0103  .QsciLexerYAML..
+00014120: 0000 0028 0054 0065 0078 0074 0062 006c  ...(.T.e.x.t.b.l
+00014130: 006f 0063 006b 0020 004d 0061 0072 006b  .o.c.k. .M.a.r.k
+00014140: 0069 0065 0072 0075 006e 0067 0800 0000  .i.e.r.u.n.g....
+00014150: 0006 0000 0011 5465 7874 2062 6c6f 636b  ......Text block
+00014160: 206d 6172 6b65 7207 0000 000d 5173 6369   marker.....Qsci
+00014170: 4c65 7865 7259 414d 4c01 0300 0000 1200  LexerYAML.......
+00014180: 2600 4b00 6f00 7000 6900 6500 7200 6500  &.K.o.p.i.e.r.e.
+00014190: 6e08 0000 0000 0600 0000 0526 436f 7079  n..........&Copy
+000141a0: 0700 0000 0d51 7363 6953 6369 6e74 696c  .....QsciScintil
+000141b0: 6c61 0103 0000 0012 0045 0069 006e 0026  la.......E.i.n.&
+000141c0: 0066 00fc 0067 0065 006e 0800 0000 0006  .f...g.e.n......
+000141d0: 0000 0006 2650 6173 7465 0700 0000 0d51  ....&Paste.....Q
+000141e0: 7363 6953 6369 6e74 696c 6c61 0103 0000  sciScintilla....
+000141f0: 0022 0057 0069 0065 0064 0065 0072 0026  .".W.i.e.d.e.r.&
+00014200: 0068 0065 0072 0073 0074 0065 006c 006c  .h.e.r.s.t.e.l.l
+00014210: 0065 006e 0800 0000 0006 0000 0005 2652  .e.n..........&R
+00014220: 6564 6f07 0000 000d 5173 6369 5363 696e  edo.....QsciScin
+00014230: 7469 6c6c 6101 0300 0000 1600 2600 5200  tilla.......&.R.
+00014240: fc00 6300 6b00 6700 e400 6e00 6700 6900  ..c.k.g...n.g.i.
+00014250: 6708 0000 0000 0600 0000 0526 556e 646f  g..........&Undo
+00014260: 0700 0000 0d51 7363 6953 6369 6e74 696c  .....QsciScintil
+00014270: 6c61 0103 0000 001a 0026 0041 0075 0073  la.......&.A.u.s
+00014280: 0073 0063 0068 006e 0065 0069 0064 0065  .s.c.h.n.e.i.d.e
+00014290: 006e 0800 0000 0006 0000 0004 4375 2674  .n..........Cu&t
+000142a0: 0700 0000 0d51 7363 6953 6369 6e74 696c  .....QsciScintil
+000142b0: 6c61 0103 0000 000e 004c 00f6 0073 0063  la.......L...s.c
+000142c0: 0068 0065 006e 0800 0000 0006 0000 0006  .h.e.n..........
+000142d0: 4465 6c65 7465 0700 0000 0d51 7363 6953  Delete.....QsciS
+000142e0: 6369 6e74 696c 6c61 0103 0000 001c 0041  cintilla.......A
+000142f0: 006c 006c 0065 0020 0061 0075 0073 0077  .l.l.e. .a.u.s.w
+00014300: 00e4 0068 006c 0065 006e 0800 0000 0006  ...h.l.e.n......
+00014310: 0000 000a 5365 6c65 6374 2041 6c6c 0700  ....Select All..
+00014320: 0000 0d51 7363 6953 6369 6e74 696c 6c61  ...QsciScintilla
+00014330: 0188 0000 0002 0101                      ........
```

### Comparing `PyQt6_QScintilla-2.13.4/src/qscintilla_es.qm` & `PyQt6_QScintilla-2.14.0/src/qscintilla_es.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscintilla_fr.qm` & `PyQt6_QScintilla-2.14.0/src/qscintilla_fr.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscintilla_pt_br.qm` & `PyQt6_QScintilla-2.14.0/src/qscintilla_pt_br.qm`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qsciprinter.cpp` & `PyQt6_QScintilla-2.14.0/src/qsciprinter.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qsciscintilla.cpp` & `PyQt6_QScintilla-2.14.0/src/qsciscintilla.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -386,16 +386,16 @@
             if (shift < sh)
                 shift = sh;
         }
 
         ct = ct_entries.join("\n");
     }
 
-    ScintillaBytes ct_bytes = textAsBytes(ct);
-    const char *cts = ScintillaBytesConstData(ct_bytes);
+    QByteArray ct_bytes = textAsBytes(ct);
+    const char *cts = ct_bytes.constData();
 
     SendScintilla(SCI_CALLTIPSHOW, adjustedCallTipPosition(shift), cts);
 
     // Done if there is more than one call tip.
     if (nr_entries > 1)
         return;
 
@@ -466,18 +466,16 @@
     // Add the arrows.
     if (ct_cursor < nr_entries - 1)
         ct.prepend('\002');
 
     if (ct_cursor > 0)
         ct.prepend('\001');
 
-    ScintillaBytes ct_bytes = textAsBytes(ct);
-    const char *cts = ScintillaBytesConstData(ct_bytes);
-
-    SendScintilla(SCI_CALLTIPSHOW, adjustedCallTipPosition(shift), cts);
+    SendScintilla(SCI_CALLTIPSHOW, adjustedCallTipPosition(shift),
+            textAsBytes(ct).constData());
 }
 
 
 // Shift the position of the call tip (to take any context into account) but
 // don't go before the start of the line.
 int QsciScintilla::adjustedCallTipPosition(int ctshift) const
 {
@@ -672,16 +670,16 @@
     QStringList context = apiContext(SendScintilla(SCI_GETCURRENTPOS), start,
             ignore);
 
     if (context.isEmpty())
         return;
 
     // Get the last word's raw data and length.
-    ScintillaBytes s = textAsBytes(context.last());
-    const char *last_data = ScintillaBytesConstData(s);
+    QByteArray s = textAsBytes(context.last());
+    const char *last_data = s.constData();
     int last_len = s.length();
 
     if (checkThresh && last_len < acThresh)
         return;
 
     // Generate the string representing the valid words to select from.
     QStringList wlist;
@@ -773,16 +771,16 @@
         return;
 
     wlist.sort();
 
     SendScintilla(SCI_AUTOCSETCHOOSESINGLE, choose_single);
     SendScintilla(SCI_AUTOCSETSEPARATOR, acSeparator);
 
-    ScintillaBytes wlist_s = textAsBytes(wlist.join(QChar(acSeparator)));
-    SendScintilla(SCI_AUTOCSHOW, last_len, ScintillaBytesConstData(wlist_s));
+    SendScintilla(SCI_AUTOCSHOW, last_len,
+            textAsBytes(wlist.join(QChar(acSeparator))).constData());
 }
 
 
 // Maintain the indentation of the previous line.
 void QsciScintilla::maintainIndentation(char ch, long pos)
 {
     if (ch != '\r' && ch != '\n')
@@ -1879,18 +1877,17 @@
 {
     if (findState.startpos == findState.endpos)
         return -1;
 
     SendScintilla(SCI_SETTARGETSTART, findState.startpos);
     SendScintilla(SCI_SETTARGETEND, findState.endpos);
 
-    ScintillaBytes s = textAsBytes(findState.expr);
+    QByteArray s = textAsBytes(findState.expr);
 
-    return SendScintilla(SCI_SEARCHINTARGET, s.length(),
-            ScintillaBytesConstData(s));
+    return SendScintilla(SCI_SEARCHINTARGET, s.length(), s.constData());
 }
 
 
 // Replace the text found with the previous find method.
 void QsciScintilla::replace(const QString &replaceStr)
 {
     if (findState.status == FindState::Idle)
@@ -1899,16 +1896,15 @@
     long start = SendScintilla(SCI_GETSELECTIONSTART);
     long orig_len = SendScintilla(SCI_GETSELECTIONEND) - start;
 
     SendScintilla(SCI_TARGETFROMSELECTION);
 
     int cmd = (findState.flags & SCFIND_REGEXP) ? SCI_REPLACETARGETRE : SCI_REPLACETARGET;
 
-    ScintillaBytes s = textAsBytes(replaceStr);
-    long len = SendScintilla(cmd, -1, ScintillaBytesConstData(s));
+    long len = SendScintilla(cmd, -1, textAsBytes(replaceStr).constData());
 
     // Reset the selection.
     SendScintilla(SCI_SETSELECTIONSTART, start);
     SendScintilla(SCI_SETSELECTIONEND, start + len);
 
     // Fix the original selection.
     findState.endpos_orig += (len - orig_len);
@@ -2182,16 +2178,16 @@
 
 
 // Append the given text.
 void QsciScintilla::append(const QString &text)
 {
     bool ro = ensureRW();
 
-    ScintillaBytes s = textAsBytes(text);
-    SendScintilla(SCI_APPENDTEXT, s.length(), ScintillaBytesConstData(s));
+    QByteArray s = textAsBytes(text);
+    SendScintilla(SCI_APPENDTEXT, s.length(), s.constData());
 
     SendScintilla(SCI_EMPTYUNDOBUFFER);
 
     setReadOnly(ro);
 }
 
 
@@ -2211,16 +2207,15 @@
 
 // Insert the given text at the given position.
 void QsciScintilla::insertAtPos(const QString &text, int pos)
 {
     bool ro = ensureRW();
 
     SendScintilla(SCI_BEGINUNDOACTION);
-    SendScintilla(SCI_INSERTTEXT, pos,
-            ScintillaBytesConstData(textAsBytes(text)));
+    SendScintilla(SCI_INSERTTEXT, pos, textAsBytes(text).constData());
     SendScintilla(SCI_ENDUNDOACTION);
 
     setReadOnly(ro);
 }
 
 
 // Begin a sequence of undoable actions.
@@ -2307,76 +2302,79 @@
     SendScintilla(SCI_REPLACESEL, "");
 }
 
 
 // Replace any selected text.
 void QsciScintilla::replaceSelectedText(const QString &text)
 {
-    SendScintilla(SCI_REPLACESEL, ScintillaBytesConstData(textAsBytes(text)));
+    SendScintilla(SCI_REPLACESEL, textAsBytes(text).constData());
 }
 
 
 // Return the current selected text.
 QString QsciScintilla::selectedText() const
 {
     if (!selText)
         return QString();
 
-    char *buf = new char[SendScintilla(SCI_GETSELECTIONEND) - SendScintilla(SCI_GETSELECTIONSTART) + 1];
+    int size = SendScintilla(SCI_GETSELECTIONEND) - SendScintilla(SCI_GETSELECTIONSTART);
+    char *buf = new char[size + 1];
 
     SendScintilla(SCI_GETSELTEXT, buf);
 
-    QString qs = bytesAsText(buf);
+    QString qs = bytesAsText(buf, size);
     delete[] buf;
 
     return qs;
 }
 
 
 // Return the current text.
 QString QsciScintilla::text() const
 {
-    int buflen = length() + 1;
-    char *buf = new char[buflen];
+    int size = length();
+    char *buf = new char[size + 1];
 
-    SendScintilla(SCI_GETTEXT, buflen, buf);
+    // Note that the docs seem to be wrong and we need to ask for the length
+    // plus the '\0'.
+    SendScintilla(SCI_GETTEXT, size + 1, buf);
 
-    QString qs = bytesAsText(buf);
+    QString qs = bytesAsText(buf, size);
     delete[] buf;
 
     return qs;
 }
 
 
 // Return the text of a line.
 QString QsciScintilla::text(int line) const
 {
-    int line_len = lineLength(line);
+    int size = lineLength(line);
 
-    if (line_len < 1)
+    if (size < 1)
         return QString();
 
-    char *buf = new char[line_len + 1];
+    char *buf = new char[size];
 
     SendScintilla(SCI_GETLINE, line, buf);
-    buf[line_len] = '\0';
 
-    QString qs = bytesAsText(buf);
+    QString qs = bytesAsText(buf, size);
     delete[] buf;
 
     return qs;
 }
 
 
 // Return the text between two positions.
 QString QsciScintilla::text(int start, int end) const
 {
-    char *buf = new char[end - start + 1];
+    int size = end - start;
+    char *buf = new char[size + 1];
     SendScintilla(SCI_GETTEXTRANGE, start, end, buf);
-    QString text = bytesAsText(buf);
+    QString text = bytesAsText(buf, size);
     delete[] buf;
 
     return text;
 }
 
 
 // Return the text as encoded bytes between two positions.
@@ -2391,15 +2389,17 @@
 
 
 // Set the given text.
 void QsciScintilla::setText(const QString &text)
 {
     bool ro = ensureRW();
 
-    SendScintilla(SCI_SETTEXT, ScintillaBytesConstData(textAsBytes(text)));
+    SendScintilla(SCI_CLEARALL);
+    QByteArray bytes = textAsBytes(text);
+    SendScintilla(SCI_ADDTEXT, bytes.size(), bytes.constData());
     SendScintilla(SCI_EMPTYUNDOBUFFER);
 
     setReadOnly(ro);
 }
 
 
 // Get the cursor position
@@ -2702,17 +2702,15 @@
 
 
 // Annotate a line.
 void QsciScintilla::setMarginText(int line, const QString &text, int style)
 {
     int style_offset = SendScintilla(SCI_MARGINGETSTYLEOFFSET);
 
-    SendScintilla(SCI_MARGINSETTEXT, line,
-            ScintillaBytesConstData(textAsBytes(text)));
-
+    SendScintilla(SCI_MARGINSETTEXT, line, textAsBytes(text).constData());
     SendScintilla(SCI_MARGINSETSTYLE, line, style - style_offset);
 }
 
 
 // Annotate a line.
 void QsciScintilla::setMarginText(int line, const QString &text, const QsciStyle &style)
 {
@@ -2731,19 +2729,18 @@
 }
 
 
 // Annotate a line.
 void QsciScintilla::setMarginText(int line, const QList<QsciStyledText> &text)
 {
     char *styles;
-    ScintillaBytes styled_text = styleText(text, &styles,
+    QByteArray styled_text = styleText(text, &styles,
             SendScintilla(SCI_MARGINGETSTYLEOFFSET));
 
-    SendScintilla(SCI_MARGINSETTEXT, line,
-            ScintillaBytesConstData(styled_text));
+    SendScintilla(SCI_MARGINSETTEXT, line, styled_text.constData());
     SendScintilla(SCI_MARGINSETSTYLES, line, styles);
 
     delete[] styles;
 }
 
 
 // Return the state of line numbers in a margin.
@@ -2803,15 +2800,15 @@
 }
 
 
 // Set the width of a margin to the width of some text.
 void QsciScintilla::setMarginWidth(int margin, const QString &s)
 {
     int width = SendScintilla(SCI_TEXTWIDTH, STYLE_LINENUMBER,
-            ScintillaBytesConstData(textAsBytes(s)));
+            textAsBytes(s).constData());
 
     setMarginWidth(margin, width);
 }
 
 
 // Set the background colour of all margins.
 void QsciScintilla::setMarginsBackgroundColor(const QColor &col)
@@ -4054,16 +4051,16 @@
 {
     // Sanity check to make sure auto-completion doesn't get confused.
     if (id <= 0)
         return;
 
     SendScintilla(SCI_AUTOCSETSEPARATOR, userSeparator);
 
-    ScintillaBytes s = textAsBytes(list.join(QChar(userSeparator)));
-    SendScintilla(SCI_USERLISTSHOW, id, ScintillaBytesConstData(s));
+    SendScintilla(SCI_USERLISTSHOW, id,
+            textAsBytes(list.join(QChar(userSeparator))).constData());
 }
 
 
 // Translate the SCN_USERLISTSELECTION notification into something more useful.
 void QsciScintilla::handleUserListSelection(const char *text, int id)
 {
     emit userListActivated(id, QString(text));
@@ -4225,17 +4222,15 @@
 
 
 // Annotate a line.
 void QsciScintilla::annotate(int line, const QString &text, int style)
 {
     int style_offset = SendScintilla(SCI_ANNOTATIONGETSTYLEOFFSET);
 
-    ScintillaBytes s = textAsBytes(text);
-
-    SendScintilla(SCI_ANNOTATIONSETTEXT, line, ScintillaBytesConstData(s));
+    SendScintilla(SCI_ANNOTATIONSETTEXT, line, textAsBytes(text).constData());
     SendScintilla(SCI_ANNOTATIONSETSTYLE, line, style - style_offset);
 
     setScrollBars();
 }
 
 
 // Annotate a line.
@@ -4256,64 +4251,63 @@
 }
 
 
 // Annotate a line.
 void QsciScintilla::annotate(int line, const QList<QsciStyledText> &text)
 {
     char *styles;
-    ScintillaBytes styled_text = styleText(text, &styles,
+    QByteArray styled_text = styleText(text, &styles,
             SendScintilla(SCI_ANNOTATIONGETSTYLEOFFSET));
 
-    SendScintilla(SCI_ANNOTATIONSETTEXT, line,
-            ScintillaBytesConstData(styled_text));
+    SendScintilla(SCI_ANNOTATIONSETTEXT, line, styled_text.constData());
     SendScintilla(SCI_ANNOTATIONSETSTYLES, line, styles);
 
     delete[] styles;
 }
 
 
 // Get the annotation for a line, if any.
 QString QsciScintilla::annotation(int line) const
 {
-    char *buf = new char[SendScintilla(SCI_ANNOTATIONGETTEXT, line, (const char *)0) + 1];
-
-    buf[SendScintilla(SCI_ANNOTATIONGETTEXT, line, buf)] = '\0';
+    int size = SendScintilla(SCI_ANNOTATIONGETTEXT, line, (const char *)0);
+    char *buf = new char[size + 1];
 
-    QString qs = bytesAsText(buf);
+    QString qs = bytesAsText(buf, size);
     delete[] buf;
 
     return qs;
 }
 
 
 // Convert a list of styled text to the low-level arrays.
-QsciScintillaBase::ScintillaBytes QsciScintilla::styleText(const QList<QsciStyledText> &styled_text, char **styles, int style_offset)
+QByteArray QsciScintilla::styleText(const QList<QsciStyledText> &styled_text,
+        char **styles, int style_offset)
 {
     QString text;
     int i;
 
     // Build the full text.
     for (i = 0; i < styled_text.count(); ++i)
     {
         const QsciStyledText &st = styled_text[i];
 
         st.apply(this);
 
         text.append(st.text());
     }
 
-    ScintillaBytes s = textAsBytes(text);
+    QByteArray s = textAsBytes(text);
 
     // There is a style byte for every byte.
     char *sp = *styles = new char[s.length()];
 
     for (i = 0; i < styled_text.count(); ++i)
     {
         const QsciStyledText &st = styled_text[i];
-        ScintillaBytes part = textAsBytes(st.text());
+        QByteArray part = textAsBytes(st.text());
         int part_length = part.length();
 
         for (int c = 0; c < part_length; ++c)
             *sp++ = (char)(st.style() - style_offset);
     }
 
     return s;
```

### Comparing `PyQt6_QScintilla-2.13.4/src/qsciscintillabase.cpp` & `PyQt6_QScintilla-2.14.0/src/qsciscintillabase.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,15 @@
         }
     }
 
     QString text = e->text();
 
     if (!text.isEmpty() && text[0].isPrint())
     {
-        ScintillaBytes bytes = textAsBytes(text);
+        QByteArray bytes = textAsBytes(text);
         sci->AddCharUTF(bytes.data(), bytes.length());
         e->accept();
     }
     else
     {
         QAbstractScrollArea::keyPressEvent(e);
     }
@@ -488,30 +488,30 @@
     }
 
     return key;
 }
 
 
 // Encode a QString as bytes.
-QsciScintillaBase::ScintillaBytes QsciScintillaBase::textAsBytes(const QString &text) const
+QByteArray QsciScintillaBase::textAsBytes(const QString &text) const
 {
     if (sci->IsUnicodeMode())
         return text.toUtf8();
 
     return text.toLatin1();
 }
 
 
 // Decode bytes as a QString.
-QString QsciScintillaBase::bytesAsText(const char *bytes) const
+QString QsciScintillaBase::bytesAsText(const char *bytes, int size) const
 {
     if (sci->IsUnicodeMode())
-        return QString::fromUtf8(bytes);
+        return QString::fromUtf8(bytes, size);
 
-    return QString::fromLatin1(bytes);
+    return QString::fromLatin1(bytes, size);
 }
 
 
 // Handle a mouse button double click.
 void QsciScintillaBase::mouseDoubleClickEvent(QMouseEvent *e)
 {
     if (e->button() != Qt::LeftButton)
```

### Comparing `PyQt6_QScintilla-2.13.4/src/qscistyle.cpp` & `PyQt6_QScintilla-2.14.0/src/qscistyle.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6_QScintilla-2.13.4/src/qscistyledtext.cpp` & `PyQt6_QScintilla-2.14.0/src/qscistyledtext.cpp`

 * *Files identical despite different names*

