# Comparing `tmp/Hydro-Quebec-API-Wrapper-3.0.6.tar.gz` & `tmp/Hydro-Quebec-API-Wrapper-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hydro-Quebec-API-Wrapper-3.0.6.tar", last modified: Sat Apr  1 18:00:49 2023, max compression
+gzip compressed data, was "Hydro-Quebec-API-Wrapper-3.0.7.tar", last modified: Mon May  1 01:18:35 2023, max compression
```

## Comparing `Hydro-Quebec-API-Wrapper-3.0.6.tar` & `Hydro-Quebec-API-Wrapper-3.0.7.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.362726 Hydro-Quebec-API-Wrapper-3.0.6/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1859 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    10998 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.354726 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7459 2023-04-01 18:00:49.000000 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2560 2023-04-01 18:00:49.000000 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 18:00:49.000000 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-01 18:00:49.000000 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-01 18:00:49.000000 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-01 18:00:49.000000 Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7459 2023-04-01 18:00:49.362726 Hydro-Quebec-API-Wrapper-3.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6828 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/config.default.yaml
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/conflict_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.354726 Hydro-Quebec-API-Wrapper-3.0.6/docs/
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.354726 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.354726 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     6049 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/_static/hydroqc-logo-128.png
--rw-rw-rw-   0 root         (0) root         (0)     8268 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/_static/hydroqc-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.354726 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/external/
--rw-rw-rw-   0 root         (0) root         (0)   348837 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/external/description-des-codes-interruption.pdf
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.contract.rst
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.hydro_api.rst
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.peak.cpc.rst
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.peak.dpc.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.peak.rst
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.rst
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.types.rst
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/docs/source/todo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/examples/
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/examples/hydro.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/account.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/consts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15445 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/common.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_d.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_d_cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4940 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_dpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_dt.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_m.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_m_gdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_residential.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/outage.py
--rw-rw-rw-   0 root         (0) root         (0)     6165 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/customer.py
--rw-rw-rw-   0 root         (0) root         (0)    15470 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/diagnostic.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    29216 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/consts.py
--rw-rw-rw-   0 root         (0) root         (0)    15695 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     6700 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/peak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     8860 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/peak.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1136 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/timerange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3695 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/account.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/common.py
--rw-rw-rw-   0 root         (0) root         (0)     5928 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/consump.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/contract.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/dpc.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/dt.py
--rw-rw-rw-   0 root         (0) root         (0)     3838 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/outage.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/webuser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.358726 Hydro-Quebec-API-Wrapper-3.0.6/logo/
--rw-rw-rw-   0 root         (0) root         (0)     6049 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/logo/hydroqc-logo-128.png
--rw-rw-rw-   0 root         (0) root         (0)     8268 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/logo/hydroqc-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2646 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/renovate.json
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-04-01 18:00:49.362726 Hydro-Quebec-API-Wrapper-3.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:00:49.362726 Hydro-Quebec-API-Wrapper-3.0.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    17588 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_common.py
--rw-rw-rw-   0 root         (0) root         (0)     2591 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_d.py
--rw-rw-rw-   0 root         (0) root         (0)     8496 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_d_cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     6711 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_dpc.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_dt.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_m.py
--rw-rw-rw-   0 root         (0) root         (0)     3247 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_m_gdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/test_timerange.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tests/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2023-04-01 18:00:37.000000 Hydro-Quebec-API-Wrapper-3.0.6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11000 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19948 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7459 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7459 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/config.default.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/conflict_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo-128.png
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/external/
+-rw-rw-rw-   0 root         (0) root         (0)   348837 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/external/description-des-codes-interruption.pdf
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.contract.rst
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.hydro_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.cpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.dpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.types.rst
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/todo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/examples/hydro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/consts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15445 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d_cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4940 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m_gdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_residential.py
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/outage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6165 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    15470 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/diagnostic.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    29216 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)    15695 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6700 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/peak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8860 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/peak.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1136 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/timerange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3695 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     5928 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/consump.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/outage.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/webuser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/logo/
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo-128.png
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2646 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/renovate.json
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    17588 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     2591 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d.py
+-rw-rw-rw-   0 root         (0) root         (0)     8496 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d_cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6711 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m.py
+-rw-rw-rw-   0 root         (0) root         (0)     3247 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m_gdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/test_timerange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4062 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tox.ini
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/.gitignore` & `Hydro-Quebec-API-Wrapper-3.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/.gitlab-ci.yml` & `Hydro-Quebec-API-Wrapper-3.0.7/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   paths:
     - .cache/pip
 
 test:
   stage: test
   tags:
   - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230331170705
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230425000953  
   script:
     #- apt-get update && apt-get install git --no-install-recommends -y graphviz jq python3.10 python3-venv python3-pip git
     - cat renovate.json |jq > /dev/null 2&>1 || ( echo "renovate.json not valid" && exit 1 )
     - pip install tox
     - tox -e pylint,flake8,pydocstyle,typing,black,deps-conflict --parallel auto
     - cat mypy-txt-report/index.txt
   artifacts:
@@ -53,15 +53,15 @@
       when: manual
     - when: never
 
 .private_test_script: &private_test_script
   stage: private_tests
   tags:
   - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230331170705
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230425000953
   script:
     #- apt update && apt install -y jq unzip curl
     - >
       OUTPUT=$(curl
       --globoff
       --header "Content-Type: application/json"
       --header "PRIVATE-TOKEN: ${HYDROQC_SA_TOKEN}"
@@ -223,15 +223,15 @@
       when: never
     - !reference [.private_test_script, rules]
 
 private_tests_done:
   stage: private_tests_done
   tags:
   - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230331170705
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230425000953
   script:
     #- apt-get update && apt-get install --no-install-recommends -y python3.10 python3-venv python3-pip --no-install-recommends git
     - echo "Private Tests done"
     - pip install tox
     - find .
     - mv -v hydroqc/.coverage* .
     - mv -v hydroqc/*.xml .
@@ -266,15 +266,15 @@
       when: manual
     - when: never
 
 package:
   stage: test
   tags:
   - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230331170705
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230425000953
   script:
     # Build a package with a version based on the commmit short sha
     - pip install --upgrade pip
     - pip install --upgrade build setuptools wheel twine setuptools_scm
     - python3 -m build -o dist
     - python3 -m twine check --strict dist/*
     - TWINE_PASSWORD=${CI_JOB_TOKEN} TWINE_USERNAME=gitlab-ci-token python3 -m twine upload --verbose --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
@@ -296,15 +296,15 @@
       when: manual
     - when: never
 
 promote2pypi:
   stage: pypi
   tags:
   - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230331170705
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20230425000953
   script:
     # TODO: try to pull the good package from gitlab pypi repo
     #       then change the version (promote)
     #       then push it to pypi
     #- rm -rf dist
     #- mkdir -p dist
     #- cd dist
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/.pre-commit-config.yaml` & `Hydro-Quebec-API-Wrapper-3.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/.pylintrc` & `Hydro-Quebec-API-Wrapper-3.0.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO` & `Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hydro-Quebec-API-Wrapper
-Version: 3.0.6
+Version: 3.0.7
 Summary: A wrapper library to access hydro quebec API and more
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: LGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc/-/issues
 Project-URL: Home-page, https://hydroqc.ca
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt` & `Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/LICENSE` & `Hydro-Quebec-API-Wrapper-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/PKG-INFO` & `Hydro-Quebec-API-Wrapper-3.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hydro-Quebec-API-Wrapper
-Version: 3.0.6
+Version: 3.0.7
 Summary: A wrapper library to access hydro quebec API and more
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: LGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc/-/issues
 Project-URL: Home-page, https://hydroqc.ca
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/README.md` & `Hydro-Quebec-API-Wrapper-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/config.default.yaml` & `Hydro-Quebec-API-Wrapper-3.0.7/config.default.yaml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/Makefile` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/make.bat` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/_static/hydroqc-logo-128.png` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo-128.png`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/_static/hydroqc-logo.svg` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo.svg`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/conf.py` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/external/description-des-codes-interruption.pdf` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/external/description-des-codes-interruption.pdf`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.contract.rst` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.contract.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.hydro_api.rst` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.hydro_api.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.peak.cpc.rst` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.cpc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.peak.dpc.rst` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.dpc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.rst` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/docs/source/reference/hydroqc.types.rst` & `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.types.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/examples/hydro.py` & `Hydro-Quebec-API-Wrapper-3.0.7/examples/hydro.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/account.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/account.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/__init__.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/common.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/common.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_d.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_d_cpc.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d_cpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_dpc.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_dt.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dt.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_m.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_m_gdp.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m_gdp.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/contract_residential.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_residential.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/contract/outage.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/outage.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/customer.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/customer.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/diagnostic.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/diagnostic.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/cache.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/cache.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/client.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/client.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/hydro_api/consts.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/consts.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 """
 # Always get the time using HydroQuebec Local Time
 REQUESTS_TIMEOUT = 30
 REQUESTS_TTL = 1
 
 HOST_LOGIN = "https://connexion.hydroquebec.com"
 HOST_SESSION = "https://session.hydroquebec.com"
-HOST_SERVICES = "https://cl-services.idp.hydroquebec.com"
-HOST_SPRING = "https://cl-ec-spring.hydroquebec.com"
+HOST_SERVICES = "https://cl-services.solutions.hydroquebec.com"
+HOST_SPRING = "https://cl-ec-lsw.solutions.hydroquebec.com"
 HOST_RB_SOL = "https://rb.solutions.hydroquebec.com"
 HOST_OUTAGES = "https://infopannes-services.solutions.hydroquebec.com"
 
 # Outages
 OUTAGES = f"{HOST_OUTAGES}/web/api/v1/lieux-conso/etats/"
 # OAUTH PATHS
 LOGIN_URL_1 = f"{HOST_LOGIN}/hqam/XUI/"  # not used
 LOGIN_URL_2 = f"{HOST_LOGIN}/hqam/json/serverinfo/*"  # not used
 AUTH_URL = f"{HOST_LOGIN}/hqam/json/realms/root/realms/clients/authenticate"
 SECURITY_URL = f"{HOST_SESSION}/config/security.json"
 TOKEN_URL = f"{HOST_LOGIN}/hqam/oauth2/access_token"
 SESSION_REFRESH_URL = f"{HOST_SESSION}/oauth2/callback/silent-refresh"
 AUTHORIZE_URL = f"{HOST_LOGIN}/hqam/oauth2/authorize"
-LOGIN_URL_6 = f"{HOST_SERVICES}/cl/prive/api/v3_0/conversion/codeAcces"
+LOGIN_URL_6 = f"{HOST_SERVICES}/web/prive/api/v3_0/conversion/codeAcces"
 CHECK_SESSION_URL = f"{HOST_LOGIN}/hqam/oauth2/connect/checkSession"
 # Initialization uri
-RELATION_URL = f"{HOST_SERVICES}/cl/prive/api/v1_0/relations"
+RELATION_URL = f"{HOST_SERVICES}/web/prive/api/v1_0/relations"
 
 FLEXD_DATA_URL = (
     f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesMoisHiverFlex"
 )
 FLEXD_PEAK_URL = f"{HOST_RB_SOL}/portraitweb/api/v3_0/conso"
 CONSO_CSV_URL = (
@@ -45,24 +45,24 @@
 )
 
 # TODO avoid all the /portail/ URLs
 SESSION_URL = f"{HOST_SPRING}/portail/prive/maj-session/"
 # TODO avoid all the /portail/ URLs
 CONTRACT_HTML_URL = f"{HOST_SPRING}/portail/fr/group/clientele/gerer-mon-compte"
 #
-INFOBASE_URL = f"{HOST_SERVICES}/cl/prive/api/v3_0/partenaires/infoBase"
+INFOBASE_URL = f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/infoBase"
 CONTRACT_SUMMARY_URL = (
-    f"{HOST_SERVICES}/cl/prive/api/v3_0/partenaires/"
+    f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/"
     "calculerSommaireContractuel?indMAJNombres=true"
 )
-CONTRACT_LIST_URL = f"{HOST_SERVICES}/cl/prive/api/v3_0/partenaires/contrats"
-# CONTRACT_URL_4 = (f"{HOST_SERVICES}/cl/prive/api/v3_0/partenaires/"
+CONTRACT_LIST_URL = f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/contrats"
+# CONTRACT_URL_4 = (f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/"
 #                  "calculerSommaireContractuel")
 
-CUSTOMER_INFO_URL = f"{HOST_SERVICES}/cl/prive/api/v3_0/partenaires/infoCompte"
+CUSTOMER_INFO_URL = f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/infoCompte"
 
 # TODO avoid all the /portail/ URLs
 PORTRAIT_URL = f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation"
 # TODO avoid all the /portail/ URLs
 PERIOD_DATA_URL = (
     f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesPeriodesConsommation"
@@ -95,12 +95,12 @@
 HOURLY_DATA_URL_2 = (
     f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesMeteoHoraires"  # not used
 )
 
 # CPC
 GET_CPC_API_URL = (
-    f"{HOST_SERVICES}/cl/prive/api/v3_0/tarificationDynamique/creditPointeCritique"
+    f"{HOST_SERVICES}/web/prive/api/v3_0/tarificationDynamique/creditPointeCritique"
 )
 
 # IS PORTAL RUNNING
 IS_HYDRO_PORTAL_UP_URL = f"{HOST_SESSION}/portail/fr/group/clientele/gerer-mon-compte"
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/logger.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/logger.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/consts.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/consts.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/handler.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/handler.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/cpc/peak.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/peak.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/consts.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/consts.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/handler.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/handler.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/peak/dpc/peak.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/peak.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/timerange.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/timerange.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/__init__.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/account.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/account.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/common.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/common.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/consump.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/consump.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/contract.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/contract.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/cpc.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/cpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/dpc.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/dpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/types/outage.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/outage.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/hydroqc/webuser.py` & `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/webuser.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/logo/hydroqc-logo-128.png` & `Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo-128.png`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/logo/hydroqc-logo.svg` & `Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo.svg`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/pyproject.toml` & `Hydro-Quebec-API-Wrapper-3.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/renovate.json` & `Hydro-Quebec-API-Wrapper-3.0.7/renovate.json`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_common.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_common.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_d.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_d_cpc.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d_cpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_dpc.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_dt.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dt.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_m.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/subtest_contract_m_gdp.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m_gdp.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/test_basic.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/test_timerange.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/test_timerange.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tests/tools.py` & `Hydro-Quebec-API-Wrapper-3.0.7/tests/tools.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.6/tox.ini` & `Hydro-Quebec-API-Wrapper-3.0.7/tox.ini`

 * *Files identical despite different names*

