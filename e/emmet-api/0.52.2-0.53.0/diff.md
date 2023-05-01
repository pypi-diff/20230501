# Comparing `tmp/emmet-api-0.52.2.tar.gz` & `tmp/emmet-api-0.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.52.2.tar", last modified: Mon May  1 19:40:13 2023, max compression
+gzip compressed data, was "emmet-api-0.53.0.tar", last modified: Mon May  1 21:34:40 2023, max compression
```

## Comparing `emmet-api-0.52.2.tar` & `emmet-api-0.53.0.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-01 19:40:07.000000 emmet-api-0.52.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 19:40:13.313458 emmet-api-0.52.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 19:40:07.000000 emmet-api-0.52.2/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.285458 emmet-api-0.52.2/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.293458 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.297458 emmet-api-0.52.2/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.301458 emmet-api-0.52.2/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-01 19:40:07.000000 emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-01 19:40:13.000000 emmet-api-0.52.2/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 19:40:12.000000 emmet-api-0.52.2/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 19:40:07.000000 emmet-api-0.52.2/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-05-01 19:40:07.000000 emmet-api-0.52.2/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-01 19:40:07.000000 emmet-api-0.52.2/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-01 19:40:07.000000 emmet-api-0.52.2/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:40:13.313458 emmet-api-0.52.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-01 19:40:07.000000 emmet-api-0.52.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 19:40:07.000000 emmet-api-0.52.2/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.289458 emmet-api-0.52.2/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.289458 emmet-api-0.52.2/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.305458 emmet-api-0.52.2/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.309458 emmet-api-0.52.2/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:13.313458 emmet-api-0.52.2/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-01 19:40:07.000000 emmet-api-0.52.2/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-01 21:34:31.000000 emmet-api-0.53.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 21:34:40.815912 emmet-api-0.53.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 21:34:31.000000 emmet-api-0.53.0/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.759912 emmet-api-0.53.0/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.767912 emmet-api-0.53.0/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.771912 emmet-api-0.53.0/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.775912 emmet-api-0.53.0/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.779912 emmet-api-0.53.0/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.779912 emmet-api-0.53.0/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.779912 emmet-api-0.53.0/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.779912 emmet-api-0.53.0/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.779912 emmet-api-0.53.0/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.779912 emmet-api-0.53.0/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.783912 emmet-api-0.53.0/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.783912 emmet-api-0.53.0/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.787912 emmet-api-0.53.0/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.791912 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.791912 emmet-api-0.53.0/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.791912 emmet-api-0.53.0/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.791912 emmet-api-0.53.0/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.791912 emmet-api-0.53.0/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.791912 emmet-api-0.53.0/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.795912 emmet-api-0.53.0/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.799912 emmet-api-0.53.0/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.799912 emmet-api-0.53.0/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-01 21:34:31.000000 emmet-api-0.53.0/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.799912 emmet-api-0.53.0/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 21:34:39.000000 emmet-api-0.53.0/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-01 21:34:40.000000 emmet-api-0.53.0/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:34:39.000000 emmet-api-0.53.0/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:34:39.000000 emmet-api-0.53.0/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 21:34:39.000000 emmet-api-0.53.0/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 21:34:39.000000 emmet-api-0.53.0/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 21:34:31.000000 emmet-api-0.53.0/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-01 21:34:31.000000 emmet-api-0.53.0/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-01 21:34:31.000000 emmet-api-0.53.0/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-05-01 21:34:31.000000 emmet-api-0.53.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:34:40.815912 emmet-api-0.53.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-01 21:34:31.000000 emmet-api-0.53.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 21:34:31.000000 emmet-api-0.53.0/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.763912 emmet-api-0.53.0/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.767912 emmet-api-0.53.0/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.803912 emmet-api-0.53.0/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.807912 emmet-api-0.53.0/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.811912 emmet-api-0.53.0/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:40.815912 emmet-api-0.53.0/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-01 21:34:31.000000 emmet-api-0.53.0/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.52.2/Dockerfile` & `emmet-api-0.53.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/app.py` & `emmet-api-0.53.0/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/core/api.py` & `emmet-api-0.53.0/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.53.0/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.53.0/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/core/documentation.py` & `emmet-api-0.53.0/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/core/global_header.py` & `emmet-api-0.53.0/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/core/settings.py` & `emmet-api-0.53.0/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.53.0/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.53.0/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.53.0/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.53.0/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/dois/resources.py` & `emmet-api-0.53.0/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.53.0/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/electrodes/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from maggma.api.query_operator import PaginationQuery, SortQuery, SparseFieldsQuery
 from emmet.api.routes.materials.electrodes.query_operators import (
     ElectrodeFormulaQuery,
     ElectrodeElementsQuery,
     ElectrodesChemsysQuery,
     WorkingIonQuery,
     ElectrodeMultiMaterialIDQuery,
-    MultiBatteryIDQuery
+    MultiBatteryIDQuery,
 )
 
 from emmet.api.core.settings import MAPISettings
 
 
 def insertion_electrodes_resource(insertion_electrodes_store):
     resource = ReadOnlyResource(
@@ -27,18 +27,19 @@
             ElectrodesChemsysQuery(),
             WorkingIonQuery(),
             ElectrodeElementsQuery(),
             NumericQuery(model=InsertionElectrodeDoc),
             SortQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
-                InsertionElectrodeDoc, default_fields=["battery_id", "last_updated"],
+                InsertionElectrodeDoc,
+                default_fields=["battery_id", "last_updated"],
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Electrodes"],
+        tags=["Materials Electrodes"],
         sub_path="/insertion_electrodes/",
         disable_validation=True,
-        timeout=MAPISettings().TIMEOUT
+        timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.53.0/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/materials/resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,55 +35,57 @@
 def find_structure_resource(materials_store):
     resource = PostOnlyResource(
         materials_store,
         FindStructure,
         key_fields=["structure", "task_id"],
         query_operators=[FindStructureQuery()],
         tags=["Materials"],
-        sub_path="/materials/find_structure/",
+        sub_path="/core/find_structure/",
         timeout=timeout,
     )
 
     return resource
 
 
 def formula_autocomplete_resource(formula_autocomplete_store):
     resource = AggregationResource(
         formula_autocomplete_store,
         FormulaAutocomplete,
         pipeline_query_operator=FormulaAutoCompleteQuery(),
         tags=["Materials"],
-        sub_path="/materials/formula_autocomplete/",
+        sub_path="/core/formula_autocomplete/",
         header_processor=GlobalHeaderProcessor(),
         timeout=timeout,
     )
 
     return resource
 
 
 def materials_resource(materials_store):
-
     resource = ReadOnlyResource(
         materials_store,
         MaterialsDoc,
         query_operators=[
             MultiMaterialIDQuery(),
             FormulaQuery(),
             ChemsysQuery(),
             ElementsQuery(),
             MultiTaskIDQuery(),
             SymmetryQuery(),
             DeprecationQuery(),
             NumericQuery(model=MaterialsDoc),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(MaterialsDoc, default_fields=["material_id", "formula_pretty", "last_updated"],),
+            SparseFieldsQuery(
+                MaterialsDoc,
+                default_fields=["material_id", "formula_pretty", "last_updated"],
+            ),
         ],
         header_processor=GlobalHeaderProcessor(),
         hint_scheme=MaterialsHintScheme(),
         tags=["Materials"],
-        sub_path="/materials/",
+        sub_path="/core/",
         disable_validation=True,
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.53.0/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.53.0/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/robocrys/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             MultiMaterialIDQuery(),
             PaginationQuery(),
             SparseFieldsQuery(
                 RobocrystallogapherDoc, default_fields=["material_id", "last_updated"]
             ),
         ],
         header_processor=GlobalHeaderProcessor(),
-        tags=["Robocrystallographer"],
+        tags=["Materials Robocrystallographer"],
         sub_path="/robocrys/",
         disable_validation=True,
         timeout=timeout,
     )
 
     return resource
```

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.53.0/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.53.0/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.53.0/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.53.0/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.53.0/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.53.0/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.53.0/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/molecules/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ElementsQuery,
     ChargeSpinQuery,
     DeprecationQuery,
     MultiTaskIDQuery,
     MultiMPculeIDQuery,
     FindMoleculeQuery,
     CalcMethodQuery,
-    HashQuery
+    HashQuery,
 )
 
 from emmet.api.core.global_header import GlobalHeaderProcessor
 from emmet.api.core.settings import MAPISettings
 
 timeout = MAPISettings().TIMEOUT
 
@@ -34,15 +34,15 @@
 def find_molecule_resource(molecules_store):
     resource = PostOnlyResource(
         molecules_store,
         FindMolecule,
         key_fields=["molecule", "molecule_id"],
         query_operators=[FindMoleculeQuery()],
         tags=["Core Molecules"],
-        sub_path="/molecules/find_molecule/",
+        sub_path="/core/find_molecule/",
         timeout=timeout,
     )
 
     return resource
 
 
 def molecules_resource(molecules_store):
@@ -58,18 +58,21 @@
             MultiTaskIDQuery(),
             CalcMethodQuery(),
             HashQuery(),
             DeprecationQuery(),
             NumericQuery(model=MoleculeDoc),
             SortQuery(),
             PaginationQuery(),
-            SparseFieldsQuery(MoleculeDoc, default_fields=["molecule_id", "formula_alphabetical", "last_updated"],),
+            SparseFieldsQuery(
+                MoleculeDoc,
+                default_fields=["molecule_id", "formula_alphabetical", "last_updated"],
+            ),
         ],
         header_processor=GlobalHeaderProcessor(),
         tags=["Core Molecules"],
-        sub_path="/molecules/",
+        sub_path="/core/",
         disable_validation=True,
         hint_scheme=MoleculesHintScheme(),
         timeout=MAPISettings().TIMEOUT,
     )
 
     return resource
```

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/utils.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.53.0/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.53.0/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/legacy_resources.py` & `emmet-api-0.53.0/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/material_resources.py` & `emmet-api-0.53.0/material_resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,122 +9,211 @@
 default_settings = MAPISettings()
 
 db_uri = os.environ.get("MPCONTRIBS_MONGO_HOST", None)
 db_version = default_settings.DB_VERSION
 db_suffix = os.environ["MAPI_DB_NAME_SUFFIX"]
 
 if db_uri:
-
     # allow db_uri to be set with a different protocol scheme
     # but prepend with mongodb+srv:// if not otherwise specified
     if len(db_uri.split("://", 1)) < 2:
         db_uri = "mongodb+srv://" + db_uri
 
     materials_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="materials"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="materials",
     )
 
     absorption_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="absorption"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="absorption",
     )
 
-    bonds_store = MongoURIStore(uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="bonds")
+    bonds_store = MongoURIStore(
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="bonds",
+    )
 
     chemenv_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="chemenv"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="chemenv",
     )
 
     formula_autocomplete_store = MongoURIStore(
-        uri=db_uri, database="mp_core", key="_id", collection_name="formula_autocomplete"
+        uri=db_uri,
+        database="mp_core",
+        key="_id",
+        collection_name="formula_autocomplete",
     )
 
-    task_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="tasks")
+    task_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="task_id", collection_name="tasks"
+    )
 
-    thermo_store = MongoURIStore(uri=db_uri, database=f"mp_core_{db_suffix}", key="thermo_id", collection_name="thermo")
+    thermo_store = MongoURIStore(
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="thermo_id",
+        collection_name="thermo",
+    )
 
     s3_phase_diagram_index = MongoURIStore(
-        uri=db_uri, database="mp_core", key="phase_diagram_id", collection_name="s3_phase_diagram_index"
+        uri=db_uri,
+        database="mp_core",
+        key="phase_diagram_id",
+        collection_name="s3_phase_diagram_index",
     )
 
     phase_diagram_store = S3Store(
         index=s3_phase_diagram_index,
         bucket="mp-phase-diagrams",
         s3_workers=24,
         key="phase_diagram_id",
         searchable_fields=["chemsys", "thermo_type", "phase_diagram_id"],
         compress=True,
     )
 
     dielectric_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="dielectric"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="dielectric",
     )
 
     piezoelectric_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="piezoelectric"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="piezoelectric",
     )
 
     magnetism_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="magnetism"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="magnetism",
     )
 
-    phonon_bs_store = MongoURIStore(uri=db_uri, database="mp_core", key="material_id", collection_name="pmg_ph_bs")
+    phonon_bs_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="material_id", collection_name="pmg_ph_bs"
+    )
 
-    eos_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="eos")
+    eos_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="task_id", collection_name="eos"
+    )
 
-    similarity_store = MongoURIStore(uri=db_uri, database="mp_core", key="material_id", collection_name="similarity")
+    similarity_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="material_id", collection_name="similarity"
+    )
 
-    xas_store = MongoURIStore(uri=db_uri, database="mp_core", key="spectrum_id", collection_name="xas")
+    xas_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="spectrum_id", collection_name="xas"
+    )
 
-    gb_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="grain_boundaries")
+    gb_store = MongoURIStore(
+        uri=db_uri,
+        database="mp_core",
+        key="task_id",
+        collection_name="grain_boundaries",
+    )
 
-    fermi_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="fermi_surface")
+    fermi_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="task_id", collection_name="fermi_surface"
+    )
 
-    elasticity_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="elasticity")
+    elasticity_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="task_id", collection_name="elasticity"
+    )
 
-    doi_store = MongoURIStore(uri=db_uri, database="mp_core", key="task_id", collection_name="dois")
+    doi_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="task_id", collection_name="dois"
+    )
 
-    substrates_store = MongoURIStore(uri=db_uri, database="mp_core", key="film_id", collection_name="substrates")
+    substrates_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="film_id", collection_name="substrates"
+    )
 
     surface_props_store = MongoURIStore(
-        uri=db_uri, database="mp_core", key="task_id", collection_name="surface_properties"
+        uri=db_uri,
+        database="mp_core",
+        key="task_id",
+        collection_name="surface_properties",
     )
 
     robo_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="robocrys"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="robocrys",
     )
 
-    synth_store = MongoURIStore(uri=db_uri, database="mp_core", key="_id", collection_name="synth_descriptions")
+    synth_store = MongoURIStore(
+        uri=db_uri, database="mp_core", key="_id", collection_name="synth_descriptions"
+    )
 
     insertion_electrodes_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="battery_id", collection_name="insertion_electrodes"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="battery_id",
+        collection_name="insertion_electrodes",
     )
 
     oxi_states_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="oxi_states"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="oxi_states",
     )
 
     provenance_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="provenance"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="provenance",
     )
 
     alloy_pairs_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="pair_id", collection_name="alloy_pairs"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="pair_id",
+        collection_name="alloy_pairs",
     )
 
     summary_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="summary"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="summary",
     )
 
     es_store = MongoURIStore(
-        uri=db_uri, database=f"mp_core_{db_suffix}", key="material_id", collection_name="electronic_structure"
+        uri=db_uri,
+        database=f"mp_core_{db_suffix}",
+        key="material_id",
+        collection_name="electronic_structure",
     )
 
-    s3_bs_index = MongoURIStore(uri=db_uri, database="mp_core", key="fs_id", collection_name="s3_bandstructure_index")
+    s3_bs_index = MongoURIStore(
+        uri=db_uri,
+        database="mp_core",
+        key="fs_id",
+        collection_name="s3_bandstructure_index",
+    )
 
-    s3_dos_index = MongoURIStore(uri=db_uri, database="mp_core", key="fs_id", collection_name="s3_dos_index")
+    s3_dos_index = MongoURIStore(
+        uri=db_uri, database="mp_core", key="fs_id", collection_name="s3_dos_index"
+    )
 
     s3_bs = S3Store(
         index=s3_bs_index,
         bucket="mp-bandstructures",
         compress=True,
         key="fs_id",
         unpack_data=False,
@@ -137,39 +226,53 @@
         compress=True,
         key="fs_id",
         unpack_data=False,
         searchable_fields=["task_id", "fs_id"],
     )
 
     s3_chgcar_index = MongoURIStore(
-        uri=db_uri, database="mp_core", key="fs_id", collection_name="atomate_chgcar_fs_index"
+        uri=db_uri,
+        database="mp_core",
+        key="fs_id",
+        collection_name="atomate_chgcar_fs_index",
     )
 
     s3_chgcar = S3Store(
         index=s3_chgcar_index,
         bucket="mp-volumetric",
         sub_dir="atomate_chgcar_fs/",
         compress=True,
         key="fs_id",
         unpack_data=False,
         searchable_fields=["task_id", "fs_id"],
     )
 
-    chgcar_url = MongoURIStore(uri=db_uri, database="mp_core", key="fs_id", collection_name="chgcar_s3_urls")
+    chgcar_url = MongoURIStore(
+        uri=db_uri, database="mp_core", key="fs_id", collection_name="chgcar_s3_urls"
+    )
 
     mpcomplete_store = MongoURIStore(
-        uri=db_uri, database="mp_consumers", key="submission_id", collection_name="mpcomplete"
+        uri=db_uri,
+        database="mp_consumers",
+        key="submission_id",
+        collection_name="mpcomplete",
     )
 
     consumer_settings_store = MongoURIStore(
-        uri=db_uri, database="mp_consumers", key="consumer_id", collection_name="settings"
+        uri=db_uri,
+        database="mp_consumers",
+        key="consumer_id",
+        collection_name="settings",
     )
 
     general_store = MongoURIStore(
-        uri=db_uri, database="mp_consumers", key="submission_id", collection_name="general_store"
+        uri=db_uri,
+        database="mp_consumers",
+        key="submission_id",
+        collection_name="general_store",
     )
 else:
     raise RuntimeError("Must specify MongoDB URI containing inputs.")
 
 # Materials
 from emmet.api.routes.materials.materials.resources import (
     find_structure_resource,
@@ -216,17 +319,22 @@
         entries_resource(task_store),
         task_deprecation_resource(materials_store),
         task_resource(task_store),
     ]
 )
 
 # Thermo
-from emmet.api.routes.materials.thermo.resources import phase_diagram_resource, thermo_resource
+from emmet.api.routes.materials.thermo.resources import (
+    phase_diagram_resource,
+    thermo_resource,
+)
 
-materials_resources.extend([phase_diagram_resource(phase_diagram_store), thermo_resource(thermo_store)])
+materials_resources.extend(
+    [phase_diagram_resource(phase_diagram_store), thermo_resource(thermo_store)]
+)
 
 # Dielectric
 from emmet.api.routes.materials.dielectric.resources import dielectric_resource
 
 materials_resources.extend([dielectric_resource(dielectric_store)])
 
 # Piezoelectric
@@ -276,31 +384,40 @@
 
 # Substrates
 from emmet.api.routes.materials.substrates.resources import substrates_resource
 
 materials_resources.extend([substrates_resource(substrates_store)])
 
 # Surface Properties
-from emmet.api.routes.materials.surface_properties.resources import surface_props_resource
+from emmet.api.routes.materials.surface_properties.resources import (
+    surface_props_resource,
+)
 
 materials_resources.extend([surface_props_resource(surface_props_store)])
 
 
 # Robocrystallographer
-from emmet.api.routes.materials.robocrys.resources import robo_resource, robo_search_resource
+from emmet.api.routes.materials.robocrys.resources import (
+    robo_resource,
+    robo_search_resource,
+)
 
-materials_resources.extend([robo_search_resource(robo_store), robo_resource(robo_store)])
+materials_resources.extend(
+    [robo_search_resource(robo_store), robo_resource(robo_store)]
+)
 
 # Synthesis
 from emmet.api.routes.materials.synthesis.resources import synth_resource
 
 materials_resources.extend([synth_resource(synth_store)])
 
 # Electrodes
-from emmet.api.routes.materials.electrodes.resources import insertion_electrodes_resource
+from emmet.api.routes.materials.electrodes.resources import (
+    insertion_electrodes_resource,
+)
 
 materials_resources.extend([insertion_electrodes_resource(insertion_electrodes_store)])
 
 # Oxidation States
 from emmet.api.routes.materials.oxidation_states.resources import oxi_states_resource
 
 materials_resources.extend([oxi_states_resource(oxi_states_store)])
@@ -312,22 +429,32 @@
 
 # Provenance
 from emmet.api.routes.materials.provenance.resources import provenance_resource
 
 materials_resources.extend([provenance_resource(provenance_store)])
 
 # Charge Density
-from emmet.api.routes.materials.charge_density.resources import charge_density_resource, charge_density_url_resource
+from emmet.api.routes.materials.charge_density.resources import (
+    charge_density_resource,
+    charge_density_url_resource,
+)
 
-materials_resources.extend([charge_density_resource(s3_chgcar), charge_density_url_resource(chgcar_url)])
+materials_resources.extend(
+    [charge_density_resource(s3_chgcar), charge_density_url_resource(chgcar_url)]
+)
 
 # Summary
-from emmet.api.routes.materials.summary.resources import summary_resource, summary_stats_resource
+from emmet.api.routes.materials.summary.resources import (
+    summary_resource,
+    summary_stats_resource,
+)
 
-materials_resources.extend([summary_stats_resource(summary_store), summary_resource(summary_store)])
+materials_resources.extend(
+    [summary_stats_resource(summary_store), summary_resource(summary_store)]
+)
 
 # Electronic Structure
 from emmet.api.routes.materials.electronic_structure.resources import (
     bs_obj_resource,
     bs_resource,
     dos_obj_resource,
     dos_resource,
@@ -348,20 +475,20 @@
 from emmet.api.routes.materials.mpcomplete.resources import mpcomplete_resource
 
 resources.update({"mpcomplete": [mpcomplete_resource(mpcomplete_store)]})
 
 # DOIs
 from emmet.api.routes.dois.resources import dois_resource
 
-resources.update({"dois": [dois_resource(doi_store)]})
+resources.update({"doi": [dois_resource(doi_store)]})
 
 # Consumers
 from emmet.api.routes._consumer.resources import settings_resource
 
 resources.update({"_user_settings": [settings_resource(consumer_settings_store)]})
 
 # General Store
 from emmet.api.routes._general_store.resources import general_store_resource
 
 resources.update({"_general_store": [general_store_resource(general_store)]})
 
-resources.update({"materials": materials_resources})
+resources.update({"materials": materials_resources})
```

### Comparing `emmet-api-0.52.2/molecule_resources.py` & `emmet-api-0.53.0/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/deployment.txt` & `emmet-api-0.53.0/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.10.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.11.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.8.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.9.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.53.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.53.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/setup.py` & `emmet-api-0.53.0/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/_consumer/test_query_operators.py` & `emmet-api-0.53.0/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/_general_store/test_query_operators.py` & `emmet-api-0.53.0/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/core/test_mapi.py` & `emmet-api-0.53.0/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.53.0/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/electrodes/test_utils.py` & `emmet-api-0.53.0/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/materials/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/materials/test_utils.py` & `emmet-api-0.53.0/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/summary/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.53.0/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.53.0/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/synthesis/test_utils.py` & `emmet-api-0.53.0/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/tasks/test_utils.py` & `emmet-api-0.53.0/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/materials/xas/test_query_operators.py` & `emmet-api-0.53.0/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.52.2/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.53.0/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

