# Comparing `tmp/napari_animation-0.0.5.tar.gz` & `tmp/napari_animation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_animation-0.0.5.tar", last modified: Sat Nov 12 17:21:06 2022, max compression
+gzip compressed data, was "napari_animation-0.0.6.tar", last modified: Mon May  1 14:39:31 2023, max compression
```

## Comparing `napari_animation-0.0.5.tar` & `napari_animation-0.0.6.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.572070 napari_animation-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.564069 napari_animation-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.568070 napari_animation-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-11-12 17:20:55.000000 napari_animation-0.0.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-11-12 17:20:55.000000 napari_animation-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-12 17:20:55.000000 napari_animation-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-11-12 17:20:55.000000 napari_animation-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-12 17:20:55.000000 napari_animation-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-11-12 17:21:06.572070 napari_animation-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4468 2022-11-12 17:20:55.000000 napari_animation-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-12 17:20:55.000000 napari_animation-0.0.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.568070 napari_animation-0.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-11-12 17:20:55.000000 napari_animation-0.0.5/examples/animate2D.py
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-11-12 17:20:55.000000 napari_animation-0.0.5/examples/animate3D.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-11-12 17:20:55.000000 napari_animation-0.0.5/examples/animateMixed.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-12 17:20:55.000000 napari_animation-0.0.5/examples/interactive_animation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.568070 napari_animation-0.0.5/napari_animation/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.568070 napari_animation-0.0.5/napari_animation/_qt/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.568070 napari_animation-0.0.5/napari_animation/_qt/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/_tests/test_animation_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     6876 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/animation_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/frame_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/keyframelistcontrol_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/keyframeslist_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     4401 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_qt/savedialog_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.572070 napari_animation-0.0.5/napari_animation/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/test_animation.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/test_easing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/test_frame_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8201 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/animation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8221 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/easing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4756 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/frame_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.572070 napari_animation-0.0.5/napari_animation/interpolation/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/interpolation/base_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/interpolation/interpolation_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/interpolation/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/interpolation/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/interpolation/viewer_state_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/key_frame.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-11-12 17:20:55.000000 napari_animation-0.0.5/napari_animation/viewer_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.568070 napari_animation-0.0.5/napari_animation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5501 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-12 17:21:06.000000 napari_animation-0.0.5/napari_animation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-11-12 17:20:55.000000 napari_animation-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-12 17:20:55.000000 napari_animation-0.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 17:21:06.572070 napari_animation-0.0.5/resources/
--rw-r--r--   0 runner    (1001) docker     (121)   607232 2022-11-12 17:20:55.000000 napari_animation-0.0.5/resources/screenshot-animation-widget.png
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-11-12 17:21:06.572070 napari_animation-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-12 17:20:55.000000 napari_animation-0.0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-11-12 17:20:55.000000 napari_animation-0.0.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.703702 napari_animation-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.695701 napari_animation-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.695701 napari_animation-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-01 14:39:12.000000 napari_animation-0.0.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-01 14:39:12.000000 napari_animation-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-01 14:39:12.000000 napari_animation-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-01 14:39:12.000000 napari_animation-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 14:39:12.000000 napari_animation-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-01 14:39:31.703702 napari_animation-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-01 14:39:12.000000 napari_animation-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 14:39:12.000000 napari_animation-0.0.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.695701 napari_animation-0.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/animate2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/animate3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/animateMixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/ease_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/interactive_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:39:12.000000 napari_animation-0.0.6/examples/programmatic_notebook_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/_qt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/_tests/test_animation_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/animation_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/frame_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/keyframelistcontrol_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/keyframeslist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_qt/savedialog_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_easing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_frame_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/easing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/frame_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/base_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/interpolation_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/interpolation/viewer_state_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/key_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-01 14:39:12.000000 napari_animation-0.0.6/napari_animation/viewer_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/napari_animation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 14:39:31.000000 napari_animation-0.0.6/napari_animation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-01 14:39:12.000000 napari_animation-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 14:39:12.000000 napari_animation-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:39:31.699702 napari_animation-0.0.6/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   607232 2023-05-01 14:39:12.000000 napari_animation-0.0.6/resources/screenshot-animation-widget.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-01 14:39:31.703702 napari_animation-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 14:39:12.000000 napari_animation-0.0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 14:39:12.000000 napari_animation-0.0.6/tox.ini
```

### Comparing `napari_animation-0.0.5/.github/workflows/test_and_deploy.yml` & `napari_animation-0.0.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/.gitignore` & `napari_animation-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/.pre-commit-config.yaml` & `napari_animation-0.0.6/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 repos:
 -   repo: https://github.com/pycqa/isort
-    rev: 5.7.0
+    rev: 5.12.0
     hooks:
     - id: isort
       exclude: _vendor|vendored|examples 
 -   repo: https://github.com/python/black
     rev: 22.3.0
     hooks:
     - id: black
       pass_filenames: true
       exclude: _vendor|vendored|examples
--   repo: https://gitlab.com/pycqa/flake8
+-   repo: https://github.com/PyCQA/flake8
     rev: 3.8.4
     hooks:
     - id: flake8
       pass_filenames: true
       # this seems to need to be here in addition to setup.cfg
       exclude: _vendor|vendored|__init__.py|examples
 -   repo: https://github.com/asottile/pyupgrade
```

### Comparing `napari_animation-0.0.5/LICENSE` & `napari_animation-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/PKG-INFO` & `napari_animation-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_animation
-Version: 0.0.5
+Version: 0.0.6
 Summary: A plugin for making animations in napari
 Home-page: https://github.com/napari/napari-animation
 Download-URL: https://github.com/napari/napari-animation
 Author: Nicholas Sofroniew, Alister Burt, Guillaume Witz, Faris Abouakil, Talley Lambert
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -36,14 +36,18 @@
 
 <p align="center">
   <img width="500" src="https://user-images.githubusercontent.com/7307488/196110138-6c4663b1-67b2-4c79-97b7-57b706d1d49c.gif">
 </p>
 
 ----------------------------------
 
+[Merlin Lange](https://twitter.com/Merlin_Lange) used *napari-animation* to create one of [Nature's best science images for September 2022](https://www.nature.com/immersive/d41586-022-03051-6/index.html)
+
+----------------------------------
+
 This plugin is built on [naparimovie](https://github.com/guiwitz/naparimovie) from @guiwitz. naparimovie was submitted to napari in [PR#851](https://github.com/napari/napari/pull/780) before napari plugin infrastructure existed.
 
 ----------------------------------
 ## Overview
 
 **napari-animation** provides a framework for the creation of animations in napari, the plugin contains:
 - an easy to use GUI for creating animations interactively
```

### Comparing `napari_animation-0.0.5/README.md` & `napari_animation-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 <p align="center">
   <img width="500" src="https://user-images.githubusercontent.com/7307488/196110138-6c4663b1-67b2-4c79-97b7-57b706d1d49c.gif">
 </p>
 
 ----------------------------------
 
+[Merlin Lange](https://twitter.com/Merlin_Lange) used *napari-animation* to create one of [Nature's best science images for September 2022](https://www.nature.com/immersive/d41586-022-03051-6/index.html)
+
+----------------------------------
+
 This plugin is built on [naparimovie](https://github.com/guiwitz/naparimovie) from @guiwitz. naparimovie was submitted to napari in [PR#851](https://github.com/napari/napari/pull/780) before napari plugin infrastructure existed.
 
 ----------------------------------
 ## Overview
 
 **napari-animation** provides a framework for the creation of animations in napari, the plugin contains:
 - an easy to use GUI for creating animations interactively
```

### Comparing `napari_animation-0.0.5/examples/animate2D.py` & `napari_animation-0.0.6/examples/animate2D.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/examples/animate3D.py` & `napari_animation-0.0.6/examples/animate3D.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/examples/animateMixed.py` & `napari_animation-0.0.6/examples/animateMixed.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_qt/_tests/test_animation_widget.py` & `napari_animation-0.0.6/napari_animation/_qt/_tests/test_animation_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_qt/animation_widget.py` & `napari_animation-0.0.6/napari_animation/_qt/animation_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_qt/frame_widget.py` & `napari_animation-0.0.6/napari_animation/_qt/frame_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_qt/keyframelistcontrol_widget.py` & `napari_animation-0.0.6/napari_animation/_qt/keyframelistcontrol_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_qt/keyframeslist_widget.py` & `napari_animation-0.0.6/napari_animation/_qt/keyframeslist_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_qt/savedialog_widget.py` & `napari_animation-0.0.6/napari_animation/_qt/savedialog_widget.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_tests/conftest.py` & `napari_animation-0.0.6/napari_animation/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_tests/test_animation.py` & `napari_animation-0.0.6/napari_animation/_tests/test_animation.py`

 * *Files 20% similar despite different names*

```diff
@@ -106,14 +106,29 @@
         assert saved_filename == expected_filename
     elif ext == "":
         expected = [output_filename / f"test_{i:06d}.png" for i in range(30)]
         saved_files = [call[0][0] for call in imsave.call_args_list]
         assert saved_files == expected
 
 
+@pytest.mark.parametrize("ext", [".mp4", ".mov", ".avi"])
+def test_animation_file_metadata(animation_with_key_frames, tmp_path, ext):
+    """Test output video file contians napari version metadata()"""
+    animation = animation_with_key_frames
+    output_filename = tmp_path / f"test{ext}"
+    animation.animate(output_filename)
+    # Read metadata back in, and check for napari version information
+    # We expect to see a metadata line in the metadata like this:
+    # title="napari version 0.4.17 https://napari.org/"
+    with open(output_filename, "rb") as f:
+        content = f.read()
+    assert b"napari version" in content
+    assert b"https://napari.org" in content
+
+
 @pytest.mark.parametrize("attribute", CAPTURED_LAYER_ATTRIBUTES)
 def test_layer_attribute_capture(layer_state, attribute):
     """Test that 'attribute' is captured in the layer state dictionary"""
     for layer_state_dict in layer_state.values():
         assert attribute in layer_state_dict.keys()
```

### Comparing `napari_animation-0.0.5/napari_animation/_tests/test_easing.py` & `napari_animation-0.0.6/napari_animation/_tests/test_easing.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_tests/test_frame_sequence.py` & `napari_animation-0.0.6/napari_animation/_tests/test_frame_sequence.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_tests/test_interpolation.py` & `napari_animation-0.0.6/napari_animation/_tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/_tests/test_utils.py` & `napari_animation-0.0.6/napari_animation/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/animation.py` & `napari_animation-0.0.6/napari_animation/animation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from itertools import count
 from pathlib import Path
 from time import sleep
 
 import imageio
 import numpy as np
+from napari._version import __version__ as napari_version
 from napari.utils.io import imsave
 from tqdm import tqdm
 
 from napari_animation.easing import Easing
 
 from .frame_sequence import FrameSequence
 from .key_frame import KeyFrame, KeyFrameList
@@ -41,14 +42,16 @@
             self._on_active_keyframe_changed
         )
 
         self._keyframe_counter = count()  # track number of frames created
 
         self._frames = FrameSequence(self.key_frames)
 
+        self._filename = None
+
     def capture_keyframe(
         self, steps=15, ease=Easing.LINEAR, insert=True, position: int = None
     ):
         """Record current key-frame
 
         Parameters
         ----------
@@ -151,17 +154,21 @@
             viewer.
         scale_factor : float
             Rescaling factor for the image size. Only used without
             viewer (with_viewer = False).
         """
         self._validate_animation()
 
+        description = f"napari version {napari_version} https://napari.org/"
+        output_params = ["-metadata", f'title="{description}"']
+
         # create path object
         file_path = Path(filename)
         folder_path = file_path.absolute().parent.joinpath(file_path.stem)
+        self._filename = file_path
 
         # if path has no extension, save as fold of PNG
         save_as_folder = False
         if file_path.suffix == "":
             save_as_folder = True
 
         # try to create an ffmpeg writer. If not installed default to folder creation
@@ -179,18 +186,22 @@
                     ".wmv",
                 ]:
                     writer = imageio.get_writer(
                         filename,
                         fps=fps,
                         quality=quality,
                         format=format,
+                        output_params=output_params,
                     )
                 else:
                     writer = imageio.get_writer(
-                        filename, fps=fps, format=format
+                        filename,
+                        fps=fps,
+                        format=format,
+                        output_params=output_params,
                     )
             except ValueError as err:
                 print(err)
                 print("Your file will be saved as a series of PNG files")
                 save_as_folder = True
 
         if save_as_folder:
@@ -239,7 +250,14 @@
         self.key_frames.selection.active = event.value
 
     def _on_active_keyframe_changed(self, event):
         active_keyframe = event.value
         if active_keyframe:
             keyframe_index = self.key_frames.index(active_keyframe)
             self.set_key_frame_index(keyframe_index)
+
+    def _repr_html_(self):
+        if self._filename is None:
+            return 'Video animation not yet available (use the "animate" method to generate it).'
+        else:
+            html = f'<video width="100%" height="100%" controls> <source src="{self._filename}"> </video>'
+            return html
```

### Comparing `napari_animation-0.0.5/napari_animation/easing.py` & `napari_animation-0.0.6/napari_animation/easing.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/frame_sequence.py` & `napari_animation-0.0.6/napari_animation/frame_sequence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from collections import deque
 from typing import TYPE_CHECKING, Dict, Iterator, Sequence, Tuple
 
 import numpy as np
 from napari.utils.events import EmitterGroup
 
 from .interpolation import (
     Interpolation,
@@ -15,14 +16,43 @@
 
 if TYPE_CHECKING:
     import napari
 
     from .key_frame import KeyFrame, KeyFrameList
 
 
+class LRUDict(dict):
+    def __init__(self, *args, cache_size=None, **kwargs):
+        self._cache_size = None
+        if cache_size is not None and cache_size > 0:
+            self._cache_size = cache_size
+        self._q = deque()
+        super().__init__(*args, **kwargs)
+
+    def __getitem__(self, key):
+        value = super().__getitem__(key)
+        if self._cache_size is not None:
+            # bring that key back to the top
+            self._q.remove(key)
+            self._q.append(key)
+        return value
+
+    def __setitem__(self, key, value):
+        if self._cache_size is not None:
+            while len(self) >= self._cache_size:
+                evicted_key = self._q.popleft()
+                super().__delitem__(evicted_key)
+            super().__setitem__(key, value)
+            self._q.append(key)
+
+    def clear(self):
+        self._q.clear()
+        super().clear()
+
+
 class FrameSequence(Sequence[ViewerState]):
     """Final sequence of of rendered animation frames, based on keyframes.
 
     This object acts like an immutable sequence of frames, interpolated from
     a sequence of (mutable) KeyFrames.  It can be indexed at any (valid) frame
     in the animation, and will inteprolate (and cache) viewer state on demand.
 
@@ -30,15 +60,15 @@
 
     Parameters
     ----------
     key_frames : KeyFrameList
         A KeyFrameList from which to render the final frame sequence.
     """
 
-    def __init__(self, key_frames: KeyFrameList) -> None:
+    def __init__(self, key_frames: KeyFrameList, cache_size: int = 10) -> None:
         super().__init__()
         self._key_frames = key_frames
         key_frames.events.inserted.connect(self._rebuild_keyframe_index)
         key_frames.events.removed.connect(self._rebuild_keyframe_index)
         key_frames.events.changed.connect(self._rebuild_keyframe_index)
         key_frames.events.reordered.connect(self._rebuild_keyframe_index)
 
@@ -49,15 +79,15 @@
 
         self.state_interpolation_map: InterpolationMap = {
             "camera.angles": Interpolation.SLERP,
             "camera.zoom": Interpolation.LOG,
         }
 
         # cache of interpolated viewer states
-        self._cache: Dict[int, ViewerState] = {}
+        self._cache: Dict[int, ViewerState] = LRUDict(cache_size=cache_size)
 
         # map of frame number -> (kf0, kf1, fraction)
         self._keyframe_index: Dict[int, Tuple[KeyFrame, KeyFrame, float]] = {}
         self._rebuild_keyframe_index()
 
     def _rebuild_keyframe_index(self, event=None):
         """Create a map of frame number -> (kf0, kf1, fraction)"""
@@ -87,14 +117,15 @@
         """The total frame count of the animation"""
         return len(self._keyframe_index)
 
     def __getitem__(self, key: int) -> ViewerState:
         """Get the interpolated state at frame `key` in the animation."""
         if key < 0:
             key += len(self)
+
         if key not in self._cache:
             try:
                 kf0, kf1, frac = self._keyframe_index[key]
             except KeyError:
                 raise IndexError(
                     f"Frame index ({key}) out of range ({len(self)} frames)"
                 )
```

### Comparing `napari_animation-0.0.5/napari_animation/interpolation/base_interpolation.py` & `napari_animation-0.0.6/napari_animation/interpolation/base_interpolation.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/interpolation/interpolation_constants.py` & `napari_animation-0.0.6/napari_animation/interpolation/interpolation_constants.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/interpolation/utils.py` & `napari_animation-0.0.6/napari_animation/interpolation/utils.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/interpolation/viewer_state_interpolation.py` & `napari_animation-0.0.6/napari_animation/interpolation/viewer_state_interpolation.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/key_frame.py` & `napari_animation-0.0.6/napari_animation/key_frame.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/utils.py` & `napari_animation-0.0.6/napari_animation/utils.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation/viewer_state.py` & `napari_animation-0.0.6/napari_animation/viewer_state.py`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/napari_animation.egg-info/PKG-INFO` & `napari_animation-0.0.6/napari_animation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-animation
-Version: 0.0.5
+Version: 0.0.6
 Summary: A plugin for making animations in napari
 Home-page: https://github.com/napari/napari-animation
 Download-URL: https://github.com/napari/napari-animation
 Author: Nicholas Sofroniew, Alister Burt, Guillaume Witz, Faris Abouakil, Talley Lambert
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -36,14 +36,18 @@
 
 <p align="center">
   <img width="500" src="https://user-images.githubusercontent.com/7307488/196110138-6c4663b1-67b2-4c79-97b7-57b706d1d49c.gif">
 </p>
 
 ----------------------------------
 
+[Merlin Lange](https://twitter.com/Merlin_Lange) used *napari-animation* to create one of [Nature's best science images for September 2022](https://www.nature.com/immersive/d41586-022-03051-6/index.html)
+
+----------------------------------
+
 This plugin is built on [naparimovie](https://github.com/guiwitz/naparimovie) from @guiwitz. naparimovie was submitted to napari in [PR#851](https://github.com/napari/napari/pull/780) before napari plugin infrastructure existed.
 
 ----------------------------------
 ## Overview
 
 **napari-animation** provides a framework for the creation of animations in napari, the plugin contains:
 - an easy to use GUI for creating animations interactively
```

### Comparing `napari_animation-0.0.5/napari_animation.egg-info/SOURCES.txt` & `napari_animation-0.0.6/napari_animation.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
 examples/animate2D.py
 examples/animate3D.py
 examples/animateMixed.py
+examples/ease_function.py
 examples/interactive_animation.py
+examples/programmatic_notebook_example.ipynb
 napari_animation/__init__.py
 napari_animation/_version.py
 napari_animation/animation.py
 napari_animation/easing.py
 napari_animation/frame_sequence.py
 napari_animation/key_frame.py
 napari_animation/napari.yaml
```

### Comparing `napari_animation-0.0.5/resources/screenshot-animation-widget.png` & `napari_animation-0.0.6/resources/screenshot-animation-widget.png`

 * *Files identical despite different names*

### Comparing `napari_animation-0.0.5/setup.cfg` & `napari_animation-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,20 @@
 	scipy
 	tqdm>=4.56.0
 	superqt
 
 [options.extras_require]
 testing = 
 	pytest
+	pytest-qt
 dev = 
 	pre-commit
 	black
 	flake8
+	isort
 	check-manifest
 	PyQt5>=5.12.3,!=5.15.0
 	%(testing)s
 
 [options.entry_points]
 napari.manifest = 
 	napari-animation = napari_animation:napari.yaml
```

### Comparing `napari_animation-0.0.5/tox.ini` & `napari_animation-0.0.6/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 platform = 
     macos: darwin
     linux: linux
     windows: win32
 passenv = 
     CI
     GITHUB_ACTIONS
-    DISPLAY XAUTHORITY
+    DISPLAY
+    XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
 conda_deps =
     # use conda to install numcodecs on mac py3.9
     py39-macos: numcodecs
 conda_channels =
     conda-forge
```

