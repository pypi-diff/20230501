# Comparing `tmp/emmet-api-0.52.1.tar.gz` & `tmp/emmet-api-0.52.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.52.1.tar", last modified: Tue Apr 25 21:19:06 2023, max compression
+gzip compressed data, was "emmet-api-0.52.2.tar", last modified: Mon May  1 19:40:13 2023, max compression
```

## Comparing `emmet-api-0.52.1.tar` & `emmet-api-0.52.2.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-25 21:19:01.000000 emmet-api-0.52.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 21:19:06.856557 emmet-api-0.52.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-25 21:19:01.000000 emmet-api-0.52.1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.828557 emmet-api-0.52.1/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.836557 emmet-api-0.52.1/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.840557 emmet-api-0.52.1/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.844557 emmet-api-0.52.1/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-25 21:19:01.000000 emmet-api-0.52.1/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 21:19:06.000000 emmet-api-0.52.1/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-04-25 21:19:06.000000 emmet-api-0.52.1/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:19:06.000000 emmet-api-0.52.1/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:19:06.000000 emmet-api-0.52.1/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-25 21:19:06.000000 emmet-api-0.52.1/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 21:19:06.000000 emmet-api-0.52.1/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-25 21:19:01.000000 emmet-api-0.52.1/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-25 21:19:01.000000 emmet-api-0.52.1/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-25 21:19:01.000000 emmet-api-0.52.1/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.848557 emmet-api-0.52.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-04-25 21:19:01.000000 emmet-api-0.52.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:19:06.856557 emmet-api-0.52.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-25 21:19:01.000000 emmet-api-0.52.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-25 21:19:01.000000 emmet-api-0.52.1/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.832557 emmet-api-0.52.1/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.832557 emmet-api-0.52.1/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.852557 emmet-api-0.52.1/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:06.856557 emmet-api-0.52.1/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-25 21:19:01.000000 emmet-api-0.52.1/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-01 19:40:07.000000 emmet-api-0.52.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 19:40:13.313458 emmet-api-0.52.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 19:40:07.000000 emmet-api-0.52.2/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.285458 emmet-api-0.52.2/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-01 19:40:13.000000 emmet-api-0.52.2/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 19:40:07.000000 emmet-api-0.52.2/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-05-01 19:40:07.000000 emmet-api-0.52.2/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-01 19:40:07.000000 emmet-api-0.52.2/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:40:13.313458 emmet-api-0.52.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-01 19:40:07.000000 emmet-api-0.52.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 19:40:07.000000 emmet-api-0.52.2/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.289458 emmet-api-0.52.2/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.289458 emmet-api-0.52.2/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.52.1/Dockerfile` & `emmet-api-0.52.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/app.py` & `emmet-api-0.52.2/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/core/api.py` & `emmet-api-0.52.2/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.52.2/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.52.2/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/core/documentation.py` & `emmet-api-0.52.2/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/core/global_header.py` & `emmet-api-0.52.2/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/core/settings.py` & `emmet-api-0.52.2/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.52.2/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.52.2/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.52.2/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.52.2/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/dois/resources.py` & `emmet-api-0.52.2/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.52.2/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.52.2/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.52.2/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.52.2/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.52.2/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.52.2/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/utils.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.52.2/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/legacy_resources.py` & `emmet-api-0.52.2/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/material_resources.py` & `emmet-api-0.52.2/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/molecule_resources.py` & `emmet-api-0.52.2/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/deployment.txt` & `emmet-api-0.52.2/requirements/deployment.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
-boto3==1.26.118
+blinker==1.6.2
+    # via flask
+boto3==1.26.123
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.29.118
+botocore==1.29.123
     # via
     #   boto3
     #   s3transfer
 bytecode==0.14.1
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
@@ -44,35 +46,35 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.12.0
+ddtrace==1.12.2
     # via emmet-api (emmet/emmet-api/setup.py)
 deprecated==1.2.13
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.52.0
+emmet-core[all]==0.52.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via cattrs
 fastapi==0.95.1
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-flask==2.2.3
+flask==2.3.2
     # via mongogrant
 fonttools==4.39.3
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
@@ -104,15 +106,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.3
+maggma==0.50.4
     # via emmet-api (emmet/emmet-api/setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -157,15 +159,15 @@
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
 opentelemetry-api==1.17.0
     # via ddtrace
-orjson==3.8.10
+orjson==3.8.11
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
@@ -197,15 +199,15 @@
     # via cffi
 pydantic==1.10.7
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
-pydash==7.0.1
+pydash==7.0.2
     # via maggma
 pymatgen==2023.3.23
     # via
     #   emmet-core
     #   matminer
     #   mp-api
     #   pymatgen-analysis-alloys
@@ -234,15 +236,15 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.28.2
+requests==2.29.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
@@ -321,15 +323,15 @@
     # via pymatgen
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (emmet/emmet-api/setup.py)
-werkzeug==2.2.3
+werkzeug==2.3.3
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.10.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.11.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.8.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.9.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.52.2/requirements/macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.52.2/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/setup.py` & `emmet-api-0.52.2/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/_consumer/test_query_operators.py` & `emmet-api-0.52.2/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/_general_store/test_query_operators.py` & `emmet-api-0.52.2/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/core/test_mapi.py` & `emmet-api-0.52.2/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.52.2/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/electrodes/test_utils.py` & `emmet-api-0.52.2/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/materials/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/materials/test_utils.py` & `emmet-api-0.52.2/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/summary/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.52.2/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.52.2/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/synthesis/test_utils.py` & `emmet-api-0.52.2/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/tasks/test_utils.py` & `emmet-api-0.52.2/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/materials/xas/test_query_operators.py` & `emmet-api-0.52.2/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.1/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.52.2/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

