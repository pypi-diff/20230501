# Comparing `tmp/autora-core-3.0.0a6.tar.gz` & `tmp/autora-core-3.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-core-3.0.0a6.tar", last modified: Thu Apr 27 22:12:58 2023, max compression
+gzip compressed data, was "autora-core-3.0.0a7.tar", last modified: Mon May  1 16:04:24 2023, max compression
```

## Comparing `autora-core-3.0.0a6.tar` & `autora-core-3.0.0a7.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/autora-core.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/runConfigurations/pytest.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.687655 autora-core-3.0.0a6/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/conda/autora/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/conda/autora/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/conda/autora/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.687655 autora-core-3.0.0a6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/docs/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)   148488 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/cycle/simple_cycle_bms_model_poppernet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/docs/experimentalists/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/experimentalists/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.687655 autora-core-3.0.0a6/docs/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.691655 autora-core-3.0.0a6/docs/theorist/bms/
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bms/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bms/search_space.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1572980 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bms/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.695655 autora-core-3.0.0a6/docs/theorist/bsr/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bsr/how_it_works.md
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bsr/img.png
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bsr/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bsr/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/bsr/search_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.695655 autora-core-3.0.0a6/docs/theorist/darts/
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/darts/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   796078 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/docs/theorist/darts/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.687655 autora-core-3.0.0a6/mkdocs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.695655 autora-core-3.0.0a6/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.687655 autora-core-3.0.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.687655 autora-core-3.0.0a6/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.695655 autora-core-3.0.0a6/src/autora/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20109 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/cycle/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/cycle/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.695655 autora-core-3.0.0a6/src/autora/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.695655 autora-core-3.0.0a6/src/autora/experimentalist/pooler/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/pooler/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/pooler/random_pooler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/src/autora/experimentalist/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/sampler/assumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/sampler/dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/sampler/model_disagreement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/sampler/nearest_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/sampler/uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/experimentalist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/src/autora/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/synthetic/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/theorist/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/src/autora/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/utils/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/src/autora/variable/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/variable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/src/autora/variable/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/src/autora_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-04-27 22:12:58.000000 autora-core-3.0.0a6/src/autora_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-27 22:12:58.000000 autora-core-3.0.0a6/src/autora_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 22:12:58.000000 autora-core-3.0.0a6/src/autora_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-27 22:12:58.000000 autora-core-3.0.0a6/src/autora_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 22:12:58.000000 autora-core-3.0.0a6/src/autora_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 22:12:58.699655 autora-core-3.0.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/tests/test_cycle_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/tests/test_experimentalist_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/tests/test_experimentalist_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-27 22:12:46.000000 autora-core-3.0.0a6/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/autora-core.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/conda/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/conda/autora/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/conda/autora/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/docs/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)   148488 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/cycle/simple_cycle_bms_model_poppernet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/docs/experimentalists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/experimentalists/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/docs/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/docs/theorist/bms/
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bms/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bms/search_space.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1572980 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bms/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/docs/theorist/bsr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/how_it_works.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/img.png
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/meta_parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/search_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/docs/theorist/darts/
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/darts/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   796078 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/darts/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/mkdocs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20109 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/cycle/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/cycle/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/experimentalist/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/pooler/random_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/experimentalist/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/assumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/model_disagreement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/nearest_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/synthetic/inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/theorist/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/utils/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/variable/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/src/autora_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_cycle_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_experimentalist_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_synthetic_inventory.py
```

### Comparing `autora-core-3.0.0a6/.github/pull_request_template.md` & `autora-core-3.0.0a7/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.github/workflows/publish-package-pypi.yml` & `autora-core-3.0.0a7/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.github/workflows/test-pytest.yml` & `autora-core-3.0.0a7/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.gitignore` & `autora-core-3.0.0a7/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.idea/autora-core.iml` & `autora-core-3.0.0a7/.idea/autora-core.iml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.idea/inspectionProfiles/Project_Default.xml` & `autora-core-3.0.0a7/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.idea/runConfigurations/pytest.xml` & `autora-core-3.0.0a7/.idea/runConfigurations/pytest.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/.pre-commit-config.yaml` & `autora-core-3.0.0a7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/LICENSE.md` & `autora-core-3.0.0a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/PKG-INFO` & `autora-core-3.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0a6
+Version: 3.0.0a7
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
-Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: build
```

### Comparing `autora-core-3.0.0a6/README.md` & `autora-core-3.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/conda/autora/meta.yaml` & `autora-core-3.0.0a7/conda/autora/meta.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/cycle/simple_cycle_bms_model_poppernet.ipynb` & `autora-core-3.0.0a7/docs/cycle/simple_cycle_bms_model_poppernet.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/experimentalists/overview.md` & `autora-core-3.0.0a7/docs/experimentalists/overview.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bms/example.ipynb` & `autora-core-3.0.0a7/docs/theorist/bms/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bms/search_space.ipynb` & `autora-core-3.0.0a7/docs/theorist/bms/search_space.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bms/weber.ipynb` & `autora-core-3.0.0a7/docs/theorist/bms/weber.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bsr/how_it_works.md` & `autora-core-3.0.0a7/docs/theorist/bsr/how_it_works.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bsr/img.png` & `autora-core-3.0.0a7/docs/theorist/bsr/img.png`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bsr/introduction.md` & `autora-core-3.0.0a7/docs/theorist/bsr/introduction.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bsr/meta_parameters.md` & `autora-core-3.0.0a7/docs/theorist/bsr/meta_parameters.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/bsr/search_space.md` & `autora-core-3.0.0a7/docs/theorist/bsr/search_space.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/darts/example.ipynb` & `autora-core-3.0.0a7/docs/theorist/darts/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/docs/theorist/darts/weber.ipynb` & `autora-core-3.0.0a7/docs/theorist/darts/weber.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/mkdocs/overrides/main.html` & `autora-core-3.0.0a7/mkdocs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/mkdocs.yml` & `autora-core-3.0.0a7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/pyproject.toml` & `autora-core-3.0.0a7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 mypy_path="./src"
 
 [[tool.mypy.overrides]]
 module = ["matplotlib.*", "sklearn.*", "pandas.*", "numpy.*"]
 ignore_missing_imports=true
 
 [project.urls]
-homepage = "https://www.empiricalresearch.ai"
+homepage = "http://www.empiricalresearch.ai"
 repository = "https://github.com/AutoResearch/autora-theorist-template"
 documentation = "https://autoresearch.github.io/autora/"
 
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `autora-core-3.0.0a6/src/autora/cycle/plot_utils.py` & `autora-core-3.0.0a7/src/autora/cycle/plot_utils.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/cycle/simple.py` & `autora-core-3.0.0a7/src/autora/cycle/simple.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/pipeline.py` & `autora-core-3.0.0a7/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/pooler/grid.py` & `autora-core-3.0.0a7/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/pooler/random_pooler.py` & `autora-core-3.0.0a7/src/autora/experimentalist/pooler/random_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/sampler/assumption.py` & `autora-core-3.0.0a7/src/autora/experimentalist/sampler/assumption.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/sampler/dissimilarity.py` & `autora-core-3.0.0a7/src/autora/experimentalist/sampler/dissimilarity.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/sampler/model_disagreement.py` & `autora-core-3.0.0a7/src/autora/experimentalist/sampler/model_disagreement.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/sampler/nearest_value.py` & `autora-core-3.0.0a7/src/autora/experimentalist/sampler/nearest_value.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/sampler/uncertainty.py` & `autora-core-3.0.0a7/src/autora/experimentalist/sampler/uncertainty.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/experimentalist/utils.py` & `autora-core-3.0.0a7/src/autora/experimentalist/utils.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/synthetic/inventory.py` & `autora-core-3.0.0a7/src/autora/synthetic/inventory.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/variable/__init__.py` & `autora-core-3.0.0a7/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora/variable/time.py` & `autora-core-3.0.0a7/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/src/autora_core.egg-info/PKG-INFO` & `autora-core-3.0.0a7/src/autora_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0a6
+Version: 3.0.0a7
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
-Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: build
```

### Comparing `autora-core-3.0.0a6/src/autora_core.egg-info/SOURCES.txt` & `autora-core-3.0.0a7/src/autora_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/tests/README.md` & `autora-core-3.0.0a7/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/tests/test_cycle_plots.py` & `autora-core-3.0.0a7/tests/test_cycle_plots.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/tests/test_experimentalist_pipeline.py` & `autora-core-3.0.0a7/tests/test_experimentalist_pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/tests/test_experimentalist_random.py` & `autora-core-3.0.0a7/tests/test_experimentalist_random.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a6/tests/test_synthetic_inventory.py` & `autora-core-3.0.0a7/tests/test_synthetic_inventory.py`

 * *Files identical despite different names*

