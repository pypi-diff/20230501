# Comparing `tmp/tensorcircuit-nightly-0.8.0.dev20230429.tar.gz` & `tmp/tensorcircuit-nightly-0.8.0.dev20230430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230429.tar", last modified: Sat Apr 29 12:37:41 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230430.tar", last modified: Sun Apr 30 12:36:46 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.8.0.dev20230429.tar` & `tensorcircuit-nightly-0.8.0.dev20230430.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.756441 tensorcircuit-nightly-0.8.0.dev20230429/
--rw-r--r--   0 runner    (1001) docker     (122)    23547 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-29 12:37:41.756441 tensorcircuit-nightly-0.8.0.dev20230429/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.740440 tensorcircuit-nightly-0.8.0.dev20230429/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.744440 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27390 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 12:37:41.756441 tensorcircuit-nightly-0.8.0.dev20230429/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-29 12:37:36.000000 tensorcircuit-nightly-0.8.0.dev20230429/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.748440 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-29 12:37:36.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.748440 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.748440 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.748440 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.748440 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.752441 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.752441 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.752441 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.752441 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-29 12:37:41.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-29 12:37:41.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 12:37:41.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-29 12:37:41.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-29 12:37:41.000000 tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 12:37:41.756441 tensorcircuit-nightly-0.8.0.dev20230429/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-29 12:14:53.000000 tensorcircuit-nightly-0.8.0.dev20230429/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.587030 tensorcircuit-nightly-0.8.0.dev20230430/
+-rw-r--r--   0 runner    (1001) docker     (122)    23547 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-30 12:36:46.587030 tensorcircuit-nightly-0.8.0.dev20230430/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.567030 tensorcircuit-nightly-0.8.0.dev20230430/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.575030 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27390 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-30 12:36:46.587030 tensorcircuit-nightly-0.8.0.dev20230430/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-30 12:36:41.000000 tensorcircuit-nightly-0.8.0.dev20230430/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.579030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1407 2023-04-30 12:36:41.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.579030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.583030 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-30 12:36:46.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-30 12:36:46.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-30 12:36:46.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-30 12:36:46.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-30 12:36:46.000000 tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-30 12:36:46.587030 tensorcircuit-nightly-0.8.0.dev20230430/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-30 12:15:26.000000 tensorcircuit-nightly-0.8.0.dev20230430/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/CHANGELOG.md` & `tensorcircuit-nightly-0.8.0.dev20230430/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/HISTORY.md` & `tensorcircuit-nightly-0.8.0.dev20230430/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/LICENSE` & `tensorcircuit-nightly-0.8.0.dev20230430/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230430/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230429
+Version: 0.8.0.dev20230430
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/README.md` & `tensorcircuit-nightly-0.8.0.dev20230430/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/README_cn.md` & `tensorcircuit-nightly-0.8.0.dev20230430/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/advance.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/cnconf.py` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/conf.py` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/contribution.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/faq.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/index.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/infras.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/modules.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230430/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/setup.py` & `tensorcircuit-nightly-0.8.0.dev20230430/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0.dev20230429"
+__version__ = "0.8.0.dev20230430"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/about.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230429
+Version: 0.8.0.dev20230430
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.8.0.dev20230430/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/conftest.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_backends.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_calibrating.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_channels.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_gates.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_interfaces.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_keras.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_miscs.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_qaoa.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_results.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_templates.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230429/tests/test_van.py` & `tensorcircuit-nightly-0.8.0.dev20230430/tests/test_van.py`

 * *Files identical despite different names*

