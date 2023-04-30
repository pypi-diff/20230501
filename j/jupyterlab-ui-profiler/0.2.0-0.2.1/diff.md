# Comparing `tmp/jupyterlab_ui_profiler-0.2.0.tar.gz` & `tmp/jupyterlab_ui_profiler-0.2.1.tar.gz`

## Comparing `jupyterlab_ui_profiler-0.2.0.tar` & `jupyterlab_ui_profiler-0.2.1.tar`

### file list

```diff
@@ -1,106 +1,107 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.stylelintrc
--rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/babel.config.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jest.config.js
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/package.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/readthedocs.yml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/setup.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   400810 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/yarn.lock
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/make.bat
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/docs/source/_static/logo-icon.png
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyter-config/nb-config/jupyterlab_ui_profiler.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyter-config/server-config/jupyterlab_ui_profiler.json
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/_version.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/package.json
--rw-r--r--   0        0        0    65688 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/148.d0923e85cee15af0e9d9.js
--rw-r--r--   0        0        0   373774 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js.LICENSE.txt
--rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js
--rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/remoteEntry.2c015c9bba0ac87e826d.js
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/style.js
--rw-r--r--   0        0        0    58872 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/benchmark.ts
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/browserProfiler.d.ts
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/css.ts
--rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/dramaturg.ts
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/index.ts
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/jsBenchmarks.ts
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/lumino.tsx
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/profiler.ts
--rw-r--r--   0        0        0    18902 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/scenarios.ts
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/statistics.ts
--rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/styleBenchmarks.tsx
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/table.ts
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/templates.tsx
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/tokens.ts
--rw-r--r--   0        0        0    40154 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/ui.tsx
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/utils.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/__tests__/jupyterlab-ui-profiler.spec.ts
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/__tests__/statistics.spec.ts
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-base.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-execution.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-profile.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-group.json
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-usage.json
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-base.json
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-completer.json
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-debugger.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-menu-open.json
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-scroll.json
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-sidebars.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/schema/scenario-tabs.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-base.ts
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-execution.ts
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-profile.ts
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-group.ts
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-usage.ts
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule.ts
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-base.ts
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-completer.ts
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-debugger.ts
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-menu-open.ts
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-scroll.ts
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-sidebars.ts
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/src/types/_scenario-tabs.ts
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/package.json
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   131668 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts
--rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png
--rw-r--r--   0        0        0    28608 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png
--rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png
--rw-r--r--   0        0        0   103844 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png
--rw-r--r--   0        0        0   109606 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png
--rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png
--rw-r--r--   0        0        0    64015 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png
--rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png
--rw-r--r--   0        0        0   117877 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png
--rw-r--r--   0        0        0   102798 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png
--rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png
--rw-r--r--   0        0        0    58453 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/LICENSE
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/README.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.eslintignore
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.eslintrc.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.stylelintrc
+-rw-r--r--   0        0        0    10523 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/babel.config.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jest.config.js
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/package.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/readthedocs.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/setup.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0   400810 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/yarn.lock
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/make.bat
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/changelog.rst
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/docs/source/_static/logo-icon.png
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyter-config/nb-config/jupyterlab_ui_profiler.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyter-config/server-config/jupyterlab_ui_profiler.json
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/_version.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/package.json
+-rw-r--r--   0        0        0    66876 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/148.386a0716eefd6e346348.js
+-rw-r--r--   0        0        0   373774 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js.LICENSE.txt
+-rw-r--r--   0        0        0    11327 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js
+-rw-r--r--   0        0        0     7445 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/remoteEntry.b7edad4eeff456a5f798.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/style.js
+-rw-r--r--   0        0        0    58872 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/benchmark.ts
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/browserProfiler.d.ts
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/css.ts
+-rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/dramaturg.ts
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/index.ts
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/jsBenchmarks.ts
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/lumino.tsx
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/profiler.ts
+-rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/scenarios.ts
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/statistics.ts
+-rw-r--r--   0        0        0    17780 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/styleBenchmarks.tsx
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/table.ts
+-rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/templates.tsx
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/tokens.ts
+-rw-r--r--   0        0        0    40154 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/ui.tsx
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/utils.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/__tests__/jupyterlab-ui-profiler.spec.ts
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/__tests__/statistics.spec.ts
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-base.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-execution.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-profile.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-group.json
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-usage.json
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-base.json
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-completer.json
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-debugger.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-menu-open.json
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-scroll.json
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-sidebars.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/schema/scenario-tabs.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-base.ts
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-execution.ts
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-profile.ts
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-group.ts
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-usage.ts
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule.ts
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-base.ts
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-completer.ts
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-debugger.ts
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-menu-open.ts
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-scroll.ts
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-sidebars.ts
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/_scenario-tabs.ts
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/src/types/index.ts
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/package.json
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   131668 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png
+-rw-r--r--   0        0        0    28608 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png
+-rw-r--r--   0        0        0    19430 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png
+-rw-r--r--   0        0        0   103844 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png
+-rw-r--r--   0        0        0   109606 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png
+-rw-r--r--   0        0        0    48391 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png
+-rw-r--r--   0        0        0    64015 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png
+-rw-r--r--   0        0        0   117877 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png
+-rw-r--r--   0        0        0   102798 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png
+-rw-r--r--   0        0        0   123587 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png
+-rw-r--r--   0        0        0    58453 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 jupyterlab_ui_profiler-0.2.1/PKG-INFO
```

### Comparing `jupyterlab_ui_profiler-0.2.0/.eslintrc.js` & `jupyterlab_ui_profiler-0.2.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/CHANGELOG.md` & `jupyterlab_ui_profiler-0.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.1
+
+([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.2.0...308598c8f2f2c344fee6d9ccffd1c379f8b8ecbc))
+
+### Enhancements made
+
+- Expose option types for more convenient use downstream [#49](https://github.com/jupyterlab/ui-profiler/pull/49) ([@krassowski](https://github.com/krassowski))
+
+### Bugs fixed
+
+- Allow to open editor in the same area to support small screens [#48](https://github.com/jupyterlab/ui-profiler/pull/48) ([@krassowski](https://github.com/krassowski))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/ui-profiler/graphs/contributors?from=2023-04-23&to=2023-04-30&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Agithub-actions+updated%3A2023-04-23..2023-04-30&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Akrassowski+updated%3A2023-04-23..2023-04-30&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.2.0
 
 ([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.1.8...3c4d2c8f2f80ba5e81c16b1dea2b77d76c209766))
 
 ### Enhancements made
 
 - Separate profiler out of the user interface [#46](https://github.com/jupyterlab/ui-profiler/pull/46) ([@krassowski](https://github.com/krassowski))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/ui-profiler/graphs/contributors?from=2023-04-02&to=2023-04-23&type=c))
 
 [@krassowski](https://github.com/search?q=repo%3Ajupyterlab%2Fui-profiler+involves%3Akrassowski+updated%3A2023-04-02..2023-04-23&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.8
 
 ([Full Changelog](https://github.com/jupyterlab/ui-profiler/compare/v0.1.7...528461f6f554e6656475aa2054c3ec12240f65e5))
 
 ### Bugs fixed
 
 - Use `_version.py` auto-generated by Hatchling [#44](https://github.com/jupyterlab/ui-profiler/pull/44) ([@krassowski](https://github.com/krassowski))
```

### Comparing `jupyterlab_ui_profiler-0.2.0/RELEASE.md` & `jupyterlab_ui_profiler-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/jest.config.js` & `jupyterlab_ui_profiler-0.2.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/package.json` & `jupyterlab_ui_profiler-0.2.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.0/tsconfig.json` & `jupyterlab_ui_profiler-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/yarn.lock` & `jupyterlab_ui_profiler-0.2.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/docs/Makefile` & `jupyterlab_ui_profiler-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/docs/make.bat` & `jupyterlab_ui_profiler-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/docs/source/conf.py` & `jupyterlab_ui_profiler-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/docs/source/_static/logo-icon.png` & `jupyterlab_ui_profiler-0.2.1/docs/source/_static/logo-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/__init__.py` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/package.json` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b7edad4eeff456a5f798.js'}}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -47,15 +47,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/jupyterlab/ui-profiler",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2c015c9bba0ac87e826d.js",
+            "load": "static/remoteEntry.b7edad4eeff456a5f798.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_ui_profiler/labextension",
         "sharedPackages": {
             "@lumino/datagrid": {
                 "bundled": false,
@@ -108,9 +108,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/148.d0923e85cee15af0e9d9.js` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/148.386a0716eefd6e346348.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 "use strict";
 (self.webpackChunk_jupyterlab_ui_profiler = self.webpackChunk_jupyterlab_ui_profiler || []).push([
     [148], {
         8148: (e, t, n) => {
             n.r(t), n.d(t, {
                 IUIProfiler: () => we,
-                default: () => ze
+                default: () => He
             });
             var s = n(5687),
                 i = n(3033),
                 r = n(7986),
                 o = n(7280),
                 a = n(1467),
                 l = n(3169),
                 c = n(2502),
                 u = n(3443),
-                d = n(6271),
-                p = n.n(d),
+                p = n(6271),
+                d = n.n(p),
                 m = n(8820),
                 h = n(2583),
                 f = n(1526),
                 g = n(8142),
                 w = n(1840),
                 y = n(1641);
 
@@ -153,14 +153,18 @@
                 }) {
                     return async function(e, t = {
                         delay: 0
                     }, n = null) {
                         for (const s of e) await B(s, t, n)
                     }(e, t, this.element)
                 }
+                async isVisible() {
+                    const e = this.element.getBoundingClientRect();
+                    return !(0 === e.width || 0 === e.height)
+                }
                 waitForSelector(e, t) {
                     return O(e, {
                         ...t,
                         within: this.element
                     })
                 }
             }
@@ -342,89 +346,89 @@
                             i = x.quartile(e.times, 3),
                             r = i - s,
                             o = Math.min(s + 1.5 * r, t),
                             a = Math.max(i - 1.5 * r, n),
                             l = 200 / 3,
                             c = e => e / t * 750,
                             u = e.times.map((t => x.kernelDensityEstimate(e.times, t))),
-                            d = Math.max(...u),
+                            p = Math.max(...u),
                             m = Math.round(375),
                             h = t,
                             f = Math.ceil((h - 0) / m),
                             g = Array.from(Array(m), (() => [])),
                             w = new Array(e.times.length);
                         for (let t = 0; t < e.times.length; t++) {
                             const n = e.times[t],
                                 s = Math.floor(n / f);
                             g[s].push(t), w[t] = s
                         }
                         const y = e.times.map(((e, t) => {
                                 const n = w[t],
                                     s = g[n],
-                                    i = (s.indexOf(t) / s.length - .5) * u[t] / d * l;
-                                return p().createElement("g", null, p().createElement("title", null, x.round(e, 2), " ms, ", X(t), " repeat"), p().createElement("circle", {
+                                    i = (s.indexOf(t) / s.length - .5) * u[t] / p * l;
+                                return d().createElement("g", null, d().createElement("title", null, x.round(e, 2), " ms, ", X(t), " repeat"), d().createElement("circle", {
                                     cx: c(e),
                                     cy: 100 + i,
                                     r: 2,
                                     className: "point"
                                 }))
                             })),
                             b = [1, 2, 3].map((t => {
                                 const n = x.quartile(e.times, t),
                                     s = c(n),
                                     i = 100 - l / 2;
-                                return p().createElement("g", null, p().createElement("title", null, X(t), " quartile: ", x.round(n, 2), " ms"), p().createElement("line", {
+                                return d().createElement("g", null, d().createElement("title", null, X(t), " quartile: ", x.round(n, 2), " ms"), d().createElement("line", {
                                     x1: s,
                                     y1: i,
                                     x2: s,
                                     y2: i + l,
                                     className: "box-line"
                                 }))
                             }));
-                        return p().createElement("svg", {
+                        return d().createElement("svg", {
                             viewBox: "0 0 755 200",
                             className: "up-BoxPlot"
-                        }, y, p().createElement("g", null, p().createElement("title", null, "Lower whisker, max(lowest value, q1 - 1.5 * IQR) =", " ", x.round(a, 2), " ms"), p().createElement("line", {
+                        }, y, d().createElement("g", null, d().createElement("title", null, "Lower whisker, max(lowest value, q1 - 1.5 * IQR) =", " ", x.round(a, 2), " ms"), d().createElement("line", {
                             x1: c(a),
                             y1: 100,
                             x2: c(s),
                             y2: 100,
                             className: "whisker"
-                        })), p().createElement("g", null, p().createElement("title", null, "Upper whisker, min(higher value, q3 + 1.5 * IQR) =", " ", x.round(o, 2), " ms"), p().createElement("line", {
+                        })), d().createElement("g", null, d().createElement("title", null, "Upper whisker, min(higher value, q3 + 1.5 * IQR) =", " ", x.round(o, 2), " ms"), d().createElement("line", {
                             x1: c(i),
                             y1: 100,
                             x2: c(o),
                             y2: 100,
                             className: "whisker"
-                        })), p().createElement("rect", {
+                        })), d().createElement("rect", {
                             x: c(s),
                             y: 100 - l / 2,
                             width: c(i - s),
                             height: l,
                             className: "box"
-                        }), b, p().createElement("line", {
+                        }), b, d().createElement("line", {
                             x1: "0",
                             x2: 750,
                             y1: 185,
                             y2: 185,
                             className: "timeline"
-                        }), p().createElement("text", {
+                        }), d().createElement("text", {
                             x: "0",
                             y: 200,
                             className: "tickLabel"
-                        }, "0ms"), p().createElement("text", {
+                        }, "0ms"), d().createElement("text", {
                             x: 750,
                             y: 200,
                             style: {
                                 textAnchor: "end"
                             },
                             className: "tickLabel"
                         }, Math.round(t), "ms"))
                     }));
-                    return p().createElement(p().Fragment, null, t)
+                    return d().createElement(d().Fragment, null, t)
                 }
             };
 
             function* q(e) {
                 let t = new Map;
                 for (const n of e.samples) {
                     const s = n.timestamp;
@@ -470,15 +474,15 @@
                         name: s.name,
                         column: s.column,
                         line: s.line,
                         time: n
                     }
                 }))
             }
-            const $ = {
+            const W = {
                     id: "self-profile",
                     name: "Profile JavaScript",
                     configSchema: JSON.parse('{"title":"Profile Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":100},"scale":{"title":"Profiling scale","description":"Whether to take multiple profiles, one for each repeat (mico) or one profile averaging across all repeats (macro). Macro-profiling includes setup and cleanup steps which may bias the results for scenarios where expensive operations are performed in these steps. Micro-profiling may be unsuitable for very fast scenarios, and when the browser limits the sampling interval.","type":"string","enum":["micro","macro"],"default":"micro"},"sampleInterval":{"title":"Sample interval","description":"Sampling interval (in milliseconds). Browsers are not required to take samples at this rate and may increase it (Chrome uses 16ms on Windows and 10ms elsewhere).","type":"integer","exclusiveMinimum":0,"default":5},"maxBufferSize":{"title":"Sample buffer size limit","description":"When the limit of samples gets exceeded, the profiling will stop prematurely.","type":"number","exclusiveMinimum":0,"default":10000}},"required":["repeats","scale","sampleInterval","maxBufferSize"]}'),
                     run: async (e, t, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
@@ -537,16 +541,16 @@
                             totalTime: Date.now() - a,
                             type: "profile",
                             interrupted: i
                         }
                     },
                     isAvailable: () => void 0 !== window.Profiler,
                     render: function(e) {
-                        const t = p().useRef(null),
-                            [n, s] = p().useState(0);
+                        const t = d().useRef(null),
+                            [n, s] = d().useState(0);
                         if (null === t.current || t.current.stateSource !== e.outcome) {
                             const n = {};
                             for (const t of e.outcome.results)
                                 for (const e of t.traces)
                                     for (const t of L(e)) {
                                         const e = [t.name, t.resource, t.column, t.line].join("-");
                                         if (e in n) n[e].times.push(t.time), n[e].totalTime += t.time, n[e].calls += 1;
@@ -564,89 +568,89 @@
                                         }
                                     }
                             const s = [...Object.values(n)].filter((e => {
                                 const t = void 0 === e.resource && "Profiler" === e.name,
                                     n = e.resource && (e.resource.includes("@jupyterlab-benchmarks/ui-profiler") || e.resource.includes("@jupyterlab/ui-profiler"));
                                 return !t && !n
                             }));
-                            0 !== s.length ? t.current = new G({
+                            0 !== s.length ? t.current = new V({
                                 measurements: s,
                                 stateSource: e.outcome,
                                 sortColumn: "totalTime",
                                 lowerIsBetter: !0
                             }) : t.current = null
                         }
-                        return n > e.outcome.results[0].traces.length ? (s(0), p().createElement(p().Fragment, null)) : p().createElement(p().Fragment, null, p().createElement("select", {
+                        return n > e.outcome.results[0].traces.length ? (s(0), d().createElement(d().Fragment, null)) : d().createElement(d().Fragment, null, d().createElement("select", {
                             value: n,
                             onChange: e => {
                                 s(Number(e.target.value))
                             },
                             className: "up-trace-selector"
-                        }, e.outcome.results[0].traces.map(((e, t) => p().createElement("option", {
+                        }, e.outcome.results[0].traces.map(((e, t) => d().createElement("option", {
                             value: t,
                             key: "trace-" + t
-                        }, "Trace ", t, " (", e.samples.length, " samples)")))), p().createElement(Y, {
+                        }, "Trace ", t, " (", e.samples.length, " samples)")))), d().createElement(Y, {
                             trace: e.outcome.results[0].traces[n],
                             itemHeight: 20
-                        }), t.current ? p().createElement(K, {
+                        }), t.current ? d().createElement(K, {
                             widget: t.current
                         }) : "No results available. Reduce sampling interval, use macro mode, and/or increase the number of repeats.")
                     }
                 },
-                W = e => {
+                $ = e => {
                     const t = e.load("jupyterlab"),
-                        n = e => p().createElement("div", {
+                        n = e => d().createElement("div", {
                             className: e.className
-                        }, p().createElement(e.TitleField, {
+                        }, d().createElement(e.TitleField, {
                             title: e.title,
                             required: e.required,
                             id: `${e.idSchema.$id}-title`
-                        }), p().createElement(e.DescriptionField, {
+                        }), d().createElement(e.DescriptionField, {
                             id: `${e.idSchema.$id}-description`,
                             description: e.schema.description ?? ""
-                        }), e.items.map((e => p().createElement("div", {
+                        }), e.items.map((e => d().createElement("div", {
                             key: e.key,
                             className: e.className
-                        }, e.children, p().createElement("div", {
+                        }, e.children, d().createElement("div", {
                             className: "jp-ArrayOperations"
-                        }, p().createElement("button", {
+                        }, d().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onReorderClick(e.index, e.index - 1),
                             disabled: !e.hasMoveUp
-                        }, t.__("Move Up")), p().createElement("button", {
+                        }, t.__("Move Up")), d().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onReorderClick(e.index, e.index + 1),
                             disabled: !e.hasMoveDown
-                        }, t.__("Move Down")), p().createElement("button", {
+                        }, t.__("Move Down")), d().createElement("button", {
                             className: "jp-mod-styled jp-mod-warn",
                             onClick: e.onDropIndexClick(e.index),
                             disabled: !e.hasRemove
-                        }, t.__("Remove")))))), e.canAdd && p().createElement("button", {
+                        }, t.__("Remove")))))), e.canAdd && d().createElement("button", {
                             className: "jp-mod-styled jp-mod-reject",
                             onClick: e.onAddClick
                         }, t.__("Add")));
                     return n.displayName = "JupyterLabArrayTemplate", n
                 },
                 z = e => {
                     const t = e.load("jupyterlab"),
                         n = e => {
                             const {
                                 TitleField: n,
                                 DescriptionField: s
                             } = e;
-                            return p().createElement("fieldset", {
+                            return d().createElement("fieldset", {
                                 id: e.idSchema.$id
-                            }, (e.uiSchema["ui:title"] || e.title) && p().createElement(n, {
+                            }, (e.uiSchema["ui:title"] || e.title) && d().createElement(n, {
                                 id: `${e.idSchema.$id}__title`,
                                 title: e.title || e.uiSchema["ui:title"],
                                 required: e.required
-                            }), e.description && p().createElement(s, {
+                            }), e.description && d().createElement(s, {
                                 id: `${e.idSchema.$id}__description`,
                                 description: e.description
-                            }), e.properties.map((e => e.content)), u.P6.canExpand(e.schema, e.uiSchema, e.formData) && p().createElement("button", {
+                            }), e.properties.map((e => e.content)), u.P6.canExpand(e.schema, e.uiSchema, e.formData) && d().createElement("button", {
                                 className: "jp-mod-styled jp-mod-reject",
                                 onClick: e.onAddClick(e.schema),
                                 disabled: e.disabled || e.readonly
                             }, t.__("Add")))
                         };
                     return n.displayName = "JupyterLabObjectTemplate", n
                 },
@@ -658,41 +662,41 @@
                                 label: s,
                                 displayLabel: i,
                                 id: r,
                                 errors: o,
                                 rawErrors: a,
                                 children: l,
                                 onKeyChange: c,
-                                onDropPropertyClick: d
+                                onDropPropertyClick: p
                             } = e, m = r.split("_");
                             m.shift();
                             const h = "" === m.join("."),
                                 f = !h && "object" !== n.type,
                                 g = Object.prototype.hasOwnProperty.call(n, u.P6.ADDITIONAL_PROPERTY_FLAG);
-                            return p().createElement("div", {
+                            return d().createElement("div", {
                                 className: "form-group " + (i || "boolean" === n.type ? "small-field" : "")
-                            }, a && p().createElement("div", {
+                            }, a && d().createElement("div", {
                                 className: "jp-modifiedIndicator jp-errorIndicator"
-                            }), p().createElement("div", {
+                            }), d().createElement("div", {
                                 className: "jp-FormGroup-content"
-                            }, i && !h && s && !g && p().createElement("h3", {
+                            }, i && !h && s && !g && d().createElement("h3", {
                                 className: "jp-FormGroup-fieldLabel jp-FormGroup-contentItem"
-                            }, s), g && p().createElement("input", {
+                            }, s), g && d().createElement("input", {
                                 className: "jp-FormGroup-contentItem jp-mod-styled",
                                 type: "text",
                                 onBlur: e => c(e.target.value),
                                 defaultValue: s
-                            }), p().createElement("div", {
+                            }), d().createElement("div", {
                                 className: h ? "jp-root" : "object" === n.type ? "jp-objectFieldWrapper" : "jp-inputFieldWrapper jp-FormGroup-contentItem"
-                            }, l), g && p().createElement("button", {
+                            }, l), g && d().createElement("button", {
                                 className: "jp-FormGroup-contentItem jp-mod-styled jp-mod-warn jp-FormGroup-removeButton",
-                                onClick: d(s)
-                            }, t.__("Remove")), n.description && f && p().createElement("div", {
+                                onClick: p(s)
+                            }, t.__("Remove")), n.description && f && d().createElement("div", {
                                 className: "jp-FormGroup-description"
-                            }, n.description), p().createElement("div", {
+                            }, n.description), d().createElement("div", {
                                 className: "validationErrors"
                             }, o)))
                         };
                     return n.displayName = "JupyterLabFieldTemplate", n
                 };
             var U = n(5414);
             class J extends U.BasicMouseHandler {
@@ -735,15 +739,15 @@
                 setupColumnWidths() {
                     this.fitColumnNames("all");
                     for (const [e, t] of Object.entries(this.columnWidths)) {
                         const n = this.columnNames.indexOf(e); - 1 !== n && this.resizeColumn("body", n, t)
                     }
                 }
             }
-            class G extends Q {
+            class V extends Q {
                 constructor(e) {
                     super(), this.columnWidths = {
                         source: 325,
                         content: 100,
                         selector: 175,
                         rulesInBlock: 450,
                         IQM: 55,
@@ -824,45 +828,45 @@
                 handleClick(e) {
                     if ("column-header" === e.region) {
                         const t = this.dataModel.data(e.region, e.row, e.column);
                         t === this.sortColumn ? this.sortOrder = "ascending" === this.sortOrder ? "descending" : "ascending" : this.sortColumn = t, this._setupDataModel(!0), this.update()
                     }
                 }
             }
-            var V = n(8832);
+            var G = n(8832);
             const K = e => {
-                const t = p().useRef(null);
-                return p().useEffect((() => {
+                const t = d().useRef(null);
+                return d().useEffect((() => {
                     const n = e.widget;
-                    V.Widget.attach(n, t.current);
+                    G.Widget.attach(n, t.current);
                     const s = new ResizeObserver((t => {
                         e.widget.fit()
                     }));
                     return s.observe(t.current), () => {
-                        V.Widget.detach(n), s.disconnect()
+                        G.Widget.detach(n), s.disconnect()
                     }
-                }), [e.widget]), p().createElement("div", {
+                }), [e.widget]), d().createElement("div", {
                     className: "up-LuminoWidgetWrapper",
                     ref: t
                 })
             };
-            class Y extends p().Component {
+            class Y extends d().Component {
                 constructor(e) {
                     super(e), this.deepest = 0, this.contentWidth = 100, this.contentHeight = 100, this.initialWidth = 100, this.state = {
                         scale: {
                             x: 1,
                             y: 1
                         },
                         position: {
                             x: 0,
                             y: 0
                         },
                         dimensions: null,
                         inDrag: !1
-                    }, this.handleMouseUp = this.handleMouseUp.bind(this), this.handleMouseDown = this.handleMouseDown.bind(this), this.handleMouseMove = this.handleMouseMove.bind(this), this.handleWheel = this.handleWheel.bind(this), this.container = p().createRef(), this.resizeObserver = new ResizeObserver(this.updateSizeInfo.bind(this))
+                    }, this.handleMouseUp = this.handleMouseUp.bind(this), this.handleMouseDown = this.handleMouseDown.bind(this), this.handleMouseMove = this.handleMouseMove.bind(this), this.handleWheel = this.handleWheel.bind(this), this.container = d().createRef(), this.resizeObserver = new ResizeObserver(this.updateSizeInfo.bind(this))
                 }
                 componentDidMount() {
                     const e = this.props.trace,
                         t = e.samples[0].timestamp,
                         n = Math.max(...e.samples.map((e => e.timestamp - t))),
                         s = {
                             width: this.container.current.offsetWidth,
@@ -920,25 +924,25 @@
                     }), document.addEventListener("mousemove", this.handleMouseMove), document.addEventListener("mouseup", this.handleMouseUp)
                 }
                 renderContent() {
                     const {
                         trace: e,
                         itemHeight: t
                     } = this.props;
-                    if (!e.samples) return p().createElement("div", null, "No samples in trace");
+                    if (!e.samples) return d().createElement("div", null, "No samples in trace");
                     const n = e.samples[0].timestamp,
                         s = [...q(e)];
                     this.deepest = Math.max(...s.map((e => e.stackDepth)));
                     const i = this.state.scale,
                         r = e.samples.map(((t, s) => {
                             const r = {
                                 width: (e.samples[s + 1]?.timestamp - t.timestamp) * i.x,
                                 left: (t.timestamp - n) * i.x
                             };
-                            return p().createElement("div", {
+                            return d().createElement("div", {
                                 className: "up-ProfileTrace-sample",
                                 key: "sample-" + s,
                                 style: r
                             })
                         }));
                     let o = 0;
                     const a = s.map(((s, r) => {
@@ -948,32 +952,32 @@
                         o = Math.max(o, l + c);
                         const u = {
                             width: c,
                             top: (s.stackDepth - 1) * t * i.y,
                             left: l,
                             height: t
                         };
-                        return p().createElement("div", {
+                        return d().createElement("div", {
                             className: "up-ProfileTrace-frame " + (void 0 === a.resourceId ? "up-ProfileTrace-frame-native" : ""),
                             key: "frame-" + r,
                             style: u,
                             title: [a.name, x.round(s.duration, 1) + "ms"].join("\n")
                         }, a.name)
                     }));
-                    return this.contentWidth = o, this.contentHeight = (2 + this.deepest) * this.props.itemHeight * i.y, p().createElement("div", {
+                    return this.contentWidth = o, this.contentHeight = (2 + this.deepest) * this.props.itemHeight * i.y, d().createElement("div", {
                         className: "up-ProfileTrace-content",
                         style: {
                             transform: `translate(${this.state.position.x}px, ${this.state.position.y}px)`,
                             width: o + "px",
                             height: this.contentHeight + "px"
                         }
                     }, a, r)
                 }
                 render() {
-                    return p().createElement("div", {
+                    return d().createElement("div", {
                         className: "up-ProfileTrace",
                         onWheel: this.handleWheel,
                         onMouseDown: this.handleMouseDown,
                         ref: this.container
                     }, this.state.dimensions ? this.renderContent() : "Loading")
                 }
             }
@@ -1005,33 +1009,33 @@
                     const t = JSON.parse(e.content);
                     t.result && (t.outcome = t.result), this.handleResult(t)
                 }
                 async upload(e) {
                     return await this.ensureResultsDirectory(), this.props.upload(e)
                 }
                 render() {
-                    return p().createElement("div", {
+                    return d().createElement("div", {
                         className: "up-UIProfiler"
-                    }, p().createElement(re, Object.assign({
+                    }, d().createElement(re, Object.assign({
                         onResult: this.handleResult,
                         progress: this.progress
                     }, this.props, {
                         upload: this.upload
-                    })), p().createElement(ee, Object.assign({
+                    })), d().createElement(ee, Object.assign({
                         resultAdded: this.resultAdded,
                         manager: this.manager,
                         onSelect: this.loadResult
-                    }, this.props)), p().createElement(te, {
+                    }, this.props)), d().createElement(te, {
                         result: this.result,
                         scenarios: this.props.profiler.scenarios,
                         benchmarks: this.props.profiler.benchmarks.filter((e => e.id === this.result?.benchmark))
                     }))
                 }
             }
-            class ee extends p().Component {
+            class ee extends d().Component {
                 constructor(e) {
                     super(e), this._handle = null, this.state = {
                         files: [],
                         current: null
                     }, this.update(), this.update = this.update.bind(this), this.props.resultAdded.connect((async (e, t) => {
                         await this.update(), this.setState({
                             current: se(t)
@@ -1047,112 +1051,112 @@
                 componentDidMount() {
                     this._handle = window.setInterval(this.update, 2e3)
                 }
                 componentWillUnmount() {
                     null !== this._handle && window.clearInterval(this._handle)
                 }
                 render() {
-                    let e = this.state.files.map((e => p().createElement("li", {
+                    let e = this.state.files.map((e => d().createElement("li", {
                         className: this.state.current === e.name ? "up-BenchmarkHistory-file up-BenchmarkHistory-file-active" : "up-BenchmarkHistory-file",
                         key: e.name,
                         onClick: () => {
                             this.props.onSelect(e), this.setState({
                                 current: e.path
                             })
                         }
                     }, e.name.replace(".profile.json", ""))));
-                    return this.state.files.length || (e = [p().createElement("li", {
+                    return this.state.files.length || (e = [d().createElement("li", {
                         className: "up-BenchmarkHistory-entry"
-                    }, "(No previous results found)")]), p().createElement("div", {
+                    }, "(No previous results found)")]), d().createElement("div", {
                         className: "up-BenchmarkHistory"
-                    }, p().createElement("h3", {
+                    }, d().createElement("h3", {
                         className: "up-widget-heading"
-                    }, "History"), p().createElement("ul", {
+                    }, "History"), d().createElement("ul", {
                         className: "up-BenchmarkHistory-files"
                     }, e))
                 }
             }
-            class te extends p().Component {
+            class te extends d().Component {
                 constructor() {
                     super(...arguments), this._table = null, this._previousResult = null
                 }
                 render() {
                     const {
                         result: e,
                         benchmarks: t,
                         scenarios: n
-                    } = this.props, s = e => p().createElement("div", {
+                    } = this.props, s = e => d().createElement("div", {
                         className: "up-BenchmarkResult"
                     }, e);
-                    if (!e) return s(p().createElement("div", null, "Choose a result from the panel, or run a new benchmark."));
+                    if (!e) return s(d().createElement("div", null, "Choose a result from the panel, or run a new benchmark."));
                     const i = n.find((t => t.id === e.scenario)),
                         r = t.find((t => t.id === e.benchmark));
-                    if (!i) return s(p().createElement("div", null, "Unknown scenario: ", e.scenario));
-                    if (!r) return s(p().createElement("div", null, "Unknown benchmark: ", e.benchmark));
-                    r.render || this._previousResult === e.id || ("time" === e.outcome.type ? this._table = new G({
+                    if (!i) return s(d().createElement("div", null, "Unknown scenario: ", e.scenario));
+                    if (!r) return s(d().createElement("div", null, "Unknown benchmark: ", e.benchmark));
+                    r.render || this._previousResult === e.id || ("time" === e.outcome.type ? this._table = new V({
                         measurements: e.outcome.results,
                         reference: e.outcome.reference,
                         sortColumn: r.sortColumn,
                         stateSource: null,
                         lowerIsBetter: !1
                     }) : this._table = null);
                     const o = [...Object.entries(e.outcome.tags)].map((([e, t]) => `${e}:  ${t}`)).join("\n"),
                         a = x.sum([...Object.values(e.outcome.tags)]);
-                    return s(p().createElement(p().Fragment, null, p().createElement("div", {
+                    return s(d().createElement(d().Fragment, null, d().createElement("div", {
                         className: "up-BenchmarkResult-summary"
-                    }, p().createElement("div", {
+                    }, d().createElement("div", {
                         className: "up-BenchmarkResult-benchmarkInfo"
-                    }, p().createElement("div", null, r.name, " ", i.name), "time" === e.outcome.type ? (l = e.outcome, p().createElement(p().Fragment, null, p().createElement("div", {
+                    }, d().createElement("div", null, r.name, " ", i.name), "time" === e.outcome.type ? (l = e.outcome, d().createElement(d().Fragment, null, d().createElement("div", {
                         title: [...l.reference].sort().map(x.round).join(" ms\n") + " ms"
-                    }, "Reference: IQM:", " ", x.round(x.interQuartileMean(l.reference), 1), " [", x.round(x.quartile(l.reference, 1), 1), " –", " ", x.round(x.quartile(l.reference, 3), 1), "] ms, mean:", " ", x.round(x.mean(l.reference), 1), " ms, min:", " ", x.round(x.min(l.reference), 1), " ms"), p().createElement("div", null, "Total time: ", k(l.totalTime)))) : function(e) {
+                    }, "Reference: IQM:", " ", x.round(x.interQuartileMean(l.reference), 1), " [", x.round(x.quartile(l.reference, 1), 1), " –", " ", x.round(x.quartile(l.reference, 3), 1), "] ms, mean:", " ", x.round(x.mean(l.reference), 1), " ms, min:", " ", x.round(x.min(l.reference), 1), " ms"), d().createElement("div", null, "Total time: ", k(l.totalTime)))) : function(e) {
                         const t = e.results[0];
-                        return p().createElement(p().Fragment, null, p().createElement("div", null, "Traces: ", t.traces.length, ". Average number of samples:", " ", x.round(x.mean(t.traces.map((e => e.samples.length))), 1), ", frames:", " ", x.round(x.mean(t.traces.map((e => e.frames.length))), 1), ".", " ", p().createElement("span", {
+                        return d().createElement(d().Fragment, null, d().createElement("div", null, "Traces: ", t.traces.length, ". Average number of samples:", " ", x.round(x.mean(t.traces.map((e => e.samples.length))), 1), ", frames:", " ", x.round(x.mean(t.traces.map((e => e.frames.length))), 1), ".", " ", d().createElement("span", {
                             title: "Average recorderd: " + x.round(t.averageSampleInterval, 1)
-                        }, "Sampling interval: ", x.round(t.samplingInterval, 1), " ms")), p().createElement("div", null, "Total time: ", k(e.totalTime)))
-                    }(e.outcome)), p().createElement("div", {
+                        }, "Sampling interval: ", x.round(t.samplingInterval, 1), " ms")), d().createElement("div", null, "Total time: ", k(e.totalTime)))
+                    }(e.outcome)), d().createElement("div", {
                         className: "up-BenchmarkResult-environmentInfo"
-                    }, p().createElement("div", null, "Application: ", e.jupyter.client, " ", e.jupyter.version, " ", e.jupyter.devMode ? "dev mode" : null, " ", e.jupyter.mode), p().createElement("div", null, p().createElement("span", {
+                    }, d().createElement("div", null, "Application: ", e.jupyter.client, " ", e.jupyter.version, " ", e.jupyter.devMode ? "dev mode" : null, " ", e.jupyter.mode), d().createElement("div", null, d().createElement("span", {
                         title: e.userAgent
                     }, "Browser: ", function(e) {
                         const t = [/Firefox\/\d+/, /OPR\/\d+/, /Edg\/\d+/, /Mobile\/.* Safari\/\d+/, /Chrome\/\d+/];
                         for (const n of t) {
                             const t = e.match(n);
                             if (t) return t[0]
                         }
                         return "Unknown browser"
-                    }(e.userAgent)), ", ", p().createElement("span", {
+                    }(e.userAgent)), ", ", d().createElement("span", {
                         title: o
-                    }, "DOM Elements: ", a)), p().createElement("div", null, "CPU cores: ", e.hardwareConcurrency))), p().createElement("div", {
+                    }, "DOM Elements: ", a)), d().createElement("div", null, "CPU cores: ", e.hardwareConcurrency))), d().createElement("div", {
                         className: "up-BenchmarkResult-options"
-                    }, p().createElement("details", null, p().createElement("summary", null, "Options"), p().createElement("div", {
+                    }, d().createElement("details", null, d().createElement("summary", null, "Options"), d().createElement("div", {
                         className: "up-BenchmarkResult-options-benchmark"
-                    }, p().createElement("b", null, "Benchmark"), p().createElement(y.w, {
+                    }, d().createElement("b", null, "Benchmark"), d().createElement(y.w, {
                         data: e.options.benchmark
-                    })), p().createElement("div", {
+                    })), d().createElement("div", {
                         className: "up-BenchmarkResult-options-scenario"
-                    }, p().createElement("b", null, "Scenario"), void 0 === e.options.scenario ? p().createElement("div", null, "No options") : p().createElement(y.w, {
+                    }, d().createElement("b", null, "Scenario"), void 0 === e.options.scenario ? d().createElement("div", null, "No options") : d().createElement(y.w, {
                         data: e.options.scenario
-                    })))), p().createElement("div", {
+                    })))), d().createElement("div", {
                         className: "up-BenchmarkResult-details"
-                    }, r.interpretation ? p().createElement("details", null, p().createElement("summary", null, "Interpretation"), r.interpretation) : null, r.render ? p().createElement(r.render, {
+                    }, r.interpretation ? d().createElement("details", null, d().createElement("summary", null, "Interpretation"), r.interpretation) : null, r.render ? d().createElement(r.render, {
                         outcome: e.outcome
-                    }) : this._table ? p().createElement(K, {
+                    }) : this._table ? d().createElement(K, {
                         widget: this._table
                     }) : null)));
                     var l
                 }
             }
-            class ne extends p().Component {
+            class ne extends d().Component {
                 constructor() {
                     super(...arguments), this.start = null, this.end = null
                 }
                 render() {
-                    return p().createElement("div", {
+                    return d().createElement("div", {
                         className: "up-BenchmarkMonitor"
-                    }, p().createElement(i.UseSignal, {
+                    }, d().createElement(i.UseSignal, {
                         signal: this.props.progress,
                         initialArgs: {
                             percentage: -1
                         }
                     }, ((e, t) => {
                         t || (t = {
                             percentage: -1
@@ -1160,48 +1164,48 @@
                         let n = NaN,
                             s = NaN,
                             i = "up-mod-waiting";
                         if (t.interrupted && (i = "up-mod-interrupted"), t.errored && (i += " up-mod-errored"), this.start) {
                             const e = (100 === t.percentage || t.interrupted || t.errored) && this.end ? this.end : new Date;
                             this.end = e, n = e.getTime() - this.start.getTime(), t.interrupted || t.errored || (s = (100 - t.percentage) * n / t.percentage, i = 100 === t.percentage ? "up-mod-completed" : "")
                         }
-                        return p().createElement("div", {
+                        return d().createElement("div", {
                             className: i + " up-BenchmarkMonitor-content"
-                        }, p().createElement("div", null, "Elapsed: ", k(n), ". Remaining:", " ", k(s)), p().createElement(h.ProgressBar, {
+                        }, d().createElement("div", null, "Elapsed: ", k(n), ". Remaining:", " ", k(s)), d().createElement(h.ProgressBar, {
                             percentage: t.percentage
                         }))
                     })))
                 }
             }
 
             function se(e) {
                 return e.id + ".profile.json"
             }
 
             function ie(e) {
-                return p().createElement("div", {
+                return d().createElement("div", {
                     className: "rjsf"
-                }, p().createElement("div", {
+                }, d().createElement("div", {
                     className: "jp-root"
-                }, p().createElement("fieldset", null, p().createElement("legend", null, e.name, " configuration"), "No options available for ", e.name, ".")))
+                }, d().createElement("fieldset", null, d().createElement("legend", null, e.name, " configuration"), "No options available for ", e.name, ".")))
             }
-            class re extends p().Component {
+            class re extends d().Component {
                 constructor(e) {
                     super(e), this._config = {
                         scenarios: {},
                         benchmarks: {}
                     }, this._stop = new w.Signal(this);
                     const {
                         profiler: t
                     } = e;
                     this.state = {
                         benchmarks: 0 !== t.benchmarks.length ? [t.benchmarks[0]] : [],
                         scenarios: 0 !== t.scenarios.length ? [t.scenarios[0]] : [],
                         fieldTemplate: H(this.props.translator),
-                        arrayFieldTemplate: W(this.props.translator),
+                        arrayFieldTemplate: $(this.props.translator),
                         objectFieldTemplate: z(this.props.translator),
                         isRunning: !1
                     }, this.runSelected = this.runSelected.bind(this), this.stopCurrent = this.stopCurrent.bind(this)
                 }
                 async runBenchmark(e, t, n) {
                     return this.props.profiler.runBenchmark({
                         id: e.id,
@@ -1274,103 +1278,103 @@
                     this._stop.emit(), this.props.profiler.abortBenchmark()
                 }
                 render() {
                     const {
                         profiler: e
                     } = this.props, t = e.benchmarks.map((e => {
                         const t = !!e.isAvailable && !e.isAvailable();
-                        return p().createElement("label", {
+                        return d().createElement("label", {
                             key: e.id,
                             className: t ? "up-label-disabled" : "",
                             title: t ? "This benchmark is not available on this browser" : ""
-                        }, p().createElement("input", {
+                        }, d().createElement("input", {
                             type: "checkbox",
                             defaultChecked: this.state.benchmarks.includes(e),
                             className: "up-BenchmarkLauncher-choice-input",
                             disabled: t,
                             value: e.id
                         }), e.name)
-                    })), n = e.scenarios.map((e => p().createElement("label", {
+                    })), n = e.scenarios.map((e => d().createElement("label", {
                         key: e.id
-                    }, p().createElement("input", {
+                    }, d().createElement("input", {
                         type: "checkbox",
                         defaultChecked: this.state.scenarios.includes(e),
                         className: "up-BenchmarkLauncher-choice-input",
                         value: e.id
                     }), e.name)));
-                    return p().createElement("div", {
+                    return d().createElement("div", {
                         className: "up-BenchmarkLauncher",
                         style: {
                             height: "450px"
                         }
-                    }, p().createElement("h3", {
+                    }, d().createElement("h3", {
                         className: "up-widget-heading"
-                    }, "Launch"), p().createElement("div", {
+                    }, "Launch"), d().createElement("div", {
                         className: "up-BenchmarkLauncher-cards"
-                    }, p().createElement("div", {
+                    }, d().createElement("div", {
                         className: "up-BenchmarkLauncher-card"
-                    }, p().createElement("h4", {
+                    }, d().createElement("h4", {
                         className: "up-card-heading"
-                    }, "Benchmark"), p().createElement("div", {
+                    }, "Benchmark"), d().createElement("div", {
                         className: "up-BenchmarkLauncher-choices",
                         onChange: this.onBenchmarkChanged.bind(this)
-                    }, t), p().createElement("div", {
+                    }, t), d().createElement("div", {
                         className: "up-BenchmarkLauncher-forms"
                     }, this.state.benchmarks.map((e => {
                         const t = e.configSchema.properties;
-                        return t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", p().createElement(u.ZP, {
+                        return t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", d().createElement(u.ZP, {
                             key: "up-profiler-benchmark-" + e.id,
                             schema: e.configSchema,
                             idPrefix: "up-profiler-benchmark",
                             onChange: t => {
                                 this._config.benchmarks[e.id] = t.formData
                             },
                             formData: this._config.benchmarks[e.id],
                             FieldTemplate: this.state.fieldTemplate,
                             ArrayFieldTemplate: this.state.arrayFieldTemplate,
                             ObjectFieldTemplate: this.state.objectFieldTemplate,
                             liveValidate: !0
-                        })) : p().createElement(ie, {
+                        })) : d().createElement(ie, {
                             name: e.name
                         })
-                    })))), p().createElement("div", {
+                    })))), d().createElement("div", {
                         className: "up-BenchmarkLauncher-card"
-                    }, p().createElement("h4", {
+                    }, d().createElement("h4", {
                         className: "up-card-heading"
-                    }, "Scenario"), p().createElement("div", {
+                    }, "Scenario"), d().createElement("div", {
                         className: "up-BenchmarkLauncher-choices",
                         onChange: this.onScenarioChanged.bind(this)
-                    }, n), p().createElement("div", {
+                    }, n), d().createElement("div", {
                         className: "up-BenchmarkLauncher-forms"
                     }, this.state.scenarios.map((e => {
                         const t = e.configSchema?.properties;
-                        return e.configSchema && t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", p().createElement(u.ZP, {
+                        return e.configSchema && t && 0 !== Object.keys(t).length ? (e.configSchema.title = e.name + " configuration", d().createElement(u.ZP, {
                             key: "up-profiler-scenario-" + e.id,
                             schema: e.configSchema,
                             idPrefix: "up-profiler-scenario-" + e.id,
                             onChange: t => {
                                 this._config.scenarios[e.id] = t.formData
                             },
                             formData: this._config.scenarios[e.id],
                             FieldTemplate: this.state.fieldTemplate,
                             ArrayFieldTemplate: this.state.arrayFieldTemplate,
                             ObjectFieldTemplate: this.state.objectFieldTemplate,
                             liveValidate: !0
-                        })) : p().createElement(ie, {
+                        })) : d().createElement(ie, {
                             name: e.name
                         })
-                    }))))), p().createElement("div", {
+                    }))))), d().createElement("div", {
                         className: "up-BenchmarkLauncher-launchbar"
-                    }, p().createElement(ne, Object.assign({}, this.props)), p().createElement("div", {
+                    }, d().createElement(ne, Object.assign({}, this.props)), d().createElement("div", {
                         className: "up-BenchmarkLauncher-launchbar-buttons"
-                    }, p().createElement("button", {
+                    }, d().createElement("button", {
                         onClick: this.runSelected,
                         className: "jp-mod-styled jp-mod-accept" + (this.state.isRunning ? " jp-mod-hidden" : ""),
                         disabled: 0 === this.state.scenarios.length || 0 === this.state.benchmarks.length || this.state.isRunning
-                    }, "Start"), p().createElement("button", {
+                    }, "Start"), d().createElement("button", {
                         onClick: this.stopCurrent,
                         className: "jp-mod-styled jp-mod-warn" + (this.state.isRunning ? "" : " jp-mod-hidden"),
                         disabled: !this.state.isRunning
                     }, "Stop"))))
                 }
             }
             async function oe(e) {
@@ -1408,57 +1412,57 @@
                     }
                 }
                 return s
             }
             const le = JSON.parse('{"title":"Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5}}}'),
                 ce = JSON.parse('{"title":"Style Rule Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":3},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"}}}'),
                 ue = JSON.parse('{"title":"Style Rule Group Benchmark Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"(fa-|Icon|bp3|mod-hidden)"},"minBlocks":{"title":"Block size to start with","type":"integer","minimum":1,"default":3},"maxBlocks":{"title":"Maximal block size","type":"integer","minimum":1,"default":5},"sheetRandomizations":{"title":"Number of sheet randomizations","type":"integer","minimum":0,"default":5}}}'),
-                de = JSON.parse('{"title":"Style Rule Usage Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"::"},"excludeMatchPattern":{"title":"Regular expression to filter out classes used for rule discovery","type":"string","default":"(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)"}}}');
-            class pe extends Map {
+                pe = JSON.parse('{"title":"Style Rule Usage Options","type":"object","properties":{"repeats":{"title":"Number of repeats","type":"integer","minimum":1,"default":5},"skipPattern":{"title":"Regular expression to filter out rules","type":"string","default":"::"},"excludeMatchPattern":{"title":"Regular expression to filter out classes used for rule discovery","type":"string","default":"(fa-|jp-icon|Icon|lm-Widget|lm-mod-|jp-mod-|p-mod-|p-Widget)"}}}');
+            class de extends Map {
                 add(e, t) {
                     let n = this.get(e);
                     n || (n = new Set, this.set(e, n)), n.add(t)
                 }
                 countRulesUsage() {
                     const e = new Map;
                     for (const t of this.values())
                         for (const n of t.values()) e.set(n, (e.get(n) || 0) + 1);
                     return e
                 }
             }
             const me = {
                     id: "rule-usage",
                     name: "Style Rule Usage",
-                    configSchema: de,
+                    configSchema: pe,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
                         const r = () => {
                             i = !0
                         };
                         s?.connect(r);
                         const o = t.repeats || 3,
                             a = Date.now(),
                             l = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
                             c = t.excludeMatchPattern ? new RegExp(t.excludeMatchPattern, "g") : void 0;
                         e.setupSuite && await e.setupSuite();
                         const u = await D(e, 2 * o, !0);
                         console.log("Reference for", e.name, "is:", u);
-                        const d = {
+                        const p = {
                                 subtree: !0,
                                 childList: !0,
                                 attributes: !0
                             },
-                            p = new Set,
+                            d = new Set,
                             m = e => {
-                                for (const t of S(e)) p.add(t)
+                                for (const t of S(e)) d.add(t)
                             },
                             h = new MutationObserver(m);
-                        await M(), h.observe(document.body, d), await D(e, o, !0), await M(), m(h.takeRecords()), h.disconnect();
-                        const f = [...p].filter((e => e instanceof Element)).filter((e => "body" !== e.tagName.toLocaleLowerCase()));
-                        console.log("Relevant nodes:", p);
+                        await M(), h.observe(document.body, p), await D(e, o, !0), await M(), m(h.takeRecords()), h.disconnect();
+                        const f = [...d].filter((e => e instanceof Element)).filter((e => "body" !== e.tagName.toLocaleLowerCase()));
+                        console.log("Relevant nodes:", d);
                         const g = new Set([...f.map((e => [...e.classList.values()])).flat().filter((e => !c || !e.match(c)))]),
                             w = f.filter((e => e.id)).map((e => e.id));
                         console.log("Relevant class names:", g), console.log("Relevant IDs:", w);
                         const y = [],
                             k = [...document.querySelectorAll("style")],
                             v = await ae(k, {
                                 skipPattern: l
@@ -1476,27 +1480,27 @@
                                 }
                         }
                         const x = [...E];
                         n?.emit({
                             percentage: 50 / x.length
                         });
                         const j = new Map,
-                            N = new pe,
-                            C = new pe,
+                            N = new de,
+                            C = new de,
                             O = e => {
                                 const t = new Set;
                                 for (const n of S(e)) t.add(n);
                                 for (const e of t)
                                     if (e instanceof Element)
                                         for (const t of E) e.matches(t.selector) && (j.set(t.selector, (j.get(t.selector) || 0) + 1), C.add(e, t.selector));
                                 for (const e of E)
                                     for (const t of document.querySelectorAll(e.selector)) N.add(t, e.selector)
                             },
                             I = new MutationObserver(O);
-                        I.observe(document.body, d), await D(e, o, !0), await M(), O(I.takeRecords()), I.disconnect();
+                        I.observe(document.body, p), await D(e, o, !0), await M(), O(I.takeRecords()), I.disconnect();
                         const _ = C.countRulesUsage(),
                             T = N.countRulesUsage();
                         for (let t = 0; t < x.length && !i; t++) {
                             n?.emit({
                                 percentage: 100 * (t + .5) / x.length
                             });
                             const s = x[t];
@@ -1519,15 +1523,15 @@
                             tags: b(),
                             totalTime: Date.now() - a,
                             type: "time",
                             interrupted: i
                         }
                     },
                     sortColumn: "elementsSeen",
-                    interpretation: p().createElement(p().Fragment, null, p().createElement("ul", null, p().createElement("li", null, p().createElement("code", null, "elementsSeen"), ": how many elements were seen on the entire page when executing the scenario."), p().createElement("li", null, p().createElement("code", null, "elementsTouched"), ": how many elements were modified or in the subtree of a modified element when executing the scenario."), p().createElement("li", null, p().createElement("code", null, "touchCount"), ": upper bound on how many times the rule matched an element (will be high for rules matching many elements, and for rules matching a single element that is repeatedly modified in the chosen scenario).")), p().createElement("div", null, "Low number of ", p().createElement("code", null, "elementsSeen"), " suggest potentially unused rule. Negative ", p().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
+                    interpretation: d().createElement(d().Fragment, null, d().createElement("ul", null, d().createElement("li", null, d().createElement("code", null, "elementsSeen"), ": how many elements were seen on the entire page when executing the scenario."), d().createElement("li", null, d().createElement("code", null, "elementsTouched"), ": how many elements were modified or in the subtree of a modified element when executing the scenario."), d().createElement("li", null, d().createElement("code", null, "touchCount"), ": upper bound on how many times the rule matched an element (will be high for rules matching many elements, and for rules matching a single element that is repeatedly modified in the chosen scenario).")), d().createElement("div", null, "Low number of ", d().createElement("code", null, "elementsSeen"), " suggest potentially unused rule. Negative ", d().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
                 },
                 he = {
                     id: "style-sheet",
                     name: "Style Sheets",
                     configSchema: le,
                     run: async (e, t = {}, n, s) => {
                         const i = t.repeats || 3,
@@ -1537,33 +1541,33 @@
                             o = !0
                         };
                         s?.connect(a), e.setupSuite && await e.setupSuite();
                         const l = [...document.querySelectorAll("style")],
                             c = await D(e, 2 * i, !0);
                         console.log("Reference for", e.name, "is:", c);
                         const u = [];
-                        let d = 0,
-                            p = 0;
+                        let p = 0,
+                            d = 0;
                         const m = l.filter((e => e.sheet));
                         m.length !== l.length && console.log("Skipped", l.length - m.length, "style tags without stylesheets (out of", l.length, "total)");
                         for (const t of l) {
                             if (o) break;
                             const s = t.sheet;
-                            if (p++, !s) continue;
+                            if (d++, !s) continue;
                             n?.emit({
-                                percentage: 100 * d / m.length
-                            }), d++, s.disabled = !0, await M();
+                                percentage: 100 * p / m.length
+                            }), p++, s.disabled = !0, await M();
                             const r = await D(e, i, !0);
                             await M(), s.disabled = !1;
                             const a = await oe(t.textContent);
                             u.push({
                                 ...r,
                                 content: t.textContent,
                                 source: null != a ? a.sources[0] : null,
-                                stylesheetIndex: p
+                                stylesheetIndex: d
                             })
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(a), {
                             results: u,
                             reference: c.times,
                             tags: b(),
                             totalTime: Date.now() - r,
@@ -1585,44 +1589,44 @@
                         const o = t.repeats || 3,
                             a = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
                             l = Date.now();
                         e.setupSuite && await e.setupSuite();
                         const c = [...document.querySelectorAll("style")],
                             u = await D(e, 2 * o, !0);
                         console.log("Reference for", e.name, "is:", u);
-                        const d = [],
-                            p = await ae(c, {
+                        const p = [],
+                            d = await ae(c, {
                                 skipPattern: a
                             });
-                        for (let t = 0; t < p.length && !i; t++) {
+                        for (let t = 0; t < d.length && !i; t++) {
                             n?.emit({
-                                percentage: 100 * t / p.length
+                                percentage: 100 * t / d.length
                             });
-                            const s = p[t];
+                            const s = d[t];
                             s.sheet.deleteRule(s.ruleIndex), await M();
                             const i = await D(e, o, !0);
-                            d.push({
+                            p.push({
                                 ...i,
                                 selector: s.selector,
                                 source: s.source,
                                 ruleIndex: s.ruleIndex,
                                 stylesheetIndex: s.stylesheetIndex,
                                 bgMatches: document.querySelectorAll(s.selector).length
                             }), s.sheet.insertRule(s.rule.cssText, s.ruleIndex), await M()
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(r), {
-                            results: d,
+                            results: p,
                             reference: u.times,
                             tags: b(),
                             totalTime: Date.now() - l,
                             type: "time",
                             interrupted: i
                         }
                     },
-                    interpretation: p().createElement(p().Fragment, null, p().createElement("ul", null, p().createElement("li", null, p().createElement("code", null, "bgMatches"), ": how many elements matched the rule at standby (as compared to during scenario execution); mostly useful to find too broad rules, or potentially unused rules with expensive selectors.")), p().createElement("div", null, "Negative ", p().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
+                    interpretation: d().createElement(d().Fragment, null, d().createElement("ul", null, d().createElement("li", null, d().createElement("code", null, "bgMatches"), ": how many elements matched the rule at standby (as compared to during scenario execution); mostly useful to find too broad rules, or potentially unused rules with expensive selectors.")), d().createElement("div", null, "Negative ", d().createElement("code", null, "Δ"), " highlights rules which may be deteriorating performance."))
                 },
                 ge = {
                     id: "style-rule-group",
                     name: "Style Rule Groups",
                     configSchema: ue,
                     run: async (e, t = {}, n, s) => {
                         let i = !1;
@@ -1632,29 +1636,29 @@
                         s?.connect(r);
                         const o = t.repeats || 3,
                             a = t.skipPattern ? new RegExp(t.skipPattern, "g") : void 0,
                             l = t.maxBlocks || 5,
                             c = t.minBlocks || 2,
                             u = Date.now();
                         e.setupSuite && await e.setupSuite();
-                        let d = [...document.querySelectorAll("style")];
-                        const p = await D(e, 2 * o, !0);
-                        console.log("Reference for", e.name, "is:", p);
+                        let p = [...document.querySelectorAll("style")];
+                        const d = await D(e, 2 * o, !0);
+                        console.log("Reference for", e.name, "is:", d);
                         const m = [],
                             h = t.sheetRandomizations || 0;
                         let f = 0;
                         const g = (l - c + 1) * (h + 1);
                         for (let t = 0; t < h + 1 && !i; t++) {
-                            0 !== t && (d = d.map((e => ({
+                            0 !== t && (p = p.map((e => ({
                                 value: e,
                                 sort: Math.random()
                             }))).sort(((e, t) => e.sort - t.sort)).map((({
                                 value: e
                             }) => e)));
-                            const s = await ae(d, {
+                            const s = await ae(p, {
                                 skipPattern: a
                             });
                             console.log(`Collected ${s.length} rules, randomization: ${t}`);
                             for (let r = c; r <= l && !i; r++) {
                                 f += 1, n?.emit({
                                     percentage: 100 * f / g
                                 });
@@ -1681,66 +1685,66 @@
                                     }
                                     await M()
                                 }
                             }
                         }
                         return e.cleanupSuite && await e.cleanupSuite(), s?.disconnect(r), {
                             results: m,
-                            reference: p.times,
+                            reference: d.times,
                             tags: b(),
                             totalTime: Date.now() - u,
                             type: "time",
                             interrupted: i
                         }
                     },
                     render: function(e) {
                         const t = e.outcome.results,
-                            [n, s] = p().useState("block"),
-                            i = p().useRef(null);
-                        null !== i.current && i.current.stateSource === e.outcome || (i.current = new G({
+                            [n, s] = d().useState("block"),
+                            i = d().useRef(null);
+                        null !== i.current && i.current.stateSource === e.outcome || (i.current = new V({
                             measurements: t,
                             reference: e.outcome.reference,
                             stateSource: e.outcome,
                             lowerIsBetter: !1
                         }));
-                        const r = p().useRef(null);
+                        const r = d().useRef(null);
                         if (null === r.current || r.current.stateSource !== e.outcome) {
                             const n = {};
                             for (const e of t)
                                 for (const t of e.rulesInBlock)
                                     if (t.selector in n) n[t.selector].times.push(...e.times);
                                     else {
                                         const s = {
                                             ...t,
                                             times: [...e.times],
                                             errors: e.errors ? [...e.errors] : []
                                         };
                                         delete s.sheet, delete s.rule, n[t.selector] = s
-                                    } r.current = new G({
+                                    } r.current = new V({
                                 measurements: [...Object.values(n)],
                                 reference: e.outcome.reference,
                                 stateSource: e.outcome,
                                 lowerIsBetter: !1
                             })
                         }
-                        return p().createElement(p().Fragment, null, p().createElement("div", {
+                        return d().createElement(d().Fragment, null, d().createElement("div", {
                             onChange: e => {
                                 s(e.target.value)
                             }
-                        }, p().createElement("label", null, p().createElement("input", {
+                        }, d().createElement("label", null, d().createElement("input", {
                             type: "radio",
                             checked: "block" === n,
                             value: "block"
-                        }), "Blocks"), p().createElement("label", null, p().createElement("input", {
+                        }), "Blocks"), d().createElement("label", null, d().createElement("input", {
                             type: "radio",
                             checked: "rule" === n,
                             value: "rule"
-                        }), "Rules")), "block" === n ? p().createElement(K, {
+                        }), "Rules")), "block" === n ? d().createElement(K, {
                             widget: i.current
-                        }) : p().createElement(K, {
+                        }) : d().createElement(K, {
                             widget: r.current
                         }))
                     }
                 },
                 we = new f.Token("@jupyterlab/ui-profiler:plugin");
 
             function ye(e) {
@@ -1814,18 +1818,18 @@
                         mode: g.PageConfig.getOption("mode")
                     }
                 }
             }
             const ke = JSON.parse('{"title":"Scenario Options","type":"object","properties":{}}'),
                 ve = JSON.parse('{"title":"Menu Open Scenario Options","type":"object","properties":{"menu":{"title":"The menu to open","type":"string","default":"file","enum":["file","edit","view","run","kernel","settings","help"]}},"required":["menu"]}'),
                 Se = JSON.parse('{"title":"Tab Scenario Options","type":"object","definitions":{"tab":{"description":"Tab to open","type":"object","properties":{"path":{"title":"Path","description":"Location of file/notebook to open. If empty opens a new launcher.","type":"string"}},"default":{"path":""}}},"properties":{"tabs":{"title":"List of tabs to use in scenario","description":"Series of two or more tabs","type":"array","items":{"$ref":"#/definitions/tab"},"default":[{"path":""},{"path":""}]}},"required":["tabs"]}'),
-                Ee = JSON.parse('{"title":"Completer Scenario Options","type":"object","properties":{"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"File Editor"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"setup":{"title":"Editor setup for completion","description":"How should the editor be populated?","default":{"tokenCount":1000,"tokenSize":50},"anyOf":[{"type":"object","title":"Auto-generate tokens to complete","properties":{"tokenCount":{"title":"Token count","description":"The number of completion items to generate","type":"number","minimum":1,"default":1000},"tokenSize":{"title":"Token size","description":"The number characters in each token","type":"number","minimum":1,"default":50}},"required":["tokenCount","tokenSize"]},{"type":"object","title":"I will provide a custom text","properties":{"setupText":{"title":"Trigger code","description":"Text to enter into the editor. Last line should include a partial token on which the completion will be riggered.","type":"string","default":"np."},"setupCell":{"title":"Code to run (notebook only)","description":"Code to run prior to invoking completer, e.g. `import numpy as np`. Only has an effect in notebook.","type":"string","default":"import numpy as np"}},"required":["setupText","triggerCell"]}]}},"required":["editor","setup"],"additionalProperties":false}'),
-                xe = JSON.parse('{"title":"Debugger Scenario Options","type":"object","properties":{"codeCells":{"title":"Code to execute","description":"Python code cells to execute one-by-one to populate the debugger namespace, e.g. `from numpy import *`","type":"array","items":{"type":"string"},"default":["[globals().__setitem__(f\'x{i}\', \'y\') for i in range(1000)];","z = 1"]},"expectedNumberOfVariables":{"title":"Expected number of variables","description":"The scenario waits until debugger panel is populated with at least as many variables as specified. For accurate timings should have as many members as there are code cells.","type":"array","items":{"type":"integer","min":0},"default":[1000,1001]}},"required":["codeCells","expectedNumberOfVariables"],"additionalProperties":false}'),
+                Ee = JSON.parse('{"title":"Completer Scenario Options","type":"object","properties":{"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"File Editor"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"setup":{"title":"Editor setup for completion","description":"How should the editor be populated?","default":{"tokenCount":1000,"tokenSize":50},"anyOf":[{"type":"object","title":"Auto-generate tokens to complete","properties":{"tokenCount":{"title":"Token count","description":"The number of completion items to generate","type":"number","minimum":1,"default":1000},"tokenSize":{"title":"Token size","description":"The number characters in each token","type":"number","minimum":1,"default":50}},"required":["tokenCount","tokenSize"]},{"type":"object","title":"I will provide a custom text","properties":{"setupText":{"title":"Trigger code","description":"Text to enter into the editor. Last line should include a partial token on which the completion will be riggered.","type":"string","default":"np."},"setupCell":{"title":"Code to run (notebook only)","description":"Code to run prior to invoking completer, e.g. `import numpy as np`. Only has an effect in notebook.","type":"string","default":"import numpy as np"}},"required":["setupText","triggerCell"]}]},"widgetPosition":{"title":"Widget position in the layout","description":"Where to attach the editor widget in the layout","type":"string","enum":["split-top","split-left","split-right","split-bottom","tab-before","tab-after"],"default":"split-right"}},"required":["editor","setup"],"additionalProperties":false}'),
+                xe = JSON.parse('{"title":"Debugger Scenario Options","type":"object","properties":{"codeCells":{"title":"Code to execute","description":"Python code cells to execute one-by-one to populate the debugger namespace, e.g. `from numpy import *`","type":"array","items":{"type":"string"},"default":["[globals().__setitem__(f\'x{i}\', \'y\') for i in range(1000)];","z = 1"]},"expectedNumberOfVariables":{"title":"Expected number of variables","description":"The scenario waits until debugger panel is populated with at least as many variables as specified. For accurate timings should have as many members as there are code cells.","type":"array","items":{"type":"integer","min":0},"default":[1000,1001]},"widgetPosition":{"title":"Widget position in the layout","description":"Where to attach the editor widget in the layout","type":"string","enum":["split-top","split-left","split-right","split-bottom","tab-before","tab-after"],"default":"split-right"}},"required":["codeCells","expectedNumberOfVariables"],"additionalProperties":false}'),
                 je = JSON.parse('{"title":"Sidebars Scenario Options","type":"object","properties":{"sidebars":{"title":"The sidebars to open","type":"array","default":["table-of-contents","jp-debugger-sidebar","jp-property-inspector","filebrowser","extensionmanager.main-view","jp-running-sessions"],"items":{"type":"string"}}},"required":["sidebars"]}'),
-                Ne = JSON.parse('{"title":"Scroll Scenario Options","type":"object","properties":{"scrollTop":{"title":"Scroll from top","description":"Number of pixes to scroll by","type":"number","minimum":0,"default":10000},"scrollBehavior":{"title":"Scroll behaviour","description":"Behavior of scroll, either \'smooth\' for smooth scrolling, or \'auto\' for instant scrolling.","type":"string","enum":["smooth","auto"],"default":"smooth"},"cellByCell":{"title":"Traverse cell-by-cell","description":"Instead of scrolling, traverse notebook cell-by-cell (which also combines stepwise scrolling and cell activation/deactivation). Small number of cells (50-100) is recommended for benchmarking such scenario. \'scrollTop\' and \'scrollBehavior\' have no effect if this variant is enabled. Has no effect in file editor.","type":"boolean","default":false},"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"Notebook"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"cells":{"title":"Number of cells/blocks to append","description":"If using a notebook, how many cell should be created? For file editor, how many lines?","type":"number","minimum":0,"default":1000},"editorContent":{"title":"Editor/cell content","description":"Text to populate editors/cells with.","type":"string","default":"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."}},"required":["editor","cells","scrollTop","scrollBehavior"],"additionalProperties":false}');
+                Ne = JSON.parse('{"title":"Scroll Scenario Options","type":"object","properties":{"scrollTop":{"title":"Scroll from top","description":"Number of pixes to scroll by","type":"number","minimum":0,"default":10000},"scrollBehavior":{"title":"Scroll behaviour","description":"Behavior of scroll, either \'smooth\' for smooth scrolling, or \'auto\' for instant scrolling.","type":"string","enum":["smooth","auto"],"default":"smooth"},"cellByCell":{"title":"Traverse cell-by-cell","description":"Instead of scrolling, traverse notebook cell-by-cell (which also combines stepwise scrolling and cell activation/deactivation). Small number of cells (50-100) is recommended for benchmarking such scenario. \'scrollTop\' and \'scrollBehavior\' have no effect if this variant is enabled. Has no effect in file editor.","type":"boolean","default":false},"editor":{"title":"Editor type","description":"Editor widget to test completion in","type":"string","enum":["Notebook","File Editor"],"default":"Notebook"},"path":{"title":"Path to document","description":"Optional path to an existing document of specified editor type. When empty (default) a new temporary file will be created.","type":"string","default":""},"cells":{"title":"Number of cells/blocks to append","description":"If using a notebook, how many cell should be created? For file editor, how many lines?","type":"number","minimum":0,"default":1000},"editorContent":{"title":"Editor/cell content","description":"Text to populate editors/cells with.","type":"string","default":"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."},"widgetPosition":{"title":"Widget position in the layout","description":"Where to attach the editor widget in the layout","type":"string","enum":["split-top","split-left","split-right","split-bottom","tab-before","tab-after"],"default":"split-right"}},"required":["editor","cells","scrollTop","scrollBehavior"],"additionalProperties":false}');
             async function Me(e, t = "file") {
                 await e.commands.execute(`${t}menu:open`), await P.waitForSelector(`#jp-mainmenu-${t}`, {
                     state: "attached"
                 }), await M()
             }
             async function Ce() {
                 await P.waitForSelector(".lm-Menu", {
@@ -1912,16 +1916,16 @@
                         this.path = e.path
                     }
                     const e = await this.jupyterApp.commands.execute("docmanager:open", {
                         path: this.path,
                         factory: this.useNotebook ? "Notebook" : "Editor"
                     });
                     this.widget = e, this.jupyterApp.shell.add(this.widget, "main", {
-                        mode: "split-right"
-                    }), await De(this.jupyterApp, e), await M(), this.useNotebook && await P.click(".jp-Dialog-button.jp-mod-accept");
+                        mode: this.options?.widgetPosition || "split-right"
+                    }), await Fe(this.jupyterApp, e), await M(), this.useNotebook && await P.click(".jp-Dialog-button.jp-mod-accept");
                     const t = new C(this.widget.node);
                     await t.waitForSelector(".jp-Editor", {
                         state: "attached"
                     }), await M(), await t.waitForSelector(".jp-Editor", {
                         state: "visible"
                     }), await M(), this.editor = this.useNotebook ? this.widget.node.querySelector(".jp-Notebook") : this.widget.node.querySelector(".jp-FileEditorCodeWrapper")
                 }
@@ -1938,15 +1942,15 @@
                     let e;
                     if (void 0 !== this.options.setup?.setupText) e = this.options.setup.setupText;
                     else {
                         const t = [];
                         for (let e = 0; e < this.options.setup.tokenCount; e++) t.push(("t" + e).padEnd(this.options.setup.tokenSize, "x") + " = " + e);
                         t.push("t"), e = t.join("\n")
                     }
-                    this.useNotebook && this.options.setup.setupCell ? (await Te(this.jupyterApp, this.options.setup.setupCell), await Pe(this.widget.node, "idle"), await this.jupyterApp.commands.execute("notebook:run-cell-and-insert-below"), await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:enter-edit-mode")) : await Te(this.jupyterApp, e), this.useNotebook || (this.editor.querySelector(".CodeMirror-scroll") || this.editor.querySelector(".cm-scroller")).scrollBy({
+                    this.useNotebook && this.options.setup.setupCell ? (await Te(this.jupyterApp, this.options.setup.setupCell), await De(this.widget.node, "idle"), await this.jupyterApp.commands.execute("notebook:run-cell-and-insert-below"), await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:enter-edit-mode")) : await Te(this.jupyterApp, e), this.useNotebook || (this.editor.querySelector(".CodeMirror-scroll") || this.editor.querySelector(".cm-scroller")).scrollBy({
                         top: 20 * this.options.setup.tokenCount,
                         left: 0,
                         behavior: "smooth"
                     });
                     try {
                         await this.run()
                     } catch (e) {}
@@ -1968,15 +1972,26 @@
                 }
                 async cleanup() {
                     await P.press("Escape"), await M(), await P.waitForSelector(".jp-Completer[style]", {
                         state: "hidden"
                     }), await M()
                 }
             }
-            class Ae extends Be {
+            async function Ae() {
+                const e = ".jp-Toolbar-responsive-popup",
+                    t = await P.$('.jp-Toolbar-responsive-opener > button[title="More commands"]');
+                if (t && await t.isVisible()) {
+                    const n = await P.$(e);
+                    if (n && await n.isVisible()) return;
+                    await t.click(), await P.waitForSelector(e, {
+                        state: "visible"
+                    })
+                }
+            }
+            class Pe extends Be {
                 constructor() {
                     super(...arguments), this.id = "debugger", this.name = "Debugger", this.configSchema = xe
                 }
                 setOptions(e) {
                     super.setOptions({
                         ...e,
                         editor: "Notebook",
@@ -1986,64 +2001,65 @@
                 async _goToTop() {
                     if (!this.options) throw new Error("Setup failure");
                     for (let e = 0; e < this.options.codeCells.length + 1; e++) await this.jupyterApp.commands.execute("notebook:move-cursor-up")
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     for (const e of this.options.codeCells) await Te(this.jupyterApp, e), await this.jupyterApp.commands.execute("notebook:insert-cell-below"), await M(), await M(), await this.jupyterApp.commands.execute("notebook:enter-edit-mode"), await M(), await M();
-                    await Te(this.jupyterApp, "%reset -f"), await this._goToTop(), await Pe(this.widget.node, "idle");
-                    const e = new C(this.widget.node),
-                        t = await e.waitForSelector('button[aria-disabled="false"][title="Enable Debugger"]', {
-                            state: "attached"
-                        });
+                    await Te(this.jupyterApp, "%reset -f"), await this._goToTop(), await De(this.widget.node, "idle");
+                    const e = new C(this.widget.node);
+                    await Ae();
+                    const t = await e.waitForSelector('button[aria-disabled="false"][title="Enable Debugger"]', {
+                        state: "attached"
+                    });
                     await t.click(), await P.waitForSelector(`#${CSS.escape("jp-debugger-sidebar")}`, {
                         state: "visible"
-                    }), await e.waitForSelector('button[aria-disabled="false"][title="Disable Debugger"]', {
+                    }), await Ae(), await e.waitForSelector('button[aria-disabled="false"][title="Disable Debugger"]', {
                         state: "attached"
                     }), await M(), await P.waitForSelector(".jp-DebuggerVariables-body", {
                         state: "attached"
                     }), await P.waitForSelector(".jp-DebuggerVariables-body", {
                         state: "visible"
                     })
                 }
                 async run() {
                     if (!this.widget || !this.options) throw new Error("Setup failure");
                     for (let e = 0; e < this.options.codeCells.length; e++) {
-                        await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await Pe(this.widget.node, "idle");
+                        await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await De(this.widget.node, "idle");
                         const t = this.options.expectedNumberOfVariables[e];
                         void 0 !== t && await P.waitForSelector(`.jp-DebuggerVariables-body li:nth-child(${t+2})`, {
                             state: "attached"
                         }), await M()
                     }
                 }
                 async cleanup() {
                     if (!this.widget || !this.options) throw new Error("Setup failure");
                     await M();
                     const e = Math.min(...this.options.expectedNumberOfVariables);
-                    await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await Pe(this.widget.node, "idle"), await async function(e) {
+                    await this.jupyterApp.commands.execute("notebook:run-cell-and-select-next"), await De(this.widget.node, "idle"), await async function(e) {
                         return new Promise(((t, n) => {
                             let s = 0;
                             const i = setInterval((() => document.querySelector(e) ? s > 5e3 ? (clearInterval(i), n(`${e} did not disappear in 5000ms`)) : void(s += 50) : (clearInterval(i), t())), 50)
                         }))
                     }(`.jp-DebuggerVariables-body li:nth-child(${e})`), await this._goToTop(), await M()
                 }
             }
-            async function Pe(e, t) {
+            async function De(e, t) {
                 await new C(e).waitForSelector(`.jp-Notebook-ExecutionIndicator[data-status="${t}"]`, {
                     state: "attached"
                 })
             }
-            async function De(e, t) {
+            async function Fe(e, t) {
                 await e.commands.execute("tabsmenu:activate-by-id", {
                     id: t.id
                 }), await M(), await P.waitForSelector(`li.lm-mod-current[data-id="${t.id}"]`, {
                     state: "attached"
                 }), await M()
             }
-            class Fe extends Be {
+            class qe extends Be {
                 constructor() {
                     super(...arguments), this.id = "scroll", this.name = "Scroll", this.configSchema = Ne
                 }
                 async setupSuite() {
                     if (await super.setupSuite(), !this.widget || !this.options) throw new Error("Parent setup failure");
                     const e = this.options.cells < 100 ? 20 : 50;
                     for (let t = 0; t < this.options.cells; t++) this.useNotebook && await this.jupyterApp.commands.execute("notebook:insert-cell-below"), this.options.editorContent && await Te(this.jupyterApp, this.useNotebook ? this.options.editorContent : this.options.editorContent + "\n"), (t < 5 || t % e == 0) && await M();
@@ -2073,15 +2089,15 @@
                     if (!this.widget || !this.options) throw new Error("Scrol scenario setup failure");
                     if (this.options.cellByCell && this.useNotebook) {
                         for (let e = 0; e < this.options.cells; e++) await this.jupyterApp.commands.execute("notebook:move-cursor-up");
                         await M()
                     } else this.editor.scrollTop = 0, await M()
                 }
             }
-            class qe {
+            class Le {
                 constructor(e) {
                     this.jupyterApp = e, this.id = "tabSwitch", this.name = "Switch Tabs", this.split = "first", this.configSchema = Se, this._tabs = [], this._widgets = []
                 }
                 setOptions(e) {
                     const {
                         tabs: t
                     } = e;
@@ -2094,51 +2110,51 @@
                         let t;
                         t = e.path ? await this.jupyterApp.commands.execute("docmanager:open", {
                             path: e.path
                         }) : await this.jupyterApp.commands.execute("launcher:create"), await P.waitForSelector("#" + t.id, {
                             state: "attached"
                         }), ("first" === this.split && 0 === this._widgets.length || "all" === this.split) && this.jupyterApp.shell.add(t, "main", {
                             mode: "split-right"
-                        }), await De(this.jupyterApp, t), this._widgets.push(t)
+                        }), await Fe(this.jupyterApp, t), this._widgets.push(t)
                     }
                 }
                 async cleanupSuite() {
                     for (const e of this._widgets) e.close(), await P.waitForSelector(`.lm-Widget[data-id="${e.id}"]`, {
                         state: "detached"
                     })
                 }
                 async run() {
                     if (!this._widgets.length) throw new Error("Suite not set up");
-                    for (const e of this._widgets) await De(this.jupyterApp, e)
+                    for (const e of this._widgets) await Fe(this.jupyterApp, e)
                 }
             }
-            class Le extends qe {
+            class We extends Le {
                 constructor() {
                     super(...arguments), this.id = "tabSwitchFocus", this.name = "Switch Tab Focus", this.split = "all"
                 }
             }
             const $e = {
                 id: "@jupyterlab/ui-profiler:default-scenarios",
                 autoStart: !0,
                 requires: [we],
                 activate: (e, t) => {
-                    [new Ie(e), new Oe(e), new qe(e), new Le(e), new _e(e), new Re(e), new Fe(e), new Ae(e)].map((e => t.addScenario(e)))
+                    [new Ie(e), new Oe(e), new Le(e), new We(e), new _e(e), new Re(e), new qe(e), new Pe(e)].map((e => t.addScenario(e)))
                 }
             };
-            var We;
+            var ze;
             ! function(e) {
                 e.openProfiler = "ui-profiler:open"
-            }(We || (We = {}));
-            const ze = [{
+            }(ze || (ze = {}));
+            const He = [{
                 id: "@jupyterlab/ui-profiler:plugin",
                 autoStart: !0,
                 provides: we,
                 activate: e => new be({
                     app: e,
-                    benchmarks: [F, he, fe, ge, me, $]
+                    benchmarks: [F, he, fe, ge, me, W]
                 })
             }, $e, {
                 id: "@jupyterlab/ui-profiler:user-interface",
                 autoStart: !0,
                 requires: [we, r.IDocumentManager],
                 optional: [a.ILauncher, s.ILayoutRestorer],
                 activate: (e, t, n, s, r) => {
@@ -2147,37 +2163,37 @@
                         }),
                         u = {
                             translator: l.nullTranslator,
                             profiler: t,
                             upload: e => a.upload(e),
                             resultLocation: "/ui-profiler-results/"
                         };
-                    let d = null;
-                    const p = new i.WidgetTracker({
+                    let p = null;
+                    const d = new i.WidgetTracker({
                         namespace: "ui-profiler"
                     });
-                    e.commands.addCommand(We.openProfiler, {
+                    e.commands.addCommand(ze.openProfiler, {
                         execute: async () => {
                             let t;
-                            t = !d || d.isDisposed ? (() => {
+                            t = !p || p.isDisposed ? (() => {
                                 const e = new Z(u),
                                     t = new i.MainAreaWidget({
                                         content: e
                                     });
                                 return t.id = "ui-profiler-centre", t.title.label = "UI Profiler", t.title.closable = !0, t.title.icon = c.offlineBoltIcon, t
-                            })() : d, d = t, t.isAttached || e.shell.add(t, "main"), e.shell.activateById(t.id), p.add(t)
+                            })() : p, p = t, t.isAttached || e.shell.add(t, "main"), e.shell.activateById(t.id), d.add(t)
                         },
                         label: "UI Profiler",
                         icon: c.offlineBoltIcon,
                         caption: "Open JupyterLab UI Profiler"
-                    }), r && r.restore(p, {
-                        command: We.openProfiler,
+                    }), r && r.restore(d, {
+                        command: ze.openProfiler,
                         name: e => e.title.label
                     }), s && s.add({
-                        command: We.openProfiler,
+                        command: ze.openProfiler,
                         category: "Other",
                         rank: 1
                     })
                 }
             }]
         }
     }
```

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/511.91d18779f0d0a64a6570.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/747.cddb110f7b8c43b31d07.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/remoteEntry.2c015c9bba0ac87e826d.js` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/remoteEntry.b7edad4eeff456a5f798.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, f, s, d, p, c, h, v = {
+    var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, v = {
             4299: (e, r, t) => {
-                var n = {
+                var a = {
                         "./index": () => Promise.all([t.e(511), t.e(148)]).then((() => () => t(8148))),
                         "./extension": () => Promise.all([t.e(511), t.e(148)]).then((() => () => t(8148))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var a = "default",
+                                n = t.S[a];
+                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
+                    get: () => n,
                     init: () => o
                 })
             }
         },
         b = {};
 
     function m(e) {
@@ -44,80 +44,80 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        148: "d0923e85cee15af0e9d9",
+        148: "386a0716eefd6e346348",
         511: "91d18779f0d0a64a6570",
         747: "cddb110f7b8c43b31d07"
     } [e] + ".js?v=" + {
-        148: "d0923e85cee15af0e9d9",
+        148: "386a0716eefd6e346348",
         511: "91d18779f0d0a64a6570",
         747: "cddb110f7b8c43b31d07"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/ui-profiler:", m.l = (t, n, a, o) => {
-        if (e[t]) e[t].push(n);
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/ui-profiler:", m.l = (t, a, n, o) => {
+        if (e[t]) e[t].push(a);
         else {
             var i, l;
-            if (void 0 !== a)
+            if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+                    var d = u[f];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
+            var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var n = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, m.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         m.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
-            n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+        m.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
                 m.o(m.S, t) || (m.S[t] = {});
                 var o = m.S[t],
                     i = "@jupyterlab/ui-profiler",
                     l = [];
-                return "default" === t && ((e, r, t, n) => {
-                    var a = o[e] = o[e] || {},
-                        l = a[r];
-                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (a[r] = {
+                return "default" === t && ((e, r, t, a) => {
+                    var n = o[e] = o[e] || {},
+                        l = n[r];
+                    (!l || !l.loaded && (1 != !l.eager ? a : i > l.from)) && (n[r] = {
                         get: () => Promise.all([m.e(511), m.e(148)]).then((() => () => m(8148))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab/ui-profiler", "0.2.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@jupyterlab/ui-profiler", "0.2.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -125,74 +125,74 @@
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
-            var i = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                o = (typeof n)[0];
+            if (a >= r.length) return "u" == o;
+            var i = r[a],
                 l = (typeof i)[0];
             if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
-            n++
+            if ("o" != o && "u" != o && n != i) return n < i;
+            a++
         }
-    }, a = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
-                if ("u" == s) {
-                    if (!u || "u" != d) return !1
+                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
+                if ("u" == d) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (d == s)
-                        if (l <= n) {
+                    if (s == d)
+                        if (l <= a) {
                             if (f != e[l]) return !1
                         } else {
-                            if (a ? f > e[l] : f < e[l]) return !1;
+                            if (n ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (a || l <= n) return !1;
+                else if ("s" != s && "n" != s) {
+                    if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < d != a) return !1;
+                    if (l <= a || d < s != n) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -200,89 +200,89 @@
         return !!c()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
-        var a = l(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), s(e[t][a])
-    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, a) {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
+        var n = l(e, t);
+        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(e, t, n, a)), d(e[t][n])
+    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, a, n) {
         var o = m.I(r);
-        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, a)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
-        1467: () => d("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
-        1526: () => d("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        1840: () => d("default", "@lumino/signaling", [1, 1, 10, 0]),
-        2502: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        2583: () => d("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
-        3033: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        3169: () => d("default", "@jupyterlab/translation", [1, 3, 6, 3]),
-        5414: () => d("default", "@lumino/datagrid", [2, 0, 36, 4]),
-        5687: () => d("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        6271: () => d("default", "react", [1, 17, 0, 1]),
-        7280: () => d("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
-        7986: () => d("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
-        8142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        8820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        8832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
+        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, a, n)) : e(r, m.S[r], t, a)
+    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), p = {}, c = {
+        1467: () => s("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
+        1526: () => s("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        1840: () => s("default", "@lumino/signaling", [1, 1, 10, 0]),
+        2502: () => s("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        2583: () => s("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
+        3033: () => s("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        3169: () => s("default", "@jupyterlab/translation", [1, 3, 6, 3]),
+        5414: () => s("default", "@lumino/datagrid", [2, 0, 36, 4]),
+        5687: () => s("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        6271: () => s("default", "react", [1, 17, 0, 1]),
+        7280: () => s("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        7986: () => s("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
+        8142: () => s("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        8820: () => s("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        8832: () => s("default", "@lumino/widgets", [1, 1, 37, 2])
     }, h = {
         148: [1467, 1526, 1840, 2502, 2583, 3033, 3169, 5414, 5687, 6271, 7280, 7986, 8142, 8820, 8832]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
             if (m.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
-                n = r => {
+                a = r => {
                     delete p[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
-                var a = c[e]();
-                a.then ? r.push(p[e] = a.then(t).catch(n)) : t(a)
+                var n = c[e]();
+                n.then ? r.push(p[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
         var e = {
             770: 0
         };
         m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
+            var a = m.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
+                    var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                    t.push(a[2] = n);
                     var o = m.p + m.u(r),
                         i = new Error;
                     m.l(o, (t => {
-                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
+                        if (m.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                            var n = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                            i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, l] = t,
+                var a, n, [o, i, l] = t,
                     u = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                    for (a in i) m.o(i, a) && (m.m[a] = i[a]);
                     l && l(m)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], m.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < o.length; u++) n = o[u], m.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_jupyterlab_ui_profiler = self.webpackChunk_jupyterlab_ui_profiler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), m.nc = void 0;
     var g = m(4299);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/ui-profiler"] = g
 })();
```

### Comparing `jupyterlab_ui_profiler-0.2.0/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json` & `jupyterlab_ui_profiler-0.2.1/jupyterlab_ui_profiler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/benchmark.ts` & `jupyterlab_ui_profiler-0.2.1/src/benchmark.ts`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import { JSONSchema7 } from 'json-schema';
 import { Statistic } from './statistics';
 import { reportTagCounts } from './utils';
 import { layoutReady } from './dramaturg';
 import benchmarkExecutionOptionsSchema from './schema/benchmark-execution.json';
-import type { ExecutionTimeBenchmarkOptions } from './types/_benchmark-execution';
+import type { ExecutionTimeBenchmarkOptions } from './types';
 import { renderTimings } from './ui';
 import {
   IBenchmark,
   IScenario,
   IProfileMeasurement,
   ITimingOutcome,
   ITimeMeasurement
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/browserProfiler.d.ts` & `jupyterlab_ui_profiler-0.2.1/src/browserProfiler.d.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/css.ts` & `jupyterlab_ui_profiler-0.2.1/src/css.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/dramaturg.ts` & `jupyterlab_ui_profiler-0.2.1/src/dramaturg.ts`

 * *Files 5% similar despite different names*

```diff
@@ -184,14 +184,19 @@
   }
   press(key: string, options = { delay: 0 }): Promise<void> {
     return press(key, options, this.element);
   }
   type(text: string, options = { delay: 0 }): Promise<void> {
     return type(text, options, this.element);
   }
+  async isVisible(): Promise<boolean> {
+    const size = this.element.getBoundingClientRect();
+    const notVisible = size.width === 0 || size.height === 0;
+    return !notVisible;
+  }
   waitForSelector(
     selector: string,
     options: IWaitForSelectorOptions
   ): Promise<ElementHandle> {
     return waitForSelector(selector, {
       ...options,
       within: this.element
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/index.ts` & `jupyterlab_ui_profiler-0.2.1/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -134,9 +134,10 @@
         rank: 1
       });
     }
   }
 };
 
 export * from './tokens';
+export * from './types';
 
 export default [plugin, scenariosPlugin, interfacePlugin];
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/jsBenchmarks.ts` & `jupyterlab_ui_profiler-0.2.1/src/jsBenchmarks.ts`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import { IProfilingOutcome, IProfileMeasurement } from './tokens';
 import { reportTagCounts } from './utils';
 import { layoutReady } from './dramaturg';
 import { renderProfile } from './ui';
 import { IBenchmark, IScenario } from './tokens';
 
 import benchmarkProfileOptionsSchema from './schema/benchmark-profile.json';
-import type { ProfileBenchmarkOptions } from './types/_benchmark-profile';
+import type { ProfileBenchmarkOptions } from './types';
 
 interface IFunctionTiming {
   time: number;
   readonly name: string;
   readonly line?: number;
   readonly column?: number;
   readonly resource?: string;
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/lumino.tsx` & `jupyterlab_ui_profiler-0.2.1/src/lumino.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/profiler.ts` & `jupyterlab_ui_profiler-0.2.1/src/profiler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/scenarios.ts` & `jupyterlab_ui_profiler-0.2.1/src/scenarios.ts`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,23 @@
   layoutReady,
   ElementHandle,
   waitForScrollEnd,
   waitUntilDisappears
 } from './dramaturg';
 import { IScenario, IUIProfiler } from './tokens';
 
-import type { TabScenarioOptions, Tab } from './types/_scenario-tabs';
-import type { MenuOpenScenarioOptions } from './types/_scenario-menu-open';
-import type { CompleterScenarioOptions } from './types/_scenario-completer';
-import type { SidebarsScenarioOptions } from './types/_scenario-sidebars';
-import type { ScrollScenarioOptions } from './types/_scenario-scroll';
-import type { DebuggerScenarioOptions } from './types/_scenario-debugger';
+import type { Tab } from './types/_scenario-tabs';
+import type {
+  MenuOpenScenarioOptions,
+  CompleterScenarioOptions,
+  SidebarsScenarioOptions,
+  TabScenarioOptions,
+  ScrollScenarioOptions,
+  DebuggerScenarioOptions
+} from './types';
 
 import scenarioOptionsSchema from './schema/scenario-base.json';
 import scenarioMenuOpenOptionsSchema from './schema/scenario-menu-open.json';
 import scenarioTabOptionsSchema from './schema/scenario-tabs.json';
 import scenarioCompleterOptionsSchema from './schema/scenario-completer.json';
 import scenarioDebuggerOptionsSchema from './schema/scenario-debugger.json';
 import scenarioSidebarsSchema from './schema/scenario-sidebars.json';
@@ -185,15 +188,17 @@
       'docmanager:open',
       {
         path: this.path,
         factory: this.useNotebook ? 'Notebook' : 'Editor'
       }
     );
     this.widget = widget;
-    this.jupyterApp.shell.add(this.widget, 'main', { mode: 'split-right' });
+    this.jupyterApp.shell.add(this.widget, 'main', {
+      mode: this.options?.widgetPosition || 'split-right'
+    });
     await activateTabWidget(this.jupyterApp, widget);
     await layoutReady();
     if (this.useNotebook) {
       // Accept default kernel in kernel selection dialog
       await page.click('.jp-Dialog-button.jp-mod-accept');
     }
     const handle = new ElementHandle(this.widget.node);
@@ -319,14 +324,33 @@
     await page.press('Escape');
     await layoutReady();
     await page.waitForSelector('.jp-Completer[style]', { state: 'hidden' });
     await layoutReady();
   }
 }
 
+async function ensureToolbarButtonsVisible() {
+  const secondToolbarSelector = '.jp-Toolbar-responsive-popup';
+  const moreCommandsButton = await page.$(
+    '.jp-Toolbar-responsive-opener > button[title="More commands"]'
+  );
+  if (moreCommandsButton && (await moreCommandsButton.isVisible())) {
+    const secondToolbar = await page.$(secondToolbarSelector);
+    if (secondToolbar && (await secondToolbar.isVisible())) {
+      // already visible
+      return;
+    }
+    // make sure second toolbar is visible
+    await moreCommandsButton.click();
+    await page.waitForSelector(secondToolbarSelector, {
+      state: 'visible'
+    });
+  }
+}
+
 export class DebuggerScenario
   extends SingleEditorScenario<IExtendedDebuggerScenarioOptions>
   implements IScenario
 {
   id = 'debugger';
   name = 'Debugger';
   configSchema = scenarioDebuggerOptionsSchema as any as JSONSchema7;
@@ -364,24 +388,26 @@
       await layoutReady();
     }
     await insertText(this.jupyterApp, '%reset -f');
     await this._goToTop();
 
     await waitForKernelStatus(this.widget.node, 'idle');
     const handle = new ElementHandle(this.widget.node);
+    await ensureToolbarButtonsVisible();
     const bugIcon = await handle.waitForSelector(
       'button[aria-disabled="false"][title="Enable Debugger"]',
       {
         state: 'attached'
       }
     );
     await bugIcon.click();
     await page.waitForSelector(`#${CSS.escape('jp-debugger-sidebar')}`, {
       state: 'visible'
     });
+    await ensureToolbarButtonsVisible();
     await handle.waitForSelector(
       'button[aria-disabled="false"][title="Disable Debugger"]',
       {
         state: 'attached'
       }
     );
     await layoutReady();
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/statistics.ts` & `jupyterlab_ui_profiler-0.2.1/src/statistics.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/styleBenchmarks.tsx` & `jupyterlab_ui_profiler-0.2.1/src/styleBenchmarks.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 import { IBenchmark, IScenario } from './tokens';
 
 import benchmarkOptionsSchema from './schema/benchmark-base.json';
 import benchmarkRuleOptionsSchema from './schema/benchmark-rule.json';
 import benchmarkRuleGroupOptionsSchema from './schema/benchmark-rule-group.json';
 import benchmarkRuleUsageOptionsSchema from './schema/benchmark-rule-usage.json';
 
-import type { BenchmarkOptions } from './types/_benchmark-base';
-import type { StyleRuleBenchmarkOptions } from './types/_benchmark-rule';
-import type { StyleRuleGroupBenchmarkOptions } from './types/_benchmark-rule-group';
-import type { StyleRuleUsageOptions } from './types/_benchmark-rule-usage';
+import type { BenchmarkOptions } from './types';
+import type { StyleRuleBenchmarkOptions } from './types';
+import type { StyleRuleGroupBenchmarkOptions } from './types';
+import type { StyleRuleUsageOptions } from './types';
 
 interface IStylesheetResult extends ITimeMeasurement {
   content: string | null;
   source: string | null;
   stylesheetIndex: number;
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/table.ts` & `jupyterlab_ui_profiler-0.2.1/src/table.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/templates.tsx` & `jupyterlab_ui_profiler-0.2.1/src/templates.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/tokens.ts` & `jupyterlab_ui_profiler-0.2.1/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/ui.tsx` & `jupyterlab_ui_profiler-0.2.1/src/ui.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/utils.ts` & `jupyterlab_ui_profiler-0.2.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/__tests__/statistics.spec.ts` & `jupyterlab_ui_profiler-0.2.1/src/__tests__/statistics.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-profile.json` & `jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-profile.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-group.json` & `jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-group.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/schema/benchmark-rule-usage.json` & `jupyterlab_ui_profiler-0.2.1/src/schema/benchmark-rule-usage.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-completer.json` & `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-completer.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'properties'": "{'widgetPosition': OrderedDict([('title', 'Widget position in the layout'), "*

 * *                 "('description', 'Where to attach the editor widget in the layout'), ('type', "*

 * *                 "'string'), ('enum', ['split-top', 'split-left', 'split-right', 'split-bottom', "*

 * *                 "'tab-before', 'tab-after']), ('default', 'split-right')])}"}*

```diff
@@ -68,14 +68,28 @@
             ],
             "default": {
                 "tokenCount": 1000,
                 "tokenSize": 50
             },
             "description": "How should the editor be populated?",
             "title": "Editor setup for completion"
+        },
+        "widgetPosition": {
+            "default": "split-right",
+            "description": "Where to attach the editor widget in the layout",
+            "enum": [
+                "split-top",
+                "split-left",
+                "split-right",
+                "split-bottom",
+                "tab-before",
+                "tab-after"
+            ],
+            "title": "Widget position in the layout",
+            "type": "string"
         }
     },
     "required": [
         "editor",
         "setup"
     ],
     "title": "Completer Scenario Options",
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-scroll.json` & `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-scroll.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'properties'": "{'widgetPosition': OrderedDict([('title', 'Widget position in the layout'), "*

 * *                 "('description', 'Where to attach the editor widget in the layout'), ('type', "*

 * *                 "'string'), ('enum', ['split-top', 'split-left', 'split-right', 'split-bottom', "*

 * *                 "'tab-before', 'tab-after']), ('default', 'split-right')])}"}*

```diff
@@ -48,14 +48,28 @@
         },
         "scrollTop": {
             "default": 10000,
             "description": "Number of pixes to scroll by",
             "minimum": 0,
             "title": "Scroll from top",
             "type": "number"
+        },
+        "widgetPosition": {
+            "default": "split-right",
+            "description": "Where to attach the editor widget in the layout",
+            "enum": [
+                "split-top",
+                "split-left",
+                "split-right",
+                "split-bottom",
+                "tab-before",
+                "tab-after"
+            ],
+            "title": "Widget position in the layout",
+            "type": "string"
         }
     },
     "required": [
         "editor",
         "cells",
         "scrollTop",
         "scrollBehavior"
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/schema/scenario-tabs.json` & `jupyterlab_ui_profiler-0.2.1/src/schema/scenario-tabs.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-profile.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-profile.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-group.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-group.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_benchmark-rule-usage.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_benchmark-rule-usage.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-completer.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-completer.ts`

 * *Files 21% similar despite different names*

```diff
@@ -31,19 +31,30 @@
  * Text to enter into the editor. Last line should include a partial token on which the completion will be riggered.
  */
 export type TriggerCode = string;
 /**
  * Code to run prior to invoking completer, e.g. `import numpy as np`. Only has an effect in notebook.
  */
 export type CodeToRunNotebookOnly = string;
+/**
+ * Where to attach the editor widget in the layout
+ */
+export type WidgetPositionInTheLayout =
+  | 'split-top'
+  | 'split-left'
+  | 'split-right'
+  | 'split-bottom'
+  | 'tab-before'
+  | 'tab-after';
 
 export interface CompleterScenarioOptions {
   editor: EditorType;
   path?: PathToDocument;
   setup: EditorSetupForCompletion;
+  widgetPosition?: WidgetPositionInTheLayout;
 }
 export interface AutoGenerateTokensToComplete {
   tokenCount: TokenCount;
   tokenSize: TokenSize;
   [k: string]: any;
 }
 export interface IWillProvideACustomText {
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-debugger.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-debugger.ts`

 * *Files 22% similar despite different names*

```diff
@@ -9,12 +9,23 @@
  * Python code cells to execute one-by-one to populate the debugger namespace, e.g. `from numpy import *`
  */
 export type CodeToExecute = string[];
 /**
  * The scenario waits until debugger panel is populated with at least as many variables as specified. For accurate timings should have as many members as there are code cells.
  */
 export type ExpectedNumberOfVariables = number[];
+/**
+ * Where to attach the editor widget in the layout
+ */
+export type WidgetPositionInTheLayout =
+  | 'split-top'
+  | 'split-left'
+  | 'split-right'
+  | 'split-bottom'
+  | 'tab-before'
+  | 'tab-after';
 
 export interface DebuggerScenarioOptions {
   codeCells: CodeToExecute;
   expectedNumberOfVariables: ExpectedNumberOfVariables;
+  widgetPosition?: WidgetPositionInTheLayout;
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-scroll.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-scroll.ts`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,28 @@
  * If using a notebook, how many cell should be created? For file editor, how many lines?
  */
 export type NumberOfCellsBlocksToAppend = number;
 /**
  * Text to populate editors/cells with.
  */
 export type EditorCellContent = string;
+/**
+ * Where to attach the editor widget in the layout
+ */
+export type WidgetPositionInTheLayout =
+  | 'split-top'
+  | 'split-left'
+  | 'split-right'
+  | 'split-bottom'
+  | 'tab-before'
+  | 'tab-after';
 
 export interface ScrollScenarioOptions {
   scrollTop: ScrollFromTop;
   scrollBehavior: ScrollBehaviour;
   cellByCell?: TraverseCellByCell;
   editor: EditorType;
   path?: PathToDocument;
   cells: NumberOfCellsBlocksToAppend;
   editorContent?: EditorCellContent;
+  widgetPosition?: WidgetPositionInTheLayout;
 }
```

### Comparing `jupyterlab_ui_profiler-0.2.0/src/types/_scenario-tabs.ts` & `jupyterlab_ui_profiler-0.2.1/src/types/_scenario-tabs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/style/base.css` & `jupyterlab_ui_profiler-0.2.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/README.md` & `jupyterlab_ui_profiler-0.2.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/jupyter_server_test_config.py` & `jupyterlab_ui_profiler-0.2.1/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/yarn.lock` & `jupyterlab_ui_profiler-0.2.1/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/launcher-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/profiler.spec.ts-snapshots/ui-profiler-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/boxplot-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-options-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/result-summary-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rule-usage-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/rules-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-macro-trace-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/self-profiling-micro-details-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-blocks-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-rule-groups-rules-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/style-sheets-results-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png` & `jupyterlab_ui_profiler-0.2.1/ui-tests/tests/results.spec.ts-snapshots/ui-profiler-with-boxplot-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/.gitignore` & `jupyterlab_ui_profiler-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/LICENSE` & `jupyterlab_ui_profiler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/README.md` & `jupyterlab_ui_profiler-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/pyproject.toml` & `jupyterlab_ui_profiler-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_ui_profiler-0.2.0/PKG-INFO` & `jupyterlab_ui_profiler-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-ui-profiler
-Version: 0.2.0
+Version: 0.2.1
 Summary: JupyterLab extension for profiling UI performance
 Project-URL: Homepage, https://github.com/jupyterlab/ui-profiler
 Project-URL: Bug Tracker, https://github.com/jupyterlab/ui-profiler/issues
 Project-URL: Repository, https://github.com/jupyterlab/ui-profiler.git
 Author: Project Jupyter Contributors
 License: BSD 3-Clause License
```

