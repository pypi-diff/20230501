# Comparing `tmp/wombato-0.0.1.tar.gz` & `tmp/wombato-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombat\dist\.tmp-ke4jugn1\wombato-0.0.1.tar", last modified: Mon May  1 06:58:35 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombat\dist\.tmp-569_oegr\wombato-0.0.2.tar", last modified: Mon May  1 07:55:48 2023, max compression
```

## Comparing `wombato-0.0.1.tar` & `wombato-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 06:58:35.000000 wombato-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombato-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      508 2023-05-01 06:58:35.000000 wombato-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-01 06:17:05.000000 wombato-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-01 06:27:55.000000 wombato-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      646 2023-05-01 06:58:35.000000 wombato-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 06:58:35.000000 wombato-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 06:58:35.000000 wombato-0.0.1/src/wombato.egg-info/
--rw-rw-rw-   0        0        0      508 2023-05-01 06:58:35.000000 wombato-0.0.1/src/wombato.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-05-01 06:58:35.000000 wombato-0.0.1/src/wombato.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 06:58:35.000000 wombato-0.0.1/src/wombato.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 06:58:35.000000 wombato-0.0.1/src/wombato.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:48.000000 wombato-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombato-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0      508 2023-05-01 07:55:48.000000 wombato-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-01 06:17:05.000000 wombato-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-01 06:27:55.000000 wombato-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-05-01 07:55:48.000000 wombato-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:48.000000 wombato-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:55:48.000000 wombato-0.0.2/src/wombato.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-05-01 07:55:48.000000 wombato-0.0.2/src/wombato.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-05-01 07:55:48.000000 wombato-0.0.2/src/wombato.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:55:48.000000 wombato-0.0.2/src/wombato.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:55:48.000000 wombato-0.0.2/src/wombato.egg-info/top_level.txt
```

### Comparing `wombato-0.0.1/LICENSE.md` & `wombato-0.0.2/LICENSE.md`

 * *Files identical despite different names*

