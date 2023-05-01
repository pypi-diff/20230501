# Comparing `tmp/geo-espresso-0.3.1.tar.gz` & `tmp/geo-espresso-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo-espresso-0.3.1.tar", last modified: Fri Apr 28 00:11:01 2023, max compression
+gzip compressed data, was "geo-espresso-0.3.2.tar", last modified: Mon May  1 07:01:05 2023, max compression
```

## Comparing `geo-espresso-0.3.1.tar` & `geo-espresso-0.3.2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_ext/generate_contrib_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_edit1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork.png
--rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork2.png
--rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork3.png
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_fork4.png
--rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/contrib_pr1.png
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/espresso_arch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/inlab_logo_60px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.762809 geo-espresso-0.3.1/docs/source/contributor_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/github.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/new_contrib.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/submit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/contributor_guide/video.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    96854 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/build.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/ci.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/licence.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/developer_guide/repository.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/user_guide/api/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/docs/source/user_guide/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/contrib/_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/docs/source/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.758809 geo-espresso-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/src/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_espresso_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.766809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat
--rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/compile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/src/
--rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/waveTracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_gravity_density/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/_gravity_density.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_gravity_density/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/data/gravmodel1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_gravity_density/metadata.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.758809 geo-espresso-0.3.1/src/espresso/_machine/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_machine/build_package/
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/check_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/run_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/build_package/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/_sample_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/doc_utils/gen_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.770809 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/example_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_machine/new_contribution/create_new_contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.py
--rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.py
--rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_pumping_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_pumping_test/_pumping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.774809 geo-espresso-0.3.1/src/espresso/_receiver_function/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     8122 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RF.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/dpythag.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     5500 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/dsvdcmp.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/four1.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/priorvalue.f90
--rwxr-xr-x   0 runner    (1001) docker     (123)    13138 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/qlayer.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/ran3.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/rfi_param.inc
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/svbksb.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     4197 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo_noise.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/whichcell.f90
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/_receiver_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8649 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_receiver_function/rf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_simple_regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_simple_regression/_simple_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_slug_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_slug_test/_slug_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/espresso/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_xray_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/_xray_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/csiro_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example1.dat
--rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/_xray_tracer/data/inlab_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.778809 geo-espresso-0.3.1/src/espresso/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 00:10:46.000000 geo-espresso-0.3.1/src/espresso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:11:01.782809 geo-espresso-0.3.1/src/geo_espresso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:11:01.000000 geo-espresso-0.3.1/src/geo_espresso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.066852 geo-espresso-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.042854 geo-espresso-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_ext/generate_contrib_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/contrib_edit1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/contrib_fork.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/contrib_fork2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/contrib_fork3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/contrib_fork4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/contrib_pr1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/espresso_arch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/inlab_logo_60px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/github.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/new_contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/submit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/contributor_guide/video.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.046854 geo-espresso-0.3.2/docs/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    96854 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/ci.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/developer_guide/repository.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.050853 geo-espresso-0.3.2/docs/source/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.050853 geo-espresso-0.3.2/docs/source/user_guide/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.050853 geo-espresso-0.3.2/docs/source/user_guide/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/contrib/_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/docs/source/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:01:05.066852 geo-espresso-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.042854 geo-espresso-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.050853 geo-espresso-0.3.2/src/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_espresso_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.050853 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.050853 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/fmst/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/fmst/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/fmst/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/waveTracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_gravity_density/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/_gravity_density.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_gravity_density/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/data/gravmodel1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_gravity_density/metadata.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.042854 geo-espresso-0.3.2/src/espresso/_machine/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_machine/build_package/
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/check_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/run_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/build_package/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_machine/doc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/doc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/doc_utils/_sample_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/doc_utils/gen_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/example_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_machine/new_contribution/create_new_contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.054853 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.058853 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.058853 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/example_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/field_MT.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.058853 geo-espresso-0.3.2/src/espresso/_pumping_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_pumping_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_pumping_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_pumping_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_pumping_test/_pumping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.058853 geo-espresso-0.3.2/src/espresso/_receiver_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8122 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RF.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.058853 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/dpythag.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5500 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/dsvdcmp.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/four1.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/priorvalue.f90
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13138 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/qlayer.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/ran3.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/rfi_param.inc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/svbksb.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/theo.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4197 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/theo_noise.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/whichcell.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/_receiver_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8649 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_receiver_function/rf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/src/espresso/_simple_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_simple_regression/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_simple_regression/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_simple_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_simple_regression/_simple_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/src/espresso/_slug_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_slug_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_slug_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_slug_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_slug_test/_slug_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 07:01:04.000000 geo-espresso-0.3.2/src/espresso/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/src/espresso/_xray_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/_xray_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/csiro_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/example1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/example2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/example3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/_xray_tracer/data/inlab_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/src/espresso/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 07:00:48.000000 geo-espresso-0.3.2/src/espresso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:01:05.062852 geo-espresso-0.3.2/src/geo_espresso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-01 07:01:05.000000 geo-espresso-0.3.2/src/geo_espresso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-01 07:01:05.000000 geo-espresso-0.3.2/src/geo_espresso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:01:05.000000 geo-espresso-0.3.2/src/geo_espresso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-01 07:01:05.000000 geo-espresso-0.3.2/src/geo_espresso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 07:01:05.000000 geo-espresso-0.3.2/src/geo_espresso.egg-info/top_level.txt
```

### Comparing `geo-espresso-0.3.1/.gitignore` & `geo-espresso-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/CHANGELOG.md` & `geo-espresso-0.3.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Change Log
 
+## v0.3.2 (01/05/2023)
+
+### Espresso core
+
+- `EspressoProblem.list_capabilities`
+
+### Changed examples
+
+- Fix `covariance_matrix` and `inverse_covariance_matrix` in `ReceiverFunction`
+
+
 ## v0.3.1 (27/04/2023)
 
 ### Espresso core
 
 - Fix `list_capabilities` and enhance related documentation 
 
 ## v0.3.0 (24/04/2023)
```

### Comparing `geo-espresso-0.3.1/LICENCE` & `geo-espresso-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/PKG-INFO` & `geo-espresso-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.3.1
+Version: 0.3.2
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `geo-espresso-0.3.1/README.md` & `geo-espresso-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/Makefile` & `geo-espresso-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_ext/generate_contrib_docs.py` & `geo-espresso-0.3.2/docs/source/_ext/generate_contrib_docs.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/contrib_edit1.png` & `geo-espresso-0.3.2/docs/source/_static/contrib_edit1.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/contrib_fork.png` & `geo-espresso-0.3.2/docs/source/_static/contrib_fork.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/contrib_fork2.png` & `geo-espresso-0.3.2/docs/source/_static/contrib_fork2.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/contrib_fork3.png` & `geo-espresso-0.3.2/docs/source/_static/contrib_fork3.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/contrib_fork4.png` & `geo-espresso-0.3.2/docs/source/_static/contrib_fork4.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/contrib_pr1.png` & `geo-espresso-0.3.2/docs/source/_static/contrib_pr1.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/espresso_arch.svg` & `geo-espresso-0.3.2/docs/source/_static/espresso_arch.svg`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/inlab_logo_60px.png` & `geo-espresso-0.3.2/docs/source/_static/inlab_logo_60px.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_static/style.css` & `geo-espresso-0.3.2/docs/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_templates/autosummary/class.rst` & `geo-espresso-0.3.2/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/_templates/autosummary/module.rst` & `geo-espresso-0.3.2/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/conf.py` & `geo-espresso-0.3.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     # build process.
     app.connect("builder-inited", run_autogen)
 
 
 # -- Project information -----------------------------------------------------
 project = 'Espresso'
 copyright = f"{datetime.date.today().year}, InLab, {project} development team"
-version = "dev" if "dev" in esp.__version__ else f"v{esp.__version__}".replace(".dirty", "")
+_version_short = esp.__version__.split("+")[0]
+version = "dev" if "dev" in esp.__version__ else _version_short
 
 
 # -- General configuration ---------------------------------------------------
 sys.path.append(os.path.abspath("./_ext"))
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
```

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/faq.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/faq.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/github.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/github.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/index.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/index.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/new_contrib.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/new_contrib.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/setup.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/setup.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/submit.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/submit.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/contributor_guide/video.rst` & `geo-espresso-0.3.2/docs/source/contributor_guide/video.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/developer_guide/build.rst` & `geo-espresso-0.3.2/docs/source/developer_guide/build.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/developer_guide/ci.rst` & `geo-espresso-0.3.2/docs/source/developer_guide/ci.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/developer_guide/deploy.rst` & `geo-espresso-0.3.2/docs/source/developer_guide/deploy.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/developer_guide/develop.rst` & `geo-espresso-0.3.2/docs/source/developer_guide/develop.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/developer_guide/repository.rst` & `geo-espresso-0.3.2/docs/source/developer_guide/repository.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/index.rst` & `geo-espresso-0.3.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/user_guide/examples.rst` & `geo-espresso-0.3.2/docs/source/user_guide/examples.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/user_guide/faq.rst` & `geo-espresso-0.3.2/docs/source/user_guide/faq.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/user_guide/index.rst` & `geo-espresso-0.3.2/docs/source/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/user_guide/installation.rst` & `geo-espresso-0.3.2/docs/source/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/user_guide/usage.rst` & `geo-espresso-0.3.2/docs/source/user_guide/usage.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/docs/source/user_guide/why.rst` & `geo-espresso-0.3.2/docs/source/user_guide/why.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/pyproject.toml` & `geo-espresso-0.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # pylint src/espresso
 
 # --------------------------- END NOTES -----------------------------
 
 [build-system]
 requires = [
     "setuptools>=42",
-    "scikit-build>=0.13",
+    "scikit-build>=0.13,<0.17.3",
     "cmake>=3.18",
     "ninja",
     "versioningit",
     "numpy>=1.18",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `geo-espresso-0.3.1/setup.py` & `geo-espresso-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/CMakeLists.txt` & `geo-espresso-0.3.2/src/espresso/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/__init__.py` & `geo-espresso-0.3.2/src/espresso/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_espresso_problem.py` & `geo-espresso-0.3.2/src/espresso/_espresso_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,15 +346,27 @@
         Returns
         -------
         Number
             The log probability that a system is described by ``model`` prior to 
             seeing any data.
         """
         raise NotImplementedError
-        
+
+    def list_capabilities(self):
+        """Returns a dictionary describing the capabilities of the current example
+
+        Examples
+        --------
+        >>> import espresso
+        >>> r = espresso.ReceiverFunction()
+        >>> r.list_capabilities()
+        ['model_size', 'data_size', 'good_model', 'starting_model', 'data', 'description', 'covariance_matrix', 'plot_model', 'plot_data', 'log_likelihood', 'log_prior', 'rf', 'capability_report']
+        """
+        from .capabilities import list_capabilities
+        return list_capabilities(self.__class__.__name__)[self.__class__.__name__]
 
     def __getattr__(self, key):
         if hasattr(self, "params") and key in self.params:
             return self.params[key]
         if key in self.metadata:
             return self.metadata[key]
         else:
```

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/CMakeLists.txt` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/LICENCE` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/README.md` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/__init__.py` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/compile` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/fmst/compile`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_fm_wavefront_tracker/waveTracker.py` & `geo-espresso-0.3.2/src/espresso/_fm_wavefront_tracker/waveTracker.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_gravity_density/LICENCE` & `geo-espresso-0.3.2/src/espresso/_gravity_density/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_gravity_density/README.md` & `geo-espresso-0.3.2/src/espresso/_gravity_density/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_gravity_density/_gravity_density.py` & `geo-espresso-0.3.2/src/espresso/_gravity_density/_gravity_density.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_gravity_density/metadata.yml` & `geo-espresso-0.3.2/src/espresso/_gravity_density/metadata.yml`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/_utils.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/_utils.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/build.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/build.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/check_requires.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/check_requires.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/conftest.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/conftest.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/criteria.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/criteria.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/report.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/report.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/run_examples.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/run_examples.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/test_examples.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/test_examples.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/build_package/validate.py` & `geo-espresso-0.3.2/src/espresso/_machine/build_package/validate.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/doc_utils/_sample_code.txt` & `geo-espresso-0.3.2/src/espresso/_machine/doc_utils/_sample_code.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/doc_utils/gen_docs.py` & `geo-espresso-0.3.2/src/espresso/_machine/doc_utils/gen_docs.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/LICENCE` & `geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/new_contribution/_template/example_name.py` & `geo-espresso-0.3.2/src/espresso/_machine/new_contribution/_template/example_name.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_machine/new_contribution/create_new_contrib.py` & `geo-espresso-0.3.2/src/espresso/_machine/new_contribution/create_new_contrib.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/LICENCE` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/README.md` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/__init__.py` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/example_01.py` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/field_MT.py` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/field_MT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py` & `geo-espresso-0.3.2/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_pumping_test/LICENCE` & `geo-espresso-0.3.2/src/espresso/_pumping_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_pumping_test/README.md` & `geo-espresso-0.3.2/src/espresso/_pumping_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_pumping_test/_pumping_test.py` & `geo-espresso-0.3.2/src/espresso/_pumping_test/_pumping_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/CMakeLists.txt` & `geo-espresso-0.3.2/src/espresso/_receiver_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/LICENCE` & `geo-espresso-0.3.2/src/espresso/_receiver_function/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RF.f90` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RF.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/dsvdcmp.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/dsvdcmp.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/four1.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/four1.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/qlayer.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/qlayer.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/ran3.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/ran3.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/svbksb.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/svbksb.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/theo.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/theo_noise.f` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/theo_noise.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90` & `geo-espresso-0.3.2/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/__init__.py` & `geo-espresso-0.3.2/src/espresso/_receiver_function/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/_receiver_function.py` & `geo-espresso-0.3.2/src/espresso/_receiver_function/_receiver_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,22 +95,22 @@
         return self._null_model
 
     @property
     def data(self):
         return self._data
 
     @property
-    def covariance_matrix(self):                # optional
-        Cdinv = self.rf.InvDataCov(2.5,0.01,len(self.data))
-        Cdinv /= 100        # temper the likelihood by rescaling the data covariance
-        return Cdinv
+    def covariance_matrix(self): 
+        return np.linalg.inv(self.inverse_covariance_matrix)
 
     @property
     def inverse_covariance_matrix(self):
-        raise NotImplementedError               # optional
+        Cdinv = self.rf.InvDataCov(2.5,0.01,len(self.data))
+        Cdinv /= 100        # temper the likelihood by rescaling the data covariance
+        return Cdinv
 
     def _model_setup(self, model):
         model_setup = np.copy(self._ref_model_setup)
         if self.example_number == 1:
             model_setup[self._interfaces,0] = model
         elif self.example_number == 2:
             model_setup[:,1] = model
```

### Comparing `geo-espresso-0.3.1/src/espresso/_receiver_function/rf.py` & `geo-espresso-0.3.2/src/espresso/_receiver_function/rf.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_simple_regression/LICENCE` & `geo-espresso-0.3.2/src/espresso/_simple_regression/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_simple_regression/_simple_regression.py` & `geo-espresso-0.3.2/src/espresso/_simple_regression/_simple_regression.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_slug_test/LICENCE` & `geo-espresso-0.3.2/src/espresso/_slug_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_slug_test/README.md` & `geo-espresso-0.3.2/src/espresso/_slug_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_slug_test/_slug_test.py` & `geo-espresso-0.3.2/src/espresso/_slug_test/_slug_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/LICENCE` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/README.md` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/_xray_tracer.py` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/_xray_tracer.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/csiro_logo.png` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/data/csiro_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example1.dat` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/data/example1.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example2.dat` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/data/example2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/example3.dat` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/data/example3.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/_xray_tracer/data/inlab_logo.png` & `geo-espresso-0.3.2/src/espresso/_xray_tracer/data/inlab_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/capabilities.py` & `geo-espresso-0.3.2/src/espresso/capabilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -148,15 +148,16 @@
         "covariance_matrix": 0,
         "inverse_covariance_matrix": 0,
         "jacobian": 0,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 0,
-        "log_prior": 0
+        "log_prior": 0,
+        "list_capabilities": 1
     },
     "SlugTest": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -165,15 +166,16 @@
         "covariance_matrix": 1,
         "inverse_covariance_matrix": 1,
         "jacobian": 0,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 1,
-        "log_prior": 0
+        "log_prior": 0,
+        "list_capabilities": 1
     },
     "PumpingTest": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -182,15 +184,16 @@
         "covariance_matrix": 1,
         "inverse_covariance_matrix": 1,
         "jacobian": 0,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 1,
-        "log_prior": 0
+        "log_prior": 0,
+        "list_capabilities": 1
     },
     "GravityDensity": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -199,15 +202,16 @@
         "covariance_matrix": 1,
         "inverse_covariance_matrix": 0,
         "jacobian": 1,
         "plot_model": 1,
         "plot_data": 1,
         "misfit": 0,
         "log_likelihood": 0,
-        "log_prior": 0
+        "log_prior": 0,
+        "list_capabilities": 1
     },
     "Magnetotelluric1D": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -217,17 +221,18 @@
         "inverse_covariance_matrix": 1,
         "jacobian": 1,
         "plot_model": 1,
         "plot_data": 1,
         "misfit": 1,
         "log_likelihood": 0,
         "log_prior": 0,
-        "set_start_model": 1,
+        "set_start_mesh": 1,
+        "list_capabilities": 1,
         "set_obs_data": 1,
-        "set_start_mesh": 1
+        "set_start_model": 1
     },
     "SimpleRegression": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -236,32 +241,34 @@
         "covariance_matrix": 1,
         "inverse_covariance_matrix": 1,
         "jacobian": 1,
         "plot_model": 0,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 0,
-        "log_prior": 0
+        "log_prior": 0,
+        "list_capabilities": 1
     },
     "ReceiverFunction": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
         "forward": 0,
         "description": 1,
         "covariance_matrix": 1,
-        "inverse_covariance_matrix": 0,
+        "inverse_covariance_matrix": 1,
         "jacobian": 0,
         "plot_model": 1,
         "plot_data": 1,
         "misfit": 0,
         "log_likelihood": 1,
         "log_prior": 1,
+        "list_capabilities": 1,
         "rf": 1
     },
     "FmWavefrontTracker": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
@@ -272,13 +279,14 @@
         "inverse_covariance_matrix": 0,
         "jacobian": 1,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 0,
         "log_prior": 0,
+        "tmp_files": 1,
         "tmp_paths": 1,
         "clean_tmp_files": 1,
-        "tmp_files": 1,
-        "exe_fm2dss": 1
+        "exe_fm2dss": 1,
+        "list_capabilities": 1
     }
 }
```

### Comparing `geo-espresso-0.3.1/src/espresso/exceptions.py` & `geo-espresso-0.3.2/src/espresso/exceptions.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/utils/__init__.py` & `geo-espresso-0.3.2/src/espresso/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/espresso/utils/data_loader.py` & `geo-espresso-0.3.2/src/espresso/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.3.1/src/geo_espresso.egg-info/PKG-INFO` & `geo-espresso-0.3.2/src/geo_espresso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.3.1
+Version: 0.3.2
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `geo-espresso-0.3.1/src/geo_espresso.egg-info/SOURCES.txt` & `geo-espresso-0.3.2/src/geo_espresso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

