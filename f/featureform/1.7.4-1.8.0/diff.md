# Comparing `tmp/featureform-1.7.4.tar.gz` & `tmp/featureform-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featureform-1.7.4.tar", last modified: Wed Apr 26 21:20:25 2023, max compression
+gzip compressed data, was "featureform-1.8.0.tar", last modified: Mon May  1 21:15:27 2023, max compression
```

## Comparing `featureform-1.7.4.tar` & `featureform-1.8.0.tar`

### file list

```diff
@@ -1,367 +1,368 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.870674 featureform-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-26 21:19:01.000000 featureform-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 21:19:01.000000 featureform-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 21:20:25.870674 featureform-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-26 21:19:01.000000 featureform-1.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 21:19:01.000000 featureform-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 21:20:25.870674 featureform-1.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/featureform/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/[type]/[entity].html
--rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/[type].html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/featureform/dashboard/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.818674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.850674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
--rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
--rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
--rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
--rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
--rw-r--r--   0 runner    (1001) docker     (123)  3583019 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
--rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
--rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
--rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
--rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.854674 featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/connections.html
--rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.866675 featureform-1.7.4/src/featureform/dashboard/out/static/
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Capital_One_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Kubernetes_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Postgresql_elephant.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Redis_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/Snowflake_Logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/amazon_redshift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/amazon_s3.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/apache_cassandra.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/apache_hadoop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/azure_storage_accounts.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/google_bigquery.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/google_cloud_storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/google_firestore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/mongoDB.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-26 21:20:19.000000 featureform-1.7.4/src/featureform/dashboard/out/static/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/dashboard_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    16410 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/get_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/get_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/list_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    89285 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local_dash_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/local_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.866675 featureform-1.7.4/src/featureform/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-26 21:19:43.000000 featureform-1.7.4/src/featureform/proto/metadata.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-04-26 21:19:45.000000 featureform-1.7.4/src/featureform/proto/metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-04-26 21:19:45.000000 featureform-1.7.4/src/featureform/proto/metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-26 21:19:43.000000 featureform-1.7.4/src/featureform/proto/serving.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-26 21:19:44.000000 featureform-1.7.4/src/featureform/proto/serving_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-26 21:19:44.000000 featureform-1.7.4/src/featureform/proto/serving_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   166823 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/register_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    56884 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/search_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/serving.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/serving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/sqlite_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/type_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:19:01.000000 featureform-1.7.4/src/featureform/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.822674 featureform-1.7.4/src/featureform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32977 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 21:20:25.000000 featureform-1.7.4/src/featureform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:20:25.870674 featureform-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_class_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_executor_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_getting_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_localmode_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_localmode_include_label_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_localmode_lag_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_ondemand_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_resource_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_serving_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_source_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_spark_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_tags_and_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 21:19:01.000000 featureform-1.7.4/tests/test_updating_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.333976 featureform-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-01 21:13:34.000000 featureform-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 21:13:34.000000 featureform-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 21:15:27.333976 featureform-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-01 21:13:34.000000 featureform-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-01 21:13:34.000000 featureform-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-01 21:15:27.333976 featureform-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.257973 featureform-1.8.0/src/featureform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/featureform/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/[type]/[entity].html
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/[type].html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/featureform/dashboard/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.249973 featureform-1.8.0/src/featureform/dashboard/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.313975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    83561 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74481 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   201393 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130270 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   104027 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/404-baaca4b2f4acc755.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]/[entity]-b07f3c4463890639.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/[type]-751a928da9d524e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3583019 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/_error-3f70f2d61eb8c6dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/connections-1d67ba61869dece6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/search-175858e61ba25631.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/
+-rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arff.ab502da8667e6dc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bnf.d1d39a9bd6ac45b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brainfuck.42d8625dbbdd27ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_editorconfig.17a13e6bcda1e1f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gcode.ac01f4f7ac16a003.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_git.0e0594706d30fbd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hpkp.2b3348708365f9ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hsts.5e3fe34e0eab5fdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsonp.5d313969242bf8d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16942 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nand2tetrisHdl.bd5b619f107eee8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_prolog.22a1c7ff76f01643.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_properties.c3ce1ad33d9983e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33525 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14361 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xmlDoc.3eb6beae8084d868.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yang.28bbfbd268843c68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/css/85a2addfd2efc882.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    81048 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.321975 featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/connections.html
+-rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.329976 featureform-1.8.0/src/featureform/dashboard/out/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Capital_One_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Kubernetes_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Postgresql_elephant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Redis_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61862 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/Snowflake_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/amazon_redshift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/amazon_s3.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26573 2023-05-01 21:15:19.000000 featureform-1.8.0/src/featureform/dashboard/out/static/apache_cassandra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60161 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/apache_hadoop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/azure_storage_accounts.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/google_bigquery.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/google_cloud_storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/google_firestore.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/mongoDB.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 21:15:20.000000 featureform-1.8.0/src/featureform/dashboard/out/static/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17938 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/dashboard_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/get_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/get_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/list_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89279 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local_dash_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/local_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.329976 featureform-1.8.0/src/featureform/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-05-01 21:14:32.000000 featureform-1.8.0/src/featureform/proto/metadata.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102266 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-01 21:14:32.000000 featureform-1.8.0/src/featureform/proto/serving.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/serving_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-01 21:14:33.000000 featureform-1.8.0/src/featureform/proto/serving_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159624 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17986 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/register_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58803 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/search_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34805 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/serving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29384 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/sqlite_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/type_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-01 21:13:34.000000 featureform-1.8.0/src/featureform/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.261973 featureform-1.8.0/src/featureform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33006 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 21:15:27.000000 featureform-1.8.0/src/featureform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:15:27.333976 featureform-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_class_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_executor_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_getting_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_localmode_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_localmode_include_label_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_localmode_lag_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_ondemand_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_resource_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15831 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_serving_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_source_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_spark_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30091 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_tags_and_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-01 21:13:34.000000 featureform-1.8.0/tests/test_updating_provider.py
```

### Comparing `featureform-1.7.4/LICENSE` & `featureform-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/PKG-INFO` & `featureform-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.7.4
+Version: 1.8.0
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.7.4/README.md` & `featureform-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/setup.cfg` & `featureform-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = featureform
-version = 1.7.4
+version = 1.8.0
 author = FeatureForm, Inc.
 author_email = hello@featureform.com
 description = Package for the Featureform Feature Store
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://featureform.com
 project_urls =
```

### Comparing `featureform-1.7.4/src/featureform/__init__.py` & `featureform-1.8.0/src/featureform/__init__.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/cli.py` & `featureform-1.8.0/src/featureform/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,66 +16,65 @@
     "feature",
     "source",
     "training-set",
     "label",
     "entity",
     "provider",
     "model",
-    "user"
+    "user",
 ]
 
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
+    # fmt: off
     """
     \b
     ______         _                   __                     
     |  ___|       | |                 / _|                    
     | |_ ___  __ _| |_ _   _ _ __ ___| |_ ___  _ __ _ __ ___  
     |  _/ _ \/ _` | __| | | | '__/ _ \  _/ _ \| '__| '_ ` _ \ 
     | ||  __/ (_| | |_| |_| | | |  __/ || (_) | |  | | | | | |
     \_| \___|\__,_|\__|\__,_|_|  \___|_| \___/|_|  |_| |_| |_|
 
     Interact with Featureform's Feature Store via the official command line interface.
     """
+    # fmt: on
     pass
 
 
 @cli.command()
-@click.option("--host",
-              "host",
-              required=False,
-              help="The host address of the API server to connect to")
-@click.option("--cert",
-              "cert",
-              required=False,
-              help="Path to self-signed TLS certificate")
-@click.option("--insecure",
-              is_flag=True,
-              help="Disables TLS verification")
-@click.option("--local",
-              is_flag=True,
-              help="Enables local mode")
+@click.option(
+    "--host",
+    "host",
+    required=False,
+    help="The host address of the API server to connect to",
+)
+@click.option(
+    "--cert", "cert", required=False, help="Path to self-signed TLS certificate"
+)
+@click.option("--insecure", is_flag=True, help="Disables TLS verification")
+@click.option("--local", is_flag=True, help="Enables local mode")
 @click.argument("resource_type", required=True)
 @click.argument("name", required=True)
 @click.argument("variant", required=False)
 def get(host, cert, insecure, local, resource_type, name, variant):
-    """Get resources of a given type.
-    """
+    """Get resources of a given type."""
     if local:
         if host != None:
             raise ValueError("Cannot be local and have a host")
 
     elif host == None:
-        host = os.getenv('FEATUREFORM_HOST')
+        host = os.getenv("FEATUREFORM_HOST")
         if host == None:
             raise ValueError(
-                "Host value must be set with --host flag or in env as FEATUREFORM_HOST")
+                "Host value must be set with --host flag or in env as FEATUREFORM_HOST"
+            )
 
     client = Client(host=host, local=local, insecure=insecure, cert_path=cert)
 
     resource_get_functions_variant = {
         "feature": client.print_feature,
         "label": client.print_label,
         "source": client.print_source,
@@ -97,39 +96,37 @@
     elif resource_type in resource_get_functions:
         resource_get_functions[resource_type](name=name, local=local)
     else:
         raise ValueError("Resource type not found")
 
 
 @cli.command()
-@click.option("--host",
-              "host",
-              required=False,
-              help="The host address of the API server to connect to")
-@click.option("--cert",
-              "cert",
-              required=False,
-              help="Path to self-signed TLS certificate")
-@click.option("--insecure",
-              is_flag=True,
-              help="Disables TLS verification")
-@click.option("--local",
-              is_flag=True,
-              help="Enable local mode")
+@click.option(
+    "--host",
+    "host",
+    required=False,
+    help="The host address of the API server to connect to",
+)
+@click.option(
+    "--cert", "cert", required=False, help="Path to self-signed TLS certificate"
+)
+@click.option("--insecure", is_flag=True, help="Disables TLS verification")
+@click.option("--local", is_flag=True, help="Enable local mode")
 @click.argument("resource_type", required=True)
 def list(host, cert, insecure, local, resource_type):
     if local:
         if host != None:
             raise ValueError("Cannot be local and have a host")
 
     elif host == None:
-        host = os.getenv('FEATUREFORM_HOST')
+        host = os.getenv("FEATUREFORM_HOST")
         if host == None:
             raise ValueError(
-                "Host value must be set with --host flag or in env as FEATUREFORM_HOST")
+                "Host value must be set with --host flag or in env as FEATUREFORM_HOST"
+            )
 
     client = Client(host=host, local=local, insecure=insecure, cert_path=cert)
 
     resource_list_functions = {
         "features": client.list_features,
         "labels": client.list_labels,
         "sources": client.list_sources,
@@ -154,78 +151,77 @@
 @cli.command()
 def dash():
     app.run(threaded=True, port=os.getenv("LOCALMODE_DASHBOARD_PORT", 3000))
 
 
 @cli.command()
 @click.argument("files", required=True, nargs=-1)
-@click.option("--host",
-              "host",
-              required=False,
-              help="The host address of the API server to connect to")
-@click.option("--cert",
-              "cert",
-              required=False,
-              help="Path to self-signed TLS certificate")
-@click.option("--insecure",
-              is_flag=True,
-              help="Disables TLS verification")
-@click.option("--local",
-              is_flag=True,
-              help="Enable local mode")
-@click.option("--dry-run",
-              is_flag=True,
-              help="Checks the definitions without applying them")
-@click.option("--no-wait",
-              is_flag=True,
-              help="Applies the resources asynchronously")
+@click.option(
+    "--host",
+    "host",
+    required=False,
+    help="The host address of the API server to connect to",
+)
+@click.option(
+    "--cert", "cert", required=False, help="Path to self-signed TLS certificate"
+)
+@click.option("--insecure", is_flag=True, help="Disables TLS verification")
+@click.option("--local", is_flag=True, help="Enable local mode")
+@click.option(
+    "--dry-run", is_flag=True, help="Checks the definitions without applying them"
+)
+@click.option("--no-wait", is_flag=True, help="Applies the resources asynchronously")
 def apply(host, cert, insecure, local, files, dry_run, no_wait):
     for file in files:
         if os.path.isfile(file):
             read_file(file)
         elif validators.url(file):
             read_url(file)
         else:
             raise ValueError(
-                f"Argument must be a path to a file or URL with a valid schema (http:// or https://): {file}")
+                f"Argument must be a path to a file or URL with a valid schema (http:// or https://): {file}"
+            )
 
     client = Client(
         host=host, local=local, insecure=insecure, cert_path=cert, dry_run=dry_run
     )
     asynchronous = no_wait
     client.apply(asynchronous=asynchronous)
 
 
 @cli.command()
-@click.option("--query",
-              "-q",
-              "query",
-              required=True,
-              help="The phrase to search resources (e.g. 'quick').")
-@click.option("--host",
-              "host",
-              required=False,
-              help="The host address of the API server to connect to")
-@click.option("--cert",
-              "cert",
-              required=False,
-              help="Path to self-signed TLS certificate")
-@click.option("--insecure",
-              is_flag=True,
-              help="Disables TLS verification")
-@click.option("--local",
-              is_flag=True,
-              help="Enable local mode")
+@click.option(
+    "--query",
+    "-q",
+    "query",
+    required=True,
+    help="The phrase to search resources (e.g. 'quick').",
+)
+@click.option(
+    "--host",
+    "host",
+    required=False,
+    help="The host address of the API server to connect to",
+)
+@click.option(
+    "--cert", "cert", required=False, help="Path to self-signed TLS certificate"
+)
+@click.option("--insecure", is_flag=True, help="Disables TLS verification")
+@click.option("--local", is_flag=True, help="Enable local mode")
 def search(query, host, cert, insecure, local):
     client = Client(host=host, local=local, insecure=insecure, cert_path=cert)
     results = client.search(query, local)
     if local:
         format_rows("NAME", "VARIANT", "TYPE")
         for r in results:
-            desc = r["description"][:cutoff_length] + "..." if len(r["description"]) > 0 else ""
+            desc = (
+                r["description"][:cutoff_length] + "..."
+                if len(r["description"]) > 0
+                else ""
+            )
             format_rows(r["name"], r["variant"], r["resource_type"])
 
 
 def read_file(file):
     with open(file, "r") as py:
         exec_file(py, file)
 
@@ -243,9 +239,9 @@
     # Create a new global namespace for each file to ensure that
     # global variables, such as `ff`, are not undefined in the
     # context of class attribute assignments (e.g. `label = ff.Label()`)
     file_globals = {}
     exec(code, file_globals)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `featureform-1.7.4/src/featureform/client.py` & `featureform-1.8.0/src/featureform/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .register import (
     ResourceClient,
     SourceRegistrar,
     LocalSource,
     SubscriptableTransformation,
 )
 from .serving import ServingClient
+from .constants import NO_RECORD_LIMIT
 
 
 class Client(ResourceClient, ServingClient):
     """
     Client for interacting with Featureform APIs (resources and serving)
 
     **Using the Client:**
@@ -44,21 +45,23 @@
                 self, host=host, local=local, insecure=insecure, cert_path=cert_path
             )
 
     def dataframe(
         self,
         source: Union[SourceRegistrar, LocalSource, SubscriptableTransformation, str],
         variant="default",
+        limit=NO_RECORD_LIMIT,
     ):
         """
         Compute a dataframe from a registered source or transformation
 
         Args:
             source (Union[SourceRegistrar, LocalSource, SubscriptableTransformation, str]): The source or transformation to compute the dataframe from
             variant (str): The source variant; defaults to "default" and is ignored if source argument is not a string
+            limit (int): The maximum number of records to return; defaults to NO_RECORD_LIMIT
 
         **Example:**
         ```py title="definitions.py"
         transactions_df = client.dataframe("transactions", "quickstart")
 
         avg_user_transaction_df = transactions_df.groupby("CustomerID")["TransactionAmount"].mean()
         """
@@ -68,8 +71,8 @@
             name, variant = source.name_variant()
         elif isinstance(source, str):
             name = source
         else:
             raise ValueError(
                 f"source must be of type SourceRegistrar, LocalSource, SubscriptableTransformation or str, not {type(source)}"
             )
-        return self.impl.get_source_as_df(name, variant)
+        return self.impl._get_source_as_df(name, variant, limit)
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/404.html` & `featureform-1.8.0/src/featureform/dashboard/out/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/404-baaca4b2f4acc755.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>404</b></li></ol></nav></div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/404","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/[type]/[entity].html` & `featureform-1.8.0/src/featureform/dashboard/out/[type]/[entity].html`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D/%5Bentity%5D-b07f3c4463890639.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><a href="/[type]">[type]</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[entity]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]/[entity]","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/[type].html` & `featureform-1.8.0/src/featureform/dashboard/out/[type].html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/%5Btype%5D-751a928da9d524e9.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -560,8 +560,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>[type]</b></li></ol></nav></div><div><div data-testid="notFoundId"><h1>404 Not Found :(</h1></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/[type]","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/_app-a764893ff9420ec0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter/refractor-core-import.d200df4f5651fe3c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abap.cff854fd7e5b1247.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_abnf.a1ff159f2ef1711f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_actionscript.efd417c28a28b388.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ada.156060425d9edae1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_agda.7c059beeef27c79a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_al.f8ab011377e6cffa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_antlr4.2c3a6fa926d2a251.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apacheconf.a8e9c6e2469ebb48.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_apl.17fe889a8c792ca2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_applescript.ec5486ed51b5bf2a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aql.efb695712e3f3aa3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_arduino.681aaa7ec91aa809.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asciidoc.d34ffa4ca9efdc4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_asm6502.3eb992d6df117427.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_aspnet.0ba8de8f97453373.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autohotkey.8bd8b23c56f29881.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_autoit.f687b627eb6354c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bash.fa5423ba02f0452a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_basic.18dbad942d626219.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_batch.8ca1ac5c2d037485.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bbcode.4b540b8d0f463220.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bison.3be4b74c3d3e0770.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_brightscript.5219a23e15549d0f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_bro.6a3db5175eef5a7c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_c.fba60a9486edee8d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cil.494c2357f1d5de1e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clike.065b788c95ab7f0a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_clojure.144f4fa5cb5b7c94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cmake.63bd8fd3867951a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_coffeescript.f3407609f464e5a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_concurnas.807a36085ae57a51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cpp.9073ce25850a9aee.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_crystal.500857f6d38420ca.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csharp.1ab46bae80c6b0ba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_csp.dbb73c45172741db.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_css.c6ce776800cc984e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cssExtras.9588a637662140d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_cypher.899ff7f5c7459114.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_d.3e486cddc20d2ff9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dart.9db40f270a0b6cb0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dax.f58ad34d65866793.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dhall.0ca1a915d1865fb5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_diff.e343fa532144b7a2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_django.6ee6c39cb914f163.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_dnsZoneFile.2a9886e744590498.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_docker.fde534872e6578fd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ebnf.35e28e1f6e8a00e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_eiffel.64ef4de4060b9a23.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ejs.4c4ccb70f90dea01.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elixir.a1e48f12166c723b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_elm.6765aa0f50cbaf91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erb.e48ed285a1945936.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_erlang.2a114ebcf8dd2d26.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_etlua.afcb29f06feae539.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_excelFormula.62d0fdeee42f5d64.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_factor.ce84f1b770942d68.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_firestoreSecurityRules.209ede8c07b9e60b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_flow.88a9cbf968cf47ec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fortran.ca33766cb3d9d13c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_fsharp.1aa244fc87692af1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ftl.0457d46374506e78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gdscript.afa83bf48d38ded2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gedcom.eae35079f43f4e91.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gherkin.1226aeae8764f3d7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_glsl.aaa801f4d5c6da96.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_gml.18f92cdfb2a6d10f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_go.e302653e25089bba.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_graphql.8d0455822c35e9af.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_groovy.67837d37705d722b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haml.9095964d871cb9e5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_handlebars.3a1658c72e98aa85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haskell.c37122cc55c1e696.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_haxe.4e1677441d389a66.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hcl.f5277940e647aca6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_hlsl.f778194f7f56c677.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_http.80f0633c0c6cabe9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ichigojam.154c28afdb7a6cb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_icon.ee1eca6d9d8a1a78.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_iecst.ae937df11bf15aa5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ignore.e7db33c594b328a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_inform7.25b80e018be9b4b0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ini.1305ea3d405b7b77.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_io.57902ad550c5a076.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_j.d8b9ad361d46c928.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_java.375f3f7b940d3ea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoc.9022ca32626ca861.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javadoclike.a5b69d2a868cd5a6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javascript.795b07cdb9c3aad5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_javastacktrace.8ef9f62617bbdae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jolie.fe8eb7d347ec2ee8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jq.995d87dae4a1fc6c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsExtras.a681c21d98be5d88.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsTemplates.e15b503a789336d0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsdoc.863383140825aabf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_json5.b916560a73dec284.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsstacktrace.237affac11d29a8e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_jsx.66ae31b67824e2b1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_julia.aebde82cc8e430a4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_keyman.20a6fec54a9e6dc8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_kotlin.204d94980c876688.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latex.3ea6b205c4740fcf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_latte.6c65a65bc30d6d65.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_less.571cfcc5f39892cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lilypond.b68fc0ec4de9b335.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_liquid.93e3d518888cf132.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lisp.eb4c988e1cb1b488.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_livescript.e154b07a04e47729.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_llvm.3edc24655432e967.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lolcode.920a08022d1f3fb3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_lua.b83366b41cb96d93.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_makefile.cac7a41c308ba41f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markdown.06f7de54663dea9e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markup.0001ba0d552266f8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_markupTemplating.1463fee82d988102.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_matlab.29f5102b58bb0786.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mel.18e5992de05c1caa.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_mizar.2c0399b5c03c3450.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_monkey.bb2faba45e3cee8a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_moonscript.e9dce6a537d684a9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n1ql.9924ec6c046bda5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_n4js.68b6d0a9d2b4e3b9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nasm.08df2ec010d92ce1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_neon.b4d21d37e14ff2e4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nginx.a7f671ec4fed709c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nim.b9b3330a8cc76ae6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nix.ec8c698fe8cf158f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_nsis.17532a14606f8ba0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_objectivec.a9a054b060f7e9c4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ocaml.0ce7e66b58933eec.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_opencl.343386871671e433.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_oz.3dd791c14d6789e9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parigp.01c2a6558ead9c1d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_parser.4080f0c5df8c5411.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascal.714d7fd616dffa60.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pascaligo.3d9efa4ff03d798d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pcaxis.dc2dc17ec584a4e1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_peoplecode.00b98a730fe91b5e.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_perl.a4fecd65a9c2ecd2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_php.1da6a39f37370ec1.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpExtras.8468f770a82630ef.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_phpdoc.59ba40872e3d9cfe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_plsql.6fc1cf5b4b2439a3.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powerquery.c87eb035121d7831.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_powershell.56966af030c91702.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_processing.ec8607c7392a938f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_protobuf.d96df12b0f0a2409.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pug.6b509aa2c3a57467.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_puppet.ce519d4962965362.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_pure.e3fd8806900462cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_purebasic.70942e3d774ada85.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_q.1df151a687a188a7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qml.e36896b667a01ae9.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_qore.1137d54889243367.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_r.7ca305d9455cc86f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_racket.bee31c56faa733b2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_reason.af902fad4bd674df.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_regex.074352f8c0201b38.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_renpy.5938c171f23d6f29.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rest.fcefb9b5cfa112e0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rip.5f599ff53f5c1e9a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_roboconf.49d8eaad661bcd43.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_robotframework.883fa1f592ad87e7.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_ruby.f76b4f68b3137a6f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_rust.ca92b5ca27e7312d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sas.33e0e78e18cf156f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sass.8436ff53b0701941.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scala.7db11a73d01e23d4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scheme.a224b3505cc86f4d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_scss.fbd015582067d022.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_shellSession.54615d020c9c44d5.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smali.e44f80bb9100f728.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smalltalk.e89fea8686ec9f90.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_smarty.404a8e12834103cf.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solidity.537cb7600d04dae8.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_solutionFile.53d3dde6d83fdea2.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_soy.51e9adabd56f467a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sparql.2aa3288ef8ae3374.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_splunkSpl.095636b50fe9a368.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_sqf.11b0bee7a2de8e94.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_stylus.213bb148fbffff7f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_swift.27d0fee1e44e54b6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Cs.cd31c8bc90add20f.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Templating.c87834ec2ea19f73.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_t4Vb.2cf235d46995926d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tap.a22e7b01443f999b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tcl.72a4244b8fb7ec0d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_textile.e52c4e181b801ddd.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_toml.9bf8ce9e1f31a008.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tsx.f039389d397f2bb4.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_tt2.645259383cf82689.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_turtle.69d8330a2e17bb57.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_twig.d5bfca25e9d2543d.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_typescript.d8f51be2a38383c6.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_unrealscript.9179623df9a8b80c.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vala.2e16603251de6f51.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vbnet.ac96de8240011055.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_velocity.bc75ee95252e2b47.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_verilog.4e42ac1a89cb8605.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vhdl.5ab0f6bc359d7c74.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_vim.6c4d4c01dc147971.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_visualBasic.c3e43390c4a3ee45.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_warpscript.ccc821a2177dfac0.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wasm.3ffc1a78867a6148.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_wiki.b5dc9ed00ff4ea53.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xeora.b31606451a6f896b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xojo.81cb4d9104c6ac5b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_xquery.4382c54a41b1309a.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_yaml.178577f1d765f16b.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/react-syntax-highlighter_languages_refractor_zig.a535909b59fc6987.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/media/Matter-Regular.f1ae4ce5.ttf`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/u8jMEl73MAEGHR4r4U4Dw/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js` & `featureform-1.8.0/src/featureform/dashboard/out/_next/static/xB9Lh8aE_cExc1t6WFtEI/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/connections.html` & `featureform-1.8.0/src/featureform/dashboard/out/connections.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/connections-1d67ba61869dece6.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -1058,8 +1058,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Connections</b></li></ol></nav></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center MuiGrid-grid-lg-12"></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/connections","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/index.html` & `featureform-1.8.0/src/featureform/dashboard/out/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><title>Featureform Dashboard</title><meta name="next-head-count" content="3"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/index-c2ee5b1681e97e4b.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -1456,8 +1456,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search" data-testid="searchInputId" class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><div></div></div><div><div class="jss15"><div class="jss16"><div class="jss17"></div><div class="jss23"><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-justify-content-xs-center"><div class="MuiContainer-root jss25 MuiContainer-maxWidthLg"><div class="jss24"><svg class="MuiSvgIcon-root" focusable="false" viewBox="0 0 24 24" aria-hidden="true"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path></svg></div><div class="MuiInputBase-root jss26"><input type="text" placeholder="Search..." value="" aria-label="search" data-testid="searchInputId" class="MuiInputBase-input jss27"/></div></div></div></div></div><div class="jss20"><div class="jss21"><div class="jss19"><h5 class="MuiTypography-root MuiTypography-h5"></h5></div><div><div class="MuiGrid-root MuiGrid-container MuiGrid-justify-content-xs-center"><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 MuiGrid-grid-md-6 MuiGrid-grid-lg-4"></div></div></div></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/search.html` & `featureform-1.8.0/src/featureform/dashboard/out/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js" defer=""></script><script src="/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
+<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><link rel="icon" href="/static/favicon.ico"/><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin /><link rel="preload" href="/_next/static/css/85a2addfd2efc882.css" as="style"/><link rel="stylesheet" href="/_next/static/css/85a2addfd2efc882.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-6ed703bc0f4dd2fe.js" defer=""></script><script src="/_next/static/chunks/framework-3412d1150754b2fb.js" defer=""></script><script src="/_next/static/chunks/main-2715d0c23f47c019.js" defer=""></script><script src="/_next/static/chunks/pages/_app-a764893ff9420ec0.js" defer=""></script><script src="/_next/static/chunks/pages/search-175858e61ba25631.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js" defer=""></script><script src="/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js" defer=""></script><style id="jss-server-side">.MuiTypography-root {
   margin: 0;
 }
 .MuiTypography-body2 {
   font-size: 0.875rem;
   font-family: "Matter", "Lato", "Helvetica", sans-serif;
   font-weight: 550;
   line-height: 1.43;
@@ -594,8 +594,8 @@
     position: relative;
     font-size: 3em;
     justify-self: flex-end;
   }
   .jss1 {
     padding-left: 64px;
     padding-right: 64px;
-  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div><div class="MuiContainer-root jss15 MuiContainer-maxWidthXl"><h4 class="MuiTypography-root jss17 MuiTypography-h4" style="display:flex"><div style="color:gray">No results for: </div><b></b></h4><div><nav class="MuiList-root jss15 MuiList-padding"></nav></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"8yA-hIcHsUSF2wPeJxwZa","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+  }</style><style data-href="https://fonts.googleapis.com/icon?family=Material+Icons">@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.woff) format('woff')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;font-feature-settings:'liga'}@font-face{font-family:'Material Icons';font-style:normal;font-weight:400;src:url(https://fonts.gstatic.com/s/materialicons/v140/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2) format('woff2')}.material-icons{font-family:'Material Icons';font-weight:normal;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:'liga';-webkit-font-smoothing:antialiased}</style></head><body><div id="__next" data-reactroot=""><div class="jss2"><header class="MuiPaper-root MuiAppBar-root MuiAppBar-positionStatic MuiAppBar-colorPrimary jss3 MuiPaper-elevation4"><div class="MuiToolbar-root MuiToolbar-regular jss6 MuiToolbar-gutters"><div class="jss7"><img src="/static/FeatureForm_Logo_Full_Black.svg" height="30" alt="Featureform" component="div" nowrap="true" style="cursor:pointer" sx="[object Object]"/></div><div class="jss9"></div></div></header></div><div class="MuiContainer-root MuiContainer-maxWidthXl jss1"><div class="jss11"><nav class="MuiTypography-root MuiBreadcrumbs-root jss13 MuiTypography-body1 MuiTypography-colorTextSecondary" style="margin:0.25em" aria-label="breadcrumb"><ol class="MuiBreadcrumbs-ol jss12"><li class="MuiBreadcrumbs-li"><a href="/">Home</a></li><li aria-hidden="true" class="MuiBreadcrumbs-separator jss14"><style data-emotion="css vubbuv">.css-vubbuv{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;width:1em;height:1em;display:inline-block;fill:currentColor;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;-webkit-transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:fill 200ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;font-size:1.5rem;}</style><svg class="MuiSvgIcon-root MuiSvgIcon-fontSizeMedium css-vubbuv" focusable="false" aria-hidden="true" viewBox="0 0 24 24" data-testid="NavigateNextIcon"><path d="M10 6 8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path></svg></li><li class="MuiBreadcrumbs-li"><b>Search</b></li></ol></nav></div><div><div><div class="MuiContainer-root jss15 MuiContainer-maxWidthXl"><h4 class="MuiTypography-root jss17 MuiTypography-h4" style="display:flex"><div style="color:gray">No results for: </div><b></b></h4><div><nav class="MuiList-root jss15 MuiList-padding"></nav></div></div></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/search","query":{},"buildId":"XLqQwuMDcHNwRKV5unb2J","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Apache_Spark_logo.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Apache_Spark_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Capital_One_logo.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Capital_One_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/FeatureForm_Logo_Full_Black.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Featureform_logo_pink.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Featureform_logo_pink.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Kubernetes_logo.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Kubernetes_logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Postgresql_elephant.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Postgresql_elephant.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Redis_Logo.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Redis_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/Snowflake_Logo.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/Snowflake_Logo.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/amazon-dynamoDB.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/amazon-dynamoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/amazon_redshift.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/amazon_redshift.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/amazon_s3.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/amazon_s3.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/apache_cassandra.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/apache_cassandra.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/apache_hadoop.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/apache_hadoop.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/apple-touch-icon.png` & `featureform-1.8.0/src/featureform/dashboard/out/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/azure_storage_accounts.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/azure_storage_accounts.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/favicon.ico` & `featureform-1.8.0/src/featureform/dashboard/out/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/google_bigquery.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/google_bigquery.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/google_cloud_storage.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/google_cloud_storage.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/google_firestore.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/google_firestore.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/logo192.png` & `featureform-1.8.0/src/featureform/dashboard/out/static/logo192.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/logo512.png` & `featureform-1.8.0/src/featureform/dashboard/out/static/logo512.png`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/mongoDB.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/mongoDB.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard/out/static/safari-pinned-tab.svg` & `featureform-1.8.0/src/featureform/dashboard/out/static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/dashboard_metadata.py` & `featureform-1.8.0/src/featureform/dashboard_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,344 +1,484 @@
 from flask import Blueprint, Response, jsonify, request
 from flask_cors import CORS, cross_origin
 import json
 import importlib.resources as pkg_resources
 from .sqlite_metadata import SQLiteMetadata
 from .resources import SourceType
 from .type_objects import (
-    FeatureResource, 
-    FeatureVariantResource, 
-    TrainingSetResource, 
-    TrainingSetVariantResource, 
-    SourceResource, 
-    SourceVariantResource, 
-    EntityResource, 
-    UserResource, 
+    FeatureResource,
+    FeatureVariantResource,
+    TrainingSetResource,
+    TrainingSetVariantResource,
+    SourceResource,
+    SourceVariantResource,
+    EntityResource,
+    UserResource,
     ModelResource,
     LabelResource,
     LabelVariantResource,
-    ProviderResource)
+    ProviderResource,
+)
 import os
 from featureform import ResourceClient
 import sys
 
-path = os.path.join(os.path.dirname(__file__), 'dashboard')
+path = os.path.join(os.path.dirname(__file__), "dashboard")
 
-dashboard_app = Blueprint('dashboard_app', __name__, static_folder=path + '/out/', static_url_path='')
+dashboard_app = Blueprint(
+    "dashboard_app", __name__, static_folder=path + "/out/", static_url_path=""
+)
 
 CORS(dashboard_app)
-sqlObject = SQLiteMetadata() 
+sqlObject = SQLiteMetadata()
 
-@dashboard_app.route('/')
+
+@dashboard_app.route("/")
 def index():
-    return dashboard_app.send_static_file('index.html')
+    return dashboard_app.send_static_file("index.html")
+
 
-@dashboard_app.route('/<type>')
+@dashboard_app.route("/<type>")
 def type(type):
-    return dashboard_app.send_static_file('[type].html')
+    return dashboard_app.send_static_file("[type].html")
 
-@dashboard_app.route('/<type>/<entity>')
+
+@dashboard_app.route("/<type>/<entity>")
 def entity(type, entity):
-    return dashboard_app.send_static_file('[type]/[entity].html')
+    return dashboard_app.send_static_file("[type]/[entity].html")
+
 
-@dashboard_app.route('/search')
+@dashboard_app.route("/search")
 def search():
-    return dashboard_app.send_static_file('search.html')
+    return dashboard_app.send_static_file("search.html")
 
-@dashboard_app.route('/static/<asset>')
+
+@dashboard_app.route("/static/<asset>")
 def deliver_static(asset):
-    return dashboard_app.send_static_file('static/' + asset)
+    return dashboard_app.send_static_file("static/" + asset)
+
 
 def variant_organiser(allVariantList):
     variantsDict = dict()
 
     for variant in allVariantList:
         name = variant["name"]
-        if name in variantsDict: 
+        if name in variantsDict:
             variantsDict[name].append(variant)
         else:
             variantsDict[name] = [variant]
-    
+
     return variantsDict
 
+
 def feature_variant(variantData):
     variantsDict = dict()
     allVariantList = []
     variants = []
-    
+
     for variantRow in variantData:
         featureVariant = FeatureVariantResource(
-                variantRow['created'], 
-                variantRow['description'], 
-                variantRow['entity'], 
-                variantRow['name'], 
-                variantRow['owner'], 
-                variantRow['provider'], 
-                variantRow['data_type'], 
-                variantRow['variant'], 
-                variantRow['status'], 
-                {"entity": variantRow['source_entity'],
-                "value": variantRow['source_value'], 
-                "timestamp": variantRow['source_timestamp']},
-                {"Name":variantRow['source_name'],
-                "Variant":variantRow['source_variant']},
-                json.loads(variantRow['tags']) if variantRow['tags'] is not None else [],
-                json.loads(variantRow['properties']) if variantRow['properties'] is not None else {}
-            ).toDictionary()
+            variantRow["created"],
+            variantRow["description"],
+            variantRow["entity"],
+            variantRow["name"],
+            variantRow["owner"],
+            variantRow["provider"],
+            variantRow["data_type"],
+            variantRow["variant"],
+            variantRow["status"],
+            {
+                "entity": variantRow["source_entity"],
+                "value": variantRow["source_value"],
+                "timestamp": variantRow["source_timestamp"],
+            },
+            {
+                "Name": variantRow["source_name"],
+                "Variant": variantRow["source_variant"],
+            },
+            json.loads(variantRow["tags"]) if variantRow["tags"] is not None else [],
+            json.loads(variantRow["properties"])
+            if variantRow["properties"] is not None
+            else {},
+        ).toDictionary()
 
-        allVariantList.append(variantRow['variant'])
-        variantsDict[variantRow['variant']] = featureVariant
+        allVariantList.append(variantRow["variant"])
+        variantsDict[variantRow["variant"]] = featureVariant
         variants.append(featureVariant)
     return variantsDict, allVariantList, variants
 
+
 def features(featureRow):
-    variantData = feature_variant(sqlObject.query_resource_variant("feature_variant", "name", featureRow['name']))
-    
+    variantData = feature_variant(
+        sqlObject.query_resource_variant("feature_variant", "name", featureRow["name"])
+    )
+
     return FeatureResource(
-                featureRow['name'], 
-                featureRow['default_variant'], 
-                "Feature", 
-                variantData[0], 
-                variantData[1] 
-            ).toDictionary()
+        featureRow["name"],
+        featureRow["default_variant"],
+        "Feature",
+        variantData[0],
+        variantData[1],
+    ).toDictionary()
+
 
 def training_set_variant(variantData):
     variantDict = dict()
     allVariantList = []
     variants = []
     for variantRow in variantData:
         try:
-            feature_list = sqlObject.get_training_set_features(variantRow['name'], variantRow['variant'])
+            feature_list = sqlObject.get_training_set_features(
+                variantRow["name"], variantRow["variant"]
+            )
         except ValueError:
             feature_list = []
 
         trainingSetVariant = TrainingSetVariantResource(
-                variantRow['created'], 
-                variantRow['description'], 
-                variantRow['name'], 
-                variantRow['owner'], 
-                variantRow['variant'], 
-                {"Name":variantRow['label_name'],
-                "Variant":variantRow['label_variant']}, 
-                variantRow['status'], 
-                variant_organiser(feature_variant(getTrainingSetFeatures(feature_list))[2]),
-                json.loads(variantRow['tags']) if variantRow['tags'] is not None else [],
-                json.loads(variantRow['properties']) if variantRow['properties'] is not None else {}
-            ).toDictionary()
-        allVariantList.append(variantRow['variant'])
-        variantDict[variantRow['variant']] = trainingSetVariant
+            variantRow["created"],
+            variantRow["description"],
+            variantRow["name"],
+            variantRow["owner"],
+            variantRow["variant"],
+            {"Name": variantRow["label_name"], "Variant": variantRow["label_variant"]},
+            variantRow["status"],
+            variant_organiser(feature_variant(getTrainingSetFeatures(feature_list))[2]),
+            json.loads(variantRow["tags"]) if variantRow["tags"] is not None else [],
+            json.loads(variantRow["properties"])
+            if variantRow["properties"] is not None
+            else {},
+        ).toDictionary()
+        allVariantList.append(variantRow["variant"])
+        variantDict[variantRow["variant"]] = trainingSetVariant
         variants.append(trainingSetVariant)
 
     return variantDict, allVariantList, variants
-    
+
+
 def getTrainingSetFeatures(feature_list):
     feature_variant_tuple = []
     for feature in feature_list:
-        feature_variant_tuple.append(sqlObject.get_feature_variant(feature["feature_name"], feature["feature_variant"]))
+        feature_variant_tuple.append(
+            sqlObject.get_feature_variant(
+                feature["feature_name"], feature["feature_variant"]
+            )
+        )
     return feature_variant_tuple
 
+
 def training_sets(rowData):
-    variantData = training_set_variant(sqlObject.query_resource_variant("training_set_variant", "name", rowData['name']))
-    return TrainingSetResource( 
-                "TrainingSet", 
-                rowData['default_variant'], 
-                rowData['name'], 
-                variantData[0], 
-                variantData[1] 
-            ).toDictionary()
+    variantData = training_set_variant(
+        sqlObject.query_resource_variant(
+            "training_set_variant", "name", rowData["name"]
+        )
+    )
+    return TrainingSetResource(
+        "TrainingSet",
+        rowData["default_variant"],
+        rowData["name"],
+        variantData[0],
+        variantData[1],
+    ).toDictionary()
+
 
 def source_variant(variantData):
     variantDict = dict()
     allVariantList = []
     variants = []
     for variantRow in variantData:
         try:
-            feature_list = sqlObject.get_feature_variants_from_source(variantRow['name'], variantRow['variant'])
+            feature_list = sqlObject.get_feature_variants_from_source(
+                variantRow["name"], variantRow["variant"]
+            )
         except ValueError:
             feature_list = []
         training_set_list = set()
         for f in feature_list:
             try:
-                features_training_set_list = sqlObject.get_training_set_from_features(f["name"], f["variant"])
+                features_training_set_list = sqlObject.get_training_set_from_features(
+                    f["name"], f["variant"]
+                )
                 for training_set in features_training_set_list:
-                    training_set_list.add(sqlObject.get_training_set_variant(training_set["training_set_name"], training_set["training_set_variant"]))
+                    training_set_list.add(
+                        sqlObject.get_training_set_variant(
+                            training_set["training_set_name"],
+                            training_set["training_set_variant"],
+                        )
+                    )
             except ValueError:
                 continue
         try:
-            label_list = sqlObject.get_label_variants_from_source(variantRow["name"], variantRow["variant"])
+            label_list = sqlObject.get_label_variants_from_source(
+                variantRow["name"], variantRow["variant"]
+            )
         except ValueError:
             label_list = []
         for l in label_list:
             try:
-                labels_training_set_list = sqlObject.get_training_set_variant_from_label(l["name"], l["variant"])
+                labels_training_set_list = (
+                    sqlObject.get_training_set_variant_from_label(
+                        l["name"], l["variant"]
+                    )
+                )
                 for training_set in labels_training_set_list:
                     training_set_list.add(training_set)
             except ValueError:
                 continue
-        if variantRow['transformation'] == SourceType.DF_TRANSFORMATION.value:
-            definition = str(variantRow['definition'], 'latin-1')
+        if variantRow["transformation"] == SourceType.DF_TRANSFORMATION.value:
+            definition = str(variantRow["definition"], "latin-1")
         else:
-            definition = variantRow['definition']
+            definition = variantRow["definition"]
         sourceVariant = SourceVariantResource(
-                variantRow['created'], 
-                variantRow['description'], 
-                variantRow['name'], 
-                variantRow['source_type'], 
-                variantRow['owner'], 
-                variantRow['provider'], 
-                variantRow['variant'], 
-                variantRow['status'], 
-                definition, 
-                variant_organiser(label_variant(label_list)[2]), 
-                variant_organiser(feature_variant(feature_list)[2]),
-                variant_organiser(training_set_variant(training_set_list)[2]),
-                json.loads(variantRow['tags']) if variantRow['tags'] is not None else [],
-                json.loads(variantRow['properties']) if variantRow['properties'] is not None else {}
-            ).toDictionary()
-        allVariantList.append(variantRow['name'])
-        variantDict[variantRow['variant']] = sourceVariant
+            variantRow["created"],
+            variantRow["description"],
+            variantRow["name"],
+            variantRow["source_type"],
+            variantRow["owner"],
+            variantRow["provider"],
+            variantRow["variant"],
+            variantRow["status"],
+            definition,
+            variant_organiser(label_variant(label_list)[2]),
+            variant_organiser(feature_variant(feature_list)[2]),
+            variant_organiser(training_set_variant(training_set_list)[2]),
+            json.loads(variantRow["tags"]) if variantRow["tags"] is not None else [],
+            json.loads(variantRow["properties"])
+            if variantRow["properties"] is not None
+            else {},
+        ).toDictionary()
+        allVariantList.append(variantRow["name"])
+        variantDict[variantRow["variant"]] = sourceVariant
         variants.append(sourceVariant)
-    
+
     return variantDict, allVariantList, variants
 
+
 def sources(rowData):
-    variantData = source_variant(sqlObject.query_resource_variant("source_variant", "name", rowData['name']))
-    return SourceResource( 
-                "Source", 
-                rowData['default_variant'], 
-                rowData['name'], 
-                variantData[0], 
-                variantData[1] 
-            ).toDictionary()
-    
+    variantData = source_variant(
+        sqlObject.query_resource_variant("source_variant", "name", rowData["name"])
+    )
+    return SourceResource(
+        "Source",
+        rowData["default_variant"],
+        rowData["name"],
+        variantData[0],
+        variantData[1],
+    ).toDictionary()
+
+
 def label_variant(variantData):
     variantDict = dict()
     allVariantList = []
     variants = []
 
     for variantRow in variantData:
-        labelTuple = str((variantRow['name'], variantRow['variant']))
+        labelTuple = str((variantRow["name"], variantRow["variant"]))
         labelVariant = LabelVariantResource(
-                variantRow['created'], 
-                variantRow['description'], 
-                variantRow['entity'], 
-                variantRow['name'], 
-                variantRow['owner'], 
-                variantRow['provider'], 
-                variantRow['data_type'], 
-                variantRow['variant'], 
-                {"entity": variantRow['source_entity'],
-                "value": variantRow['source_value'],
-                "timestamp": variantRow['source_timestamp']},
-                variantRow['status'], 
-                {"Name":variantRow['source_name'],
-                "Variant":variantRow['source_variant']}, 
-                variant_organiser(training_set_variant(sqlObject.get_training_set_variant_from_label(variantRow['name'], variantRow['variant']))[2]),
-                json.loads(variantRow['tags']) if variantRow['tags'] is not None else [],
-                json.loads(variantRow['properties']) if variantRow['properties'] is not None else {}
-            ).toDictionary()
-        
-        allVariantList.append(variantRow['variant'])
-        variantDict[variantRow['variant']] = labelVariant
+            variantRow["created"],
+            variantRow["description"],
+            variantRow["entity"],
+            variantRow["name"],
+            variantRow["owner"],
+            variantRow["provider"],
+            variantRow["data_type"],
+            variantRow["variant"],
+            {
+                "entity": variantRow["source_entity"],
+                "value": variantRow["source_value"],
+                "timestamp": variantRow["source_timestamp"],
+            },
+            variantRow["status"],
+            {
+                "Name": variantRow["source_name"],
+                "Variant": variantRow["source_variant"],
+            },
+            variant_organiser(
+                training_set_variant(
+                    sqlObject.get_training_set_variant_from_label(
+                        variantRow["name"], variantRow["variant"]
+                    )
+                )[2]
+            ),
+            json.loads(variantRow["tags"]) if variantRow["tags"] is not None else [],
+            json.loads(variantRow["properties"])
+            if variantRow["properties"] is not None
+            else {},
+        ).toDictionary()
+
+        allVariantList.append(variantRow["variant"])
+        variantDict[variantRow["variant"]] = labelVariant
         variants.append(labelVariant)
     return variantDict, allVariantList, variants
 
+
 def labels(rowData):
-    variantData = label_variant(sqlObject.query_resource_variant("label_variant", "name", rowData['name']))
+    variantData = label_variant(
+        sqlObject.query_resource_variant("label_variant", "name", rowData["name"])
+    )
     return LabelResource(
-                "Label", 
-                rowData['default_variant'], 
-                rowData['name'], 
-                variantData[0], 
-                variantData[1] 
-            ).toDictionary()
+        "Label",
+        rowData["default_variant"],
+        rowData["name"],
+        variantData[0],
+        variantData[1],
+    ).toDictionary()
+
 
 def entities(rowData):
-    label_list = sqlObject.query_resource_variant( "label_variant", "entity", rowData['name'])
+    label_list = sqlObject.query_resource_variant(
+        "label_variant", "entity", rowData["name"]
+    )
     training_set_list = set()
     for label in label_list:
-        for training_set in sqlObject.get_training_set_variant_from_label(label["name"], label["variant"]):
+        for training_set in sqlObject.get_training_set_variant_from_label(
+            label["name"], label["variant"]
+        ):
             training_set_list.add(training_set)
     return EntityResource(
-                rowData['name'], 
-                rowData['type'], 
-                rowData['description'], 
-                rowData['status'], 
-                variant_organiser(feature_variant(sqlObject.query_resource_variant( "feature_variant", "entity", rowData['name']))[2]),
-                variant_organiser(label_variant(label_list)[2]), 
-                variant_organiser(training_set_variant(training_set_list)[2]),
-                json.loads(rowData['tags']) if rowData['tags'] is not None else [],
-                json.loads(rowData['properties']) if rowData['properties'] is not None else {}
-            ).toDictionary()
+        rowData["name"],
+        rowData["type"],
+        rowData["description"],
+        rowData["status"],
+        variant_organiser(
+            feature_variant(
+                sqlObject.query_resource_variant(
+                    "feature_variant", "entity", rowData["name"]
+                )
+            )[2]
+        ),
+        variant_organiser(label_variant(label_list)[2]),
+        variant_organiser(training_set_variant(training_set_list)[2]),
+        json.loads(rowData["tags"]) if rowData["tags"] is not None else [],
+        json.loads(rowData["properties"]) if rowData["properties"] is not None else {},
+    ).toDictionary()
+
 
 def models(rowData):
     return ModelResource(
-                rowData['name'], 
-                "Model", 
-                rowData['description'], 
-                rowData['status'], 
-                variant_organiser(feature_variant(sqlObject.query_resource_variant( "feature_variant", "name", rowData['name']))[2]),
-                variant_organiser(label_variant(sqlObject.query_resource_variant( "label_variant", "variant", rowData['name']))[2]),
-                variant_organiser(training_set_variant(sqlObject.query_resource_variant( "training_set_variant", "name", rowData['name']))[2]),
-                json.loads(rowData['tags']) if rowData['tags'] is not None else [],
-                json.loads(rowData['properties']) if rowData['properties'] is not None else {}
-            ).toDictionary()
+        rowData["name"],
+        "Model",
+        rowData["description"],
+        rowData["status"],
+        variant_organiser(
+            feature_variant(
+                sqlObject.query_resource_variant(
+                    "feature_variant", "name", rowData["name"]
+                )
+            )[2]
+        ),
+        variant_organiser(
+            label_variant(
+                sqlObject.query_resource_variant(
+                    "label_variant", "variant", rowData["name"]
+                )
+            )[2]
+        ),
+        variant_organiser(
+            training_set_variant(
+                sqlObject.query_resource_variant(
+                    "training_set_variant", "name", rowData["name"]
+                )
+            )[2]
+        ),
+        json.loads(rowData["tags"]) if rowData["tags"] is not None else [],
+        json.loads(rowData["properties"]) if rowData["properties"] is not None else {},
+    ).toDictionary()
+
 
 def users(rowData):
     return UserResource(
-                rowData['name'], 
-                rowData['type'], 
-                rowData['status'],  
-                variant_organiser(feature_variant(sqlObject.query_resource_variant( "feature_variant", "owner", rowData['name']))[2]),
-                variant_organiser(label_variant(sqlObject.query_resource_variant( "label_variant", "owner", rowData['name']))[2]),
-                variant_organiser(training_set_variant(sqlObject.query_resource_variant( "training_set_variant", "owner", rowData['name']))[2]),
-                variant_organiser(source_variant(sqlObject.query_resource_variant( "source_variant", "owner", rowData['name']))[2]),
-                json.loads(rowData['tags']) if rowData['tags'] is not None else [],
-                json.loads(rowData['properties']) if rowData['properties'] is not None else {}
-            ).toDictionary()
+        rowData["name"],
+        rowData["type"],
+        rowData["status"],
+        variant_organiser(
+            feature_variant(
+                sqlObject.query_resource_variant(
+                    "feature_variant", "owner", rowData["name"]
+                )
+            )[2]
+        ),
+        variant_organiser(
+            label_variant(
+                sqlObject.query_resource_variant(
+                    "label_variant", "owner", rowData["name"]
+                )
+            )[2]
+        ),
+        variant_organiser(
+            training_set_variant(
+                sqlObject.query_resource_variant(
+                    "training_set_variant", "owner", rowData["name"]
+                )
+            )[2]
+        ),
+        variant_organiser(
+            source_variant(
+                sqlObject.query_resource_variant(
+                    "source_variant", "owner", rowData["name"]
+                )
+            )[2]
+        ),
+        json.loads(rowData["tags"]) if rowData["tags"] is not None else [],
+        json.loads(rowData["properties"]) if rowData["properties"] is not None else {},
+    ).toDictionary()
+
 
 def providers(rowData):
     try:
-        source_list = sqlObject.query_resource_variant( "source_variant", "provider", rowData['name'])
+        source_list = sqlObject.query_resource_variant(
+            "source_variant", "provider", rowData["name"]
+        )
     except ValueError:
         source_list = []
     try:
-        feature_list = sqlObject.query_resource_variant( "feature_variant", "provider", rowData['name'])
+        feature_list = sqlObject.query_resource_variant(
+            "feature_variant", "provider", rowData["name"]
+        )
     except ValueError:
         feature_list = []
     try:
-        label_list = sqlObject.query_resource_variant( "label_variant", "provider", rowData['name'])
+        label_list = sqlObject.query_resource_variant(
+            "label_variant", "provider", rowData["name"]
+        )
     except ValueError:
         label_list = []
     return ProviderResource(
-                rowData['name'], 
-                rowData['type'], 
-                rowData['description'], 
-                rowData['provider_type'], 
-                rowData['software'], 
-                rowData['team'], 
-                variant_organiser(source_variant(source_list)[2]), 
-                rowData['status'], 
-                rowData['serialized_config'],
-                variant_organiser(feature_variant(feature_list)[2]),
-                variant_organiser(label_variant(label_list)[2]),
-                json.loads(rowData['tags']) if rowData['tags'] is not None else [],
-                json.loads(rowData['properties']) if rowData['properties'] is not None else {}
-            ).toDictionary()
+        rowData["name"],
+        rowData["type"],
+        rowData["description"],
+        rowData["provider_type"],
+        rowData["software"],
+        rowData["team"],
+        variant_organiser(source_variant(source_list)[2]),
+        rowData["status"],
+        rowData["serialized_config"],
+        variant_organiser(feature_variant(feature_list)[2]),
+        variant_organiser(label_variant(label_list)[2]),
+        json.loads(rowData["tags"]) if rowData["tags"] is not None else [],
+        json.loads(rowData["properties"]) if rowData["properties"] is not None else {},
+    ).toDictionary()
+
 
-@dashboard_app.route("/data/<type>", methods = ['POST', 'GET'])
-@cross_origin(allow_headers=['Content-Type'])
+@dashboard_app.route("/data/<type>", methods=["POST", "GET"])
+@cross_origin(allow_headers=["Content-Type"])
 def GetMetadataList(type):
     type = type.replace("-", "_")
-    if type not in ["features", "training_sets", "sources", "labels", "entities", "models", "users", "providers"]:
+    if type not in [
+        "features",
+        "training_sets",
+        "sources",
+        "labels",
+        "entities",
+        "models",
+        "users",
+        "providers",
+    ]:
         errorData = f"invalid resource type: {type}"
         response = Response(
-        response=json.dumps(errorData),
-        status=400,
-        mimetype='application/json'
+            response=json.dumps(errorData), status=400, mimetype="application/json"
         )
         return response
     tableDataCursor = sqlObject.get_type_table(type)
     allData = []
     for row in tableDataCursor:
         if type == "features":
             allData.append(features(row))
@@ -354,63 +494,77 @@
             allData.append(models(row))
         elif type == "users":
             allData.append(users(row))
         elif type == "providers":
             allData.append(providers(row))
 
     response = Response(
-        response=json.dumps(allData),
-        status=200,
-        mimetype='application/json'
+        response=json.dumps(allData), status=200, mimetype="application/json"
     )
     return response
 
-@dashboard_app.route("/data/<type>/<resource>", methods = ['POST', 'GET'])
-@cross_origin(allow_headers=['Content-Type'])
-def GetMetadata(type, resource):
-        type = type.replace("-", "_")
-        if type not in ["features", "training_sets", "sources", "labels", "entities", "models", "users", "providers"]:
-            errorData = f"invalid resource type: {type}"
-            response = Response(
-            response=json.dumps(errorData),
-            status=400,
-            mimetype='application/json'
-            )
-            return response
-        should_fetch_tags_and_properties = type in ["entities", "models", "users", "providers"]
-        row = sqlObject.query_resource(type, "name", "".join(resource), should_fetch_tags_and_properties)[0]
-
-        if type == "features":
-            dataAsList =  features(row)
-        elif type == "training_sets":
-            dataAsList =  training_sets(row)
-        elif type == "sources":
-            dataAsList =  sources(row)
-        elif type == "labels":
-            dataAsList =  labels(row)
-        elif type == "entities":
-            dataAsList =  entities(row)
-        elif type == "models":
-            dataAsList =  models(row)
-        elif type == "users":
-            dataAsList =  users(row)
-        elif type == "providers":
-            dataAsList =  providers(row)
 
+@dashboard_app.route("/data/<type>/<resource>", methods=["POST", "GET"])
+@cross_origin(allow_headers=["Content-Type"])
+def GetMetadata(type, resource):
+    type = type.replace("-", "_")
+    if type not in [
+        "features",
+        "training_sets",
+        "sources",
+        "labels",
+        "entities",
+        "models",
+        "users",
+        "providers",
+    ]:
+        errorData = f"invalid resource type: {type}"
         response = Response(
-            response=json.dumps(dataAsList),
-            status=200,
-            mimetype='application/json'
+            response=json.dumps(errorData), status=400, mimetype="application/json"
         )
         return response
+    should_fetch_tags_and_properties = type in [
+        "entities",
+        "models",
+        "users",
+        "providers",
+    ]
+    row = sqlObject.query_resource(
+        type, "name", "".join(resource), should_fetch_tags_and_properties
+    )[0]
+
+    if type == "features":
+        dataAsList = features(row)
+    elif type == "training_sets":
+        dataAsList = training_sets(row)
+    elif type == "sources":
+        dataAsList = sources(row)
+    elif type == "labels":
+        dataAsList = labels(row)
+    elif type == "entities":
+        dataAsList = entities(row)
+    elif type == "models":
+        dataAsList = models(row)
+    elif type == "users":
+        dataAsList = users(row)
+    elif type == "providers":
+        dataAsList = providers(row)
 
-@dashboard_app.route("/data/search", methods = ['GET'])
-@cross_origin(allow_headers=['Content-Type'])
+    response = Response(
+        response=json.dumps(dataAsList), status=200, mimetype="application/json"
+    )
+    return response
+
+
+@dashboard_app.route("/data/search", methods=["GET"])
+@cross_origin(allow_headers=["Content-Type"])
 def SearchMetadata():
     raw_query = request.args["q"]
     rc = ResourceClient(local=True)
     results = rc.search(raw_query, True)
     payload = []
     for r in results:
-        payload.append({"Name":r["name"], "Variant":r["variant"],"Type":r["resource_type"]})
+        payload.append(
+            {"Name": r["name"], "Variant": r["variant"], "Type": r["resource_type"]}
+        )
 
     return json.dumps(payload)
```

### Comparing `featureform-1.7.4/src/featureform/enums.py` & `featureform-1.8.0/src/featureform/enums.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/format.py` & `featureform-1.8.0/src/featureform/format.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,52 +10,86 @@
 two_row_spacing = "{:<30} {:<25}"
 three_row_spacing = "{:<30} {:<30} {:<30}"
 four_row_spacing = "{:<30} {:<30} {:<30} {:<30}"
 five_row_spacing = "{:<30} {:<30} {:<30} {:<30} {:<30}"
 divider = "-----------------------------------------------"
 
 # maximum number of dots printing when featureform apply for Running...
-MAX_NUM_RUNNING_DOTS = 10 
+MAX_NUM_RUNNING_DOTS = 10
 
-def format_rows(format_obj, format_obj_2=None, format_obj_3=None, format_obj_4=None, format_obj_5=None):
+
+def format_rows(
+    format_obj,
+    format_obj_2=None,
+    format_obj_3=None,
+    format_obj_4=None,
+    format_obj_5=None,
+):
     # Base case for when `format_obj` is a string
     if format_obj_2 is None and type(format_obj) == str:
         print(format_obj)
     elif format_obj_2 is None:
         for s in format_obj:
             format_rows(*s)
     elif format_obj_2 is not None and format_obj_3 is None:
         print(two_row_spacing.format(format_obj, format_obj_2))
     elif format_obj_2 is not None and format_obj_3 is not None and format_obj_4 is None:
         print(three_row_spacing.format(format_obj, format_obj_2, format_obj_3))
-    elif format_obj_2 is not None and format_obj_3 is not None and format_obj_4 is not None and format_obj_5 is None:
-        print(four_row_spacing.format(format_obj, format_obj_2, format_obj_3, format_obj_4))
+    elif (
+        format_obj_2 is not None
+        and format_obj_3 is not None
+        and format_obj_4 is not None
+        and format_obj_5 is None
+    ):
+        print(
+            four_row_spacing.format(
+                format_obj, format_obj_2, format_obj_3, format_obj_4
+            )
+        )
     else:
-        print(five_row_spacing.format(format_obj, format_obj_2, format_obj_3, format_obj_4, format_obj_5))
+        print(
+            five_row_spacing.format(
+                format_obj, format_obj_2, format_obj_3, format_obj_4, format_obj_5
+            )
+        )
 
 
 def format_pg(s=""):
     print(divider)
     print(s)
 
 
 def display_statuses(stub, resources):
-    from featureform.resources import Feature, OnDemandFeature, TrainingSet, Label, Source, Provider
+    from featureform.resources import (
+        Feature,
+        OnDemandFeature,
+        TrainingSet,
+        Label,
+        Source,
+        Provider,
+    )
 
     @dataclass
     class Status:
         resource_type: Type
         name: str
         variant: str
         status: str
         error: str
 
     def get_statuses() -> List[Status]:
         statuses = []
-        resources_to_check = {Feature, OnDemandFeature, TrainingSet, Label, Source, Provider}
+        resources_to_check = {
+            Feature,
+            OnDemandFeature,
+            TrainingSet,
+            Label,
+            Source,
+            Provider,
+        }
         filtered_resources = filter(lambda r: type(r) in resources_to_check, resources)
         for r in filtered_resources:
             if r.name == "local-mode":
                 continue
             resource = r.get(stub)
             variant = getattr(resource, "variant", "")
             status = Status(
@@ -82,19 +116,21 @@
     print()
     console = Console()
     with Live(console=console, auto_refresh=True, screen=False) as live:
         i = 0
         while True:
             statuses = get_statuses()
             finished_running = is_finished(statuses)
-            
-            dots = "."*(1 + i%MAX_NUM_RUNNING_DOTS)
+
+            dots = "." * (1 + i % MAX_NUM_RUNNING_DOTS)
 
             title = (
-                f"[green]COMPLETED[/]" if finished_running else f"[yellow]RUNNING{dots}[/]"
+                f"[green]COMPLETED[/]"
+                if finished_running
+                else f"[yellow]RUNNING{dots}[/]"
             )
             table = Table(
                 title=title,
                 title_justify="left",
                 show_header=True,
                 header_style="bold",
                 box=None,
@@ -121,15 +157,15 @@
                 }
 
                 style = status_to_color[status_text]
                 table.add_row(
                     Text(resource_type),
                     Text(f"{name} ({status.variant})"),
                     Text(status_text, style=status_to_color[status_text]),
-                    Text(error, style="red")
+                    Text(error, style="red"),
                 )
 
             live.update(table)
             live.refresh()
 
             if finished_running:
                 break
```

### Comparing `featureform-1.7.4/src/featureform/get.py` & `featureform-1.8.0/src/featureform/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,101 +1,111 @@
 from featureform.proto import metadata_pb2
 import grpc
 from featureform.proto import metadata_pb2_grpc as ff_grpc
 from .format import *
 
+
 def get_user_info(stub, name):
     searchName = metadata_pb2.Name(name=name)
     try:
         for user in stub.GetUsers(iter([searchName])):
             format_rows("USER NAME: ", user.name)
             format_tags_and_properties(user.tags, user.properties)
             format_pg()
-            format_rows('NAME', 'VARIANT', 'TYPE')
+            format_rows("NAME", "VARIANT", "TYPE")
             for f in user.features:
-                format_rows(
-                    f.name, f.variant, "feature")
+                format_rows(f.name, f.variant, "feature")
             for l in user.labels:
-                format_rows(
-                    l.name, l.variant, "label")
+                format_rows(l.name, l.variant, "label")
             for t in user.trainingsets:
-                format_rows(
-                    t.name, t.variant, "training set")
+                format_rows(t.name, t.variant, "training set")
             for s in user.sources:
-                format_rows(
-                    s.name, s.variant, "source")
+                format_rows(s.name, s.variant, "source")
             format_pg()
             return user
     except grpc._channel._MultiThreadedRendezvous:
         print("User not found.")
 
+
 def get_entity_info(stub, name):
     searchName = metadata_pb2.Name(name=name)
     try:
         for x in stub.GetEntities(iter([searchName])):
-            format_rows([("ENTITY NAME: ", x.name),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)])
+            format_rows(
+                [
+                    ("ENTITY NAME: ", x.name),
+                    (
+                        "STATUS: ",
+                        x.status.Status._enum_type.values[x.status.status].name,
+                    ),
+                ]
+            )
             format_tags_and_properties(x.tags, x.properties)
             format_pg()
-            format_rows('NAME', 'VARIANT', 'TYPE')
+            format_rows("NAME", "VARIANT", "TYPE")
             for f in x.features:
-                format_rows(
-                    f.name, f.variant, "feature")
+                format_rows(f.name, f.variant, "feature")
             for l in x.labels:
-                format_rows(
-                    l.name, l.variant, "label")
+                format_rows(l.name, l.variant, "label")
             for t in x.trainingsets:
-                format_rows(
-                    t.name, t.variant, "training set")
+                format_rows(t.name, t.variant, "training set")
             format_pg()
             return x
     except grpc._channel._MultiThreadedRendezvous:
         print("Entity not found.")
 
+
 def get_resource_info(stub, resource_type, name):
     stub_get_functions = {
         "feature": stub.GetFeatures,
         "label": stub.GetLabels,
         "source": stub.GetSources,
         "trainingset": stub.GetTrainingSets,
         "training-set": stub.GetTrainingSets,
-        "model": stub.GetModels
+        "model": stub.GetModels,
     }
 
     searchName = metadata_pb2.Name(name=name)
     try:
         for x in stub_get_functions[resource_type](iter([searchName])):
             rows = [("NAME: ", x.name)]
             if hasattr(x, '"status'):
-                rows.append(("STATUS: ", x.status.Status._enum_type.values[x.status.status].name))
+                rows.append(
+                    (
+                        "STATUS: ",
+                        x.status.Status._enum_type.values[x.status.status].name,
+                    )
+                )
             format_rows(rows)
             if hasattr(x, "default_variant"):
                 format_pg("VARIANTS:")
-                format_rows(x.default_variant, 'default')
+                format_rows(x.default_variant, "default")
                 for v in x.variants:
                     if v != x.default_variant:
-                        format_rows(v, '')
+                        format_rows(v, "")
                 format_pg()
             return x
     except grpc._channel._MultiThreadedRendezvous:
         print(f"{resource_type} not found.")
 
+
 def get_feature_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetFeatureVariants(iter([searchNameVariant])):
             status = x.status.Status._enum_type.values[x.status.status].name
-            rows = [("NAME: ", x.name),
-            ("VARIANT: ", x.variant), 
-            ("TYPE:", x.type), 
-            ("ENTITY:", x.entity),
-            ("OWNER:", x.owner),
-            ("DESCRIPTION:", x.description),
-            ("PROVIDER:", x.provider),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)
+            rows = [
+                ("NAME: ", x.name),
+                ("VARIANT: ", x.variant),
+                ("TYPE:", x.type),
+                ("ENTITY:", x.entity),
+                ("OWNER:", x.owner),
+                ("DESCRIPTION:", x.description),
+                ("PROVIDER:", x.provider),
+                ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name),
             ]
             if status == "FAILED":
                 rows.append(("ERROR: ", x.status.error_message))
             format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("SOURCE: ")
             format_rows([("NAME", "VARIANT"), (x.source.name, x.source.variant)])
@@ -104,27 +114,30 @@
             for t in x.trainingsets:
                 format_rows(t.name, t.variant)
             format_pg()
             return x
     except grpc._channel._MultiThreadedRendezvous:
         print("Feature variant not found.")
 
+
 def get_label_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetLabelVariants(iter([searchNameVariant])):
             status = x.status.Status._enum_type.values[x.status.status].name
-            rows = [("NAME: ", x.name),
-            ("VARIANT: ", x.variant), 
-            ("TYPE:", x.type), 
-            ("ENTITY:", x.entity), 
-            ("OWNER:", x.owner), 
-            ("DESCRIPTION:", x.description),
-            ("PROVIDER:", x.provider),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            rows = [
+                ("NAME: ", x.name),
+                ("VARIANT: ", x.variant),
+                ("TYPE:", x.type),
+                ("ENTITY:", x.entity),
+                ("OWNER:", x.owner),
+                ("DESCRIPTION:", x.description),
+                ("PROVIDER:", x.provider),
+                ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name),
+            ]
             if status == "FAILED":
                 rows.append(("ERROR: ", x.status.error_message))
             format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("SOURCE: ")
             format_rows([("NAME", "VARIANT"), (x.source.name, x.source.variant)])
             format_pg("TRAINING SETS:")
@@ -132,26 +145,29 @@
             for t in x.trainingsets:
                 format_rows(t.name, t.variant)
             format_pg()
             return x
     except grpc._channel._MultiThreadedRendezvous:
         print("Label variant not found.")
 
+
 def get_source_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetSourceVariants(iter([searchNameVariant])):
             status = x.status.Status._enum_type.values[x.status.status].name
-            rows = [("NAME: ", x.name),
-            ("VARIANT: ", x.variant), 
-            ("OWNER:", x.owner),
-            ("DESCRIPTION:", x.description),
-            ("PROVIDER:", x.provider),
-            ("TABLE:", x.table),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            rows = [
+                ("NAME: ", x.name),
+                ("VARIANT: ", x.variant),
+                ("OWNER:", x.owner),
+                ("DESCRIPTION:", x.description),
+                ("PROVIDER:", x.provider),
+                ("TABLE:", x.table),
+                ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name),
+            ]
             if status == "FAILED":
                 rows.append(("ERROR: ", x.status.error_message))
             format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("DEFINITION:")
             print("TRANSFORMATION")
             print(x.transformation.SQLTransformation.query)
@@ -174,25 +190,28 @@
             for t in x.trainingsets:
                 format_rows(t.name, t.variant)
             format_pg()
             return x
     except grpc._channel._MultiThreadedRendezvous:
         print("Source variant not found.")
 
+
 def get_training_set_variant_info(stub, name, variant):
     searchNameVariant = metadata_pb2.NameVariant(name=name, variant=variant)
     try:
         for x in stub.GetTrainingSetVariants(iter([searchNameVariant])):
             status = x.status.Status._enum_type.values[x.status.status].name
-            rows = [("NAME: ", x.name),
-            ("VARIANT: ", x.variant),
-            ("OWNER:", x.owner),
-            ("DESCRIPTION:", x.description),
-            ("PROVIDER:", x.provider),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            rows = [
+                ("NAME: ", x.name),
+                ("VARIANT: ", x.variant),
+                ("OWNER:", x.owner),
+                ("DESCRIPTION:", x.description),
+                ("PROVIDER:", x.provider),
+                ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name),
+            ]
             if status == "FAILED":
                 rows.append(("ERROR: ", x.status.error_message))
             format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("LABEL: ")
             format_rows([("NAME", "VARIANT"), (x.label.name, x.label.variant)])
             format_pg("FEATURES:")
@@ -200,25 +219,28 @@
             for f in x.features:
                 format_rows(f.name, f.variant)
             format_pg()
             return x
     except grpc._channel._MultiThreadedRendezvous:
         print("Training set variant not found.")
 
+
 def get_provider_info(stub, name):
     searchName = metadata_pb2.Name(name=name)
     try:
         for x in stub.GetProviders(iter([searchName])):
             status = x.status.Status._enum_type.values[x.status.status].name
-            rows = [("NAME: ", x.name),
-            ("DESCRIPTION: ", x.description),
-            ("TYPE: ", x.type),
-            ("SOFTWARE: ", x.software),
-            ("TEAM: ", x.team),
-            ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name)]
+            rows = [
+                ("NAME: ", x.name),
+                ("DESCRIPTION: ", x.description),
+                ("TYPE: ", x.type),
+                ("SOFTWARE: ", x.software),
+                ("TEAM: ", x.team),
+                ("STATUS: ", x.status.Status._enum_type.values[x.status.status].name),
+            ]
             if status == "FAILED":
                 rows.append(("ERROR: ", x.status.error_message))
             format_rows(rows)
             format_tags_and_properties(x.tags, x.properties)
             format_pg("SOURCES:")
             format_rows("NAME", "VARIANT")
             for s in x.sources:
@@ -241,8 +263,13 @@
         print("Provider not found.")
 
 
 def format_tags_and_properties(tags, properties):
     if len(tags.tag):
         format_rows("TAGS:", ", ".join(tags.tag))
     if len(properties.property.items()):
-        format_rows("PROPERTIES:", ", ".join([f"{k}:{v.string_value}" for (k,v) in properties.property.items()]))
+        format_rows(
+            "PROPERTIES:",
+            ", ".join(
+                [f"{k}:{v.string_value}" for (k, v) in properties.property.items()]
+            ),
+        )
```

### Comparing `featureform-1.7.4/src/featureform/get_local.py` & `featureform-1.8.0/src/featureform/get_local.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,85 @@
 import json
 from .format import *
 from .sqlite_metadata import *
 from .resources import Model
 
+
 def get_user_info_local(name):
     user = get_resource("user", name, True)
 
     format_rows("USER NAME: ", user["name"])
     format_rows("TYPE: ", user["type"])
     format_rows("STATUS: ", user["status"])
     tags = json.loads(user["tags"]) if user["tags"] is not None else []
-    properties = json.loads(user["properties"]) if user["properties"] is not None else {}
+    properties = (
+        json.loads(user["properties"]) if user["properties"] is not None else {}
+    )
     format_tags_and_properties(tags, properties)
     return {**user, "tags": tags, "properties": properties}
 
+
 def get_entity_info_local(name):
     db = SQLiteMetadata()
     entity = get_resource("entity", name, True)
-    
-    returned_features_query_list = get_related_resources("feature_variant", "entity", name)
+
+    returned_features_query_list = get_related_resources(
+        "feature_variant", "entity", name
+    )
     returned_features_list = format_resource_list(returned_features_query_list)
 
     returned_labels_query_list = get_related_resources("label_variant", "entity", name)
     returned_labels_list = format_resource_list(returned_labels_query_list)
 
     training_set_list = set()
     for f in returned_features_list:
         try:
-            training_set_features_query_list = db.get_training_set_from_features(f["name"], f["variant"])
+            training_set_features_query_list = db.get_training_set_from_features(
+                f["name"], f["variant"]
+            )
         except ValueError:
             training_set_features_query_list = []
         for t in training_set_features_query_list:
             training_set_list.add(t)
 
-    returned_training_sets_list = format_resource_list(training_set_list, "training_set_name", "training_set_variant")
-    
+    returned_training_sets_list = format_resource_list(
+        training_set_list, "training_set_name", "training_set_variant"
+    )
+
     returned_entity = {
         "name": name,
         "status": entity["status"],
         "features": returned_features_list,
         "labels": returned_labels_list,
         "trainingsets": returned_training_sets_list,
         "tags": json.loads(entity["tags"]) if entity["tags"] is not None else [],
-        "properties": json.loads(entity["properties"]) if entity["properties"] is not None else {},
+        "properties": json.loads(entity["properties"])
+        if entity["properties"] is not None
+        else {},
     }
 
-    format_rows([("ENTITY NAME: ", returned_entity["name"]),
-    ("STATUS: ", returned_entity["status"])])
+    format_rows(
+        [
+            ("ENTITY NAME: ", returned_entity["name"]),
+            ("STATUS: ", returned_entity["status"]),
+        ]
+    )
     format_tags_and_properties(returned_entity["tags"], returned_entity["properties"])
     format_pg()
-    format_rows('NAME', 'VARIANT', 'TYPE')
+    format_rows("NAME", "VARIANT", "TYPE")
     for f in returned_entity["features"]:
-        format_rows(
-            f["name"], f["variant"], "feature")
+        format_rows(f["name"], f["variant"], "feature")
     for l in returned_entity["labels"]:
-        format_rows(
-            l["name"], l["variant"], "label")
+        format_rows(l["name"], l["variant"], "label")
     for t in returned_entity["trainingsets"]:
-        format_rows(
-            t["name"], t["variant"], "training set")
+        format_rows(t["name"], t["variant"], "training set")
     format_pg()
     return returned_entity
 
+
 def get_resource_info_local(resource_type, name):
     resource = get_resource(resource_type, name)
 
     variants_list = get_variant_list(resource_type, name)
 
     returned_resource_list = {
         "name": resource["name"],
@@ -78,170 +92,211 @@
         format_rows("STATUS: ", resource["status"])
     format_pg("VARIANTS:")
     formatted_variants = [("NAME", "DEFAULT", "TAGS", "PROPERTIES")]
     for v, t, p in returned_resource_list["variants"]:
         t = json.loads(t) if t is not None else []
         p = json.loads(p) if p is not None else {}
         default = "" if v != returned_resource_list["default_variant"] else "default"
-        formatted_variants.append((v, default, ", ".join(t), ", ".join([f"{k}:{v}" for (k,v) in p.items()])))
+        formatted_variants.append(
+            (v, default, ", ".join(t), ", ".join([f"{k}:{v}" for (k, v) in p.items()]))
+        )
     format_rows(formatted_variants)
     format_pg()
     return returned_resource_list
 
+
 def get_feature_variant_info_local(name, variant):
     db = SQLiteMetadata()
     feature = get_variant("feature", name, variant)
 
     try:
-        returned_training_sets_query_list = db.get_training_set_from_features(feature["name"], feature["variant"])
+        returned_training_sets_query_list = db.get_training_set_from_features(
+            feature["name"], feature["variant"]
+        )
     except ValueError:
         returned_training_sets_query_list = []
-    returned_training_sets_list = format_resource_list(returned_training_sets_query_list, "training_set_name", "training_set_variant")
+    returned_training_sets_list = format_resource_list(
+        returned_training_sets_query_list, "training_set_name", "training_set_variant"
+    )
 
     returned_feature = {
         "name": feature["name"],
         "variant": feature["variant"],
         "type": feature["data_type"],
         "entity": feature["entity"],
         "owner": feature["owner"],
         "description": feature["description"],
         "provider": feature["provider"],
         "status": feature["status"],
-        "source": { 
+        "source": {
             "name": feature["source_name"],
-            "variant": feature["source_variant"]
+            "variant": feature["source_variant"],
         },
         "trainingsets": returned_training_sets_list,
         "tags": json.loads(feature["tags"]) if feature["tags"] is not None else [],
-        "properties": json.loads(feature["properties"]) if feature["properties"] is not None else {},
-
+        "properties": json.loads(feature["properties"])
+        if feature["properties"] is not None
+        else {},
     }
-    format_rows([("NAME: ", returned_feature["name"]), 
-    ("VARIANT: ", returned_feature["variant"]), 
-    ("TYPE:", returned_feature["type"]), 
-    ("ENTITY:", returned_feature["entity"]),
-    ("OWNER:", returned_feature["owner"]),
-    ("DESCRIPTION:", returned_feature["description"]),
-    ("PROVIDER:", returned_feature["provider"]),
-    ("STATUS: ", returned_feature["status"])
-    ])
+    format_rows(
+        [
+            ("NAME: ", returned_feature["name"]),
+            ("VARIANT: ", returned_feature["variant"]),
+            ("TYPE:", returned_feature["type"]),
+            ("ENTITY:", returned_feature["entity"]),
+            ("OWNER:", returned_feature["owner"]),
+            ("DESCRIPTION:", returned_feature["description"]),
+            ("PROVIDER:", returned_feature["provider"]),
+            ("STATUS: ", returned_feature["status"]),
+        ]
+    )
     format_tags_and_properties(returned_feature["tags"], returned_feature["properties"])
     format_pg("SOURCE: ")
-    format_rows([("NAME", "VARIANT"), (returned_feature["source"]["name"], returned_feature["source"]["variant"])])
+    format_rows(
+        [
+            ("NAME", "VARIANT"),
+            (returned_feature["source"]["name"], returned_feature["source"]["variant"]),
+        ]
+    )
     format_pg("TRAINING SETS:")
     format_rows("NAME", "VARIANT")
     for t in returned_feature["trainingsets"]:
         format_rows(t["name"], t["variant"])
     format_pg()
     return returned_feature
 
+
 def get_label_variant_info_local(name, variant):
     db = SQLiteMetadata()
     label = get_variant("label", name, variant)
 
     try:
-        returned_training_sets_query_list = db.get_training_set_from_labels(label["name"], label["variant"])
+        returned_training_sets_query_list = db.get_training_set_from_labels(
+            label["name"], label["variant"]
+        )
     except ValueError:
         returned_training_sets_query_list = []
-    
-    returned_training_sets_list = format_resource_list(returned_training_sets_query_list)
+
+    returned_training_sets_list = format_resource_list(
+        returned_training_sets_query_list
+    )
 
     returned_label = {
         "name": label["name"],
         "variant": label["variant"],
         "type": label["data_type"],
         "entity": label["entity"],
         "owner": label["owner"],
         "description": label["description"],
         "provider": label["provider"],
         "status": label["status"],
-        "source": { 
-            "name": label["source_name"],
-            "variant": label["source_variant"]
-        },
+        "source": {"name": label["source_name"], "variant": label["source_variant"]},
         "trainingsets": returned_training_sets_list,
         "tags": json.loads(label["tags"]) if label["tags"] is not None else [],
-        "properties": json.loads(label["properties"]) if label["properties"] is not None else {},
+        "properties": json.loads(label["properties"])
+        if label["properties"] is not None
+        else {},
     }
-    format_rows([("NAME: ", returned_label["name"]), 
-    ("VARIANT: ", returned_label["variant"]), 
-    ("TYPE:", returned_label["type"]), 
-    ("ENTITY:", returned_label["entity"]),
-    ("OWNER:", returned_label["owner"]),
-    ("DESCRIPTION:", returned_label["description"]),
-    ("PROVIDER:", returned_label["provider"]),
-    ("STATUS: ", returned_label["status"])
-    ])
+    format_rows(
+        [
+            ("NAME: ", returned_label["name"]),
+            ("VARIANT: ", returned_label["variant"]),
+            ("TYPE:", returned_label["type"]),
+            ("ENTITY:", returned_label["entity"]),
+            ("OWNER:", returned_label["owner"]),
+            ("DESCRIPTION:", returned_label["description"]),
+            ("PROVIDER:", returned_label["provider"]),
+            ("STATUS: ", returned_label["status"]),
+        ]
+    )
     format_tags_and_properties(returned_label["tags"], returned_label["properties"])
     format_pg("SOURCE: ")
-    format_rows([("NAME", "VARIANT"), (returned_label["source"]["name"], returned_label["source"]["variant"])])
+    format_rows(
+        [
+            ("NAME", "VARIANT"),
+            (returned_label["source"]["name"], returned_label["source"]["variant"]),
+        ]
+    )
     format_pg("TRAINING SETS:")
     format_rows("NAME", "VARIANT")
     for t in returned_label["trainingsets"]:
         format_rows(t["name"], t["variant"])
     format_pg()
     return returned_label
 
+
 def get_source_variant_info_local(name, variant):
     db = SQLiteMetadata()
     source = get_variant("source", name, variant)
 
     try:
-        returned_features_query_list = db.get_feature_variants_from_source(name, variant)
+        returned_features_query_list = db.get_feature_variants_from_source(
+            name, variant
+        )
         returned_features_list = format_resource_list(returned_features_query_list)
     except ValueError:
         returned_features_list = []
 
     try:
         returned_labels_query_list = db.get_label_variants_from_source(name, variant)
         returned_labels_list = format_resource_list(returned_labels_query_list)
     except ValueError:
         returned_labels_list = []
 
     training_set_list = set()
 
     for f in returned_features_list:
         try:
-            training_set_features_query_list = db.get_training_set_from_features(f["name"], f["variant"])
+            training_set_features_query_list = db.get_training_set_from_features(
+                f["name"], f["variant"]
+            )
         except ValueError:
             training_set_features_query_list = []
         for t in training_set_features_query_list:
             training_set_list.add(t)
-    
+
     for l in returned_labels_list:
         try:
-            training_set_labels_query_list = db.get_training_set_variant_from_label(l["name"], l["variant"])
+            training_set_labels_query_list = db.get_training_set_variant_from_label(
+                l["name"], l["variant"]
+            )
         except ValueError:
             training_set_labels_query_list = []
         for t in training_set_labels_query_list:
             training_set_list.add(t)
 
     returned_training_sets_list = format_resource_list(training_set_list)
-    
+
     returned_source = {
         "name": source["name"],
         "variant": source["variant"],
         "owner": source["owner"],
         "description": source["description"],
         "provider": source["provider"],
         "status": source["status"],
         "definition": source["definition"],
         "features": returned_features_list,
         "labels": returned_labels_list,
         "trainingsets": returned_training_sets_list,
         "tags": json.loads(source["tags"]) if source["tags"] is not None else [],
-        "properties": json.loads(source["properties"]) if source["properties"] is not None else {},
+        "properties": json.loads(source["properties"])
+        if source["properties"] is not None
+        else {},
     }
 
-    format_rows([("NAME: ", returned_source["name"]),
-    ("VARIANT: ", returned_source["variant"]), 
-    ("OWNER:", returned_source["owner"]),
-    ("DESCRIPTION:", returned_source["description"]),
-    ("PROVIDER:", returned_source["provider"]),
-    ("STATUS: ", returned_source["status"])])
+    format_rows(
+        [
+            ("NAME: ", returned_source["name"]),
+            ("VARIANT: ", returned_source["variant"]),
+            ("OWNER:", returned_source["owner"]),
+            ("DESCRIPTION:", returned_source["description"]),
+            ("PROVIDER:", returned_source["provider"]),
+            ("STATUS: ", returned_source["status"]),
+        ]
+    )
     format_tags_and_properties(returned_source["tags"], returned_source["properties"])
     format_pg("DEFINITION:")
     print(returned_source["definition"])
     print("FEATURES:")
     format_rows("NAME", "VARIANT")
     for f in returned_source["features"]:
         format_rows(f["name"], f["variant"])
@@ -252,164 +307,202 @@
     format_pg("TRAINING SETS:")
     format_rows("NAME", "VARIANT")
     for t in returned_source["trainingsets"]:
         format_rows(t["name"], t["variant"])
     format_pg()
     return returned_source
 
+
 def get_training_set_variant_info_local(name, variant):
     db = SQLiteMetadata()
     training_set = get_variant("training-set", name, variant)
 
     try:
         returned_features_query_list = db.get_training_set_features(name, variant)
     except ValueError:
         returned_features_query_list = []
-    returned_features_list = format_resource_list(returned_features_query_list, "feature_name", "feature_variant")
-    
+    returned_features_list = format_resource_list(
+        returned_features_query_list, "feature_name", "feature_variant"
+    )
+
     returned_training_set = {
         "name": training_set["name"],
         "variant": training_set["variant"],
         "owner": training_set["owner"],
         "description": training_set["description"],
         "status": training_set["status"],
         "label": {
             "name": training_set["label_name"],
-            "variant": training_set["label_variant"]
+            "variant": training_set["label_variant"],
         },
         "features": returned_features_list,
-        "tags": json.loads(training_set["tags"]) if training_set["tags"] is not None else [],
-        "properties": json.loads(training_set["properties"]) if training_set["properties"] is not None else {},
+        "tags": json.loads(training_set["tags"])
+        if training_set["tags"] is not None
+        else [],
+        "properties": json.loads(training_set["properties"])
+        if training_set["properties"] is not None
+        else {},
     }
 
-    format_rows([("NAME: ", returned_training_set["name"]),
-    ("VARIANT: ", returned_training_set["variant"]),
-    ("OWNER:", returned_training_set["owner"]),
-    ("DESCRIPTION:", returned_training_set["description"]),
-    ("STATUS: ", returned_training_set["status"])])
-    format_tags_and_properties(returned_training_set["tags"], returned_training_set["properties"])
+    format_rows(
+        [
+            ("NAME: ", returned_training_set["name"]),
+            ("VARIANT: ", returned_training_set["variant"]),
+            ("OWNER:", returned_training_set["owner"]),
+            ("DESCRIPTION:", returned_training_set["description"]),
+            ("STATUS: ", returned_training_set["status"]),
+        ]
+    )
+    format_tags_and_properties(
+        returned_training_set["tags"], returned_training_set["properties"]
+    )
     format_pg("LABEL: ")
-    format_rows([("NAME", "VARIANT"), (returned_training_set["label"]["name"], returned_training_set["label"]["variant"])])
+    format_rows(
+        [
+            ("NAME", "VARIANT"),
+            (
+                returned_training_set["label"]["name"],
+                returned_training_set["label"]["variant"],
+            ),
+        ]
+    )
     format_pg("FEATURES:")
     format_rows("NAME", "VARIANT")
     for f in returned_training_set["features"]:
         format_rows(f["name"], f["variant"])
     format_pg()
     return returned_training_set
 
+
 def get_provider_info_local(name):
     db = SQLiteMetadata()
     provider = get_resource("provider", name, True)
 
     try:
         returned_features_query_list = db.get_feature_variants_from_provider(name)
         returned_features_list = format_resource_list(returned_features_query_list)
     except ValueError:
         returned_features_list = []
 
     try:
         returned_labels_query_list = db.get_label_variants_from_provider(name)
-        returned_labels_list = format_resource_list(returned_labels_query_list)                         
+        returned_labels_list = format_resource_list(returned_labels_query_list)
     except ValueError:
         returned_labels_list = []
-    
+
     returned_provider = {
         "name": provider["name"],
         "type": provider["type"],
         "description": provider["description"],
         "type": provider["provider_type"],
         "software": provider["software"],
         "team": provider["team"],
         "status": provider["status"],
         "serializedConfig": provider["serialized_config"],
         "sources": provider["sources"],
         "features": returned_features_list,
         "labels": returned_labels_list,
         "tags": json.loads(provider["tags"]) if provider["tags"] is not None else [],
-        "properties": json.loads(provider["properties"]) if provider["properties"] is not None else {},
+        "properties": json.loads(provider["properties"])
+        if provider["properties"] is not None
+        else {},
     }
 
-    format_rows([("NAME: ", returned_provider["name"]),
-    ("DESCRIPTION: ", returned_provider["description"]),
-    ("TYPE: ", returned_provider["type"]),
-    ("SOFTWARE: ", returned_provider["software"]),
-    ("TEAM: ", returned_provider["team"]),
-    ("STATUS: ", returned_provider["status"])])
-    format_tags_and_properties(returned_provider["tags"], returned_provider["properties"])
+    format_rows(
+        [
+            ("NAME: ", returned_provider["name"]),
+            ("DESCRIPTION: ", returned_provider["description"]),
+            ("TYPE: ", returned_provider["type"]),
+            ("SOFTWARE: ", returned_provider["software"]),
+            ("TEAM: ", returned_provider["team"]),
+            ("STATUS: ", returned_provider["status"]),
+        ]
+    )
+    format_tags_and_properties(
+        returned_provider["tags"], returned_provider["properties"]
+    )
     format_rows("SOURCE:", returned_provider["sources"])
     format_pg("FEATURES:")
     format_rows("NAME", "VARIANT")
     for f in returned_provider["features"]:
         format_rows(f["name"], f["variant"])
     format_pg("LABELS:")
     format_rows("NAME", "VARIANT")
     for l in returned_provider["labels"]:
         format_rows(l["name"], l["variant"])
     format_pg()
     return returned_provider
 
+
 def get_related_resources(table, column, name):
     db = SQLiteMetadata()
     try:
         res_list = db.query_resource(table, column, name)
     except ValueError:
         res_list = []
     return res_list
 
+
 def get_resource(resource_type, name, should_fetch_tags_properties=False):
     db = SQLiteMetadata()
     resource_sql_functions = {
         "user": db.get_user,
         "entity": db.get_entity,
         "feature": db.get_feature,
         "label": db.get_label,
         "source": db.get_source,
         "training-set": db.get_training_set,
         "model": db.get_model,
-        "provider": db.get_provider
+        "provider": db.get_provider,
     }
     res_list = resource_sql_functions[resource_type](name, should_fetch_tags_properties)
     return res_list
 
+
 def get_variant_list(resource_type, name):
     db = SQLiteMetadata()
     variant_list_sql_functions = {
         "feature": db.get_feature_variants_from_feature,
         "label": db.get_label_variants_from_label,
         "source": db.get_source_variants_from_source,
-        "training-set": db.get_training_set_variant_from_training_set
+        "training-set": db.get_training_set_variant_from_training_set,
     }
-    
+
     res_list = variant_list_sql_functions[resource_type](name)
     return res_list
 
+
 def get_variant(resource_type, name, variant):
     db = SQLiteMetadata()
 
     variant_sql_functions = {
         "feature": db.get_feature_variant,
         "label": db.get_label_variant,
         "source": db.get_source_variant,
-        "training-set": db.get_training_set_variant
+        "training-set": db.get_training_set_variant,
     }
 
     res_list = variant_sql_functions[resource_type](name, variant)
     return res_list
 
+
 def format_resource_list(res_list, name_col="name", var_col="variant"):
-    formatted_res = [{ "name": r[name_col], "variant": r[var_col]} for r in res_list]
+    formatted_res = [{"name": r[name_col], "variant": r[var_col]} for r in res_list]
     return formatted_res
 
+
 def get_model_info_local(name) -> Model:
     model = get_resource("model", name)
 
     format_rows("MODEL NAME: ", model["name"])
     format_rows("TYPE: ", model["type"])
 
     return Model(model["name"], tags=[], properties={})
 
+
 def format_tags_and_properties(tags, properties):
     if len(tags):
         format_rows("TAGS:", ", ".join(tags))
     if len(properties):
-        format_rows("PROPERTIES:", ", ".join([f"{k}:{v}" for (k,v) in properties.items()]))
-
+        format_rows(
+            "PROPERTIES:", ", ".join([f"{k}:{v}" for (k, v) in properties.items()])
+        )
```

### Comparing `featureform-1.7.4/src/featureform/get_test.py` & `featureform-1.8.0/src/featureform/get_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 from .register import Client
 from io import StringIO
 from unittest.mock import patch
 import re
 import os
 
-rc = Client("localhost:8000", False, False, './tls.crt')
+rc = Client("localhost:8000", False, False, "./tls.crt")
+
 
 def check_print_return(expected_print, expected_return, resource_type):
-  rc_get_functions = {
-    "provider": [rc.get_provider, "redis-quickstart"],
-    "entity": [rc.get_entity, "user"],
-    "feature": [rc.get_feature, "avg_transactions"],
-    "label": [rc.get_label, "fraudulent"],
-    "user": [rc.get_user, "featureformer"],
-    "source": [rc.get_source, "transactions"],
-    "training_set": [rc.get_training_set, "fraud_training"]
-  }
-
-  rc_get_functions_var = {
-    "source_var": [rc.get_source, "transactions", "kaggle"],
-    "feature_var": [rc.get_feature, "avg_transactions", "quickstart"],
-    "label_var": [rc.get_label, "fraudulent", "quickstart"],
-    "training_set_var": [rc.get_training_set, "fraud_training", "quickstart"]
-  }
-
-  with patch('sys.stdout', new = StringIO()) as fake_out:
-    if resource_type in rc_get_functions:
-      value = rc_get_functions[resource_type][0](rc_get_functions[resource_type][1])
-    if resource_type in rc_get_functions_var:
-      value = rc_get_functions_var[resource_type][0](rc_get_functions_var[resource_type][1], rc_get_functions_var[resource_type][2])
-    assert (fake_out.getvalue().replace(" ","") == expected_print.replace(" ", ""))
-  assert re.match(expected_return.replace(" ", ""), str(value).replace(" ", ""))
+    rc_get_functions = {
+        "provider": [rc.get_provider, "redis-quickstart"],
+        "entity": [rc.get_entity, "user"],
+        "feature": [rc.get_feature, "avg_transactions"],
+        "label": [rc.get_label, "fraudulent"],
+        "user": [rc.get_user, "featureformer"],
+        "source": [rc.get_source, "transactions"],
+        "training_set": [rc.get_training_set, "fraud_training"],
+    }
+
+    rc_get_functions_var = {
+        "source_var": [rc.get_source, "transactions", "kaggle"],
+        "feature_var": [rc.get_feature, "avg_transactions", "quickstart"],
+        "label_var": [rc.get_label, "fraudulent", "quickstart"],
+        "training_set_var": [rc.get_training_set, "fraud_training", "quickstart"],
+    }
+
+    with patch("sys.stdout", new=StringIO()) as fake_out:
+        if resource_type in rc_get_functions:
+            value = rc_get_functions[resource_type][0](
+                rc_get_functions[resource_type][1]
+            )
+        if resource_type in rc_get_functions_var:
+            value = rc_get_functions_var[resource_type][0](
+                rc_get_functions_var[resource_type][1],
+                rc_get_functions_var[resource_type][2],
+            )
+        assert fake_out.getvalue().replace(" ", "") == expected_print.replace(" ", "")
+    assert re.match(expected_return.replace(" ", ""), str(value).replace(" ", ""))
+
 
 def test_get_provider():
-  expected_print_provider = """NAME:                          redis-quickstart
+    expected_print_provider = """NAME:                          redis-quickstart
                               DESCRIPTION:                   A Redis deployment we created for the Featureform quickstart
                               TYPE:                          REDIS_ONLINE
                               SOFTWARE:                      redis
                               STATUS:                        NO_STATUS
                               -----------------------------------------------
                               SOURCES:
                               NAME                           VARIANT
@@ -49,67 +56,68 @@
                               LABELS:
                               NAME                           VARIANT
                               -----------------------------------------------
                               TRAINING SETS:
                               NAME                           VARIANT
                               -----------------------------------------------\n
                               """
-  expected_return_provider = r"""name: "redis-quickstart"
+    expected_return_provider = r"""name: "redis-quickstart"
                                 description: "A Redis deployment we created for the Featureform quickstart"
                                 type: "REDIS_ONLINE"
                                 software: "redis"
                                 serialized_config: "{\\"Addr\\":\\"quickstart-redis:6379\\", \\"Password\\": \\"\\", \\"DB\\": 0}"
                                 features {
                                   name: "avg_transactions"
                                   variant: "quickstart"
                                 }
                                 """
-  check_print_return(expected_print_provider, expected_return_provider, "provider")
-  
+    check_print_return(expected_print_provider, expected_return_provider, "provider")
+
 
 def test_get_entity():
-  expected_print_entity = """ENTITY NAME:                   user
+    expected_print_entity = """ENTITY NAME:                   user
                           STATUS:                        NO_STATUS
                           -----------------------------------------------
 
                           NAME                           VARIANT                        TYPE
                           avg_transactions               quickstart                     feature
                           fraudulent                     quickstart                     label
                           fraud_training                 quickstart                     training set
                           -----------------------------------------------\n
                           """
-  expected_return_entity = r"""name: "user"
+    expected_return_entity = r"""name: "user"
                             features {
                               name: "avg_transactions"
                               variant: "quickstart"
                             }
                             labels {
                               name: "fraudulent"
                               variant: "quickstart"
                             }
                             trainingsets {
                               name: "fraud_training"
                               variant: "quickstart"
                             }
                             """
-  check_print_return(expected_print_entity, expected_return_entity, "entity")
+    check_print_return(expected_print_entity, expected_return_entity, "entity")
+
 
 def test_get_user():
-  expected_print_user = """USER NAME:                     featureformer
+    expected_print_user = """USER NAME:                     featureformer
                           -----------------------------------------------
 
                           NAME                           VARIANT                        TYPE
                           avg_transactions               quickstart                     feature
                           fraudulent                     quickstart                     label
                           fraud_training                 quickstart                     training set
                           transactions                   kaggle                         source
                           average_user_transaction       quickstart                     source
                           -----------------------------------------------\n
                           """
-  expected_return_user = r"""name: "featureformer"
+    expected_return_user = r"""name: "featureformer"
                             features {
                               name: "avg_transactions"
                               variant: "quickstart"
                             }
                             labels {
                               name: "fraudulent"
                               variant: "quickstart"
@@ -122,32 +130,34 @@
                               name: "transactions"
                               variant: "kaggle"
                             }
                             sources {
                               name: "average_user_transaction"
                               variant: "quickstart"
                             }\n"""
-  check_print_return(expected_print_user, expected_return_user, "user")
+    check_print_return(expected_print_user, expected_return_user, "user")
+
 
 def test_get_source():
-  expected_print_source = """NAME:                          transactions
+    expected_print_source = """NAME:                          transactions
                           STATUS:                        NO_STATUS
                           -----------------------------------------------
                           VARIANTS:
                           kaggle                         default
                           -----------------------------------------------\n
                           """
-  expected_return_source = r"""name: "transactions"
+    expected_return_source = r"""name: "transactions"
                             default_variant: "kaggle"
                             variants: "kaggle"
                             """
-  check_print_return(expected_print_source, expected_return_source, "source")
+    check_print_return(expected_print_source, expected_return_source, "source")
+
 
 def test_get_source_var():
-  expected_print_source_var = """NAME:                          transactions
+    expected_print_source_var = """NAME:                          transactions
                                 VARIANT:                       kaggle
                                 OWNER:                         featureformer
                                 DESCRIPTION:                   Fraud Dataset From Kaggle
                                 PROVIDER:                      postgres-quickstart
                                 STATUS:                        NO_STATUS
                                 -----------------------------------------------
                                 DEFINITION:
@@ -167,15 +177,15 @@
                                 fraudulent                     quickstart
                                 -----------------------------------------------
                                 TRAINING SETS:
                                 NAME                           VARIANT
                                 fraud_training                 quickstart
                                 -----------------------------------------------\n
                                 """
-  expected_return_source_var = r"""name: "transactions"
+    expected_return_source_var = r"""name: "transactions"
                                   variant: "kaggle"
                                   owner: "featureformer"
                                   description: "Fraud Dataset From Kaggle"
                                   provider: "postgres-quickstart"
                                   created {
                                     seconds: [0-9]+
                                     nanos: [0-9]+
@@ -190,32 +200,36 @@
                                   }
                                   primaryData {
                                     table {
                                       name: "Transactions"
                                     }
                                   }
                                   """
-  check_print_return(expected_print_source_var, expected_return_source_var, "source_var")
+    check_print_return(
+        expected_print_source_var, expected_return_source_var, "source_var"
+    )
+
 
 def test_get_feature():
-  expected_print_feature = """NAME:                          avg_transactions
+    expected_print_feature = """NAME:                          avg_transactions
                               STATUS:                        NO_STATUS
                               -----------------------------------------------
                               VARIANTS:
                               quickstart                     default
                               -----------------------------------------------\n
                           """
-  expected_return_feature = """name: "avg_transactions"
+    expected_return_feature = """name: "avg_transactions"
                               default_variant: "quickstart"
                               variants: "quickstart"
                               """
-  check_print_return(expected_print_feature, expected_return_feature, "feature")
+    check_print_return(expected_print_feature, expected_return_feature, "feature")
+
 
 def test_get_feature_var():
-  expected_print_feature_var = """NAME:                          avg_transactions
+    expected_print_feature_var = """NAME:                          avg_transactions
                                 VARIANT:                       quickstart
                                 TYPE:                          float32
                                 ENTITY:                        user
                                 OWNER:                         featureformer
                                 PROVIDER:                      redis-quickstart
                                 STATUS:                        NO_STATUS
                                 -----------------------------------------------
@@ -224,15 +238,15 @@
                                 average_user_transaction       quickstart
                                 -----------------------------------------------
                                 TRAINING SETS:
                                 NAME                           VARIANT
                                 fraud_training                 quickstart
                                 -----------------------------------------------\n
                                 """
-  expected_return_feature_var = r"""name: "avg_transactions"
+    expected_return_feature_var = r"""name: "avg_transactions"
                                   variant: "quickstart"
                                   source {
                                     name: "average_user_transaction"
                                     variant: "quickstart"
                                   }
                                   type: "float32"
                                   entity: "user"
@@ -247,32 +261,36 @@
                                     variant: "quickstart"
                                   }
                                   columns {
                                     entity: "user_id"
                                     value: "avg_transaction_amt"
                                   }
                                   """
-  check_print_return(expected_print_feature_var, expected_return_feature_var, "feature_var")
+    check_print_return(
+        expected_print_feature_var, expected_return_feature_var, "feature_var"
+    )
+
 
 def test_get_label():
-  expected_print_label = """NAME:                          fraudulent
+    expected_print_label = """NAME:                          fraudulent
                             STATUS:                        NO_STATUS
                             -----------------------------------------------
                             VARIANTS:
                             quickstart                     default
                             -----------------------------------------------\n
                           """
-  expected_return_label = """name: "fraudulent"
+    expected_return_label = """name: "fraudulent"
                               default_variant: "quickstart"
                               variants: "quickstart"
                               """
-  check_print_return(expected_print_label, expected_return_label, "label")
+    check_print_return(expected_print_label, expected_return_label, "label")
+
 
 def test_get_label_var():
-  expected_print_label_var = """NAME:                          fraudulent
+    expected_print_label_var = """NAME:                          fraudulent
                                   VARIANT:                       quickstart
                                   TYPE:                          bool
                                   ENTITY:                        user
                                   OWNER:                         featureformer
                                   PROVIDER:                      postgres-quickstart
                                   STATUS:                        NO_STATUS
                                   -----------------------------------------------
@@ -281,15 +299,15 @@
                                   transactions                   kaggle
                                   -----------------------------------------------
                                   TRAINING SETS:
                                   NAME                           VARIANT
                                   fraud_training                 quickstart
                                   -----------------------------------------------\n
                                 """
-  expected_return_label_var = r"""name: "fraudulent"
+    expected_return_label_var = r"""name: "fraudulent"
                                   variant: "quickstart"
                                   type: "bool"
                                   source {
                                     name: "transactions"
                                     variant: "kaggle"
                                   }
                                   entity: "user"
@@ -304,47 +322,51 @@
                                     variant: "quickstart"
                                   }
                                   columns {
                                     entity: "customerid"
                                     value: "isfraud"
                                   }
                                   """
-  check_print_return(expected_print_label_var, expected_return_label_var, "label_var")
+    check_print_return(expected_print_label_var, expected_return_label_var, "label_var")
+
 
 def test_get_training_set():
-  expected_print_training_set = """NAME:                          fraud_training
+    expected_print_training_set = """NAME:                          fraud_training
                                   STATUS:                        NO_STATUS
                                   -----------------------------------------------
                                   VARIANTS:
                                   quickstart                     default
                                   -----------------------------------------------\n
                                   """
-  expected_return_training_set = """name: "fraud_training"
+    expected_return_training_set = """name: "fraud_training"
                                     default_variant: "quickstart"
                                     variants: "quickstart"
                                     """
-  check_print_return(expected_print_training_set, expected_return_training_set, "training_set")
+    check_print_return(
+        expected_print_training_set, expected_return_training_set, "training_set"
+    )
+
 
 def test_get_training_set_var():
-  expected_print_training_set_var = """NAME:                          fraud_training
+    expected_print_training_set_var = """NAME:                          fraud_training
                                       VARIANT:                       quickstart
                                       OWNER:                         featureformer
                                       PROVIDER:                      postgres-quickstart
                                       STATUS:                        NO_STATUS
                                       -----------------------------------------------
                                       LABEL:
                                       NAME                           VARIANT
                                       fraudulent                     quickstart
                                       -----------------------------------------------
                                       FEATURES:
                                       NAME                           VARIANT
                                       avg_transactions               quickstart
                                       -----------------------------------------------\n
                                 """
-  expected_return_training_set_var = r"""name: "fraud_training"
+    expected_return_training_set_var = r"""name: "fraud_training"
                                         variant: "quickstart"
                                         owner: "featureformer"
                                         created {
                                           seconds: [0-9]+
                                           nanos: [0-9]+
                                         }
                                         provider: "postgres-quickstart"
@@ -353,8 +375,12 @@
                                           variant: "quickstart"
                                         }
                                         label {
                                           name: "fraudulent"
                                           variant: "quickstart"
                                         }
                                         """
-  check_print_return(expected_print_training_set_var, expected_return_training_set_var, "training_set_var")
+    check_print_return(
+        expected_print_training_set_var,
+        expected_return_training_set_var,
+        "training_set_var",
+    )
```

### Comparing `featureform-1.7.4/src/featureform/list.py` & `featureform-1.8.0/src/featureform/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,124 @@
 from featureform.proto import metadata_pb2
 from .format import *
 
 cutoff_length = 60
 
+
 def list_name(stub, resource_type):
     stub_list_functions = {
         "model": stub.ListModels,
     }
     format_rows("NAME")
-    res = sorted([received for received in stub_list_functions[resource_type](metadata_pb2.Empty())], key=lambda x:x.name)
+    res = sorted(
+        [
+            received
+            for received in stub_list_functions[resource_type](metadata_pb2.Empty())
+        ],
+        key=lambda x: x.name,
+    )
     for f in res:
         format_rows(f.name)
     return res
 
+
 def list_name_status(stub, resource_type):
-    stub_list_functions = {
-        "entity": stub.ListEntities,
-        "user": stub.ListUsers
-    }
+    stub_list_functions = {"entity": stub.ListEntities, "user": stub.ListUsers}
     format_rows("NAME", "STATUS")
-    res = sorted([received for received in stub_list_functions[resource_type](metadata_pb2.Empty())], key=lambda x:x.name)
+    res = sorted(
+        [
+            received
+            for received in stub_list_functions[resource_type](metadata_pb2.Empty())
+        ],
+        key=lambda x: x.name,
+    )
     for f in res:
         format_rows(f.name, f.status.Status._enum_type.values[f.status.status].name)
     return res
 
+
 def list_name_status_desc(stub, resource_type):
-    stub_list_functions = {
-        "model": stub.ListModels,
-        "provider": stub.ListProviders
-    }
+    stub_list_functions = {"model": stub.ListModels, "provider": stub.ListProviders}
     format_rows("NAME", "STATUS", "DESCRIPTION")
-    res = sorted([received for received in stub_list_functions[resource_type](metadata_pb2.Empty())], key=lambda x:x.name)
+    res = sorted(
+        [
+            received
+            for received in stub_list_functions[resource_type](metadata_pb2.Empty())
+        ],
+        key=lambda x: x.name,
+    )
     for f in res:
-        format_rows(f.name, f.status.Status._enum_type.values[f.status.status].name, f.description[:cutoff_length])
+        format_rows(
+            f.name,
+            f.status.Status._enum_type.values[f.status.status].name,
+            f.description[:cutoff_length],
+        )
     return res
 
+
 def list_name_variant_status(stub, resource_type):
     stub_list_functions = {
         "feature": [stub.ListFeatures, stub.GetFeatureVariants],
-        "label": [stub.ListLabels, stub.GetLabelVariants]
+        "label": [stub.ListLabels, stub.GetLabelVariants],
     }
 
     format_rows("NAME", "VARIANT", "STATUS")
-    res = sorted([received for received in stub_list_functions[resource_type][0](metadata_pb2.Empty())], key=lambda x:x.name)
+    res = sorted(
+        [
+            received
+            for received in stub_list_functions[resource_type][0](metadata_pb2.Empty())
+        ],
+        key=lambda x: x.name,
+    )
     for f in res:
         for v in f.variants:
             searchNameVariant = metadata_pb2.NameVariant(name=f.name, variant=v)
             for x in stub_list_functions[resource_type][1](iter([searchNameVariant])):
                 if x.variant == f.default_variant:
-                    format_rows(f.name, f"{f.default_variant} (default)", x.status.Status._enum_type.values[x.status.status].name)
+                    format_rows(
+                        f.name,
+                        f"{f.default_variant} (default)",
+                        x.status.Status._enum_type.values[x.status.status].name,
+                    )
                 else:
-                    format_rows(x.name, x.variant, x.status.Status._enum_type.values[x.status.status].name)
+                    format_rows(
+                        x.name,
+                        x.variant,
+                        x.status.Status._enum_type.values[x.status.status].name,
+                    )
     return res
 
+
 def list_name_variant_status_desc(stub, resource_type):
     stub_list_functions = {
         "source": [stub.ListSources, stub.GetSourceVariants],
         "training-set": [stub.ListTrainingSets, stub.GetTrainingSetVariants],
-        "trainingset": [stub.ListTrainingSets, stub.GetTrainingSetVariants]
+        "trainingset": [stub.ListTrainingSets, stub.GetTrainingSetVariants],
     }
 
     format_rows("NAME", "VARIANT", "STATUS", "DESCRIPTION")
-    res = sorted([received for received in stub_list_functions[resource_type][0](metadata_pb2.Empty())], key=lambda x:x.name)
+    res = sorted(
+        [
+            received
+            for received in stub_list_functions[resource_type][0](metadata_pb2.Empty())
+        ],
+        key=lambda x: x.name,
+    )
     for f in res:
         for v in f.variants:
             searchNameVariant = metadata_pb2.NameVariant(name=f.name, variant=v)
             for x in stub_list_functions[resource_type][1](iter([searchNameVariant])):
                 if x.variant == f.default_variant:
-                    format_rows(f.name, f"{f.default_variant} (default)", x.status.Status._enum_type.values[x.status.status].name, x.description)
+                    format_rows(
+                        f.name,
+                        f"{f.default_variant} (default)",
+                        x.status.Status._enum_type.values[x.status.status].name,
+                        x.description,
+                    )
                 else:
-                    format_rows(x.name, x.variant, x.status.Status._enum_type.values[x.status.status].name, x.description)
-    return res
+                    format_rows(
+                        x.name,
+                        x.variant,
+                        x.status.Status._enum_type.values[x.status.status].name,
+                        x.description,
+                    )
+    return res
```

### Comparing `featureform-1.7.4/src/featureform/list_local.py` & `featureform-1.8.0/src/featureform/list_local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 from .sqlite_metadata import *
 from .format import *
 from enum import Enum
 
 cutoff_length = 60
 
+
 def get_sorted_list(resource_type, variant=False):
     db = SQLiteMetadata()
     local_list_args = {
         "entity": ["entities"],
         "user": ["users"],
         "model": ["models"],
         "provider": ["providers"],
         "feature": ["features", "feature_variant"],
         "label": ["labels", "label_variant"],
         "source": ["sources", "source_variant"],
-        "training-set": ["training_sets", "training_set_variant"]
+        "training-set": ["training_sets", "training_set_variant"],
     }
     if variant:
         received = db.get_type_table(local_list_args[resource_type][1])
-        res = sorted([r for r in received], key=lambda x:x["name"])
+        res = sorted([r for r in received], key=lambda x: x["name"])
     else:
-        received =  db.get_type_table(local_list_args[resource_type][0])
-        res = sorted([r for r in received], key=lambda x:x["name"])
+        received = db.get_type_table(local_list_args[resource_type][0])
+        res = sorted([r for r in received], key=lambda x: x["name"])
     return res
 
+
 class ColumnName(Enum):
     NAME = 0
     STATUS = 1
     VARIANT = 2
     DESCRIPTION = 3
 
+
 def list_conditions(x, clm_name, default_variant=None):
     if clm_name == "variant" and default_variant == x[clm_name]:
         return f"{x[clm_name]} (default)"
     if clm_name == "description":
         return x[clm_name][:cutoff_length]
     return x[clm_name]
 
+
 def list_local(resource_type, fields):
     field_to_clm = {
         ColumnName.NAME: "name",
         ColumnName.VARIANT: "variant",
         ColumnName.STATUS: "status",
-        ColumnName.DESCRIPTION: "description"
+        ColumnName.DESCRIPTION: "description",
     }
     clm_names = [field_to_clm[field] for field in fields]
     format_rows(*[field.name for field in fields])
     res = get_sorted_list(resource_type)
     if "variant" in clm_names:
         res_variants = get_sorted_list(resource_type, True)
         for r in res:
             for v in filter(lambda x: x["name"] == r["name"], res_variants):
-                format_list = [list_conditions(v, clm_name, r["default_variant"]) for clm_name in clm_names]
+                format_list = [
+                    list_conditions(v, clm_name, r["default_variant"])
+                    for clm_name in clm_names
+                ]
                 format_rows(*format_list)
     else:
         for r in res:
             format_list = [list_conditions(r, clm_name) for clm_name in clm_names]
             format_rows(*format_list)
     return res
```

### Comparing `featureform-1.7.4/src/featureform/list_test.py` & `featureform-1.8.0/src/featureform/list_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from .register import Client
 from io import StringIO
 from unittest.mock import patch
 import os
 
-rc = Client("localhost:8000", False, False, './tls.crt')
+rc = Client("localhost:8000", False, False, "./tls.crt")
+
 
 def check_print_return(expected_print, expected_return, resource_type):
-  rc_list_functions = {
-    "provider": rc.list_providers,
-    "entity": rc.list_entities,
-    "feature": rc.list_features,
-    "label": rc.list_labels,
-    "user": rc.list_users,
-    "source": rc.list_sources,
-    "training_set": rc.list_training_sets
-  }
-
-  with patch('sys.stdout', new = StringIO()) as fake_out:
-    if resource_type in rc_list_functions:
-      value = rc_list_functions[resource_type]()
-    else:
-        raise ValueError("resource type not in Resource Client list functions")
-    assert (fake_out.getvalue().replace(" ","") == expected_print.replace(" ", ""))
-  assert (str(value).replace(" ", "") ==  expected_return.replace(" ", ""))
+    rc_list_functions = {
+        "provider": rc.list_providers,
+        "entity": rc.list_entities,
+        "feature": rc.list_features,
+        "label": rc.list_labels,
+        "user": rc.list_users,
+        "source": rc.list_sources,
+        "training_set": rc.list_training_sets,
+    }
+
+    with patch("sys.stdout", new=StringIO()) as fake_out:
+        if resource_type in rc_list_functions:
+            value = rc_list_functions[resource_type]()
+        else:
+            raise ValueError("resource type not in Resource Client list functions")
+        assert fake_out.getvalue().replace(" ", "") == expected_print.replace(" ", "")
+    assert str(value).replace(" ", "") == expected_return.replace(" ", "")
+
 
 def test_list_provider():
-  expected_print_provider = """NAME                           STATUS                         DESCRIPTION
+    expected_print_provider = """NAME                           STATUS                         DESCRIPTION
                             postgres-quickstart            NO_STATUS                      A Postgres deployment we created for the Featureform quickst
                             redis-quickstart               NO_STATUS                      A Redis deployment we created for the Featureform quickstart
                             """
-  expected_return_provider = """[name: "postgres-quickstart"
+    expected_return_provider = """[name: "postgres-quickstart"
                                 description: "A Postgres deployment we created for the Featureform quickstart"
                                 type: "POSTGRES_OFFLINE"
                                 software: "postgres"
                                 serialized_config: "{\\"Host\\": \\"quickstart-postgres\\", \\"Port\\": \\"5432\\", \\"Username\\": \\"postgres\\", \\"Password\\": \\"password\\", \\"Database\\": \\"postgres\\"}"
                                 sources {
                                 name: "transactions"
                                 variant: "kaggle"
@@ -56,42 +58,43 @@
                                 software: "redis"
                                 serialized_config: "{\\"Addr\\": \\"quickstart-redis:6379\\", \\"Password\\": \\"\\", \\"DB\\": 0}"
                                 features {
                                 name: "avg_transactions"
                                 variant: "quickstart"
                                 }
                                 ]"""
-  check_print_return(expected_print_provider, expected_return_provider, "provider")
-  
+    check_print_return(expected_print_provider, expected_return_provider, "provider")
+
 
 def test_list_entity():
-  expected_print_entity = """NAME                           STATUS
+    expected_print_entity = """NAME                           STATUS
                             user                           NO_STATUS
                           """
-  expected_return_entity = """[name: "user"
+    expected_return_entity = """[name: "user"
                             features {
                             name: "avg_transactions"
                             variant: "quickstart"
                             }
                             labels {
                             name: "fraudulent"
                             variant: "quickstart"
                             }
                             trainingsets {
                             name: "fraud_training"
                             variant: "quickstart"
                             }
                             ]"""
-  check_print_return(expected_print_entity, expected_return_entity, "entity")
+    check_print_return(expected_print_entity, expected_return_entity, "entity")
+
 
 def test_list_user():
-  expected_print_user = """NAME                           STATUS
+    expected_print_user = """NAME                           STATUS
                         featureformer                  NO_STATUS
                         """
-  expected_return_user = """[name: "featureformer"
+    expected_return_user = """[name: "featureformer"
                             features {
                             name: "avg_transactions"
                             variant: "quickstart"
                             }
                             labels {
                             name: "fraudulent"
                             variant: "quickstart"
@@ -105,52 +108,58 @@
                             variant: "kaggle"
                             }
                             sources {
                             name: "average_user_transaction"
                             variant: "quickstart"
                             }
                             ]"""
-  check_print_return(expected_print_user, expected_return_user, "user")
+    check_print_return(expected_print_user, expected_return_user, "user")
+
 
 def test_list_source():
-  expected_print_source = """NAME                           VARIANT                        STATUS                         DESCRIPTION
+    expected_print_source = """NAME                           VARIANT                        STATUS                         DESCRIPTION
                             average_user_transaction       quickstart (default)           NO_STATUS                      the average transaction amount for a user
                             transactions                   kaggle (default)               NO_STATUS                      Fraud Dataset From Kaggle
                             """
-  expected_return_source = """[name: "average_user_transaction"
+    expected_return_source = """[name: "average_user_transaction"
                             default_variant: "quickstart"
                             variants: "quickstart"
                             , name: "transactions"
                             default_variant: "kaggle"
                             variants: "kaggle"
                             ]"""
-  check_print_return(expected_print_source, expected_return_source, "source")
+    check_print_return(expected_print_source, expected_return_source, "source")
+
 
 def test_list_feature():
-  expected_print_feature = """NAME                           VARIANT                        STATUS
+    expected_print_feature = """NAME                           VARIANT                        STATUS
                             avg_transactions               quickstart (default)           NO_STATUS
                             """
-  expected_return_feature = """[name: "avg_transactions"
+    expected_return_feature = """[name: "avg_transactions"
                                 default_variant: "quickstart"
                                 variants: "quickstart"
                                 ]"""
-  check_print_return(expected_print_feature, expected_return_feature, "feature")
+    check_print_return(expected_print_feature, expected_return_feature, "feature")
+
 
 def test_list_label():
-  expected_print_label = """NAME                           VARIANT                        STATUS
+    expected_print_label = """NAME                           VARIANT                        STATUS
                             fraudulent                     quickstart (default)           NO_STATUS
                             """
-  expected_return_label = """[name: "fraudulent"
+    expected_return_label = """[name: "fraudulent"
                             default_variant: "quickstart"
                             variants: "quickstart"
                             ]"""
-  check_print_return(expected_print_label, expected_return_label, "label")
+    check_print_return(expected_print_label, expected_return_label, "label")
+
 
 def test_list_training_set():
-  expected_print_training_set = """NAME                           VARIANT                        STATUS                         DESCRIPTION
+    expected_print_training_set = """NAME                           VARIANT                        STATUS                         DESCRIPTION
                                 fraud_training                 quickstart (default)           NO_STATUS
                                 """
-  expected_return_training_set = """[name: "fraud_training"
+    expected_return_training_set = """[name: "fraud_training"
                                     default_variant: "quickstart"
                                     variants: "quickstart"
                                     ]"""
-  check_print_return(expected_print_training_set, expected_return_training_set, "training_set")
+    check_print_return(
+        expected_print_training_set, expected_return_training_set, "training_set"
+    )
```

### Comparing `featureform-1.7.4/src/featureform/local_cache.py` & `featureform-1.8.0/src/featureform/local_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,17 @@
         if source_files_from_db:
             self._invalidate_cache_if_source_files_changed(
                 source_files_from_db, file_path
             )
 
         source_files = set()
         if source_files_from_db:
-            source_files.update(set(map(lambda x: x["file_path"], source_files_from_db)))
+            source_files.update(
+                set(map(lambda x: x["file_path"], source_files_from_db))
+            )
         else:
             ts_variant = self.db.get_training_set_variant(
                 training_set_name, training_set_variant
             )
             label_variant = self.db.get_label_variant(
                 ts_variant["label_name"], ts_variant["label_variant"]
             )
```

### Comparing `featureform-1.7.4/src/featureform/local_dash_test.py` & `featureform-1.8.0/src/featureform/local_dash_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     {
         "all-variants": ["average_user_transaction"],
         "type": "Source",
         "default-variant": "quickstart",
         "name": "average_user_transaction",
         "variants": {
             "quickstart": {
-                "description": "the average transaction amount for a user ",
+                "description": "the average transaction amount for a user",
                 "name": "average_user_transaction",
                 "source-type": "Source",
                 "owner": "default_user",
                 "provider": "local-mode",
                 "variant": "quickstart",
                 "status": "ready",
                 "labels": {},
@@ -735,15 +735,15 @@
                             }
                         ]
                     },
                 }
             ],
             "average_user_transaction": [
                 {
-                    "description": "the average transaction amount for a user ",
+                    "description": "the average transaction amount for a user",
                     "name": "average_user_transaction",
                     "source-type": "Source",
                     "owner": "default_user",
                     "provider": "local-mode",
                     "variant": "quickstart",
                     "status": "ready",
                     "labels": {},
@@ -946,15 +946,15 @@
                     },
                     "tags": [],
                     "properties": {},
                 }
             ],
             "average_user_transaction": [
                 {
-                    "description": "the average transaction amount for a user ",
+                    "description": "the average transaction amount for a user",
                     "name": "average_user_transaction",
                     "source-type": "Source",
                     "owner": "default_user",
                     "provider": "local-mode",
                     "variant": "quickstart",
                     "status": "ready",
                     "labels": {},
@@ -1304,15 +1304,15 @@
                 },
                 "tags": [],
                 "properties": {},
             }
         ],
         "average_user_transaction": [
             {
-                "description": "the average transaction amount for a user ",
+                "description": "the average transaction amount for a user",
                 "name": "average_user_transaction",
                 "source-type": "Source",
                 "owner": "default_user",
                 "provider": "local-mode",
                 "variant": "quickstart",
                 "status": "ready",
                 "labels": {},
@@ -1512,15 +1512,15 @@
                 },
                 "tags": [],
                 "properties": {},
             }
         ],
         "average_user_transaction": [
             {
-                "description": "the average transaction amount for a user ",
+                "description": "the average transaction amount for a user",
                 "name": "average_user_transaction",
                 "source-type": "Source",
                 "owner": "default_user",
                 "provider": "local-mode",
                 "variant": "quickstart",
                 "status": "ready",
                 "labels": {},
@@ -1624,15 +1624,15 @@
 average_user_transaction = {
     "all-variants": ["average_user_transaction"],
     "type": "Source",
     "default-variant": "quickstart",
     "name": "average_user_transaction",
     "variants": {
         "quickstart": {
-            "description": "the average transaction amount for a user ",
+            "description": "the average transaction amount for a user",
             "name": "average_user_transaction",
             "source-type": "Source",
             "owner": "default_user",
             "provider": "local-mode",
             "variant": "quickstart",
             "status": "ready",
             "labels": {},
```

### Comparing `featureform-1.7.4/src/featureform/local_utils.py` & `featureform-1.8.0/src/featureform/local_utils.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/proto/metadata.proto` & `featureform-1.8.0/src/featureform/proto/metadata.proto`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/proto/metadata_pb2.py` & `featureform-1.8.0/src/featureform/proto/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/proto/metadata_pb2_grpc.py` & `featureform-1.8.0/src/featureform/proto/metadata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/src/featureform/proto/serving.proto` & `featureform-1.8.0/src/featureform/proto/serving.proto`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 option go_package = "github.com/featureform/proto";
 
 package featureform.serving.proto;
 
 service Feature {
   rpc TrainingData(TrainingDataRequest) returns (stream TrainingDataRow) {}
   rpc FeatureServe(FeatureServeRequest) returns (FeatureRow) {}
+  rpc SourceData(SourceDataRequest) returns (stream SourceDataRow) {}
+  rpc SourceColumns(SourceColumnRequest) returns (SourceDataColumns) {}
 }
 
 message Model {
   string name = 1;
 }
 
 message TrainingDataRequest {
@@ -60,7 +62,29 @@
         double double_value = 4;
         int64  int64_value = 5;
         int32  int32_value = 6;
         bool   bool_value = 7;
         bytes on_demand_function = 8;
     }
 }
+
+message SourceID {
+  string name = 1;
+  string version = 2;
+}
+
+message SourceDataRequest {
+  SourceID id = 1;
+  int64 limit = 2;
+}
+
+message SourceColumnRequest {
+  SourceID id = 1;
+}
+
+message SourceDataRow {
+  repeated Value rows = 1;
+}
+
+message SourceDataColumns {
+  repeated string columns = 1;
+}
```

### Comparing `featureform-1.7.4/src/featureform/proto/serving_pb2.py` & `featureform-1.8.0/src/featureform/proto/serving_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\">\n\nFeatureRow\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcb\x01\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12on_demand_function\x18\x08 \x01(\x0cH\x00\x42\x07\n\x05value2\xe2\x01\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x66\x65\x61tureform/proto/serving.proto\x12\x19\x66\x65\x61tureform.serving.proto\"\x15\n\x05Model\x12\x0c\n\x04name\x18\x01 \x01(\t\"}\n\x13TrainingDataRequest\x12\x35\n\x02id\x18\x01 \x01(\x0b\x32).featureform.serving.proto.TrainingDataID\x12/\n\x05model\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Model\"/\n\x0eTrainingDataID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"v\n\x0fTrainingDataRow\x12\x32\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\x12/\n\x05label\x18\x02 \x01(\x0b\x32 .featureform.serving.proto.Value\"\xb3\x01\n\x13\x46\x65\x61tureServeRequest\x12\x36\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32$.featureform.serving.proto.FeatureID\x12\x33\n\x08\x65ntities\x18\x02 \x03(\x0b\x32!.featureform.serving.proto.Entity\x12/\n\x05model\x18\x03 \x01(\x0b\x32 .featureform.serving.proto.Model\">\n\nFeatureRow\x12\x30\n\x06values\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"*\n\tFeatureID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n\x06\x45ntity\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xcb\x01\n\x05Value\x12\x13\n\tstr_value\x18\x01 \x01(\tH\x00\x12\x13\n\tint_value\x18\x02 \x01(\x05H\x00\x12\x15\n\x0b\x66loat_value\x18\x03 \x01(\x02H\x00\x12\x16\n\x0c\x64ouble_value\x18\x04 \x01(\x01H\x00\x12\x15\n\x0bint64_value\x18\x05 \x01(\x03H\x00\x12\x15\n\x0bint32_value\x18\x06 \x01(\x05H\x00\x12\x14\n\nbool_value\x18\x07 \x01(\x08H\x00\x12\x1c\n\x12on_demand_function\x18\x08 \x01(\x0cH\x00\x42\x07\n\x05value\")\n\x08SourceID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"S\n\x11SourceDataRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32#.featureform.serving.proto.SourceID\x12\r\n\x05limit\x18\x02 \x01(\x03\"F\n\x13SourceColumnRequest\x12/\n\x02id\x18\x01 \x01(\x0b\x32#.featureform.serving.proto.SourceID\"?\n\rSourceDataRow\x12.\n\x04rows\x18\x01 \x03(\x0b\x32 .featureform.serving.proto.Value\"$\n\x11SourceDataColumns\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t2\xbd\x03\n\x07\x46\x65\x61ture\x12n\n\x0cTrainingData\x12..featureform.serving.proto.TrainingDataRequest\x1a*.featureform.serving.proto.TrainingDataRow\"\x00\x30\x01\x12g\n\x0c\x46\x65\x61tureServe\x12..featureform.serving.proto.FeatureServeRequest\x1a%.featureform.serving.proto.FeatureRow\"\x00\x12h\n\nSourceData\x12,.featureform.serving.proto.SourceDataRequest\x1a(.featureform.serving.proto.SourceDataRow\"\x00\x30\x01\x12o\n\rSourceColumns\x12..featureform.serving.proto.SourceColumnRequest\x1a,.featureform.serving.proto.SourceDataColumns\"\x00\x42\x1eZ\x1cgithub.com/featureform/protob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'featureform.proto.serving_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\034github.com/featureform/proto'
@@ -35,10 +35,20 @@
   _FEATUREROW._serialized_end=625
   _FEATUREID._serialized_start=627
   _FEATUREID._serialized_end=669
   _ENTITY._serialized_start=671
   _ENTITY._serialized_end=708
   _VALUE._serialized_start=711
   _VALUE._serialized_end=914
-  _FEATURE._serialized_start=917
-  _FEATURE._serialized_end=1143
+  _SOURCEID._serialized_start=916
+  _SOURCEID._serialized_end=957
+  _SOURCEDATAREQUEST._serialized_start=959
+  _SOURCEDATAREQUEST._serialized_end=1042
+  _SOURCECOLUMNREQUEST._serialized_start=1044
+  _SOURCECOLUMNREQUEST._serialized_end=1114
+  _SOURCEDATAROW._serialized_start=1116
+  _SOURCEDATAROW._serialized_end=1179
+  _SOURCEDATACOLUMNS._serialized_start=1181
+  _SOURCEDATACOLUMNS._serialized_end=1217
+  _FEATURE._serialized_start=1220
+  _FEATURE._serialized_end=1665
 # @@protoc_insertion_point(module_scope)
```

### Comparing `featureform-1.7.4/src/featureform/proto/serving_pb2_grpc.py` & `featureform-1.8.0/src/featureform/proto/serving_pb2_grpc.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,14 +20,24 @@
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRow.FromString,
                 )
         self.FeatureServe = channel.unary_unary(
                 '/featureform.serving.proto.Feature/FeatureServe',
                 request_serializer=featureform_dot_proto_dot_serving__pb2.FeatureServeRequest.SerializeToString,
                 response_deserializer=featureform_dot_proto_dot_serving__pb2.FeatureRow.FromString,
                 )
+        self.SourceData = channel.unary_stream(
+                '/featureform.serving.proto.Feature/SourceData',
+                request_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataRequest.SerializeToString,
+                response_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataRow.FromString,
+                )
+        self.SourceColumns = channel.unary_unary(
+                '/featureform.serving.proto.Feature/SourceColumns',
+                request_serializer=featureform_dot_proto_dot_serving__pb2.SourceColumnRequest.SerializeToString,
+                response_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataColumns.FromString,
+                )
 
 
 class FeatureServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def TrainingData(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -37,27 +47,49 @@
 
     def FeatureServe(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SourceData(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SourceColumns(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_FeatureServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'TrainingData': grpc.unary_stream_rpc_method_handler(
                     servicer.TrainingData,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.TrainingDataRow.SerializeToString,
             ),
             'FeatureServe': grpc.unary_unary_rpc_method_handler(
                     servicer.FeatureServe,
                     request_deserializer=featureform_dot_proto_dot_serving__pb2.FeatureServeRequest.FromString,
                     response_serializer=featureform_dot_proto_dot_serving__pb2.FeatureRow.SerializeToString,
             ),
+            'SourceData': grpc.unary_stream_rpc_method_handler(
+                    servicer.SourceData,
+                    request_deserializer=featureform_dot_proto_dot_serving__pb2.SourceDataRequest.FromString,
+                    response_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataRow.SerializeToString,
+            ),
+            'SourceColumns': grpc.unary_unary_rpc_method_handler(
+                    servicer.SourceColumns,
+                    request_deserializer=featureform_dot_proto_dot_serving__pb2.SourceColumnRequest.FromString,
+                    response_serializer=featureform_dot_proto_dot_serving__pb2.SourceDataColumns.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'featureform.serving.proto.Feature', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -93,7 +125,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/featureform.serving.proto.Feature/FeatureServe',
             featureform_dot_proto_dot_serving__pb2.FeatureServeRequest.SerializeToString,
             featureform_dot_proto_dot_serving__pb2.FeatureRow.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SourceData(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/featureform.serving.proto.Feature/SourceData',
+            featureform_dot_proto_dot_serving__pb2.SourceDataRequest.SerializeToString,
+            featureform_dot_proto_dot_serving__pb2.SourceDataRow.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SourceColumns(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/featureform.serving.proto.Feature/SourceColumns',
+            featureform_dot_proto_dot_serving__pb2.SourceColumnRequest.SerializeToString,
+            featureform_dot_proto_dot_serving__pb2.SourceDataColumns.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `featureform-1.7.4/src/featureform/register.py` & `featureform-1.8.0/src/featureform/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,173 +13,229 @@
 
 from .get import *
 from .list import *
 from .get_local import *
 from .list_local import *
 from .sqlite_metadata import SQLiteMetadata
 from .tls import insecure_channel, secure_channel
-from .resources import ColumnTypes, Model, ResourceState, Provider, RedisConfig, FirestoreConfig, CassandraConfig, DynamodbConfig, \
-    MongoDBConfig, PostgresConfig, SnowflakeConfig, LocalConfig, RedshiftConfig, BigQueryConfig, SparkConfig, \
-    AzureFileStoreConfig, OnlineBlobConfig, K8sConfig, S3StoreConfig, GCSFileStoreConfig, User, Location, Source, PrimaryData, SQLTable, \
-    SQLTransformation, DFTransformation, Entity, Feature, Label, ResourceColumnMapping, TrainingSet, ProviderReference, \
-    EntityReference, SourceReference, ExecutorCredentials, ResourceRedefinedError, ResourceStatus, Transformation, \
-    K8sArgs, AWSCredentials, GCPCredentials, HDFSConfig, K8sResourceSpecs, FilePrefix, OnDemandFeature
+from .resources import (
+    ColumnTypes,
+    Model,
+    ResourceState,
+    Provider,
+    RedisConfig,
+    FirestoreConfig,
+    CassandraConfig,
+    DynamodbConfig,
+    MongoDBConfig,
+    PostgresConfig,
+    SnowflakeConfig,
+    LocalConfig,
+    RedshiftConfig,
+    BigQueryConfig,
+    SparkConfig,
+    AzureFileStoreConfig,
+    OnlineBlobConfig,
+    K8sConfig,
+    S3StoreConfig,
+    GCSFileStoreConfig,
+    User,
+    Location,
+    Source,
+    PrimaryData,
+    SQLTable,
+    SQLTransformation,
+    DFTransformation,
+    Entity,
+    Feature,
+    Label,
+    ResourceColumnMapping,
+    TrainingSet,
+    ProviderReference,
+    EntityReference,
+    SourceReference,
+    ExecutorCredentials,
+    ResourceRedefinedError,
+    ResourceStatus,
+    Transformation,
+    K8sArgs,
+    AWSCredentials,
+    GCPCredentials,
+    HDFSConfig,
+    K8sResourceSpecs,
+    FilePrefix,
+    OnDemandFeature,
+)
 
 from .proto import metadata_pb2_grpc as ff_grpc
 from .search_local import search_local
 from .search import search
 from .enums import FileFormat
 
 NameVariant = Tuple[str, str]
 
 s3_config = S3StoreConfig("", "", AWSCredentials("id", "secret"))
 NON_INFERENCE_STORES = [s3_config.type()]
 
 
 class EntityRegistrar:
-
     def __init__(self, registrar, entity):
         self.__registrar = registrar
         self.__entity = entity
 
     def name(self) -> str:
         return self.__entity.name
 
 
 class UserRegistrar:
-
     def __init__(self, registrar, user):
         self.__registrar = registrar
         self.__user = user
 
     def name(self) -> str:
         return self.__user.name
 
     def make_default_owner(self):
         self.__registrar.set_default_owner(self.name())
 
 
 class OfflineProvider:
-
     def __init__(self, registrar, provider):
         self.__registrar = registrar
         self.__provider = provider
 
     def name(self) -> str:
         return self.__provider.name
 
 
 class OfflineSQLProvider(OfflineProvider):
-
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
-    def register_table(self,
-                       name: str,
-                       table: str,
-                       variant: str = "default",
-                       owner: Union[str, UserRegistrar] = "",
-                       description: str = "",
-                       tags: List[str] = [],
-                       properties: dict = {}):
+    def register_table(
+        self,
+        name: str,
+        table: str,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a SQL table as a primary data source.
 
         Args:
             name (str): Name of table to be registered
             variant (str): Name of variant to be registered
             table (str): Name of SQL table
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of table to be registered
 
         Returns:
             source (ColumnSourceRegistrar): source
         """
-        return self.__registrar.register_primary_data(name=name,
-                                                      variant=variant,
-                                                      location=SQLTable(table),
-                                                      owner=owner,
-                                                      provider=self.name(),
-                                                      description=description,
-                                                      tags=tags,
-                                                      properties=properties)
-
-    def sql_transformation(self,
-                           owner: Union[str, UserRegistrar] = "",
-                           variant: str = "default",
-                           name: str = "",
-                           schedule: str = "",
-                           description: str = "",
-                           tags: List[str] = [],
-                           properties: dict = {}):
-        return self.__registrar.sql_transformation(name=name,
-                                                   variant=variant,
-                                                   owner=owner,
-                                                   schedule=schedule,
-                                                   provider=self.name(),
-                                                   description=description,
-                                                   tags=tags,
-                                                   properties=properties)
+        return self.__registrar.register_primary_data(
+            name=name,
+            variant=variant,
+            location=SQLTable(table),
+            owner=owner,
+            provider=self.name(),
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
+
+    def sql_transformation(
+        self,
+        owner: Union[str, UserRegistrar] = "",
+        variant: str = "default",
+        name: str = "",
+        schedule: str = "",
+        description: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
+        return self.__registrar.sql_transformation(
+            name=name,
+            variant=variant,
+            owner=owner,
+            schedule=schedule,
+            provider=self.name(),
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
 
 
 class OfflineSparkProvider(OfflineProvider):
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
-    def register_file(self,
-                        name: str,
-                        file_path: str,
-                        variant: str = "default",
-                        owner: Union[str, UserRegistrar] = "",
-                        description: str = "",
-                        tags: List[str] = [],
-                        properties: dict = {}):
+    def register_file(
+        self,
+        name: str,
+        file_path: str,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Spark data source as a primary data source.
 
         Args:
             name (str): Name of table to be registered
             variant (str): Name of variant to be registered
             file_path (str): The path to file
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of table to be registered
 
         Returns:
             source (ColumnSourceRegistrar): source
         """
-        return self.__registrar.register_primary_data(name=name,
-                                                      variant=variant,
-                                                      location=SQLTable(file_path),
-                                                      owner=owner,
-                                                      provider=self.name(),
-                                                      description=description,
-                                                      tags=tags,
-                                                      properties=properties)
-    
-    def register_parquet_file(self,
-                              name: str,
-                              file_path: str,
-                              variant: str = "default",
-                              owner: Union[str, UserRegistrar] = "",
-                              description: str = "", ):
-        if self.__provider.config.executor_type != "EMR" and file_path.startswith(FilePrefix.S3.value):
+        return self.__registrar.register_primary_data(
+            name=name,
+            variant=variant,
+            location=SQLTable(file_path),
+            owner=owner,
+            provider=self.name(),
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
+
+    def register_parquet_file(
+        self,
+        name: str,
+        file_path: str,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+    ):
+        if self.__provider.config.executor_type != "EMR" and file_path.startswith(
+            FilePrefix.S3.value
+        ):
             file_path = file_path.replace(FilePrefix.S3.value, FilePrefix.S3A.value)
 
         return self.register_file(name, file_path, variant, owner, description)
 
-    def sql_transformation(self,
-                           variant: str = "default",
-                           owner: Union[str, UserRegistrar] = "",
-                           name: str = "",
-                           schedule: str = "",
-                           description: str = "",
-                           tags: List[str] = [],
-                           properties: dict = {}):
+    def sql_transformation(
+        self,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        name: str = "",
+        schedule: str = "",
+        description: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """
         Register a SQL transformation source. The spark.sql_transformation decorator takes the returned string in the
         following function and executes it as a SQL Query.
 
         The name of the function is the name of the resulting source.
 
         Sources for the transformation can be specified by adding the Name and Variant in brackets '{{ name.variant }}'.
@@ -199,31 +255,35 @@
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of primary data to be registered
 
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.sql_transformation(name=name,
-                                                   variant=variant,
-                                                   owner=owner,
-                                                   schedule=schedule,
-                                                   provider=self.name(),
-                                                   description=description,
-                                                   tags=tags,
-                                                   properties=properties)
-
-    def df_transformation(self,
-                          variant: str = "default",
-                          owner: Union[str, UserRegistrar] = "",
-                          name: str = "",
-                          description: str = "",
-                          inputs: list = [],
-                          tags: List[str] = [],
-                          properties: dict = {}):
+        return self.__registrar.sql_transformation(
+            name=name,
+            variant=variant,
+            owner=owner,
+            schedule=schedule,
+            provider=self.name(),
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
+
+    def df_transformation(
+        self,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        name: str = "",
+        description: str = "",
+        inputs: list = [],
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """
         Register a Dataframe transformation source. The spark.df_transformation decorator takes the contents
         of the following function and executes the code it contains at serving time.
 
         The name of the function is used as the name of the source when being registered.
 
         The specified inputs are loaded into dataframes that can be accessed using the function parameters.
@@ -241,69 +301,77 @@
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of primary data to be registered
             inputs (list[Tuple(str, str)]): A list of Source NameVariant Tuples to input into the transformation
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.df_transformation(name=name,
-                                                  variant=variant,
-                                                  owner=owner,
-                                                  provider=self.name(),
-                                                  description=description,
-                                                  inputs=inputs,
-                                                  tags=tags,
-                                                  properties=properties)
+        return self.__registrar.df_transformation(
+            name=name,
+            variant=variant,
+            owner=owner,
+            provider=self.name(),
+            description=description,
+            inputs=inputs,
+            tags=tags,
+            properties=properties,
+        )
 
 
 class OfflineK8sProvider(OfflineProvider):
     def __init__(self, registrar, provider):
         super().__init__(registrar, provider)
         self.__registrar = registrar
         self.__provider = provider
 
-    def register_file(self,
-                      name: str,
-                      path: str,
-                      variant: str = "default",
-                      owner: Union[str, UserRegistrar] = "",
-                      description: str = "",
-                      tags: List[str] = [],
-                      properties: dict = {}):
+    def register_file(
+        self,
+        name: str,
+        path: str,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a blob data source path as a primary data source.
 
         Args:
             name (str): Name of table to be registered
             variant (str): Name of variant to be registered
             path (str): The path to blob store file
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of table to be registered
 
         Returns:
             source (ColumnSourceRegistrar): source
         """
-        return self.__registrar.register_primary_data(name=name,
-                                                      variant=variant,
-                                                      location=SQLTable(path),
-                                                      owner=owner,
-                                                      provider=self.name(),
-                                                      description=description,
-                                                      tags=tags,
-                                                      properties=properties)
-
-    def sql_transformation(self,
-                           variant: str = "default",
-                           owner: Union[str, UserRegistrar] = "",
-                           name: str = "",
-                           schedule: str = "",
-                           description: str = "",
-                           docker_image: str = "",
-                           resource_specs: Union[K8sResourceSpecs, None] = None,
-                           tags: List[str] = [],
-                           properties: dict = {}):
+        return self.__registrar.register_primary_data(
+            name=name,
+            variant=variant,
+            location=SQLTable(path),
+            owner=owner,
+            provider=self.name(),
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
+
+    def sql_transformation(
+        self,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        name: str = "",
+        schedule: str = "",
+        description: str = "",
+        docker_image: str = "",
+        resource_specs: Union[K8sResourceSpecs, None] = None,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """
         Register a SQL transformation source. The k8s.sql_transformation decorator takes the returned string in the
         following function and executes it as a SQL Query.
 
         The name of the function is the name of the resulting source.
 
         Sources for the transformation can be specified by adding the Name and Variant in brackets '{{ name.variant }}'.
@@ -325,34 +393,38 @@
             docker_image (str): A custom Docker image to run the transformation
             resource_specs (K8sResourceSpecs): Custom resource requests and limits
 
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.sql_transformation(name=name,
-                                                   variant=variant,
-                                                   owner=owner,
-                                                   schedule=schedule,
-                                                   provider=self.name(),
-                                                   description=description,
-                                                   args=K8sArgs(docker_image=docker_image, specs=resource_specs),
-                                                   tags=tags,
-                                                   properties=properties)
-
-    def df_transformation(self,
-                          variant: str = "default",
-                          owner: Union[str, UserRegistrar] = "",
-                          name: str = "",
-                          description: str = "",
-                          inputs: list = [],
-                          docker_image: str = "",
-                          resource_specs: Union[K8sResourceSpecs, None] = None,
-                          tags: List[str] = [],
-                          properties: dict = {}):
+        return self.__registrar.sql_transformation(
+            name=name,
+            variant=variant,
+            owner=owner,
+            schedule=schedule,
+            provider=self.name(),
+            description=description,
+            args=K8sArgs(docker_image=docker_image, specs=resource_specs),
+            tags=tags,
+            properties=properties,
+        )
+
+    def df_transformation(
+        self,
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        name: str = "",
+        description: str = "",
+        inputs: list = [],
+        docker_image: str = "",
+        resource_specs: Union[K8sResourceSpecs, None] = None,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """
         Register a Dataframe transformation source. The k8s_azure.df_transformation decorator takes the contents
         of the following function and executes the code it contains at serving time.
 
         The name of the function is used as the name of the source when being registered.
 
         The specified inputs are loaded into dataframes that can be accessed using the function parameters.
@@ -372,23 +444,25 @@
             inputs (list[Tuple(str, str)]): A list of Source NameVariant Tuples to input into the transformation
             docker_image (str): A custom Docker image to run the transformation
             resource_specs (K8sResourceSpecs): Custom resource requests and limits
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
-        return self.__registrar.df_transformation(name=name,
-                                                  variant=variant,
-                                                  owner=owner,
-                                                  provider=self.name(),
-                                                  description=description,
-                                                  inputs=inputs,
-                                                  args=K8sArgs(docker_image=docker_image, specs=resource_specs),
-                                                  tags=tags,
-                                                  properties=properties)
+        return self.__registrar.df_transformation(
+            name=name,
+            variant=variant,
+            owner=owner,
+            provider=self.name(),
+            description=description,
+            inputs=inputs,
+            args=K8sArgs(docker_image=docker_image, specs=resource_specs),
+            tags=tags,
+            properties=properties,
+        )
 
 
 class OnlineProvider:
     def __init__(self, registrar, provider):
         self.__registrar = registrar
         self.__provider = provider
 
@@ -599,15 +673,14 @@
             description=description,
             tags=tags,
             properties=properties,
         )
 
 
 class SourceRegistrar:
-
     def __init__(self, registrar, source):
         self.__registrar = registrar
         self.__source = source
 
     def id(self) -> NameVariant:
         return self.__source.name, self.__source.variant
 
@@ -628,22 +701,24 @@
 
 
 class LocalSource:
     """
     LocalSource creates a reference to a source that can be accessed locally.
     """
 
-    def __init__(self,
-                 registrar,
-                 name: str,
-                 owner: str,
-                 variant: str,
-                 provider: str,
-                 path: str,
-                 description: str = ""):
+    def __init__(
+        self,
+        registrar,
+        name: str,
+        owner: str,
+        variant: str,
+        provider: str,
+        path: str,
+        description: str = "",
+    ):
         self.registrar = registrar
         self.name = name
         self.variant = variant
         self.owner = owner
         self.provider = provider
         self.path = path
         self.description = description
@@ -656,17 +731,21 @@
         self.__set_query(fn())
         fn.register_resources = self.register_resources
         return fn
 
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
-            raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
+            raise Exception(
+                f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns"
+            )
         elif col_len > 3:
-            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
+            raise Exception(
+                f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column"
+            )
         return (self.registrar, self.name_variant(), columns)
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def pandas(self):
         """
@@ -674,22 +753,22 @@
 
         Returns:
         dataframe (pandas.Dataframe): A pandas Dataframe
         """
         return pd.read_csv(self.path)
 
     def register_resources(
-            self,
-            entity: Union[str, EntityRegistrar],
-            entity_column: str,
-            owner: Union[str, UserRegistrar] = "",
-            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-            features: List[ColumnMapping] = None,
-            labels: List[ColumnMapping] = None,
-            timestamp_column: str = "",
+        self,
+        entity: Union[str, EntityRegistrar],
+        entity_column: str,
+        owner: Union[str, UserRegistrar] = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        features: List[ColumnMapping] = None,
+        labels: List[ColumnMapping] = None,
+        timestamp_column: str = "",
     ):
         """
         Registers a features and/or labels that can be used in training sets or served.
 
         **Examples**:
         ``` py
         average_user_transaction.register_resources(
@@ -741,15 +820,22 @@
     feature = ff.Feature(average_user_transaction[["user_id", "avg_transaction_amt"]])
     ```
 
     Given the function type does not implement __getitem__ we need to wrap it in a class that 
     enables this behavior while still maintaining the original function signature and behavior.
     """
 
-    def __init__(self, fn, registrar, provider, decorator_register_resources_method, decorator_name_variant_method):
+    def __init__(
+        self,
+        fn,
+        registrar,
+        provider,
+        decorator_register_resources_method,
+        decorator_name_variant_method,
+    ):
         self.fn = fn
         self.registrar = registrar
         self.provider = provider
         # Previously, the descriptor protocol was used to apply methods from the decorator classes
         # to instances of SubscriptableTransformation such that a user could call `fn.name_variant()`
         # and receive a tuple of (name, variant) where name was the name of the wrapped function and
         # variant was either the value passed to the decorator or the default value. This was achieved
@@ -759,36 +845,41 @@
         # the decorator methods to the SubscriptableTransformation class.
         self.register_resources = decorator_register_resources_method
         self.name_variant = decorator_name_variant_method
 
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
-            raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
+            raise Exception(
+                f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns"
+            )
         elif col_len > 3:
-            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
+            raise Exception(
+                f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column"
+            )
         return (self.registrar, self.name_variant(), columns)
 
     def __call__(self, *args, **kwds):
         return self.fn(*args, **kwds)
 
 
 class SQLTransformationDecorator:
-
-    def __init__(self,
-                 registrar,
-                 owner: str,
-                 provider: str,
-                 tags: List[str],
-                 properties: dict,
-                 variant: str = "default",
-                 name: str = "",
-                 schedule: str = "",
-                 description: str = "",
-                 args: K8sArgs = None):
+    def __init__(
+        self,
+        registrar,
+        owner: str,
+        provider: str,
+        tags: List[str],
+        properties: dict,
+        variant: str = "default",
+        name: str = "",
+        schedule: str = "",
+        description: str = "",
+        args: K8sArgs = None,
+    ):
         self.registrar = registrar
         self.name = name
         self.variant = variant
         self.owner = owner
         self.schedule = schedule
         self.provider = provider
         self.description = description
@@ -803,15 +894,15 @@
             self.name = fn.__name__
         self.__set_query(fn())
         return SubscriptableTransformation(
             fn,
             self.registrar,
             self.provider,
             self.register_resources,
-            self.name_variant
+            self.name_variant,
         )
 
     @typechecked
     def __set_query(self, query: str):
         if query == "":
             raise ValueError("Query cannot be an empty string")
         self.query = query
@@ -822,31 +913,31 @@
             variant=self.variant,
             definition=SQLTransformation(self.query, self.args),
             owner=self.owner,
             schedule=self.schedule,
             provider=self.provider,
             description=self.description,
             tags=self.tags,
-            properties=self.properties
+            properties=self.properties,
         )
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def register_resources(
-            self,
-            entity: Union[str, EntityRegistrar],
-            entity_column: str,
-            owner: Union[str, UserRegistrar] = "",
-            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-            features: List[ColumnMapping] = None,
-            labels: List[ColumnMapping] = None,
-            timestamp_column: str = "",
-            description: str = "",
-            schedule: str = "",
+        self,
+        entity: Union[str, EntityRegistrar],
+        entity_column: str,
+        owner: Union[str, UserRegistrar] = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        features: List[ColumnMapping] = None,
+        labels: List[ColumnMapping] = None,
+        timestamp_column: str = "",
+        description: str = "",
+        schedule: str = "",
     ):
         return self.registrar.register_column_resources(
             source=(self.name, self.variant),
             entity=entity,
             entity_column=entity_column,
             owner=owner,
             inference_store=inference_store,
@@ -855,26 +946,27 @@
             timestamp_column=timestamp_column,
             description=description,
             schedule=schedule,
         )
 
 
 class DFTransformationDecorator:
-
-    def __init__(self,
-                 registrar,
-                 owner: str,
-                 provider: str,
-                 tags: List[str],
-                 properties: dict,
-                 variant: str = "default",
-                 name: str = "",
-                 description: str = "",
-                 inputs: list = [],
-                 args: K8sArgs = None):
+    def __init__(
+        self,
+        registrar,
+        owner: str,
+        provider: str,
+        tags: List[str],
+        properties: dict,
+        variant: str = "default",
+        name: str = "",
+        description: str = "",
+        inputs: list = [],
+        args: K8sArgs = None,
+    ):
         self.registrar = registrar
         self.name = name
         self.variant = variant
         self.owner = owner
         self.provider = provider
         self.description = description
         self.inputs = inputs
@@ -886,49 +978,51 @@
         if self.description == "" and fn.__doc__ is not None:
             self.description = fn.__doc__
         if self.name == "":
             self.name = fn.__name__
 
         for nv in self.inputs:
             if self.name is nv[0] and self.variant is nv[1]:
-                raise ValueError(f"Transformation cannot be input for itself: {self.name} {self.variant}")
+                raise ValueError(
+                    f"Transformation cannot be input for itself: {self.name} {self.variant}"
+                )
         self.query = dill.dumps(fn.__code__)
         return SubscriptableTransformation(
             fn,
             self.registrar,
             self.provider,
             self.register_resources,
-            self.name_variant
+            self.name_variant,
         )
 
     def to_source(self) -> Source:
         return Source(
             name=self.name,
             variant=self.variant,
             definition=DFTransformation(self.query, self.inputs, self.args),
             owner=self.owner,
             provider=self.provider,
             description=self.description,
             tags=self.tags,
-            properties=self.properties
+            properties=self.properties,
         )
 
     def name_variant(self):
         return (self.name, self.variant)
 
     def register_resources(
-            self,
-            entity: Union[str, EntityRegistrar],
-            entity_column: str,
-            owner: Union[str, UserRegistrar] = "",
-            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-            features: List[ColumnMapping] = None,
-            labels: List[ColumnMapping] = None,
-            timestamp_column: str = "",
-            description: str = ""
+        self,
+        entity: Union[str, EntityRegistrar],
+        entity_column: str,
+        owner: Union[str, UserRegistrar] = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        features: List[ColumnMapping] = None,
+        labels: List[ColumnMapping] = None,
+        timestamp_column: str = "",
+        description: str = "",
     ):
         return self.registrar.register_column_resources(
             source=(self.name, self.variant),
             entity=entity,
             entity_column=entity_column,
             owner=owner,
             inference_store=inference_store,
@@ -936,34 +1030,37 @@
             labels=labels,
             timestamp_column=timestamp_column,
             description=description,
         )
 
 
 class ColumnSourceRegistrar(SourceRegistrar):
-
     def __getitem__(self, columns: List[str]):
         col_len = len(columns)
         if col_len < 2:
-            raise Exception(f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns")
+            raise Exception(
+                f"Expected 2 columns, but found {col_len}. Missing entity and/or source columns"
+            )
         elif col_len > 3:
-            raise Exception(f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column")
+            raise Exception(
+                f"Found unrecognized columns {', '.join(columns[3:])}. Expected 2 required columns and an optional 3rd timestamp column"
+            )
         return (self.registrar(), self.id(), columns)
 
     def register_resources(
-            self,
-            entity: Union[str, EntityRegistrar],
-            entity_column: str,
-            owner: Union[str, UserRegistrar] = "",
-            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-            features: List[ColumnMapping] = None,
-            labels: List[ColumnMapping] = None,
-            timestamp_column: str = "",
-            description: str = "",
-            schedule: str = "",
+        self,
+        entity: Union[str, EntityRegistrar],
+        entity_column: str,
+        owner: Union[str, UserRegistrar] = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        features: List[ColumnMapping] = None,
+        labels: List[ColumnMapping] = None,
+        timestamp_column: str = "",
+        description: str = "",
+        schedule: str = "",
     ):
         """
         Registers a features and/or labels that can be used in training sets or served.
 
         **Examples**:
         ``` py
         average_user_transaction.register_resources(
@@ -999,51 +1096,53 @@
             timestamp_column=timestamp_column,
             description=description,
             schedule=schedule,
         )
 
 
 class ResourceRegistrar:
-
     def __init__(self, registrar, features, labels):
         self.__registrar = registrar
         self.__features = features
         self.__labels = labels
 
-    def create_training_set(self,
-                            name: str,
-                            variant: str = "default",
-                            label: NameVariant = None,
-                            schedule: str = "",
-                            features: List[NameVariant] = None,
-                            resources: List = None,
-                            owner: Union[str, UserRegistrar] = "",
-                            description: str = ""):
+    def create_training_set(
+        self,
+        name: str,
+        variant: str = "default",
+        label: NameVariant = None,
+        schedule: str = "",
+        features: List[NameVariant] = None,
+        resources: List = None,
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+    ):
         if len(self.__labels) == 0:
             raise ValueError("A label must be included in a training set")
         if len(self.__features) == 0:
             raise ValueError("A feature must be included in a training set")
         if len(self.__labels) > 1 and label == None:
-            raise ValueError(
-                "Only one label may be specified in a TrainingSet.")
+            raise ValueError("Only one label may be specified in a TrainingSet.")
         if features is not None:
-            featureSet = set([(feature["name"], feature["variant"])
-                              for feature in self.__features])
+            featureSet = set(
+                [(feature["name"], feature["variant"]) for feature in self.__features]
+            )
             for feature in features:
                 if feature not in featureSet:
                     raise ValueError(f"Feature {feature} not found.")
         else:
-            features = [(feature["name"], feature["variant"])
-                        for feature in self.__features]
+            features = [
+                (feature["name"], feature["variant"]) for feature in self.__features
+            ]
         if label is None:
             label = (self.__labels[0]["name"], self.__labels[0]["variant"])
         else:
-            labelSet = set([
-                (label["name"], label["variant"]) for label in self.__labels
-            ])
+            labelSet = set(
+                [(label["name"], label["variant"]) for label in self.__labels]
+            )
             if label not in labelSet:
                 raise ValueError(f"Label {label} not found.")
         return self.__registrar.register_training_set(
             name=name,
             variant=variant,
             label=label,
             features=features,
@@ -1055,24 +1154,25 @@
 
     def features(self):
         return self.__features
 
     def label(self):
         if isinstance(self.__labels, list):
             if len(self.__labels) > 1:
-                raise ValueError("A resource used has multiple labels. A training set can only have one label")
+                raise ValueError(
+                    "A resource used has multiple labels. A training set can only have one label"
+                )
             elif len(self.__labels) == 1:
                 self.__labels = (self.__labels[0]["name"], self.__labels[0]["variant"])
             else:
                 self.__labels = ()
         return self.__labels
 
 
 class ModelRegistrar:
-
     def __init__(self, registrar, model):
         self.__registrar = registrar
         self.__model = model
 
     def name(self) -> str:
         return self.__model.name
 
@@ -1100,15 +1200,17 @@
 
     def add_resource(self, resource):
         self.__resources.append(resource)
 
     def get_resources(self):
         return self.__resources
 
-    def register_user(self, name: str, tags: List[str] = [], properties: dict = {}) -> UserRegistrar:
+    def register_user(
+        self, name: str, tags: List[str] = [], properties: dict = {}
+    ) -> UserRegistrar:
         """Register a user.
 
         Args:
             name (str): User to be registered.
 
         Returns:
             UserRegistrar: User
@@ -1127,16 +1229,15 @@
 
     def default_owner(self) -> str:
         return self.__default_owner
 
     def must_get_default_owner(self) -> str:
         owner = self.default_owner()
         if owner == "":
-            raise ValueError(
-                "Owner must be set or a default owner must be specified.")
+            raise ValueError("Owner must be set or a default owner must be specified.")
         return owner
 
     def get_source(self, name, variant, local=False):
         """Get a source. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1156,36 +1257,46 @@
 
         Returns:
             source (ColumnSourceRegistrar): Source
         """
         get = SourceReference(name=name, variant=variant, obj=None)
         self.__resources.append(get)
         if local:
-            return LocalSource(self,
-                               name=name,
-                               owner="",
-                               variant=variant,
-                               provider="",
-                               description="",
-                               path="")
+            return LocalSource(
+                self,
+                name=name,
+                owner="",
+                variant=variant,
+                provider="",
+                description="",
+                path="",
+            )
         else:
             fakeDefinition = PrimaryData(location=SQLTable(name=""))
-            fakeSource = Source(name=name,
-                                variant=variant,
-                                definition=fakeDefinition,
-                                owner="",
-                                provider="",
-                                description="")
+            fakeSource = Source(
+                name=name,
+                variant=variant,
+                definition=fakeDefinition,
+                owner="",
+                provider="",
+                description="",
+            )
             return ColumnSourceRegistrar(self, fakeSource)
 
     def get_local_provider(self, name="local-mode"):
         get = ProviderReference(name=name, provider_type="local", obj=None)
         self.__resources.append(get)
         fakeConfig = LocalConfig()
-        fakeProvider = Provider(name=name, function="LOCAL_ONLINE", description="", team="", config=fakeConfig)
+        fakeProvider = Provider(
+            name=name,
+            function="LOCAL_ONLINE",
+            description="",
+            team="",
+            config=fakeConfig,
+        )
         return LocalProvider(self, fakeProvider)
 
     def get_redis(self, name):
         """Get a Redis provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1205,15 +1316,17 @@
 
         Returns:
             redis (OnlineProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="redis", obj=None)
         self.__resources.append(get)
         fakeConfig = RedisConfig(host="", port=123, password="", db=123)
-        fakeProvider = Provider(name=name, function="ONLINE", description="", team="", config=fakeConfig)
+        fakeProvider = Provider(
+            name=name, function="ONLINE", description="", team="", config=fakeConfig
+        )
         return OnlineProvider(self, fakeProvider)
 
     def get_mongodb(self, name):
         """Get a MongoDB provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1233,15 +1346,17 @@
 
         Returns:
             mongodb (OnlineProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="mongodb", obj=None)
         self.__resources.append(get)
         mock_config = MongoDBConfig()
-        mock_provider = Provider(name=name, function="ONLINE", description="", team="", config=mock_config)
+        mock_provider = Provider(
+            name=name, function="ONLINE", description="", team="", config=mock_config
+        )
         return OnlineProvider(self, mock_provider)
 
     def get_blob_store(self, name):
         """Get a Azure Blob provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1260,17 +1375,23 @@
             name (str): Name of Azure blob provider to be retrieved
 
         Returns:
             azure_blob (FileStoreProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="AZURE", obj=None)
         self.__resources.append(get)
-        fake_azure_config = AzureFileStoreConfig(account_name="", account_key="", container_name="", root_path="")
-        fake_config = OnlineBlobConfig(store_type="AZURE", store_config=fake_azure_config.config())
-        fakeProvider = Provider(name=name, function="ONLINE", description="", team="", config=fake_config)
+        fake_azure_config = AzureFileStoreConfig(
+            account_name="", account_key="", container_name="", root_path=""
+        )
+        fake_config = OnlineBlobConfig(
+            store_type="AZURE", store_config=fake_azure_config.config()
+        )
+        fakeProvider = Provider(
+            name=name, function="ONLINE", description="", team="", config=fake_config
+        )
         return FileStoreProvider(self, fakeProvider, fake_config, "AZURE")
 
     def get_postgres(self, name):
         """Get a Postgres provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1287,15 +1408,17 @@
 
         Returns:
             postgres (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="postgres", obj=None)
         self.__resources.append(get)
         fakeConfig = PostgresConfig(host="", port="", database="", user="", password="")
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_snowflake(self, name):
         """Get a Snowflake provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1311,18 +1434,27 @@
             name (str): Name of Snowflake provider to be retrieved
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="snowflake", obj=None)
         self.__resources.append(get)
-        fakeConfig = SnowflakeConfig(account="ff_fake", database="ff_fake", organization="ff_fake", username="ff_fake", password="ff_fake", schema="ff_fake")
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeConfig = SnowflakeConfig(
+            account="ff_fake",
+            database="ff_fake",
+            organization="ff_fake",
+            username="ff_fake",
+            password="ff_fake",
+            schema="ff_fake",
+        )
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineSQLProvider(self, fakeProvider)
-    
+
     def get_snowflake_legacy(self, name: str):
         """Get a Snowflake provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
         snowflake = ff.get_snowflake_legacy("snowflake-quickstart")
         transactions = snowflake.register_table(
@@ -1337,16 +1469,26 @@
 
         Returns:
             snowflake_legacy (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="snowflake", obj=None)
         self.__resources.append(get)
 
-        fakeConfig = SnowflakeConfig(account_locator="ff_fake", database="ff_fake", username="ff_fake", password="ff_fake", schema="ff_fake", warehouse="ff_fake", role="ff_fake")
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeConfig = SnowflakeConfig(
+            account_locator="ff_fake",
+            database="ff_fake",
+            username="ff_fake",
+            password="ff_fake",
+            schema="ff_fake",
+            warehouse="ff_fake",
+            role="ff_fake",
+        )
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_redshift(self, name):
         """Get a Redshift provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1363,15 +1505,17 @@
 
         Returns:
             redshift (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="redshift", obj=None)
         self.__resources.append(get)
         fakeConfig = RedshiftConfig(host="", port="", database="", user="", password="")
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_bigquery(self, name):
         """Get a BigQuery provider. The returned object can be used to register additional resources.
 
         **Examples**:
         ``` py
@@ -1388,15 +1532,17 @@
 
         Returns:
             bigquery (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="bigquery", obj=None)
         self.__resources.append(get)
         fakeConfig = BigQueryConfig(project_id="", dataset_id="", credentials_path="")
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineSQLProvider(self, fakeProvider)
 
     def get_spark(self, name):
         """Get a Spark provider. The returned object can be used to register additional resources.
         **Examples**:
         ``` py
         spark = ff.get_spark("spark-quickstart")
@@ -1410,16 +1556,20 @@
         Args:
             name (str): Name of Spark provider to be retrieved
         Returns:
             spark (OfflineSQLProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="spark", obj=None)
         self.__resources.append(get)
-        fakeConfig = SparkConfig(executor_type="", executor_config={}, store_type="", store_config={})
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeConfig = SparkConfig(
+            executor_type="", executor_config={}, store_type="", store_config={}
+        )
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineSparkProvider(self, fakeProvider)
 
     def get_kubernetes(self, name):
         """
         Get a k8s Azure provider. The returned object can be used to register additional resources.
         **Examples**:
         ``` py
@@ -1437,15 +1587,17 @@
         Returns:
             k8s_azure (OfflineK8sProvider): Provider
         """
         get = ProviderReference(name=name, provider_type="k8s-azure", obj=None)
         self.__resources.append(get)
 
         fakeConfig = K8sConfig(store_type="", store_config={})
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineK8sProvider(self, fakeProvider)
 
     def get_s3(self, name):
         """
         Get a S3 provider. The returned object can be used with other providers such as Spark and Databricks.
         **Examples**:
         ``` py
@@ -1464,35 +1616,43 @@
         Returns:
             s3 (FileStore): Provider
         """
         get = ProviderReference(name=name, provider_type="S3", obj=None)
         self.__resources.append(get)
 
         fake_creds = AWSCredentials("id", "secret")
-        fakeConfig = S3StoreConfig(bucket_path="", bucket_region="", credentials=fake_creds)
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=s3_config)
+        fakeConfig = S3StoreConfig(
+            bucket_path="", bucket_region="", credentials=fake_creds
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=s3_config,
+        )
         return FileStoreProvider(provider, s3_config, s3_config.type())
-    
+
     def get_gcs(self, name):
         get = ProviderReference(name=name, provider_type="GCS", obj=None)
         self.__resources.append(get)
 
         filename = "fake_secrets.json"
         if not exists(filename):
             self._create_mock_creds_file(filename, {"test": "creds"})
 
         fake_creds = GCPCredentials("id", filename)
-        fakeConfig = GCSStoreConfig(bucket_name="", bucket_path="", credentials=fake_creds)
-        fakeProvider = Provider(name=name, function="OFFLINE", description="", team="", config=fakeConfig)
+        fakeConfig = GCSStoreConfig(
+            bucket_name="", bucket_path="", credentials=fake_creds
+        )
+        fakeProvider = Provider(
+            name=name, function="OFFLINE", description="", team="", config=fakeConfig
+        )
         return OfflineK8sProvider(self, fakeProvider)
-    
+
     def _create_mock_creds_file(self, filename, json_data):
         with open(filename, "w") as f:
             json.dumps(json_data, f)
 
     def get_entity(self, name, local=False):
         """Get an entity. The returned object can be used to register additional resources.
 
@@ -1515,24 +1675,26 @@
             entity (EntityRegistrar): Entity
         """
         get = EntityReference(name=name, obj=None)
         self.__resources.append(get)
         fakeEntity = Entity(name=name, description="")
         return EntityRegistrar(self, fakeEntity)
 
-    def register_redis(self,
-                       name: str,
-                       description: str = "",
-                       team: str = "",
-                       host: str = "0.0.0.0",
-                       port: int = 6379,
-                       password: str = "",
-                       db: int = 0,
-                       tags: List[str] = [],
-                       properties: dict = {}):
+    def register_redis(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        host: str = "0.0.0.0",
+        port: int = 6379,
+        password: str = "",
+        db: int = 0,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Redis provider.
 
         **Examples**:
         ```
         redis = ff.register_redis(
             name="redis-quickstart",
             host="quickstart-redis",  # The internal dns name for redis
@@ -1551,48 +1713,51 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             redis (OnlineProvider): Provider
         """
         config = RedisConfig(host=host, port=port, password=password, db=db)
-        provider = Provider(name=name,
-                            function="ONLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        provider = Provider(
+            name=name,
+            function="ONLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_blob_store(self,
-                            name: str,
-                            account_name: str,
-                            account_key: str,
-                            container_name: str,
-                            root_path: str,
-                            description: str = "",
-                            team: str = "",
-                            tags: List[str] = [],
-                            properties: dict = {}):
-
+    def register_blob_store(
+        self,
+        name: str,
+        account_name: str,
+        account_key: str,
+        container_name: str,
+        root_path: str,
+        description: str = "",
+        team: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register an azure blob store provider.
 
         This has the functionality of an online store and can be used as a parameter
         to a k8s or spark provider
 
         **Examples**:
         ```
         blob = ff.register_blob_store(
             name="azure-quickstart",
             container_name="my_company_container"
             root_path="custom/path/in/container"
             account_name=<azure_account_name>
-            account_key=<azure_account_key> 
+            account_key=<azure_account_key>
             description="An azure blob store provider to store offline and inference data"
         )
         ```
         Args:
             name (str): Name of Azure blob store to be registered
             container_name (str): Azure container name
             root_path (str): custom path in container to store data
@@ -1604,38 +1769,48 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             blob (StorageProvider): Provider
                 has all the functionality of OnlineProvider
         """
 
-        azure_config = AzureFileStoreConfig(account_name=account_name, account_key=account_key,
-                                            container_name=container_name, root_path=root_path)
-        config = OnlineBlobConfig(store_type="AZURE", store_config=azure_config.config())
-
-        provider = Provider(name=name,
-                            function="ONLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        azure_config = AzureFileStoreConfig(
+            account_name=account_name,
+            account_key=account_key,
+            container_name=container_name,
+            root_path=root_path,
+        )
+        config = OnlineBlobConfig(
+            store_type="AZURE", store_config=azure_config.config()
+        )
+
+        provider = Provider(
+            name=name,
+            function="ONLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, azure_config, "AZURE")
 
-    def register_s3(self,
-                    name: str,
-                    credentials: AWSCredentials,
-                    bucket_path: str,
-                    bucket_region: str,
-                    path: str = "",
-                    description: str = "",
-                    team: str = "",
-                    tags: List[str] = [],
-                    properties: dict = {}):
+    def register_s3(
+        self,
+        name: str,
+        credentials: AWSCredentials,
+        bucket_path: str,
+        bucket_region: str,
+        path: str = "",
+        description: str = "",
+        team: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a S3 store provider.
 
         This has the functionality of an offline store and can be used as a parameter
         to a k8s or spark provider
 
         **Examples**:
         ```
@@ -1659,36 +1834,44 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             s3 (FileStoreProvider): Provider
                 has all the functionality of OfflineProvider
         """
 
-        s3_config = S3StoreConfig(bucket_path=bucket_path, bucket_region=bucket_region, credentials=credentials, path=path)
+        s3_config = S3StoreConfig(
+            bucket_path=bucket_path,
+            bucket_region=bucket_region,
+            credentials=credentials,
+            path=path,
+        )
 
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=s3_config,
-                            tags=tags,
-                            properties=properties)
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=s3_config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, s3_config, s3_config.type())
 
-
-    def register_gcs(self,
-                    name: str,
-                    credentials: GCPCredentials,
-                    bucket_name: str,
-                    bucket_path: str = "",
-                    description: str = "",
-                    team: str = "",
-                    tags: List[str] = [],
-                    properties: dict = {}):
+    def register_gcs(
+        self,
+        name: str,
+        credentials: GCPCredentials,
+        bucket_name: str,
+        bucket_path: str = "",
+        description: str = "",
+        team: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a GCS store provider.
                 **Examples**:
         ```
         gcs = ff.register_gcs(
             name="gcs-quickstart",
             credentials=gcp_creds,
             bucket_name="bucket_name",
@@ -1706,33 +1889,41 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             gcs (FileStoreProvider): Provider
                 has all the functionality of OfflineProvider
         """
 
-        gcs_config = GCSFileStoreConfig(bucket_name=bucket_name, bucket_path=bucket_path, credentials=credentials)
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=gcs_config,
-                            tags=tags,
-                            properties=properties)
+        gcs_config = GCSFileStoreConfig(
+            bucket_name=bucket_name, bucket_path=bucket_path, credentials=credentials
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=gcs_config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, gcs_config, gcs_config.type())
 
-    def register_hdfs(self,
-                      name: str,
-                      host: str,
-                      port: str,
-                      username: str = "",
-                      path: str = "",
-                      description: str = "",
-                      team: str = "", ):
+    def register_hdfs(
+        self,
+        name: str,
+        host: str,
+        port: str,
+        username: str = "",
+        path: str = "",
+        description: str = "",
+        team: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a HDFS store provider.
 
         This has the functionality of an offline store and can be used as a parameter
         to a k8s or spark provider
 
         **Examples**:
         ```
@@ -1744,42 +1935,48 @@
             username=<username>
             description="An hdfs store provider to store offline"
         )
         ```
         Args:
             name (str): Name of HDFS store to be registered
             host (str): The hostname for HDFS
-            port (str): The port for the namenode for HDFS
+            port (str): The IPC port for the Namenode for HDFS. (Typically 8020 or 9000)
             path (str): A storage path within HDFS
             username (str): A Username for HDFS
             description (str): Description of HDFS provider to be registered
             team (str): The name of the team registering HDFS
         Returns:
             hdfs (FileStoreProvider): Provider
         """
 
         hdfs_config = HDFSConfig(host=host, port=port, path=path, username=username)
 
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=hdfs_config)
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=hdfs_config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return FileStoreProvider(self, provider, hdfs_config, hdfs_config.type())
 
-    def register_firestore(self,
-                           name: str,
-                           collection: str,
-                           project_id: str,
-                           credentials_path: str,
-                           description: str = "",
-                           team: str = "",
-                           tags: List[str] = [],
-                           properties: dict = {}):
+    def register_firestore(
+        self,
+        name: str,
+        collection: str,
+        project_id: str,
+        credentials_path: str,
+        description: str = "",
+        team: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Firestore provider.
 
         **Examples**:
         ```
         firestore = ff.register_firestore(
             name="firestore-quickstart",
             description="A Firestore deployment we created for the Featureform quickstart",
@@ -1795,38 +1992,46 @@
             collection (str): The Collection name in Firestore under the given project ID
             credentials_path (str): A path to a Google Credentials file with access permissions for Firestore
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
         Returns:
             firestore (OfflineSQLProvider): Provider
         """
-        config = FirestoreConfig(collection=collection, project_id=project_id, credentials_path=credentials_path)
-        provider = Provider(name=name,
-                            function="ONLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = FirestoreConfig(
+            collection=collection,
+            project_id=project_id,
+            credentials_path=credentials_path,
+        )
+        provider = Provider(
+            name=name,
+            function="ONLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_cassandra(self,
-                           name: str,
-                           description: str = "",
-                           team: str = "",
-                           host: str = "0.0.0.0",
-                           port: int = 9042,
-                           username: str = "cassandra",
-                           password: str = "cassandra",
-                           keyspace: str = "",
-                           consistency: str = "THREE",
-                           replication: int = 3,
-                           tags: List[str] = [],
-                           properties: dict = {}):
+    def register_cassandra(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        host: str = "0.0.0.0",
+        port: int = 9042,
+        username: str = "cassandra",
+        password: str = "cassandra",
+        keyspace: str = "",
+        consistency: str = "THREE",
+        replication: int = 3,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Cassandra provider.
 
         **Examples**:
         ```
         cassandra = ff.register_cassandra(
                 name = "cassandra",
                 description = "Example inference store",
@@ -1851,35 +2056,46 @@
             replication (int): Replication
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             cassandra (OnlineProvider): Provider
         """
-        config = CassandraConfig(host=host, port=port, username=username, password=password, keyspace=keyspace,
-                                 consistency=consistency, replication=replication)
-        provider = Provider(name=name,
-                            function="ONLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = CassandraConfig(
+            host=host,
+            port=port,
+            username=username,
+            password=password,
+            keyspace=keyspace,
+            consistency=consistency,
+            replication=replication,
+        )
+        provider = Provider(
+            name=name,
+            function="ONLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_dynamodb(self,
-                          name: str,
-                          description: str = "",
-                          team: str = "",
-                          access_key: str = None,
-                          secret_key: str = None,
-                          region: str = None,
-                          tags: List[str] = [],
-                          properties: dict = {}):
+    def register_dynamodb(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        access_key: str = None,
+        secret_key: str = None,
+        region: str = None,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a DynamoDB provider.
 
         **Examples**:
         ```
         dynamodb = ff.register_dynamodb(
             name="dynamodb-quickstart",
             description="A Dynamodb deployment we created for the Featureform quickstart",
@@ -1897,38 +2113,43 @@
             region (str): Region
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             dynamodb (OnlineProvider): Provider
         """
-        config = DynamodbConfig(access_key=access_key, secret_key=secret_key, region=region)
-        provider = Provider(name=name,
-                            function="ONLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = DynamodbConfig(
+            access_key=access_key, secret_key=secret_key, region=region
+        )
+        provider = Provider(
+            name=name,
+            function="ONLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
-    def register_mongodb(self,
-                         name: str,
-                         description: str = "",
-                         team: str = "",
-                         username: str = None,
-                         password: str = None,
-                         database: str = None,
-                         host: str = None,
-                         port: str = None,
-                         throughput: int = 1000,
-                         tags: List[str] = [],
-                         properties: dict = {}
-                         ):
+    def register_mongodb(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        username: str = None,
+        password: str = None,
+        database: str = None,
+        host: str = None,
+        port: str = None,
+        throughput: int = 1000,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a MongoDB provider.
 
         **Examples**:
         ```
         mongodb = ff.register_mongodb(
             name="mongodb-quickstart",
             description="A MongoDB deployment",
@@ -1953,40 +2174,49 @@
             throughput (int): The maximum RU limit for autoscaling
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             mongodb (OnlineProvider): Provider
         """
-        config = MongoDBConfig(username=username, password=password, host=host, port=port, database=database,
-                               throughput=throughput)
-        provider = Provider(name=name,
-                            function="ONLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = MongoDBConfig(
+            username=username,
+            password=password,
+            host=host,
+            port=port,
+            database=database,
+            throughput=throughput,
+        )
+        provider = Provider(
+            name=name,
+            function="ONLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OnlineProvider(self, provider)
 
     def register_snowflake_legacy(
-                self,
-                name: str,
-                username: str,
-                password: str,
-                account_locator: str,
-                database: str,
-                schema: str = "PUBLIC",
-                description: str = "",
-                team: str = "",
-                warehouse: str = "",
-                role: str = "",
-                tags: List[str] = [],
-                properties: dict = {}):
+        self,
+        name: str,
+        username: str,
+        password: str,
+        account_locator: str,
+        database: str,
+        schema: str = "PUBLIC",
+        description: str = "",
+        team: str = "",
+        warehouse: str = "",
+        role: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Snowflake provider using legacy credentials.
 
         **Examples**:
         ```
         snowflake = ff.register_snowflake_legacy(
             name="snowflake-quickstart",
             username="snowflake",
@@ -2010,46 +2240,51 @@
             role (str): Specifies the role to use by default for accessing Snowflake objects in the client session
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
-        config = SnowflakeConfig(account_locator=account_locator,
-                                 database=database,
-                                 username=username,
-                                 password=password,
-                                 schema=schema,
-                                 warehouse=warehouse,
-                                 role=role)
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = SnowflakeConfig(
+            account_locator=account_locator,
+            database=database,
+            username=username,
+            password=password,
+            schema=schema,
+            warehouse=warehouse,
+            role=role,
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
     def register_snowflake(
-            self,
-            name: str,
-            username: str,
-            password: str,
-            account: str,
-            organization: str,
-            database: str,
-            schema: str = "PUBLIC",
-            description: str = "",
-            team: str = "",
-            warehouse: str = "",
-            role: str = "",
-            tags: List[str] = [],
-            properties: dict = {}):
+        self,
+        name: str,
+        username: str,
+        password: str,
+        account: str,
+        organization: str,
+        database: str,
+        schema: str = "PUBLIC",
+        description: str = "",
+        team: str = "",
+        warehouse: str = "",
+        role: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Snowflake provider.
 
         **Examples**:
         ```
         snowflake = ff.register_snowflake(
             name="snowflake-quickstart",
             username="snowflake",
@@ -2075,43 +2310,49 @@
             role (str): Specifies the role to use by default for accessing Snowflake objects in the client session
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             snowflake (OfflineSQLProvider): Provider
         """
-        config = SnowflakeConfig(account=account,
-                                 database=database,
-                                 organization=organization,
-                                 username=username,
-                                 password=password,
-                                 schema=schema,
-                                 warehouse=warehouse,
-                                 role=role)
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = SnowflakeConfig(
+            account=account,
+            database=database,
+            organization=organization,
+            username=username,
+            password=password,
+            schema=schema,
+            warehouse=warehouse,
+            role=role,
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_postgres(self,
-                          name: str,
-                          description: str = "",
-                          team: str = "",
-                          host: str = "0.0.0.0",
-                          port: str = "5432",
-                          user: str = "postgres",
-                          password: str = "password",
-                          database: str = "postgres",
-                          tags: List[str] = None,
-                          properties: dict = None):
+    def register_postgres(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        host: str = "0.0.0.0",
+        port: str = "5432",
+        user: str = "postgres",
+        password: str = "password",
+        database: str = "postgres",
+        tags: List[str] = None,
+        properties: dict = None,
+    ):
         """Register a Postgres provider.
 
         **Examples**:
         ```
         postgres = ff.register_postgres(
             name="postgres-quickstart",
             description="A Postgres deployment we created for the Featureform quickstart",
@@ -2133,40 +2374,43 @@
             database (str): Database
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             postgres (OfflineSQLProvider): Provider
         """
-        config = PostgresConfig(host=host,
-                                port=port,
-                                database=database,
-                                user=user,
-                                password=password)
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags or [],
-                            properties=properties or {})
+        config = PostgresConfig(
+            host=host, port=port, database=database, user=user, password=password
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags or [],
+            properties=properties or {},
+        )
+
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_redshift(self,
-                          name: str,
-                          description: str = "",
-                          team: str = "",
-                          host: str = "",
-                          port: int = 5432,
-                          user: str = "redshift",
-                          password: str = "password",
-                          database: str = "dev",
-                          tags: List[str] = [],
-                          properties: dict = {}):
+    def register_redshift(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        host: str = "",
+        port: int = 5432,
+        user: str = "redshift",
+        password: str = "password",
+        database: str = "dev",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Redshift provider.
 
         **Examples**:
         ```
         redshift = ff.register_redshift(
             name="redshift-quickstart",
             description="A Redshift deployment we created for the Featureform quickstart",
@@ -2188,38 +2432,40 @@
             database (str): Database
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             redshift (OfflineSQLProvider): Provider
         """
-        config = RedshiftConfig(host=host,
-                                port=port,
-                                database=database,
-                                user=user,
-                                password=password)
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = RedshiftConfig(
+            host=host, port=port, database=database, user=user, password=password
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_bigquery(self,
-                          name: str,
-                          description: str = "",
-                          team: str = "",
-                          project_id: str = "",
-                          dataset_id: str = "",
-                          credentials_path: str = "",
-                          tags: List[str] = [],
-                          properties: dict = {}):
+    def register_bigquery(
+        self,
+        name: str,
+        description: str = "",
+        team: str = "",
+        project_id: str = "",
+        dataset_id: str = "",
+        credentials_path: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a BigQuery provider.
 
         **Examples**:
         ```
         bigquery = ff.register_bigquery(
             name="bigquery-quickstart",
             description="A BigQuery deployment we created for the Featureform quickstart",
@@ -2236,35 +2482,41 @@
             credentials_path (str): A path to a Google Credentials file with access permissions for BigQuery
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             bigquery (OfflineSQLProvider): Provider
         """
-        config = BigQueryConfig(project_id=project_id,
-                                dataset_id=dataset_id,
-                                credentials_path=credentials_path, )
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        config = BigQueryConfig(
+            project_id=project_id,
+            dataset_id=dataset_id,
+            credentials_path=credentials_path,
+        )
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OfflineSQLProvider(self, provider)
 
-    def register_spark(self,
-                       name: str,
-                       executor: ExecutorCredentials,
-                       filestore: FileStoreProvider,
-                       description: str = "",
-                       team: str = "",
-                       tags: List[str] = [],
-                       properties: dict = {}):
+    def register_spark(
+        self,
+        name: str,
+        executor: ExecutorCredentials,
+        filestore: FileStoreProvider,
+        description: str = "",
+        team: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Spark on Executor provider.
         **Examples**:
         ```
         spark = ff.register_spark(
             name="spark-quickstart",
             description="A Spark deployment we created for the Featureform quickstart",
             team="featureform-team",
@@ -2285,37 +2537,42 @@
             spark (OfflineSparkProvider): Provider
         """
 
         config = SparkConfig(
             executor_type=executor.type(),
             executor_config=executor.config(),
             store_type=filestore.store_type(),
-            store_config=filestore.config())
+            store_config=filestore.config(),
+        )
 
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OfflineSparkProvider(self, provider)
 
-    def register_k8s(self,
-                     name: str,
-                     store: FileStoreProvider,
-                     description: str = "",
-                     team: str = "",
-                     docker_image: str = "",
-                     tags: List[str] = [],
-                     properties: dict = {}):
+    def register_k8s(
+        self,
+        name: str,
+        store: FileStoreProvider,
+        description: str = "",
+        team: str = "",
+        docker_image: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """
         Register an offline store provider to run on featureform's own k8s deployment
-        
+
         Args:
             name (str): Name of provider
             store (FileStoreProvider): Reference to registered file store provider
             description (str): Description of primary data to be registered
             team (str): A string parameter describing the team that owns the provider
             docker_image (str): A custom docker image using the base image featureformcom/k8s_runner
             tags (List[str]): Optional grouping mechanism for resources
@@ -2330,59 +2587,65 @@
             docker_image="my-repo/image:version"
         )
         ```
         """
         config = K8sConfig(
             store_type=store.store_type(),
             store_config=store.config(),
-            docker_image=docker_image
+            docker_image=docker_image,
         )
 
-        provider = Provider(name=name,
-                            function="OFFLINE",
-                            description=description,
-                            team=team,
-                            config=config,
-                            tags=tags,
-                            properties=properties)
+        provider = Provider(
+            name=name,
+            function="OFFLINE",
+            description=description,
+            team=team,
+            config=config,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(provider)
         return OfflineK8sProvider(self, provider)
 
     def register_local(self):
         """Register a Local provider.
 
         **Examples**:
         ```
             local = register_local()
         ```
         Returns:
             local (LocalProvider): Provider
         """
         config = LocalConfig()
-        provider = Provider(name="local-mode",
-                            function="LOCAL_ONLINE",
-                            description="This is local mode",
-                            team="team",
-                            config=config,
-                            tags=['local-mode'],
-                            properties={"resource_type": "Provider"})
+        provider = Provider(
+            name="local-mode",
+            function="LOCAL_ONLINE",
+            description="This is local mode",
+            team="team",
+            config=config,
+            tags=["local-mode"],
+            properties={"resource_type": "Provider"},
+        )
         self.__resources.append(provider)
         local_provider = LocalProvider(self, provider)
         local_provider.insert_provider()
         return local_provider
 
-    def register_primary_data(self,
-                              name: str,
-                              variant: str,
-                              location: Location,
-                              provider: Union[str, OfflineProvider],
-                              tags: List[str],
-                              properties: dict,
-                              owner: Union[str, UserRegistrar] = "",
-                              description: str = ""):
+    def register_primary_data(
+        self,
+        name: str,
+        variant: str,
+        location: Location,
+        provider: Union[str, OfflineProvider],
+        tags: List[str],
+        properties: dict,
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+    ):
         """Register a primary data source.
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             location (Location): Location of primary data
             provider (Union[str, OfflineProvider]): Provider
@@ -2394,36 +2657,40 @@
         """
         if not isinstance(owner, str):
             owner = owner.name()
         if owner == "":
             owner = self.must_get_default_owner()
         if not isinstance(provider, str):
             provider = provider.name()
-        source = Source(name=name,
-                        variant=variant,
-                        definition=PrimaryData(location=location),
-                        owner=owner,
-                        provider=provider,
-                        description=description,
-                        tags=tags,
-                        properties=properties)
+        source = Source(
+            name=name,
+            variant=variant,
+            definition=PrimaryData(location=location),
+            owner=owner,
+            provider=provider,
+            description=description,
+            tags=tags,
+            properties=properties,
+        )
         self.__resources.append(source)
         return ColumnSourceRegistrar(self, source)
 
-    def register_sql_transformation(self,
-                                    name: str,
-                                    query: str,
-                                    provider: Union[str, OfflineProvider],
-                                    variant: str = "default",
-                                    owner: Union[str, UserRegistrar] = "",
-                                    description: str = "",
-                                    schedule: str = "",
-                                    args: K8sArgs = None,
-                                    tags: List[str] = [],
-                                    properties: dict = {}):
+    def register_sql_transformation(
+        self,
+        name: str,
+        query: str,
+        provider: Union[str, OfflineProvider],
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        schedule: str = "",
+        args: K8sArgs = None,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a SQL transformation source.
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             query (str): SQL query
             provider (Union[str, OfflineProvider]): Provider
@@ -2448,29 +2715,31 @@
             variant=variant,
             definition=SQLTransformation(query, args),
             owner=owner,
             schedule=schedule,
             provider=provider,
             description=description,
             tags=tags,
-            properties=properties
+            properties=properties,
         )
         self.__resources.append(source)
         return ColumnSourceRegistrar(self, source)
 
-    def sql_transformation(self,
-                           provider: Union[str, OfflineProvider],
-                           variant: str = "default",
-                           name: str = "",
-                           schedule: str = "",
-                           owner: Union[str, UserRegistrar] = "",
-                           description: str = "",
-                           args: K8sArgs = None,
-                           tags: List[str] = [],
-                           properties: dict = {}):
+    def sql_transformation(
+        self,
+        provider: Union[str, OfflineProvider],
+        variant: str = "default",
+        name: str = "",
+        schedule: str = "",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        args: K8sArgs = None,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """SQL transformation decorator.
 
         Args:
             variant (str): Name of variant
             provider (Union[str, OfflineProvider]): Provider
             name (str): Name of source
             schedule (str): Kubernetes CronJob schedule string ("* * * * *")
@@ -2495,31 +2764,33 @@
             variant=variant,
             provider=provider,
             schedule=schedule,
             owner=owner,
             description=description,
             args=args,
             tags=tags,
-            properties=properties
+            properties=properties,
         )
         self.__resources.append(decorator)
         return decorator
 
-    def register_df_transformation(self,
-                                   name: str,
-                                   query: str,
-                                   provider: Union[str, OfflineProvider],
-                                   variant: str = "default",
-                                   owner: Union[str, UserRegistrar] = "",
-                                   description: str = "",
-                                   inputs: list = [],
-                                   schedule: str = "",
-                                   args: K8sArgs = None,
-                                   tags: List[str] = [],
-                                   properties: dict = {}):
+    def register_df_transformation(
+        self,
+        name: str,
+        query: str,
+        provider: Union[str, OfflineProvider],
+        variant: str = "default",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        inputs: list = [],
+        schedule: str = "",
+        args: K8sArgs = None,
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a Dataframe transformation source.
 
         Args:
             name (str): Name of source
             variant (str): Name of variant
             query (str): SQL query
             provider (Union[str, OfflineProvider]): Provider
@@ -2549,30 +2820,31 @@
             variant=variant,
             definition=DFTransformation(query, inputs, args),
             owner=owner,
             schedule=schedule,
             provider=provider,
             description=description,
             tags=tags,
-            properties=properties
+            properties=properties,
         )
         self.__resources.append(source)
         return ColumnSourceRegistrar(self, source)
 
-    def df_transformation(self,
-                          provider: Union[str, OfflineProvider],
-                          tags: List[str],
-                          properties: dict,
-                          variant: str = "default",
-                          name: str = "",
-                          owner: Union[str, UserRegistrar] = "",
-                          description: str = "",
-                          inputs: list = [],
-                          args: K8sArgs = None
-                          ):
+    def df_transformation(
+        self,
+        provider: Union[str, OfflineProvider],
+        tags: List[str],
+        properties: dict,
+        variant: str = "default",
+        name: str = "",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        inputs: list = [],
+        args: K8sArgs = None,
+    ):
         """Dataframe transformation decorator.
 
         Args:
             variant (str): Name of variant
             provider (Union[str, OfflineProvider]): Provider
             name (str): Name of source
             owner (Union[str, UserRegistrar]): Owner
@@ -2601,28 +2873,30 @@
             variant=variant,
             provider=provider,
             owner=owner,
             description=description,
             inputs=inputs,
             args=args,
             tags=tags,
-            properties=properties
+            properties=properties,
         )
         self.__resources.append(decorator)
         return decorator
 
-    def ondemand_feature(self, 
-                          fn=None, *,
-                          tags: List[str] = None,
-                          properties: dict = None,
-                          variant: str = "default",
-                          name: str = "",
-                          owner: Union[str, UserRegistrar] = "",
-                          description: str = "",
-                          ):
+    def ondemand_feature(
+        self,
+        fn=None,
+        *,
+        tags: List[str] = None,
+        properties: dict = None,
+        variant: str = "default",
+        name: str = "",
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+    ):
         """On Demand Feature decorator.
 
         Args:
             variant (str): Name of variant
             name (str): Name of source
             owner (Union[str, UserRegistrar]): Owner
             description (str): Description of on demand feature
@@ -2640,48 +2914,60 @@
         ```
         """
 
         if not isinstance(owner, str):
             owner = owner.name()
         if owner == "":
             owner = self.must_get_default_owner()
-    
+
         decorator = OnDemandFeature(
             name=name,
             variant=variant,
             owner=owner,
             description=description,
             tags=tags or [],
             properties=properties or {},
         )
         self.__resources.append(decorator)
-        
+
         if fn is None:
             return decorator
         else:
             return decorator(fn)
 
     def state(self):
         for resource in self.__resources:
             try:
-                if isinstance(resource, SQLTransformationDecorator) or isinstance(resource, DFTransformationDecorator):
+                if isinstance(resource, SQLTransformationDecorator) or isinstance(
+                    resource, DFTransformationDecorator
+                ):
                     resource = resource.to_source()
                 self.__state.add(resource)
             except ResourceRedefinedError:
                 raise
             except Exception as e:
-                resource_variant = f" ({resource.variant})" if hasattr(resource, 'variant') else ""
-                raise Exception(f"Could not add apply {resource.name}{resource_variant}: {e}")
+                resource_variant = (
+                    f" ({resource.variant})" if hasattr(resource, "variant") else ""
+                )
+                raise Exception(
+                    f"Could not add apply {resource.name}{resource_variant}: {e}"
+                )
         self.__resources = []
         return self.__state
 
     def clear_state(self):
         self.__state = ResourceState()
 
-    def register_entity(self, name: str, description: str = "", tags: List[str] = [], properties: dict = {}):
+    def register_entity(
+        self,
+        name: str,
+        description: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register an entity.
 
         **Examples**:
         ``` py
             user = ff.register_entity("user")
         ```
         Args:
@@ -2689,30 +2975,33 @@
             description (str): Description of entity to be registered
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             entity (EntityRegistrar): Entity
         """
-        entity = Entity(name=name, description=description, tags=tags, properties=properties)
+        entity = Entity(
+            name=name, description=description, tags=tags, properties=properties
+        )
         self.__resources.append(entity)
         return EntityRegistrar(self, entity)
 
     def register_column_resources(
-            self,
-            source: Union[NameVariant, SourceRegistrar, SQLTransformationDecorator],
-            entity: Union[str, EntityRegistrar],
-            entity_column: str,
-            owner: Union[str, UserRegistrar] = "",
-            inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-            features: List[ColumnMapping] = None,
-            labels: List[ColumnMapping] = None,
-            timestamp_column: str = "",
-            description: str = "",
-            schedule: str = "",):
+        self,
+        source: Union[NameVariant, SourceRegistrar, SQLTransformationDecorator],
+        entity: Union[str, EntityRegistrar],
+        entity_column: str,
+        owner: Union[str, UserRegistrar] = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        features: List[ColumnMapping] = None,
+        labels: List[ColumnMapping] = None,
+        timestamp_column: str = "",
+        description: str = "",
+        schedule: str = "",
+    ):
         """Create features and labels from a source. Used in the register_resources function.
 
         Args:
             source (Union[NameVariant, SourceRegistrar, SQLTransformationDecorator]): Source of features, labels, entity
             entity (Union[str, EntityRegistrar]): Entity
             entity_column (str): Column of entity in source
             owner (Union[str, UserRegistrar]): Owner
@@ -2724,32 +3013,36 @@
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
         Returns:
             resource (ResourceRegistrar): resource
         """
 
-        if type(inference_store) == FileStoreProvider and inference_store.store_type() in NON_INFERENCE_STORES:
-            raise Exception(f"cannot use '{inference_store.store_type()}' as an inference store.")
+        if (
+            type(inference_store) == FileStoreProvider
+            and inference_store.store_type() in NON_INFERENCE_STORES
+        ):
+            raise Exception(
+                f"cannot use '{inference_store.store_type()}' as an inference store."
+            )
 
         if features is None:
             features = []
         if labels is None:
             labels = []
         if len(features) == 0 and len(labels) == 0:
             raise ValueError("No features or labels set")
         if not isinstance(source, tuple):
             source = source.id()
         if not isinstance(entity, str):
             entity = entity.name()
         if not isinstance(inference_store, str):
             inference_store = inference_store.name()
         if len(features) > 0 and inference_store == "":
-            raise ValueError(
-                "Inference store must be set when defining features")
+            raise ValueError("Inference store must be set when defining features")
         if not isinstance(owner, str):
             owner = owner.name()
         if owner == "":
             owner = self.must_get_default_owner()
         feature_resources = []
         label_resources = []
         for feature in features:
@@ -2769,15 +3062,15 @@
                 schedule=schedule,
                 location=ResourceColumnMapping(
                     entity=entity_column,
                     value=feature["column"],
                     timestamp=timestamp_column,
                 ),
                 tags=feature_tags,
-                properties=feature_properties
+                properties=feature_properties,
             )
             self.__resources.append(resource)
             feature_resources.append(resource)
 
         for label in labels:
             variant = label.get("variant", "default")
             desc = label.get("description", "")
@@ -2794,15 +3087,15 @@
                 description=desc,
                 location=ResourceColumnMapping(
                     entity=entity_column,
                     value=label["column"],
                     timestamp=timestamp_column,
                 ),
                 tags=label_tags,
-                properties=label_properties
+                properties=label_properties,
             )
             self.__resources.append(resource)
             label_resources.append(resource)
         return ResourceRegistrar(self, features, labels)
 
     def __get_feature_nv(self, features):
         feature_nv_list = []
@@ -2812,28 +3105,35 @@
                 feature_nv = (feature, "default")
                 feature_nv_list.append(feature_nv)
             elif isinstance(feature, dict):
                 lag = feature.get("lag")
                 if lag:
                     required_lag_keys = set(["lag", "feature", "variant"])
                     received_lag_keys = set(feature.keys())
-                    if required_lag_keys.intersection(received_lag_keys) != required_lag_keys:
+                    if (
+                        required_lag_keys.intersection(received_lag_keys)
+                        != required_lag_keys
+                    ):
                         raise ValueError(
-                            f"feature lags require 'lag', 'feature', 'variant' fields. Received: {feature.keys()}")
+                            f"feature lags require 'lag', 'feature', 'variant' fields. Received: {feature.keys()}"
+                        )
 
                     if not isinstance(lag, timedelta):
                         raise ValueError(
-                            f"the lag, '{lag}', needs to be of type 'datetime.timedelta'. Received: {type(lag)}.")
+                            f"the lag, '{lag}', needs to be of type 'datetime.timedelta'. Received: {type(lag)}."
+                        )
 
                     feature_name_variant = (feature["feature"], feature["variant"])
                     if feature_name_variant not in feature_nv_list:
                         feature_nv_list.append(feature_name_variant)
 
                     lag_name = f"{feature['feature']}_{feature['variant']}_lag_{lag}"
-                    sanitized_lag_name = lag_name.replace(" ", "").replace(",", "_").replace(":", "_")
+                    sanitized_lag_name = (
+                        lag_name.replace(" ", "").replace(",", "_").replace(":", "_")
+                    )
                     feature["name"] = feature.get("name", sanitized_lag_name)
 
                     feature_lags.append(feature)
                 else:
                     feature_nv = (feature["name"], feature["variant"])
                     feature_nv_list.append(feature_nv)
             elif isinstance(feature, list):
@@ -2844,25 +3144,27 @@
                 if len(feature_lags_list) != 0:
                     feature_lags.extend(feature_lags_list)
             else:
                 feature_nv_list.append(feature)
 
         return feature_nv_list, feature_lags
 
-    def register_training_set(self,
-                              name: str,
-                              variant: str = "default",
-                              features: list = [],
-                              label: NameVariant = (),
-                              resources: list = [],
-                              owner: Union[str, UserRegistrar] = "",
-                              description: str = "",
-                              schedule: str = "",
-                              tags: List[str] = [],
-                              properties: dict = {}):
+    def register_training_set(
+        self,
+        name: str,
+        variant: str = "default",
+        features: list = [],
+        label: NameVariant = (),
+        resources: list = [],
+        owner: Union[str, UserRegistrar] = "",
+        description: str = "",
+        schedule: str = "",
+        tags: List[str] = [],
+        properties: dict = {},
+    ):
         """Register a training set.
 
         Args:
             name (str): Name of training set to be registered
             variant (str): Name of variant to be registered
             label (NameVariant): Label of training set
             features (List[NameVariant]): Features of training set
@@ -2917,15 +3219,17 @@
             features=features,
             feature_lags=feature_lags,
             tags=tags,
             properties=properties,
         )
         self.__resources.append(resource)
 
-    def register_model(self, name: str, tags: List[str] = [], properties: dict = {}) -> Model:
+    def register_model(
+        self, name: str, tags: List[str] = [], properties: dict = {}
+    ) -> Model:
         """Register a model.
 
         Args:
             name (str): Model to be registered
             tags (List[str]): Optional grouping mechanism for resources
             properties (dict): Optional grouping mechanism for resources
 
@@ -2948,15 +3252,17 @@
     rc = ResourceClient("localhost:8000")
 
     # example query:
     redis = rc.get_provider("redis-quickstart")
     ```
     """
 
-    def __init__(self, host=None, local=False, insecure=False, cert_path=None, dry_run=False):
+    def __init__(
+        self, host=None, local=False, insecure=False, cert_path=None, dry_run=False
+    ):
         """Initialise a Resource Client object.
 
         Args:
             host (str): The hostname of the Featureform instance. Exclude if using Localmode.
             local (bool): True if using Localmode.
             insecure (bool): True if connecting to an insecure Featureform endpoint. False if using a self-signed or public TLS certificate
             cert_path (str): The path to a public certificate if using a self-signed certificate.
@@ -2975,19 +3281,19 @@
 
         if dry_run:
             return
 
         if local and host:
             raise ValueError("Cannot be local and have a host")
         elif not local:
-            host = host or os.getenv('FEATUREFORM_HOST')
+            host = host or os.getenv("FEATUREFORM_HOST")
             if host is None:
                 raise RuntimeError(
-                    'If not in local mode then `host` must be passed or the environment'
-                    ' variable FEATUREFORM_HOST must be set.'
+                    "If not in local mode then `host` must be passed or the environment"
+                    " variable FEATUREFORM_HOST must be set."
                 )
             if insecure:
                 channel = insecure_channel(host)
             else:
                 channel = secure_channel(host, cert_path)
             self._stub = ff_grpc.ApiStub(channel)
             self._host = host
@@ -3010,15 +3316,14 @@
 
         if not asynchronous and self._stub:
             resources = resource_state.sorted_list()
             display_statuses(self._stub, resources)
 
         clear_state()
 
-
     def get_user(self, name, local=False):
         """Get a user. Prints out name of user, and all resources associated with the user.
 
         **Examples:**
 
         ``` py title="Input"
         featureformer = rc.get_user("featureformer")
@@ -3241,15 +3546,15 @@
             source=(feature.source.name, feature.source.variant),
             value_type=feature.type,
             entity=feature.entity,
             owner=feature.owner,
             provider=feature.provider,
             location=ResourceColumnMapping("", "", ""),
             description=feature.description,
-            status=feature.status.Status._enum_type.values[feature.status.status].name
+            status=feature.status.Status._enum_type.values[feature.status.status].name,
         )
 
     def print_feature(self, name, variant=None, local=False):
         """Get a feature. Prints out information on feature, and all variants associated with the feature. If variant is included, print information on that specific variant and all resources associated with it.
 
         **Examples:**
 
@@ -3364,15 +3669,15 @@
             source=(label.source.name, label.source.variant),
             value_type=label.type,
             entity=label.entity,
             owner=label.owner,
             provider=label.provider,
             location=ResourceColumnMapping("", "", ""),
             description=label.description,
-            status=label.status.Status._enum_type.values[label.status.status].name
+            status=label.status.Status._enum_type.values[label.status.status].name,
         )
 
     def print_label(self, name, variant=None, local=False):
         """Get a label. Prints out information on label, and all variants associated with the label. If variant is included, print information on that specific variant and all resources associated with it.
 
         **Examples:**
 
@@ -3605,38 +3910,34 @@
             definition=definition,
             owner=source.owner,
             provider=source.provider,
             description=source.description,
             variant=source.variant,
             status=source.status.Status._enum_type.values[source.status.status].name,
             tags=[],
-            properties={}
+            properties={},
         )
 
     def _get_source_definition(self, source):
         if source.primaryData.table.name:
-            return PrimaryData(
-                Location(source.primaryData.table.name)
-            )
+            return PrimaryData(Location(source.primaryData.table.name))
         elif source.transformation:
             return self._get_transformation_definition(source)
         else:
             raise Exception(f"Invalid source type {source}")
 
     def _get_transformation_definition(self, source):
         if source.transformation.DFTransformation.query != bytes():
             transformation = source.transformation.DFTransformation
             return DFTransformation(
                 query=transformation.query,
-                inputs=[(input.name, input.variant) for input in transformation.inputs]
+                inputs=[(input.name, input.variant) for input in transformation.inputs],
             )
         elif source.transformation.SQLTransformation.query != "":
-            return SQLTransformation(
-                source.transformation.SQLTransformation.query
-            )
+            return SQLTransformation(source.transformation.SQLTransformation.query)
         else:
             raise Exception(f"Invalid transformation type {source}")
 
     def print_source(self, name, variant=None, local=False):
         """Get a source. Prints out information on source, and all variants associated with the source. If variant is included, print information on that specific variant and all resources associated with it.
 
         **Examples:**
@@ -3784,15 +4085,17 @@
         ]
         ```
 
         Returns:
             features (List[Feature]): List of Feature Objects
         """
         if local:
-            return list_local("feature", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS])
+            return list_local(
+                "feature", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS]
+            )
         return list_name_variant_status(self._stub, "feature")
 
     def list_labels(self, local=False):
         """List all labels.
 
         **Examples:**
         ``` py title="Input"
@@ -3825,15 +4128,17 @@
         ]
         ```
 
         Returns:
             labels (List[Label]): List of Label Objects
         """
         if local:
-            return list_local("label", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS])
+            return list_local(
+                "label", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS]
+            )
         return list_name_variant_status(self._stub, "label")
 
     def list_users(self, local=False):
         """List all users. Prints a list of all users.
 
         **Examples:**
         ``` py title="Input"
@@ -3987,16 +4292,23 @@
         ]
         ```
 
         Returns:
             sources (List[Source]): List of Source Objects
         """
         if local:
-            return list_local("source",
-                              [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS, ColumnName.DESCRIPTION])
+            return list_local(
+                "source",
+                [
+                    ColumnName.NAME,
+                    ColumnName.VARIANT,
+                    ColumnName.STATUS,
+                    ColumnName.DESCRIPTION,
+                ],
+            )
         return list_name_variant_status_desc(self._stub, "source")
 
     def list_training_sets(self, local=False):
         """List all training sets. Prints a list of all training sets.
 
         **Examples:**
         ``` py title="Input"
@@ -4028,15 +4340,17 @@
         ]
         ```
 
         Returns:
             training_sets (List[TrainingSet]): List of TrainingSet Objects
         """
         if local:
-            return list_local("training-set", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS])
+            return list_local(
+                "training-set", [ColumnName.NAME, ColumnName.VARIANT, ColumnName.STATUS]
+            )
         return list_name_variant_status_desc(self._stub, "training-set")
 
     def list_models(self, local=False) -> List[Model]:
         """List all models. Prints a list of all models.
 
         Returns:
             models (List[Model]): List of Model Objects
@@ -4044,15 +4358,17 @@
         models = []
         if local:
             rows = list_local("model", [ColumnName.NAME])
             models = [Model(row["name"], tags=[], properties={}) for row in rows]
         else:
             model_protos = list_name(self._stub, "model")
             # TODO: apply values from proto
-            models = [Model(proto.name, tags=[], properties={}) for proto in model_protos]
+            models = [
+                Model(proto.name, tags=[], properties={}) for proto in model_protos
+            ]
 
         return models
 
     def list_providers(self, local=False):
         """List all providers. Prints a list of all providers.
 
         **Examples:**
@@ -4116,15 +4432,17 @@
         ]
         ```
 
         Returns:
             providers (List[Provider]): List of Provider Objects
         """
         if local:
-            return list_local("provider", [ColumnName.NAME, ColumnName.STATUS, ColumnName.DESCRIPTION])
+            return list_local(
+                "provider", [ColumnName.NAME, ColumnName.STATUS, ColumnName.DESCRIPTION]
+            )
         return list_name_status_desc(self._stub, "provider")
 
     def search(self, raw_query, local=False):
         """Search for registered resources. Prints a list of results.
 
         **Examples:**
         ``` py title="Input"
@@ -4136,15 +4454,15 @@
 
         NAME                           VARIANT            TYPE
         avg_transactions               default            Source
         ```
         """
         if type(raw_query) != str or len(raw_query) == 0:
             raise Exception("query must be string and cannot be empty")
-        processed_query = raw_query.translate({ ord(i): None for i in '.,-@!*#'})
+        processed_query = raw_query.translate({ord(i): None for i in ".,-@!*#"})
         if local:
             return search_local(processed_query)
         else:
             return search(processed_query, self._host)
 
 
 class ColumnResource:
@@ -4152,14 +4470,15 @@
     Base class for all column resources. This class is not meant to be instantiated directly.
     In the original syntax, features and labels were registered using the `register_resources`
     method on the sources (e.g. SQL/DF transformation or tables sources); however, in the new
     Class API syntax, features and labels can now be declared as class attributes on an entity
     class. This means that all possible params for either resource must be passed into this base
     class prior to calling `register_column_resources` on the registrar.
     """
+
     def __init__(
         self,
         transformation_args: tuple,
         type: Union[ColumnTypes, str],
         resource_type: str,
         entity: Union[Entity, str],
         variant: str,
@@ -4203,25 +4522,27 @@
             owner=self.owner,
             inference_store=self.inference_store,
             features=features,
             labels=labels,
             timestamp_column=self.timestamp_column,
             schedule=self.schedule,
         )
-    
+
     def features_and_labels(self) -> Tuple[List[ColumnMapping], List[ColumnMapping]]:
-        resources = [{
-            "name": self.name,
-            "variant": self.variant,
-            "column": self.source_column,
-            "type": self.type,
-            "description": self.description,
-            "tags": self.tags,
-            "properties": self.properties,
-        }]
+        resources = [
+            {
+                "name": self.name,
+                "variant": self.variant,
+                "column": self.source_column,
+                "type": self.type,
+                "description": self.description,
+                "tags": self.tags,
+                "properties": self.properties,
+            }
+        ]
         if self.resource_type == "feature":
             features = resources
             labels = []
         elif self.resource_type == "label":
             features = []
             labels = resources
         else:
@@ -4245,65 +4566,73 @@
 
     def register(self):
         for resource in self.resources.values():
             resource.register()
 
 
 class FeatureColumnResource(ColumnResource):
-    def __init__(self,
-                 transformation_args: tuple,
-                 type: Union[ColumnTypes, str],
-                 entity: Union[Entity, str] = "",
-                 variant="default",
-                 owner: str = "",
-                 inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-                 timestamp_column: str = "",
-                 description: str = "",
-                 schedule: str = "",
-                 tags: List[str] = [],
-                 properties: Dict[str, str] = {}):
-        super().__init__(transformation_args=transformation_args,
-                            type=type,
-                            resource_type="feature",
-                            entity=entity,
-                            variant=variant,
-                            owner=owner,
-                            inference_store=inference_store,
-                            timestamp_column=timestamp_column,
-                            description=description,
-                            schedule=schedule,
-                            tags=tags,
-                            properties=properties)
+    def __init__(
+        self,
+        transformation_args: tuple,
+        type: Union[ColumnTypes, str],
+        entity: Union[Entity, str] = "",
+        variant="default",
+        owner: str = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        timestamp_column: str = "",
+        description: str = "",
+        schedule: str = "",
+        tags: List[str] = [],
+        properties: Dict[str, str] = {},
+    ):
+        super().__init__(
+            transformation_args=transformation_args,
+            type=type,
+            resource_type="feature",
+            entity=entity,
+            variant=variant,
+            owner=owner,
+            inference_store=inference_store,
+            timestamp_column=timestamp_column,
+            description=description,
+            schedule=schedule,
+            tags=tags,
+            properties=properties,
+        )
 
 
 class LabelColumnResource(ColumnResource):
-    def __init__(self,
-                 transformation_args: tuple,
-                 type: Union[ColumnTypes, str],
-                 entity: Union[Entity, str] = "",
-                 variant="default",
-                 owner: str = "",
-                 inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
-                 timestamp_column: str = "",
-                 description: str = "",
-                 schedule: str = "",
-                 tags: List[str] = [],
-                 properties: Dict[str, str] = {}):
-        super().__init__(transformation_args=transformation_args,
-                            type=type,
-                            resource_type="label",
-                            entity=entity,
-                            variant=variant,
-                            owner=owner,
-                            inference_store=inference_store,
-                            timestamp_column=timestamp_column,
-                            description=description,
-                            schedule=schedule,
-                            tags=tags,
-                            properties=properties)
+    def __init__(
+        self,
+        transformation_args: tuple,
+        type: Union[ColumnTypes, str],
+        entity: Union[Entity, str] = "",
+        variant="default",
+        owner: str = "",
+        inference_store: Union[str, OnlineProvider, FileStoreProvider] = "",
+        timestamp_column: str = "",
+        description: str = "",
+        schedule: str = "",
+        tags: List[str] = [],
+        properties: Dict[str, str] = {},
+    ):
+        super().__init__(
+            transformation_args=transformation_args,
+            type=type,
+            resource_type="label",
+            entity=entity,
+            variant=variant,
+            owner=owner,
+            inference_store=inference_store,
+            timestamp_column=timestamp_column,
+            description=description,
+            schedule=schedule,
+            tags=tags,
+            properties=properties,
+        )
 
 
 def entity(cls):
     """
     Class decorator for registering entities and their associated features and labels.
 
     **Examples**
```

### Comparing `featureform-1.7.4/src/featureform/register_test.py` & `featureform-1.8.0/src/featureform/register_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,274 +1,314 @@
 import pytest
 from featureform.register import Registrar
-from featureform.resources import SQLTable, SQLTransformation, Source, User, PrimaryData, Entity, Feature, Label, ResourceColumnMapping
-
+from featureform.resources import (
+    SQLTable,
+    SQLTransformation,
+    Source,
+    User,
+    PrimaryData,
+    Entity,
+    Feature,
+    Label,
+    ResourceColumnMapping,
+)
 
 
 @pytest.fixture
 def registrar():
     return Registrar()
 
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "snowflake",
-        "username": "user",
-        "password": "abc",
-        "database": "db",
-        "account": "db",
-        "organization": "org",
-    },
-    {
-        "name": "snowflake",
-        "description": "test",
-        "team": "featureform",
-        "username": "user",
-        "password": "abc",
-        "database": "db",
-        "account": "db",
-        "organization": "org",
-        "schema": "private",
-    },
-])
+@pytest.mark.parametrize(
+    "args",
+    [
+        {
+            "name": "snowflake",
+            "username": "user",
+            "password": "abc",
+            "database": "db",
+            "account": "db",
+            "organization": "org",
+        },
+        {
+            "name": "snowflake",
+            "description": "test",
+            "team": "featureform",
+            "username": "user",
+            "password": "abc",
+            "database": "db",
+            "account": "db",
+            "organization": "org",
+            "schema": "private",
+        },
+    ],
+)
 def test_register_snowflake(registrar, args):
     registrar.register_snowflake(**args)
 
+
 minimal_postgres_args = {
     "name": "postgres",
 }
 
 
-@pytest.mark.parametrize("args", [
-    minimal_postgres_args,
-    {
-        "name": "postgres",
-        "description": "test",
-        "team": "featureform",
-        "host": "localhost",
-        "port": "1234",
-        "user": "Abc",
-        "password": "abc",
-        "database": "db",
-    },
-])
+@pytest.mark.parametrize(
+    "args",
+    [
+        minimal_postgres_args,
+        {
+            "name": "postgres",
+            "description": "test",
+            "team": "featureform",
+            "host": "localhost",
+            "port": "1234",
+            "user": "Abc",
+            "password": "abc",
+            "database": "db",
+        },
+    ],
+)
 def test_register_postgres(registrar, args):
     registrar.register_postgres(**args)
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "azure_blob"
-    },
-    {
-        "name": "azure_blob",
-        "description": "test",
-        "team": "featureform",
-        "account_name": "<account_name>",
-        "account_key": "<account_key>",
-        "container_name": "container",
-        "root_path": "example/path",
-    }
-])
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "azure_blob"},
+        {
+            "name": "azure_blob",
+            "description": "test",
+            "team": "featureform",
+            "account_name": "<account_name>",
+            "account_key": "<account_key>",
+            "container_name": "container",
+            "root_path": "example/path",
+        },
+    ],
+)
 def test_register_blob_store(registrar, args):
     registrar.register_blob_store(**args)
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "redis"
-    },
-    {
-        "name": "redis",
-        "description": "test",
-        "team": "featureform",
-        "host": "localhost",
-        "port": 1234,
-        "password": "abc",
-        "db": 4
-    },
-])
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "redis"},
+        {
+            "name": "redis",
+            "description": "test",
+            "team": "featureform",
+            "host": "localhost",
+            "port": 1234,
+            "password": "abc",
+            "db": 4,
+        },
+    ],
+)
 def test_register_redis(registrar, args):
     registrar.register_redis(**args)
 
 
 minimal_user_args = {
     "name": "user",
 }
 
+
 @pytest.mark.parametrize("args,expected", [(minimal_user_args, User("user"))])
 def test_register_user(registrar, args, expected):
     registrar.register_user(**args)
     assert registrar.state().sorted_list() == [
         expected,
     ]
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "firestore"
-    },
-    {
-        "name": "firestore",
-        "description": "test",
-        "team": "featureform",
-        "collection": "abc",
-        "project_id": "abc",
-        "credentials_path": "abc"
-    },
-])
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "firestore"},
+        {
+            "name": "firestore",
+            "description": "test",
+            "team": "featureform",
+            "collection": "abc",
+            "project_id": "abc",
+            "credentials_path": "abc",
+        },
+    ],
+)
 def test_register_firestore(registrar, args):
     registrar.register_firestore(**args)
-   
+
+
 minimal_user_args = {
     "name": "user",
     "collection": "abc",
     "project_id": "abc",
-    "credentials_path": "abc"
+    "credentials_path": "abc",
 }
-    
+
+
 @pytest.mark.parametrize("args,expected", [(minimal_user_args, User("user"))])
 def test_register_user(registrar, args, expected):
     registrar.register_user(**args)
     assert registrar.state().sorted_list() == [
         expected,
     ]
-    
-@pytest.mark.parametrize("args", [
-    {
-        "name": "dynamodb"
-    },
-    {
-        "name": "dynamodb",
-        "description": "test",
-        "team": "featureform",
-        "region": "abc",
-        "access_key": "abc",
-        "secret_key": "abc"
-    },
-])
+
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "dynamodb"},
+        {
+            "name": "dynamodb",
+            "description": "test",
+            "team": "featureform",
+            "region": "abc",
+            "access_key": "abc",
+            "secret_key": "abc",
+        },
+    ],
+)
 def test_register_dynamodb(registrar, args):
     registrar.register_dynamodb(**args)
 
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "redshift"
-    },
-    {
-        "name": "redshift",
-        "description": "test",
-        "team": "featureform",
-        "project_id": "abc",
-        "dataset_id": "abc",
-    },
-])
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "redshift"},
+        {
+            "name": "redshift",
+            "description": "test",
+            "team": "featureform",
+            "project_id": "abc",
+            "dataset_id": "abc",
+        },
+    ],
+)
 def test_register_redshift(registrar, args):
     registrar.register_redshift(**args)
 
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "bigquery"
-    },
-    {
-        "name": "bigquery",
-        "description": "test",
-        "team": "featureform",
-        "project_id": "abc",
-        "dataset_id": "abc",
-        "credentials_path": "abc",
-    },
-])
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "bigquery"},
+        {
+            "name": "bigquery",
+            "description": "test",
+            "team": "featureform",
+            "project_id": "abc",
+            "dataset_id": "abc",
+            "credentials_path": "abc",
+        },
+    ],
+)
 def test_register_bigquery(registrar, args):
     registrar.register_bigquery(**args)
 
-    
+
 minimal_user_args = {
     "name": "user",
     "region": "abc",
     "access_key": "abc",
-    "secret_key": "abc"
+    "secret_key": "abc",
 }
 
 
 @pytest.mark.parametrize("args,expected", [(minimal_user_args, User("user"))])
 def test_register_user(registrar, args, expected):
     registrar.register_user(**args)
     assert registrar.state().sorted_list() == [
         expected,
     ]
 
-@pytest.mark.parametrize("args", [
-    {
-        "name": "cassandra"
-    },
-    {
-        "name": "cassandra",
-        "description": "test",
-        "team": "featureform",
-        "host": "localhost",
-        "port": 123,
-        "username" :"abc",
-        "password": "abc",
-        "keyspace": "",
-        "consistency": "THREE",
-        "replication": 3
-    },
-])
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"name": "cassandra"},
+        {
+            "name": "cassandra",
+            "description": "test",
+            "team": "featureform",
+            "host": "localhost",
+            "port": 123,
+            "username": "abc",
+            "password": "abc",
+            "keyspace": "",
+            "consistency": "THREE",
+            "replication": 3,
+        },
+    ],
+)
 def test_register_cassandra(registrar, args):
     registrar.register_cassandra(**args)
 
 
 minimal_user_args = {
     "name": "user",
     "username": "abc",
     "password": "abc",
     "keyspace": "",
     "consistency": "THREE",
-    "replication": 3
+    "replication": 3,
 }
 
+
 @pytest.mark.parametrize("args,expected", [(minimal_user_args, User("user"))])
 def test_register_user(registrar, args, expected):
     registrar.register_user(**args)
     assert registrar.state().sorted_list() == [
         expected,
     ]
 
-@pytest.mark.parametrize("args, expected", [
-    ({
-        "name": "data",
-        "variant": "var",
-        "location": SQLTable("name"),
-        "owner": "user",
-        "provider": "snowflake",
-    },
-     Source(
-         name="data",
-         variant="var",
-         definition=PrimaryData(location=SQLTable("name")),
-         owner="user",
-         provider="snowflake",
-         description="",
-     )),
-    ({
-        "name": "data",
-        "variant": "var",
-        "location": SQLTable("name"),
-        "owner": "user",
-        "provider": "snowflake",
-        "description": "desc",
-    },
-     Source(
-         name="data",
-         variant="var",
-         definition=PrimaryData(location=SQLTable("name")),
-         owner="user",
-         provider="snowflake",
-         description="desc",
-     )),
-])
+
+@pytest.mark.parametrize(
+    "args, expected",
+    [
+        (
+            {
+                "name": "data",
+                "variant": "var",
+                "location": SQLTable("name"),
+                "owner": "user",
+                "provider": "snowflake",
+            },
+            Source(
+                name="data",
+                variant="var",
+                definition=PrimaryData(location=SQLTable("name")),
+                owner="user",
+                provider="snowflake",
+                description="",
+            ),
+        ),
+        (
+            {
+                "name": "data",
+                "variant": "var",
+                "location": SQLTable("name"),
+                "owner": "user",
+                "provider": "snowflake",
+                "description": "desc",
+            },
+            Source(
+                name="data",
+                variant="var",
+                definition=PrimaryData(location=SQLTable("name")),
+                owner="user",
+                provider="snowflake",
+                description="desc",
+            ),
+        ),
+    ],
+)
 def test_register_primary_data(registrar, args, expected):
     registrar.register_primary_data(**args)
     assert registrar.state().sorted_list() == [expected]
 
 
 def test_register_primary_data_with_registrars(registrar):
     user = registrar.register_user(**minimal_user_args)
@@ -326,17 +366,17 @@
         description="doc string",
     )
 
 
 def test_sql_transformation_decorator_with_registrar(registrar):
     user = registrar.register_user(**minimal_user_args)
     postgres = registrar.register_postgres(**minimal_postgres_args)
-    decorator = registrar.sql_transformation(variant="var",
-                                             owner=user,
-                                             provider=postgres)
+    decorator = registrar.sql_transformation(
+        variant="var", owner=user, provider=postgres
+    )
     decorator(name)
     assert decorator.to_source() == Source(
         name="name",
         variant="var",
         definition=SQLTransformation(query="query"),
         owner="user",
         provider="postgres",
@@ -344,15 +384,17 @@
     )
 
 
 def test_offline_store_sql_transformation_decorator(registrar):
     user = registrar.register_user(**minimal_user_args)
     user.make_default_owner()
     postgres = registrar.register_postgres(**minimal_postgres_args)
-    decorator = postgres.sql_transformation(variant="var",)
+    decorator = postgres.sql_transformation(
+        variant="var",
+    )
     decorator(name)
     assert decorator.to_source() == Source(
         name="name",
         variant="var",
         definition=SQLTransformation(query="query"),
         owner="user",
         provider="postgres",
@@ -432,137 +474,138 @@
         variant="var",
         query="query",
         provider=postgres,
         description="doc string",
     )
 
 
-@pytest.mark.parametrize("args, expected", [
-    ({
-        "name": "user",
-    }, Entity(
-        name="user",
-        description="",
-    )),
-    ({
-        "name": "user",
-        "description": "desc",
-    }, Entity(
-        name="user",
-        description="desc",
-    )),
-])
+@pytest.mark.parametrize(
+    "args, expected",
+    [
+        (
+            {
+                "name": "user",
+            },
+            Entity(
+                name="user",
+                description="",
+            ),
+        ),
+        (
+            {
+                "name": "user",
+                "description": "desc",
+            },
+            Entity(
+                name="user",
+                description="desc",
+            ),
+        ),
+    ],
+)
 def test_register_entity(registrar, args, expected):
     registrar.register_entity(**args)
     assert registrar.state().sorted_list() == [expected]
 
 
 def test_register_column_resources(registrar):
     registrar.register_column_resources(
         source=("name", "variant"),
         entity="user",
         entity_column="user_clm",
         inference_store="redis",
-        features=[{
-            "name": "f1",
-            "variant": "v1",
-            "column": "value",
-            "type": "float32"
-        }],
-        labels=[{
-            "name": "l1",
-            "variant": "lv1",
-            "column": "label",
-            "type": "string"
-        }],
+        features=[
+            {"name": "f1", "variant": "v1", "column": "value", "type": "float32"}
+        ],
+        labels=[{"name": "l1", "variant": "lv1", "column": "label", "type": "string"}],
         owner="user",
         timestamp_column="date",
     )
     expected = [
-        Feature(name="f1",
-                variant="v1",
-                source=("name", "variant"),
-                value_type="float32",
-                entity="user",
-                owner="user",
-                provider="redis",
-                description="",
-                location=ResourceColumnMapping(entity="user_clm",
-                                               value="value",
-                                               timestamp="date")),
-        Label(name="l1",
-              variant="lv1",
-              source=("name", "variant"),
-              value_type="string",
-              entity="user",
-              owner="user",
-              description="",
-              location=ResourceColumnMapping(entity="user_clm",
-                                             value="label",
-                                             timestamp="date")),
+        Feature(
+            name="f1",
+            variant="v1",
+            source=("name", "variant"),
+            value_type="float32",
+            entity="user",
+            owner="user",
+            provider="redis",
+            description="",
+            location=ResourceColumnMapping(
+                entity="user_clm", value="value", timestamp="date"
+            ),
+        ),
+        Label(
+            name="l1",
+            variant="lv1",
+            source=("name", "variant"),
+            value_type="string",
+            entity="user",
+            owner="user",
+            description="",
+            location=ResourceColumnMapping(
+                entity="user_clm", value="label", timestamp="date"
+            ),
+        ),
     ]
     assert registrar.state().sorted_list() == expected
 
 
 def test_register_column_features(registrar):
     registrar.register_column_resources(
         source=("name", "variant"),
         entity="user",
         entity_column="user_clm",
         inference_store="redis",
-        features=[{
-            "name": "f1",
-            "variant": "v1",
-            "column": "value",
-            "type": "float32"
-        }],
+        features=[
+            {"name": "f1", "variant": "v1", "column": "value", "type": "float32"}
+        ],
         owner="user",
         timestamp_column="date",
     )
     expected = [
-        Feature(name="f1",
-                variant="v1",
-                source=("name", "variant"),
-                value_type="float32",
-                entity="user",
-                owner="user",
-                provider="redis",
-                description="",
-                location=ResourceColumnMapping(entity="user_clm",
-                                               value="value",
-                                               timestamp="date")),
+        Feature(
+            name="f1",
+            variant="v1",
+            source=("name", "variant"),
+            value_type="float32",
+            entity="user",
+            owner="user",
+            provider="redis",
+            description="",
+            location=ResourceColumnMapping(
+                entity="user_clm", value="value", timestamp="date"
+            ),
+        ),
     ]
     assert registrar.state().sorted_list() == expected
 
 
 def test_register_column_labels(registrar):
     registrar.register_column_resources(
         source=("name", "variant"),
         entity="user",
         entity_column="user_clm",
-        labels=[{
-            "name": "l1",
-            "variant": "lv1",
-            "column": "label",
-            "type": "string"
-        }],
+        labels=[{"name": "l1", "variant": "lv1", "column": "label", "type": "string"}],
         owner="user",
         timestamp_column="date",
     )
     expected = [
-        Label(name="l1",
-              variant="lv1",
-              source=("name", "variant"),
-              value_type="string",
-              entity="user",
-              owner="user",
-              description="",
-              location=ResourceColumnMapping(entity="user_clm",
-                                             value="label",
-                                             timestamp="date")),
+        Label(
+            name="l1",
+            variant="lv1",
+            source=("name", "variant"),
+            value_type="string",
+            entity="user",
+            owner="user",
+            description="",
+            location=ResourceColumnMapping(
+                entity="user_clm", value="label", timestamp="date"
+            ),
+        ),
     ]
     assert registrar.state().sorted_list() == expected
 
 
 def test_register_column_no_resources_error(registrar):
     with pytest.raises(ValueError):
         registrar.register_column_resources(
@@ -577,37 +620,31 @@
 def test_register_column_no_inference_store_error(registrar):
     with pytest.raises(ValueError):
         registrar.register_column_resources(
             source=("name", "variant"),
             entity="user",
             entity_column="user_clm",
             owner="user",
-            features=[{
-                "name": "f1",
-                "variant": "v1",
-                "column": "value",
-                "type": "float32"
-            }],
+            features=[
+                {"name": "f1", "variant": "v1", "column": "value", "type": "float32"}
+            ],
             timestamp_column="date",
         )
 
 
 def test_register_column_no_owner_error(registrar):
     with pytest.raises(ValueError):
         registrar.register_column_resources(
             source=("name", "variant"),
             entity="user",
             entity_column="user_clm",
             inference_store="redis",
-            features=[{
-                "name": "f1",
-                "variant": "v1",
-                "column": "value",
-                "type": "float32"
-            }],
+            features=[
+                {"name": "f1", "variant": "v1", "column": "value", "type": "float32"}
+            ],
             timestamp_column="date",
         )
 
 
 def test_register_column_resources_with_registrar(registrar):
     entity = registrar.register_entity("user")
     redis = registrar.register_redis("redis")
@@ -619,46 +656,42 @@
         owner="user",
         provider="snowflake",
     )
     source.register_resources(
         entity=entity,
         entity_column="user_clm",
         inference_store=redis,
-        features=[{
-            "name": "f1",
-            "variant": "v1",
-            "column": "value",
-            "type": "float32"
-        }],
-        labels=[{
-            "name": "l1",
-            "variant": "lv1",
-            "column": "label",
-            "type": "string"
-        }],
+        features=[
+            {"name": "f1", "variant": "v1", "column": "value", "type": "float32"}
+        ],
+        labels=[{"name": "l1", "variant": "lv1", "column": "label", "type": "string"}],
         owner=user,
         timestamp_column="date",
     )
     expected = [
-        Feature(name="f1",
-                variant="v1",
-                source=("name", "variant"),
-                value_type="float32",
-                entity="user",
-                owner="person",
-                provider="redis",
-                description="",
-                location=ResourceColumnMapping(entity="user_clm",
-                                               value="value",
-                                               timestamp="date")),
-        Label(name="l1",
-              variant="lv1",
-              source=("name", "variant"),
-              value_type="string",
-              entity="user",
-              owner="person",
-              description="",
-              location=ResourceColumnMapping(entity="user_clm",
-                                             value="label",
-                                             timestamp="date")),
+        Feature(
+            name="f1",
+            variant="v1",
+            source=("name", "variant"),
+            value_type="float32",
+            entity="user",
+            owner="person",
+            provider="redis",
+            description="",
+            location=ResourceColumnMapping(
+                entity="user_clm", value="value", timestamp="date"
+            ),
+        ),
+        Label(
+            name="l1",
+            variant="lv1",
+            source=("name", "variant"),
+            value_type="string",
+            entity="user",
+            owner="person",
+            description="",
+            location=ResourceColumnMapping(
+                entity="user_clm", value="label", timestamp="date"
+            ),
+        ),
     ]
     assert registrar.state().sorted_list()[-2:] == expected
```

### Comparing `featureform-1.7.4/src/featureform/resources.py` & `featureform-1.8.0/src/featureform/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,20 @@
         return OperationType.CREATE
 
     def type(self) -> str:
         return "schedule"
 
     def _create(self, stub) -> None:
         serialized = pb.SetScheduleChangeRequest(
-            resource=pb.ResourceId(pb.NameVariant(name=self.name, variant=self.variant),
-                                   resource_type=self.resource_type), schedule=self.schedule_string)
+            resource=pb.ResourceId(
+                pb.NameVariant(name=self.name, variant=self.variant),
+                resource_type=self.resource_type,
+            ),
+            schedule=self.schedule_string,
+        )
         stub.RequestScheduleChange(serialized)
 
 
 @typechecked
 @dataclass
 class RedisConfig:
     host: str
@@ -78,20 +82,24 @@
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class AWSCredentials:
-    def __init__(self,
-                 aws_access_key_id: str = "",
-                 aws_secret_access_key: str = "",):
+    def __init__(
+        self,
+        aws_access_key_id: str = "",
+        aws_secret_access_key: str = "",
+    ):
         empty_strings = aws_access_key_id == "" or aws_secret_access_key == ""
         if empty_strings:
-            raise Exception("'AWSCredentials' requires all parameters: 'aws_access_key_id', 'aws_secret_access_key'")
+            raise Exception(
+                "'AWSCredentials' requires all parameters: 'aws_access_key_id', 'aws_secret_access_key'"
+            )
 
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
 
     def type(self):
         return "AWS_CREDENTIALS"
 
@@ -101,18 +109,19 @@
             "AWSSecretKey": self.aws_secret_access_key,
         }
 
 
 @typechecked
 @dataclass
 class GCPCredentials:
-    def __init__(self,
-                 project_id: str,
-                 credentials_path: str,):
-
+    def __init__(
+        self,
+        project_id: str,
+        credentials_path: str,
+    ):
         self.project_id = project_id
         self.credentials = json.load(open(credentials_path))
 
     def type(self):
         return "GCPCredentials"
 
     def config(self):
@@ -188,24 +197,26 @@
     def store_type(self):
         return self.type()
 
 
 @typechecked
 @dataclass
 class S3StoreConfig:
-    def __init__(self, 
-                 bucket_path: str,
-                 bucket_region: str,
-                 credentials: AWSCredentials,
-                 path: str = ""):
+    def __init__(
+        self,
+        bucket_path: str,
+        bucket_region: str,
+        credentials: AWSCredentials,
+        path: str = "",
+    ):
         bucket_path_ends_with_slash = len(bucket_path) != 0 and bucket_path[-1] == "/"
 
         if bucket_path_ends_with_slash:
             raise Exception("The 'bucket_path' cannot end with '/'.")
-                 
+
         self.bucket_path = bucket_path
         self.bucket_region = bucket_region
         self.credentials = credentials
         self.path = path
 
     def software(self) -> str:
         return "S3"
@@ -220,26 +231,23 @@
     def config(self):
         return {
             "Credentials": self.credentials.config(),
             "BucketRegion": self.bucket_region,
             "BucketPath": self.bucket_path,
             "Path": self.path,
         }
-    
+
     def store_type(self):
         return self.type()
 
+
 @typechecked
 @dataclass
 class HDFSConfig:
-    def __init__(self,
-                 host: str,
-                 port: str,
-                 path: str,
-                 username: str):
+    def __init__(self, host: str, port: str, path: str, username: str):
         bucket_path_ends_with_slash = len(path) != 0 and path[-1] == "/"
 
         if bucket_path_ends_with_slash:
             raise Exception("The 'bucket_path' cannot end with '/'.")
 
         self.path = path
         self.host = host
@@ -253,24 +261,24 @@
         return "HDFS"
 
     def serialize(self) -> bytes:
         config = {
             "Host": self.host,
             "Port": self.port,
             "Path": self.path,
-            "Username": self.username
+            "Username": self.username,
         }
         return bytes(json.dumps(config), "utf-8")
 
     def config(self):
         return {
             "Host": self.host,
             "Port": self.port,
             "Path": self.path,
-            "Username": self.username
+            "Username": self.username,
         }
 
     def store_type(self):
         return self.type()
 
 
 @typechecked
@@ -338,15 +346,15 @@
     def serialize(self) -> bytes:
         config = {
             "Keyspace": self.keyspace,
             "Addr": f"{self.host}:{self.port}",
             "Username": self.username,
             "Password": self.password,
             "Consistency": self.consistency,
-            "Replication": self.replication
+            "Replication": self.replication,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class DynamodbConfig:
@@ -360,15 +368,15 @@
     def type(self) -> str:
         return "DYNAMODB_ONLINE"
 
     def serialize(self) -> bytes:
         config = {
             "Region": self.region,
             "AccessKey": self.access_key,
-            "SecretKey": self.secret_key
+            "SecretKey": self.secret_key,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class MongoDBConfig:
@@ -388,32 +396,30 @@
     def serialize(self) -> bytes:
         config = {
             "Username": self.username,
             "Password": self.password,
             "Host": self.host,
             "Port": self.port,
             "Database": self.database,
-            "Throughput": self.throughput
+            "Throughput": self.throughput,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class LocalConfig:
-
     def software(self) -> str:
         return "localmode"
 
     def type(self) -> str:
         return "LOCAL_ONLINE"
 
     def serialize(self) -> bytes:
-        config = {
-        }
+        config = {}
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class SnowflakeConfig:
     username: str
@@ -424,24 +430,28 @@
     database: str = ""
     account_locator: str = ""
     warehouse: str = ""
     role: str = ""
 
     def __post_init__(self):
         if self.__has_legacy_credentials() and self.__has_current_credentials():
-            raise ValueError("Cannot create configure Snowflake with both current and legacy credentials")
+            raise ValueError(
+                "Cannot create configure Snowflake with both current and legacy credentials"
+            )
 
         if not self.__has_legacy_credentials() and not self.__has_current_credentials():
             raise ValueError("Cannot create configure Snowflake without credentials")
 
     def __has_legacy_credentials(self) -> bool:
         return self.account_locator != ""
 
     def __has_current_credentials(self) -> bool:
-        if (self.account != "" and self.organization == "") or (self.account == "" and self.organization != ""):
+        if (self.account != "" and self.organization == "") or (
+            self.account == "" and self.organization != ""
+        ):
             raise ValueError("Both Snowflake organization and account must be included")
         elif self.account != "" and self.organization != "":
             return True
         else:
             return False
 
     def software(self) -> str:
@@ -456,15 +466,15 @@
             "Password": self.password,
             "Organization": self.organization,
             "AccountLocator": self.account_locator,
             "Account": self.account,
             "Schema": self.schema,
             "Database": self.database,
             "Warehouse": self.warehouse,
-            "Role": self.role
+            "Role": self.role,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
 @dataclass
 class PostgresConfig:
@@ -558,34 +568,38 @@
             "ExecutorType": self.executor_type,
             "StoreType": self.store_type,
             "ExecutorConfig": self.executor_config,
             "StoreConfig": self.store_config,
         }
         return bytes(json.dumps(config), "utf-8")
 
+
 @typechecked
 @dataclass
 class K8sResourceSpecs:
     cpu_request: str = ""
     cpu_limit: str = ""
     memory_request: str = ""
     memory_limit: str = ""
 
+
 @typechecked
 @dataclass
 class K8sArgs:
     docker_image: str
     specs: Union[K8sResourceSpecs, None] = None
 
     def apply(self, transformation: pb.Transformation):
         transformation.kubernetes_args.docker_image = self.docker_image
         if self.specs is not None:
             transformation.kubernetes_args.specs.cpu_request = self.specs.cpu_request
             transformation.kubernetes_args.specs.cpu_limit = self.specs.cpu_limit
-            transformation.kubernetes_args.specs.memory_request = self.specs.memory_request
+            transformation.kubernetes_args.specs.memory_request = (
+                self.specs.memory_request
+            )
             transformation.kubernetes_args.specs.memory_limit = self.specs.memory_limit
         return transformation
 
 
 @typechecked
 @dataclass
 class K8sConfig:
@@ -598,17 +612,15 @@
 
     def type(self) -> str:
         return "K8S_OFFLINE"
 
     def serialize(self) -> bytes:
         config = {
             "ExecutorType": "K8S",
-            "ExecutorConfig": {
-                "docker_image": self.docker_image
-            },
+            "ExecutorConfig": {"docker_image": self.docker_image},
             "StoreType": self.store_type,
             "StoreConfig": self.store_config,
         }
         return bytes(json.dumps(config), "utf-8")
 
 
 @typechecked
@@ -621,19 +633,33 @@
         return ""
 
     def serialize(self) -> bytes:
         return bytes("", "utf-8")
 
 
 Config = Union[
-    RedisConfig, SnowflakeConfig, PostgresConfig, RedshiftConfig, LocalConfig, BigQueryConfig,
-    FirestoreConfig, SparkConfig, OnlineBlobConfig, AzureFileStoreConfig, S3StoreConfig, K8sConfig,
-    MongoDBConfig, GCSFileStoreConfig, EmptyConfig
+    RedisConfig,
+    SnowflakeConfig,
+    PostgresConfig,
+    RedshiftConfig,
+    LocalConfig,
+    BigQueryConfig,
+    FirestoreConfig,
+    SparkConfig,
+    OnlineBlobConfig,
+    AzureFileStoreConfig,
+    S3StoreConfig,
+    K8sConfig,
+    MongoDBConfig,
+    GCSFileStoreConfig,
+    EmptyConfig,
+    HDFSConfig,
 ]
 
+
 @typechecked
 @dataclass
 class Properties:
     properties: dict
 
     def __post_init__(self):
         self.serialized = pb.Properties()
@@ -661,28 +687,30 @@
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
         return "provider"
 
-    def get(self, stub) -> 'Provider':
+    def get(self, stub) -> "Provider":
         name = pb.Name(name=self.name)
         provider = next(stub.GetProviders(iter([name])))
 
         return Provider(
             name=provider.name,
             description=provider.description,
             function=provider.type,
             team=provider.team,
             config=EmptyConfig(),  # TODO add deserializer to configs
             tags=list(provider.tags.tag),
             properties={k: v for k, v in provider.properties.property.items()},
-            status=provider.status.Status._enum_type.values[provider.status.status].name,
-            error=provider.status.error_message
+            status=provider.status.Status._enum_type.values[
+                provider.status.status
+            ].name,
+            error=provider.status.error_message,
         )
 
     def _create(self, stub) -> None:
         serialized = pb.Provider(
             name=self.name,
             description=self.description,
             type=self.config.type(),
@@ -691,29 +719,32 @@
             serialized_config=self.config.serialize(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateProvider(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("providers",
-                  self.name,
-                  "Provider",
-                  self.description,
-                  self.config.type(),
-                  self.config.software(),
-                  self.team,
-                  "sources",
-                  "ready",
-                  str(self.config.serialize(), 'utf-8')
-                  )
+        db.insert(
+            "providers",
+            self.name,
+            "Provider",
+            self.description,
+            self.config.type(),
+            self.config.software(),
+            self.team,
+            "sources",
+            "ready",
+            str(self.config.serialize(), "utf-8"),
+        )
         if len(self.tags):
             db.upsert("tags", self.name, "", "providers", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert("properties", self.name, "", "providers", json.dumps(self.properties))
+            db.upsert(
+                "properties", self.name, "", "providers", json.dumps(self.properties)
+            )
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
@@ -737,19 +768,15 @@
             name=self.name,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateUser(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("users",
-                  self.name,
-                  "User",
-                  "ready"
-                  )
+        db.insert("users", self.name, "User", "ready")
         if len(self.tags):
             db.upsert("tags", self.name, "", "users", json.dumps(self.tags))
         if len(self.properties):
             db.upsert("properties", self.name, "", "users", json.dumps(self.properties))
 
     def __eq__(self, other):
         for attribute in vars(self):
@@ -770,17 +797,19 @@
 @typechecked
 @dataclass
 class PrimaryData:
     location: Location
 
     def kwargs(self):
         return {
-            "primaryData":
-                pb.PrimaryData(table=pb.PrimarySQLTable(
-                    name=self.location.name, ), ),
+            "primaryData": pb.PrimaryData(
+                table=pb.PrimarySQLTable(
+                    name=self.location.name,
+                ),
+            ),
         }
 
     def name(self):
         return self.location.name
 
 
 class Transformation:
@@ -802,17 +831,15 @@
                 query=self.query,
             )
         )
 
         if self.args is not None:
             transformation = self.args.apply(transformation)
 
-        return {
-            "transformation": transformation
-        }
+        return {"transformation": transformation}
 
 
 @typechecked
 @dataclass
 class DFTransformation(Transformation):
     query: bytes
     inputs: list
@@ -821,24 +848,22 @@
     def type(self):
         return SourceType.DF_TRANSFORMATION.value
 
     def kwargs(self):
         transformation = pb.Transformation(
             DFTransformation=pb.DFTransformation(
                 query=self.query,
-                inputs=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.inputs]
+                inputs=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.inputs],
             )
         )
-        
+
         if self.args is not None:
             transformation = self.args.apply(transformation)
 
-        return {
-            "transformation": transformation
-        }
+        return {"transformation": transformation}
 
 
 SourceDefinition = Union[PrimaryData, Transformation]
 
 
 @typechecked
 @dataclass
@@ -851,19 +876,25 @@
     tags: list
     properties: dict
     status: str = "NO_STATUS"
     variant: str = "default"
     schedule: str = ""
     schedule_obj: Schedule = None
     is_transformation = SourceType.PRIMARY_SOURCE.value
-    inputs = [],
+    inputs = ([],)
     error: Optional[str] = None
+    status: str = "NO_STATUS"
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=7, schedule_string=schedule)
+        self.schedule_obj = Schedule(
+            name=self.name,
+            variant=self.variant,
+            resource_type=7,
+            schedule_string=schedule,
+        )
         self.schedule = schedule
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
@@ -886,33 +917,29 @@
             properties={k: v for k, v in source.properties.property.items()},
             status=source.status.Status._enum_type.values[source.status.status].name,
             error=source.status.error_message,
         )
 
     def _get_source_definition(self, source):
         if source.primaryData.table.name:
-            return PrimaryData(
-                Location(source.primaryData.table.name)
-            )
+            return PrimaryData(Location(source.primaryData.table.name))
         elif source.transformation:
             return self._get_transformation_definition(source)
         else:
             raise Exception(f"Invalid source type {source}")
 
     def _get_transformation_definition(self, source):
         if source.transformation.DFTransformation.query != bytes():
             transformation = source.transformation.DFTransformation
             return DFTransformation(
                 query=transformation.query,
-                inputs=[(input.name, input.variant) for input in transformation.inputs]
+                inputs=[(input.name, input.variant) for input in transformation.inputs],
             )
         elif source.transformation.SQLTransformation.query != "":
-            return SQLTransformation(
-                source.transformation.SQLTransformation.query
-            )
+            return SQLTransformation(source.transformation.SQLTransformation.query)
         else:
             raise Exception(f"Invalid transformation type {source}")
 
     def _create(self, stub) -> None:
         defArgs = self.definition.kwargs()
         serialized = pb.SourceVariant(
             name=self.name,
@@ -934,40 +961,44 @@
             self.definition = self.definition.query
         elif type(self.definition) == SQLTransformation:
             self.is_transformation = SourceType.SQL_TRANSFORMATION.value
             self.definition = self.definition.query
         elif type(self.definition) == PrimaryData:
             self.definition = self.definition.name()
             self.is_transformation = SourceType.PRIMARY_SOURCE.value
-        db.insert_source("source_variant",
-                         str(time.time()),
-                         self.description,
-                         self.name,
-                         "Source",
-                         self.owner,
-                         self.provider,
-                         self.variant,
-                         "ready",
-                         self.is_transformation,
-                         json.dumps(self.inputs),
-                         self.definition
-                         )
+        db.insert_source(
+            "source_variant",
+            str(time.time()),
+            self.description,
+            self.name,
+            "Source",
+            self.owner,
+            self.provider,
+            self.variant,
+            "ready",
+            self.is_transformation,
+            json.dumps(self.inputs),
+            self.definition,
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "source_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags", self.name, self.variant, "source_variant", json.dumps(self.tags)
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "source_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "source_variant",
+                json.dumps(self.properties),
+            )
         self._create_source_resource(db)
 
     def _create_source_resource(self, db) -> None:
-        db.insert(
-            "sources",
-            "Source",
-            self.variant,
-            self.name
-        )
+        db.insert("sources", "Source", self.variant, self.name)
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1000,24 +1031,21 @@
             description=self.description,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateEntity(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("entities",
-                  self.name,
-                  "Entity",
-                  self.description,
-                  "ready"
-                  )
+        db.insert("entities", self.name, "Entity", self.description, "ready")
         if len(self.tags):
             db.upsert("tags", self.name, "", "entities", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert("properties", self.name, "", "entities", json.dumps(self.properties))
+            db.upsert(
+                "properties", self.name, "", "entities", json.dumps(self.properties)
+            )
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
@@ -1058,18 +1086,25 @@
     schedule_obj: Schedule = None
     status: str = "NO_STATUS"
     error: Optional[str] = None
 
     def __post_init__(self):
         col_types = [member.value for member in ColumnTypes]
         if self.value_type not in col_types:
-            raise ValueError(f"Invalid feature type ({self.value_type}) must be one of: {col_types}")
+            raise ValueError(
+                f"Invalid feature type ({self.value_type}) must be one of: {col_types}"
+            )
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=4, schedule_string=schedule)
+        self.schedule_obj = Schedule(
+            name=self.name,
+            variant=self.variant,
+            resource_type=4,
+            schedule_string=schedule,
+        )
         self.schedule = schedule
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
@@ -1114,34 +1149,47 @@
             mode=ComputationMode.PRECOMPUTED.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateFeatureVariant(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("feature_variant",
-                  str(time.time()),
-                  self.description,
-                  self.entity,
-                  self.name,
-                  self.owner,
-                  self.provider,
-                  self.value_type,
-                  self.variant,
-                  "ready",
-                  self.location.entity,
-                  self.location.timestamp,
-                  self.location.value,
-                  self.source[0],
-                  self.source[1]
-                  )
+        db.insert(
+            "feature_variant",
+            str(time.time()),
+            self.description,
+            self.entity,
+            self.name,
+            self.owner,
+            self.provider,
+            self.value_type,
+            self.variant,
+            "ready",
+            self.location.entity,
+            self.location.timestamp,
+            self.location.value,
+            self.source[0],
+            self.source[1],
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "feature_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags",
+                self.name,
+                self.variant,
+                "feature_variant",
+                json.dumps(self.tags),
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "feature_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "feature_variant",
+                json.dumps(self.properties),
+            )
 
         self._write_feature_variant_and_mode(db)
 
     def _write_feature_variant_and_mode(self, db) -> None:
         db.insert(
             "features",
             self.name,
@@ -1165,14 +1213,15 @@
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
+
 @typechecked
 @dataclass
 class OnDemandFeature:
     owner: str
     tags: List[str] = field(default_factory=list)
     properties: dict = field(default_factory=dict)
     variant: str = "default"
@@ -1216,27 +1265,40 @@
             status=pb.ResourceStatus(status=pb.ResourceStatus.READY),
         )
         stub.CreateFeatureVariant(serialized)
 
     def _create_local(self, db) -> None:
         decode_query = base64.b64encode(self.query).decode("ascii")
 
-        db.insert("ondemand_feature_variant",
-                  str(time.time()),
-                  self.description,
-                  self.name,
-                  self.owner,
-                  self.variant,
-                  "ready",
-                  decode_query,
-                  )
+        db.insert(
+            "ondemand_feature_variant",
+            str(time.time()),
+            self.description,
+            self.name,
+            self.owner,
+            self.variant,
+            "ready",
+            decode_query,
+        )
         if self.tags and len(self.tags):
-            db.upsert("tags", self.name, self.variant, "feature_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags",
+                self.name,
+                self.variant,
+                "feature_variant",
+                json.dumps(self.tags),
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "feature_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "feature_variant",
+                json.dumps(self.properties),
+            )
 
         self._write_feature_variant_and_mode(db)
 
     def _write_feature_variant_and_mode(self, db) -> None:
         db.insert(
             "features",
             self.name,
@@ -1248,27 +1310,29 @@
         db.insert(
             "feature_computation_mode",
             self.name,
             self.variant,
             ComputationMode.CLIENT_COMPUTED.value,
             is_on_demand,
         )
-    
+
     def get(self, stub) -> "OnDemandFeature":
         name_variant = pb.NameVariant(name=self.name, variant=self.variant)
         ondemand_feature = next(stub.GetFeatureVariants(iter([name_variant])))
 
         return OnDemandFeature(
             name=ondemand_feature.name,
             variant=ondemand_feature.variant,
             owner=ondemand_feature.owner,
             description=ondemand_feature.description,
             tags=list(ondemand_feature.tags.tag),
             properties={k: v for k, v in ondemand_feature.properties.property.items()},
-            status=ondemand_feature.status.Status._enum_type.values[ondemand_feature.status.status].name,
+            status=ondemand_feature.status.Status._enum_type.values[
+                ondemand_feature.status.status
+            ].name,
             error=ondemand_feature.status.error_message,
         )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
@@ -1297,15 +1361,17 @@
     status: str = "NO_STATUS"
     variant: str = "default"
     error: Optional[str] = None
 
     def __post_init__(self):
         col_types = [member.value for member in ColumnTypes]
         if self.value_type not in col_types:
-            raise ValueError(f"Invalid label type ({self.value_type}) must be one of: {col_types}")
+            raise ValueError(
+                f"Invalid label type ({self.value_type}) must be one of: {col_types}"
+            )
 
     @staticmethod
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     @staticmethod
     def type() -> str:
@@ -1324,15 +1390,15 @@
             owner=label.owner,
             provider=label.provider,
             location=ResourceColumnMapping("", "", ""),
             description=label.description,
             tags=list(label.tags.tag),
             properties={k: v for k, v in label.properties.property.items()},
             status=label.status.Status._enum_type.values[label.status.status].name,
-            error=label.status.error_message
+            error=label.status.error_message,
         )
 
     def _create(self, stub) -> None:
         serialized = pb.LabelVariant(
             name=self.name,
             variant=self.variant,
             source=pb.NameVariant(
@@ -1346,43 +1412,47 @@
             columns=self.location.proto(),
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateLabelVariant(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("label_variant",
-                  str(time.time()),
-                  self.description,
-                  self.entity,
-                  self.name,
-                  self.owner,
-                  self.provider,
-                  self.value_type,
-                  self.variant,
-                  self.location.entity,
-                  self.location.timestamp,
-                  self.location.value,
-                  "ready",
-                  self.source[0],
-                  self.source[1]
-                  )
+        db.insert(
+            "label_variant",
+            str(time.time()),
+            self.description,
+            self.entity,
+            self.name,
+            self.owner,
+            self.provider,
+            self.value_type,
+            self.variant,
+            self.location.entity,
+            self.location.timestamp,
+            self.location.value,
+            "ready",
+            self.source[0],
+            self.source[1],
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "label_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags", self.name, self.variant, "label_variant", json.dumps(self.tags)
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "label_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "label_variant",
+                json.dumps(self.properties),
+            )
         self._create_label_resource(db)
 
     def _create_label_resource(self, db) -> None:
-        db.insert(
-            "labels",
-            self.value_type,
-            self.variant,
-            self.name
-        )
+        db.insert("labels", self.value_type, self.variant, self.name)
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
 
@@ -1439,15 +1509,17 @@
 
     def _get(self, stub):
         providerList = stub.GetProviders(iter([pb.Name(name=self.name)]))
         try:
             for provider in providerList:
                 self.obj = provider
         except grpc._channel._MultiThreadedRendezvous:
-            raise ValueError(f"Provider {self.name} of type {self.provider_type} not found.")
+            raise ValueError(
+                f"Provider {self.name} of type {self.provider_type} not found."
+            )
 
     def _get_local(self, db):
         local_provider = db.query_resource("providers", "name", self.name)
         if local_provider == []:
             raise ValueError("Local mode provider not found.")
         self.obj = local_provider
 
@@ -1464,15 +1536,17 @@
         return OperationType.GET
 
     @staticmethod
     def type() -> str:
         return "source"
 
     def _get(self, stub):
-        sourceList = stub.GetSourceVariants(iter([pb.NameVariant(name=self.name, variant=self.variant)]))
+        sourceList = stub.GetSourceVariants(
+            iter([pb.NameVariant(name=self.name, variant=self.variant)])
+        )
         try:
             for source in sourceList:
                 self.obj = source
         except grpc._channel._MultiThreadedRendezvous:
             raise ValueError(f"Source {self.name}, variant {self.variant} not found.")
 
     def _get_local(self, db):
@@ -1497,15 +1571,20 @@
     schedule: str = ""
     schedule_obj: Schedule = None
     provider: str = ""
     status: str = "NO_STATUS"
     error: Optional[str] = None
 
     def update_schedule(self, schedule) -> None:
-        self.schedule_obj = Schedule(name=self.name, variant=self.variant, resource_type=6, schedule_string=schedule)
+        self.schedule_obj = Schedule(
+            name=self.name,
+            variant=self.variant,
+            resource_type=6,
+            schedule_string=schedule,
+        )
         self.schedule = schedule
 
     def __post_init__(self):
         if not valid_name_variant(self.label):
             raise ValueError("Label must be set")
         if len(self.features) == 0:
             raise ValueError("A training-set must have atleast one feature")
@@ -1555,65 +1634,79 @@
 
         serialized = pb.TrainingSetVariant(
             name=self.name,
             variant=self.variant,
             description=self.description,
             schedule=self.schedule,
             owner=self.owner,
-            features=[
-                pb.NameVariant(name=v[0], variant=v[1]) for v in self.features
-            ],
+            features=[pb.NameVariant(name=v[0], variant=v[1]) for v in self.features],
             label=pb.NameVariant(name=self.label[0], variant=self.label[1]),
             feature_lags=feature_lags,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateTrainingSetVariant(serialized)
 
     def _create_local(self, db) -> None:
         self._check_insert_training_set_resources(db)
-        db.insert("training_set_variant",
-                  str(time.time()),
-                  self.description,
-                  self.name,
-                  self.owner,
-                  self.variant,
-                  self.label[0],
-                  self.label[1],
-                  "ready"
-                  )
+        db.insert(
+            "training_set_variant",
+            str(time.time()),
+            self.description,
+            self.name,
+            self.owner,
+            self.variant,
+            self.label[0],
+            self.label[1],
+            "ready",
+        )
         if len(self.tags):
-            db.upsert("tags", self.name, self.variant, "training_set_variant", json.dumps(self.tags))
+            db.upsert(
+                "tags",
+                self.name,
+                self.variant,
+                "training_set_variant",
+                json.dumps(self.tags),
+            )
         if len(self.properties):
-            db.upsert("properties", self.name, self.variant, "training_set_variant", json.dumps(self.properties))
+            db.upsert(
+                "properties",
+                self.name,
+                self.variant,
+                "training_set_variant",
+                json.dumps(self.properties),
+            )
         self._create_training_set_resource(db)
 
     def _create_training_set_resource(self, db) -> None:
-        db.insert(
-            "training_sets",
-            "TrainingSet",
-            self.variant,
-            self.name
-        )
+        db.insert("training_sets", "TrainingSet", self.variant, self.name)
 
     def _check_insert_training_set_resources(self, db) -> None:
         try:
             db.get_label_variant(self.label[0], self.label[1])
         except ValueError:
-            raise ValueError(f"{self.label[0]} does not exist. Failed to register training set")
+            raise ValueError(
+                f"{self.label[0]} does not exist. Failed to register training set"
+            )
 
         for feature_name, feature_variant in self.features:
             try:
-                is_on_demand = db.get_feature_variant_on_demand(feature_name, feature_variant)
+                is_on_demand = db.get_feature_variant_on_demand(
+                    feature_name, feature_variant
+                )
                 if is_on_demand:
-                    raise InvalidTrainingSetFeatureComputationMode(feature_name, feature_variant)
+                    raise InvalidTrainingSetFeatureComputationMode(
+                        feature_name, feature_variant
+                    )
             except InvalidTrainingSetFeatureComputationMode as e:
                 raise e
             except Exception as e:
-                raise Exception(f"{feature_name}:{feature_variant} does not exist. Failed to register training set. Error: {e}")
+                raise Exception(
+                    f"{feature_name}:{feature_variant} does not exist. Failed to register training set. Error: {e}"
+                )
 
             db.insert(
                 "training_set_features",
                 self.name,
                 self.variant,
                 feature_name,  # feature name
                 feature_variant,  # feature variant
@@ -1624,24 +1717,26 @@
             feature_variant = feature["variant"]
             feature_new_name = feature["name"]
             feature_lag = feature["lag"].total_seconds()
 
             try:
                 db.get_feature_variant(feature_name, feature_variant)
             except Exception as e:
-                raise Exception(f"{feature_name} does not exist. Failed to register training set. Error: {e}")
+                raise Exception(
+                    f"{feature_name} does not exist. Failed to register training set. Error: {e}"
+                )
 
             db.insert(
                 "training_set_lag_features",
                 self.name,
                 self.variant,
                 feature_name,  # feature name
                 feature_variant,  # feature variant
                 feature_new_name,  # feature new name
-                feature_lag  # feature_lag
+                feature_lag,  # feature_lag
             )
 
     def get_status(self):
         return ResourceStatus(self.status)
 
     def is_ready(self):
         return self.status == ResourceStatus.READY.value
@@ -1664,74 +1759,94 @@
     def operation_type() -> OperationType:
         return OperationType.CREATE
 
     def type(self) -> str:
         return "model"
 
     def _create(self, stub) -> None:
-        properties = pb.Properties(
-            property=self.properties
-        )
+        properties = pb.Properties(property=self.properties)
         serialized = pb.Model(
             name=self.name,
             tags=pb.Tags(tag=self.tags),
             properties=Properties(self.properties).serialized,
         )
         stub.CreateModel(serialized)
 
     def _create_local(self, db) -> None:
-        db.insert("models",
-                  self.name,
-                  "Model",
-                  )
+        db.insert(
+            "models",
+            self.name,
+            "Model",
+        )
         if len(self.tags):
             db.upsert("tags", self.name, "", "models", json.dumps(self.tags))
         if len(self.properties):
-            db.upsert("properties", self.name, "", "models", json.dumps(self.properties))
+            db.upsert(
+                "properties", self.name, "", "models", json.dumps(self.properties)
+            )
 
     def __eq__(self, other):
         for attribute in vars(self):
             if getattr(self, attribute) != getattr(other, attribute):
                 return False
         return True
 
 
-Resource = Union[PrimaryData, Provider, Entity, User, Feature, Label,
-                 TrainingSet, Source, Schedule, ProviderReference, SourceReference, EntityReference, Model, OnDemandFeature]
+Resource = Union[
+    PrimaryData,
+    Provider,
+    Entity,
+    User,
+    Feature,
+    Label,
+    TrainingSet,
+    Source,
+    Schedule,
+    ProviderReference,
+    SourceReference,
+    EntityReference,
+    Model,
+    OnDemandFeature,
+]
 
 
 class ResourceRedefinedError(Exception):
     @typechecked
     def __init__(self, resource: Resource):
-        variantStr = f" variant {resource.variant}" if hasattr(
-            resource, 'variant') else ""
+        variantStr = (
+            f" variant {resource.variant}" if hasattr(resource, "variant") else ""
+        )
         resourceId = f"{resource.name}{variantStr}"
         super().__init__(
             f"{resource.type()} resource {resourceId} defined in multiple places"
         )
 
 
 class ResourceState:
-
     def __init__(self):
         self.__state = {}
 
     @typechecked
     def add(self, resource: Resource) -> None:
-        if hasattr(resource, 'variant'):
-            key = (resource.operation_type().name, resource.type(), resource.name, resource.variant)
+        if hasattr(resource, "variant"):
+            key = (
+                resource.operation_type().name,
+                resource.type(),
+                resource.name,
+                resource.variant,
+            )
         else:
             key = (resource.operation_type().name, resource.type(), resource.name)
         if key in self.__state:
             if resource == self.__state[key]:
                 print(f"Resource {resource.type()} already registered.")
                 return
             raise ResourceRedefinedError(resource)
         self.__state[key] = resource
-        if hasattr(resource, 'schedule_obj') and resource.schedule_obj != None:
+        if hasattr(resource, "schedule_obj") and resource.schedule_obj != None:
             my_schedule = resource.schedule_obj
             key = (my_schedule.type(), my_schedule.name)
             self.__state[key] = my_schedule
 
     def sorted_list(self) -> List[Resource]:
         resource_order = {
             "user": 0,
@@ -1739,15 +1854,15 @@
             "source": 2,
             "entity": 3,
             "feature": 4,
             "ondemand_feature": 5,
             "label": 6,
             "training-set": 7,
             "schedule": 8,
-            "model": 9
+            "model": 9,
         }
 
         def to_sort_key(res):
             resource_num = resource_order[res.type()]
             variant = res.variant if hasattr(res, "variant") else ""
             return (resource_num, res.name, variant)
 
@@ -1778,107 +1893,133 @@
         for resource in self.sorted_list():
             if resource.type() == "provider" and resource.name == "local-mode":
                 continue
             try:
                 # NOTE: There is an extra space before the variant name to better handle the case
                 # where a resource has no variant; ultimately, we should separate data access and
                 # logging/CLI output to avoid this unnecessary coupling.
-                resource_variant = f" {resource.variant}" if hasattr(resource, "variant") else ""
+                resource_variant = (
+                    f" {resource.variant}" if hasattr(resource, "variant") else ""
+                )
                 if resource.operation_type() is OperationType.GET:
-                    print(f"Getting {resource.type()} {resource.name}{resource_variant}")
+                    print(
+                        f"Getting {resource.type()} {resource.name}{resource_variant}"
+                    )
                     resource._get(stub)
                 if resource.operation_type() is OperationType.CREATE:
-                    print(f"Creating {resource.type()} {resource.name}{resource_variant}")
+                    print(
+                        f"Creating {resource.type()} {resource.name}{resource_variant}"
+                    )
                     resource._create(stub)
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.ALREADY_EXISTS:
                     print(f"{resource.name}{resource_variant} already exists.")
                     continue
 
                 raise e
 
 
 ## Executor Providers
 @typechecked
 class DatabricksCredentials:
-    def __init__(self,
-                 username: str = "",
-                 password: str = "",
-                 host: str = "",
-                 token: str = "",
-                 cluster_id: str = ""):
+    def __init__(
+        self,
+        username: str = "",
+        password: str = "",
+        host: str = "",
+        token: str = "",
+        cluster_id: str = "",
+    ):
         self.username = username
         self.password = password
         self.host = host
         self.token = token
         self.cluster_id = cluster_id
 
-        host_token_provided = username == "" and password == "" and host != "" and token != ""
-        username_password_provided = username != "" and password != "" and host == "" and token == ""
+        host_token_provided = (
+            username == "" and password == "" and host != "" and token != ""
+        )
+        username_password_provided = (
+            username != "" and password != "" and host == "" and token == ""
+        )
 
-        if not host_token_provided and not username_password_provided or host_token_provided and username_password_provided:
+        if (
+            not host_token_provided
+            and not username_password_provided
+            or host_token_provided
+            and username_password_provided
+        ):
             raise Exception(
-                "The DatabricksCredentials requires only one credentials set ('username' and 'password' or 'host' and 'token' set.)")
+                "The DatabricksCredentials requires only one credentials set ('username' and 'password' or 'host' and 'token' set.)"
+            )
 
         if not cluster_id:
             raise Exception("Cluster_id of existing cluster must be provided")
 
     def type(self):
         return "DATABRICKS"
 
     def config(self):
         return {
             "Username": self.username,
             "Password": self.password,
             "Host": self.host,
             "Token": self.token,
-            "Cluster": self.cluster_id
+            "Cluster": self.cluster_id,
         }
 
 
-
 @typechecked
 @dataclass
 class EMRCredentials:
-    def __init__(self,
-                 emr_cluster_id: str,
-                 emr_cluster_region: str,
-                 credentials: AWSCredentials):
-        
+    def __init__(
+        self, emr_cluster_id: str, emr_cluster_region: str, credentials: AWSCredentials
+    ):
         self.emr_cluster_id = emr_cluster_id
         self.emr_cluster_region = emr_cluster_region
         self.credentials = credentials
 
     def type(self):
         return "EMR"
 
     def config(self):
         return {
             "ClusterName": self.emr_cluster_id,
             "ClusterRegion": self.emr_cluster_region,
             "Credentials": self.credentials.config(),
         }
 
+
 @typechecked
 @dataclass
 class SparkCredentials:
-    def __init__(self,
-                 master: str,
-                 deploy_mode: str,
-                 python_version: str = "",
-                ):
-        
+    def __init__(
+        self,
+        master: str,
+        deploy_mode: str,
+        python_version: str = "",
+        core_site_path: str = "",
+        yarn_site_path: str = "",
+    ):
         self.master = master.lower()
         self.deploy_mode = deploy_mode.lower()
+        self.core_site_path = core_site_path
+        self.yarn_site_path = yarn_site_path
 
         if self.deploy_mode != "cluster" and self.deploy_mode != "client":
-            raise Exception(f"Spark does not support '{self.deploy_mode}' deploy mode. It only supports 'cluster' and 'client'.")
+            raise Exception(
+                f"Spark does not support '{self.deploy_mode}' deploy mode. It only supports 'cluster' and 'client'."
+            )
+
+        self.python_version = self._verify_python_version(
+            self.deploy_mode, python_version
+        )
+
+        self._verify_yarn_config()
 
-        self.python_version = self._verify_python_version(self.deploy_mode, python_version)
-    
     def _verify_python_version(self, deploy_mode, version):
         if deploy_mode == "cluster" and version == "":
             client_python_version = sys.version_info
             client_major = str(client_python_version.major)
             client_minor = str(client_python_version.minor)
 
             if client_major != MAJOR_VERSION:
@@ -1887,38 +2028,62 @@
                 client_minor = "7"
 
             version = f"{client_major}.{client_minor}"
 
         if version.count(".") == 2:
             major, minor, _ = version.split(".")
         elif version.count(".") == 1:
-            major, minor = version.split(".")    
+            major, minor = version.split(".")
         else:
-            raise Exception("Please specify your Python version on the Spark cluster. Accepted formats: Major.Minor or Major.Minor.Patch; ex. '3.7' or '3.7.16")
+            raise Exception(
+                "Please specify your Python version on the Spark cluster. Accepted formats: Major.Minor or Major.Minor.Patch; ex. '3.7' or '3.7.16"
+            )
 
         if major != MAJOR_VERSION or minor not in MINOR_VERSIONS:
-            raise Exception(f"The Python version {version} is not supported. Currently, supported versions are 3.7-3.10.")
-        
+            raise Exception(
+                f"The Python version {version} is not supported. Currently, supported versions are 3.7-3.10."
+            )
+
         """
         The Python versions on the Docker image are 3.7.16, 3.8.16, 3.9.16, 3.10.10, and 3.11.2.
         This conditional statement sets the patch number based on the minor version. 
         """
         if minor == "10":
             patch = "10"
         elif minor == "11":
             patch = "2"
         else:
             patch = "16"
-        
+
         return f"{major}.{minor}.{patch}"
 
+    def _verify_yarn_config(self):
+        if self.master == "yarn" and (
+            self.core_site_path == "" or self.yarn_site_path == ""
+        ):
+            raise Exception(
+                "Yarn requires core-site.xml and yarn-site.xml files."
+                "Please copy these files from your Spark instance to local, then provide the local path in "
+                "core_site_path and yarn_site_path. "
+            )
+
     def type(self):
         return "SPARK"
 
     def config(self):
+        core_site = (
+            "" if self.core_site_path == "" else open(self.core_site_path, "r").read()
+        )
+        yarn_site = (
+            "" if self.yarn_site_path == "" else open(self.yarn_site_path, "r").read()
+        )
+
         return {
             "Master": self.master,
             "DeployMode": self.deploy_mode,
-            "PythonVersion": self.python_version
+            "PythonVersion": self.python_version,
+            "CoreSite": core_site,
+            "YarnSite": yarn_site,
         }
 
+
 ExecutorCredentials = Union[EMRCredentials, DatabricksCredentials, SparkCredentials]
```

### Comparing `featureform-1.7.4/src/featureform/search.py` & `featureform-1.8.0/src/featureform/search.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from .format import *
 
 
 def search(phrase, host):
     response = requests.get(f"http://{host}/data/search?q={phrase}")
 
     if response.status_code is not 200:
-        print(f"Search request for {phrase} resulted in HTTP status {response.status_code}")
+        print(
+            f"Search request for {phrase} resulted in HTTP status {response.status_code}"
+        )
         return
-    
+
     results = response.json()
-    
+
     if len(results) == 0:
         print(f"Search phrase {phrase} returned no results.")
     else:
         format_rows("NAME", "VARIANT", "TYPE")
         for r in results:
             format_rows(r["Name"], r["Variant"], r["Type"])
-    
+
     return results
```

### Comparing `featureform-1.7.4/src/featureform/serving.py` & `featureform-1.8.0/src/featureform/serving.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .sqlite_metadata import SQLiteMetadata
 from featureform.proto import serving_pb2_grpc
 
 from .resources import Model, SourceType, ComputationMode
 from .tls import insecure_channel, secure_channel
 from .version import check_up_to_date
 from .enums import FileFormat
+from .constants import NO_RECORD_LIMIT
 
 
 def check_feature_type(features):
     checked_features = []
     for feature in features:
         if isinstance(feature, tuple):
             checked_features.append(feature)
@@ -186,19 +187,34 @@
                 func = types.FunctionType(code, globals(), "transformation")
                 parsed_value = func(self, params, entities)
 
             feature_values.append(parsed_value)
 
         return feature_values
 
-    def get_source_as_df(self, name, variant):
-        warnings.warn(
-            "Computing dataframes on sources in hosted mode is not yet supported."
-        )
-        return pd.DataFrame()
+    def _get_source_as_df(self, name, variant, limit):
+        columns = self._get_source_columns(name, variant)
+        data = self._get_source_data(name, variant, limit)
+        return pd.DataFrame(data=data, columns=columns)
+
+    def _get_source_data(self, name, variant, limit):
+        id = serving_pb2.SourceID(name=name, version=variant)
+        req = serving_pb2.SourceDataRequest(id=id, limit=limit)
+        resp = self._stub.SourceData(req)
+        data = []
+        for rows in resp:
+            row = [getattr(r, r.WhichOneof("value")) for r in rows.rows]
+            data.append(row)
+        return data
+
+    def _get_source_columns(self, name, variant):
+        id = serving_pb2.SourceID(name=name, version=variant)
+        req = serving_pb2.SourceDataRequest(id=id)
+        resp = self._stub.SourceColumns(req)
+        return resp.columns
 
 
 class LocalClientImpl:
     def __init__(self):
         self.db = SQLiteMetadata()
         self.local_cache = LocalCache(self.db)
         check_up_to_date(True, "serving")
@@ -649,16 +665,22 @@
     ):
         name = model if isinstance(model, str) else model.name
         type = "Model" if isinstance(model, str) else model.type()
 
         self.db.insert("models", name, type)
         self.db.insert(look_up_table, name, association_name, association_variant)
 
-    def get_source_as_df(self, name, variant):
-        return self.get_input_df(name, variant)
+    def _get_source_as_df(self, name, variant, limit):
+        if limit == 0:
+            raise ValueError("limit must be greater than 0")
+        df = self.get_input_df(name, variant)
+        if limit != NO_RECORD_LIMIT:
+            return df[:limit]
+        else:
+            return df
 
 
 class Stream:
     def __init__(self, stub, name, version, model: Union[str, Model] = None):
         req = serving_pb2.TrainingDataRequest()
         req.id.name = name
         req.id.version = version
```

### Comparing `featureform-1.7.4/src/featureform/sqlite_metadata.py` & `featureform-1.8.0/src/featureform/sqlite_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,26 @@
     def commit(self):
         with self.__lock:
             return self.__conn.commit()
 
 
 class SQLiteMetadata:
     def __init__(self):
-        self.path = '.featureform/SQLiteDB'
+        self.path = ".featureform/SQLiteDB"
         if not os.path.exists(self.path):
             os.makedirs(self.path)
-        raw_conn = sqlite3.connect(self.path + '/metadata.db', check_same_thread=False)
+        raw_conn = sqlite3.connect(self.path + "/metadata.db", check_same_thread=False)
         raw_conn.row_factory = sqlite3.Row
         self.__conn = SyncSQLExecutor(raw_conn)
         self.createTables()
 
     def createTables(self):
         # Features variant table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS feature_variant(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS feature_variant(
           created text,
           description text,
           entity text NOT NULL,
           name text NOT NULL,
           owner text,
           provider text NOT NULL,
           data_type text NOT NULL,
@@ -59,108 +60,128 @@
           source_variant text NOT NULL,
 
           PRIMARY KEY(name, variant),
 
           FOREIGN KEY(name) REFERENCES features(name),
           FOREIGN KEY(entity) REFERENCES entities(name),
           FOREIGN KEY(provider) REFERENCES providers(name),
-          FOREIGN KEY(source_name) REFERENCES sources(name))''')
-      
+          FOREIGN KEY(source_name) REFERENCES sources(name))"""
+        )
+
         # OnDemand Features variant table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS ondemand_feature_variant(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS ondemand_feature_variant(
           created text,
           description text,
           name text NOT NULL,
           owner text,
           variant text NOT NULL,
           status text,
           query text,
 
           PRIMARY KEY(name, variant),
 
-          FOREIGN KEY(name) REFERENCES features(name))''')
+          FOREIGN KEY(name) REFERENCES features(name))"""
+        )
 
         # Features table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS features(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS features(
           name text NOT NULL,
           default_variant text NOT NULL,
           type text,
-          PRIMARY KEY (name));''')
+          PRIMARY KEY (name));"""
+        )
 
         # features type table
         # this is used to determine if it is a pre-calculated or client-calculated feature
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS feature_computation_mode (
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS feature_computation_mode (
           name text NOT NULL,
           variant text NOT NULL,
           mode text,
           is_on_demand integer,
-          PRIMARY KEY (name, variant));''')
+          PRIMARY KEY (name, variant));"""
+        )
 
         # training set variant
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS training_set_variant(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS training_set_variant(
           created text,
           description text,            
           name text NOT NULL,
           owner text,
           variant text,
           label_name text,
           label_variant text,
           status text,
           PRIMARY KEY(name, variant),
-          FOREIGN KEY(name) REFERENCES training_sets(name));''')
+          FOREIGN KEY(name) REFERENCES training_sets(name));"""
+        )
 
         # Training-set table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS training_sets(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS training_sets(
           type text NOT NULL,
           default_variant text,
-          name text PRIMARY KEY NOT NULL);''')
+          name text PRIMARY KEY NOT NULL);"""
+        )
 
         # Training set features
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS training_set_features(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS training_set_features(
           training_set_name text NOT NULL,
           training_set_variant text NOT NULL,
           feature_name text NOT NULL,
           feature_variant text NOT NULL,
-          UNIQUE(training_set_name, training_set_variant, feature_name, feature_variant));''')
+          UNIQUE(training_set_name, training_set_variant, feature_name, feature_variant));"""
+        )
 
         # Training set lag features
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS training_set_lag_features(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS training_set_lag_features(
           training_set_name text NOT NULL,
           training_set_variant text NOT NULL,
           feature_name text NOT NULL,
           feature_variant text NOT NULL,
           feature_new_name text,
           feature_lag real,
-          UNIQUE(training_set_name, training_set_variant, feature_name, feature_variant, feature_new_name, feature_lag));''')
+          UNIQUE(training_set_name, training_set_variant, feature_name, feature_variant, feature_new_name, feature_lag));"""
+        )
 
         # source variant
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS source_variant(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS source_variant(
           created     text,
           description text,
           name  text NOT NULL,
           source_type  text,
           owner       text,
           provider    text NOT NULL,
           variant    text,
           status      text,
           transformation text,
           inputs text, 
           definition  BLOB,
           PRIMARY KEY(name, variant),
           FOREIGN KEY(provider) REFERENCES providers(name),
-          FOREIGN KEY(name) REFERENCES sources(name));''')
+          FOREIGN KEY(name) REFERENCES sources(name));"""
+        )
 
         # sources table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS sources(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS sources(
           type           text NOT NULL,
           default_variant text,
-          name           text PRIMARY KEY NOT NULL);''')
+          name           text PRIMARY KEY NOT NULL);"""
+        )
 
         # labels variant
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS label_variant(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS label_variant(
           created         text,
           description     text,
           entity          text,
           name            text NOT NULL,
           owner           text,
           provider        text,
           data_type       text,
@@ -169,376 +190,473 @@
           source_timestamp text,
           source_value     text,
           status          text,
           source_name      text,
           source_variant   text,
           FOREIGN KEY(provider) REFERENCES providers(name),
           PRIMARY KEY(name, variant),
-          FOREIGN KEY(name) REFERENCES labels(name));''')
+          FOREIGN KEY(name) REFERENCES labels(name));"""
+        )
 
         # labels table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS labels(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS labels(
           type           text,
           default_variant text,
-          name           text PRIMARY KEY);''')
+          name           text PRIMARY KEY);"""
+        )
 
         # entity table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS entities(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS entities(
           name        text PRIMARY KEY NOT NULL,
           type        text,
           description text,
-          status      text);''')
+          status      text);"""
+        )
 
         # user table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS users(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS users(
           name   text PRIMARY KEY NOT NULL,
           type   text,
-          status text);''')
+          status text);"""
+        )
 
         # models table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS models(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS models(
           name        text PRIMARY KEY NOT NULL,
-          type        text);''')
+          type        text);"""
+        )
 
         # models training sets table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS model_training_sets(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS model_training_sets(
           model_name           text NOT NULL,
           training_set_name    text NOT NULL,
           training_set_variant text NOT NULL,
-          UNIQUE(model_name, training_set_name, training_set_variant));''')
+          UNIQUE(model_name, training_set_name, training_set_variant));"""
+        )
 
         # models features sets table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS model_features(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS model_features(
           model_name           text NOT NULL,
           feature_name    text NOT NULL,
           feature_variant text NOT NULL,
-          UNIQUE(model_name, feature_name, feature_variant));''')
+          UNIQUE(model_name, feature_name, feature_variant));"""
+        )
 
         # providers table
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS providers(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS providers(
           name             text PRIMARY KEY NOT NULL,
           type             text,
           description      text,
           provider_type     text,
           software         text,
           team             text,
           sources          text,
           status           text,
-          serialized_config text)''')
+          serialized_config text)"""
+        )
 
         # source files for a resource
         # tracks the source files that have been used to create a resource and contains the files last_updated
         # this is used to determined if caches need to be invalidated
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS resource_source_files(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS resource_source_files(
             resource_type text NOT NULL,
             name text NOT NULL,
             variant text NOT NULL,
             file_path text NOT NULL,
             updated_at text NOT NULL,
-            PRIMARY KEY(resource_type, name, variant, file_path))''')
+            PRIMARY KEY(resource_type, name, variant, file_path))"""
+        )
 
         # full-text search table
-        self.__conn.execute('''CREATE VIRTUAL TABLE IF NOT EXISTS resources_fts USING fts5(
+        self.__conn.execute(
+            """CREATE VIRTUAL TABLE IF NOT EXISTS resources_fts USING fts5(
           resource_type, -- an "enum" column to filter with (e.g. feature, training_set, source, provider, entity, label, model, user)
           name,
           variant,
           description,
           status,
-        );''')
+        );"""
+        )
 
         # resource table triggers to populate fts table
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS feature_variant_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS feature_variant_after_insert
         AFTER INSERT ON feature_variant
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('feature', new.name, new.variant, new.description, new.status);
-        END;''')
+        END;"""
+        )
 
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS training_set_variant_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS training_set_variant_after_insert
         AFTER INSERT ON training_set_variant
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('training_set', new.name, new.variant, new.description, new.status);
-        END;''')
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS source_variant_after_insert
+        END;"""
+        )
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS source_variant_after_insert
         AFTER INSERT ON source_variant
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('source', new.name, new.variant, new.description, new.status);
-        END;''')
+        END;"""
+        )
 
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS label_variant_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS label_variant_after_insert
         AFTER INSERT ON label_variant
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('label', new.name, new.variant, new.description, new.status);
-        END;''')
+        END;"""
+        )
 
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS entities_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS entities_after_insert
         AFTER INSERT ON entities
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('entity', new.name, '', new.description, new.status);
-        END;''')
+        END;"""
+        )
 
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS users_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS users_after_insert
         AFTER INSERT ON users
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('user', new.name, '', '', new.status);
-        END;''')
+        END;"""
+        )
 
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS models_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS models_after_insert
         AFTER INSERT ON models
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('model', new.name, '', '', '');
-        END;''')
+        END;"""
+        )
 
-        self.__conn.execute('''CREATE TRIGGER IF NOT EXISTS provider_after_insert
+        self.__conn.execute(
+            """CREATE TRIGGER IF NOT EXISTS provider_after_insert
         AFTER INSERT ON providers
         BEGIN
         INSERT INTO resources_fts(resource_type, name, variant, description, status)
         VALUES ('provider', new.name, '', new.description, new.status);
-        END;''')
+        END;"""
+        )
 
         # Tags and Properties tables
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS tags(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS tags(
           name text NOT NULL,
           variant text,
           type text,
           tag_list text,
-          UNIQUE(name,variant,type));''')
+          UNIQUE(name,variant,type));"""
+        )
 
-        self.__conn.execute('''CREATE TABLE IF NOT EXISTS properties(
+        self.__conn.execute(
+            """CREATE TABLE IF NOT EXISTS properties(
           name text NOT NULL,
           variant text,
           type text,
           property_list text,
-          UNIQUE(name,variant,type));''')
+          UNIQUE(name,variant,type));"""
+        )
 
         self.__conn.commit()
 
     def get_type_table(self, tablename):
         if tablename in ["entities", "models", "users", "providers"]:
-          query = '''SELECT r.*, t.tag_list as tags, p.property_list as properties
+            query = """SELECT r.*, t.tag_list as tags, p.property_list as properties
           FROM {0} r
           LEFT JOIN tags t ON t.name = r.name
           LEFT JOIN properties p ON p.name = r.name     ;
-          '''.format(tablename)
+          """.format(
+                tablename
+            )
         else:
-          query = f"SELECT * FROM {tablename}"
+            query = f"SELECT * FROM {tablename}"
         type_data = self.__conn.execute(query)
         self.__conn.commit()
         return type_data.fetchall()
 
-    def query_resource(self, table, column, resource_name, should_fetch_tags_properties=False):
+    def query_resource(
+        self, table, column, resource_name, should_fetch_tags_properties=False
+    ):
         if should_fetch_tags_properties:
-           query = '''SELECT r.*, t.tag_list as tags, p.property_list as properties
+            query = """SELECT r.*, t.tag_list as tags, p.property_list as properties
            FROM {0} r
            LEFT JOIN tags t ON t.name = r.name
            LEFT JOIN properties p ON p.name = r.name
-           WHERE r.{1} = '{2}';'''.format(table, column, resource_name)
+           WHERE r.{1} = '{2}';""".format(
+                table, column, resource_name
+            )
         else:
-          query = f"SELECT * FROM {table} WHERE {column}='{resource_name}';"
+            query = f"SELECT * FROM {table} WHERE {column}='{resource_name}';"
         resource_data = self.__conn.execute(query)
         self.__conn.commit()
         resource_data_list = resource_data.fetchall()
         if len(resource_data_list) == 0 and column != "owner":
-          raise ValueError(f"{table} with {column}: {resource_name} not found")
+            raise ValueError(f"{table} with {column}: {resource_name} not found")
         return resource_data_list
 
     def query_resource_variant(self, table, column, resource_name):
-        query = '''SELECT r.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT r.*, t.tag_list as tags, p.property_list as properties
            FROM {0} r
            LEFT JOIN tags t ON t.name = r.name AND t.variant = r.variant
            LEFT JOIN properties p ON p.name = r.name AND p.variant = r.variant
-           WHERE r.{1} = '{2}';'''.format(table, column, resource_name)
+           WHERE r.{1} = '{2}';""".format(
+            table, column, resource_name
+        )
         variant_data = self.__conn.execute(query)
         self.__conn.commit()
         variant_data_list = variant_data.fetchall()
         if len(variant_data_list) == 0 and column != "owner":
-          raise ValueError(f"{table} with {column}: {resource_name} not found")
+            raise ValueError(f"{table} with {column}: {resource_name} not found")
         return variant_data_list
 
     def fetch_data(self, query, type, name, variant):
         variant_data = self.__conn.execute(query)
         self.__conn.commit()
         variant_data_list = variant_data.fetchall()
         if len(variant_data_list) == 0:
-          raise ValueError(f"{type} with name: {name} and variant: {variant} not found")
+            raise ValueError(
+                f"{type} with name: {name} and variant: {variant} not found"
+            )
         return variant_data_list
 
     def fetch_data_safe(self, query, type, name, variant):
         variant_data = self.__conn.execute(query)
         self.__conn.commit()
         variant_data_list = variant_data.fetchall()
         if len(variant_data_list) == 0:
-          return []
+            return []
         return variant_data_list
 
     def get_user(self, name, should_fetch_tags_properties):
-      return self.query_resource("users", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource("users", "name", name, should_fetch_tags_properties)[
+            0
+        ]
 
     def get_entity(self, name, should_fetch_tags_properties):
-      return self.query_resource("entities", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "entities", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_feature(self, name, should_fetch_tags_properties):
-      return self.query_resource("features", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "features", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_label(self, name, should_fetch_tags_properties):
-      return self.query_resource("labels", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "labels", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_source(self, name, should_fetch_tags_properties):
-      return self.query_resource("sources", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "sources", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_training_set(self, name, should_fetch_tags_properties):
-      return self.query_resource("training_sets", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "training_sets", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_model(self, name, should_fetch_tags_properties):
-      return self.query_resource("models", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "models", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_provider(self, name, should_fetch_tags_properties):
-      return self.query_resource("providers", "name", name, should_fetch_tags_properties)[0]
+        return self.query_resource(
+            "providers", "name", name, should_fetch_tags_properties
+        )[0]
 
     def get_feature_variant(self, name, variant):
-        query = '''SELECT fv.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT fv.*, t.tag_list as tags, p.property_list as properties
         FROM feature_variant fv
         LEFT JOIN tags t ON t.name = fv.name AND t.variant = fv.variant
         LEFT JOIN properties p ON p.name = fv.name AND p.variant = fv.variant
-        WHERE fv.name = '{0}' AND fv.variant = '{1}';'''.format(name, variant)
+        WHERE fv.name = '{0}' AND fv.variant = '{1}';""".format(
+            name, variant
+        )
         return self.fetch_data(query, "feature_variant", name, variant)[0]
 
     def get_feature_variants_from_provider(self, name):
         return self.query_resource_variant("feature_variant", "provider", name)
 
     def get_feature_variants_from_source(self, name, variant):
-        query = '''SELECT fv.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT fv.*, t.tag_list as tags, p.property_list as properties
         FROM feature_variant fv
         LEFT JOIN tags t ON t.name = fv.name AND t.variant = fv.variant
         LEFT JOIN properties p ON p.name = fv.name AND p.variant = fv.variant
-        WHERE fv.source_name = '{0}' AND fv.source_variant = '{1}';'''.format(name, variant)
+        WHERE fv.source_name = '{0}' AND fv.source_variant = '{1}';""".format(
+            name, variant
+        )
         return self.fetch_data_safe(query, "feature_variant", name, variant)
 
     def get_feature_variants_from_feature(self, name):
-      return self.query_resource_variant("feature_variant", "name", name)
-    
+        return self.query_resource_variant("feature_variant", "name", name)
+
     def get_feature_variant_mode(self, name, variant):
-      query = f"SELECT mode FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
-      return self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0]["mode"]
-    
+        query = f"SELECT mode FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
+        return self.fetch_data_safe(query, "feature_computation_mode", name, variant)[
+            0
+        ]["mode"]
+
     def get_feature_variant_on_demand(self, name, variant):
-      query = f"SELECT is_on_demand FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
-      return bool(self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0]["is_on_demand"])
+        query = f"SELECT is_on_demand FROM feature_computation_mode WHERE name='{name}' AND variant='{variant}'"
+        return bool(
+            self.fetch_data_safe(query, "feature_computation_mode", name, variant)[0][
+                "is_on_demand"
+            ]
+        )
 
     def get_ondemand_feature_query(self, name, variant):
-      query = f"SELECT query FROM ondemand_feature_variant WHERE name='{name}' AND variant='{variant}'"
-      return self.fetch_data_safe(query, "ondemand_feature_variant", name, variant)[0]["query"]
+        query = f"SELECT query FROM ondemand_feature_variant WHERE name='{name}' AND variant='{variant}'"
+        return self.fetch_data_safe(query, "ondemand_feature_variant", name, variant)[
+            0
+        ]["query"]
 
     def get_training_set_variant(self, name, variant):
         query = f"SELECT * FROM training_set_variant WHERE name = '{name}' AND variant = '{variant}';"
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
         WHERE v.name = '{0}' AND v.variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data(query, "training_set_variant", name, variant)[0]
 
     def get_training_set_variant_from_training_set(self, name):
         return self.query_resource_variant("training_set_variant", "name", name)
-    
+
     def get_training_set_variant_from_label(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
         WHERE v.label_name = '{0}' AND v.label_variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data_safe(query, "training_set_variant", name, variant)
-    
+
     def get_label_variant(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM label_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
         WHERE v.name = '{0}' AND v.variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data(query, "label_variant", name, variant)[0]
-    
+
     def get_label_variants_from_label(self, name):
         return self.query_resource_variant("label_variant", "name", name)
 
     def get_label_variants_from_provider(self, name):
         return self.query_resource_variant("label_variant", "provider", name)
-    
+
     def get_label_variants_from_source(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM label_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
         WHERE v.source_name = '{0}' AND v.source_variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data_safe(query, "label_variant", name, variant)
 
     def get_source_variant(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM source_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
         WHERE v.name = '{0}' AND v.variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data(query, "source_variant", name, variant)[0]
 
     def get_source_variants_from_source(self, name):
         return self.query_resource_variant("source_variant", "name", name)
 
     def get_training_set_from_features(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_features v
         LEFT JOIN tags t ON t.name = v.training_set_name AND t.variant = v.training_set_variant
         LEFT JOIN properties p ON p.name = v.training_set_name AND p.variant = v.training_set_variant
         WHERE v.feature_name = '{0}' AND v.feature_variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data_safe(query, "training_set_features", name, variant)
 
     def get_training_set_from_labels(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_variant v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
         WHERE v.label_name = '{0}' AND v.label_variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data_safe(query, "training_set_variant", name, variant)
 
     def get_training_set_features(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_features v
         LEFT JOIN tags t ON t.name = v.training_set_name AND t.variant = v.training_set_variant
         LEFT JOIN properties p ON p.name = v.training_set_name AND p.variant = v.training_set_variant
          WHERE v.training_set_name = '{0}' AND v.training_set_variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data(query, "training_set_features", name, variant)
-      
+
     def get_training_set_lag_features(self, name, variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM training_set_lag_features v
         LEFT JOIN tags t ON t.name = v.training_set_name AND t.variant = v.training_set_variant
         LEFT JOIN properties p ON p.name = v.training_set_name AND p.variant = v.training_set_variant
          WHERE v.training_set_name = '{0}' AND v.training_set_variant = '{1}';
-        '''.format(name, variant)
+        """.format(
+            name, variant
+        )
         return self.fetch_data_safe(query, "training_set_lag_features", name, variant)
 
     def get_resource_with_source(self, tablename, source_name, source_variant):
-        query = '''SELECT v.*, t.tag_list as tags, p.property_list as properties
+        query = """SELECT v.*, t.tag_list as tags, p.property_list as properties
         FROM {0} v
         LEFT JOIN tags t ON t.name = v.name AND t.variant = v.variant
         LEFT JOIN properties p ON p.name = v.name AND p.variant = v.variant
          WHERE v.source_name = '{1}' AND v.source_variant = '{2}';
-        '''.format(tablename, source_name, source_variant)
+        """.format(
+            tablename, source_name, source_variant
+        )
         return self.fetch_data(query, tablename, source_name, source_variant)
 
     def is_transformation(self, name, variant):
         query = f"SELECT transformation FROM source_variant WHERE name='{name}' and variant='{variant}';"
         transformation = self.__conn.execute(query)
         self.__conn.commit()
         t = transformation.fetchall()
@@ -580,32 +698,32 @@
         )
         self.__conn.execute(query)
         self.__conn.commit()
 
     # TODO get something generic working, possibly consider using the above insert or update
     def upsert(self, tablename, *args):
         if tablename == "tags" or tablename == "properties":
-           query, is_update = self.upsert_tags_properties(tablename, *args)
+            query, is_update = self.upsert_tags_properties(tablename, *args)
         else:
-           raise NotImplementedError(f"UPSERT not implemented for table {tablename}")
+            raise NotImplementedError(f"UPSERT not implemented for table {tablename}")
 
         if is_update:
-          self.__conn.execute(query)
-          self.__conn.commit()
+            self.__conn.execute(query)
+            self.__conn.commit()
         else:
-           self.insert(tablename, *args)
+            self.insert(tablename, *args)
 
     def close(self):
         self.__conn.close()
 
     def search(self, phrase, resource_type=None):
         if resource_type is None:
-          query = f"SELECT * FROM resources_fts WHERE resources_fts match '{{name variant description status}} : {phrase}*';"
+            query = f"SELECT * FROM resources_fts WHERE resources_fts match '{{name variant description status}} : {phrase}*';"
         else:
-          query = f"SELECT * FROM resources_fts WHERE resources_fts match '{{name variant description status}} : {phrase}*' AND resource_type = '{resource_type}';"
+            query = f"SELECT * FROM resources_fts WHERE resources_fts match '{{name variant description status}} : {phrase}*' AND resource_type = '{resource_type}';"
 
         search_results = self.__conn.execute(query)
         self.__conn.commit()
         results_list = search_results.fetchall()
 
         return results_list
 
@@ -616,24 +734,34 @@
         query = ""
         updatable_column = "tag_list" if tablename == "tags" else "property_list"
         default_value = [] if tablename == "tags" else {}
         is_update = False
         name = args[0]
         variant = args[1]
 
-        cursor = self.__conn.execute(f"SELECT * FROM {tablename} WHERE name = '{name}' AND variant = '{variant}';")
+        cursor = self.__conn.execute(
+            f"SELECT * FROM {tablename} WHERE name = '{name}' AND variant = '{variant}';"
+        )
         self.__conn.commit()
         existing = cursor.fetchall()
 
         if len(existing):
-          existing_val = json.loads(existing[result_idx][updatable_column]) if existing[result_idx][updatable_column] is not None else default_value
-          if tablename == "tags":
-            updated = json.dumps(list(set(existing_val + json.loads(args[updatable_column_idx]))))
-          else:
-             updated = json.dumps({**existing_val, **json.loads(args[updatable_column_idx])})
-          args = list(args)
-          args[updatable_column_idx] = updated
-          query = f"UPDATE {tablename} SET name = '{name}', variant = '{variant}', type = '{args[type_idx]}', {updatable_column} = '{args[updatable_column_idx]}'"
-          query += f"WHERE name = '{name}' AND variant = '{variant}';"
-          is_update = True
+            existing_val = (
+                json.loads(existing[result_idx][updatable_column])
+                if existing[result_idx][updatable_column] is not None
+                else default_value
+            )
+            if tablename == "tags":
+                updated = json.dumps(
+                    list(set(existing_val + json.loads(args[updatable_column_idx])))
+                )
+            else:
+                updated = json.dumps(
+                    {**existing_val, **json.loads(args[updatable_column_idx])}
+                )
+            args = list(args)
+            args[updatable_column_idx] = updated
+            query = f"UPDATE {tablename} SET name = '{name}', variant = '{variant}', type = '{args[type_idx]}', {updatable_column} = '{args[updatable_column_idx]}'"
+            query += f"WHERE name = '{name}' AND variant = '{variant}';"
+            is_update = True
 
         return (query, is_update)
```

### Comparing `featureform-1.7.4/src/featureform/type_objects.py` & `featureform-1.8.0/src/featureform/type_objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,376 +1,377 @@
 from ssl import create_default_context
 import json
 
+
 class FeatureVariantResource:
-    def __init__(self, 
-        created=None, 
-        description="", 
-        entity="", 
-        name="", 
+    def __init__(
+        self,
+        created=None,
+        description="",
+        entity="",
+        name="",
         owner="",
         provider="",
-        dataType="", 
+        dataType="",
         variant="",
         status="",
         location=None,
         source=None,
         tags=[],
-        properties={}):
-
-          self.__dictionary = {
+        properties={},
+    ):
+        self.__dictionary = {
             "created": created,
             "description": description,
             "entity": entity,
             "name": name,
             "owner": owner,
             "provider": provider,
             "data-type": dataType,
             "variant": variant,
             "status": status,
-            "location":location,
-            "source":source,
+            "location": location,
+            "source": source,
             "tags": tags,
             "properties": properties,
             # Training Set[] is missing
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
 
 class FeatureResource:
-    def __init__(self, 
-        name="",
-        defaultVariant="",
-        type = "",
-        variants=None,
-        allVariants=[]):
-
-          self.__dictionary = {
+    def __init__(
+        self, name="", defaultVariant="", type="", variants=None, allVariants=[]
+    ):
+        self.__dictionary = {
             "all-variants": allVariants,
-            "type" : type,
-            "default-variant" : defaultVariant,
-            "name" : name,
-            "variants" : variants
+            "type": type,
+            "default-variant": defaultVariant,
+            "name": name,
+            "variants": variants,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class TrainingSetVariantResource:
-    def __init__(self, 
-        created=None, 
-        description="", 
-        name="", 
-        owner="", 
+    def __init__(
+        self,
+        created=None,
+        description="",
+        name="",
+        owner="",
         variant="",
         label=None,
         status="",
         features=None,
         tags=[],
-        properties={}):
-
-          self.__dictionary = {
-            "created" : created,
-            "description" : description,
-            "name" : name,
-            "owner" : owner,
-            "variant" : variant,
-            "status" : status,
-            "label" : label,
-            "features" : features,
+        properties={},
+    ):
+        self.__dictionary = {
+            "created": created,
+            "description": description,
+            "name": name,
+            "owner": owner,
+            "variant": variant,
+            "status": status,
+            "label": label,
+            "features": features,
             "tags": tags,
             "properties": properties,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
-class TrainingSetResource:
-    def __init__(self,
-        type = "",
-        defaultVariant="",
-        name="",
-        variants=None,
-        allVariants=[]):
 
+class TrainingSetResource:
+    def __init__(
+        self, type="", defaultVariant="", name="", variants=None, allVariants=[]
+    ):
         self.__dictionary = {
-          "all-variants":allVariants,
-          "type":type,
-          "default-variant":defaultVariant,
-          "name":name,
-          "variants":variants
+            "all-variants": allVariants,
+            "type": type,
+            "default-variant": defaultVariant,
+            "name": name,
+            "variants": variants,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class SourceVariantResource:
-    def __init__(self, 
-        created=None, 
+    def __init__(
+        self,
+        created=None,
         description="",
         name="",
-        sourceType = "",
-        owner="", 
-        provider="", 
+        sourceType="",
+        owner="",
+        provider="",
         variant="",
         status="",
         definition="",
         labels=None,
         features=None,
         trainingSets=None,
         tags=[],
-        properties={}):
-
+        properties={},
+    ):
         self.__dictionary = {
-          "created":created,
-          "description":description,
-          "name":name,
-          "source-type":sourceType,
-          "owner":owner,
-          "provider":provider,
-          "variant":variant,
-         "status":status,
-         "definition":definition,
-         "labels":labels,
-         "features":features,
-         "training-sets":trainingSets,
-         "tags": tags,
-         "properties": properties,
+            "created": created,
+            "description": description,
+            "name": name,
+            "source-type": sourceType,
+            "owner": owner,
+            "provider": provider,
+            "variant": variant,
+            "status": status,
+            "definition": definition,
+            "labels": labels,
+            "features": features,
+            "training-sets": trainingSets,
+            "tags": tags,
+            "properties": properties,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
-class SourceResource:
-    def __init__(self, 
-        type = "",
-        defaultVariant="",
-        name="",
-        variants=None,
-        allVariants=[]):
 
+class SourceResource:
+    def __init__(
+        self, type="", defaultVariant="", name="", variants=None, allVariants=[]
+    ):
         self.__dictionary = {
-         "all-variants":allVariants,
-         "type":type,
-         "default-variant":defaultVariant,
-         "name":name,
-         "variants":variants
+            "all-variants": allVariants,
+            "type": type,
+            "default-variant": defaultVariant,
+            "name": name,
+            "variants": variants,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class LabelVariantResource:
-    def __init__(self, 
-        created=None, 
+    def __init__(
+        self,
+        created=None,
         description="",
         entity="",
         name="",
-        owner="", 
+        owner="",
         provider="",
-        dataType = "", 
+        dataType="",
         variant="",
         location=None,
         status="",
         source=None,
         trainingSets=None,
         tags=[],
-        properties={}):
-
-
+        properties={},
+    ):
         self.__dictionary = {
-         "created":created,
-         "description":description,
-         "entity":entity,
-         "data-type":dataType,
-         "name":name,
-         "owner":owner,
-         "provider":provider,
-         "variant":variant,
-         "status":status,
-         "location":location,
-         "source":source,
-         "trainingSets":trainingSets,
-         "tags": tags,
-         "properties": properties,
-        #  source is missing
+            "created": created,
+            "description": description,
+            "entity": entity,
+            "data-type": dataType,
+            "name": name,
+            "owner": owner,
+            "provider": provider,
+            "variant": variant,
+            "status": status,
+            "location": location,
+            "source": source,
+            "trainingSets": trainingSets,
+            "tags": tags,
+            "properties": properties,
+            #  source is missing
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
-class LabelResource:
-    def __init__(self, 
-        type = "",
-        defaultVariant="",
-        name="",
-        variants=None,
-        allVariants=[]):
 
+class LabelResource:
+    def __init__(
+        self, type="", defaultVariant="", name="", variants=None, allVariants=[]
+    ):
         self.__dictionary = {
-         "all-variants":allVariants,
-         "type":type,
-         "default-variant":defaultVariant,
-         "name":name,
-         "variants":variants
+            "all-variants": allVariants,
+            "type": type,
+            "default-variant": defaultVariant,
+            "name": name,
+            "variants": variants,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class EntityResource:
-    def __init__(self,
-        name="", 
+    def __init__(
+        self,
+        name="",
         type="",
         description="",
         status="",
         features=None,
         labels=None,
         trainingSets=None,
         tags=[],
-        properties={}):
-
+        properties={},
+    ):
         self.__dictionary = {
-         "description":description,
-         "type":type,
-         "name":name,
-         "features":features,
-         "labels":labels,
-         "training-sets":trainingSets,
-         "status":status,
-         "tags": tags,
-         "properties": properties,
+            "description": description,
+            "type": type,
+            "name": name,
+            "features": features,
+            "labels": labels,
+            "training-sets": trainingSets,
+            "status": status,
+            "tags": tags,
+            "properties": properties,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class UserResource:
-    def __init__(self, 
+    def __init__(
+        self,
         name="",
         type="",
         status="",
         features=None,
         labels=None,
         trainingSets=None,
         sources=None,
         tags=[],
-        properties={}):
-
+        properties={},
+    ):
         self.__dictionary = {
-         "name":name,
-         "type":type,
-         "features":features,
-         "labels":labels,
-         "training-sets":trainingSets,
-         "sources":sources,
-         "status":status,
-         "tags": tags,
-         "properties": properties,
+            "name": name,
+            "type": type,
+            "features": features,
+            "labels": labels,
+            "training-sets": trainingSets,
+            "sources": sources,
+            "status": status,
+            "tags": tags,
+            "properties": properties,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class ModelResource:
-    def __init__(self, 
+    def __init__(
+        self,
         name="",
         type="",
         description="",
         status="",
         features=None,
         labels=None,
         trainingSets=None,
         tags=[],
-        properties={}):
-
+        properties={},
+    ):
         self.__dictionary = {
-         "name":name,
-         "type":type,
-         "description":description,
-         "features":features,
-         "labels":labels,
-         "training-sets":trainingSets,
-         "status":status,
-         "tags": tags,
-         "properties": properties,
+            "name": name,
+            "type": type,
+            "description": description,
+            "features": features,
+            "labels": labels,
+            "training-sets": trainingSets,
+            "status": status,
+            "tags": tags,
+            "properties": properties,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
 
+
 class ProviderResource:
-    def __init__(self, 
+    def __init__(
+        self,
         name="",
         type="",
         description="",
         providerType="",
         software="",
         team="",
         sources=None,
         status="",
         serializedConfig="",
         features=None,
         labels=None,
         tags=[],
         properties={}
-        #trainingSets=None
-        ):
-
-         self.__dictionary = {
-            "name" :name,
-            "type" :type,
-             "description":description,
-             "provider-type":providerType,
-             "software":software,
-             "team":team,
-             "sources":sources,
-             "features":features,
-              "labels":labels,
-              #"training-sets":trainingSets,
-              "status":status ,
+        # trainingSets=None
+    ):
+        self.__dictionary = {
+            "name": name,
+            "type": type,
+            "description": description,
+            "provider-type": providerType,
+            "software": software,
+            "team": team,
+            "sources": sources,
+            "features": features,
+            "labels": labels,
+            # "training-sets":trainingSets,
+            "status": status,
             #   Seems like we dont need serialised config
-              "serializedConfig":serializedConfig,
-              "tags": tags,
-              "properties": properties,
+            "serializedConfig": serializedConfig,
+            "tags": tags,
+            "properties": properties,
         }
 
     def toDictionary(self):
         return self.__dictionary
 
     def toJsonLiteral(self):
         return json.dumps(self.__dictionary)
```

### Comparing `featureform-1.7.4/src/featureform/version.py` & `featureform-1.8.0/src/featureform/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,17 +4,24 @@
 
 version_check_url = "https://version.featureform.com"
 
 
 def get_package_version():
     return pkg_resources.get_distribution("featureform").version
 
+
 def check_up_to_date(local, client):
-    download_thread = threading.Thread(target=run_version_check, name="Downloader", args=(local, client))
+    download_thread = threading.Thread(
+        target=run_version_check, name="Downloader", args=(local, client)
+    )
     download_thread.start()
 
+
 def run_version_check(local, client):
     try:
         version = get_package_version()
-        requests.get(version_check_url, params={"local": local, "client": client, "version": version})
+        requests.get(
+            version_check_url,
+            params={"local": local, "client": client, "version": version},
+        )
     except:
-        pass
+        pass
```

### Comparing `featureform-1.7.4/src/featureform.egg-info/PKG-INFO` & `featureform-1.8.0/src/featureform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featureform
-Version: 1.7.4
+Version: 1.8.0
 Summary: Package for the Featureform Feature Store
 Home-page: https://featureform.com
 Author: FeatureForm, Inc.
 Author-email: hello@featureform.com
 Project-URL: Bug Tracker, https://github.com/featureform/embeddinghub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `featureform-1.7.4/src/featureform.egg-info/SOURCES.txt` & `featureform-1.8.0/src/featureform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/featureform/__init__.py
 src/featureform/__main__.py
 src/featureform/cli.py
 src/featureform/client.py
+src/featureform/constants.py
 src/featureform/dashboard_metadata.py
 src/featureform/enums.py
 src/featureform/exceptions.py
 src/featureform/format.py
 src/featureform/get.py
 src/featureform/get_local.py
 src/featureform/get_test.py
@@ -42,18 +43,18 @@
 src/featureform/dashboard/out/[type].html
 src/featureform/dashboard/out/connections.html
 src/featureform/dashboard/out/index.html
 src/featureform/dashboard/out/robots.txt
 src/featureform/dashboard/out/search.html
 src/featureform/dashboard/out/site.webmanifest
 src/featureform/dashboard/out/[type]/[entity].html
-src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_buildManifest.js
-src/featureform/dashboard/out/_next/static/8yA-hIcHsUSF2wPeJxwZa/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_buildManifest.js
 src/featureform/dashboard/out/_next/static/Jopdpwd8wB7tMgkcaVnsn/_ssgManifest.js
+src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_buildManifest.js
+src/featureform/dashboard/out/_next/static/XLqQwuMDcHNwRKV5unb2J/_ssgManifest.js
 src/featureform/dashboard/out/_next/static/chunks/72a30a16.5298cad0ba46633d.js
 src/featureform/dashboard/out/_next/static/chunks/7679.34cabcdac6ff42f5.js
 src/featureform/dashboard/out/_next/static/chunks/7856.43cc2293f00befb0.js
 src/featureform/dashboard/out/_next/static/chunks/ad7f724d.b238476ad0e6f6d2.js
 src/featureform/dashboard/out/_next/static/chunks/framework-3412d1150754b2fb.js
 src/featureform/dashboard/out/_next/static/chunks/main-2715d0c23f47c019.js
 src/featureform/dashboard/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
```

### Comparing `featureform-1.7.4/tests/test_class_api.py` & `featureform-1.8.0/tests/test_class_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
                     description="Whether a user's transaction is fraudulent.",
                     variant="quickstart",
                     type=ff.Bool,
                 ),
             }
         )
 
+
 @pytest.mark.local
 def test_subscriptable_transformation_decorator_method_call():
     df_transformation_decorator = DFTransformationDecorator(
         registrar=Registrar(),
         provider="test_provider",
         owner="test_owner",
         tags=[],
@@ -96,18 +97,27 @@
 
     name_variant = df_transformation_decorator.name_variant()
     column_resource = df_transformation_decorator.register_resources(
         entity="user",
         entity_column="user_id",
         owner="test_owner",
         inference_store="test_store",
-        features=[{"name": "avg_transactions", "variant": "quickstart", "column": "TransactionAmount", "type": "float32"}],
+        features=[
+            {
+                "name": "avg_transactions",
+                "variant": "quickstart",
+                "column": "TransactionAmount",
+                "type": "float32",
+            }
+        ],
     )
 
-    assert name_variant == ("test_function", "default") and isinstance(column_resource, ResourceRegistrar)
+    assert name_variant == ("test_function", "default") and isinstance(
+        column_resource, ResourceRegistrar
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local",
     [
         pytest.param("local_provider_source", True, marks=pytest.mark.local),
         pytest.param("hosted_sql_provider_and_source", False, marks=pytest.mark.hosted),
```

### Comparing `featureform-1.7.4/tests/test_cli.py` & `featureform-1.8.0/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,58 @@
 import pytest
 import sys
 from click.testing import CliRunner
 
-sys.path.insert(0, 'client/src/')
+sys.path.insert(0, "client/src/")
 from featureform.cli import apply
 
+
 class TestApply:
     def test_invalid_empty(self):
         runner = CliRunner()
         result = runner.invoke(apply)
         assert result.exit_code == 2
 
     def test_invalid_path(self):
         runner = CliRunner()
-        with pytest.raises(ValueError, match="Argument must be a path to a file or URL with a valid schema"):
+        with pytest.raises(
+            ValueError,
+            match="Argument must be a path to a file or URL with a valid schema",
+        ):
             runner.invoke(apply, ". --dry-run".split(), catch_exceptions=False)
 
     def test_invalid_url(self):
         runner = CliRunner()
-        with pytest.raises(ValueError, match="Argument must be a path to a file or URL with a valid schema"):
-            runner.invoke(apply, "www.something.com --dry-run".split(), catch_exceptions=False)
+        with pytest.raises(
+            ValueError,
+            match="Argument must be a path to a file or URL with a valid schema",
+        ):
+            runner.invoke(
+                apply, "www.something.com --dry-run".split(), catch_exceptions=False
+            )
 
     def test_valid_url(self):
         runner = CliRunner()
-        result = runner.invoke(apply, "https://featureform-demo-files.s3.amazonaws.com/quickstart.py --dry-run".split(), catch_exceptions=False)
+        result = runner.invoke(
+            apply,
+            "https://featureform-demo-files.s3.amazonaws.com/quickstart.py --dry-run".split(),
+            catch_exceptions=False,
+        )
         assert result.exit_code == 0
 
     def test_valid_file(self):
         runner = CliRunner()
-        result = runner.invoke(apply, "client/examples/quickstart.py --dry-run".split(), catch_exceptions=False)
+        result = runner.invoke(
+            apply,
+            "client/examples/quickstart.py --dry-run".split(),
+            catch_exceptions=False,
+        )
         assert result.exit_code == 0
 
     def test_multiple_values(self):
         runner = CliRunner()
-        result = runner.invoke(apply, "client/examples/quickstart.py https://featureform-demo-files.s3.amazonaws.com/quickstart.py --dry-run".split(), catch_exceptions=False)
-        assert result.exit_code == 0
+        result = runner.invoke(
+            apply,
+            "client/examples/quickstart.py https://featureform-demo-files.s3.amazonaws.com/quickstart.py --dry-run".split(),
+            catch_exceptions=False,
+        )
+        assert result.exit_code == 0
```

### Comparing `featureform-1.7.4/tests/test_executor_resources.py` & `featureform-1.8.0/tests/test_executor_resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,63 @@
-
 import pytest
 
 from featureform.resources import DatabricksCredentials, EMRCredentials
 
 
 @pytest.mark.parametrize(
-        "username,password,host,token,cluster_id",
-    [   
-        ("a", "b", "", "","c"),
-        ("", "", "a", "b","c"),
-        pytest.param("a", "b", "a","b","c", marks=pytest.mark.xfail),
-        pytest.param("", "", "", "","c", marks=pytest.mark.xfail),
-        pytest.param("a", "b", "","","", marks=pytest.mark.xfail)
-
-    ]
+    "username,password,host,token,cluster_id",
+    [
+        ("a", "b", "", "", "c"),
+        ("", "", "a", "b", "c"),
+        pytest.param("a", "b", "a", "b", "c", marks=pytest.mark.xfail),
+        pytest.param("", "", "", "", "c", marks=pytest.mark.xfail),
+        pytest.param("a", "b", "", "", "", marks=pytest.mark.xfail),
+    ],
 )
 def test_databricks_credentials(username, password, host, token, cluster_id):
-    databricks = DatabricksCredentials(username=username, password=password, host=host, token=token, cluster_id=cluster_id)
+    databricks = DatabricksCredentials(
+        username=username,
+        password=password,
+        host=host,
+        token=token,
+        cluster_id=cluster_id,
+    )
 
     expected_config = {
         "Username": username,
         "Password": password,
         "Host": host,
         "Token": token,
-        "Cluster": cluster_id
+        "Cluster": cluster_id,
     }
 
     assert databricks.type() == "databricks"
     assert databricks.config() == expected_config
 
 
 @pytest.mark.parametrize(
-        "aws_access_key_id,aws_secret_access_key,emr_cluster_id,emr_cluster_region",
-    [   
+    "aws_access_key_id,aws_secret_access_key,emr_cluster_id,emr_cluster_region",
+    [
         ("a", "b", "c", "d"),
         pytest.param("", "", "a", "b", marks=pytest.mark.xfail),
-        pytest.param("", "", "", "", marks=pytest.mark.xfail)
-    ]
+        pytest.param("", "", "", "", marks=pytest.mark.xfail),
+    ],
 )
-def test_emr_credentials(aws_access_key_id, aws_secret_access_key, emr_cluster_id, emr_cluster_region):
-    emr = EMRCredentials(aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key, emr_cluster_id=emr_cluster_id, emr_cluster_region=emr_cluster_region)
+def test_emr_credentials(
+    aws_access_key_id, aws_secret_access_key, emr_cluster_id, emr_cluster_region
+):
+    emr = EMRCredentials(
+        aws_access_key_id=aws_access_key_id,
+        aws_secret_access_key=aws_secret_access_key,
+        emr_cluster_id=emr_cluster_id,
+        emr_cluster_region=emr_cluster_region,
+    )
 
     expected_config = {
         "AWSAccessKeyId": aws_access_key_id,
         "AWSSecretKey": aws_secret_access_key,
         "ClusterName": emr_cluster_id,
-        "ClusterRegion": emr_cluster_region
+        "ClusterRegion": emr_cluster_region,
     }
 
     assert emr.type() == "emr"
     assert emr.config() == expected_config
```

### Comparing `featureform-1.7.4/tests/test_getting_model.py` & `featureform-1.8.0/tests/test_getting_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import pytest
 from featureform.register import ModelRegistrar
 from featureform.resources import Model
 import featureform as ff
 
+
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_getting_model_successfully(is_local, is_insecure):
     model_name = "model_i"
 
     resource_client = arrange_resources(model_name, is_local, is_insecure)
 
     model = resource_client.get_model(model_name, is_local)
 
-    assert isinstance(model, Model) and model.name == model_name and model.type() == "model"
+    assert (
+        isinstance(model, Model)
+        and model.name == model_name
+        and model.type() == "model"
+    )
 
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_getting_model_by_unregistered_name(is_local, is_insecure):
     model_name = "model_j"
 
     resource_client = arrange_resources(model_name, is_local, is_insecure)
 
     if is_local:
@@ -44,30 +49,33 @@
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_getting_model_no_name(is_local, is_insecure):
     model_name = "model_k"
 
     resource_client = arrange_resources(model_name, is_local, is_insecure)
 
-    with pytest.raises(TypeError, match="missing 1 required positional argument: 'name'"):
+    with pytest.raises(
+        TypeError, match="missing 1 required positional argument: 'name'"
+    ):
         resource_client.get_model(local=is_local)
 
 
 @pytest.fixture(autouse=True)
 def before_and_after_each(setup_teardown):
     setup_teardown()
     yield
     setup_teardown()
 
+
 def arrange_resources(model_name, is_local, is_insecure):
     ff.register_model(model_name)
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply(asynchronous=True)
 
     return resource_client
```

### Comparing `featureform-1.7.4/tests/test_localmode_caching.py` & `featureform-1.8.0/tests/test_localmode_caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,9 +250,7 @@
         feature = fixture.serving_client.impl.db.get_feature_variant(
             "avg_transactions", "quickstart"
         )
         feature_df = fixture.serving_client.impl.get_feature_dataframe(feature)
 
         # ensure all values are 0
         assert feature_df["avg_transactions.quickstart"].all() == 0
-
-
```

### Comparing `featureform-1.7.4/tests/test_localmode_include_label_ts.py` & `featureform-1.8.0/tests/test_localmode_include_label_ts.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,62 +5,80 @@
 
 
 def setup():
     transactions = local.register_file(
         name="transactions",
         variant="quickstart",
         description="A dataset of fraudulent transactions",
-        path="transactions.csv"
+        path="transactions.csv",
     )
 
-    @local.df_transformation(variant="quickstart",
-                                inputs=[("transactions", "quickstart")])
+    @local.df_transformation(
+        variant="quickstart", inputs=[("transactions", "quickstart")]
+    )
     def average_user_transaction(transactions):
-        """the average transaction amount for a user """
+        """the average transaction amount for a user"""
         return transactions.groupby("CustomerID")["TransactionAmount"].mean()
 
     user = ff.register_entity("user")
 
     # Register a column from our transformation as a feature
     average_user_transaction.register_resources(
         entity=user,
         entity_column="CustomerID",
         inference_store=local,
         features=[
-            {"name": "avg_transactions", "variant": "quickstart", "column": "TransactionAmount", "type": "float32"},
+            {
+                "name": "avg_transactions",
+                "variant": "quickstart",
+                "column": "TransactionAmount",
+                "type": "float32",
+            },
         ],
     )
 
     # Register label from our base Transactions table
     transactions.register_resources(
         entity=user,
         entity_column="CustomerID",
         timestamp_column="Timestamp",
         labels=[
-            {"name": "fraudulent", "variant": "quickstart", "column": "IsFraud", "type": "bool"},
+            {
+                "name": "fraudulent",
+                "variant": "quickstart",
+                "column": "IsFraud",
+                "type": "bool",
+            },
         ],
     )
 
     # Register label from our base Transactions table
     transactions.register_resources(
         entity=user,
         entity_column="CustomerID",
         labels=[
-            {"name": "fraudulent", "variant": "quickstart-no-ts", "column": "IsFraud", "type": "bool"},
+            {
+                "name": "fraudulent",
+                "variant": "quickstart-no-ts",
+                "column": "IsFraud",
+                "type": "bool",
+            },
         ],
     )
 
     ff.register_training_set(
-        "fraud_training", "quickstart",
+        "fraud_training",
+        "quickstart",
         label=("fraudulent", "quickstart"),
         features=[("avg_transactions", "quickstart")],
     )
 
     ff.register_training_set(
-        "fraud_training", "quickstart-no-ts",
+        "fraud_training",
+        "quickstart-no-ts",
         label=("fraudulent", "quickstart-no-ts"),
         features=[("avg_transactions", "quickstart")],
     )
 
     resource_client = ff.ResourceClient(local=True)
     resource_client.apply()
 
@@ -68,18 +86,23 @@
 @pytest.mark.parametrize(
     "training_set_variant, include_label_timestamp, expected_in_keys",
     [
         ("quickstart", True, True),
         ("quickstart", False, False),
         ("quickstart-no-ts", True, False),
         ("quickstart-no-ts", False, False),
-    ]
+    ],
 )
-def test_include_label_timestamp(training_set_variant, include_label_timestamp, expected_in_keys):
-
+def test_include_label_timestamp(
+    training_set_variant, include_label_timestamp, expected_in_keys
+):
     serving_client = ff.ServingClient(local=True)
-    dataset = serving_client.training_set('fraud_training', training_set_variant, include_label_timestamp=include_label_timestamp)
+    dataset = serving_client.training_set(
+        "fraud_training",
+        training_set_variant,
+        include_label_timestamp=include_label_timestamp,
+    )
     dataset_pandas = dataset.pandas()
-    
+
     result = "label_timestamp" in dataset_pandas.keys()
 
     assert result == expected_in_keys
```

### Comparing `featureform-1.7.4/tests/test_localmode_lag_features.py` & `featureform-1.8.0/tests/test_localmode_lag_features.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,198 +7,319 @@
 from featureform import local
 from featureform.serving import LocalClientImpl
 
 real_path = os.path.realpath(__file__)
 dir_path = os.path.dirname(real_path)
 SOURCE_FILE = f"{dir_path}/test_files/input_files/lag_features_testing.csv"
 
+
 def setup():
     ff.register_user("featureformer").make_default_owner()
 
     local = ff.register_local()
 
     test_source_file = local.register_file(
         name="source_file",
         variant="testing",
         description="source file",
-        path=SOURCE_FILE
+        path=SOURCE_FILE,
     )
 
-    @local.df_transformation(name=f"source_entity", 
-                            variant="testing",
-                            inputs=[(f"source_file", "testing")])
+    @local.df_transformation(
+        name=f"source_entity", variant="testing", inputs=[(f"source_file", "testing")]
+    )
     def source_entity_transformation(df):
-        """ the source dataset with entity """
+        """the source dataset with entity"""
         df["entity_1"] = "source_entity"
         return df
 
-    @local.df_transformation(name=f"source_transformation", 
-                            variant="testing",
-                            inputs=[(f"source_entity", "testing")])
+    @local.df_transformation(
+        name=f"source_transformation",
+        variant="testing",
+        inputs=[(f"source_entity", "testing")],
+    )
     def source_transformation(df):
         return df
 
     entity = ff.register_entity("entity")
 
     # Register a column from our transformation as a feature
     source_transformation.register_resources(
         entity=entity,
         entity_column="entity_1",
         timestamp_column="timestamp",
         inference_store=local,
         features=[
-            {"name": "testing_feature", "variant": "testing", "column": "value", "type": "float32"},
+            {
+                "name": "testing_feature",
+                "variant": "testing",
+                "column": "value",
+                "type": "float32",
+            },
         ],
     )
 
     # Register label from our base Transactions table
     source_entity_transformation.register_resources(
         entity=entity,
         entity_column="entity_1",
         timestamp_column="timestamp",
         labels=[
-            {"name": f"testing_label", "variant": "testing", "column": "score", "type": "float32"},
+            {
+                "name": f"testing_label",
+                "variant": "testing",
+                "column": "score",
+                "type": "float32",
+            },
         ],
     )
 
     ff.register_training_set(
-        "testing_training", "no_lag_features",
+        "testing_training",
+        "no_lag_features",
         label=(f"testing_label", "testing"),
         features=[
             (f"testing_feature", "testing"),
         ],
     )
 
     ff.register_training_set(
-        "testing_training", "one_lag_features",
+        "testing_training",
+        "one_lag_features",
         label=(f"testing_label", "testing"),
         features=[
             (f"testing_feature", "testing"),
-            {"feature": f"testing_feature", "variant": "testing", "name": "testing_feature_lag_1h", "lag": timedelta(hours=1)},
+            {
+                "feature": f"testing_feature",
+                "variant": "testing",
+                "name": "testing_feature_lag_1h",
+                "lag": timedelta(hours=1),
+            },
         ],
     )
 
     ff.register_training_set(
-        "testing_training", "two_lag_features",
+        "testing_training",
+        "two_lag_features",
         label=(f"testing_label", "testing"),
         features=[
             (f"testing_feature", "testing"),
-            {"feature": f"testing_feature", "variant": "testing", "name": "testing_feature_lag_1h", "lag": timedelta(hours=1)},
-            {"feature": f"testing_feature", "variant": "testing", "name": "testing_feature_lag_2h", "lag": timedelta(hours=2)},
+            {
+                "feature": f"testing_feature",
+                "variant": "testing",
+                "name": "testing_feature_lag_1h",
+                "lag": timedelta(hours=1),
+            },
+            {
+                "feature": f"testing_feature",
+                "variant": "testing",
+                "name": "testing_feature_lag_2h",
+                "lag": timedelta(hours=2),
+            },
         ],
     )
 
     ff.register_training_set(
-        "testing_training", "three_lag_features",
+        "testing_training",
+        "three_lag_features",
         label=(f"testing_label", "testing"),
         features=[
             (f"testing_feature", "testing"),
-            {"feature": f"testing_feature", "variant": "testing", "name": "testing_feature_lag_1h", "lag": timedelta(hours=1)},
-            {"feature": f"testing_feature", "variant": "testing", "name": "testing_feature_lag_2h", "lag": timedelta(hours=2)},
-            {"feature": f"testing_feature", "variant": "testing", "lag": timedelta(seconds=10800)},
+            {
+                "feature": f"testing_feature",
+                "variant": "testing",
+                "name": "testing_feature_lag_1h",
+                "lag": timedelta(hours=1),
+            },
+            {
+                "feature": f"testing_feature",
+                "variant": "testing",
+                "name": "testing_feature_lag_2h",
+                "lag": timedelta(hours=2),
+            },
+            {
+                "feature": f"testing_feature",
+                "variant": "testing",
+                "lag": timedelta(seconds=10800),
+            },
         ],
     )
 
     resource_client = ff.ResourceClient(local=True)
     resource_client.apply()
 
 
-
 @pytest.fixture()
 def source_df():
     df = pd.read_csv(SOURCE_FILE)
     df["timestamp"] = pd.to_datetime(df.timestamp)
-    df.rename(columns = {'value':'testing_feature.testing', 'timestamp':'label_timestamp', 'score': 'label'}, inplace=True)
+    df.rename(
+        columns={
+            "value": "testing_feature.testing",
+            "timestamp": "label_timestamp",
+            "score": "label",
+        },
+        inplace=True,
+    )
     return df
 
+
 @pytest.fixture()
 def df_no_lag(source_df):
-    return source_df[['testing_feature.testing', 'label_timestamp', 'label']]
+    return source_df[["testing_feature.testing", "label_timestamp", "label"]]
+
 
 @pytest.fixture()
 def df_one_lag(source_df):
     source_df.set_index("label_timestamp", inplace=True)
-    source_df["testing_feature_lag_1h"] = source_df["testing_feature.testing"].shift(freq=timedelta(hours=1))
+    source_df["testing_feature_lag_1h"] = source_df["testing_feature.testing"].shift(
+        freq=timedelta(hours=1)
+    )
     source_df.reset_index(inplace=True)
-    return source_df[['testing_feature.testing', 'testing_feature_lag_1h', 'label_timestamp', 'label']]
+    return source_df[
+        [
+            "testing_feature.testing",
+            "testing_feature_lag_1h",
+            "label_timestamp",
+            "label",
+        ]
+    ]
+
 
 @pytest.fixture()
 def df_two_lags(source_df):
     source_df.set_index("label_timestamp", inplace=True)
-    source_df["testing_feature_lag_1h"] = source_df["testing_feature.testing"].shift(freq=timedelta(hours=1))
-    source_df["testing_feature_lag_2h"] = source_df["testing_feature.testing"].shift(freq=timedelta(hours=2))
+    source_df["testing_feature_lag_1h"] = source_df["testing_feature.testing"].shift(
+        freq=timedelta(hours=1)
+    )
+    source_df["testing_feature_lag_2h"] = source_df["testing_feature.testing"].shift(
+        freq=timedelta(hours=2)
+    )
     source_df.reset_index(inplace=True)
-    return source_df[['testing_feature.testing', 'testing_feature_lag_1h', 'testing_feature_lag_2h', 'label_timestamp', 'label']]
+    return source_df[
+        [
+            "testing_feature.testing",
+            "testing_feature_lag_1h",
+            "testing_feature_lag_2h",
+            "label_timestamp",
+            "label",
+        ]
+    ]
 
 
 # @pytest.fixture()
 # def df_three_lags(source_df):
 #     source_df.set_index("label_timestamp", inplace=True)
 #     source_df["testing_feature_lag_1h"] = source_df["testing_feature.testing"].shift(freq=timedelta(hours=1))
 #     source_df["testing_feature_lag_2h"] = source_df["testing_feature.testing"].shift(freq=timedelta(hours=2))
 #     source_df["testing_feature_testing_lag_3_00_00"] = source_df["testing_feature.testing"].shift(freq=timedelta(hours=3))
 #     source_df.reset_index(inplace=True)
 #     return source_df[['testing_feature.testing', 'testing_feature_lag_1h', 'testing_feature_lag_2h', 'testing_feature_testing_lag_3_00_00', 'label_timestamp', 'label']]
 
+
 @pytest.mark.parametrize(
     "training_set_variant, expected_df_name",
     [
         ("no_lag_features", "df_no_lag"),
         ("one_lag_features", "df_one_lag"),
         ("two_lag_features", "df_two_lags"),
         # ("three_lag_features", "df_three_lags"),
-    ]
+    ],
 )
 def test_local_lag_features(training_set_variant, expected_df_name, request):
     expected_df = request.getfixturevalue(expected_df_name)
     serving_client = ff.ServingClient(local=True)
-    dataset = serving_client.training_set('testing_training', training_set_variant, include_label_timestamp=True)
+    dataset = serving_client.training_set(
+        "testing_training", training_set_variant, include_label_timestamp=True
+    )
     df = dataset.pandas()
     df["label_timestamp"] = pd.to_datetime(df.label_timestamp)
 
-    assert df.equals(expected_df), f"The dataframes do not match. Expected: {expected_df.head()}, Got: {df.head()}, Expected Info: {expected_df.info()} Got: {df.info()}"
-
+    assert df.equals(
+        expected_df
+    ), f"The dataframes do not match. Expected: {expected_df.head()}, Got: {df.head()}, Expected Info: {expected_df.info()} Got: {df.info()}"
 
 
 @pytest.fixture()
 def no_lag_feature_sql():
     return "SELECT * FROM source_0"
 
+
 @pytest.fixture()
 def one_lag_feature_sql():
     return """SELECT entity_1, timestamp, "testing_feature.testing", "lag_1h", label FROM (SELECT * FROM (SELECT *, row_number FROM ( SELECT entity_1, timestamp, label, "testing_feature.testing", "lag_1h", ROW_NUMBER() over (PARTITION BY entity_1, label, timestamp ORDER BY timestamp DESC, t0_ts DESC) as row_number FROM (( SELECT * FROM source_0 ) 
                          LEFT OUTER JOIN ( SELECT * FROM ( SELECT entity_1 AS t0_entity, "testing_feature.testing" AS "lag_1h", timestamp AS t0_ts
                          FROM source_0) 
                          ORDER BY t0_ts ASC) t0
                          ON (t0_entity = entity_1 AND DATETIME(t0_ts, "+3600.0 seconds") <= timestamp)
                          ) tt ) WHERE row_number=1 ORDER BY timestamp ASC ))"""
 
+
 @pytest.fixture()
 def two_lag_feature_sql():
     return """SELECT entity_1, timestamp, "testing_feature.testing", "lag_1h", "lag_2h", label FROM (SELECT * FROM (SELECT *, row_number FROM ( SELECT entity_1, timestamp, label, "testing_feature.testing", "lag_1h", "lag_2h", ROW_NUMBER() over (PARTITION BY entity_1, label, timestamp ORDER BY timestamp DESC, t0_ts DESC, t1_ts DESC) as row_number FROM (( SELECT * FROM source_0 ) 
                          LEFT OUTER JOIN ( SELECT * FROM ( SELECT entity_1 AS t0_entity, "testing_feature.testing" AS "lag_1h", timestamp AS t0_ts
                          FROM source_0) 
                          ORDER BY t0_ts ASC) t0
                          ON (t0_entity = entity_1 AND DATETIME(t0_ts, "+3600.0 seconds") <= timestamp)
                          
                          LEFT OUTER JOIN ( SELECT * FROM ( SELECT entity_1 AS t1_entity, "testing_feature.testing" AS "lag_2h", timestamp AS t1_ts
                          FROM source_0) 
                          ORDER BY t1_ts ASC) t1
                          ON (t1_entity = entity_1 AND DATETIME(t1_ts, "+7200.0 seconds") <= timestamp)
                          ) tt ) WHERE row_number=1 ORDER BY timestamp ASC ))"""
 
+
 @pytest.mark.parametrize(
     "lag_features, feature_columns, entity, label, ts, expected_sql_query",
     [
         ([], "", "", "", "", "no_lag_feature_sql"),
-        ([{"feature_name": "testing_feature", "feature_variant": "testing", "feature_lag": timedelta(hours=1).total_seconds(), "feature_new_name": "lag_1h"}], ["testing_feature.testing"], "entity_1", "label", "timestamp", "one_lag_feature_sql"),
-        ([{"feature_name": "testing_feature", "feature_variant": "testing", "feature_lag": timedelta(hours=1).total_seconds(), "feature_new_name": "lag_1h"}, {"feature_name": "testing_feature", "feature_variant": "testing", "feature_lag": timedelta(hours=2).total_seconds(), "feature_new_name": "lag_2h"}], ["testing_feature.testing"], "entity_1", "label", "timestamp", "two_lag_feature_sql"),
-    ]
+        (
+            [
+                {
+                    "feature_name": "testing_feature",
+                    "feature_variant": "testing",
+                    "feature_lag": timedelta(hours=1).total_seconds(),
+                    "feature_new_name": "lag_1h",
+                }
+            ],
+            ["testing_feature.testing"],
+            "entity_1",
+            "label",
+            "timestamp",
+            "one_lag_feature_sql",
+        ),
+        (
+            [
+                {
+                    "feature_name": "testing_feature",
+                    "feature_variant": "testing",
+                    "feature_lag": timedelta(hours=1).total_seconds(),
+                    "feature_new_name": "lag_1h",
+                },
+                {
+                    "feature_name": "testing_feature",
+                    "feature_variant": "testing",
+                    "feature_lag": timedelta(hours=2).total_seconds(),
+                    "feature_new_name": "lag_2h",
+                },
+            ],
+            ["testing_feature.testing"],
+            "entity_1",
+            "label",
+            "timestamp",
+            "two_lag_feature_sql",
+        ),
+    ],
 )
-def test_get_lag_features_sql_query(lag_features, feature_columns, entity, label, ts, expected_sql_query, request):
+def test_get_lag_features_sql_query(
+    lag_features, feature_columns, entity, label, ts, expected_sql_query, request
+):
     expected_sql_query = request.getfixturevalue(expected_sql_query)
 
     local_client = LocalClientImpl()
 
-    lag_sql_query = local_client.get_lag_features_sql_query(lag_features, feature_columns, entity, label, ts)
+    lag_sql_query = local_client.get_lag_features_sql_query(
+        lag_features, feature_columns, entity, label, ts
+    )
 
     assert lag_sql_query == expected_sql_query
```

### Comparing `featureform-1.7.4/tests/test_ondemand_features.py` & `featureform-1.8.0/tests/test_ondemand_features.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,22 +46,56 @@
 
 @pytest.mark.local
 @pytest.mark.parametrize(
     "features,entity,expected_output",
     [
         ([("avg_transactions", "quickstart")], {"user": "C8837983"}, [1875.0]),
         ([("pi", "default")], {"user": "C8837983"}, [3.141592653589793]),
-        ([("avg_transactions", "quickstart"), ("pi", "default")], {"user": "C8837983"}, [1875.0, 3.141592653589793]),
-        ([("pi", "default"), ("avg_transactions", "quickstart")], {"user": "C8837983"}, [3.141592653589793, 1875.0]),
-        ([("avg_transactions", "quickstart"), ("pi", "default"), ("avg_transactions", "quickstart")], {"user": "C8837983"}, [1875.0, 3.141592653589793, 1875.0]),
-        ([("avg_transactions", "quickstart"), ("pi", "default"), ("avg_transactions", "quickstart"), ("pi", "default")], {"user": "C8837983"}, [1875.0, 3.141592653589793, 1875.0, 3.141592653589793]),
-        ([("avg_transactions", "quickstart"), ("pi", "default"), ("pi", "pi_named"), ("pi_called", "default")], {"user": "C8837983"}, [1875.0, 3.141592653589793, 3.141592653589793, 3.141592653589793]),
+        (
+            [("avg_transactions", "quickstart"), ("pi", "default")],
+            {"user": "C8837983"},
+            [1875.0, 3.141592653589793],
+        ),
+        (
+            [("pi", "default"), ("avg_transactions", "quickstart")],
+            {"user": "C8837983"},
+            [3.141592653589793, 1875.0],
+        ),
+        (
+            [
+                ("avg_transactions", "quickstart"),
+                ("pi", "default"),
+                ("avg_transactions", "quickstart"),
+            ],
+            {"user": "C8837983"},
+            [1875.0, 3.141592653589793, 1875.0],
+        ),
+        (
+            [
+                ("avg_transactions", "quickstart"),
+                ("pi", "default"),
+                ("avg_transactions", "quickstart"),
+                ("pi", "default"),
+            ],
+            {"user": "C8837983"},
+            [1875.0, 3.141592653589793, 1875.0, 3.141592653589793],
+        ),
+        (
+            [
+                ("avg_transactions", "quickstart"),
+                ("pi", "default"),
+                ("pi", "pi_named"),
+                ("pi_called", "default"),
+            ],
+            {"user": "C8837983"},
+            [1875.0, 3.141592653589793, 3.141592653589793, 3.141592653589793],
+        ),
         pytest.param([], {}, [], marks=pytest.mark.xfail),
         pytest.param([("pi", "default")], None, [], marks=pytest.mark.xfail),
-    ]
+    ],
 )
 def test_serving_ondemand_precalculated_feature(features, entity, expected_output):
     register_resources()
     client = ff.ServingClient(local=True)
 
     features = client.features(features, entity)
     assert features.tolist() == expected_output
@@ -74,58 +108,73 @@
 
     local = ff.register_local()
 
     transactions = local.register_file(
         name="transactions",
         variant="quickstart",
         description="A dataset of fraudulent transactions",
-        path="transactions.csv"
+        path="transactions.csv",
     )
 
-    @local.df_transformation(variant="quickstart",
-                            inputs=[("transactions", "quickstart")])
+    @local.df_transformation(
+        variant="quickstart", inputs=[("transactions", "quickstart")]
+    )
     def average_user_transaction(transactions):
-        """the average transaction amount for a user """
+        """the average transaction amount for a user"""
         return transactions.groupby("CustomerID")["TransactionAmount"].mean()
 
     @ff.ondemand_feature
     def pi(serving_client, entities, params):
         import math
+
         return math.pi
 
     @ff.ondemand_feature()
     def pi_called(serving_client, entities, params):
         import math
+
         return math.pi
 
     @ff.ondemand_feature(variant="pi_named")
     def pi(serving_client, entities, params):
         import math
+
         return math.pi
 
     user = ff.register_entity("user")
     # Register a column from our transformation as a feature
     average_user_transaction.register_resources(
         entity=user,
         entity_column="CustomerID",
         inference_store=local,
         features=[
-            {"name": "avg_transactions", "variant": "quickstart", "column": "TransactionAmount", "type": "float32"},
+            {
+                "name": "avg_transactions",
+                "variant": "quickstart",
+                "column": "TransactionAmount",
+                "type": "float32",
+            },
         ],
     )
     # Register label from our base Transactions table
     transactions.register_resources(
         entity=user,
         entity_column="CustomerID",
         labels=[
-            {"name": "fraudulent", "variant": "quickstart", "column": "IsFraud", "type": "bool"},
+            {
+                "name": "fraudulent",
+                "variant": "quickstart",
+                "column": "IsFraud",
+                "type": "bool",
+            },
         ],
     )
 
     ff.register_training_set(
-        "fraud_training", "quickstart",
+        "fraud_training",
+        "quickstart",
         label=("fraudulent", "quickstart"),
         features=[("avg_transactions", "quickstart")],
     )
 
     resource_client = ff.ResourceClient(local=True)
     resource_client.apply()
```

### Comparing `featureform-1.7.4/tests/test_resource_registration.py` & `featureform-1.8.0/tests/test_resource_registration.py`

 * *Files identical despite different names*

### Comparing `featureform-1.7.4/tests/test_search.py` & `featureform-1.8.0/tests/test_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,131 +5,197 @@
 import pytest
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
-    ]
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
 )
 def test_simple_search(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
+    ]
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider, source, inference_store, is_local, is_insecure
+    )
 
     phrase_a_results = resource_client.search("quick", is_local)
     phrase_b_results = resource_client.search("transact", is_local)
     phrase_c_results = resource_client.search("dataset", is_local)
     phrase_d_results = resource_client.search("foo", is_local)
 
-    counts = [len(phrase_a_results), len(phrase_b_results), len(phrase_c_results), len(phrase_d_results)]
+    counts = [
+        len(phrase_a_results),
+        len(phrase_b_results),
+        len(phrase_c_results),
+        len(phrase_d_results),
+    ]
 
     assert counts == [4, 3, 1, 0]
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
-    ]
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
 )
 def test_special_character_search(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
+    ]
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider, source, inference_store, is_local, is_insecure
+    )
 
     phrase_a_results = resource_client.search("qui#ck!", is_local)
     phrase_b_results = resource_client.search("t*ran.saction!", is_local)
     phrase_c_results = resource_client.search("d,ata@se-t", is_local)
 
-    assert len(phrase_a_results) == 4 and len(phrase_b_results) == 3 and len(phrase_c_results) == 1
+    assert (
+        len(phrase_a_results) == 4
+        and len(phrase_b_results) == 3
+        and len(phrase_c_results) == 1
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
-    ]
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
 )
 def test_empty_query_to_search(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
+    ]
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider, source, inference_store, is_local, is_insecure
+    )
 
     with pytest.raises(Exception, match="query must be string and cannot be empty"):
         phrase = resource_client.search(raw_query="", local=is_local)
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
-    ]
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
 )
 def test_query_type_in_search(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
+    ]
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider, source, inference_store, is_local, is_insecure
+    )
 
-    with pytest.raises(TypeError, match="missing 1 required positional argument: 'raw_query'"):
+    with pytest.raises(
+        TypeError, match="missing 1 required positional argument: 'raw_query'"
+    ):
         phrase = resource_client.search(local=is_local)
 
 
 @pytest.fixture(autouse=True)
 def before_and_after_each(setup_teardown):
     setup_teardown()
     yield
     setup_teardown()
 
 
 def arrange_resources(provider, source, online_store, is_local, is_insecure):
     if is_local:
-        @provider.df_transformation(variant="quickstart", inputs=[("transactions", "quickstart")])
+
+        @provider.df_transformation(
+            variant="quickstart", inputs=[("transactions", "quickstart")]
+        )
         def average_user_transaction(transactions):
             return transactions.groupby("CustomerID")["TransactionAmount"].mean()
+
     else:
+
         @provider.sql_transformation(variant="quickstart")
         def average_user_transaction():
             return "SELECT customerid as user_id, avg(transactionamount) as avg_transaction_amt from {{transactions.quickstart}} GROUP BY user_id"
 
     user = ff.register_entity("user")
     feature_column = "TransactionAmount" if is_local else "avg_transaction_amt"
     label_column = "IsFraud" if is_local else "isfraud"
     inference_store = provider if is_local else online_store
 
     average_user_transaction.register_resources(
         entity=user,
         entity_column="CustomerID" if is_local else "user_id",
         inference_store=inference_store,
         features=[
-            {"name": "avg_transactions", "variant": "quickstart", "column": feature_column, "type": "float32"},
+            {
+                "name": "avg_transactions",
+                "variant": "quickstart",
+                "column": feature_column,
+                "type": "float32",
+            },
         ],
     )
 
     source.register_resources(
         entity=user,
         entity_column="CustomerID" if is_local else "customerid",
         labels=[
-            {"name": "fraudulent", "variant": "quickstart", "column": label_column, "type": "bool"},
+            {
+                "name": "fraudulent",
+                "variant": "quickstart",
+                "column": label_column,
+                "type": "bool",
+            },
         ],
     )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     return resource_client
```

### Comparing `featureform-1.7.4/tests/test_source_dataframe.py` & `featureform-1.8.0/tests/test_source_dataframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     [
         pytest.param(
             "local_provider_source",
             True,
             True,
             marks=pytest.mark.local,
         ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
     ],
 )
 def test_dataframe_for_name_variant_args(
     provider_source_fxt, is_local, is_insecure, request
 ):
     custom_marks = [
         mark.name for mark in request.node.own_markers if mark.name != "parametrize"
@@ -24,17 +30,22 @@
     provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
         custom_marks
     )
 
     transformation = arrange_transformation(provider, is_local)
 
     client = ff.Client(local=is_local, insecure=is_insecure)
-    client.apply(asynchronous=True)
+    # If we're running in a hosted context, `apply` needs to be synchronous
+    # to ensure resources are ready to test.
+    client.apply(asynchronous=is_local)
 
-    source_df = client.dataframe(source.name, source.variant)
+    if is_local:
+        source_df = client.dataframe(source.name, source.variant)
+    else:
+        source_df = client.dataframe(*source.name_variant())
     transformation_df = client.dataframe(*transformation.name_variant())
 
     assert isinstance(source_df, pd.DataFrame) and isinstance(
         transformation_df, (pd.DataFrame, pd.Series)
     )
 
     if is_local:
@@ -46,28 +57,36 @@
     [
         pytest.param(
             "local_provider_source",
             True,
             True,
             marks=pytest.mark.local,
         ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
     ],
 )
 def test_dataframe_for_source_args(provider_source_fxt, is_local, is_insecure, request):
     custom_marks = [
         mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
     provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
         custom_marks
     )
 
     transformation = arrange_transformation(provider, is_local)
 
     client = ff.Client(local=is_local, insecure=is_insecure)
-    client.apply(asynchronous=True)
+    # If we're running in a hosted context, `apply` needs to be synchronous
+    # to ensure resources are ready to test.
+    client.apply(asynchronous=is_local)
 
     source_df = client.dataframe(source)
     transformation_df = client.dataframe(transformation)
 
     assert isinstance(source_df, pd.DataFrame) and isinstance(
         transformation_df, (pd.DataFrame, pd.Series)
     )
@@ -127,10 +146,10 @@
         def average_user_transaction(transactions):
             return transactions.groupby("CustomerID")["TransactionAmount"].mean()
 
     else:
 
         @provider.sql_transformation(variant="quickstart")
         def average_user_transaction():
-            return "SELECT customerid as user_id, avg(transactionamount) as avg_transaction_amt from {{transactions.quickstart}} GROUP BY user_id"
+            return "SELECT customerid as user_id, avg(transactionamount) AS avg_transaction_amt FROM {{transactions.quickstart}} GROUP BY user_id"
 
     return average_user_transaction
```

### Comparing `featureform-1.7.4/tests/test_spark_provider.py` & `featureform-1.8.0/tests/test_spark_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,67 @@
 import dill
 
 import pytest
 
 from featureform.register import ColumnSourceRegistrar, OfflineSparkProvider, Registrar
-from featureform.resources import DFTransformation, Provider, Source, SparkConfig, SQLTransformation, DatabricksCredentials, AzureFileStoreConfig, SparkCredentials
+from featureform.resources import (
+    DFTransformation,
+    Provider,
+    Source,
+    SparkConfig,
+    SQLTransformation,
+    DatabricksCredentials,
+    AzureFileStoreConfig,
+    SparkCredentials,
+)
 
 
 @pytest.mark.parametrize(
     "executor_fixture, filestore_fixture",
     [
         ("databricks", "azure_blob"),
         ("databricks", "s3"),
         ("emr", "azure_blob"),
         ("emr", "s3"),
-    ]
+    ],
 )
 def test_create_provider(executor_fixture, filestore_fixture, request):
     executor = request.getfixturevalue(executor_fixture)
     filestore = request.getfixturevalue(filestore_fixture)
 
     provider_name = "test_offline_spark_provider"
-    r = Registrar() 
-    
-    config = SparkConfig(executor_type=executor.type(), executor_config=executor.config(), store_type=filestore.store_type(), store_config=filestore.config())
-    provider = Provider(name=provider_name, function="OFFLINE", description="", team="", config=config, tags=[], properties={})
-    
+    r = Registrar()
+
+    config = SparkConfig(
+        executor_type=executor.type(),
+        executor_config=executor.config(),
+        store_type=filestore.store_type(),
+        store_config=filestore.config(),
+    )
+    provider = Provider(
+        name=provider_name,
+        function="OFFLINE",
+        description="",
+        team="",
+        config=config,
+        tags=[],
+        properties={},
+    )
+
     offline_spark_provider = OfflineSparkProvider(r, provider)
     assert type(offline_spark_provider) == OfflineSparkProvider
     assert offline_spark_provider.name() == provider_name
 
 
 @pytest.mark.parametrize(
     "test_name,file_path,default_variant",
     [
         ("file", "test_files/input/transaction", False),
         ("file", "test_files/input/transaction", True),
-    ]
+    ],
 )
 def test_register_file(test_name, file_path, default_variant, spark_provider):
     if default_variant:
         variant = "default"
         s = spark_provider.register_file(
             name=test_name,
             file_path=file_path,
@@ -53,22 +75,22 @@
         )
 
     assert type(s) == ColumnSourceRegistrar
 
     src = s._SourceRegistrar__source
     assert src.owner == spark_provider._OfflineSparkProvider__registrar.default_owner()
     assert src.provider == spark_provider.name()
-    assert src.variant == variant 
+    assert src.variant == variant
 
 
 @pytest.mark.parametrize(
     "name,variant,sql",
     [
-        ("test_name", "test_variant","SELECT * FROM {{test_name.test_variant}}"),
-    ]
+        ("test_name", "test_variant", "SELECT * FROM {{test_name.test_variant}}"),
+    ],
 )
 def test_sql_transformation(name, variant, sql, spark_provider):
     def transformation():
         """doc string"""
         return sql
 
     decorator = spark_provider.sql_transformation(name=name, variant=variant)
@@ -78,23 +100,23 @@
         name=name,
         variant=variant,
         definition=SQLTransformation(query=sql),
         owner="tester",
         provider="spark",
         description="doc string",
         tags=[],
-        properties={}
+        properties={},
     )
 
 
 @pytest.mark.parametrize(
     "sql",
     [
         ("SELECT * FROM {{test_name.test_variant}}"),
-    ]
+    ],
 )
 def test_sql_transformation_without_variant(sql, spark_provider):
     def transformation():
         """doc string"""
         return sql
 
     decorator = spark_provider.sql_transformation()
@@ -104,103 +126,116 @@
         name=transformation.__name__,
         variant="default",
         definition=SQLTransformation(query=sql),
         owner="tester",
         provider="spark",
         description="doc string",
         tags=[],
-        properties={}
+        properties={},
     )
 
 
 @pytest.mark.parametrize(
     "name,variant,inputs,transformation",
     [
         ("test_input", "primary_dataset", "primary_dataset", "avg_user_transaction"),
-        ("test_input", "df_transformation", "df_transformation_src", "avg_user_transaction"),
-        ("test_input", "sql_transformation", "sql_transformation_src", "avg_user_transaction"),
+        (
+            "test_input",
+            "df_transformation",
+            "df_transformation_src",
+            "avg_user_transaction",
+        ),
+        (
+            "test_input",
+            "sql_transformation",
+            "sql_transformation_src",
+            "avg_user_transaction",
+        ),
         ("test_input", "tuples", "tuple_inputs", "avg_user_transaction"),
-    ]
+    ],
 )
-def test_df_transformation(name, variant, inputs, transformation, spark_provider, request):
+def test_df_transformation(
+    name, variant, inputs, transformation, spark_provider, request
+):
     df_transformation = request.getfixturevalue(transformation)
     inputs = request.getfixturevalue(inputs)
 
-    decorator = spark_provider.df_transformation(name=name, variant=variant, inputs=inputs)
+    decorator = spark_provider.df_transformation(
+        name=name, variant=variant, inputs=inputs
+    )
     decorator(df_transformation)
 
     query = dill.dumps(df_transformation.__code__)
 
     decorator_src = decorator.to_source()
     expected_src = Source(
         name=name,
         variant=variant,
         definition=DFTransformation(query=query, inputs=inputs),
         owner="tester",
         provider="spark",
         description="doc string",
         tags=[],
-        properties={}
+        properties={},
     )
-    
+
     assert decorator_src.name == expected_src.name
     assert decorator_src.owner == expected_src.owner
-    assert decorator_src.provider == expected_src.provider 
+    assert decorator_src.provider == expected_src.provider
     assert decorator_src.description == expected_src.description
     assert decorator_src.definition.type() == expected_src.definition.type()
     assert decorator_src.definition.kwargs() == expected_src.definition.kwargs()
 
 
-
 @pytest.mark.parametrize(
     "store_config",
     [
         "s3_config",
         "azure_file_config",
         pytest.param("s3_config_slash", marks=pytest.mark.xfail),
         pytest.param("s3_config_slash_ending", marks=pytest.mark.xfail),
-    ]
+    ],
 )
 def test_store_config(store_config, request):
     store, expected_config = request.getfixturevalue(store_config)
 
     assert store.config() == expected_config
 
 
 @pytest.mark.parametrize(
     "executor_config",
     [
         "databricks_config",
         "emr_config",
         "spark_executor",
         pytest.param("spark_executor_incorrect_deploy_mode", marks=pytest.mark.xfail),
-    ]
+    ],
 )
 def test_executor_config(executor_config, request):
     executor, expected_config = request.getfixturevalue(executor_config)
 
     assert executor.config() == expected_config
 
 
 @pytest.mark.parametrize(
     "version,expected_version",
     [
-        ("3.7","3.7.16"),
-        ("3.8","3.8.16"),
-        ("3.9","3.9.16"),
-        ("3.10","3.10.10"),
-        ("3.7.10","3.7.16"),
-        ("3.7.1","3.7.16"),
-        ("3.8.16","3.8.16"),
-        ("3.9.11","3.9.16"),
-        ("3.10.10","3.10.10"),
-        ("3.11.2","3.11.2"),
-        pytest.param("3","", marks=pytest.mark.xfail),
-        pytest.param("3.","", marks=pytest.mark.xfail),
-        pytest.param("2.10","", marks=pytest.mark.xfail),
-        pytest.param("3.10.10.0","", marks=pytest.mark.xfail),
-    ]
+        ("3.7", "3.7.16"),
+        ("3.8", "3.8.16"),
+        ("3.9", "3.9.16"),
+        ("3.10", "3.10.10"),
+        ("3.7.10", "3.7.16"),
+        ("3.7.1", "3.7.16"),
+        ("3.8.16", "3.8.16"),
+        ("3.9.11", "3.9.16"),
+        ("3.10.10", "3.10.10"),
+        ("3.11.2", "3.11.2"),
+        pytest.param("3", "", marks=pytest.mark.xfail),
+        pytest.param("3.", "", marks=pytest.mark.xfail),
+        pytest.param("2.10", "", marks=pytest.mark.xfail),
+        pytest.param("3.10.10.0", "", marks=pytest.mark.xfail),
+    ],
 )
 def test__verify_python_version(version, expected_version):
     spark = SparkCredentials("local", "client", version)
 
     assert spark.python_version == expected_version
```

### Comparing `featureform-1.7.4/tests/test_tags_and_properties.py` & `featureform-1.8.0/tests/test_tags_and_properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,92 +3,96 @@
 import os
 import pytest
 import time
 
 real_path = os.path.realpath(__file__)
 dir_path = os.path.dirname(real_path)
 
+
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_adding_tags_and_properties_to_provider(is_local, is_insecure, request):
     name = "postgres_docs"
     tags = ["pg_offline_provider", "ff_team"]
     properties = {"primary_offline_provider": "true"}
 
     ff.register_postgres(
-        name = name,
-        description = "Example offline store store",
-        team = "Featureform",
-        host = "0.0.0.0",
-        port = "5432",
-        user = "postgres",
-        password = "password",
-        database = "postgres",
+        name=name,
+        description="Example offline store store",
+        team="Featureform",
+        host="0.0.0.0",
+        port="5432",
+        user="postgres",
+        password="password",
+        database="postgres",
         tags=tags,
-        properties=properties
+        properties=properties,
     )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     postgres = resource_client.get_provider(name, is_local)
-    assert get_tags(postgres, is_local) == tags and get_properties(postgres, is_local) == properties
+    assert (
+        get_tags(postgres, is_local) == tags
+        and get_properties(postgres, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_updating_tags_and_properties_for_provider(is_local, is_insecure, request):
     name = "postgres_docs"
     tags = ["pg_offline_provider", "ff_team"]
     properties = {"primary_offline_provider": "true"}
 
     ff.register_postgres(
-        name = name,
-        description = "Example offline store store",
-        team = "Featureform",
-        host = "0.0.0.0",
-        port = "5432",
-        user = "postgres",
-        password = "password",
-        database = "postgres",
+        name=name,
+        description="Example offline store store",
+        team="Featureform",
+        host="0.0.0.0",
+        port="5432",
+        user="postgres",
+        password="password",
+        database="postgres",
         tags=tags,
-        properties=properties
+        properties=properties,
     )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     ff.clear_state()
 
     additional_tags = ["training_data"]
     additional_properties = {"is_active": "true"}
 
     ff.register_postgres(
-        name = name,
-        description = "Example offline store store",
-        team = "Featureform",
-        host = "0.0.0.0",
-        port = "5432",
-        user = "postgres",
-        password = "password",
-        database = "postgres",
+        name=name,
+        description="Example offline store store",
+        team="Featureform",
+        host="0.0.0.0",
+        port="5432",
+        user="postgres",
+        password="password",
+        database="postgres",
         tags=additional_tags,
-        properties=additional_properties
+        properties=additional_properties,
     )
     resource_client.apply()
     postgres = resource_client.get_provider(name, is_local)
 
     expected_tags = set(tags + additional_tags)
     expected_properties = {**properties, **additional_properties}
 
@@ -100,55 +104,58 @@
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_adding_tags_and_properties_to_user(is_local, is_insecure, request):
     username = "ff_user"
     tags = ["primary_user"]
     properties = {"rotated_credentials": "yes"}
 
-    ff.register_user(username,tags=tags, properties=properties)
+    ff.register_user(username, tags=tags, properties=properties)
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     user = resource_client.get_user(username, is_local)
 
-    assert get_tags(user, is_local) == tags and get_properties(user, is_local) == properties
+    assert (
+        get_tags(user, is_local) == tags
+        and get_properties(user, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_updating_tags_and_properties_for_user(is_local, is_insecure, request):
     username = "ff_user"
     tags = ["primary_user"]
     properties = {"rotated_credentials": "yes"}
 
-    ff.register_user(username,tags=tags, properties=properties)
+    ff.register_user(username, tags=tags, properties=properties)
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     ff.clear_state()
 
     additional_tags = ["shared_credentials"]
     additional_properties = {"credential_location": "secret_vault"}
 
-    ff.register_user(username,tags=additional_tags, properties=additional_properties)
+    ff.register_user(username, tags=additional_tags, properties=additional_properties)
     resource_client.apply()
 
     user = resource_client.get_user(username, is_local)
 
     expected_tags = set(tags + additional_tags)
     expected_properties = {**properties, **additional_properties}
 
@@ -158,86 +165,109 @@
     assert actual_tags == expected_tags and actual_properties == expected_properties
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_adding_tags_and_properties_to_source(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_adding_tags_and_properties_to_source(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     name = "transactions_src"
     variant = "quickstart_v2"
     tags = ["fraud_project", "primary_source"]
     properties = {"project_type": "fraud_prediction"}
 
     if is_local:
         provider.register_file(
             name=name,
             variant=variant,
             description="A dataset of fraudulent transactions.",
             path=f"{dir_path}/test_files/input_files/transactions.csv",
             tags=tags,
-            properties=properties
+            properties=properties,
         )
     else:
         provider.register_table(
             name=name,
-            table="Transactions", # This is the table's name in Postgres
+            table="Transactions",  # This is the table's name in Postgres
             variant=variant,
             tags=tags,
-            properties=properties
+            properties=properties,
         )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     source = resource_client.print_source(name, variant, is_local)
 
-    assert get_tags(source, is_local) == tags and get_properties(source, is_local) == properties
+    assert (
+        get_tags(source, is_local) == tags
+        and get_properties(source, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_updating_tags_and_properties_for_source(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_updating_tags_and_properties_for_source(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     name = "transactions_src_2"
     variant = "quickstart_v1"
     tags = ["fraud_project", "primary_source"]
     properties = {"project_type": "fraud_prediction"}
 
     if is_local:
         provider.register_file(
             name=name,
             variant=variant,
             description="A dataset of fraudulent transactions.",
             path=f"{dir_path}/test_files/input_files/transactions.csv",
             tags=tags,
-            properties=properties
+            properties=properties,
         )
     else:
         provider.register_table(
             name=name,
-            table="Transactions", # This is the table's name in Postgres
+            table="Transactions",  # This is the table's name in Postgres
             variant=variant,
             tags=tags,
-            properties=properties
+            properties=properties,
         )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     ff.clear_state()
 
@@ -247,23 +277,23 @@
     if is_local:
         provider.register_file(
             name=name,
             variant=variant,
             description="A dataset of fraudulent transactions.",
             path=f"{dir_path}/test_files/input_files/transactions.csv",
             tags=additional_tags,
-            properties=additional_properties
+            properties=additional_properties,
         )
     else:
         provider.register_table(
             name=name,
-            table="Transactions", # This is the table's name in Postgres
+            table="Transactions",  # This is the table's name in Postgres
             variant=variant,
             tags=additional_tags,
-            properties=additional_properties
+            properties=additional_properties,
         )
 
     resource_client.apply()
 
     source = resource_client.print_source(name, variant, is_local)
 
     expected_tags = set(tags + additional_tags)
@@ -275,83 +305,136 @@
     assert actual_tags == expected_tags and actual_properties == expected_properties
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_adding_tags_and_properties_to_transformation(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_adding_tags_and_properties_to_transformation(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
-    tags=["user_avg"]
-    properties={"aggregate_type": "avg"}
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
+    tags = ["user_avg"]
+    properties = {"aggregate_type": "avg"}
     variant = "quickstart"
     if is_local:
-        @provider.df_transformation(variant=variant, inputs=[("transactions", "quickstart")], tags=tags, properties=properties)
+
+        @provider.df_transformation(
+            variant=variant,
+            inputs=[("transactions", "quickstart")],
+            tags=tags,
+            properties=properties,
+        )
         def average_user_transaction_v1(transactions):
             return transactions.groupby("CustomerID")["TransactionAmount"].mean()
+
     else:
+
         @provider.sql_transformation(variant=variant, tags=tags, properties=properties)
         def average_user_transaction_v1():
             return "SELECT customerid as user_id, avg(transactionamount) as avg_transaction_amt from {{transactions.quickstart}} GROUP BY user_id"
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
-    source = resource_client.print_source("average_user_transaction_v1", variant, is_local)
+    source = resource_client.print_source(
+        "average_user_transaction_v1", variant, is_local
+    )
 
-    assert get_tags(source, is_local) == tags and get_properties(source, is_local) == properties
+    assert (
+        get_tags(source, is_local) == tags
+        and get_properties(source, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_updating_tags_and_properties_for_transformation(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_updating_tags_and_properties_for_transformation(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
-    tags=["user_avg"]
-    properties={"aggregate_type": "avg"}
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
+    tags = ["user_avg"]
+    properties = {"aggregate_type": "avg"}
     variant = "quickstart"
     if is_local:
-        @provider.df_transformation(variant=variant, inputs=[("transactions", "quickstart")], tags=tags, properties=properties)
+
+        @provider.df_transformation(
+            variant=variant,
+            inputs=[("transactions", "quickstart")],
+            tags=tags,
+            properties=properties,
+        )
         def average_user_transaction_v2(transactions):
             return transactions.groupby("CustomerID")["TransactionAmount"].mean()
+
     else:
+
         @provider.sql_transformation(variant=variant, tags=tags, properties=properties)
         def average_user_transaction_v2():
             return "SELECT customerid as user_id, avg(transactionamount) as avg_transaction_amt from {{transactions.quickstart}} GROUP BY user_id"
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     ff.clear_state()
 
     additional_tags = ["avg_user_transaction_v2"]
     additional_properties = {"version": "2"}
 
     if is_local:
-        @provider.df_transformation(variant=variant, inputs=[("transactions", "quickstart")], tags=additional_tags, properties=additional_properties)
+
+        @provider.df_transformation(
+            variant=variant,
+            inputs=[("transactions", "quickstart")],
+            tags=additional_tags,
+            properties=additional_properties,
+        )
         def average_user_transaction_v2(transactions):
             return transactions.groupby("CustomerID")["TransactionAmount"].mean()
+
     else:
-        @provider.sql_transformation(variant=variant, tags=additional_tags, properties=additional_properties)
+
+        @provider.sql_transformation(
+            variant=variant, tags=additional_tags, properties=additional_properties
+        )
         def average_user_transaction_v2():
             return "SELECT customerid as user_id, avg(transactionamount) as avg_transaction_amt from {{transactions.quickstart}} GROUP BY user_id"
 
     resource_client.apply()
-    source = resource_client.print_source("average_user_transaction_v2", variant, is_local)
+    source = resource_client.print_source(
+        "average_user_transaction_v2", variant, is_local
+    )
 
     expected_tags = set(tags + additional_tags)
     expected_properties = {**properties, **additional_properties}
 
     actual_tags = set(get_tags(source, is_local))
     actual_properties = get_properties(source, is_local)
 
@@ -360,42 +443,51 @@
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_adding_tags_and_properties_to_entity(is_local, is_insecure, request):
     name = "cc_user"
     tags = ["customers", "user_ent"]
-    properties = {"entity_name": "user", "is_user_data": "yes",}
+    properties = {
+        "entity_name": "user",
+        "is_user_data": "yes",
+    }
 
     ff.register_entity(name, tags=tags, properties=properties)
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     entity = resource_client.get_entity(name, is_local)
 
-    assert get_tags(entity, is_local) == tags and get_properties(entity, is_local) == properties
+    assert (
+        get_tags(entity, is_local) == tags
+        and get_properties(entity, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "is_local,is_insecure",
     [
         pytest.param(True, True, marks=pytest.mark.local),
         pytest.param(False, False, marks=pytest.mark.hosted),
         pytest.param(False, True, marks=pytest.mark.docker),
-    ]
+    ],
 )
 def test_updating_tags_and_properties_for_entity(is_local, is_insecure, request):
     name = "cc_user_2"
     tags = ["customers", "user_ent"]
-    properties = {"entity_name": "user", "is_user_data": "yes",}
+    properties = {
+        "entity_name": "user",
+        "is_user_data": "yes",
+    }
 
     ff.register_entity(name, tags=tags, properties=properties)
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     ff.clear_state()
 
@@ -416,53 +508,109 @@
     assert actual_tags == expected_tags and actual_properties == expected_properties
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_adding_tags_and_properties_to_feature(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_adding_tags_and_properties_to_feature(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
     tags = ["feat_1", "feat_2", "feat_3"]
-    properties = {"feat_prop_key_1": "feat_prop_val_1", "feat_prop_key_2": "feat_prop_val_2"}
+    properties = {
+        "feat_prop_key_1": "feat_prop_val_1",
+        "feat_prop_key_2": "feat_prop_val_2",
+    }
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, tags, properties, "feature", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        tags,
+        properties,
+        "feature",
+        is_local,
+        is_insecure,
+    )
 
     feature = resource_client.print_feature("avg_transactions", "quickstart", is_local)
 
-    assert get_tags(feature, is_local) == tags and get_properties(feature, is_local) == properties
+    assert (
+        get_tags(feature, is_local) == tags
+        and get_properties(feature, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_updating_tags_and_properties_for_feature(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_updating_tags_and_properties_for_feature(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
     tags = ["feat_1", "feat_2", "feat_3"]
-    properties = {"feat_prop_key_1": "feat_prop_val_1", "feat_prop_key_2": "feat_prop_val_2"}
+    properties = {
+        "feat_prop_key_1": "feat_prop_val_1",
+        "feat_prop_key_2": "feat_prop_val_2",
+    }
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, tags, properties, "feature", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        tags,
+        properties,
+        "feature",
+        is_local,
+        is_insecure,
+    )
 
     ff.clear_state()
 
     additional_tags = ["feat_tag_4", "feat_tag_5"]
     additional_properties = {"feat_prop_key_3": "feat_prop_val_3"}
 
-    resource_client = arrange_resources(provider, source, inference_store, additional_tags, additional_properties, "feature", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        additional_tags,
+        additional_properties,
+        "feature",
+        is_local,
+        is_insecure,
+    )
 
     feature = resource_client.print_feature("avg_transactions", "quickstart", is_local)
 
     expected_tags = set(tags + additional_tags)
     expected_properties = {**properties, **additional_properties}
 
     actual_tags = set(get_tags(feature, is_local))
@@ -471,53 +619,109 @@
     assert actual_tags == expected_tags and actual_properties == expected_properties
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_adding_tags_and_properties_to_label(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_adding_tags_and_properties_to_label(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
     tags = ["lbl_tag_1", "lbl_tag_2", "lbl_tag_3"]
-    properties = {"lbl_prop_key_1": "lbl_prop_val_1", "lbl_prop_key_1": "lbl_prop_val_2"}
+    properties = {
+        "lbl_prop_key_1": "lbl_prop_val_1",
+        "lbl_prop_key_1": "lbl_prop_val_2",
+    }
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, tags, properties, "label", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        tags,
+        properties,
+        "label",
+        is_local,
+        is_insecure,
+    )
 
     label = resource_client.print_label("fraudulent", "quickstart", is_local)
 
-    assert get_tags(label, is_local) == tags and get_properties(label, is_local) == properties
+    assert (
+        get_tags(label, is_local) == tags
+        and get_properties(label, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_updating_tags_and_properties_for_label(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_updating_tags_and_properties_for_label(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
     tags = ["lbl_tag_1", "lbl_tag_2", "lbl_tag_3"]
-    properties = {"lbl_prop_key_1": "lbl_prop_val_1", "lbl_prop_key_1": "lbl_prop_val_2"}
+    properties = {
+        "lbl_prop_key_1": "lbl_prop_val_1",
+        "lbl_prop_key_1": "lbl_prop_val_2",
+    }
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, tags, properties, "label", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        tags,
+        properties,
+        "label",
+        is_local,
+        is_insecure,
+    )
 
     ff.clear_state()
 
     additional_tags = ["lbl_tag_4", "lbl_tag_5"]
     additional_properties = {"lbl_prop_key_3": "lbl_prop_val_3"}
 
-    resource_client = arrange_resources(provider, source, inference_store, additional_tags, additional_properties, "label", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        additional_tags,
+        additional_properties,
+        "label",
+        is_local,
+        is_insecure,
+    )
 
     label = resource_client.print_label("fraudulent", "quickstart", is_local)
 
     expected_tags = set(tags + additional_tags)
     expected_properties = {**properties, **additional_properties}
 
     actual_tags = set(get_tags(label, is_local))
@@ -526,55 +730,109 @@
     assert actual_tags == expected_tags and actual_properties == expected_properties
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_adding_tags_and_properties_to_training_set(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_adding_tags_and_properties_to_training_set(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
     tags = ["ts_tag_1", "ts_tag_2", "ts_tag_3"]
     properties = {"ts_prop_key_1": "ts_prop_val_1", "ts_prop_key_1": "ts_prop_val_2"}
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, tags, properties, "training-set", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        tags,
+        properties,
+        "training-set",
+        is_local,
+        is_insecure,
+    )
 
-    training_set = resource_client.print_training_set("fraud_training", "quickstart", is_local)
+    training_set = resource_client.print_training_set(
+        "fraud_training", "quickstart", is_local
+    )
 
-    assert get_tags(training_set, is_local) == tags and get_properties(training_set, is_local) == properties
+    assert (
+        get_tags(training_set, is_local) == tags
+        and get_properties(training_set, is_local) == properties
+    )
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
+)
+def test_updating_tags_and_properties_for_training_set(
+    provider_source_fxt, is_local, is_insecure, request
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
     ]
-)
-def test_updating_tags_and_properties_for_training_set(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
     tags = ["ts_tag_1", "ts_tag_2", "ts_tag_3"]
     properties = {"ts_prop_key_1": "ts_prop_val_1", "ts_prop_key_1": "ts_prop_val_2"}
     # Arranges the resources context following the Quickstart pattern
-    resource_client = arrange_resources(provider, source, inference_store, tags, properties, "training-set", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        tags,
+        properties,
+        "training-set",
+        is_local,
+        is_insecure,
+    )
 
     ff.clear_state()
 
     additional_tags = ["ts_tag_4", "ts_tag_5"]
     additional_properties = {"ts_prop_key_3": "ts_prop_val_3"}
 
-    resource_client = arrange_resources(provider, source, inference_store, additional_tags, additional_properties, "training-set", is_local, is_insecure)
+    resource_client = arrange_resources(
+        provider,
+        source,
+        inference_store,
+        additional_tags,
+        additional_properties,
+        "training-set",
+        is_local,
+        is_insecure,
+    )
 
-    training_set = resource_client.print_training_set("fraud_training", "quickstart", is_local)
+    training_set = resource_client.print_training_set(
+        "fraud_training", "quickstart", is_local
+    )
 
     expected_tags = set(tags + additional_tags)
     expected_properties = {**properties, **additional_properties}
 
     actual_tags = set(get_tags(training_set, is_local))
     actual_properties = get_properties(training_set, is_local)
 
@@ -584,20 +842,34 @@
 @pytest.fixture(autouse=True)
 def before_and_after_each(setup_teardown):
     setup_teardown()
     yield
     setup_teardown()
 
 
-def arrange_resources(provider, source, online_store, tags, properties, resource_type, is_local, is_insecure):
+def arrange_resources(
+    provider,
+    source,
+    online_store,
+    tags,
+    properties,
+    resource_type,
+    is_local,
+    is_insecure,
+):
     if is_local:
-        @provider.df_transformation(variant="quickstart", inputs=[("transactions", "quickstart")])
+
+        @provider.df_transformation(
+            variant="quickstart", inputs=[("transactions", "quickstart")]
+        )
         def average_user_transaction(transactions):
             return transactions.groupby("CustomerID")["TransactionAmount"].mean()
+
     else:
+
         @provider.sql_transformation(variant="quickstart")
         def average_user_transaction():
             return "SELECT customerid as user_id, avg(transactionamount) as avg_transaction_amt from {{transactions.quickstart}} GROUP BY user_id"
 
     user = ff.register_entity("user")
     feature_column = "TransactionAmount" if is_local else "avg_transaction_amt"
     label_column = "IsFraud" if is_local else "isfraud"
@@ -609,60 +881,85 @@
 
     if resource_type != "label":
         average_user_transaction.register_resources(
             entity=user,
             entity_column="CustomerID" if is_local else "user_id",
             inference_store=inference_store,
             features=[
-                {"name": "avg_transactions", "variant": "quickstart", "column": feature_column, "type": "float32", "tags": feature_tags, "properties": feature_properties},
+                {
+                    "name": "avg_transactions",
+                    "variant": "quickstart",
+                    "column": feature_column,
+                    "type": "float32",
+                    "tags": feature_tags,
+                    "properties": feature_properties,
+                },
             ],
         )
 
     if resource_type != "feature":
         source.register_resources(
             entity=user,
             entity_column="CustomerID" if is_local else "customerid",
             labels=[
-                {"name": "fraudulent", "variant": "quickstart", "column": label_column, "type": "bool", "tags": label_tags, "properties": label_properties},
+                {
+                    "name": "fraudulent",
+                    "variant": "quickstart",
+                    "column": label_column,
+                    "type": "bool",
+                    "tags": label_tags,
+                    "properties": label_properties,
+                },
             ],
         )
 
     training_set_name = "fraud_training"
     training_set_variant = "quickstart"
 
     if resource_type == "training-set":
         ff.register_training_set(
-            training_set_name, training_set_variant,
+            training_set_name,
+            training_set_variant,
             label=("fraudulent", "quickstart"),
             features=[("avg_transactions", "quickstart")],
             tags=tags,
-            properties=properties
+            properties=properties,
         )
 
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     if not is_local and resource_type == "training-set":
         start = time.time()
         while True:
             time.sleep(3)
-            ts = resource_client.get_training_set(training_set_name, training_set_variant)
+            ts = resource_client.get_training_set(
+                training_set_name, training_set_variant
+            )
             elapsed_wait = time.time() - start
             if (elapsed_wait >= 60) and ts.status != "READY":
-                print(f"Wait time for training set status exceeded; status is {ts.status}")
+                print(
+                    f"Wait time for training set status exceeded; status is {ts.status}"
+                )
                 break
             elif ts.status == "READY":
                 print(f"Training set is ready")
                 break
             else:
-                print(f"Training set status is currently {ts.status} after {elapsed_wait} seconds ...")
+                print(
+                    f"Training set status is currently {ts.status} after {elapsed_wait} seconds ..."
+                )
                 continue
 
     return resource_client
 
 
 def get_tags(resource, is_local):
     return resource["tags"] if is_local else resource.tags.tag
 
 
 def get_properties(resource, is_local):
-    return resource["properties"] if is_local else {k:v.string_value for (k, v) in resource.properties.property.items()}
+    return (
+        resource["properties"]
+        if is_local
+        else {k: v.string_value for (k, v) in resource.properties.property.items()}
+    )
```

### Comparing `featureform-1.7.4/tests/test_updating_provider.py` & `featureform-1.8.0/tests/test_updating_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,34 @@
 from types import SimpleNamespace
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
-    ]
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
 )
 def test_valid_provider_update(provider_source_fxt, is_local, is_insecure, request):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
+    ]
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     # Arranges the resources context following the Quickstart pattern
-    resource_client, postgres_name, redis_name = arrange_resources(provider, source, inference_store, is_local, is_insecure)
+    resource_client, postgres_name, redis_name = arrange_resources(
+        provider, source, inference_store, is_local, is_insecure
+    )
 
     # Must clear global state to simulate two separate calls to apply;
     # otherwise, a ResourceRedefinedError is thrown
     ff.clear_state()
 
     # DESCRIPTION
     postgres_description = "This is an updated description for Provider A"
@@ -34,70 +44,90 @@
     redis_password = "password_b_updated"
 
     if is_local:
         postgres_host = "0.0.0.0"
         redis_host = "0.0.0.0"
     else:
         # The host name for postgres is different between Docker and Minikube
-        postgres_host = "host.docker.internal" if "docker" in custom_marks else "quickstart-postgres"
-        redis_host = "host.docker.internal" if "docker" in custom_marks else "quickstart-redis"
+        postgres_host = (
+            "host.docker.internal"
+            if "docker" in custom_marks
+            else "quickstart-postgres"
+        )
+        redis_host = (
+            "host.docker.internal" if "docker" in custom_marks else "quickstart-redis"
+        )
 
     postgres = ff.register_postgres(
         name=postgres_name,
         host=postgres_host,
         port="5432",
         database="postgres",
         user=postgres_username,
         password=postgres_password,
-        description=postgres_description
+        description=postgres_description,
     )
 
     redis = ff.register_redis(
         name=redis_name,
         host=redis_host,
         port=6379,
         password=redis_password,
-        description=redis_description
+        description=redis_description,
     )
 
     resource_client.apply()
 
     updated_postgres = resource_client.get_provider(postgres_name)
     updated_redis = resource_client.get_provider(redis_name)
 
-    postgres_config, redis_config = get_postgres_redis_configs(updated_postgres, updated_redis)
+    postgres_config, redis_config = get_postgres_redis_configs(
+        updated_postgres, updated_redis
+    )
 
     postgres_updates = [
         updated_postgres.description == postgres_description,
         postgres_config.Username == postgres_username,
-        postgres_config.Password == postgres_password
+        postgres_config.Password == postgres_password,
     ]
 
     redis_updates = [
         updated_redis.description == redis_description,
         redis_config.Password == redis_password,
     ]
-    
+
     assert all(postgres_updates) and all(redis_updates)
 
 
 @pytest.mark.parametrize(
     "provider_source_fxt,is_local,is_insecure",
     [
         pytest.param("local_provider_source", True, True, marks=pytest.mark.local),
-        pytest.param("hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted),
-        pytest.param("hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker),
-    ]
+        pytest.param(
+            "hosted_sql_provider_and_source", False, False, marks=pytest.mark.hosted
+        ),
+        pytest.param(
+            "hosted_sql_provider_and_source", False, True, marks=pytest.mark.docker
+        ),
+    ],
 )
-def test_invalid_provider_update(provider_source_fxt, is_local, is_insecure, request, capsys):
-    custom_marks = [mark.name for mark in request.node.own_markers if mark.name != 'parametrize']
-    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(custom_marks)
+def test_invalid_provider_update(
+    provider_source_fxt, is_local, is_insecure, request, capsys
+):
+    custom_marks = [
+        mark.name for mark in request.node.own_markers if mark.name != "parametrize"
+    ]
+    provider, source, inference_store = request.getfixturevalue(provider_source_fxt)(
+        custom_marks
+    )
 
     # Arranges the resources context following the Quickstart pattern
-    resource_client, postgres_name, redis_name = arrange_resources(provider, source, inference_store, is_local, is_insecure)
+    resource_client, postgres_name, redis_name = arrange_resources(
+        provider, source, inference_store, is_local, is_insecure
+    )
 
     # Must clear global state to simulate two separate calls to apply;
     # otherwise, a ResourceRedefinedError is thrown
     ff.clear_state()
 
     updated_postgres_host = "updated-quickstart-postgres"
     updated_postgres_database = "updated-postgres"
@@ -105,15 +135,15 @@
     postgres = ff.register_postgres(
         name=postgres_name,
         host=updated_postgres_host,
         database=updated_postgres_database,
         port="5432",
         user="postgres",
         password="password",
-        description = "A Postgres deployment we created for the Featureform quickstart"
+        description="A Postgres deployment we created for the Featureform quickstart",
     )
 
     resource_client.apply()
     out, err = capsys.readouterr()
     postgres_logs = [ln for ln in out.split("\n")]
 
     ff.clear_state()
@@ -130,23 +160,29 @@
     resource_client.apply()
     out, err = capsys.readouterr()
     redis_logs = [ln for ln in out.split("\n")]
 
     updated_postgres = resource_client.get_provider(postgres_name)
     updated_redis = resource_client.get_provider(redis_name)
 
-    postgres_config, redis_config = get_postgres_redis_configs(updated_postgres, updated_redis)
+    postgres_config, redis_config = get_postgres_redis_configs(
+        updated_postgres, updated_redis
+    )
 
     no_updates = [
         postgres_config.Host != updated_postgres_host,
         postgres_config.Database != updated_postgres_database,
         redis_config.Addr != f"{updated_redis_host}:{updated_redis_port}",
     ]
 
-    assert "postgres-quickstart already exists." in postgres_logs and  "redis-quickstart already exists." in redis_logs and all(no_updates)
+    assert (
+        "postgres-quickstart already exists." in postgres_logs
+        and "redis-quickstart already exists." in redis_logs
+        and all(no_updates)
+    )
 
 
 @pytest.fixture(autouse=True)
 def before_and_after_each(setup_teardown):
     setup_teardown()
     yield
     setup_teardown()
@@ -154,39 +190,43 @@
 
 def arrange_resources(provider, source, online_store, is_local, is_insecure):
     if is_local:
         postgres_name = "postgres-quickstart"
         redis_name = "redis-quickstart"
 
         postgres = ff.register_postgres(
-            name = "postgres-quickstart",
-            host= "0.0.0.0",
+            name="postgres-quickstart",
+            host="0.0.0.0",
             port="5432",
             user="postgres",
             password="password",
             database="postgres",
-            description = "A Postgres deployment we created for the Featureform quickstart"
+            description="A Postgres deployment we created for the Featureform quickstart",
         )
 
         redis = ff.register_redis(
-            name = "redis-quickstart",
+            name="redis-quickstart",
             host="0.0.0.0",
             port=6379,
         )
     else:
         postgres_name = provider._OfflineProvider__provider.name
         redis_name = online_store._OnlineProvider__provider.name
 
-
     resource_client = ff.ResourceClient(local=is_local, insecure=is_insecure)
     resource_client.apply()
 
     return (resource_client, postgres_name, redis_name)
 
+
 def get_postgres_redis_configs(postgres_resource, redis_resouce):
     postgres_config_json = postgres_resource.serialized_config.decode("UTF-8")
-    postgres_config = json.loads(postgres_config_json, object_hook=lambda d: SimpleNamespace(**d))
+    postgres_config = json.loads(
+        postgres_config_json, object_hook=lambda d: SimpleNamespace(**d)
+    )
 
     redis_config_json = redis_resouce.serialized_config.decode("UTF-8")
-    redis_config = json.loads(redis_config_json, object_hook=lambda d: SimpleNamespace(**d))
+    redis_config = json.loads(
+        redis_config_json, object_hook=lambda d: SimpleNamespace(**d)
+    )
 
     return (postgres_config, redis_config)
```

