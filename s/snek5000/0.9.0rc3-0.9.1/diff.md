# Comparing `tmp/snek5000-0.9.0rc3.tar.gz` & `tmp/snek5000-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek5000-0.9.0rc3.tar", last modified: Fri Jan  6 09:01:44 2023, max compression
+gzip compressed data, was "snek5000-0.9.1.tar", last modified: Mon May  1 21:08:54 2023, max compression
```

## Comparing `snek5000-0.9.0rc3.tar` & `snek5000-0.9.1.tar`

### file list

```diff
@@ -1,217 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.932939 snek5000-0.9.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.exrc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.896939 snek5000-0.9.0rc3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.896939 snek5000-0.9.0rc3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-01-06 09:01:44.932939 snek5000-0.9.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/activate.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.904939 snek5000-0.9.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)   114703 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.904939 snek5000-0.9.0rc3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/_static/doxy_style.css
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/_static/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/_static/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.904939 snek5000-0.9.0rc3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/autosum.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.892939 snek5000-0.9.0rc3/docs/debug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.904939 snek5000-0.9.0rc3/docs/debug/gh-163-snakemake-resources/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/debug/gh-163-snakemake-resources/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/debug/gh-163-snakemake-resources/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/debug/gh-163-snakemake-resources/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/debug/gh-163-snakemake-resources/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.908939 snek5000-0.9.0rc3/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/edit_tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/filtering.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/howto_doc.md
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/howto_test.md
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/nek.rst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/output.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/phys_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/release.md
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/dev/solver.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.892939 snek5000-0.9.0rc3/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.908939 snek5000-0.9.0rc3/docs/examples/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/scripts/simul_cbox_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/scripts/tuto_cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/scripts/tuto_phill.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/scripts/tuto_tgv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.908939 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.892939 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.908939 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/canonical.usr.f
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/phys_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.912939 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   100219 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/ref_data_spectral_code.csv
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.892939 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.912939 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.par.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.usr.f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.916939 snek5000-0.9.0rc3/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/archive-simulation-data.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/control-fortran-warnings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/export-sans-snek5000.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/history_points.md
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/load_plot_log_data.md
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/load_state_stat_files.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/read-write-par-files.md
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/rebuild-nek.md
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/restart.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/run-background-foreground.md
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/snek-make.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/how-to/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/html_theme_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/install_opt.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/ls_intersphinx_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/ls_no_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_cbox.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_packaging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_phill_make.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_phill_script.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_phill_setup.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tuto_tgv.myst.md
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.916939 snek5000-0.9.0rc3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/default.nix
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/tests-editable.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/requirements/vcs_packages.in
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-06 09:01:44.932939 snek5000-0.9.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.892939 snek5000-0.9.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.920939 snek5000-0.9.0rc3/src/snek5000/
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/make.py
--rw-r--r--   0 runner    (1001) docker     (123)    21441 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.920939 snek5000-0.9.0rc3/src/snek5000/output/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27790 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/history_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/phys_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/print_stdout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.920939 snek5000-0.9.0rc3/src/snek5000/output/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/readers/pymech_.py
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/readers/try_paraview_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/remaining_clock_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/simple_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/output/spatial_means.py
--rw-r--r--   0 runner    (1001) docker     (123)    17634 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.924939 snek5000-0.9.0rc3/src/snek5000/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/SIZE.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/box.j2
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/compile.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/compiler.smk
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/default_configfile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/internal.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/io.smk
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/makefile_usr.inc.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/resources/nek5000.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.924939 snek5000-0.9.0rc3/src/snek5000/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/solvers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/solvers/kth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.928939 snek5000-0.9.0rc3/src/snek5000/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/gfortran_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/src/snek5000/util/smake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.920939 snek5000-0.9.0rc3/src/snek5000.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-06 09:01:44.000000 snek5000-0.9.0rc3/src/snek5000.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.932939 snek5000-0.9.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_load_simul.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 09:01:44.932939 snek5000-0.9.0rc3/tests/test_oper/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_oper/test_box_2d.box
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_oper/test_box_template.box
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_oper/test_size_2d.f
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_oper/test_size_template.f
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_oper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_restart_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_sim_executed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_tgv.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_tuto_packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-06 09:01:26.000000 snek5000-0.9.0rc3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.341755 snek5000-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-01 21:08:34.000000 snek5000-0.9.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-01 21:08:34.000000 snek5000-0.9.1/.exrc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 21:08:34.000000 snek5000-0.9.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 21:08:34.000000 snek5000-0.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.277754 snek5000-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 21:08:34.000000 snek5000-0.9.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.277754 snek5000-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-01 21:08:34.000000 snek5000-0.9.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-01 21:08:34.000000 snek5000-0.9.1/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 21:08:34.000000 snek5000-0.9.1/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-01 21:08:34.000000 snek5000-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-01 21:08:34.000000 snek5000-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 21:08:34.000000 snek5000-0.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 21:08:34.000000 snek5000-0.9.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-01 21:08:34.000000 snek5000-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-01 21:08:34.000000 snek5000-0.9.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-01 21:08:34.000000 snek5000-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 21:08:34.000000 snek5000-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 21:08:34.000000 snek5000-0.9.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-01 21:08:54.341755 snek5000-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-01 21:08:34.000000 snek5000-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-01 21:08:34.000000 snek5000-0.9.1/activate.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.289754 snek5000-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)   114703 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.289754 snek5000-0.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/_static/doxy_style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/_static/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/_static/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.293754 snek5000-0.9.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/autosum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.261754 snek5000-0.9.1/docs/debug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.293754 snek5000-0.9.1/docs/debug/gh-163-snakemake-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/debug/gh-163-snakemake-resources/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/debug/gh-163-snakemake-resources/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/debug/gh-163-snakemake-resources/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/debug/gh-163-snakemake-resources/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.297754 snek5000-0.9.1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/edit_tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/howto_doc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/howto_test.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/nek.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/phys_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/release.md
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/dev/solver.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.265754 snek5000-0.9.1/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.301754 snek5000-0.9.1/docs/examples/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/scripts/simul_cbox_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/scripts/tuto_cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/scripts/tuto_phill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/scripts/tuto_tgv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.301754 snek5000-0.9.1/docs/examples/snek5000-canonical/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.265754 snek5000-0.9.1/docs/examples/snek5000-canonical/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.305754 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/canonical.usr.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/phys_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.305754 snek5000-0.9.1/docs/examples/snek5000-tgv/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   100219 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/ref_data_spectral_code.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.265754 snek5000-0.9.1/docs/examples/snek5000-tgv/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.309754 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.par.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.usr.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.317754 snek5000-0.9.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/adaptive_time_step.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/archive-simulation-data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/config-c-fortran-compilers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/control-fortran-warnings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/export-sans-snek5000.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/history_points.md
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/load_plot_log_data.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/load_state_stat_files.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/read-write-par-files.md
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/rebuild-nek.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/restart.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/run-background-foreground.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/snek-make.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/how-to/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/html_theme_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/install_opt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.317754 snek5000-0.9.1/docs/joss_paper/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/joss_paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/joss_paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/joss_paper/generate_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/joss_paper/joss-defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/joss_paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/joss_paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/ls_intersphinx_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/ls_no_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_cbox.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_packaging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_phill_make.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_phill_script.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_phill_setup.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tuto_tgv.myst.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-01 21:08:34.000000 snek5000-0.9.1/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-05-01 21:08:34.000000 snek5000-0.9.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-01 21:08:34.000000 snek5000-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.321754 snek5000-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/default.nix
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/tests-editable.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 21:08:34.000000 snek5000-0.9.1/requirements/vcs_packages.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-01 21:08:54.341755 snek5000-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.269754 snek5000-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.325755 snek5000-0.9.1/src/snek5000/
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21441 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.333754 snek5000-0.9.1/src/snek5000/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28030 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/history_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/phys_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/print_stdout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.333754 snek5000-0.9.1/src/snek5000/output/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/readers/pymech_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/readers/try_paraview_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/remaining_clock_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/simple_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/output/spatial_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17643 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.333754 snek5000-0.9.1/src/snek5000/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/SIZE.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/box.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/compile.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/compiler.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/default_configfile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/internal.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/io.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/makefile_usr.inc.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/resources/nek5000.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.333754 snek5000-0.9.1/src/snek5000/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/solvers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/solvers/kth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.337755 snek5000-0.9.1/src/snek5000/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/gfortran_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 21:08:34.000000 snek5000-0.9.1/src/snek5000/util/smake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.329754 snek5000-0.9.1/src/snek5000.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 21:08:54.000000 snek5000-0.9.1/src/snek5000.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.341755 snek5000-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_load_simul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:08:54.341755 snek5000-0.9.1/tests/test_oper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_oper/test_box_2d.box
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_oper/test_box_template.box
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_oper/test_size_2d.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_oper/test_size_template.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_oper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_restart_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_sim_executed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_tgv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_tuto_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-01 21:08:34.000000 snek5000-0.9.1/tests/test_util.py
```

### Comparing `snek5000-0.9.0rc3/.editorconfig` & `snek5000-0.9.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/.exrc` & `snek5000-0.9.1/.exrc`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/.github/workflows/build.yaml` & `snek5000-0.9.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/.github/workflows/deploy.yaml` & `snek5000-0.9.1/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/.gitignore` & `snek5000-0.9.1/.gitignore`

 * *Files 23% similar despite different names*

```diff
@@ -93,7 +93,11 @@
 bin/*.stdout
 bin/*.stderr
 bin/launcher_*.*
 bin/*_JOB.md
 
 # Nix
 requirements/.mamba
+
+# paper
+docs/joss_paper/*.pdf
+docs/joss_paper/.whedon
```

### Comparing `snek5000-0.9.0rc3/.pre-commit-config.yaml` & `snek5000-0.9.1/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -6,30 +6,26 @@
   hooks:
   - id: check-toml
   - id: check-yaml
   - id: end-of-file-fixer
   - id: check-added-large-files
 
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.3.0
   hooks:
   - id: black
-- repo: https://github.com/PyCQA/isort
-  rev: 5.11.4
+- repo: https://github.com/charliermarsh/ruff-pre-commit
+  rev: v0.0.262
   hooks:
-  - id: isort
-- repo: https://github.com/PyCQA/flake8
-  rev: 6.0.0
-  hooks:
-  - id: flake8
+  - id: ruff
 - repo: https://github.com/snakemake/snakefmt
-  rev: v0.8.0
+  rev: v0.8.4
   hooks:
   - id: snakefmt
-- repo: https://github.com/executablebooks/mdformat
-  rev: 0.7.16
-  hooks:
-  - id: mdformat
-    additional_dependencies:
-    - mdformat-tables
-    - mdformat-frontmatter
-    - mdformat-myst
+# - repo: https://github.com/executablebooks/mdformat
+#   rev: 0.7.16
+#   hooks:
+#   - id: mdformat
+#     additional_dependencies:
+#     - mdformat-tables
+#     - mdformat-frontmatter
+#     - mdformat-myst
```

### Comparing `snek5000-0.9.0rc3/.readthedocs.yml` & `snek5000-0.9.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/CHANGELOG.md` & `snek5000-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,24 +26,40 @@
 
 -->
 
 <!-- (changelog/unreleased)= -->
 
 ## [Unreleased]
 
-### Added
+## [0.9.1] - 2023-05-01
 
-- {func}`snek5000.output.base.Output.post_init_create_additional_source_files`,
-  {func}`snek5000.resources.get_base_templates` and
-  {func}`snek5000.resources.get_base_template`.
+## Added
+
+- New command `snek-make-nek` to clean and rebuild Nek5000 tools
+- JOSS paper draft
+
+Documentation
 
-## [0.9.0rc0]
+- How to use adaptive time step
+- How to configure C and Fortran compilers
+- Document the new copier template
+
+## Changed
+
+- Use `remaining_clock_time` by default
+- Replace isort and flake8 with ruff, upgrade hooks
+
+## [0.9.0] - 2023-01-11
 
 ### Added
 
+- {mod}`snek5000.output.remaining_clock_time`.
+- {func}`snek5000.output.base.Output.post_init_create_additional_source_files`,
+  {func}`snek5000.resources.get_base_templates` and
+  {func}`snek5000.resources.get_base_template`.
 - {class}`snek5000.output.spatial_means.SpatialMeans`.
 - New block `user_size` in `SIZE.j2` template (see {mod}`snek5000.resources`).
 
 ### Removed
 
 - Functions deprecated in 0.8.0 (`source_root`, `get_asset`, `get_root`,
   `get_configfile`, `_complete_params_from_par_file`).
@@ -375,10 +391,11 @@
 [0.4.1b0]: https://github.com/snek5000/snek5000/compare/0.4.0b1...0.4.1b0
 [0.4.1b1]: https://github.com/snek5000/snek5000/compare/0.4.1b0...0.4.1b1
 [0.5.0b0]: https://github.com/snek5000/snek5000/compare/0.4.1b1...0.5.0b0
 [0.6.0b0]: https://github.com/snek5000/snek5000/compare/0.5.0b0...0.6.0b0
 [0.6.1b0]: https://github.com/snek5000/snek5000/compare/0.6.0b0...0.6.1b0
 [0.7.0b0]: https://github.com/snek5000/snek5000/compare/0.6.1b0...0.7.0b0
 [0.8.0]: https://github.com/snek5000/snek5000/compare/0.7.0b0...0.8.0
-[0.9.0rc0]: https://github.com/snek5000/snek5000/compare/0.8.0...0.9.0rc0
+[0.9.0]: https://github.com/snek5000/snek5000/compare/0.8.0...0.9.0
+[0.9.1]: https://github.com/snek5000/snek5000/compare/0.9.0...0.9.1
 [@paugier]: https://github.com/paugier
-[unreleased]: https://github.com/snek5000/snek5000/compare/0.8.0...HEAD
+[unreleased]: https://github.com/snek5000/snek5000/compare/0.9.1...HEAD
```

### Comparing `snek5000-0.9.0rc3/CITATION.cff` & `snek5000-0.9.1/CITATION.cff`

 * *Files 27% similar despite different names*

```diff
@@ -16,11 +16,12 @@
   - family-names: Khoubani
     given-names: Arman
 
   - family-names: Augier
     given-names: Pierre
     orcid: https://orcid.org/0000-0001-9481-4459
 
+version: 0.9.1
+date-released: 2023-05-01
 doi: 10.5281/zenodo.7399621
-date-released: 2022-12-06
 license: BSD-3-Clause
 repository-code: "https://github.com/snek5000/snek5000"
```

### Comparing `snek5000-0.9.0rc3/CONTRIBUTING.md` & `snek5000-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/LICENSE` & `snek5000-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/Makefile` & `snek5000-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/PKG-INFO` & `snek5000-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek5000
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: Python framework for Nek5000
 Home-page: https://github.com/snek5000/snek5000
 Author: Ashwin Vishnu Mohanan
 Author-email: ashwinvis+gh@protonmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/snek5000/snek5000/issues
 Project-URL: Documentation, https://snek5000.readthedocs.io
@@ -47,15 +47,15 @@
 **Documentation**: <https://snek5000.readthedocs.io/>
 
 Snek5000 is a Python package which allows one to write [Fluidsim] solvers based
 for the simulations on the Fortran [CFD] code [Nek5000]. There are open-source
 solvers (in particular [snek5000-phill], [snek5000-cbox] and [snek5000-tgv])
 and it's not difficult to write your own solver based on your Nek5000 cases (as
 shown in [this
-tutorial](https://snek5000.readthedocs.io/en/latest/packaging.html)).
+tutorial](https://snek5000.readthedocs.io/en/latest/tuto_packaging.html)).
 
 With a Snek5000-Fluidsim solver, it becomes very easy to
 
 - launch/restart simulations with Python scripts and terminal commands,
 - load simulations, read the associated parameters/data and produce nice
   figures/movies.
```

### Comparing `snek5000-0.9.0rc3/README.md` & `snek5000-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 **Documentation**: <https://snek5000.readthedocs.io/>
 
 Snek5000 is a Python package which allows one to write [Fluidsim] solvers based
 for the simulations on the Fortran [CFD] code [Nek5000]. There are open-source
 solvers (in particular [snek5000-phill], [snek5000-cbox] and [snek5000-tgv])
 and it's not difficult to write your own solver based on your Nek5000 cases (as
 shown in [this
-tutorial](https://snek5000.readthedocs.io/en/latest/packaging.html)).
+tutorial](https://snek5000.readthedocs.io/en/latest/tuto_packaging.html)).
 
 With a Snek5000-Fluidsim solver, it becomes very easy to
 
 - launch/restart simulations with Python scripts and terminal commands,
 - load simulations, read the associated parameters/data and produce nice
   figures/movies.
```

### Comparing `snek5000-0.9.0rc3/activate.sh` & `snek5000-0.9.1/activate.sh`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/CHANGELOG.md` & `snek5000-0.9.1/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,24 +26,40 @@
 
 -->
 
 <!-- (changelog/unreleased)= -->
 
 ## [Unreleased]
 
-### Added
+## [0.9.1] - 2023-05-01
 
-- {func}`snek5000.output.base.Output.post_init_create_additional_source_files`,
-  {func}`snek5000.resources.get_base_templates` and
-  {func}`snek5000.resources.get_base_template`.
+## Added
+
+- New command `snek-make-nek` to clean and rebuild Nek5000 tools
+- JOSS paper draft
+
+Documentation
 
-## [0.9.0rc0]
+- How to use adaptive time step
+- How to configure C and Fortran compilers
+- Document the new copier template
+
+## Changed
+
+- Use `remaining_clock_time` by default
+- Replace isort and flake8 with ruff, upgrade hooks
+
+## [0.9.0] - 2023-01-11
 
 ### Added
 
+- {mod}`snek5000.output.remaining_clock_time`.
+- {func}`snek5000.output.base.Output.post_init_create_additional_source_files`,
+  {func}`snek5000.resources.get_base_templates` and
+  {func}`snek5000.resources.get_base_template`.
 - {class}`snek5000.output.spatial_means.SpatialMeans`.
 - New block `user_size` in `SIZE.j2` template (see {mod}`snek5000.resources`).
 
 ### Removed
 
 - Functions deprecated in 0.8.0 (`source_root`, `get_asset`, `get_root`,
   `get_configfile`, `_complete_params_from_par_file`).
@@ -375,10 +391,11 @@
 [0.4.1b0]: https://github.com/snek5000/snek5000/compare/0.4.0b1...0.4.1b0
 [0.4.1b1]: https://github.com/snek5000/snek5000/compare/0.4.1b0...0.4.1b1
 [0.5.0b0]: https://github.com/snek5000/snek5000/compare/0.4.1b1...0.5.0b0
 [0.6.0b0]: https://github.com/snek5000/snek5000/compare/0.5.0b0...0.6.0b0
 [0.6.1b0]: https://github.com/snek5000/snek5000/compare/0.6.0b0...0.6.1b0
 [0.7.0b0]: https://github.com/snek5000/snek5000/compare/0.6.1b0...0.7.0b0
 [0.8.0]: https://github.com/snek5000/snek5000/compare/0.7.0b0...0.8.0
-[0.9.0rc0]: https://github.com/snek5000/snek5000/compare/0.8.0...0.9.0rc0
+[0.9.0]: https://github.com/snek5000/snek5000/compare/0.8.0...0.9.0
+[0.9.1]: https://github.com/snek5000/snek5000/compare/0.9.0...0.9.1
 [@paugier]: https://github.com/paugier
-[unreleased]: https://github.com/snek5000/snek5000/compare/0.8.0...HEAD
+[unreleased]: https://github.com/snek5000/snek5000/compare/0.9.1...HEAD
```

### Comparing `snek5000-0.9.0rc3/docs/CONTRIBUTING.md` & `snek5000-0.9.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/Doxyfile` & `snek5000-0.9.1/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/LICENSE` & `snek5000-0.9.1/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/Makefile` & `snek5000-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/_static/favicon.ico` & `snek5000-0.9.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/_static/icon.png` & `snek5000-0.9.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/_static/icon.svg` & `snek5000-0.9.1/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/_templates/layout.html` & `snek5000-0.9.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/conf.py` & `snek5000-0.9.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = [
     "_build",
     "Thumbs.db",
     ".DS_Store",
     "examples/snek5000-*/README.md",
+    "joss_paper/paper.md",
 ]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
```

### Comparing `snek5000-0.9.0rc3/docs/debug/gh-163-snakemake-resources/noxfile.py` & `snek5000-0.9.1/docs/debug/gh-163-snakemake-resources/noxfile.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/edit_tutorials.md` & `snek5000-0.9.1/docs/dev/edit_tutorials.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/filtering.rst` & `snek5000-0.9.1/docs/dev/filtering.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/howto_test.md` & `snek5000-0.9.1/docs/dev/howto_test.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/index.rst` & `snek5000-0.9.1/docs/dev/index.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/nek.rst` & `snek5000-0.9.1/docs/dev/nek.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/output.rst` & `snek5000-0.9.1/docs/dev/output.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/params.rst` & `snek5000-0.9.1/docs/dev/params.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/release.md` & `snek5000-0.9.1/docs/dev/release.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # How to release
 
 ## Via GitHub Actions
 
-- Update {ref}`changelog/unreleased` with version comparison links and detailed
-  description.
+- Update [Unreleased](../CHANGELOG.md#unreleased) with version comparison links and
+  detailed description.
 - Update version and date in `CITATION.cff`.
 - Make a [new release] on Github.
 - Inspect upload in [TestPyPI].
 - Execute manual [deploy workflow] to download from [TestPyPI], run tests and publish to
   [PyPI].
 
 ## Manual method (not recommended)
```

### Comparing `snek5000-0.9.0rc3/docs/dev/roadmap.rst` & `snek5000-0.9.1/docs/dev/roadmap.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/dev/solver.rst` & `snek5000-0.9.1/docs/dev/solver.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/scripts/simul_cbox_movie.py` & `snek5000-0.9.1/docs/examples/scripts/simul_cbox_movie.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/scripts/tuto_cbox.py` & `snek5000-0.9.1/docs/examples/scripts/tuto_cbox.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/scripts/tuto_tgv.py` & `snek5000-0.9.1/docs/examples/scripts/tuto_tgv.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-canonical/LICENSE` & `snek5000-0.9.1/docs/examples/snek5000-canonical/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2019, Ashwin Vishnu
+Copyright (c) 2023, Ashwin Vishnu
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/Snakefile` & `snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/Snakefile`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/output.py` & `snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from snek5000.output.base import Output as OutputBase
 from snek5000.resources import get_base_templates
 
 box, makefile_usr, size = get_base_templates()
 
 
 class OutputCanonical(OutputBase):
-
     template_box = box
     template_makefile_usr = makefile_usr
     template_size = size
 
     @classmethod
     def _set_info_solver_classes(cls, classes):
         """Set the classes for info_solver.classes.Output
```

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/phys_fields.py` & `snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/phys_fields.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-canonical/src/snek5000_canonical/solver.py` & `snek5000-0.9.1/docs/examples/snek5000-canonical/src/snek5000_canonical/solver.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-tgv/LICENSE` & `snek5000-0.9.1/docs/examples/snek5000-tgv/LICENSE`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-tgv/ref_data_spectral_code.csv` & `snek5000-0.9.1/docs/examples/snek5000-tgv/ref_data_spectral_code.csv`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/Snakefile` & `snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/Snakefile`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/output.py` & `snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/output.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,17 +26,9 @@
             "SpatialMeans",
             dict(
                 module_name="snek5000.output.spatial_means",
                 class_name="SpatialMeans",
             ),
         )
 
-        classes._set_child(
-            "RemainingClockTime",
-            dict(
-                module_name="snek5000.output.remaining_clock_time",
-                class_name="RemainingClockTime",
-            ),
-        )
-
 
 Output = OutputTGV
```

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/solver.py` & `snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
 
         # Snek5000 also has a human-friendly interface for userParams## parameter in the par file
         # Here we map the mesh length to userParam01, which is used in subroutine usrdat
         params.oper._record_nek_user_params({"Lx": 1})
 
         # Read defaults for `params.nek` from `tgv.par.cfg` (original code)
         complete_params_from_par_file(
-            params, Path(__file__).parent / f"{cls.info_solver.short_name}.par.cfg"
+            params,
+            Path(__file__).parent / f"{cls.info_solver.short_name}.par.cfg",
         )
 
         # Boundary conditions
         # Symmetric on top and bottom; periodic on all 6 faces
         params.oper.boundary = ["P"] * 6
 
         # NOTE: These are only default parameters for a minimal simulation -
```

### Comparing `snek5000-0.9.0rc3/docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.usr.f` & `snek5000-0.9.1/docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.usr.f`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/archive-simulation-data.md` & `snek5000-0.9.1/docs/how-to/archive-simulation-data.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/export-sans-snek5000.myst.md` & `snek5000-0.9.1/docs/how-to/export-sans-snek5000.myst.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/history_points.md` & `snek5000-0.9.1/docs/how-to/history_points.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```py
 params.output.history_points.write_interval: int = ...
 params.output.history_points.coords: list[tuple[float, float, float] | tuple[float, float]] = ...
 ```
 
 For example, see the
-[parameters used in the tutorial for snek5000-cbox](../tuto_cbox.myst.md#a-more-advanced-script-adated-for-a-particular-instability).
+[parameters used in the tutorial for snek5000-cbox](../tuto_cbox.myst.md#a-more-advanced-script-adapted-for-a-particular-instability).
 
 This should be coupled along with a `hpts()` call in `userchk()` subroutine in the
 Nek5000 user file. For more information, see *documentation for
 `params.output.history_points`* in {class}`snek5000.output.base.Output`.
 
 ## Loading and plotting
```

### Comparing `snek5000-0.9.0rc3/docs/how-to/load_plot_log_data.md` & `snek5000-0.9.1/docs/how-to/load_plot_log_data.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/load_state_stat_files.md` & `snek5000-0.9.1/docs/how-to/load_state_stat_files.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/read-write-par-files.md` & `snek5000-0.9.1/docs/how-to/read-write-par-files.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/restart.myst.md` & `snek5000-0.9.1/docs/how-to/restart.myst.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/run-background-foreground.md` & `snek5000-0.9.1/docs/how-to/run-background-foreground.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/snek-make.myst.md` & `snek5000-0.9.1/docs/how-to/snek-make.myst.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/how-to/templates.md` & `snek5000-0.9.1/docs/how-to/templates.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/html_theme_options.py` & `snek5000-0.9.1/docs/html_theme_options.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/index.rst` & `snek5000-0.9.1/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,17 @@
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to *Snek5000*'s documentation!
 ======================================
 
 Snek5000 is a Python package and a thin interface over Nek5000_. It provides a
-framework to organize parameters and launch multiple simulations. Snek5000's
-internals rely on FluidSim's core_ to build its API.
+framework to (i) organize parameters, (ii) launch/restart multiple simulations
+and (iii) load simulations to read the associated parameters/data and produce
+nice figures/movies.
 
 .. raw:: html
 
    <!--
       Icon derived from "wind slap icon" by Lorc. Available at
       https://game-icons.net/1x1/lorc/wind-slap.html .
       License: https://creativecommons.org/licenses/by/3.0/
```

### Comparing `snek5000-0.9.0rc3/docs/install.rst` & `snek5000-0.9.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/install_opt.rst` & `snek5000-0.9.1/docs/install_opt.rst`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/ls_intersphinx_targets.py` & `snek5000-0.9.1/docs/ls_intersphinx_targets.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/ls_no_extensions.py` & `snek5000-0.9.1/docs/ls_no_extensions.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/make.bat` & `snek5000-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/tuto_cbox.myst.md` & `snek5000-0.9.1/docs/tuto_cbox.myst.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 # Demo sidewall convection (`snek5000-cbox` solver)
 
-## A more advanced script adated for a particular instability
+## A more advanced script adapted for a particular instability
 
 This example is based on
 [the study *From onset of unsteadiness to chaos in a differentially heated square cavity* by Le Quéré & Behnia (1998)](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/from-onset-of-unsteadiness-to-chaos-in-a-differentially-heated-square-cavity/617F4CB2C23DD74C3D0CB872AE7C0045).
 
 The configuration is convection in a 2D square cavity heated and cooled at two opposite
 sides. The control parameters are the Prandtl number $Pr= 0.71$ and the Rayleigh number
 $Ra = 2 \times 10^{8}$. The mesh size is $64 \times 64$ (8 elements in each direction).
```

### Comparing `snek5000-0.9.0rc3/docs/tuto_config.rst` & `snek5000-0.9.1/docs/tuto_config.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 run, but also the **compilation** and **execution**, you would often need to customize
 the compiler and its flags. By default it is configured to use gcc,
 gfortran and OpenMPI to compile the code.
 
 .. literalinclude:: ../src/snek5000/resources/default_configfile.yml
    :language: yaml
 
+.. _config_files:
+
 Customization via config files
 ------------------------------
 
 You are expected to keep one configuration file for per machine / cluster where
 ``snek5000`` is executed. When a file is not found during runtime it issues a
 warning similar to::
 
@@ -53,14 +55,16 @@
 
 .. code-block:: python
 
    sim.output.write_snakemake_config(
        custom_env_vars={"MPIEXEC_FLAGS": "--report-pid PID.txt"}
    )
 
+.. _override_config_env:
+
 Overriding configuration with environment variables
 ---------------------------------------------------
 
 To allow for reproducible runs, it is discouraged to rely on environment
 variables to set the configuration. Nevertheless, it is possible to do so by
 setting up the environment variable ``SNEK_UPDATE_CONFIG_ENV_SENSITIVE`` as
 follows::
```

### Comparing `snek5000-0.9.0rc3/docs/tuto_packaging.rst` & `snek5000-0.9.1/docs/tuto_packaging.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _packaging:
 
 Create your own Snek5000 solver, packaging your Nek5000 user source code
 ========================================================================
 
+.. tip::
+   You can now use the Copier template
+   <https://github.com/snek5000/template-snek5000-solver/> to render the
+   following packaging structure effortlessly!
+
+
 This document describes how to package a Nek5000 source code in your own
 repository via ``snek5000``'s API. What is described is the bare minimum to
 get started.  Assume your files are named ``canonical.usr``, ``canonical.par``
 etc. and you wish to package it under a name say ``snek5000_canonical``.
 
 .. note::
    The package name does not have to contain ``snek5000`` or ``canonical``. It
@@ -15,16 +21,15 @@
 
 One first has to create a directory structure, (preferably in a git / mercurial
 repository) like this::
 
    .
    ├── LICENSE
    ├── README.md
-   ├── setup.cfg
-   ├── setup.py
+   ├── pyproject.toml
    └── src
        └── snek5000_canonical
            ├── Snakefile
            ├── __init__.py
            ├── canonical.usr.f
            ├── output.py
            └── solver.py
@@ -36,26 +41,23 @@
 
 .. note::
 
    The Nek5000 ``.usr`` files have to contain Fortran 77 code in strict form
    layout. In snek5000 solvers, one can rename this file with the ``.usr.f``
    extension so that editors can correctly highlight the Fortran code.
 
-setup.py
---------
-
-.. literalinclude:: examples/snek5000-canonical/setup.py
-
 .. _setup.cfg:
+.. _pyproject.toml:
 
-setup.cfg
----------
+pyproject.toml
+--------------
 
-.. literalinclude:: examples/snek5000-canonical/setup.cfg
-   :language: cfg
+.. literalinclude:: examples/snek5000-canonical/pyproject.toml
+   :language: toml
+   :end-before: [tool.coverage.run]
 
 .. _init.py:
 
 src/snek5000_canonical/__init__.py
 ----------------------------------
 
 .. literalinclude:: examples/snek5000-canonical/src/snek5000_canonical/__init__.py
```

### Comparing `snek5000-0.9.0rc3/docs/tuto_phill_make.myst.md` & `snek5000-0.9.1/docs/tuto_phill_make.myst.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/tuto_phill_script.myst.md` & `snek5000-0.9.1/docs/tuto_phill_script.myst.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/tuto_phill_setup.myst.md` & `snek5000-0.9.1/docs/tuto_phill_setup.myst.md`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 One can also print only one section:
 
 ```{code-cell}
 print(params.nek.general)
 ```
 
-of alternatively, with the method `_print_as_code` (useful for copy-pasting):
+or alternatively, with the method `_print_as_code` (useful for copy-pasting):
 
 ```{code-cell}
 params.nek.general._print_as_code()
 ```
 
 Note that it is easy to print some help about some parameters:
```

### Comparing `snek5000-0.9.0rc3/docs/tuto_tgv.myst.md` & `snek5000-0.9.1/docs/tuto_tgv.myst.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/docs/tutorials.md` & `snek5000-0.9.1/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/noxfile.py` & `snek5000-0.9.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,15 +297,16 @@
                 "logs",
                 "*.tar.gz",
                 "*.f?????",
             )
         )
     )
     run_ext(
-        session, f"ctags -f {output} --language-force=Fortran -R {sources['nek5000']}"
+        session,
+        f"ctags -f {output} --language-force=Fortran -R {sources['nek5000']}",
     )
     run_ext(session, f"ctags -f {output} {excludes} --append -R {sources['snek5000']}")
 
 
 @no_venv_session
 def testpypi(session):
     """Release clean, build, upload to TestPyPI"""
@@ -378,15 +379,21 @@
     if BUILD_SYSTEM == "poetry":
         poetry_conf = CWD / "poetry.toml"
         assert (
             not poetry_conf.exists()
         ), "Poetry local configuration exists. Please remove to continue"
         session.install("poetry")
         session.run(
-            "python", "-m", "poetry", "config", "--local", "virtualenvs.create", "false"
+            "python",
+            "-m",
+            "poetry",
+            "config",
+            "--local",
+            "virtualenvs.create",
+            "false",
         )
         pytest_cmd = install_with_tests(session, ["--no-root"])
     else:
         pytest_cmd = install_with_tests(session)
 
     dist_packages = [str(p) for p in Path("./dist").glob(pattern)]
     session.install(*dist_packages)
```

### Comparing `snek5000-0.9.0rc3/pyproject.toml` & `snek5000-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     "setuptools_scm[toml]>=7.0.0",
     ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/snek5000/_version.py"
 
-[tool.isort]
-known_first_party = ["fluiddyn", "fluidsim_core", "snek5000"]
-# multi_line_output = 3
-profile = "black"
-line_length = 82
+[tool.ruff]
+ignore = ["E501", "W505"]
+
+[tool.ruff.isort]
+known-first-party = ["fluiddyn", "fluidsim_core", "snek5000"]
 
 [tool.coverage.run]
 source = ["snek5000", "snek5000_canonical", "./tests"]
 data_file = ".coverage/coverage"
 omit = [
     "*/try_*.py",
     "*/_old_*.py"
```

### Comparing `snek5000-0.9.0rc3/requirements/default.nix` & `snek5000-0.9.1/requirements/default.nix`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/requirements/dev.txt` & `snek5000-0.9.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/requirements/docs.txt` & `snek5000-0.9.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/requirements/main.txt` & `snek5000-0.9.1/requirements/main.txt`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/requirements/tests-editable.txt` & `snek5000-0.9.1/requirements/tests-editable.txt`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/requirements/tests.txt` & `snek5000-0.9.1/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/setup.cfg` & `snek5000-0.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 	kth = snek5000.solvers.kth
 console_scripts = 
 	snek-generate-config = snek5000.config:ensure_config_file
 	snek-info = snek5000.util.console:print_versions
 	snek-ipy-load = snek5000.util.console:start_ipython_load_sim
 	snek-make = snek5000.make:snek_make
 	snek-restart = snek5000.util.restart:main
+	snek-make-nek = snek5000.make:snek_make_nek
 
 [options.extras_require]
 docs = 
 	sphinx
 	myst-parser
 	myst-nb
 	docutils <0.18, >=0.14  # sphinx, myst-parser and myst-nb is incompatible with docutils==0.18
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/__init__.py` & `snek5000-0.9.1/src/snek5000/__init__.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/clusters.py` & `snek5000-0.9.1/src/snek5000/clusters.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/config.py` & `snek5000-0.9.1/src/snek5000/config.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/const.py` & `snek5000-0.9.1/src/snek5000/const.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/info.py` & `snek5000-0.9.1/src/snek5000/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,23 +49,29 @@
                     "cvode",
                 },
             }
         )
         self._set_child("classes")
         self.classes._set_child(
             "Oper",
-            attribs={"module_name": "snek5000.operators", "class_name": "Operators"},
+            attribs={
+                "module_name": "snek5000.operators",
+                "class_name": "Operators",
+            },
         )
 
 
 class InfoSolverMake(InfoSolverNek):
     """Contain the information on a solver which uses Snakemake."""
 
     def _init_root(self):
         super()._init_root()
         self.classes._set_child(
             "Output",
-            attribs={"module_name": "snek5000.output.base", "class_name": "Output"},
+            attribs={
+                "module_name": "snek5000.output.base",
+                "class_name": "Output",
+            },
         )
         self.classes._set_child(
             "Make", attribs={"module_name": "snek5000.make", "class_name": "Make"}
         )
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/log.py` & `snek5000-0.9.1/src/snek5000/log.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/magic.py` & `snek5000-0.9.1/src/snek5000/magic.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/make.py` & `snek5000-0.9.1/src/snek5000/make.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Snakemake interface
 ======================
 
 """
 import argparse
+import subprocess
 import sys
 from pathlib import Path
 from typing import Iterable
 from warnings import warn
 
 import yaml
 from filelock import FileLock
@@ -25,51 +26,55 @@
 class Make:
     """Snakemake interface for the solvers.
 
     :param sim: A simulation instance
 
     """
 
-    def __init__(self, sim=None, path_run=None):
-
+    def __init__(self, sim=None, path_run=None, snakefile=None):
         if (sim is None and path_run is None) or (
             sim is not None and path_run is not None
         ):
             raise ValueError("Either sim of path_run has to be given.")
 
+        if snakefile:
+            snakefile = Path(snakefile)
+
         if path_run is None:
             self.path_run = sim.output.path_run
             try:
-                self.file = next(
+                self.file = snakefile or next(
                     f for f in sim.output.get_paths() if f.name == "Snakefile"
                 )
             except AttributeError:
                 raise AttributeError("Unable to get path of Snakefile via Output class")
             except StopIteration:
                 raise FileNotFoundError(f"No Snakefile in {self.path_run}")
         else:
             if not path_run.exists():
                 raise FileNotFoundError(f"{path_run} does not exist.")
             self.path_run = Path(path_run)
-            self.file = self.path_run / "Snakefile"
+            self.file = snakefile or self.path_run / "Snakefile"
             if not self.file.exists():
                 raise FileNotFoundError(f"No Snakefile in {path_run}")
 
         self.log_handler = []
 
-    def list(self):
+    def list(self, **kwargs):
         """List rules.
 
         Equivalent to::
 
           snakemake --list-target-rules
 
         """
         with change_dir(self.path_run):
-            return snakemake(self.file, listrules=True, log_handler=self.log_handler)
+            return snakemake(
+                self.file, listrules=True, log_handler=self.log_handler, **kwargs
+            )
 
     def exec(
         self,
         *rules,
         set_resources=None,
         dryrun=False,
         keep_incomplete=True,
@@ -329,7 +334,61 @@
 
     make.exec(
         args.rule,
         dryrun=args.dry_run,
         keep_incomplete=not args.clean_after_fail,
         nproc=args.nproc,
     )
+
+
+def snek_make_nek():
+    """Used for the command snek-make-nek"""
+    parser = argparse.ArgumentParser(
+        prog="snek-make-nek",
+        description="Execute Snakemake rules to build Nek5000 tools and libraries",
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+
+    parser.add_argument(
+        "rule",
+        nargs="?",
+        default=None,
+        help="Snakemake rule to be executed.",
+    )
+    parser.add_argument(
+        "-l",
+        "--list-rules",
+        action="store_true",
+        help="List rules and exit.",
+    )
+    parser.add_argument(
+        "-c",
+        "--clean-git",
+        action="store_true",
+        help="Apply git-clean on Nek5000 repository before building.",
+    )
+
+    args = parser.parse_args()
+
+    # make = Make(path_run=Path(snek5000.get_nek_source_root()), snakefile=snek5000.get_snek_resource("nek5000.smk"))
+    #
+    make = _Nek5000Make()
+
+    from snek5000.output.base import Output
+
+    with Output.find_configfile().open() as fp:
+        config = yaml.safe_load(fp)
+
+    Output.update_snakemake_config(config, "snek-make-nek", env_sensitive=True)
+
+    if args.list_rules:
+        make.list(config=config)
+        sys.exit(0)
+
+    if args.clean_git:
+        with change_dir(snek5000.get_nek_source_root()):
+            subprocess.run(["git", "clean", "-xdf"])
+
+    if args.rule is None:
+        make.build(config)
+    else:
+        make.exec(args.rule, nproc=4, config=config)
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/operators.py` & `snek5000-0.9.1/src/snek5000/operators.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/__init__.py` & `snek5000-0.9.1/src/snek5000/output/__init__.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/base.py` & `snek5000-0.9.1/src/snek5000/output/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,24 @@
             "PhysFields",
             dict(module_name="snek5000.output.phys_fields", class_name="PhysFields"),
         )
 
         classes._set_child(
             "HistoryPoints",
             dict(
-                module_name="snek5000.output.history_points", class_name="HistoryPoints"
+                module_name="snek5000.output.history_points",
+                class_name="HistoryPoints",
+            ),
+        )
+
+        classes._set_child(
+            "RemainingClockTime",
+            dict(
+                module_name="snek5000.output.remaining_clock_time",
+                class_name="RemainingClockTime",
             ),
         )
 
     @classmethod
     def _complete_info_solver(cls, info_solver):
         """Complete the info_solver instance with child class details (module
         and class names).
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/history_points.py` & `snek5000-0.9.1/src/snek5000/output/history_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
                 self._data = pd.concat(
                     [self._data, df_more], ignore_index=True, sort=False
                 )
 
             return self.coords, self._data
 
     def _load_full(self):
-
         with open(self.path_file) as file:
             nb_points = int(file.readline().split(" ", 1)[0])
             coords = np.loadtxt(file, max_rows=nb_points)
             lines = file.readlines()
 
         if coords.ndim == 1:
             coords = coords.reshape((1, coords.size))
@@ -144,15 +143,14 @@
 
         df = self._create_df_from_lines(lines, nb_points)
         self._data = df
 
         return self.coords, df
 
     def _create_df_from_lines(self, lines, nb_points):
-
         columns = ["time", "ux", "uy"]
 
         sim = self.output.sim
         if sim.params.oper.dim == 3:
             columns.append("uz")
 
         columns.append("pressure")
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/phys_fields.py` & `snek5000-0.9.1/src/snek5000/output/phys_fields.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/print_stdout.py` & `snek5000-0.9.1/src/snek5000/output/print_stdout.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/readers/__init__.py` & `snek5000-0.9.1/src/snek5000/output/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/readers/pymech_.py` & `snek5000-0.9.1/src/snek5000/output/readers/pymech_.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/readers/try_paraview_.py` & `snek5000-0.9.1/src/snek5000/output/readers/try_paraview_.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/output/simple_csv.py` & `snek5000-0.9.1/src/snek5000/output/simple_csv.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/params.py` & `snek5000-0.9.1/src/snek5000/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     from snek5000.util.files import _path_try_from_fluidsim_path
 
     path_dir = _path_try_from_fluidsim_path(path_dir)
     short_name = get_solver_short_name(path_dir)
     Simul = import_cls_simul(short_name)
 
     return Simul.load_params_from_file(
-        path_xml=path_dir / "params_simul.xml", path_par=path_dir / f"{short_name}.par"
+        path_xml=path_dir / "params_simul.xml",
+        path_par=path_dir / f"{short_name}.par",
     )
 
 
 class Parameters(_Parameters):
     """Container for reading, modifying and writing :ref:`par files
     <nek:case_files_par>`.
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/SIZE.j2` & `snek5000-0.9.1/src/snek5000/resources/SIZE.j2`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/__init__.py` & `snek5000-0.9.1/src/snek5000/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/box.j2` & `snek5000-0.9.1/src/snek5000/resources/box.j2`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/compile.sh.j2` & `snek5000-0.9.1/src/snek5000/resources/compile.sh.j2`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/compiler.smk` & `snek5000-0.9.1/src/snek5000/resources/compiler.smk`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/internal.smk` & `snek5000-0.9.1/src/snek5000/resources/internal.smk`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/io.smk` & `snek5000-0.9.1/src/snek5000/resources/io.smk`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/makefile_usr.inc.j2` & `snek5000-0.9.1/src/snek5000/resources/makefile_usr.inc.j2`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/resources/nek5000.smk` & `snek5000-0.9.1/src/snek5000/resources/nek5000.smk`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/solvers/__init__.py` & `snek5000-0.9.1/src/snek5000/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/solvers/base.py` & `snek5000-0.9.1/src/snek5000/solvers/base.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/solvers/kth.py` & `snek5000-0.9.1/src/snek5000/solvers/kth.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/__init__.py` & `snek5000-0.9.1/src/snek5000/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/archive.py` & `snek5000-0.9.1/src/snek5000/util/archive.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/console.py` & `snek5000-0.9.1/src/snek5000/util/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from textwrap import dedent
 
 from snek5000.solvers import available_solvers
 
 
 def print_versions():
-
     import pymech
     import snakemake
 
     import fluiddyn
     import fluidsim_core
     import snek5000
```

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/files.py` & `snek5000-0.9.1/src/snek5000/util/files.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/gfortran_log.py` & `snek5000-0.9.1/src/snek5000/util/gfortran_log.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/restart.py` & `snek5000-0.9.1/src/snek5000/util/restart.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000/util/smake.py` & `snek5000-0.9.1/src/snek5000/util/smake.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/src/snek5000.egg-info/PKG-INFO` & `snek5000-0.9.1/src/snek5000.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek5000
-Version: 0.9.0rc3
+Version: 0.9.1
 Summary: Python framework for Nek5000
 Home-page: https://github.com/snek5000/snek5000
 Author: Ashwin Vishnu Mohanan
 Author-email: ashwinvis+gh@protonmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/snek5000/snek5000/issues
 Project-URL: Documentation, https://snek5000.readthedocs.io
@@ -47,15 +47,15 @@
 **Documentation**: <https://snek5000.readthedocs.io/>
 
 Snek5000 is a Python package which allows one to write [Fluidsim] solvers based
 for the simulations on the Fortran [CFD] code [Nek5000]. There are open-source
 solvers (in particular [snek5000-phill], [snek5000-cbox] and [snek5000-tgv])
 and it's not difficult to write your own solver based on your Nek5000 cases (as
 shown in [this
-tutorial](https://snek5000.readthedocs.io/en/latest/packaging.html)).
+tutorial](https://snek5000.readthedocs.io/en/latest/tuto_packaging.html)).
 
 With a Snek5000-Fluidsim solver, it becomes very easy to
 
 - launch/restart simulations with Python scripts and terminal commands,
 - load simulations, read the associated parameters/data and produce nice
   figures/movies.
```

### Comparing `snek5000-0.9.0rc3/src/snek5000.egg-info/SOURCES.txt` & `snek5000-0.9.1/src/snek5000.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 activate.sh
 noxfile.py
 pyproject.toml
 setup.cfg
 .github/CODEOWNERS
 .github/workflows/build.yaml
 .github/workflows/deploy.yaml
+.github/workflows/draft-pdf.yml
 docs/AUTHORS.md
 docs/CHANGELOG.md
 docs/CONTRIBUTING.md
 docs/Doxyfile
 docs/LICENSE
 docs/Makefile
 docs/autosum.rst
@@ -65,16 +66,18 @@
 docs/dev/release.md
 docs/dev/roadmap.rst
 docs/dev/solver.rst
 docs/examples/scripts/simul_cbox_movie.py
 docs/examples/scripts/tuto_cbox.py
 docs/examples/scripts/tuto_phill.py
 docs/examples/scripts/tuto_tgv.py
+docs/examples/snek5000-canonical/.copier-answers.yml
 docs/examples/snek5000-canonical/LICENSE
 docs/examples/snek5000-canonical/README.md
+docs/examples/snek5000-canonical/pyproject.toml
 docs/examples/snek5000-canonical/setup.cfg
 docs/examples/snek5000-canonical/setup.py
 docs/examples/snek5000-canonical/src/snek5000_canonical/Snakefile
 docs/examples/snek5000-canonical/src/snek5000_canonical/__init__.py
 docs/examples/snek5000-canonical/src/snek5000_canonical/canonical.usr.f
 docs/examples/snek5000-canonical/src/snek5000_canonical/output.py
 docs/examples/snek5000-canonical/src/snek5000_canonical/phys_fields.py
@@ -86,27 +89,35 @@
 docs/examples/snek5000-tgv/setup.py
 docs/examples/snek5000-tgv/src/snek5000_tgv/Snakefile
 docs/examples/snek5000-tgv/src/snek5000_tgv/__init__.py
 docs/examples/snek5000-tgv/src/snek5000_tgv/output.py
 docs/examples/snek5000-tgv/src/snek5000_tgv/solver.py
 docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.par.cfg
 docs/examples/snek5000-tgv/src/snek5000_tgv/tgv.usr.f
+docs/how-to/adaptive_time_step.md
 docs/how-to/archive-simulation-data.md
+docs/how-to/config-c-fortran-compilers.md
 docs/how-to/control-fortran-warnings.md
 docs/how-to/export-sans-snek5000.myst.md
 docs/how-to/history_points.md
 docs/how-to/index.md
 docs/how-to/load_plot_log_data.md
 docs/how-to/load_state_stat_files.md
 docs/how-to/read-write-par-files.md
 docs/how-to/rebuild-nek.md
 docs/how-to/restart.myst.md
 docs/how-to/run-background-foreground.md
 docs/how-to/snek-make.myst.md
 docs/how-to/templates.md
+docs/joss_paper/Makefile
+docs/joss_paper/codemeta.json
+docs/joss_paper/generate_metadata.py
+docs/joss_paper/joss-defaults.yaml
+docs/joss_paper/paper.bib
+docs/joss_paper/paper.md
 requirements/README.md
 requirements/default.nix
 requirements/dev.txt
 requirements/docs.txt
 requirements/environment.yaml
 requirements/main.txt
 requirements/tests-editable.txt
```

### Comparing `snek5000-0.9.0rc3/src/snek5000.egg-info/requires.txt` & `snek5000-0.9.1/src/snek5000.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/conftest.py` & `snek5000-0.9.1/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,14 @@
             print(file.read())
         raise RuntimeError("tgv simulation failed")
 
     return sim
 
 
 def create_fake_nek_files(path_dir, name_solver, nb_files=1):
-
     nx = 2
     ny = 4
     nz = 6
     nx_elem = ny_elem = nz_elem = 2
 
     hexa_data = pymech.core.HexaData(
         ndim=3,
```

### Comparing `snek5000-0.9.0rc3/tests/test_archive.py` & `snek5000-0.9.1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_cbox.py` & `snek5000-0.9.1/tests/test_cbox.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_config.py` & `snek5000-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_files.py` & `snek5000-0.9.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_oper/test_box_2d.box` & `snek5000-0.9.1/tests/test_oper/test_box_2d.box`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_oper/test_box_template.box` & `snek5000-0.9.1/tests/test_oper/test_box_template.box`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_oper/test_size_2d.f` & `snek5000-0.9.1/tests/test_oper/test_size_2d.f`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_oper/test_size_template.f` & `snek5000-0.9.1/tests/test_oper/test_size_template.f`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_oper.py` & `snek5000-0.9.1/tests/test_oper.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_params.py` & `snek5000-0.9.1/tests/test_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,14 @@
 
         return sorted(ftext)
 
     assert format_par(par1) == format_par(par2)
 
 
 def test_user_params():
-
     tmp_dir = Path(tempfile.mkdtemp("snek5000", __name__))
 
     def complete_create_default_params(p):
         if hasattr(p.nek.general, "_recorded_user_params"):
             p.nek.general._recorded_user_params.clear()
         p._set_attribs({"prandtl": 0.71, "rayleigh": 1.8e8})
         p._record_nek_user_params({"prandtl": 1, "rayleigh": 2})
```

### Comparing `snek5000-0.9.0rc3/tests/test_resources.py` & `snek5000-0.9.1/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_restart.py` & `snek5000-0.9.1/tests/test_restart.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_restart_command.py` & `snek5000-0.9.1/tests/test_restart_command.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_solver.py` & `snek5000-0.9.1/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `snek5000-0.9.0rc3/tests/test_tuto_packaging.py` & `snek5000-0.9.1/tests/test_tuto_packaging.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,13 +11,15 @@
     for module in tuple(sys.modules):
         if module.startswith("snek5000_canonical"):
             del sys.modules[module]
 
     sim2 = load(sim_canonical.path_run, reader="pymech_avg")
     with pytest.raises(IOError, match="no files to open"):
         sim2.output.phys_fields.plot_mean_vel()
+    with pytest.raises(IOError, match="No file "):
+        sim2.output.remaining_clock_time.load()
 
 
 @pytest.mark.slow
 def test_package_canonical(sim_canonical):
     sim = sim_canonical
     assert sim.make.exec("compile")
```

### Comparing `snek5000-0.9.0rc3/tests/test_util.py` & `snek5000-0.9.1/tests/test_util.py`

 * *Files identical despite different names*

