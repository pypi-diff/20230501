# Comparing `tmp/MCSimPython-0.1.1.tar.gz` & `tmp/MCSimPython-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCSimPython-0.1.1.tar", last modified: Mon Apr 24 08:55:48 2023, max compression
+gzip compressed data, was "MCSimPython-0.1.2.tar", last modified: Mon May  1 10:53:07 2023, max compression
```

## Comparing `MCSimPython-0.1.1.tar` & `MCSimPython-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-04-24 08:55:32.000000 MCSimPython-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 08:55:32.000000 MCSimPython-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-24 08:55:32.000000 MCSimPython-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.990908 MCSimPython-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.990908 MCSimPython-0.1.1/src/MCSimPython/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 08:55:40.000000 MCSimPython-0.1.1/src/MCSimPython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/control/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/adaptiveFS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/backstepping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/guidance/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/guidance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/guidance/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/guidance/path_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/observer/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/ltv_kf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/nonlinobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/csad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/gunnerus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/thruster_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/vessel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/thruster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/vessel_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/freqs.npy
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/headings.npy
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/thruster_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
--rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vessel_json.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.006908 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel.json
--rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/src/MCSimPython/waves/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/wave_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/wave_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/wave_spreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.990908 MCSimPython-0.1.1/src/MCSimPython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/tests/test_wave_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-01 10:52:50.000000 MCSimPython-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-01 10:52:50.000000 MCSimPython-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-01 10:52:50.000000 MCSimPython-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 10:53:00.000000 MCSimPython-0.1.2/src/MCSimPython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/adaptiveFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/backstepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/control/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython/guidance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/guidance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/guidance/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/guidance/path_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/observer/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/ltv_kf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/observer/nonlinobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/csad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/gunnerus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/thruster_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/simulator/vessel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/thruster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27663 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/vessel_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.970147 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/freqs.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/headings.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/thruster_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vessel_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.986147 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/src/MCSimPython/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/wave_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/wave_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/src/MCSimPython/waves/wave_spreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.966147 MCSimPython-0.1.2/src/MCSimPython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 10:53:07.000000 MCSimPython-0.1.2/src/MCSimPython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:53:07.994147 MCSimPython-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-01 10:52:52.000000 MCSimPython-0.1.2/tests/test_wave_spectra.py
```

### Comparing `MCSimPython-0.1.1/LICENSE` & `MCSimPython-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/PKG-INFO` & `MCSimPython-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -44,16 +44,16 @@
 ## Demos
 
 Demonstration of how the individual components of the python package can be used is given in `demos`. Some demos of combination of the different components are also given here. 
 
 ## Visualization
 
 ### RVG 6DOF model in beam sea
-![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/wave_motion1d.gif)
-
-### RVG 6DOF model in multidirectional sea
-![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg2.gif)
+![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg_waveangle_90.gif)
 
+### RVG 6DOF model in head sea
+![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg_waveangle_180.gif)
 
+<!---
 ### CSAD 6DOF model in multidirectional sea
 ![6DOF CSAD 2D Visualisation](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d_22.gif)
-
+--->
```

### Comparing `MCSimPython-0.1.1/README.md` & `MCSimPython-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 ## Demos
 
 Demonstration of how the individual components of the python package can be used is given in `demos`. Some demos of combination of the different components are also given here. 
 
 ## Visualization
 
 ### RVG 6DOF model in beam sea
-![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/wave_motion1d.gif)
-
-### RVG 6DOF model in multidirectional sea
-![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg2.gif)
+![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg_waveangle_90.gif)
 
+### RVG 6DOF model in head sea
+![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg_waveangle_180.gif)
 
+<!---
 ### CSAD 6DOF model in multidirectional sea
 ![6DOF CSAD 2D Visualisation](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d_22.gif)
-
+--->
```

### Comparing `MCSimPython-0.1.1/pyproject.toml` & `MCSimPython-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/control/adaptiveFS.py` & `MCSimPython-0.1.2/src/MCSimPython/control/adaptiveFS.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/control/backstepping.py` & `MCSimPython-0.1.2/src/MCSimPython/control/backstepping.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/control/basic.py` & `MCSimPython-0.1.2/src/MCSimPython/control/basic.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/guidance/__init__.py` & `MCSimPython-0.1.2/src/MCSimPython/guidance/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/guidance/filter.py` & `MCSimPython-0.1.2/src/MCSimPython/guidance/filter.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/guidance/path_param.py` & `MCSimPython-0.1.2/src/MCSimPython/guidance/path_param.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/observer/__init__.py` & `MCSimPython-0.1.2/src/MCSimPython/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/observer/ekf.py` & `MCSimPython-0.1.2/src/MCSimPython/observer/ekf.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/observer/ltv_kf.py` & `MCSimPython-0.1.2/src/MCSimPython/observer/ltv_kf.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/observer/nonlinobs.py` & `MCSimPython-0.1.2/src/MCSimPython/observer/nonlinobs.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/simulator/__init__.py` & `MCSimPython-0.1.2/src/MCSimPython/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/simulator/csad.py` & `MCSimPython-0.1.2/src/MCSimPython/simulator/csad.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/simulator/gunnerus.py` & `MCSimPython-0.1.2/src/MCSimPython/simulator/gunnerus.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/simulator/thruster_dynamics.py` & `MCSimPython-0.1.2/src/MCSimPython/simulator/thruster_dynamics.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/simulator/vessel.py` & `MCSimPython-0.1.2/src/MCSimPython/simulator/vessel.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/allocation.py` & `MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/constraints.py` & `MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/constraints.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/thruster.py` & `MCSimPython-0.1.2/src/MCSimPython/thrust_allocation/thruster.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vessel_json.json` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/CSAD/vessel_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel.json` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel_2.json` & `MCSimPython-0.1.2/src/MCSimPython/vessel_data/gunnerus/vessel_2.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/waves/wave_loads.py` & `MCSimPython-0.1.2/src/MCSimPython/waves/wave_loads.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/waves/wave_spectra.py` & `MCSimPython-0.1.2/src/MCSimPython/waves/wave_spectra.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython/waves/wave_spreading.py` & `MCSimPython-0.1.2/src/MCSimPython/waves/wave_spreading.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/src/MCSimPython.egg-info/PKG-INFO` & `MCSimPython-0.1.2/src/MCSimPython.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -44,16 +44,16 @@
 ## Demos
 
 Demonstration of how the individual components of the python package can be used is given in `demos`. Some demos of combination of the different components are also given here. 
 
 ## Visualization
 
 ### RVG 6DOF model in beam sea
-![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/wave_motion1d.gif)
-
-### RVG 6DOF model in multidirectional sea
-![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg2.gif)
+![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg_waveangle_90.gif)
 
+### RVG 6DOF model in head sea
+![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg_waveangle_180.gif)
 
+<!---
 ### CSAD 6DOF model in multidirectional sea
 ![6DOF CSAD 2D Visualisation](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d_22.gif)
-
+--->
```

### Comparing `MCSimPython-0.1.1/src/MCSimPython.egg-info/SOURCES.txt` & `MCSimPython-0.1.2/src/MCSimPython.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/MCSimPython/vessel_data/CSAD/thruster_data.py
 src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
 src/MCSimPython/vessel_data/CSAD/vessel_json.json
 src/MCSimPython/vessel_data/gunnerus/__init__.py
 src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
 src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
 src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+src/MCSimPython/vessel_data/gunnerus/rvg_config.json
 src/MCSimPython/vessel_data/gunnerus/vessel.json
 src/MCSimPython/vessel_data/gunnerus/vessel_2.json
 src/MCSimPython/waves/__init__.py
 src/MCSimPython/waves/wave_loads.py
 src/MCSimPython/waves/wave_spectra.py
 src/MCSimPython/waves/wave_spreading.py
 tests/test_utils.py
```

### Comparing `MCSimPython-0.1.1/tests/test_utils.py` & `MCSimPython-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.1/tests/test_wave_spectra.py` & `MCSimPython-0.1.2/tests/test_wave_spectra.py`

 * *Files identical despite different names*

