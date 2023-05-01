# Comparing `tmp/qp-prob-0.8.1.tar.gz` & `tmp/qp-prob-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qp-prob-0.8.1.tar", last modified: Wed Apr 12 20:45:53 2023, max compression
+gzip compressed data, was "qp-prob-0.8.2.tar", last modified: Mon May  1 20:10:57 2023, max compression
```

## Comparing `qp-prob-0.8.1.tar` & `qp-prob-0.8.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.777543 qp-prob-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.757542 qp-prob-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.761542 qp-prob-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-12 20:45:40.000000 qp-prob-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-12 20:45:53.777543 qp-prob-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-12 20:45:40.000000 qp-prob-0.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)       52 2023-04-12 20:45:40.000000 qp-prob-0.8.1/do_cover.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.765542 qp-prob-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)   861344 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/demo.html
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (122)   757141 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/practical_example.html
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/qp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.765542 qp-prob-0.8.1/nb/
--rw-r--r--   0 runner    (1001) docker     (122)    32323 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/iterator_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    15156 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/metrics_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/mixmod_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    11839 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/practical_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    37404 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/quantile_parameterization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-04-12 20:45:40.000000 qp-prob-0.8.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)      326 2023-04-12 20:45:40.000000 qp-prob-0.8.1/render_nb.sh
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-12 20:45:40.000000 qp-prob-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 20:45:53.777543 qp-prob-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-12 20:45:40.000000 qp-prob-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.757542 qp-prob-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.769542 qp-prob-0.8.1/src/qp/
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-12 20:45:52.000000 qp-prob-0.8.1/src/qp/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    11419 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/conversion_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.769542 qp-prob-0.8.1/src/qp/data/
--rw-r--r--   0 runner    (1001) docker     (122)   161680 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/data/CFHTLens_sample.P.npy
--rw-r--r--   0 runner    (1001) docker     (122)    16848 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/data/test.hdf5
--rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/dict_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    21140 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/hist_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    12842 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/interp_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/lazy_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/src/qp/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/array_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/brier.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/goodness_of_fit.py
--rw-r--r--   0 runner    (1001) docker     (122)    17889 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7560 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/pit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6155 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/mixmod_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/packed_interp_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/packing_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14160 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/pdf_gen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quant_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
--rw-r--r--   0 runner    (1001) docker     (122)     6796 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/dual_spline_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_constant.py
--rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/scipy_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/sparse_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    10121 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/sparse_rep.py
--rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/spline_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)    23972 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/src/qp_prob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        3 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.757542 qp-prob-0.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/tests/qp/
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.777543 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
--rw-r--r--   0 runner    (1001) docker     (122)     4145 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (122)     4607 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_brier.py
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_eval_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_flex_coefs.npy
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (122)    15872 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_pit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5816 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_scipy_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.288384 qp-prob-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.288384 qp-prob-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-05-01 20:10:41.000000 qp-prob-0.8.2/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-05-01 20:10:41.000000 qp-prob-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-05-01 20:10:57.296384 qp-prob-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-05-01 20:10:41.000000 qp-prob-0.8.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)       52 2023-05-01 20:10:41.000000 qp-prob-0.8.2/do_cover.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.292384 qp-prob-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   861344 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/demo.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   757141 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/practical_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/qp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-01 20:10:41.000000 qp-prob-0.8.2/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.292384 qp-prob-0.8.2/nb/
+-rw-r--r--   0 runner    (1001) docker     (122)    32323 2023-05-01 20:10:41.000000 qp-prob-0.8.2/nb/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-05-01 20:10:41.000000 qp-prob-0.8.2/nb/iterator_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    15156 2023-05-01 20:10:41.000000 qp-prob-0.8.2/nb/metrics_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-05-01 20:10:41.000000 qp-prob-0.8.2/nb/mixmod_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11839 2023-05-01 20:10:41.000000 qp-prob-0.8.2/nb/practical_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    37404 2023-05-01 20:10:41.000000 qp-prob-0.8.2/nb/quantile_parameterization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-05-01 20:10:41.000000 qp-prob-0.8.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      326 2023-05-01 20:10:41.000000 qp-prob-0.8.2/render_nb.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-01 20:10:41.000000 qp-prob-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 20:10:57.296384 qp-prob-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-01 20:10:41.000000 qp-prob-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.288384 qp-prob-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/src/qp/
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-01 20:10:56.000000 qp-prob-0.8.2/src/qp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11419 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/conversion_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/src/qp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)   161680 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/data/CFHTLens_sample.P.npy
+-rw-r--r--   0 runner    (1001) docker     (122)    16848 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/data/test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/dict_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21140 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/hist_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12842 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/lazy_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/src/qp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/metrics/array_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/metrics/brier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/metrics/goodness_of_fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17889 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8213 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/metrics/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6155 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/mixmod_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/packed_interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/packing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14160 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/pdf_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quant_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6796 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/quantile_pdf_constructors/piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/scipy_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/sparse_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10121 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/sparse_rep.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/spline_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23972 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-01 20:10:41.000000 qp-prob-0.8.2/src/qp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/src/qp_prob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-05-01 20:10:57.000000 qp-prob-0.8.2/src/qp_prob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-05-01 20:10:57.000000 qp-prob-0.8.2/src/qp_prob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 20:10:57.000000 qp-prob-0.8.2/src/qp_prob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-01 20:10:57.000000 qp-prob-0.8.2/src/qp_prob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        3 2023-05-01 20:10:57.000000 qp-prob-0.8.2/src/qp_prob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.288384 qp-prob-0.8.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/tests/qp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:57.296384 qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4145 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4607 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_brier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_eval_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_flex_coefs.npy
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15872 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3612 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5816 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_scipy_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-05-01 20:10:41.000000 qp-prob-0.8.2/tests/qp/test_utils.py
```

### Comparing `qp-prob-0.8.1/.github/workflows/pypi.yaml` & `qp-prob-0.8.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/.github/workflows/python-package.yml` & `qp-prob-0.8.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/.gitignore` & `qp-prob-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/.travis.yml` & `qp-prob-0.8.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/LICENSE` & `qp-prob-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/PKG-INFO` & `qp-prob-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.8.1
+Version: 0.8.2
 License: MIT License
         
         Copyright (c) 2016 Alex Malz & Phil Marshall
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `qp-prob-0.8.1/README.md` & `qp-prob-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/.gitignore` & `qp-prob-0.8.2/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/Makefile` & `qp-prob-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/conf.py` & `qp-prob-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/contributing.rst` & `qp-prob-0.8.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/demo.html` & `qp-prob-0.8.2/docs/demo.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/index.rst` & `qp-prob-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/install.rst` & `qp-prob-0.8.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/practical_example.html` & `qp-prob-0.8.2/docs/practical_example.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/docs/qp.rst` & `qp-prob-0.8.2/docs/qp.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/nb/demo.ipynb` & `qp-prob-0.8.2/nb/demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/nb/iterator_demo.ipynb` & `qp-prob-0.8.2/nb/iterator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/nb/metrics_examples.ipynb` & `qp-prob-0.8.2/nb/metrics_examples.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/nb/mixmod_examples.ipynb` & `qp-prob-0.8.2/nb/mixmod_examples.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/nb/practical_example.ipynb` & `qp-prob-0.8.2/nb/practical_example.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/nb/quantile_parameterization_demo.ipynb` & `qp-prob-0.8.2/nb/quantile_parameterization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/pyproject.toml` & `qp-prob-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/__init__.py` & `qp-prob-0.8.2/src/qp/__init__.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/conversion_funcs.py` & `qp-prob-0.8.2/src/qp/conversion_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/data/CFHTLens_sample.P.npy` & `qp-prob-0.8.2/src/qp/data/CFHTLens_sample.P.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/data/test.hdf5` & `qp-prob-0.8.2/src/qp/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/dict_utils.py` & `qp-prob-0.8.2/src/qp/dict_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/ensemble.py` & `qp-prob-0.8.2/src/qp/ensemble.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/factory.py` & `qp-prob-0.8.2/src/qp/factory.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/hist_pdf.py` & `qp-prob-0.8.2/src/qp/hist_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/interp_pdf.py` & `qp-prob-0.8.2/src/qp/interp_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/metrics/array_metrics.py` & `qp-prob-0.8.2/src/qp/metrics/array_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/metrics/brier.py` & `qp-prob-0.8.2/src/qp/metrics/brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/metrics/goodness_of_fit.py` & `qp-prob-0.8.2/src/qp/metrics/goodness_of_fit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/metrics/metrics.py` & `qp-prob-0.8.2/src/qp/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/metrics/pit.py` & `qp-prob-0.8.2/src/qp/metrics/pit.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,28 +35,28 @@
         qp_ens : Ensemble
             A collection of N distribution objects
         true_vals : [float]
             An array-like sequence of N float values representing the known true value for each distribution
         eval_grid : [float], optional
             A strictly increasing array-like sequence in the range [0,1], by default DEFAULT_QUANTS
         """
-
         self._true_vals = true_vals
 
         # For each distribution in the Ensemble, calculate the CDF where x = known_true_value
         self._pit_samps = np.array([qp_ens[i].cdf(self._true_vals[i])[0][0] for i in range(len(self._true_vals))])
 
         n_pit = np.min([len(self._pit_samps), len(eval_grid)])
         if n_pit < len(eval_grid):
             logging.warning('Number of pit samples is smaller than the evaluation grid size. '
                             'Will create a new evaluation grid with size = number of pit samples')
             eval_grid = np.linspace(0, 1, n_pit)
 
         data_quants = np.quantile(self._pit_samps, eval_grid)
-        self._pit = qp.Ensemble(qp.quant, data=dict(quants=eval_grid, locs=np.atleast_2d(data_quants)))
+        quant_mask = self._create_quant_mask(data_quants)
+        self._pit = qp.Ensemble(qp.quant, data=dict(quants=eval_grid[quant_mask], locs=np.atleast_2d(data_quants[quant_mask])))
 
     @property
     def pit_samps(self):
         """Returns the PIT samples. i.e. ``CDF(true_vals)`` for each distribution in the Ensemble used to initialize the PIT object.
 
         Returns
         -------
@@ -162,14 +162,33 @@
         Returns
         -------
         float
             The percentage of outliers in this distribution given the min and max bounds.
         """
         return calculate_outlier_rate(self._pit, pit_min, pit_max)[0]
 
+    @classmethod
+    def _create_quant_mask(self, data_quants):
+        """ Create a numpy mask such that, when applied only values greater than
+        0 and less than 1.0 are kept. While this function is fairly simple,
+        separating it into a small helper method makes testing much easier.
+
+        Parameters
+        ----------
+        data_quants : np.array [float]
+            An array of values.
+
+        Returns
+        -------
+        np.array [bool]
+            The boolean mask
+        """
+
+        return np.bitwise_and(data_quants > 0., data_quants < 1)
+
     def _trim_pit_values(self, cdf_min, cdf_max):
         """Remove and report any cdf(x) that are outside the min/max range.
 
         Parameters
         ----------
         cdf_min : float
             The minimum cdf(x) value to accept
```

### Comparing `qp-prob-0.8.1/src/qp/mixmod_pdf.py` & `qp-prob-0.8.2/src/qp/mixmod_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/packed_interp_pdf.py` & `qp-prob-0.8.2/src/qp/packed_interp_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/packing_utils.py` & `qp-prob-0.8.2/src/qp/packing_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/pdf_gen.py` & `qp-prob-0.8.2/src/qp/pdf_gen.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/plotting.py` & `qp-prob-0.8.2/src/qp/plotting.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/quant_pdf.py` & `qp-prob-0.8.2/src/qp/quant_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py` & `qp-prob-0.8.2/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py` & `qp-prob-0.8.2/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/dual_spline_average.py` & `qp-prob-0.8.2/src/qp/quantile_pdf_constructors/dual_spline_average.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_constant.py` & `qp-prob-0.8.2/src/qp/quantile_pdf_constructors/piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_linear.py` & `qp-prob-0.8.2/src/qp/quantile_pdf_constructors/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/scipy_pdfs.py` & `qp-prob-0.8.2/src/qp/scipy_pdfs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/sparse_pdf.py` & `qp-prob-0.8.2/src/qp/sparse_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/sparse_rep.py` & `qp-prob-0.8.2/src/qp/sparse_rep.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/spline_pdf.py` & `qp-prob-0.8.2/src/qp/spline_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/test_data.py` & `qp-prob-0.8.2/src/qp/test_data.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/test_funcs.py` & `qp-prob-0.8.2/src/qp/test_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp/utils.py` & `qp-prob-0.8.2/src/qp/utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/src/qp_prob.egg-info/PKG-INFO` & `qp-prob-0.8.2/src/qp_prob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.8.1
+Version: 0.8.2
 License: MIT License
         
         Copyright (c) 2016 Alex Malz & Phil Marshall
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `qp-prob-0.8.1/src/qp_prob.egg-info/SOURCES.txt` & `qp-prob-0.8.2/src/qp_prob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/.gitignore` & `qp-prob-0.8.2/tests/qp/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/benchmark.py` & `qp-prob-0.8.2/tests/qp/benchmark.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/fidelity.py` & `qp-prob-0.8.2/tests/qp/fidelity.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py` & `qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py` & `qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py` & `qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py` & `qp-prob-0.8.2/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_auto.py` & `qp-prob-0.8.2/tests/qp/test_auto.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_brier.py` & `qp-prob-0.8.2/tests/qp/test_brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_ensemble.py` & `qp-prob-0.8.2/tests/qp/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_eval_funcs.py` & `qp-prob-0.8.2/tests/qp/test_eval_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_flex_coefs.npy` & `qp-prob-0.8.2/tests/qp/test_flex_coefs.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_infrastructure.py` & `qp-prob-0.8.2/tests/qp/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_metrics.py` & `qp-prob-0.8.2/tests/qp/test_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_parallel.py` & `qp-prob-0.8.2/tests/qp/test_parallel.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_pit.py` & `qp-prob-0.8.2/tests/qp/test_pit.py`

 * *Files 27% similar despite different names*

```diff
@@ -65,7 +65,41 @@
 
     def test_pit_metric_small_eval_grid(self):
         """Test PIT metric warning message when number of pit samples is smaller than the evaluation grid"""
         with self.assertLogs(level='WARNING') as log:
             quant_grid = np.linspace(0, 1, 1000)
             _ = PIT(self.grid_ens, self.true_zs, quant_grid)
             self.assertIn('Number of pit samples is smaller', log.output[0])
+
+    def test_pit_metric_masking(self):
+        """The normal distributions created in this test will produce a quantile
+        array in PIT that have multiple values of 1.0. This test will confirm
+        that the some quants have been removed. 
+
+        If no quants had been removed, then the final length would be 101.
+        """
+
+        true_zs = np.random.uniform(low=NMAX-0.1, high=NMAX, size=NPDF)
+
+        locs = np.expand_dims(true_zs + np.random.normal(0.0, 0.01, NPDF), -1)
+        scales = np.ones((NPDF, 1)) * 0.001
+        n_ens = Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
+
+        grid_ens = n_ens.convert_to(interp_gen, xvals=ZGRID)
+
+        quant_grid = np.linspace(0, 1, 101)
+        pit_obj = PIT(grid_ens, true_zs, quant_grid)
+        pit_ens = pit_obj.pit
+        assert len(pit_ens.dist.quants) == 90
+
+    def test_pit_create_quant_mask(self):
+        """Basic test where all values should be returned"""
+        input = np.linspace(0.1, 0.9, 10)
+        mask = PIT._create_quant_mask(input)
+        assert np.all(input[mask] == input)
+
+    def test_pit_create_quant_mask_with_exclusions(self):
+        """Test with values that should be excluded"""
+        input = np.linspace(-0.1, 1.1, 10)
+        mask = PIT._create_quant_mask(input)
+        assert np.all(input[mask] > 0)
+        assert np.all(input[mask] < 1)
```

### Comparing `qp-prob-0.8.1/tests/qp/test_scipy_vectorization.py` & `qp-prob-0.8.2/tests/qp/test_scipy_vectorization.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.1/tests/qp/test_utils.py` & `qp-prob-0.8.2/tests/qp/test_utils.py`

 * *Files identical despite different names*

