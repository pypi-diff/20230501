# Comparing `tmp/fsps-0.4.2rc1.tar.gz` & `tmp/fsps-0.4.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsps-0.4.2rc1.tar", last modified: Mon Sep 26 12:59:49 2022, max compression
+gzip compressed data, was "fsps-0.4.3rc1.tar", last modified: Mon May  1 10:34:45 2023, max compression
```

## Comparing `fsps-0.4.2rc1.tar` & `fsps-0.4.3rc1.tar`

### file list

```diff
@@ -1,83 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.106217 fsps-0.4.2rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-09-26 12:59:49.106217 fsps-0.4.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.102217 fsps-0.4.2rc1/demos/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/demos/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/demos/dao69.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/demos/feature_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1444 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/demos/plot_sdss_2mass_transmission.py
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/demos/specbymass.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.102217 fsps-0.4.2rc1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2230 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/scripts/fsps_filter_table.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-26 12:59:49.106217 fsps-0.4.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3165 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.098217 fsps-0.4.2rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.102217 fsps-0.4.2rc1/src/fsps/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/src/fsps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5831 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/src/fsps/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    16799 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/src/fsps/fsps.f90
--rw-r--r--   0 runner    (1001) docker     (121)    49522 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/src/fsps/fsps.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-26 12:59:49.000000 fsps-0.4.2rc1/src/fsps/fsps_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.102217 fsps-0.4.2rc1/src/fsps/libfsps/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.106217 fsps-0.4.2rc1/src/fsps/libfsps/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     4887 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/add_agb_dust.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/add_bs.f90
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/add_dust.f90
--rw-r--r--   0 runner    (1001) docker     (121)     4284 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/add_nebular.f90
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/add_remnants.f90
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/agn_dust.f90
--rw-r--r--   0 runner    (1001) docker     (121)     6449 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/attn_curve.f90
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/autosps.f90
--rw-r--r--   0 runner    (1001) docker     (121)    17238 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/compsp.f90
--rw-r--r--   0 runner    (1001) docker     (121)    14221 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/csp_gen.f90
--rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/funcint.f90
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/get_lumdist.f90
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/get_tuniv.f90
--rw-r--r--   0 runner    (1001) docker     (121)     3538 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/getindx.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/getmags.f90
--rw-r--r--   0 runner    (1001) docker     (121)     9004 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/getspec.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/igm_absorb.f90
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/imf.f90
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/imf_weight.f90
--rw-r--r--   0 runner    (1001) docker     (121)     7368 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/intsfwght.f90
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/lesssimple.f90
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/linterp.f90
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/linterparr.f90
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/locate.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/mod_gb.f90
--rw-r--r--   0 runner    (1001) docker     (121)     5619 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/mod_hb.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2796 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/pz_convol.f90
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sbf.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/setup_tabular_sfh.f90
--rw-r--r--   0 runner    (1001) docker     (121)     4603 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sfh_weight.f90
--rw-r--r--   0 runner    (1001) docker     (121)     6986 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sfhinfo.f90
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sfhlimit.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sfhstat.f90
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/simple.f90
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/smoothspec.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/spec_bin.f90
--rw-r--r--   0 runner    (1001) docker     (121)    44636 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sps_setup.f90
--rw-r--r--   0 runner    (1001) docker     (121)    11436 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sps_utils.f90
--rw-r--r--   0 runner    (1001) docker     (121)    21786 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/sps_vars.f90
--rw-r--r--   0 runner    (1001) docker     (121)     9295 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/ssp_gen.f90
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/tsum.f90
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/vacairconv.f90
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/write_isochrone.f90
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-09-26 12:59:27.000000 fsps-0.4.2rc1/src/fsps/libfsps/src/ztinterp.f90
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/src/fsps/sps_home.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.102217 fsps-0.4.2rc1/src/fsps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-09-26 12:59:49.000000 fsps-0.4.2rc1/src/fsps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-09-26 12:59:49.000000 fsps-0.4.2rc1/src/fsps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 12:59:49.000000 fsps-0.4.2rc1/src/fsps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 12:59:48.000000 fsps-0.4.2rc1/src/fsps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-26 12:59:49.000000 fsps-0.4.2rc1/src/fsps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-26 12:59:49.000000 fsps-0.4.2rc1/src/fsps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 12:59:49.106217 fsps-0.4.2rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/tests/simple_test_script.py
--rw-r--r--   0 runner    (1001) docker     (121)    10358 2022-09-26 12:58:45.000000 fsps-0.4.2rc1/tests/tests.py
+-rw-r--r--   0        0        0       24 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/.gitattributes
+-rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/.gitignore
+-rw-r--r--   0        0        0       97 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/.gitmodules
+-rw-r--r--   0        0        0      203 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/AUTHORS.rst
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/LICENSE.rst
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/README.rst
+-rw-r--r--   0        0        0        7 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/.gitignore
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/dao69.py
+-rw-r--r--   0        0        0     3952 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/feature_demo.py
+-rwxr-xr-x   0        0        0     1444 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/plot_sdss_2mass_transmission.py
+-rw-r--r--   0        0        0     6026 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/specbymass.py
+-rw-r--r--   0        0        0       37 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/.gitignore
+-rw-r--r--   0        0        0     5647 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/Makefile
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/README.rst
+-rw-r--r--   0        0        0    10307 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_static/pyfsps_logo.svg
+-rwxr-xr-x   0        0        0      340 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_templates/sidebarintro.html
+-rwxr-xr-x   0        0        0      340 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_templates/sidebarlogo.html
+-rwxr-xr-x   0        0        0     1923 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/LICENSE
+-rwxr-xr-x   0        0        0      346 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/README.rst
+-rwxr-xr-x   0        0        0      799 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/layout.html
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/localtoc.html
+-rwxr-xr-x   0        0        0      590 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/relations.html
+-rwxr-xr-x   0        0        0     8516 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/static/flasky.css_t
+-rwxr-xr-x   0        0        0      122 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/theme.conf
+-rwxr-xr-x   0        0        0     4875 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/conf.py
+-rw-r--r--   0        0        0    18397 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/filter_table.rst
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/filters.rst
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/filters_api.rst
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/index.rst
+-rw-r--r--   0        0        0     4298 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/installation.rst
+-rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/stellarpop_api.rst
+-rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/meson.build
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/noxfile.py
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/pyproject.toml
+-rw-r--r--   0        0        0        6 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/requirements.txt
+-rwxr-xr-x   0        0        0     2230 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/scripts/fsps_filter_table.py
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/__init__.py
+-rwxr-xr-x   0        0        0     5807 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/filters.py
+-rw-r--r--   0        0        0    17442 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/fsps.f90
+-rw-r--r--   0        0        0    51091 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/fsps.py
+-rw-r--r--   0        0        0      163 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/fsps_version.py
+-rw-r--r--   0        0        0      129 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/.gitignore
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/LICENSE
+-rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/README.md
+-rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/Makefile
+-rw-r--r--   0        0        0     4887 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_agb_dust.f90
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_bs.f90
+-rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_dust.f90
+-rw-r--r--   0        0        0     4284 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_nebular.f90
+-rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_remnants.f90
+-rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_xrb.f90
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/agn_dust.f90
+-rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/attn_curve.f90
+-rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/autosps.f90
+-rw-r--r--   0        0        0    17238 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/compsp.f90
+-rw-r--r--   0        0        0    14221 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/csp_gen.f90
+-rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/funcint.f90
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/get_lumdist.f90
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/get_tuniv.f90
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/getindx.f90
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/getmags.f90
+-rw-r--r--   0        0        0     9004 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/getspec.f90
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/igm_absorb.f90
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/imf.f90
+-rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/imf_weight.f90
+-rw-r--r--   0        0        0     7368 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/intsfwght.f90
+-rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/lesssimple.f90
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/linterp.f90
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/linterparr.f90
+-rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/locate.f90
+-rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/mod_gb.f90
+-rw-r--r--   0        0        0     5619 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/mod_hb.f90
+-rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/pz_convol.f90
+-rw-r--r--   0        0        0     3136 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sbf.f90
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/setup_tabular_sfh.f90
+-rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfh_weight.f90
+-rw-r--r--   0        0        0     6986 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfhinfo.f90
+-rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfhlimit.f90
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfhstat.f90
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/simple.f90
+-rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/smoothspec.f90
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/spec_bin.f90
+-rw-r--r--   0        0        0    46130 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sps_setup.f90
+-rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sps_utils.f90
+-rw-r--r--   0        0        0    22246 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sps_vars.f90
+-rw-r--r--   0        0        0     9606 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/ssp_gen.f90
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/tsum.f90
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/vacairconv.f90
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/write_isochrone.f90
+-rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/ztinterp.f90
+-rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/meson.build
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/sps_home.py
+-rw-r--r--   0        0        0      176 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tests/options.py
+-rw-r--r--   0        0        0       99 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tests/simple.py
+-rw-r--r--   0        0        0    13125 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tests/tests.py
+-rwxr-xr-x   0        0        0      660 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tools/dist.py
+-rwxr-xr-x   0        0        0      191 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tools/f2py_include.py
+-rwxr-xr-x   0        0        0      303 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tools/version.py
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/PKG-INFO
```

### Comparing `fsps-0.4.2rc1/LICENSE.rst` & `fsps-0.4.3rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/PKG-INFO` & `fsps-0.4.3rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: fsps
-Version: 0.4.2rc1
-Summary: Python bindings for Charlie Conroy's FSPS.
-Home-page: https://github.com/dfm/python-fsps
-Author: Python-FSPS developers
-Author-email: foreman.mackey@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 0.4.3rc1
+Summary: Python bindings for Charlie Conroy's FSPS
+Author-Email: Dan Foreman-Mackey <foreman.mackey@gmail.com>
+License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-License-File: LICENSE.rst
-License-File: AUTHORS.rst
+Project-URL: Homepage, https://dfm.io/python-fsps
+Project-URL: Source, https://github.com/dfm/python-fsps
+Project-URL: Bug tracker, https://github.com/dfm/python-fsps/issues
+Requires-Python: >=3.7
+Requires-Dist: numpy
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Provides-Extra: test
+Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/dfm/python-fsps/workflows/Tests/badge.svg
   :target: https://github.com/dfm/python-fsps/actions?query=workflow%3ATests
 
 **Read the documentation:**
 `dfm.io/python-fsps <https://dfm.io/python-fsps>`_
 
 If you use this code, follow the citation requirements `on the FSPS
 homepage <https://github.com/cconroy20/fsps>`_ and reference
 these Python bindings:
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.591505.svg
    :target: https://doi.org/10.5281/zenodo.591505
-
-
```

### Comparing `fsps-0.4.2rc1/demos/dao69.py` & `fsps-0.4.3rc1/demos/dao69.py`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/demos/feature_demo.py` & `fsps-0.4.3rc1/demos/feature_demo.py`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/demos/plot_sdss_2mass_transmission.py` & `fsps-0.4.3rc1/demos/plot_sdss_2mass_transmission.py`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/demos/specbymass.py` & `fsps-0.4.3rc1/demos/specbymass.py`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/scripts/fsps_filter_table.py` & `fsps-0.4.3rc1/scripts/fsps_filter_table.py`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/filters.py` & `fsps-0.4.3rc1/src/fsps/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Tools for working with the FSPS filter set.
 
 This module uses filter information shipped with FSPS itself in
 ``$SPS_HOME/data``.
 """
```

### Comparing `fsps-0.4.2rc1/src/fsps/fsps.f90` & `fsps-0.4.3rc1/src/fsps/fsps.f90`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 module driver
 
-  use sps_vars; use sps_utils
+  use sps_vars
+  use sps_utils
   implicit none
   save
 
   !f2py intent(hide) pset
   type(PARAMS) :: pset
 
   !f2py intent(hide) ocompsp
@@ -41,37 +42,38 @@
   end subroutine
 
   subroutine set_ssp_params(imf_type0,imf_upper_limit0,imf_lower_limit0,&
                             imf1,imf2,imf3,vdmc,mdave,dell,&
                             delt,sbss,fbhb,pagb,add_stellar_remnants0,&
                             tpagb_norm_type0,add_agb_dust_model0,agb_dust,&
                             redgb,agb,masscut,fcstar,evtype,use_wr_spectra0,&
-                            logt_wmb_hot0,smooth_lsf0)
+                            logt_wmb_hot0,add_xrb_emission0,frac_xrb,smooth_lsf0)
 
     ! Set the parameters that affect the SSP computation.
 
     implicit none
 
     integer, intent(in) :: imf_type0,add_stellar_remnants0,tpagb_norm_type0,&
-                           add_agb_dust_model0,use_wr_spectra0,smooth_lsf0
+                           add_agb_dust_model0,use_wr_spectra0,add_xrb_emission0,smooth_lsf0
     double precision, intent(in) :: imf_upper_limit0, imf_lower_limit0,&
                                     imf1,imf2,imf3,vdmc,mdave,dell,&
                                     delt,sbss,fbhb,pagb,agb_dust,&
                                     redgb,agb,masscut,fcstar,evtype,&
-                                    logt_wmb_hot0
+                                    logt_wmb_hot0,frac_xrb
 
     imf_type=imf_type0
     imf_upper_limit=imf_upper_limit0
     imf_lower_limit=imf_lower_limit0
     add_stellar_remnants=add_stellar_remnants0
     tpagb_norm_type=tpagb_norm_type0
     add_agb_dust_model=add_agb_dust_model0
     use_wr_spectra=use_wr_spectra0
     logt_wmb_hot=logt_wmb_hot0
     smooth_lsf=smooth_lsf0
+    add_xrb_emission=add_xrb_emission0
     pset%imf1=imf1
     pset%imf2=imf2
     pset%imf3=imf3
     pset%vdmc=vdmc
     pset%mdave=mdave
     pset%dell=dell
     pset%delt=delt
@@ -80,26 +82,27 @@
     pset%pagb=pagb
     pset%agb_dust=agb_dust
     pset%redgb=redgb
     pset%agb=agb
     pset%masscut=masscut
     pset%fcstar=fcstar
     pset%evtype=evtype
+    pset%frac_xrb=frac_xrb
 
     has_ssp(:) = 0
     has_ssp_age(:,:) = 0
 
   end subroutine
 
   subroutine set_csp_params(smooth_velocity0,redshift_colors0,&
                             compute_light_ages0,nebemlineinspec0,&
                             dust_type0,add_dust_emission0,add_neb_emission0,&
                             add_neb_continuum0,cloudy_dust0,add_igm_absorption0,&
                             zmet,sfh,wgp1,wgp2,wgp3,tau,&
-                            const,tage,fburst,tburst,dust1,dust2,&
+                            const,tage,fburst,tburst,dust1,dust2,dust3,&
                             logzsol,zred,pmetals,dust_clumps,frac_nodust,&
                             dust_index,dust_tesc,frac_obrun,uvb,mwr,&
                             dust1_index,sf_start,sf_trunc,sf_slope,&
                             duste_gamma,duste_umin,duste_qpah,&
                             sigma_smooth,min_wave_smooth,max_wave_smooth,&
                             gas_logu,gas_logz,igm_factor,fagn,agn_tau)
 
@@ -109,15 +112,15 @@
 
     integer, intent(in) :: smooth_velocity0,redshift_colors0,&
                            compute_light_ages0,nebemlineinspec0,&
                            dust_type0,add_dust_emission0,add_neb_emission0,&
                            add_neb_continuum0,cloudy_dust0,add_igm_absorption0,&
                            zmet,sfh,wgp1,wgp2,wgp3
     double precision, intent(in) :: tau,&
-                            const,tage,fburst,tburst,dust1,dust2,&
+                            const,tage,fburst,tburst,dust1,dust2,dust3,&
                             logzsol,zred,pmetals,dust_clumps,frac_nodust,&
                             dust_index,dust_tesc,frac_obrun,uvb,mwr,&
                             dust1_index,sf_start,sf_trunc,sf_slope,&
                             duste_gamma,duste_umin,duste_qpah,&
                             sigma_smooth,min_wave_smooth,max_wave_smooth,&
                             gas_logu,gas_logz,igm_factor,fagn,agn_tau
 
@@ -141,14 +144,15 @@
     pset%tau=tau
     pset%const=const
     pset%tage=tage
     pset%fburst=fburst
     pset%tburst=tburst
     pset%dust1=dust1
     pset%dust2=dust2
+    pset%dust3=dust3
     pset%logzsol=logzsol
     pset%zred=zred
     pset%pmetals=pmetals
     pset%dust_clumps=dust_clumps
     pset%frac_nodust=frac_nodust
     pset%dust_index=dust_index
     pset%dust_tesc=dust_tesc
@@ -361,14 +365,25 @@
     double precision, intent(in) :: mact, logt, lbol, logg, phase, ffco, lmdot, wght
     double precision, dimension(ns), intent(inout) :: spec_out
 
     call getspec(pset,mact,logt,lbol,logg,phase,ffco,lmdot,wght,spec_out)
 
   end subroutine
 
+  subroutine get_ssp_weights(n_age, n_z, ssp_wghts_out)
+
+    ! Return the weights of each SSP in the CSP
+
+    implicit none
+    integer, intent(in) :: n_age,n_z
+    double precision, dimension(n_age,n_z), intent(inout) :: ssp_wghts_out
+    ssp_wghts_out = weight_ssp
+
+  end subroutine
+
   subroutine get_ssp_spec(ns,n_age,n_z,ssp_spec_out,ssp_mass_out,ssp_lbol_out)
 
     ! Return the contents of the ssp spectral array,
     ! regenerating the ssps if necessary
 
     implicit none
     integer, intent(in) :: ns,n_age,n_z
@@ -395,29 +410,29 @@
     integer, intent(in) :: ntab
     double precision, dimension(ntab), intent(in) :: age, sfr, met
     ntabsfh = ntab
     sfh_tab(1,1:ntabsfh) = age
     sfh_tab(2, 1:ntabsfh) = sfr
     sfh_tab(3, 1:ntabsfh) = met
 
-  end subroutine set_sfh_tab
+  end subroutine
 
   subroutine set_ssp_lsf(nsv, sigma, wlo, whi)
 
     ! Fill the lsfinfo structure
 
     implicit none
     integer, intent(in) :: nsv
     double precision, dimension(nsv), intent(in) :: sigma
     double precision, intent(in) :: wlo, whi
     lsfinfo%minlam = wlo
     lsfinfo%maxlam = whi
     lsfinfo%lsf = sigma
 
-  end subroutine set_ssp_lsf
+  end subroutine
 
   subroutine get_setup_vars(cvms, vta_flag)
 
     implicit none
     integer, intent(out) :: cvms, vta_flag
     cvms = compute_vega_mags
     vta_flag = vactoair_flag
@@ -524,14 +539,24 @@
        lambda = vactoair(spec_lambda)
     else
        lambda = spec_lambda
     endif
 
   end subroutine
 
+  subroutine get_res(ns,res)
+
+    ! Get the resolution array of the spectral library
+    implicit none
+    integer, intent(in) :: ns
+    double precision, dimension(ns), intent(out) :: res
+    res = spec_res
+
+  end subroutine
+
   subroutine get_libraries(isocname,specname,dustname)
 
     implicit none
 
     character(4), intent(out) :: isocname
     character(5), intent(out) :: specname
     character(6), intent(out) :: dustname
```

### Comparing `fsps-0.4.2rc1/src/fsps/fsps.py` & `fsps-0.4.3rc1/src/fsps/fsps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["StellarPopulation"]
 
 import os
 import numpy as np
 
-from ._fsps import driver
-from .filters import FILTERS
+from fsps._fsps import driver
+from fsps.filters import FILTERS
 
 
 class StellarPopulation(object):
     r"""
     This is the main interface to use when interacting with FSPS from Python.
     Most of the Fortran API is exposed through Python hooks with various
     features added for user friendliness. It is recommended to only
@@ -159,14 +157,17 @@
         K. See Conroy et al. (2009a) for details and a plausible range.
 
     :param pagb: (default: 1.0)
         Weight given to the post–AGB phase. A value of 0.0 turns off post-AGB
         stars; a value of 1.0 implies that the Vassiliadis & Wood (1994) tracks
         are implemented as–is.
 
+    :param frac_xrb: (default: 1.0)
+        Scaling factor for the X-ray source spectrum to be added to the SSPs.
+
     :param zred: (default: 0.0)
         Redshift. If this value is non-zero and if ``redshift_colors=1``, the
         magnitudes will be computed for the spectrum placed at redshift
         ``zred``.
 
     :param zmet: (default: 1)
         The metallicity is specified as an integer ranging between 1 and nz. If
@@ -235,14 +236,17 @@
         Turn on/off the WR spectral library.  If off (0), will use the main
         default library instead
 
     :param logt_wmb_hot: (default: 0.0)
         Use the Eldridge (2017) WMBasic hot star library above this value of
         :math:`\log T_\mathrm{eff}` or 25,000K, whichever is larger.
 
+    :param add_xrb_emission: (default: 0)
+        Turn on/off the x-ray binary population spectra from Garofali et al.
+
     :param masscut: (default: 150.0)
         Truncate the IMF above this value.
 
     :param sigma_smooth: (default: 0.0)
         If smooth_velocity is True, this gives the velocity dispersion in km/s.
         Otherwise, it gives the width of the gaussian wavelength smoothing in
         Angstroms.  These widths are in terms of :math:`\sigma`, *not* FWHM.
@@ -348,14 +352,19 @@
         Dust parameter describing the attenuation of young stellar light,
         i.e. where ``t <= dust_tesc`` (for details, see Conroy et al. 2009a).
 
     :param dust2: (default: 0.0)
         Dust parameter describing the attenuation of old stellar light,
         i.e. where ``t > dust_tesc`` (for details, see Conroy et al. 2009a).
 
+    :param dust3: (default: 0.0)
+        Dust parameter describing extra attenuation of old stellar light that
+        does _not_ afect the young (``t < dust_tesc`` ) star light.  The
+        attenuation curve will be the one specified by ``dust_type``
+
     :param dust_clumps: (default: -99.)
         Dust parameter describing the dispersion of a Gaussian PDF density
         distribution for the old dust. Setting this value to -99.0 sets the
         distribution to a uniform screen. See Conroy et al. (2009b) for
         details.  Values other than -99 are no longer supported.
 
     :param frac_nodust: (default: 0.0)
@@ -407,25 +416,25 @@
         and a value of 1 corresponds to a clumpy distribution. See Witt &
         Gordon (2000) for details.
 
     :param duste_gamma: (default: 0.01)
         Parameter of the Draine & Li (2007) dust emission model. Specifies the
         relative contribution of dust heated at a radiation field strength of
         :math:`U_\mathrm{min}` and dust heated at :math:`U_\mathrm{min} < U \le
-        U_\mathrm{max}`. Allowable range is 0.0 – 1.0.
+        U_\mathrm{max}`. Allowable range is 0.0 - 1.0.
 
     :param duste_umin: (default: 1.0)
         Parameter of the Draine & Li (2007) dust emission model. Specifies the
         minimum radiation field strength in units of the MW value. Valid range
-        is 0.1 – 25.0.
+        is 0.1 - 25.0.
 
     :param duste_qpah: (default: 3.5)
         Parameter of the Draine & Li (2007) dust emission model. Specifies the
         grain size distribution through the fraction of grain mass in
-        PAHs. This parameter has units of % and a valid range of 0.0 − 10.0.
+        PAHs. This parameter has units of % and a valid range of 0.0 - 10.0.
 
     :param fagn: (default: 0.0)
         The total luminosity of the AGN, expressed as a fraction of the
         bolometric stellar luminosity (so it can be greater than 1). The shape
         of the AGN SED is from the Nenkova et al. 2008 templates.
 
     :param agn_tau: (default: 10)
@@ -458,14 +467,15 @@
             delt=0.0,
             redgb=1.0,
             agb=1.0,
             fcstar=1.0,
             fbhb=0.0,
             sbss=0.0,
             pagb=1.0,
+            frac_xrb=1.0,
             zred=0.0,
             zmet=1,
             logzsol=0.0,
             pmetals=2.0,
             imf_type=2,
             imf_upper_limit=120,
             imf_lower_limit=0.08,
@@ -473,14 +483,15 @@
             imf2=2.3,
             imf3=2.3,
             vdmc=0.08,
             mdave=0.5,
             evtype=-1,
             use_wr_spectra=1,
             logt_wmb_hot=0.0,
+            add_xrb_emission=0,
             masscut=150.0,
             sigma_smooth=0.0,
             min_wave_smooth=1e3,
             max_wave_smooth=1e4,
             gas_logu=-2,
             gas_logz=0.0,
             igm_factor=1.0,
@@ -493,14 +504,15 @@
             dust_tesc=7.0,
             fburst=0.0,
             tburst=11.0,
             sf_slope=0.0,
             dust_type=0,
             dust1=0.0,
             dust2=0.0,
+            dust3=0.0,
             dust_clumps=-99.0,
             frac_nodust=0.0,
             frac_obrun=0.0,
             dust_index=-0.7,
             dust1_index=-1.0,
             mwr=3.1,
             uvb=1.0,
@@ -532,14 +544,15 @@
         else:
             cvms, vtaflag = driver.get_setup_vars()
             assert compute_vega_mags == bool(cvms)
             assert vactoair_flag == bool(vtaflag)
         self._zcontinuous = zcontinuous
         # Caching.
         self._wavelengths = None
+        self._resolutions = None
         self._emwavelengths = None
         self._zlegend = None
         self._solar_metallicity = None
         self._ssp_ages = None
         self._stats = None
         self._libraries = None
 
@@ -764,14 +777,29 @@
         if peraa:
             wavegrid = self.wavelengths
             factor = 3e18 / wavegrid ** 2
             spec *= factor[:, None, None]
 
         return spec, mass, lbol
 
+    def _ssp_weights(self):
+         """Get the weights of the SSPs for the CSP
+
+         :returns weights:
+             The weights ``w`` of each SSP s.t. the total spectrum is the sum
+             :math:`L_{\lambda} = \sum_i,j w_i,j \, S_{i,j,\lambda}` where
+             math:`i,j` run over age and metallicity.
+         """
+
+         NTFULL = driver.get_ntfull()
+         NZ = driver.get_nz()
+         weights = np.zeros([NTFULL, NZ], order="F")
+         driver.get_ssp_weights(weights)
+         return weights
+
     def _get_stellar_spectrum(
         self,
         mact,
         logt,
         lbol,
         logg,
         phase,
@@ -876,15 +904,15 @@
         with open(absfile, "r") as f:
             # drop the comment hash and mags field
             header = f.readline().split()[1:-1]
         header += list_filters()
         cmd_data = np.loadtxt(
             absfile,
             comments="#",
-            dtype=np.dtype([(n, np.float) for n in header]),
+            dtype=np.dtype([(n, float) for n in header]),
         )
         return cmd_data
 
     def set_tabular_sfh(self, age, sfr, Z=None):
         r"""
         Set a tabular SFH for use with the ``sfh=3`` option.  See the FSPS
         documentation for information about tabular SFHs.  This SFH will be
@@ -1031,14 +1059,24 @@
         r"""The wavelength scale for the computed spectra, in Angstroms"""
         if self._wavelengths is None:
             NSPEC = driver.get_nspec()
             self._wavelengths = driver.get_lambda(NSPEC)
         return self._wavelengths.copy()
 
     @property
+    def resolutions(self):
+        r"""The resolution array, in km/s dispersion. Negative numbers indicate
+         poorly defined, approximate, resolution (based on coarse opacity
+         binning in theoretical spectra)"""
+        if self._resolutions is None:
+            NSPEC = driver.get_nspec()
+            self._resolutions = driver.get_res(NSPEC)
+        return self._resolutions.copy()
+
+    @property
     def emline_wavelengths(self):
         r"""Emission line wavelengths, in Angstroms"""
         if self._emwavelengths is None:
             NLINE = driver.get_nemline()
             self._emwavelengths = driver.get_emlambda(NLINE)
         return self._emwavelengths.copy()
 
@@ -1228,14 +1266,16 @@
         "redgb",
         "agb",
         "masscut",
         "fcstar",
         "evtype",
         "use_wr_spectra",
         "logt_wmb_hot",
+        "add_xrb_emission",
+        "frac_xrb",
         "smooth_lsf",
     ]
 
     csp_params = [
         "smooth_velocity",
         "redshift_colors",
         "compute_light_ages",
@@ -1254,14 +1294,15 @@
         "tau",
         "const",
         "tage",
         "fburst",
         "tburst",
         "dust1",
         "dust2",
+        "dust3",
         "logzsol",
         "zred",
         "pmetals",
         "dust_clumps",
         "frac_nodust",
         "dust_index",
         "dust_tesc",
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/Makefile` & `fsps-0.4.3rc1/src/fsps/libfsps/src/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 PROGS = simple lesssimple autosps spec_bin
 
 COMMON = sps_vars.o sps_utils.o compsp.o csp_gen.o ssp_gen.o \
 	getmags.o locate.o funcint.o sps_setup.o pz_convol.o \
 	get_tuniv.o intsfwght.o imf.o imf_weight.o add_dust.o \
 	getspec.o sbf.o add_bs.o mod_hb.o add_remnants.o getindx.o \
-	smoothspec.o mod_gb.o add_nebular.o write_isochrone.o \
+	smoothspec.o mod_gb.o add_nebular.o add_xrb.o write_isochrone.o \
 	sfhstat.o linterp.o tsum.o add_agb_dust.o linterparr.o \
 	ztinterp.o vacairconv.o igm_absorb.o get_lumdist.o attn_curve.o \
 	sfh_weight.o sfhlimit.o sfhinfo.o setup_tabular_sfh.o agn_dust.o
 
 all : $(PROGS)
 
 clean :
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/add_agb_dust.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/add_agb_dust.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/add_bs.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/add_bs.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/add_dust.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/add_dust.f90`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,52 @@
 SUBROUTINE ADD_DUST(pset,csp1,csp2,specdust,mdust,ncsp1,ncsp2,nebdust)
 
+  ! Inputs
+  ! ---------
+  !
+  ! pset:
+  !   A `PARAMS` structure containing the dust parameters
+  !
+  !  csp1:
+  !   The spectrum of the young stars
+  !
+  !  csp2:
+  !   The spectrum of the old stars
+  !
+  !  ncsp1:
+  !   The nebular fluxes for the young stars
+  !
+  !  ncsp2:
+  !   The nebular fluxes for the old stars
+  !
+  ! Outputs
+  ! ---------
+  !
+  ! specdust:
+  !  The combined spectrum including dust attenuation and dust emission
+  !
+  ! nebdust:
+  !   The combined nebular emission line fluxes including dust absorption
+  !
+  ! mdust:
+  !  The dust mass required to produce the absorbed luminosity for the given dust emission parameters
+
+
   USE sps_vars
   USE sps_utils, ONLY : tsum, locate, attn_curve, linterparr
   IMPLICIT NONE
 
   REAL(SP), DIMENSION(nspec), INTENT(in) :: csp1,csp2
   TYPE(PARAMS), INTENT(in) :: pset
   REAL(SP), DIMENSION(nspec), INTENT(out) :: specdust
   REAL(SP), INTENT(out) :: mdust
   REAL(SP), DIMENSION(nemline), INTENT(in) :: ncsp1,ncsp2
   REAL(SP), DIMENSION(nemline), INTENT(out) :: nebdust
   INTEGER :: i,qlo,ulo,iself=0
-  REAL(SP), DIMENSION(nspec)  :: diff_dust,tau2,cspi
+  REAL(SP), DIMENSION(nspec)  :: diff_dust,tau_diff,cspi
   REAL(SP), DIMENSION(nemline)  :: diff_dust_neb,ncspi
   REAL(SP), DIMENSION(nspec)  :: nu,dumin,dumax
   REAL(SP), DIMENSION(nspec)  :: mduste,duste,oduste,sduste,tduste
   REAL(SP) :: clump_ave,lboln,lbold,labs,gamma,norm,dq,du
 
   !---------------------------------------------------------------!
   !----------------------Test input params------------------------!
@@ -49,44 +80,53 @@
   ENDIF
 
   !---------------------------------------------------------------!
   !----------------------Add dust absorption----------------------!
   !---------------------------------------------------------------!
 
   !compute attenuation curve for diffuse dust
-  diff_dust = EXP(-attn_curve(spec_lambda,dust_type,pset))
- 
+  tau_diff = attn_curve(spec_lambda,dust_type,pset)
+
   !combine old and young stars, attenuating the young
   !with a fixed power-law attn curve, and allowing a fraction
   !of the young stars to be dust-free ("OB runaways")
+  !and an extra attenuation towards old stars (patchy dust)
   cspi = csp1 * EXP(-pset%dust1*(spec_lambda/5500.)**(pset%dust1_index))*&
-       (1-pset%frac_obrun) + csp1*pset%frac_obrun + csp2
-  
+       (1-pset%frac_obrun) + csp1*pset%frac_obrun + &
+       csp2 * EXP(-pset%dust3*tau_diff)
+
+  !normalize diffuse dust curve unless Witt & Gordon
+  IF (dust_type.EQ.3) THEN
+    diff_dust = EXP(-tau_diff)
+  ELSE
+    diff_dust = EXP(-pset%dust2 * tau_diff)
+  ENDIF
+
   !allow a fraction of the diffuse dust spectrum to be dust-free
-  specdust  = cspi*diff_dust*(1-pset%frac_nodust) + &
-       cspi*pset%frac_nodust
+  specdust  = (1-pset%frac_nodust) * cspi*diff_dust + &
+               cspi*pset%frac_nodust
 
   !as above, for nebular line luminosities
   diff_dust_neb = linterparr(spec_lambda,diff_dust,nebem_line_pos)
   ncspi = ncsp1 * EXP(-pset%dust1*(nebem_line_pos/5500.)**(pset%dust1_index))*&
        (1-pset%frac_obrun) + ncsp1*pset%frac_obrun + ncsp2
   nebdust  = ncspi*diff_dust_neb*(1-pset%frac_nodust) + &
        ncspi*pset%frac_nodust
 
   !---------------------------------------------------------------!
   !----------------------Add dust emission------------------------!
   !---------------------------------------------------------------!
-  
+
   ! The dust spectrum is computed according to Draine & Li 2007
   ! we are computing the integral of the dust spectrum over P(U)dU
-  ! by considering two components, a delta function at Umin and 
+  ! by considering two components, a delta function at Umin and
   ! a power-law distribution from Umin to Umax=1E6 and alpha=2
   ! the relative weights of the two components are given by gamma
-  
-  IF (add_dust_emission.EQ.1) THEN 
+
+  IF (add_dust_emission.EQ.1) THEN
 
      !only add dust emission if there is absorption
      IF (pset%dust2.GT.tiny_number.OR.pset%dust1.GT.tiny_number) THEN
 
         iself=0
         !compute Lbol both before and after dust attenuation
         !this will determine the normalization of the dust emission
@@ -97,15 +137,15 @@
            lboln = lboln + SUM(ncsp1) + SUM(ncsp2) - SUM(nebdust)
         ENDIF
 
         !set up qpah interpolation
         qlo = MAX(MIN(locate(qpaharr,pset%duste_qpah),nqpah_dustem-1),1)
         dq  = (pset%duste_qpah-qpaharr(qlo))/(qpaharr(qlo+1)-qpaharr(qlo))
         dq  = MIN(MAX(dq,0.0),1.0)  !no extrapolation
-        
+
         !set up Umin interpolation
         !set limits on Umin: 0.1<Umin<25.0
         ulo = MAX(MIN(locate(uminarr,pset%duste_umin),numin_dustem),1)
         du  = (pset%duste_umin-uminarr(ulo))/(uminarr(ulo+1)-uminarr(ulo))
         du  = MIN(MAX(du,0.0),1.0)  !no extrapolation
 
         !set limits to gamma (gamma is a fraction)
@@ -137,32 +177,32 @@
         !will re-emit and be re-absorbed, etc.
         tduste = 0.0
         DO WHILE (((lboln-lbold).GT.1E-2).OR.iself.EQ.0)
 
            oduste = duste
            duste  = duste * diff_dust
            tduste = tduste + duste
-           
+
            lbold = TSUM(nu,duste)  !after  self-abs
            lboln = TSUM(nu,oduste) !before self-abs
 
            duste = MAX(mduste/norm*(lboln-lbold),tiny_number)
-           
+
            iself=1
 
         ENDDO
 
         !this factor assumes Md/Mh=0.01 (appropriate for the 
         !MW3.1 models), and includes conversion factors from 
         !Jy -> Lsun and the hydrogen mass in solar units
         mdust = 3.21E-3 / 4/mypi * labs/norm
 
         !add the dust emission to the stellar spectrum
         specdust = specdust + tduste
-        
+
      ELSE
         mdust = tiny_number
      ENDIF
 
   ENDIF
 
 END SUBROUTINE ADD_DUST
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/add_nebular.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/add_nebular.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/add_remnants.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/add_remnants.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/agn_dust.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/agn_dust.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/attn_curve.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/attn_curve.f90`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 FUNCTION ATTN_CURVE(lambda,dtype,pset)
 
-  ! Routine to generate and return the attenuation curve for a chosen 
-  ! dust type.  The V-band optical depth (dust2) is passed via the 
-  ! pset variable.  Option 3 (Witt & Gordon models) do not use the
-  ! dust2 option as those grids fully predict the actual attn curves.
+  ! Routine to generate and return the attenuation curve for a chosen dust type.
+  ! The V-band optical depth is 1 unless option 3 (Witt & Gordon models) is
+  ! selected as those grids fully predict the actual attn curves.
 
   USE sps_vars
   USE sps_utils, ONLY : locate
   IMPLICIT NONE
 
   INTEGER, INTENT(in) :: dtype
   TYPE(PARAMS), INTENT(in) :: pset
+  REAL(SP) :: tauv=1.0
   INTEGER  :: w63,w1,w2
   REAL(SP) :: eb,zero=0.0,dd63=6300.00,lamv=5500.0,dlam=350.0,lamuvb=2175.0
   REAL(SP), INTENT(in), DIMENSION(nspec) :: lambda
   REAL(SP), DIMENSION(nspec) :: x,a,b,y,fa,fb,hack,cal00,reddy
   REAL(SP), DIMENSION(nspec) :: attn_curve,drude,tmp
- 
+
   !---------------------------------------------------------------------!
 
   attn_curve = 0.0
 
   IF (dtype.LT.0.OR.dtype.GT.6) THEN
      WRITE(*,*) 'ATTN_CURVE ERROR: dust_type out of range:',dtype
      STOP
   ENDIF
-  
+
   !-------------------------power-law attenuation-----------------------!
 
   !power-law attenuation
-  IF (dtype.EQ.0) THEN 
+  IF (dtype.EQ.0) THEN
 
-     attn_curve = (lambda/lamv)**pset%dust_index * pset%dust2
+     attn_curve = (lambda/lamv)**pset%dust_index * tauv
 
   !-----------------CCM89 MW curve w/ variable UV bump------------------!
 
   !MW extinction law w/ UV bump
-  ELSE IF (dtype.EQ.1) THEN 
+  ELSE IF (dtype.EQ.1) THEN
 
      tmp = 0.0
 
      !use CCM89 extinction curve parameterization
      x = 1E4/lambda
      y = x-1.82
 
@@ -95,75 +95,75 @@
 
      !set to a constant at lambda < 12 um^-1
      a = -1.073-0.628*(12.-8.)+0.137*(12.-8.)**2-0.070*(12.-8.)**3
      b = 13.67+4.257*(12.-8.)-0.42*(12.-8.)**2+0.374*(12.-8.)**3
      tmp(:mwdindex(6)) = &
           a(:mwdindex(6)) + b(:mwdindex(6))/pset%mwr
 
-     attn_curve = pset%dust2*tmp
+     attn_curve = tauv*tmp
 
 
   !------------------Calzetti et al. 2000 attenuation-------------------!
 
-  ELSE IF (dtype.EQ.2) THEN 
+  ELSE IF (dtype.EQ.2) THEN
 
      w63   = locate(lambda,dd63)
      cal00 = 0.0
      cal00(w63+1:) = 1.17*( -1.857+1.04*(1E4/lambda(w63+1:)) ) + 1.78
      cal00(1:w63)  = 1.17*(-2.156+1.509*(1E4/lambda(1:w63))-&
           0.198*(1E4/lambda(1:w63))**2 + &
           0.011*(1E4/lambda(1:w63))**3) + 1.78
      cal00 = cal00/0.44/4.05  !R=4.05
      w63   = locate(cal00,zero)
      IF (w63.NE.nspec) THEN
         cal00(w63+1:) = 0.0
      ENDIF
- 
-     attn_curve = cal00 * pset%dust2
+
+     attn_curve = cal00 * tauv
 
   !------------------Witt & Gordon 2000 attenuation--------------------!
 
   ELSE IF (dtype.EQ.3) THEN
-  
+
      attn_curve = wgdust(:,pset%wgp1,pset%wgp2,pset%wgp3)
 
   !------------------Kriek & Conroy 2013 attenuation-------------------!
 
   ELSE IF (dtype.EQ.4) THEN
 
      !Calzetti curve
      w63   = locate(lambda,dd63)
      cal00 = 0.0
      cal00(w63+1:) = 1.17*( -1.857+1.04*(1E4/lambda(w63+1:)) ) + 1.78
      cal00(1:w63)  = 1.17*(-2.156+1.509*(1E4/lambda(1:w63))-&
           0.198*(1E4/lambda(1:w63))**2 + &
           0.011*(1E4/lambda(1:w63))**3) + 1.78
      !R=4.05 NB: I'm not sure I have this normalization correct...
-     cal00 = cal00/0.44/4.05 
+     cal00 = cal00/0.44/4.05
      w63   = locate(cal00,zero)
      IF (w63.NE.nspec) THEN
         cal00(w63+1:) = 0.0
      ENDIF
 
      eb = 0.85 - 1.9 * pset%dust_index  !KC13 Eqn 3
 
      !Drude profile for 2175A bump
      drude = eb*(lambda*dlam)**2 / &
           ( (lambda**2-lamuvb**2)**2 + (lambda*dlam)**2 )
 
-     attn_curve = pset%dust2*(cal00+drude/4.05)*&
+     attn_curve = tauv*(cal00+drude/4.05)*&
           (lambda/lamv)**pset%dust_index
 
 
   !-----------------Gordon et al. (2003) SMC exctincion----------------!
 
   ELSE IF (dtype.EQ.5) THEN
 
-     attn_curve = pset%dust2*g03smcextn
-     
+     attn_curve = tauv*g03smcextn
+
   !------------------Reddy et al. (2015) attenuation-------------------!
 
   ELSE IF (dtype.EQ.6) THEN
 
      reddy = 0.0
 
      ! see Eqn. 8 in Reddy et al. (2015)
@@ -181,13 +181,13 @@
      ! two functions continuous at 0.6um
      reddy(w1:w2) = -2.672 - 0.010/(lambda(w1:w2)/1E4) + 1.532/(lambda(w1:w2)/1E4)**2 + &
           -0.412/(lambda(w1:w2)/1E4)**3 + 2.505 - 0.036221981
 
      ! convert k_lam to A_lam/A_V assuming Rv=2.505
      reddy = reddy/2.505
 
-     attn_curve = pset%dust2*reddy
+     attn_curve = tauv*reddy
      
   ENDIF
 
 
 END FUNCTION ATTN_CURVE
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/autosps.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/autosps.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/compsp.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/compsp.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/csp_gen.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/csp_gen.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/funcint.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/funcint.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/get_lumdist.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/get_lumdist.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/get_tuniv.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/get_tuniv.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/getindx.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/getindx.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/getmags.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/getmags.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/getspec.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/getspec.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/igm_absorb.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/igm_absorb.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/imf.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/imf.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/imf_weight.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/imf_weight.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/intsfwght.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/intsfwght.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/lesssimple.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/lesssimple.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/linterp.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/linterp.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/linterparr.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/linterparr.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/locate.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/locate.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/mod_gb.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/mod_gb.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/mod_hb.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/mod_hb.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/pz_convol.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/pz_convol.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sbf.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sbf.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/setup_tabular_sfh.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/setup_tabular_sfh.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sfh_weight.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sfh_weight.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sfhinfo.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sfhinfo.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sfhlimit.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sfhlimit.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sfhstat.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sfhstat.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/simple.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/simple.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/smoothspec.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/smoothspec.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/spec_bin.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/spec_bin.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sps_setup.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sps_setup.f90`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   INTEGER, PARAMETER :: nzwmb=12, nspec_wmb=5508
   INTEGER :: n_isoc,z,zmin,zmax,nlam
   CHARACTER(1) :: char,sqpah
   CHARACTER(6) :: zstype
   CHARACTER(5) :: zstype5
   REAL(SP) :: dumr1,d1,d2,logage,x,a,zero=0.0,d,one=1.0,dz,dlam
   CHARACTER(5), DIMENSION(nz) :: zlegend_str=''
+  CHARACTER(5), DIMENSION(nz_xrb) :: zz_str_xrb=''
   REAL(SP), DIMENSION(nspec) :: tspec=0.
   REAL(SP), DIMENSION(ntlam) :: tvega_lam=0.,tvega_spec=0.
   REAL(SP), DIMENSION(ntlam) :: tsun_lam=0.,tsun_spec=0.
   REAL(SP), DIMENSION(nlamwr) :: tlamwr=0.,tspecwr=0.
   REAL(SP), DIMENSION(nlamwr,ndim_wr,5) :: twrc=0.,twrn=0.
   REAL(SP), DIMENSION(5) :: twrzmet=0.
   REAL(SP), DIMENSION(50000) :: readlamb=0.,readband=0.
@@ -43,21 +44,23 @@
   REAL(SP), DIMENSION(nspec_agb)  :: agb_lam=0.0
   REAL(SP), DIMENSION(nspec_aringer)  :: aringer_lam=0.0
   REAL(SP), DIMENSION(nspec_agb,n_agb_o) :: agb_specinit_o=0.
   REAL(SP), DIMENSION(nspec_agb,n_agb_c) :: agb_specinit_c=0.
   REAL(SP), DIMENSION(nspec_aringer,n_agb_car) :: aringer_specinit=0.
   REAL(SP), DIMENSION(nagndust_spec)           :: agndust_lam=0.
   REAL(SP), DIMENSION(nagndust_spec,nagndust)  :: agndust_specinit=0.
-  REAL(KIND(1.0)), DIMENSION(nspec,nzinit,ndim_logt,ndim_logg) :: speclibinit=0.
+  !REAL(KIND(1.0)), DIMENSION(nspec,nzinit,ndim_logt,ndim_logg) :: speclibinit=0.
+  REAL(KIND(1.0)), allocatable :: speclibinit(:,:,:,:)
   REAL(SP), DIMENSION(nspec,nzwmb,ndim_wmb_logt,ndim_wmb_logg) :: wmbsi=0.
   REAL(SP), DIMENSION(nzwmb)     :: zwmb=0.
   REAL(SP), DIMENSION(nspec_wmb) :: wmb_lam=0.
   REAL(SP), DIMENSION(nspec_wmb,ndim_wmb_logt,ndim_wmb_logg) :: wmb_specinit=0.
   REAL(SP), DIMENSION(ntabmax)   :: lsflam=0.,lsfsig=0.
   REAL(SP), DIMENSION(30) :: g03lam=0., g03smc=0.
+  REAL(SP), DIMENSION(nspec_xrb) :: tspec_xrb
   
   !---------------------------------------------------------------!
   !---------------------------------------------------------------!
 
   IF (verbose.EQ.1) THEN 
      WRITE(*,*) 
      WRITE(*,*) '    Setting up SPS...'
@@ -218,15 +221,15 @@
   
   !read in wavelength array and spectral metallicity grid
   IF (spec_type.EQ.'basel') THEN
      OPEN(91,FILE=TRIM(SPS_HOME)//'/SPECTRA/BaSeL3.1/basel.lambda',&
           STATUS='OLD',iostat=stat,ACTION='READ')
      OPEN(93,FILE=TRIM(SPS_HOME)//'/SPECTRA/BaSeL3.1/zlegend.dat',&
           STATUS='OLD',iostat=stat,ACTION='READ')
-     OPEN(94,FILE=TRIM(SPS_HOME)//'SPECTRA/BaSeL3.1/basel.res',&
+     OPEN(94,FILE=TRIM(SPS_HOME)//'/SPECTRA/BaSeL3.1/basel.res',&
           STATUS='OLD',iostat=stat,ACTION='READ')
   ELSE IF (spec_type.EQ.'miles') THEN
      OPEN(91,FILE=TRIM(SPS_HOME)//'/SPECTRA/MILES/miles.lambda',&
           STATUS='OLD',iostat=stat,ACTION='READ')
      OPEN(93,FILE=TRIM(SPS_HOME)//'/SPECTRA/MILES/zlegend.dat',&
           STATUS='OLD',iostat=stat,ACTION='READ')
      OPEN(94,FILE=TRIM(SPS_HOME)//'/SPECTRA/MILES/miles.res',&
@@ -244,18 +247,20 @@
      STOP 
   ENDIF
   DO i=1,nspec
      READ(91,*) spec_lambda(i)
   ENDDO
   CLOSE(91)
 
+  !read in spectral resolution
   DO i=1,nspec
      READ(94,*) spec_res(i)
   ENDDO
-  CLOSE(94)  
+  CLOSE(94)
+  
   !read in primary logg and logt arrays
   !NB: these are the same for all spectral libraries
   OPEN(91,FILE=TRIM(SPS_HOME)//'/SPECTRA/BaSeL3.1/basel_logt.dat',&
        STATUS='OLD',iostat=stat,ACTION='READ')
   DO i=1,ndim_logt
      READ(91,*) speclib_logt(i)
   ENDDO
@@ -263,14 +268,17 @@
   OPEN(91,FILE=TRIM(SPS_HOME)//'/SPECTRA/BaSeL3.1/basel_logg.dat',&
        STATUS='OLD',iostat=stat,ACTION='READ')
   DO i=1,ndim_logg
      READ(91,*) speclib_logg(i)
   ENDDO
   CLOSE(91)
 
+  ALLOCATE(speclibinit(nspec,nzinit,ndim_logt,ndim_logg))
+  speclibinit = 0.0
+  
   !read in each metallicity
   DO z=1,nzinit
 
      READ(93,*) zlegendinit(z)
      WRITE(zstype,'(F6.4)') zlegendinit(z)
 
      !read in the spectral library
@@ -317,14 +325,16 @@
 
      speclib(:,z,:,:) = (1-dz)*LOG10(speclibinit(:,i1,:,:)+tiny_number) + &
           dz*LOG10(speclibinit(:,i1+1,:,:)+tiny_number)
      speclib(:,z,:,:) = 10**speclib(:,z,:,:)
 
   ENDDO
 
+  DEALLOCATE(speclibinit)
+  
   !--------------Read WMBasic Grid from JJ Eldridge----------------;
 
   !read in Teff array
   OPEN(93,FILE=TRIM(SPS_HOME)//'/SPECTRA/Hot_spectra/WMBASIC.teff',&
        STATUS='OLD',iostat=stat,ACTION='READ')
   IF (stat.NE.0) THEN
      WRITE(*,*) 'SPS_SETUP ERROR: /SPECTRA/Hot_spectra/'//&
@@ -875,15 +885,15 @@
   i1 = locate(spec_lambda,agndust_lam(1))
   i2 = locate(spec_lambda,agndust_lam(nagndust_spec))
   DO i=1,nagndust
      agndust_spec(i1:i2,i) = 10**linterparr(LOG10(agndust_lam),&
           LOG10(agndust_specinit(:,i)+tiny30),LOG10(spec_lambda(i1:i2)))-tiny30
   ENDDO
 
-
+  
   !----------------------------------------------------------------!
   !----------------Set up nebular emission arrays------------------!
   !----------------------------------------------------------------!
 
   IF (isoc_type.EQ.'mist'.OR.isoc_type.EQ.'pdva'.OR.&
      isoc_type.EQ.'prsc'.OR.isoc_type.EQ.'bpss') THEN
   
@@ -972,15 +982,56 @@
                 EXP(-(spec_lambda-nebem_line_pos(i))**2/2/dlam**2)  / &
                 clight*nebem_line_pos(i)**2
         ENDDO
      ENDIF
 
   ENDIF
 
- 
+
+  !----------------------------------------------------------------!
+  !------------------Set up X-ray binary arrays--------------------!
+  !----------------------------------------------------------------!
+
+  OPEN(98,FILE=TRIM(SPS_HOME)//'/SPECTRA/xrb/xsp.lambda',&
+       STATUS='OLD',iostat=stat,ACTION='READ')
+  IF (stat.NE.0) THEN
+     WRITE(*,*) 'SPS_SETUP ERROR: xsp.lambda cannot be opened'
+     STOP 
+  ENDIF  
+
+  DO i=1,nspec_xrb
+     READ(98,*) lam_xrb(i)
+  ENDDO
+
+  CLOSE(98)
+
+  ages_xrb = LOG10((/1.0,3.0,5.0,8.0,10.0,15.0,20.0/))+6.0
+  zmet_xrb = (/-2.0,-1.0,0.0/)
+
+  zz_str_xrb = (/'-2.00','-1.00','+0.00'/)
+
+  DO j=1,3
+     OPEN(98,FILE=TRIM(SPS_HOME)//'/SPECTRA/xrb/xsp_feh'//zz_str_xrb(j)&
+          //'.spec',STATUS='OLD',iostat=stat,ACTION='READ')
+     IF (stat.NE.0) THEN
+        WRITE(*,*) 'SPS_SETUP ERROR: xsp_feh'//zz_str_xrb(j)//&
+             '.spec cannot be opened'
+        STOP 
+     ENDIF
+     DO i=1,nt_xrb
+        READ(98,*) tspec_xrb
+        !interpolate to the main wavelength array
+        spec_xrb(:,i,j) = MAX(linterparr(lam_xrb,tspec_xrb,spec_lambda),tiny_number)
+     ENDDO
+     CLOSE(98)
+  ENDDO
+
+  !convert to Lsun/Hz/Msun
+  spec_xrb = spec_xrb * lsun
+  
   !----------------------------------------------------------------!
   !-------------------Set up magnitude info------------------------!
   !----------------------------------------------------------------!
 
   !read in Vega-like star (lambda, Flambda)
   !(this is actually a Kurucz (1992) model for Vega)
   OPEN(98,FILE=TRIM(SPS_HOME)//'/SPECTRA/A0V_KURUCZ_92.SED',&
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sps_utils.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sps_utils.f90`

 * *Files 4% similar despite different names*

```diff
@@ -37,19 +37,27 @@
   INTERFACE
      SUBROUTINE ADD_NEBULAR(pset,sspi,sspo,nebemline)
        USE sps_vars
        TYPE(PARAMS), INTENT(in) :: pset
        REAL(SP), INTENT(in), DIMENSION(nspec,ntfull)    :: sspi
        REAL(SP), INTENT(inout), DIMENSION(nspec,ntfull) :: sspo
        REAL(SP), INTENT(inout), DIMENSION(nemline,ntfull), OPTIONAL :: nebemline
-
      END SUBROUTINE ADD_NEBULAR
   END INTERFACE
 
   INTERFACE
+     SUBROUTINE ADD_XRB(pset,sspi,sspo)
+       USE sps_vars
+       TYPE(PARAMS), INTENT(in) :: pset
+       REAL(SP), INTENT(in), DIMENSION(nspec,ntfull)    :: sspi
+       REAL(SP), INTENT(inout), DIMENSION(nspec,ntfull) :: sspo
+     END SUBROUTINE ADD_XRB
+  END INTERFACE
+
+  INTERFACE
      SUBROUTINE ADD_REMNANTS(mass,maxmass)
        USE sps_vars
        REAL(SP), INTENT(inout) :: mass
        REAL(SP), INTENT(in) :: maxmass
      END SUBROUTINE ADD_REMNANTS
   END INTERFACE
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/sps_vars.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/sps_vars.f90`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,17 @@
   INTEGER  :: add_neb_continuum=1
   !include dust in the Cloudy tables or not
   INTEGER :: cloudy_dust=0
 
   !turn on/off IGM absorption a la Madau (1995)
   INTEGER :: add_igm_absorption=0
 
+  !turn on/off the X-ray binary (ULX) model from Garofali et al. (in prep)
+  INTEGER :: add_xrb_emission=0
+
   !turn on/off the addition of stellar remnants to the
   !computation of stellar masses
   INTEGER :: add_stellar_remnants=1
 
   !if set, use a simpler, algorithm to smooth
   !the spectra.  Accurate to ~0.1% and somewhat faster than the
   !correct approach.  NB: one should be careful when choosing
@@ -283,15 +286,15 @@
   !number of indices defined in allindices.dat
   INTEGER, PARAMETER :: nindx=30
 
   !The following parameters should never be changed
   !unless you are changing the libraries
 
   !max dimension of array for each isochrone
-  INTEGER, PARAMETER :: nm=2000  !10000
+  INTEGER, PARAMETER :: nm=2000
   !max number of lines to read in
   INTEGER, PARAMETER ::  nlines=1000000
   !max number of lines in tabulated SFH, LSF
   INTEGER, PARAMETER :: ntabmax=20000
   !dimensions of BaSeL library
   INTEGER, PARAMETER :: ndim_logt=68, ndim_logg=19
   !number of O-rich, C-rich AGB spectra (and Aringer C-rich spec)
@@ -309,14 +312,18 @@
   !number of metallicity, age, and ionization parameter points
   INTEGER, PARAMETER :: nebnz=11, nebnage=10, nebnip=7
   !number of optical depths for AGN dust models
   INTEGER, PARAMETER :: nagndust=9
   !number of spectral points in the input library
   INTEGER, PARAMETER :: nagndust_spec=125
 
+  INTEGER, PARAMETER :: nspec_xrb=15000
+  INTEGER, PARAMETER :: nt_xrb=7
+  INTEGER, PARAMETER :: nz_xrb=3
+  
   !------------IMF-related Constants--------------!
 
   !Salpeter IMF index
   REAL(SP) :: salp_ind= 2.35
   !min/max masses for the IMF
   REAL(SP) :: imf_lower_limit = 0.08, imf_upper_limit=120.
   REAL(SP) :: imf_lower_bound
@@ -535,28 +542,34 @@
   !array for ssp weights
   REAL(SP), DIMENSION(ntfull,nz)       :: weight_ssp=0.
 
   !array for full BPASS SSPs
   REAL(SP), DIMENSION(nspec,nt,nz) :: bpass_spec_ssp=0.
   REAL(SP), DIMENSION(nt,nz)       :: bpass_mass_ssp=0.
 
+  !arrays for X-ray binaries
+  REAL(SP), DIMENSION(nspec_xrb) :: lam_xrb=0.
+  REAL(SP), DIMENSION(nspec,nt_xrb,nz_xrb) :: spec_xrb=0.
+  REAL(SP), DIMENSION(nt_xrb) :: ages_xrb=0.0
+  REAL(SP), DIMENSION(nz_xrb) :: zmet_xrb=0.0
+  
   !------------Define TYPE structures-------------!
 
   !structure for the set of parameters necessary to generate a model
   TYPE PARAMS
      REAL(SP) :: pagb=1.0,dell=0.,delt=0.,fbhb=0.,sbss=0.,tau=1.0,&
           const=0.,tage=0.,fburst=0.,tburst=11.0,dust1=0.,dust2=0.,&
           logzsol=0.,zred=0.,pmetals=0.02,imf1=1.3,imf2=2.3,imf3=2.3,&
           vdmc=0.08,dust_clumps=-99.,frac_nodust=0.,dust_index=-0.7,&
           dust_tesc=7.0,frac_obrun=0.,uvb=1.0,mwr=3.1,redgb=1.0,agb=1.0,&
           dust1_index=-1.0,mdave=0.5,sf_start=0.,sf_trunc=0.,sf_slope=0.,&
           duste_gamma=0.01,duste_umin=1.0,duste_qpah=3.5,fcstar=1.0,&
           masscut=150.0,sigma_smooth=0.,agb_dust=1.0,min_wave_smooth=1E3,&
           max_wave_smooth=1E4,gas_logu=-2.0,gas_logz=0.,igm_factor=1.0,&
-          fagn=0.0,agn_tau=10.0
+          fagn=0.0,agn_tau=10.0,frac_xrb=1.0,dust3=0.
      INTEGER :: zmet=1,sfh=0,wgp1=1,wgp2=1,wgp3=1,evtype=-1
      INTEGER, DIMENSION(nbands) :: mag_compute=1
      INTEGER, DIMENSION(nt) :: ssp_gen_age=1
      CHARACTER(50) :: imf_filename='', sfh_filename=''
   END TYPE PARAMS
 
   !structure for the output of the compsp routine
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/ssp_gen.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/ssp_gen.f90`

 * *Files 6% similar despite different names*

```diff
@@ -240,14 +240,23 @@
 
   IF (add_neb_emission.EQ.2) THEN
      CALL ADD_NEBULAR(pset,spec_ssp,tspec_ssp)
      spec_ssp = tspec_ssp
   ENDIF
 
   !-------------------------------------------------------------!
+  !---------------add X-ray binaries the SSP level--------------!
+  !-------------------------------------------------------------!
+
+  IF (add_xrb_emission.EQ.1) THEN
+     CALL ADD_XRB(pset,spec_ssp,tspec_ssp)
+     spec_ssp = tspec_ssp
+  ENDIF
+
+  !-------------------------------------------------------------!
   !--------now smooth by an instrumental LSF if provided--------!
   !-------------------------------------------------------------!
 
   IF (smooth_lsf.EQ.1) THEN
      DO j=1,ntfull
         CALL SMOOTHSPEC(spec_lambda,spec_ssp(:,j),99.d0,lsfinfo%minlam,&
              lsfinfo%maxlam,lsfinfo%lsf)
```

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/tsum.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/tsum.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/vacairconv.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/vacairconv.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/write_isochrone.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/write_isochrone.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/libfsps/src/ztinterp.f90` & `fsps-0.4.3rc1/src/fsps/libfsps/src/ztinterp.f90`

 * *Files identical despite different names*

### Comparing `fsps-0.4.2rc1/src/fsps/sps_home.py` & `fsps-0.4.3rc1/src/fsps/sps_home.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 __all__ = ["check_sps_home"]
 
 import os
 
 
 def check_sps_home():
     if "SPS_HOME" not in os.environ:
```

### Comparing `fsps-0.4.2rc1/tests/tests.py` & `fsps-0.4.3rc1/tests/tests.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
-import subprocess
-
 import numpy as np
 import pytest
-from numpy.testing import assert_allclose
-
 from fsps import StellarPopulation, filters
+from numpy.testing import assert_allclose
 
-
-def test_fortran_error():
-    output = subprocess.check_output(
-        [
-            sys.executable,
-            os.path.join(
-                os.path.dirname(os.path.abspath(__file__)), "simple_test_script.py"
-            ),
-        ]
-    )
-    assert output.decode("ascii").strip() == "success"
+skip_slow_tests = pytest.mark.skipif(
+    (sys.platform.startswith("win") or sys.platform.startswith("darwin"))
+    and "CI" in os.environ,
+    reason="Slow tests only run on Linux CI",
+)
 
 
 @pytest.fixture(scope="module")
 def pop_and_params():
     pop = StellarPopulation(zcontinuous=1)
     params = dict([(k, pop.params[k]) for k in pop.params.all_params])
     return pop, params
@@ -32,40 +23,58 @@
 
 def _reset_default_params(pop, params):
     pop._zcontinuous = 1
     for k in pop.params.all_params:
         pop.params[k] = params[k]
 
 
-def _get_model(pop, theta):
-    pop.params["imf3"] = theta
-    assert pop.params.dirtiness == 2
-    return pop.get_spectrum(tage=0.2)[1]
+@skip_slow_tests
+def test_isochrones(pop_and_params):
+    """Just test that `isochrones()` method runs"""
 
+    # recomputes SSPs
 
-# def test_imf3_multiprocessing():
-#     from multiprocessing import Pool
-#     pool = Pool()
-#     thetas = np.linspace(2.3, 8.3, 4)
-#     single = map(_get_model, thetas)
-#     multi = pool.map(_get_model, thetas)
-#     assert_allclose(single, multi)
+    pop, params = pop_and_params
+    _reset_default_params(pop, params)
+    pop.params["imf_type"] = 0
+    iso = pop.isochrones()
 
 
-def test_libraries(pop_and_params):
-    """This does not require or build clean SSPs"""
+@skip_slow_tests
+def test_imf3(pop_and_params):
+    """Make sure that changing the (upper) imf changes the parameter dirtiness
+    and also the SSP spectrum"""
+
+    # recomputes SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
-    ilib, splib, dlib = pop.libraries
-    assert ilib == pop.isoc_library
-    assert splib == pop.spec_library
-    assert dlib == pop.duste_library
+    pop.params["imf_type"] = 2
+    pop.params["imf3"] = 2.3
+    w, model1 = pop.get_spectrum(tage=0.2)
+
+    # check that changing the IMF does something
+    pop.params["imf3"] = 8.3
+    assert pop.params.dirtiness == 2
+    w, model2 = pop.get_spectrum(tage=0.2)
+    assert not np.allclose(model1 / model2 - 1.0, 0.0)
+
+    # Do we *really* need to do this second check?
+    pop.params["imf3"] = 2.3
+    assert pop.params.dirtiness == 2
+    w, model1b = pop.get_spectrum(tage=0.2)
+    assert pop.params.dirtiness == 0
+
+    assert_allclose(model1 / model1b - 1.0, 0.0)
 
 
 def test_param_checks(pop_and_params):
+
+    # recomputes SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 1
     pop.params["tage"] = 2
     pop.params["sf_start"] = 0.5
     # this should never raise an error:
     w, s = pop.get_spectrum(tage=pop.params["tage"])
@@ -78,51 +87,154 @@
     with pytest.raises(AssertionError):
         w, s = pop.get_spectrum(tage=pop.params["tage"])
     pop.params["tage"] = 1.0
     pop.params["sf_start"] = 0.1
     w, s = pop.get_spectrum(tage=pop.params["tage"])
 
 
-def test_filters():
-    """Test all the filters got transmission data loaded."""
-    flist = filters.list_filters()
-    # force trans cache to load
-    filters.FILTERS[flist[0]]._load_transmission_cache()
-    for f in flist:
-        assert f in filters.TRANS_CACHE, "transmission not loaded for {}".format(f)
+def test_smooth_lsf(pop_and_params):
+
+    # recomputes SSPs
+
+    pop, params = pop_and_params
+    _reset_default_params(pop, params)
+    tmax = 1.0
+    wave_lsf = np.arange(4000, 7000.0, 10)
+    x = (wave_lsf - 5500) / 1500.0
+    # a quadratic lsf dependence that goes from ~50 to ~100 km/s
+    sigma_lsf = 50 * (1.0 + 0.4 * x + 0.6 * x**2)
+    w, spec = pop.get_spectrum(tage=tmax)
+    pop.params["smooth_lsf"] = True
+    assert pop.params.dirtiness == 2
+    pop.set_lsf(wave_lsf, sigma_lsf)
+    w, smspec = pop.get_spectrum(tage=tmax)
+    hi = w > 7100
+    sm = (w < 7000) & (w > 3000)
+    assert np.allclose(spec[hi] / smspec[hi] - 1.0, 0.0)
+    assert not np.allclose(spec[sm] / smspec[sm] - 1.0, 0.0)
+    pop.set_lsf(wave_lsf, sigma_lsf * 2)
+    assert pop.params.dirtiness == 2
+
+
+@skip_slow_tests
+def test_tabular(pop_and_params):
+    """Test that you get the right shape spectral arrays for tabular SFHs, that
+    the parameter dirtiness is appropriately managed for changing tabular SFH,
+    and that multi-metallicity SFH work."""
+
+    # uses default SSPs, but makes them for every metallicity
+
+    pop, params = pop_and_params
+    _reset_default_params(pop, params)
+
+    import os
+
+    fn = os.path.join(os.environ["SPS_HOME"], "data/sfh.dat")
+    age, sfr, z = np.genfromtxt(fn, unpack=True, skip_header=0)
+
+    # Mono-metallicity
+    pop.params["sfh"] = 3
+    pop.set_tabular_sfh(age, sfr)
+    w, spec = pop.get_spectrum(tage=0)
+    pop.set_tabular_sfh(age, sfr)
+    assert pop.params.dirty
+    w, spec = pop.get_spectrum(tage=0)
+    assert spec.shape[0] == len(pop.ssp_ages)
+    assert pop.params["sfh"] == 3
+    w, spec_last = pop.get_spectrum(tage=-99)
+    assert spec_last.ndim == 1
+    w, spec = pop.get_spectrum(tage=age.max())
+    assert np.allclose(spec / spec_last - 1.0, 0.0)
+    pop.params["logzsol"] = -1
+    w, spec_lowz = pop.get_spectrum(tage=age.max())
+    assert not np.allclose(spec / spec_lowz - 1.0, 0.0)
+
+    # test the formed mass for single age
+    assert np.allclose(np.trapz(sfr, age) * 1e9, pop.formed_mass)
+
+    # Multi-metallicity
+    pop._zcontinuous = 3
+    pop.set_tabular_sfh(age, sfr, z)
+    w, spec_multiz = pop.get_spectrum(tage=age.max())
+    assert not np.allclose(spec_lowz / spec_multiz - 1.0, 0.0)
+
+    pop._zcontinuous = 1
+    pop.set_tabular_sfh(age, sfr)
+    # get mass weighted metallicity
+    mbin = np.gradient(age) * sfr
+    mwz = (z * mbin).sum() / mbin.sum()
+    pop.params["logzsol"] = np.log10(mwz / pop.solar_metallicity)
+    w, spec_onez = pop.get_spectrum(tage=age.max())
+    assert not np.allclose(spec_onez / spec_multiz - 1.0, 0.0)
 
 
 def test_get_mags(pop_and_params):
     """Basic test for supplying filter names to get_mags"""
+
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     fuv1 = pop.get_mags(bands=["galex_fuv"])[:, 0]
     mags = pop.get_mags()
     fuv2 = mags[:, 61]  # this should be galex_FUV
     fuv3 = mags[:, 62]  # this should *not* be galex_FUV
     assert np.all(fuv1 == fuv2)
     assert np.all(fuv1 != fuv3)
 
 
 def test_ssp(pop_and_params):
+    """Test that you get a sensible wavelength array, and that you get a
+    sensible V-band magnitude for a 1-Gyr SSP"""
+
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 0
     wave, spec = pop.get_spectrum(tage=1, peraa=True)
     assert (wave[0] > 0) & (wave[0] < wave[-1]) & (wave[0] < 912.0)
     assert (wave[-1] > 1e6) & (wave[-1] < 1e10)
     Mv = 4.62  # AB absolute magnitude for a Zsol 1Gyr old SSP
     # This also tests get_mags
     mag = pop.get_mags(tage=1, bands=["v"])
     assert np.all(abs(mag - Mv) < 1.0)
     assert np.all((pop.stellar_mass < 1.0) & (pop.stellar_mass > 0))
     assert pop.params.dirtiness == 0
 
 
+def test_libraries(pop_and_params):
+    """This does not require or build clean SSPs"""
+
+    # uses default SSPs
+
+    pop, params = pop_and_params
+    _reset_default_params(pop, params)
+    ilib, splib, dlib = pop.libraries
+    assert ilib == pop.isoc_library
+    assert splib == pop.spec_library
+    assert dlib == pop.duste_library
+
+
+def test_filters():
+    """Test all the filters got transmission data loaded."""
+
+    # uses default SSPs
+
+    flist = filters.list_filters()
+    # force trans cache to load
+    filters.FILTERS[flist[0]]._load_transmission_cache()
+    for f in flist:
+        assert f in filters.TRANS_CACHE, "transmission not loaded for {}".format(f)
+
+
 def test_csp_dirtiness(pop_and_params):
+    """Make sure that changing CSP parameters increases dirtiness to 1"""
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 1
     pop.params["tau"] = 1.0
     wave, spec = pop.get_spectrum(tage=1.0)
     assert pop.params.dirtiness == 0
     pop.params["tau"] = 3.0
@@ -130,14 +242,17 @@
 
 
 def test_redshift(pop_and_params):
     """Test redshifting, make sure that
     1. redshifting does not persist in cached arrays
     2. specifying redshift via get_mags keyword or param key are consistent
     """
+
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 0
     pop.params["zred"] = 0.0
     pop.params["add_igm_absorption"] = False
     v1 = pop.get_mags(redshift=1.0, tage=1.0, bands=["v"])
     v2 = pop.get_mags(redshift=1.0, tage=1.0, bands=["v"])
@@ -149,16 +264,48 @@
     v5 = pop.get_mags(redshift=0.0, tage=1.0, bands=["v"])
     assert np.all(v3 == v4)
 
     assert np.all(v3 == v1)
     assert np.all(v5 != v4)
 
 
+def test_dust3(pop_and_params):
+    """Make sure nebular lines are actually added."""
+
+    # uses default SSPs
+
+    pop, params = pop_and_params
+    _reset_default_params(pop, params)
+    pop.params["sfh"] = 4
+    pop.params["dust_type"] = 4
+    pop.params["tau"] = 5.0
+    pop.params["dust1"] = 0
+    pop.params["dust2"] = 0.5
+
+    # make sure dust3 affects the population when there are old stars
+    pop.params["dust3"] = 0.0
+    mag1 = pop.get_mags(tage=1.0, bands=["u", "b"])
+    pop.params["dust3"] = 1.0
+    mag2 = pop.get_mags(tage=1.0, bands=["u", "b"])
+    assert np.all(mag2 > mag1)
+
+    # make sure the dust3 isn't affecting young populations
+    pop.params["dust_tesc"] = 8
+    pop.params["dust3"] = 0.0
+    mag3 = pop.get_mags(tage=0.05, bands=["u", "b"])
+    pop.params["dust3"] = 1.0
+    mag4 = pop.get_mags(tage=0.05, bands=["u", "b"])
+    assert_allclose(mag3, mag4)
+
+
 def test_nebemlineinspec(pop_and_params):
     """Make sure nebular lines are actually added."""
+
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 4
     pop.params["tau"] = 5.0
     pop.params["add_neb_emission"] = True
     pop.params["nebemlineinspec"] = False
     wave, spec_neboff = pop.get_spectrum(tage=1.0)
@@ -168,27 +315,35 @@
     assert np.all(np.isfinite(pop.emline_luminosity))
     assert np.all(np.isfinite(pop.emline_wavelengths))
     ha_idx = (wave > 6556) & (wave < 6573)
     assert (spec_nebon - spec_neboff)[ha_idx].sum() > 0
 
 
 def test_mformed(pop_and_params):
+    """Make sure formed mass integrates to 1 for parameteric SFH"""
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 1
     pop.params["const"] = 0.5
     w, s = pop.get_spectrum(tage=0)
     assert pop.formed_mass[-1] == 1
     assert pop.formed_mass[50] < 1.0
     assert pop.formed_mass[50] > 0.0
     w, s = pop.get_spectrum(tage=0)
     assert pop.formed_mass[-1] == 1.0
 
 
 def test_light_ages(pop_and_params):
+    """Make sure light weighting works, and gives sensible answers for the
+    light-weighted age in the FUV and mass-weighted age stored in
+    `stellar_mass`"""
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     tmax = 5.0
     pop.params["sfh"] = 1
     pop.params["const"] = 0.5
     w, spec = pop.get_spectrum(tage=tmax)
     mstar = pop.stellar_mass
@@ -205,118 +360,63 @@
     assert pop.stellar_mass < tmax
     # luminosity weighted age always less than mass-weighted age
     # assert pop.log_lbol < pop.stellar_mass
 
 
 def test_smoothspec(pop_and_params):
     # FIXME: This is not very stringent
+
+    # uses default SSPs
+
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     wave, spec = pop.get_spectrum(tage=1, peraa=True)
     spec2 = pop.smoothspec(wave, spec, 160.0, minw=1e3, maxw=1e4)
     assert (spec - spec2 == 0.0).sum() > 0
 
 
-def test_imf3(pop_and_params):
-    pop, params = pop_and_params
-    _reset_default_params(pop, params)
-    pop.params["imf_type"] = 2
-    pop.params["imf3"] = 2.3
-    w, model1 = pop.get_spectrum(tage=0.2)
+@skip_slow_tests
+def test_ssp_weights(pop_and_params):
+    """Check that weights dotted into ssp is the same as the returned spectrum
+    when there's no dust or emission lines and zcontinuous=0"""
 
-    # check that changing the IMF does something
-    pop.params["imf3"] = 8.3
-    assert pop.params.dirtiness == 2
-    w, model2 = pop.get_spectrum(tage=0.2)
-    assert not np.allclose(model1 / model2 - 1.0, 0.0)
-
-    # Do we *really* need to do this second check?
-    pop.params["imf3"] = 2.3
-    assert pop.params.dirtiness == 2
-    w, model1b = pop.get_spectrum(tage=0.2)
-    assert pop.params.dirtiness == 0
+    # uses default SSPs
 
-    assert_allclose(model1 / model1b - 1.0, 0.0)
-
-
-def test_tabular(pop_and_params):
     pop, params = pop_and_params
     _reset_default_params(pop, params)
 
     import os
-
     fn = os.path.join(os.environ["SPS_HOME"], "data/sfh.dat")
     age, sfr, z = np.genfromtxt(fn, unpack=True, skip_header=0)
-
-    # Mono-metallicity
     pop.params["sfh"] = 3
     pop.set_tabular_sfh(age, sfr)
-    w, spec = pop.get_spectrum(tage=0)
-    pop.set_tabular_sfh(age, sfr)
-    assert pop.params.dirty
-    w, spec = pop.get_spectrum(tage=0)
-    assert spec.shape[0] == len(pop.ssp_ages)
-    assert pop.params["sfh"] == 3
-    w, spec_last = pop.get_spectrum(tage=-99)
-    assert spec_last.ndim == 1
-    w, spec = pop.get_spectrum(tage=age.max())
-    assert np.allclose(spec / spec_last - 1.0, 0.0)
-    pop.params["logzsol"] = -1
-    w, spec_lowz = pop.get_spectrum(tage=age.max())
-    assert not np.allclose(spec / spec_lowz - 1.0, 0.0)
-
-    # Multi-metallicity
-    pop._zcontinuous = 3
-    pop.set_tabular_sfh(age, sfr, z)
-    w, spec_multiz = pop.get_spectrum(tage=age.max())
-    assert not np.allclose(spec_lowz / spec_multiz - 1.0, 0.0)
-
-    pop._zcontinuous = 1
-    pop.set_tabular_sfh(age, sfr)
-    # get mass weighted metallicity
-    mbin = np.gradient(age) * sfr
-    mwz = (z * mbin).sum() / mbin.sum()
-    pop.params["logzsol"] = np.log10(mwz / 0.019)
-    w, spec_onez = pop.get_spectrum(tage=age.max())
-    assert not np.allclose(spec_onez / spec_multiz - 1.0, 0.0)
-
-
-def test_isochrones(pop_and_params):
-    # Just test that `isochrones()` method runs
-    pop, params = pop_and_params
-    _reset_default_params(pop, params)
-    pop.params["imf_type"] = 0
-    iso = pop.isochrones()
+    zind = -3
+    pop.params["logzsol"] = np.log10(pop.zlegend[zind]/pop.solar_metallicity)
 
+    wave, spec = pop.get_spectrum(tage=age.max())
+    mstar = pop.stellar_mass
+    wght = pop._ssp_weights()
+    ssp, smass, slbol = pop._all_ssp_spec()
 
-def test_smooth_lsf(pop_and_params):
-    pop, params = pop_and_params
-    _reset_default_params(pop, params)
-    tmax = 1.0
-    wave_lsf = np.arange(4000, 7000.0, 10)
-    x = (wave_lsf - 5500) / 1500.0
-    # a quadratic lsf dependence that goes from ~50 to ~100 km/s
-    sigma_lsf = 50 * (1.0 + 0.4 * x + 0.6 * x ** 2)
-    w, spec = pop.get_spectrum(tage=tmax)
-    pop.params["smooth_lsf"] = True
-    assert pop.params.dirtiness == 2
-    pop.set_lsf(wave_lsf, sigma_lsf)
-    w, smspec = pop.get_spectrum(tage=tmax)
-    hi = w > 7100
-    sm = (w < 7000) & (w > 3000)
-    assert np.allclose(spec[hi] / smspec[hi] - 1.0, 0.0)
-    assert not np.allclose(spec[sm] / smspec[sm] - 1.0, 0.0)
-    pop.set_lsf(wave_lsf, sigma_lsf * 2)
-    assert pop.params.dirtiness == 2
+    assert np.allclose((smass[:, zind] * wght[:, 0]).sum(), mstar)
 
 
 # Requires scipy
 # def test_sfr_avg():
 
 #    _reset_default_params()
 #    pop.params['sfh'] = 1.0
 #    pop.params['const'] = 0.5
 #    w, spec = pop.get_spectrum(tage=0)
 #    sfr6 = pop.sfr_avg(dt=1e-3)
 #    dsfr = np.log10(pop.sfr/pop.sfr6)
 #    good = pop.ssp_age > 6
 #    assert np.all(np.abs(dsfr[good]) < 1e-2)
+
+
+# def test_imf3_multiprocessing():
+#     from multiprocessing import Pool
+#     pool = Pool()
+#     thetas = np.linspace(2.3, 8.3, 4)
+#     single = map(_get_model, thetas)
+#     multi = pool.map(_get_model, thetas)
+#     assert_allclose(single, multi)
```

