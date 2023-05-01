# Comparing `tmp/auditwheel-5.3.0.tar.gz` & `tmp/auditwheel-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auditwheel-5.3.0.tar", last modified: Sat Nov 19 11:21:03 2022, max compression
+gzip compressed data, was "auditwheel-5.4.0.tar", last modified: Mon May  1 08:26:39 2023, max compression
```

## Comparing `auditwheel-5.3.0.tar` & `auditwheel-5.4.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.744444 auditwheel-5.3.0/
--rw-r--r--   0 Matt       (501) staff       (20)    16998 2022-11-19 11:17:29.000000 auditwheel-5.3.0/CHANGELOG.md
--rw-r--r--   0 Matt       (501) staff       (20)     4774 2022-10-15 11:29:02.000000 auditwheel-5.3.0/LICENSE
--rw-r--r--   0 Matt       (501) staff       (20)      431 2022-10-22 09:02:02.000000 auditwheel-5.3.0/MANIFEST.in
--rw-r--r--   0 Matt       (501) staff       (20)     7239 2022-11-19 11:21:03.744551 auditwheel-5.3.0/PKG-INFO
--rw-r--r--   0 Matt       (501) staff       (20)     6125 2022-11-12 13:03:26.000000 auditwheel-5.3.0/README.rst
--rw-r--r--   0 Matt       (501) staff       (20)      555 2022-11-12 13:03:26.000000 auditwheel-5.3.0/pyproject.toml
--rw-r--r--   0 Matt       (501) staff       (20)     1386 2022-11-19 11:21:03.745846 auditwheel-5.3.0/setup.cfg
--rwxr-xr-x   0 Matt       (501) staff       (20)      265 2022-11-12 13:03:26.000000 auditwheel-5.3.0/setup.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.500295 auditwheel-5.3.0/src/
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.575577 auditwheel-5.3.0/src/auditwheel/
--rw-r--r--   0 Matt       (501) staff       (20)        0 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)       84 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/__main__.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.579378 auditwheel-5.3.0/src/auditwheel/_vendor/
--rw-r--r--   0 Matt       (501) staff       (20)        0 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/__init__.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.583550 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/
--rw-r--r--   0 Matt       (501) staff       (20)     1125 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/LICENSE.txt
--rw-r--r--   0 Matt       (501) staff       (20)       23 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/__init__.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.587266 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/
--rw-r--r--   0 Matt       (501) staff       (20)     2572 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)     9498 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/convert.py
--rw-r--r--   0 Matt       (501) staff       (20)     3196 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/pack.py
--rw-r--r--   0 Matt       (501) staff       (20)      673 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/unpack.py
--rw-r--r--   0 Matt       (501) staff       (20)     1257 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/pkginfo.py
--rw-r--r--   0 Matt       (501) staff       (20)      938 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/util.py
--rw-r--r--   0 Matt       (501) staff       (20)     7326 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/_vendor/wheel/wheelfile.py
--rw-r--r--   0 Matt       (501) staff       (20)     1107 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/condatools.py
--rw-r--r--   0 Matt       (501) staff       (20)     4990 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/elfutils.py
--rw-r--r--   0 Matt       (501) staff       (20)       98 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/error.py
--rw-r--r--   0 Matt       (501) staff       (20)      676 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/genericpkgctx.py
--rw-r--r--   0 Matt       (501) staff       (20)      349 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/hashfile.py
--rw-r--r--   0 Matt       (501) staff       (20)    14346 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/lddtree.py
--rw-r--r--   0 Matt       (501) staff       (20)      431 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/libc.py
--rw-r--r--   0 Matt       (501) staff       (20)     1604 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/main.py
--rw-r--r--   0 Matt       (501) staff       (20)     2051 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/main_addtag.py
--rw-r--r--   0 Matt       (501) staff       (20)      443 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/main_lddtree.py
--rw-r--r--   0 Matt       (501) staff       (20)     5899 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/main_repair.py
--rw-r--r--   0 Matt       (501) staff       (20)     4414 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/main_show.py
--rw-r--r--   0 Matt       (501) staff       (20)     1069 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/musllinux.py
--rw-r--r--   0 Matt       (501) staff       (20)     2357 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/patcher.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.593445 auditwheel-5.3.0/src/auditwheel/policy/
--rw-r--r--   0 Matt       (501) staff       (20)     6348 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/policy/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)     3147 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/policy/external_references.py
--rw-r--r--   0 Matt       (501) staff       (20)    53261 2022-11-19 09:57:11.000000 auditwheel-5.3.0/src/auditwheel/policy/manylinux-policy.json
--rw-r--r--   0 Matt       (501) staff       (20)     1862 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/policy/musllinux-policy.json
--rw-r--r--   0 Matt       (501) staff       (20)     1706 2022-10-15 11:29:02.000000 auditwheel-5.3.0/src/auditwheel/policy/policy-schema.json
--rw-r--r--   0 Matt       (501) staff       (20)     1698 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/policy/versioned_symbols.py
--rw-r--r--   0 Matt       (501) staff       (20)     7989 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/repair.py
--rw-r--r--   0 Matt       (501) staff       (20)     3000 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/tmpdirs.py
--rw-r--r--   0 Matt       (501) staff       (20)     4512 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/tools.py
--rw-r--r--   0 Matt       (501) staff       (20)    10995 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/wheel_abi.py
--rw-r--r--   0 Matt       (501) staff       (20)     9516 2022-11-12 13:03:26.000000 auditwheel-5.3.0/src/auditwheel/wheeltools.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.579168 auditwheel-5.3.0/src/auditwheel.egg-info/
--rw-r--r--   0 Matt       (501) staff       (20)     7239 2022-11-19 11:21:03.000000 auditwheel-5.3.0/src/auditwheel.egg-info/PKG-INFO
--rw-r--r--   0 Matt       (501) staff       (20)     4964 2022-11-19 11:21:03.000000 auditwheel-5.3.0/src/auditwheel.egg-info/SOURCES.txt
--rw-r--r--   0 Matt       (501) staff       (20)        1 2022-11-19 11:21:03.000000 auditwheel-5.3.0/src/auditwheel.egg-info/dependency_links.txt
--rw-r--r--   0 Matt       (501) staff       (20)       52 2022-11-19 11:21:03.000000 auditwheel-5.3.0/src/auditwheel.egg-info/entry_points.txt
--rw-r--r--   0 Matt       (501) staff       (20)        1 2022-01-03 13:37:36.000000 auditwheel-5.3.0/src/auditwheel.egg-info/not-zip-safe
--rw-r--r--   0 Matt       (501) staff       (20)      263 2022-11-19 11:21:03.000000 auditwheel-5.3.0/src/auditwheel.egg-info/requires.txt
--rw-r--r--   0 Matt       (501) staff       (20)       11 2022-11-19 11:21:03.000000 auditwheel-5.3.0/src/auditwheel.egg-info/top_level.txt
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.506691 auditwheel-5.3.0/tests/
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.613129 auditwheel-5.3.0/tests/integration/
--rw-r--r--   0 Matt       (501) staff       (20)   326432 2019-09-28 14:21:15.000000 auditwheel-5.3.0/tests/integration/cffi-1.5.0-cp27-none-linux_x86_64.whl
--rw-r--r--   0 Matt       (501) staff       (20)       42 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/conftest.py
--rw-r--r--   0 Matt       (501) staff       (20)      345 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/foo.f90
--rw-r--r--   0 Matt       (501) staff       (20)    14180 2019-09-28 14:21:15.000000 auditwheel-5.3.0/tests/integration/fpewheel-0.0.0-cp35-cp35m-linux_x86_64.whl
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.617992 auditwheel-5.3.0/tests/integration/internal_rpath/
--rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/MANIFEST.in
--rw-r--r--   0 Matt       (501) staff       (20)      289 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/internal_rpath/Makefile
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.618580 auditwheel-5.3.0/tests/integration/internal_rpath/internal_rpath/
--rw-r--r--   0 Matt       (501) staff       (20)        0 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/internal_rpath/__init__.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.502147 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.619868 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/a/
--rw-r--r--   0 Matt       (501) staff       (20)       32 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/a/a.c
--rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/a/a.h
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.621476 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/b/
--rw-r--r--   0 Matt       (501) staff       (20)       32 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/b/b.c
--rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/lib-src/b/b.h
--rw-r--r--   0 Matt       (501) staff       (20)      100 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/pyproject.toml
--rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/internal_rpath/setup.cfg
--rw-r--r--   0 Matt       (501) staff       (20)      791 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/internal_rpath/setup.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.622846 auditwheel-5.3.0/tests/integration/internal_rpath/src/
--rw-r--r--   0 Matt       (501) staff       (20)       79 2022-10-15 13:09:48.000000 auditwheel-5.3.0/tests/integration/internal_rpath/src/example_a.pyx
--rw-r--r--   0 Matt       (501) staff       (20)       79 2022-10-15 13:09:48.000000 auditwheel-5.3.0/tests/integration/internal_rpath/src/example_b.pyx
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.626538 auditwheel-5.3.0/tests/integration/multiple_top_level/
--rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/MANIFEST.in
--rw-r--r--   0 Matt       (501) staff       (20)      335 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/Makefile
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.504190 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.628277 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/a/
--rw-r--r--   0 Matt       (501) staff       (20)       55 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/a/a.c
--rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/a/a.h
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.633278 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/b/
--rw-r--r--   0 Matt       (501) staff       (20)       32 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/b/b.c
--rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/lib-src/b/b.h
--rw-r--r--   0 Matt       (501) staff       (20)      100 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/pyproject.toml
--rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/setup.cfg
--rw-r--r--   0 Matt       (501) staff       (20)      673 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/setup.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.634664 auditwheel-5.3.0/tests/integration/multiple_top_level/src/
--rw-r--r--   0 Matt       (501) staff       (20)       79 2022-10-15 13:09:48.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/src/example_a.pyx
--rw-r--r--   0 Matt       (501) staff       (20)       84 2022-10-15 13:09:48.000000 auditwheel-5.3.0/tests/integration/multiple_top_level/src/example_b.pyx
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.673603 auditwheel-5.3.0/tests/integration/nonpy_rpath/
--rw-r--r--   0 Matt       (501) staff       (20)      605 2021-03-19 07:24:41.000000 auditwheel-5.3.0/tests/integration/nonpy_rpath/README.md
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.675102 auditwheel-5.3.0/tests/integration/nonpy_rpath/extensions/
--rw-r--r--   0 Matt       (501) staff       (20)      230 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/nonpy_rpath/extensions/testcrypt.cpp
--rw-r--r--   0 Matt       (501) staff       (20)       67 2021-03-19 07:24:41.000000 auditwheel-5.3.0/tests/integration/nonpy_rpath/extensions/testcrypt.h
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.688006 auditwheel-5.3.0/tests/integration/nonpy_rpath/nonpy_rpath/
--rw-r--r--   0 Matt       (501) staff       (20)       73 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/nonpy_rpath/nonpy_rpath/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)      699 2021-03-19 07:24:41.000000 auditwheel-5.3.0/tests/integration/nonpy_rpath/nonpy_rpath.cpp
--rw-r--r--   0 Matt       (501) staff       (20)     2560 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/nonpy_rpath/setup.py
--rw-r--r--   0 Matt       (501) staff       (20)   115068 2020-11-07 17:54:50.000000 auditwheel-5.3.0/tests/integration/plumbum-1.6.8-py2.py3-none-any.whl
--rw-r--r--   0 Matt       (501) staff       (20)    18874 2019-09-28 14:21:15.000000 auditwheel-5.3.0/tests/integration/python_snappy-0.5.2-pp260-pypy_41-linux_x86_64.whl
--rw-r--r--   0 Matt       (501) staff       (20)      298 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/quick_check_numpy.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.694744 auditwheel-5.3.0/tests/integration/sample_extension/
--rw-r--r--   0 Matt       (501) staff       (20)      101 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/sample_extension/pyproject.toml
--rw-r--r--   0 Matt       (501) staff       (20)      179 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/sample_extension/setup.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.696282 auditwheel-5.3.0/tests/integration/sample_extension/src/
--rw-r--r--   0 Matt       (501) staff       (20)       81 2022-10-15 13:09:48.000000 auditwheel-5.3.0/tests/integration/sample_extension/src/sample_extension.pyx
--rw-r--r--   0 Matt       (501) staff       (20)      389 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/test_addtag.py
--rw-r--r--   0 Matt       (501) staff       (20)     2788 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/test_bundled_wheels.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.698599 auditwheel-5.3.0/tests/integration/test_glibcxx_3_4_25/
--rw-r--r--   0 Matt       (501) staff       (20)      293 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/test_glibcxx_3_4_25/setup.py
--rw-r--r--   0 Matt       (501) staff       (20)      636 2022-10-15 11:30:21.000000 auditwheel-5.3.0/tests/integration/test_glibcxx_3_4_25/testentropy.cpp
--rw-r--r--   0 Matt       (501) staff       (20)    39275 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/test_manylinux.py
--rw-r--r--   0 Matt       (501) staff       (20)      547 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/test_nonplatform_wheel.py
--rw-r--r--   0 Matt       (501) staff       (20)      840 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/test_policy_files.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.718863 auditwheel-5.3.0/tests/integration/testdependencies/
--rw-r--r--   0 Matt       (501) staff       (20)      646 2022-10-15 11:30:21.000000 auditwheel-5.3.0/tests/integration/testdependencies/dependency.c
--rw-r--r--   0 Matt       (501) staff       (20)       19 2019-09-28 14:21:15.000000 auditwheel-5.3.0/tests/integration/testdependencies/dependency.h
--rw-r--r--   0 Matt       (501) staff       (20)      802 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/testdependencies/setup.py
--rw-r--r--   0 Matt       (501) staff       (20)     1553 2022-10-15 11:30:21.000000 auditwheel-5.3.0/tests/integration/testdependencies/testdependencies.c
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.719760 auditwheel-5.3.0/tests/integration/testpackage/
--rw-r--r--   0 Matt       (501) staff       (20)        0 2019-09-28 14:21:15.000000 auditwheel-5.3.0/tests/integration/testpackage/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)      302 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/testpackage/setup.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.725844 auditwheel-5.3.0/tests/integration/testpackage/testpackage/
--rw-r--r--   0 Matt       (501) staff       (20)      210 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/testpackage/testpackage/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)      632 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/testpackage/testpackage/testprogram.c
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.727442 auditwheel-5.3.0/tests/integration/testrpath/
--rw-r--r--   0 Matt       (501) staff       (20)       16 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/MANIFEST.in
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.729003 auditwheel-5.3.0/tests/integration/testrpath/a/
--rw-r--r--   0 Matt       (501) staff       (20)       55 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/a/a.c
--rw-r--r--   0 Matt       (501) staff       (20)       14 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/a/a.h
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.730313 auditwheel-5.3.0/tests/integration/testrpath/b/
--rw-r--r--   0 Matt       (501) staff       (20)       32 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/b/b.c
--rw-r--r--   0 Matt       (501) staff       (20)       14 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/b/b.h
--rw-r--r--   0 Matt       (501) staff       (20)      787 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/testrpath/setup.py
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.506299 auditwheel-5.3.0/tests/integration/testrpath/src/
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.731170 auditwheel-5.3.0/tests/integration/testrpath/src/testrpath/
--rw-r--r--   0 Matt       (501) staff       (20)        0 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/src/testrpath/__init__.py
--rw-r--r--   0 Matt       (501) staff       (20)      610 2019-10-12 11:03:05.000000 auditwheel-5.3.0/tests/integration/testrpath/src/testrpath/testrpath.c
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.732525 auditwheel-5.3.0/tests/integration/testsimple/
--rw-r--r--   0 Matt       (501) staff       (20)      163 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/testsimple/setup.py
--rw-r--r--   0 Matt       (501) staff       (20)      561 2021-03-19 07:24:10.000000 auditwheel-5.3.0/tests/integration/testsimple/testsimple.c
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.733957 auditwheel-5.3.0/tests/integration/testzlib/
--rw-r--r--   0 Matt       (501) staff       (20)      344 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/integration/testzlib/setup.py
--rw-r--r--   0 Matt       (501) staff       (20)      984 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/integration/testzlib/testzlib.c
-drwxr-xr-x   0 Matt       (501) staff       (20)        0 2022-11-19 11:21:03.744307 auditwheel-5.3.0/tests/unit/
--rw-r--r--   0 Matt       (501) staff       (20)     8236 2022-10-15 11:29:02.000000 auditwheel-5.3.0/tests/unit/test-permissions.zip.xz
--rw-r--r--   0 Matt       (501) staff       (20)      842 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_condatools.py
--rw-r--r--   0 Matt       (501) staff       (20)     3486 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_elfpatcher.py
--rw-r--r--   0 Matt       (501) staff       (20)     5525 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_elfutils.py
--rw-r--r--   0 Matt       (501) staff       (20)      289 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_hashfile.py
--rw-r--r--   0 Matt       (501) staff       (20)      662 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_main.py
--rw-r--r--   0 Matt       (501) staff       (20)     1295 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_musllinux.py
--rw-r--r--   0 Matt       (501) staff       (20)     6271 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_policy.py
--rw-r--r--   0 Matt       (501) staff       (20)     4652 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_repair.py
--rw-r--r--   0 Matt       (501) staff       (20)     1349 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_tmpdirs.py
--rw-r--r--   0 Matt       (501) staff       (20)     3217 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_tools.py
--rw-r--r--   0 Matt       (501) staff       (20)     1768 2022-11-12 13:03:26.000000 auditwheel-5.3.0/tests/unit/test_wheel_abi.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.207026 auditwheel-5.4.0/
+-rw-r--r--   0 Matt       (501) staff       (20)    17551 2023-05-01 08:23:11.000000 auditwheel-5.4.0/CHANGELOG.md
+-rw-r--r--   0 Matt       (501) staff       (20)     4774 2022-10-15 11:29:02.000000 auditwheel-5.4.0/LICENSE
+-rw-r--r--   0 Matt       (501) staff       (20)      431 2022-10-22 09:02:02.000000 auditwheel-5.4.0/MANIFEST.in
+-rw-r--r--   0 Matt       (501) staff       (20)     7189 2023-05-01 08:26:39.207134 auditwheel-5.4.0/PKG-INFO
+-rw-r--r--   0 Matt       (501) staff       (20)     6074 2023-05-01 08:24:42.000000 auditwheel-5.4.0/README.rst
+-rw-r--r--   0 Matt       (501) staff       (20)      581 2023-04-10 17:25:28.000000 auditwheel-5.4.0/pyproject.toml
+-rw-r--r--   0 Matt       (501) staff       (20)     1387 2023-05-01 08:26:39.207983 auditwheel-5.4.0/setup.cfg
+-rwxr-xr-x   0 Matt       (501) staff       (20)      301 2023-03-05 10:07:34.000000 auditwheel-5.4.0/setup.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.105537 auditwheel-5.4.0/src/
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.119196 auditwheel-5.4.0/src/auditwheel/
+-rw-r--r--   0 Matt       (501) staff       (20)        0 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)      120 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/__main__.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.147852 auditwheel-5.4.0/src/auditwheel/_vendor/
+-rw-r--r--   0 Matt       (501) staff       (20)        0 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/__init__.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.149264 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/
+-rw-r--r--   0 Matt       (501) staff       (20)     1125 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0 Matt       (501) staff       (20)       23 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/__init__.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.149950 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/
+-rw-r--r--   0 Matt       (501) staff       (20)     2572 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)     9498 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/convert.py
+-rw-r--r--   0 Matt       (501) staff       (20)     3196 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/pack.py
+-rw-r--r--   0 Matt       (501) staff       (20)      673 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1257 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/pkginfo.py
+-rw-r--r--   0 Matt       (501) staff       (20)      938 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/util.py
+-rw-r--r--   0 Matt       (501) staff       (20)     7326 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/_vendor/wheel/wheelfile.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1106 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/condatools.py
+-rw-r--r--   0 Matt       (501) staff       (20)     4979 2023-04-10 17:25:28.000000 auditwheel-5.4.0/src/auditwheel/elfutils.py
+-rw-r--r--   0 Matt       (501) staff       (20)      135 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/error.py
+-rw-r--r--   0 Matt       (501) staff       (20)      667 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/genericpkgctx.py
+-rw-r--r--   0 Matt       (501) staff       (20)      385 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/hashfile.py
+-rw-r--r--   0 Matt       (501) staff       (20)    14266 2023-04-10 17:25:28.000000 auditwheel-5.4.0/src/auditwheel/lddtree.py
+-rw-r--r--   0 Matt       (501) staff       (20)      467 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/libc.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1608 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/main.py
+-rw-r--r--   0 Matt       (501) staff       (20)     2087 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/main_addtag.py
+-rw-r--r--   0 Matt       (501) staff       (20)      479 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/main_lddtree.py
+-rw-r--r--   0 Matt       (501) staff       (20)     5935 2023-03-05 08:21:51.000000 auditwheel-5.4.0/src/auditwheel/main_repair.py
+-rw-r--r--   0 Matt       (501) staff       (20)     4450 2023-03-05 08:21:51.000000 auditwheel-5.4.0/src/auditwheel/main_show.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1105 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/musllinux.py
+-rw-r--r--   0 Matt       (501) staff       (20)     2366 2023-04-10 17:25:28.000000 auditwheel-5.4.0/src/auditwheel/patcher.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.150904 auditwheel-5.4.0/src/auditwheel/policy/
+-rw-r--r--   0 Matt       (501) staff       (20)     6559 2023-05-01 08:14:13.000000 auditwheel-5.4.0/src/auditwheel/policy/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)     3158 2023-05-01 08:14:13.000000 auditwheel-5.4.0/src/auditwheel/policy/external_references.py
+-rw-r--r--   0 Matt       (501) staff       (20)    53261 2022-11-19 13:31:45.000000 auditwheel-5.4.0/src/auditwheel/policy/manylinux-policy.json
+-rw-r--r--   0 Matt       (501) staff       (20)     1862 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/policy/musllinux-policy.json
+-rw-r--r--   0 Matt       (501) staff       (20)     1706 2022-10-15 11:29:02.000000 auditwheel-5.4.0/src/auditwheel/policy/policy-schema.json
+-rw-r--r--   0 Matt       (501) staff       (20)     1683 2023-04-10 17:25:28.000000 auditwheel-5.4.0/src/auditwheel/policy/versioned_symbols.py
+-rw-r--r--   0 Matt       (501) staff       (20)     7967 2023-04-10 17:25:28.000000 auditwheel-5.4.0/src/auditwheel/repair.py
+-rw-r--r--   0 Matt       (501) staff       (20)     2981 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/tmpdirs.py
+-rw-r--r--   0 Matt       (501) staff       (20)     4529 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/tools.py
+-rw-r--r--   0 Matt       (501) staff       (20)    10994 2023-04-10 17:25:28.000000 auditwheel-5.4.0/src/auditwheel/wheel_abi.py
+-rw-r--r--   0 Matt       (501) staff       (20)     9515 2022-11-19 13:30:29.000000 auditwheel-5.4.0/src/auditwheel/wheeltools.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.147668 auditwheel-5.4.0/src/auditwheel.egg-info/
+-rw-r--r--   0 Matt       (501) staff       (20)     7189 2023-05-01 08:26:38.000000 auditwheel-5.4.0/src/auditwheel.egg-info/PKG-INFO
+-rw-r--r--   0 Matt       (501) staff       (20)     4964 2023-05-01 08:26:39.000000 auditwheel-5.4.0/src/auditwheel.egg-info/SOURCES.txt
+-rw-r--r--   0 Matt       (501) staff       (20)        1 2023-05-01 08:26:38.000000 auditwheel-5.4.0/src/auditwheel.egg-info/dependency_links.txt
+-rw-r--r--   0 Matt       (501) staff       (20)       52 2023-05-01 08:26:38.000000 auditwheel-5.4.0/src/auditwheel.egg-info/entry_points.txt
+-rw-r--r--   0 Matt       (501) staff       (20)        1 2022-01-03 13:37:36.000000 auditwheel-5.4.0/src/auditwheel.egg-info/not-zip-safe
+-rw-r--r--   0 Matt       (501) staff       (20)      263 2023-05-01 08:26:38.000000 auditwheel-5.4.0/src/auditwheel.egg-info/requires.txt
+-rw-r--r--   0 Matt       (501) staff       (20)       11 2023-05-01 08:26:38.000000 auditwheel-5.4.0/src/auditwheel.egg-info/top_level.txt
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.114202 auditwheel-5.4.0/tests/
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.176013 auditwheel-5.4.0/tests/integration/
+-rw-r--r--   0 Matt       (501) staff       (20)   326432 2019-09-28 14:21:15.000000 auditwheel-5.4.0/tests/integration/cffi-1.5.0-cp27-none-linux_x86_64.whl
+-rw-r--r--   0 Matt       (501) staff       (20)       78 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/conftest.py
+-rw-r--r--   0 Matt       (501) staff       (20)      345 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/foo.f90
+-rw-r--r--   0 Matt       (501) staff       (20)    14180 2019-09-28 14:21:15.000000 auditwheel-5.4.0/tests/integration/fpewheel-0.0.0-cp35-cp35m-linux_x86_64.whl
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.182681 auditwheel-5.4.0/tests/integration/internal_rpath/
+-rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/MANIFEST.in
+-rw-r--r--   0 Matt       (501) staff       (20)      289 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/internal_rpath/Makefile
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.182895 auditwheel-5.4.0/tests/integration/internal_rpath/internal_rpath/
+-rw-r--r--   0 Matt       (501) staff       (20)        0 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/internal_rpath/__init__.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.107278 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.185522 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/a/
+-rw-r--r--   0 Matt       (501) staff       (20)       32 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/a/a.c
+-rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/a/a.h
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.186958 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/b/
+-rw-r--r--   0 Matt       (501) staff       (20)       32 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/b/b.c
+-rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/lib-src/b/b.h
+-rw-r--r--   0 Matt       (501) staff       (20)      100 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/pyproject.toml
+-rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/internal_rpath/setup.cfg
+-rw-r--r--   0 Matt       (501) staff       (20)      827 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/internal_rpath/setup.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.194904 auditwheel-5.4.0/tests/integration/internal_rpath/src/
+-rw-r--r--   0 Matt       (501) staff       (20)       79 2022-10-15 13:09:48.000000 auditwheel-5.4.0/tests/integration/internal_rpath/src/example_a.pyx
+-rw-r--r--   0 Matt       (501) staff       (20)       79 2022-10-15 13:09:48.000000 auditwheel-5.4.0/tests/integration/internal_rpath/src/example_b.pyx
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.197183 auditwheel-5.4.0/tests/integration/multiple_top_level/
+-rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/MANIFEST.in
+-rw-r--r--   0 Matt       (501) staff       (20)      335 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/Makefile
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.108557 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.197494 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/a/
+-rw-r--r--   0 Matt       (501) staff       (20)       55 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/a/a.c
+-rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/a/a.h
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.197806 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/b/
+-rw-r--r--   0 Matt       (501) staff       (20)       32 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/b/b.c
+-rw-r--r--   0 Matt       (501) staff       (20)       14 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/lib-src/b/b.h
+-rw-r--r--   0 Matt       (501) staff       (20)      100 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/pyproject.toml
+-rw-r--r--   0 Matt       (501) staff       (20)       33 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/setup.cfg
+-rw-r--r--   0 Matt       (501) staff       (20)      709 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/setup.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.198096 auditwheel-5.4.0/tests/integration/multiple_top_level/src/
+-rw-r--r--   0 Matt       (501) staff       (20)       79 2022-10-15 13:09:48.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/src/example_a.pyx
+-rw-r--r--   0 Matt       (501) staff       (20)       84 2022-10-15 13:09:48.000000 auditwheel-5.4.0/tests/integration/multiple_top_level/src/example_b.pyx
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.198576 auditwheel-5.4.0/tests/integration/nonpy_rpath/
+-rw-r--r--   0 Matt       (501) staff       (20)      605 2021-03-19 07:24:41.000000 auditwheel-5.4.0/tests/integration/nonpy_rpath/README.md
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.198895 auditwheel-5.4.0/tests/integration/nonpy_rpath/extensions/
+-rw-r--r--   0 Matt       (501) staff       (20)      230 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/nonpy_rpath/extensions/testcrypt.cpp
+-rw-r--r--   0 Matt       (501) staff       (20)       67 2021-03-19 07:24:41.000000 auditwheel-5.4.0/tests/integration/nonpy_rpath/extensions/testcrypt.h
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.199066 auditwheel-5.4.0/tests/integration/nonpy_rpath/nonpy_rpath/
+-rw-r--r--   0 Matt       (501) staff       (20)      109 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/nonpy_rpath/nonpy_rpath/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)      699 2021-03-19 07:24:41.000000 auditwheel-5.4.0/tests/integration/nonpy_rpath/nonpy_rpath.cpp
+-rw-r--r--   0 Matt       (501) staff       (20)     2596 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/nonpy_rpath/setup.py
+-rw-r--r--   0 Matt       (501) staff       (20)   115068 2020-11-07 17:54:50.000000 auditwheel-5.4.0/tests/integration/plumbum-1.6.8-py2.py3-none-any.whl
+-rw-r--r--   0 Matt       (501) staff       (20)    18874 2019-09-28 14:21:15.000000 auditwheel-5.4.0/tests/integration/python_snappy-0.5.2-pp260-pypy_41-linux_x86_64.whl
+-rw-r--r--   0 Matt       (501) staff       (20)      334 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/quick_check_numpy.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.199359 auditwheel-5.4.0/tests/integration/sample_extension/
+-rw-r--r--   0 Matt       (501) staff       (20)      101 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/sample_extension/pyproject.toml
+-rw-r--r--   0 Matt       (501) staff       (20)      215 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/sample_extension/setup.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.199513 auditwheel-5.4.0/tests/integration/sample_extension/src/
+-rw-r--r--   0 Matt       (501) staff       (20)       81 2022-10-15 13:09:48.000000 auditwheel-5.4.0/tests/integration/sample_extension/src/sample_extension.pyx
+-rw-r--r--   0 Matt       (501) staff       (20)      425 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/test_addtag.py
+-rw-r--r--   0 Matt       (501) staff       (20)     2824 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/test_bundled_wheels.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.199808 auditwheel-5.4.0/tests/integration/test_glibcxx_3_4_25/
+-rw-r--r--   0 Matt       (501) staff       (20)      329 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/test_glibcxx_3_4_25/setup.py
+-rw-r--r--   0 Matt       (501) staff       (20)      636 2022-10-15 11:30:21.000000 auditwheel-5.4.0/tests/integration/test_glibcxx_3_4_25/testentropy.cpp
+-rw-r--r--   0 Matt       (501) staff       (20)    38712 2023-05-01 08:14:13.000000 auditwheel-5.4.0/tests/integration/test_manylinux.py
+-rw-r--r--   0 Matt       (501) staff       (20)      569 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/test_nonplatform_wheel.py
+-rw-r--r--   0 Matt       (501) staff       (20)      876 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/test_policy_files.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.200390 auditwheel-5.4.0/tests/integration/testdependencies/
+-rw-r--r--   0 Matt       (501) staff       (20)      646 2022-10-15 11:30:21.000000 auditwheel-5.4.0/tests/integration/testdependencies/dependency.c
+-rw-r--r--   0 Matt       (501) staff       (20)       19 2019-09-28 14:21:15.000000 auditwheel-5.4.0/tests/integration/testdependencies/dependency.h
+-rw-r--r--   0 Matt       (501) staff       (20)      838 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/testdependencies/setup.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1553 2022-10-15 11:30:21.000000 auditwheel-5.4.0/tests/integration/testdependencies/testdependencies.c
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.200689 auditwheel-5.4.0/tests/integration/testpackage/
+-rw-r--r--   0 Matt       (501) staff       (20)        0 2019-09-28 14:21:15.000000 auditwheel-5.4.0/tests/integration/testpackage/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)      338 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/testpackage/setup.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.201033 auditwheel-5.4.0/tests/integration/testpackage/testpackage/
+-rw-r--r--   0 Matt       (501) staff       (20)      246 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/testpackage/testpackage/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)      632 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/testpackage/testpackage/testprogram.c
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.201356 auditwheel-5.4.0/tests/integration/testrpath/
+-rw-r--r--   0 Matt       (501) staff       (20)       16 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/MANIFEST.in
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.201687 auditwheel-5.4.0/tests/integration/testrpath/a/
+-rw-r--r--   0 Matt       (501) staff       (20)       55 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/a/a.c
+-rw-r--r--   0 Matt       (501) staff       (20)       14 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/a/a.h
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.201966 auditwheel-5.4.0/tests/integration/testrpath/b/
+-rw-r--r--   0 Matt       (501) staff       (20)       32 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/b/b.c
+-rw-r--r--   0 Matt       (501) staff       (20)       14 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/b/b.h
+-rw-r--r--   0 Matt       (501) staff       (20)      823 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/testrpath/setup.py
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.113473 auditwheel-5.4.0/tests/integration/testrpath/src/
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.202274 auditwheel-5.4.0/tests/integration/testrpath/src/testrpath/
+-rw-r--r--   0 Matt       (501) staff       (20)        0 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/src/testrpath/__init__.py
+-rw-r--r--   0 Matt       (501) staff       (20)      610 2019-10-12 11:03:05.000000 auditwheel-5.4.0/tests/integration/testrpath/src/testrpath/testrpath.c
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.202633 auditwheel-5.4.0/tests/integration/testsimple/
+-rw-r--r--   0 Matt       (501) staff       (20)      199 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/testsimple/setup.py
+-rw-r--r--   0 Matt       (501) staff       (20)      561 2021-03-19 07:24:10.000000 auditwheel-5.4.0/tests/integration/testsimple/testsimple.c
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.202976 auditwheel-5.4.0/tests/integration/testzlib/
+-rw-r--r--   0 Matt       (501) staff       (20)      380 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/integration/testzlib/setup.py
+-rw-r--r--   0 Matt       (501) staff       (20)      984 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/integration/testzlib/testzlib.c
+drwxr-xr-x   0 Matt       (501) staff       (20)        0 2023-05-01 08:26:39.206913 auditwheel-5.4.0/tests/unit/
+-rw-r--r--   0 Matt       (501) staff       (20)     8236 2022-10-15 11:29:02.000000 auditwheel-5.4.0/tests/unit/test-permissions.zip.xz
+-rw-r--r--   0 Matt       (501) staff       (20)      878 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_condatools.py
+-rw-r--r--   0 Matt       (501) staff       (20)     3522 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_elfpatcher.py
+-rw-r--r--   0 Matt       (501) staff       (20)     5561 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_elfutils.py
+-rw-r--r--   0 Matt       (501) staff       (20)      325 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_hashfile.py
+-rw-r--r--   0 Matt       (501) staff       (20)      698 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_main.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1331 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_musllinux.py
+-rw-r--r--   0 Matt       (501) staff       (20)     7477 2023-05-01 08:14:13.000000 auditwheel-5.4.0/tests/unit/test_policy.py
+-rw-r--r--   0 Matt       (501) staff       (20)     4688 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_repair.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1385 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_tmpdirs.py
+-rw-r--r--   0 Matt       (501) staff       (20)     3253 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_tools.py
+-rw-r--r--   0 Matt       (501) staff       (20)     1804 2022-11-19 13:30:29.000000 auditwheel-5.4.0/tests/unit/test_wheel_abi.py
```

### Comparing `auditwheel-5.3.0/CHANGELOG.md` & `auditwheel-5.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # auditwheel changelog
 
 ## HEAD
 
+## 5.4.0
+
+Released May 1, 2023
+
+### User-facing changes
+- [FEATURE] Add python 3.11 support ([#407](https://github.com/pypa/auditwheel/pull/407))
+- [FEATURE] Drop python 3.6 support ([#400](https://github.com/pypa/auditwheel/pull/400))
+- [FEATURE] Use armv7l policy for 64-bit arm kernel in 32-bit mode (armv8l), BETA feature ([#419](https://github.com/pypa/auditwheel/pull/419))
+- [BUGFIX] Filter libpythonXY with X/Y more than single digits ([#424](https://github.com/pypa/auditwheel/pull/424), [#418](https://github.com/pypa/auditwheel/issues/418))
+
 ## 5.3.0
 
 Released Nov. 19, 2022
 
 ### User-facing changes
 - [FEATURE] Add `manylinux_2_34` & `manylinux_2_35` policies ([#405](https://github.com/pypa/auditwheel/pull/405), [#388](https://github.com/pypa/auditwheel/issues/388))
```

### Comparing `auditwheel-5.3.0/LICENSE` & `auditwheel-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/PKG-INFO` & `auditwheel-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: auditwheel
-Version: 5.3.0
+Version: 5.4.0
 Summary: Cross-distribution Linux wheels
 Home-page: https://github.com/pypa/auditwheel
 Author: Robert T. McGibbon
 Author-email: rmcgibbo@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: coverage
 Provides-Extra: develop
 License-File: LICENSE
 
 auditwheel
@@ -66,15 +66,15 @@
 will be picked up at runtime. This accomplishes a similar result as if the libraries had
 been statically linked without requiring changes to the build system. Packagers are
 advised that bundling, like static linking, may implicate copyright concerns.
 
 Requirements
 ------------
 - OS: Linux
-- Python: 3.6+
+- Python: 3.7+
 - `patchelf <https://github.com/NixOS/patchelf>`_: 0.14+
 
 Only systems that use `ELF
 <https://en.wikipedia.org/wiki/Executable_and_Linkable_Format>`_-based linkage
 are supported (this should be essentially every Linux).
 
 In general, building ``manylinux1`` wheels requires running on a CentOS5
@@ -161,19 +161,18 @@
 test dependencies.
 
 Some of the integration tests also require a running and accessible Docker
 daemon. These tests will pull a number of docker images if they are not already
 available on your system, but it won't update existing images.
 To update these images manually, run::
 
-    docker pull python:3.6-slim
+    docker pull python:3.7-slim
     docker pull quay.io/pypa/manylinux1_x86_64
     docker pull quay.io/pypa/manylinux2010_x86_64
     docker pull quay.io/pypa/manylinux2014_x86_64
-    docker pull quay.io/pypa/manylinux_2_24_x86_64
     docker pull quay.io/pypa/manylinux_2_28_x86_64
 
 You may also remove these images using ``docker rmi``.
 
 Code of Conduct
 ---------------
```

### Comparing `auditwheel-5.3.0/README.rst` & `auditwheel-5.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 will be picked up at runtime. This accomplishes a similar result as if the libraries had
 been statically linked without requiring changes to the build system. Packagers are
 advised that bundling, like static linking, may implicate copyright concerns.
 
 Requirements
 ------------
 - OS: Linux
-- Python: 3.6+
+- Python: 3.7+
 - `patchelf <https://github.com/NixOS/patchelf>`_: 0.14+
 
 Only systems that use `ELF
 <https://en.wikipedia.org/wiki/Executable_and_Linkable_Format>`_-based linkage
 are supported (this should be essentially every Linux).
 
 In general, building ``manylinux1`` wheels requires running on a CentOS5
@@ -131,19 +131,18 @@
 test dependencies.
 
 Some of the integration tests also require a running and accessible Docker
 daemon. These tests will pull a number of docker images if they are not already
 available on your system, but it won't update existing images.
 To update these images manually, run::
 
-    docker pull python:3.6-slim
+    docker pull python:3.7-slim
     docker pull quay.io/pypa/manylinux1_x86_64
     docker pull quay.io/pypa/manylinux2010_x86_64
     docker pull quay.io/pypa/manylinux2014_x86_64
-    docker pull quay.io/pypa/manylinux_2_24_x86_64
     docker pull quay.io/pypa/manylinux_2_28_x86_64
 
 You may also remove these images using ``docker rmi``.
 
 Code of Conduct
 ---------------
```

### Comparing `auditwheel-5.3.0/pyproject.toml` & `auditwheel-5.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # enable version inference
 
 [tool.black]
-target-version = ["py36", "py37", "py38", "py39"]
+target-version = ["py37", "py38", "py39", "py310", "py311"]
 extend-exclude = "src/auditwheel/_vendor"
 
 [tool.isort]
+py_version = 37
 profile = "black"
 extend_skip_glob = "src/auditwheel/_vendor/**/*.py"
 
 [tool.mypy]
 follow_imports = "silent"
 ignore_missing_imports = true
 warn_unused_ignores = true
```

### Comparing `auditwheel-5.3.0/setup.cfg` & `auditwheel-5.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 classifier = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Software Development
 	Topic :: Software Development :: Build Tools
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
 install_requires = 
 	pyelftools>=0.24
 	importlib_metadata; python_version < "3.8"
 packages = find:
 package_dir = 
 	=src
-python_requires = >=3.6
+python_requires = >=3.7
 zip_safe = False
 
 [options.package_data]
 auditwheel = *.json
 
 [options.packages.find]
 where = src
```

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/LICENSE.txt` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/__init__.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/convert.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/pack.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/cli/unpack.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/pkginfo.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/util.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/_vendor/wheel/wheelfile.py` & `auditwheel-5.4.0/src/auditwheel/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/condatools.py` & `auditwheel-5.4.0/src/auditwheel/condatools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Context managers like those in wheeltools.py for unpacking
 conda packages.
 """
+from __future__ import annotations
+
 import os
-from typing import List, Optional
 
 from .tmpdirs import InTemporaryDirectory
 from .tools import tarbz2todir
 
 
 class InCondaPkg(InTemporaryDirectory):
     def __init__(self, in_conda_pkg: str) -> None:
@@ -18,19 +19,19 @@
         tarbz2todir(self.in_conda_pkg, self.name)
         return super().__enter__()
 
 
 class InCondaPkgCtx(InCondaPkg):
     def __init__(self, in_conda_pkg: str) -> None:
         super().__init__(in_conda_pkg)
-        self.path: Optional[str] = None
+        self.path: str | None = None
 
     def __enter__(self):
         self.path = super().__enter__()
         return self
 
-    def iter_files(self) -> List[str]:
+    def iter_files(self) -> list[str]:
         if self.path is None:
             raise ValueError("This function should be called from context manager")
         files = os.path.join(self.path, "info", "files")
         with open(files) as f:
             return [line.strip() for line in f.readlines()]
```

### Comparing `auditwheel-5.3.0/src/auditwheel/elfutils.py` & `auditwheel-5.4.0/src/auditwheel/elfutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+from __future__ import annotations
+
 import os
 from os.path import basename, realpath, relpath
-from typing import Dict, Iterator, List, Optional, Set, Tuple
+from typing import Iterator
 
 from elftools.common.exceptions import ELFError
 from elftools.elf.elffile import ELFFile
 
 from .lddtree import parse_ld_paths
 
 
-def elf_read_dt_needed(fn: str) -> List[str]:
+def elf_read_dt_needed(fn: str) -> list[str]:
     needed = []
     with open(fn, "rb") as f:
         elf = ELFFile(f)
         section = elf.get_section_by_name(".dynamic")
         if section is None:
             raise ValueError("Could not find soname in %s" % fn)
 
         for t in section.iter_tags():
             if t.entry.d_tag == "DT_NEEDED":
                 needed.append(t.needed)
 
     return needed
 
 
-def elf_file_filter(paths: Iterator[str]) -> Iterator[Tuple[str, ELFFile]]:
+def elf_file_filter(paths: Iterator[str]) -> Iterator[tuple[str, ELFFile]]:
     """Filter through an iterator of filenames and load up only ELF
     files
     """
 
     for path in paths:
         if path.endswith(".py"):
             continue
@@ -37,15 +39,15 @@
                     candidate = ELFFile(f)
                     yield path, candidate
             except ELFError:
                 # not an elf file
                 continue
 
 
-def elf_find_versioned_symbols(elf: ELFFile) -> Iterator[Tuple[str, str]]:
+def elf_find_versioned_symbols(elf: ELFFile) -> Iterator[tuple[str, str]]:
     section = elf.get_section_by_name(".gnu.version_r")
 
     if section is not None:
         for verneed, verneed_iter in section.iter_versions():
             if verneed.name.startswith("ld-linux") or verneed.name in [
                 "ld64.so.2",
                 "ld64.so.1",
@@ -61,15 +63,14 @@
         # look for UCS2 symbols that are externally referenced
         for sym in section.iter_symbols():
             if (
                 "PyUnicodeUCS2_" in sym.name
                 and sym["st_shndx"] == "SHN_UNDEF"
                 and sym["st_info"]["type"] == "STT_FUNC"
             ):
-
                 yield sym.name
 
 
 def elf_references_PyFPE_jbuf(elf: ELFFile) -> bool:
     offending_symbol_names = ("PyFPE_jbuf", "PyFPE_dummy", "PyFPE_counter")
     section = elf.get_section_by_name(".dynsym")
     if section is not None:
@@ -80,15 +81,15 @@
                 and sym["st_shndx"] == "SHN_UNDEF"
                 and sym["st_info"]["type"] in ("STT_FUNC", "STT_NOTYPE")
             ):
                 return True
     return False
 
 
-def elf_is_python_extension(fn: str, elf: ELFFile) -> Tuple[bool, Optional[int]]:
+def elf_is_python_extension(fn: str, elf: ELFFile) -> tuple[bool, int | None]:
     modname = basename(fn).split(".", 1)[0]
     module_init_f = {
         "init" + modname: 2,
         "PyInit_" + modname: 3,
         "_cffi_pypyinit_" + modname: 2,
     }
 
@@ -98,22 +99,21 @@
 
     for sym in sect.iter_symbols():
         if (
             sym.name in module_init_f
             and sym["st_shndx"] != "SHN_UNDEF"
             and sym["st_info"]["type"] == "STT_FUNC"
         ):
-
             return True, module_init_f[sym.name]
 
     return False, None
 
 
-def elf_read_rpaths(fn: str) -> Dict[str, List[str]]:
-    result = {"rpaths": [], "runpaths": []}  # type: Dict[str, List[str]]
+def elf_read_rpaths(fn: str) -> dict[str, list[str]]:
+    result: dict[str, list[str]] = {"rpaths": [], "runpaths": []}
 
     with open(fn, "rb") as f:
         elf = ELFFile(f)
         section = elf.get_section_by_name(".dynamic")
         if section is None:
             return result
 
@@ -135,30 +135,30 @@
 
     relative = relpath(path, directory)
     if relative.startswith(os.pardir):
         return False
     return True
 
 
-def get_undefined_symbols(path: str) -> Set[str]:
+def get_undefined_symbols(path: str) -> set[str]:
     undef_symbols = set()
     with open(path, "rb") as f:
         elf = ELFFile(f)
         section = elf.get_section_by_name(".dynsym")
         if section is not None:
             # look for all undef symbols
             for sym in section.iter_symbols():
                 if sym["st_shndx"] == "SHN_UNDEF":
                     undef_symbols.add(sym.name)
     return undef_symbols
 
 
 def filter_undefined_symbols(
-    path: str, symbols: Dict[str, List[str]]
-) -> Dict[str, List[str]]:
+    path: str, symbols: dict[str, list[str]]
+) -> dict[str, list[str]]:
     if not symbols:
         return {}
     undef_symbols = set("*") | get_undefined_symbols(path)
     result = {}
     for lib, sym_list in symbols.items():
         intersection = set(sym_list) & undef_symbols
         if intersection:
```

### Comparing `auditwheel-5.3.0/src/auditwheel/genericpkgctx.py` & `auditwheel-5.4.0/src/auditwheel/genericpkgctx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional, Union
+from __future__ import annotations
 
 from .condatools import InCondaPkgCtx
 from .wheeltools import InWheelCtx
 
 
 def InGenericPkgCtx(
-    in_path: str, out_path: Optional[str] = None
-) -> Union[InWheelCtx, InCondaPkgCtx]:
+    in_path: str, out_path: str | None = None
+) -> InWheelCtx | InCondaPkgCtx:
     """Factory that returns a InWheelCtx or InCondaPkgCtx
     context manager depending on the file extension
     """
     if in_path.endswith(".whl"):
         return InWheelCtx(in_path, out_path)
     if in_path.endswith(".tar.bz2"):
         if out_path is not None:
```

### Comparing `auditwheel-5.3.0/src/auditwheel/lddtree.py` & `auditwheel-5.4.0/src/auditwheel/lddtree.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 """Read the ELF dependency tree
 
 This does not work like `ldd` in that we do not execute/load code (only read
 files on disk), and we parse the dependency structure as a tree rather than
  a flat list.
 """
 
+from __future__ import annotations
+
 import errno
 import functools
 import glob
 import logging
 import os
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any
 
 from elftools.elf.elffile import ELFFile
 
 from .libc import Libc, get_libc
 
 log = logging.getLogger(__name__)
 __all__ = ["lddtree"]
@@ -68,21 +70,21 @@
 
     while os.path.islink(root + path):
         path = os.path.join(os.path.dirname(path), os.readlink(root + path))
 
     return normpath((root + path) if prefixed else path)
 
 
-def dedupe(items: List[str]) -> List[str]:
+def dedupe(items: list[str]) -> list[str]:
     """Remove all duplicates from ``items`` (keeping order)"""
-    seen = {}  # type: Dict[str, str]
+    seen: dict[str, str] = {}
     return [seen.setdefault(x, x) for x in items if x not in seen]
 
 
-def parse_ld_paths(str_ldpaths: str, path: str, root: str = "") -> List[str]:
+def parse_ld_paths(str_ldpaths: str, path: str, root: str = "") -> list[str]:
     """Parse the colon-delimited list of paths and apply ldso rules to each
 
     Note the special handling as dictated by the ldso:
     - Empty paths are equivalent to $PWD
     - $ORIGIN is expanded to the path of the given file
     - (TODO) $LIB and friends
 
@@ -95,29 +97,29 @@
     path
         The object actively being parsed (used for $ORIGIN)
 
     Returns
     -------
         list of processed paths
     """
-    ldpaths = []  # type: List[str]
+    ldpaths: list[str] = []
     for ldpath in str_ldpaths.split(":"):
         if ldpath == "":
             # The ldso treats "" paths as $PWD.
             ldpath = os.getcwd()
         elif "$ORIGIN" in ldpath:
             ldpath = ldpath.replace("$ORIGIN", os.path.dirname(os.path.abspath(path)))
         else:
             ldpath = root + ldpath
         ldpaths.append(normpath(ldpath))
     return [p for p in dedupe(ldpaths) if os.path.isdir(p)]
 
 
 @functools.lru_cache()
-def parse_ld_so_conf(ldso_conf: str, root: str = "/", _first: bool = True) -> List[str]:
+def parse_ld_so_conf(ldso_conf: str, root: str = "/", _first: bool = True) -> list[str]:
     """Load all the paths from a given ldso config file
 
     This should handle comments, whitespace, and "include" statements.
 
     Parameters
     ----------
     ldso_conf
@@ -127,15 +129,15 @@
     _first
         Recursive use only; is this the first ELF?
 
     Returns
     -------
     list of paths found
     """
-    paths = []  # type: List[str]
+    paths: list[str] = []
 
     dbg_pfx = "" if _first else "  "
     try:
         log.debug("%sparse_ld_so_conf(%s)", dbg_pfx, ldso_conf)
         with open(ldso_conf) as f:
             for line in f.readlines():
                 line = line.split("#", 1)[0].strip()
@@ -161,15 +163,15 @@
         # Remove duplicate entries to speed things up.
         paths = [p for p in dedupe(paths) if os.path.isdir(p)]
 
     return paths
 
 
 @functools.lru_cache()
-def load_ld_paths(root: str = "/", prefix: str = "") -> Dict[str, List[str]]:
+def load_ld_paths(root: str = "/", prefix: str = "") -> dict[str, list[str]]:
     """Load linker paths from common locations
 
     This parses the ld.so.conf and LD_LIBRARY_PATH env var.
 
     Parameters
     ----------
     root
@@ -177,15 +179,15 @@
     prefix
         The path under ``root`` to search
 
     Returns
     -------
     dict containing library paths to search
     """
-    ldpaths = {"conf": [], "env": [], "interp": []}  # type: Dict
+    ldpaths: dict = {"conf": [], "env": [], "interp": []}
 
     # Load up $LD_LIBRARY_PATH.
     env_ldpath = os.environ.get("LD_LIBRARY_PATH")
     if env_ldpath is not None:
         if root != "/":
             log.warning("ignoring LD_LIBRARY_PATH due to ROOT usage")
         else:
@@ -254,26 +256,26 @@
         and elf1.elfclass == elf2.elfclass
         and elf1.little_endian == elf2.little_endian
         and elf1.header["e_machine"] == elf2.header["e_machine"]
     )
 
 
 def find_lib(
-    elf: ELFFile, lib: str, ldpaths: List[str], root: str = "/"
-) -> Tuple[Optional[str], Optional[str]]:
+    elf: ELFFile, lib: str, ldpaths: list[str], root: str = "/"
+) -> tuple[str | None, str | None]:
     """Try to locate a ``lib`` that is compatible to ``elf`` in the given
     ``ldpaths``
 
     Parameters
     ----------
     elf : ELFFile
         The elf which the library should be compatible with (ELF wise)
     lib : str
         The library (basename) to search for
-    ldpaths : List[str]
+    ldpaths : list[str]
         A list of paths to search
     root : str
        The root path to resolve symlinks
 
     Returns
     -------
     Tuple of the full path to the desired library and the real path to it
@@ -292,19 +294,19 @@
     return (None, None)
 
 
 def lddtree(
     path: str,
     root: str = "/",
     prefix: str = "",
-    ldpaths: Optional[Dict[str, List[str]]] = None,
-    display: Optional[str] = None,
+    ldpaths: dict[str, list[str]] | None = None,
+    display: str | None = None,
     _first: bool = True,
-    _all_libs: Dict = {},
-) -> Dict:
+    _all_libs: dict = {},
+) -> dict:
     """Parse the ELF dependency tree of the specified file
 
     Parameters
     ----------
     path
         The ELF to scan
     root
@@ -343,23 +345,23 @@
     """
     if not ldpaths:
         ldpaths = load_ld_paths().copy()
 
     if _first:
         _all_libs = {}
 
-    ret = {
+    ret: dict[str, Any] = {
         "interp": None,
         "path": path if display is None else display,
         "realpath": path,
         "needed": [],
         "rpath": [],
         "runpath": [],
         "libs": _all_libs,
-    }  # type: Dict[str, Any]
+    }
 
     log.debug("lddtree(%s)" % path)
 
     with open(path, "rb") as f:
         elf = ELFFile(f)
 
         # If this is the first ELF, extract the interpreter.
@@ -383,17 +385,17 @@
                         root + prefix + "/usr" + os.path.dirname(interp).lstrip(prefix)
                     ),
                 ]
                 log.debug("  ldpaths[interp]  = %s", ldpaths["interp"])
                 break
 
         # Parse the ELF's dynamic tags.
-        libs = []  # type: List[str]
-        rpaths = []  # type: List[str]
-        runpaths = []  # type: List[str]
+        libs: list[str] = []
+        rpaths: list[str] = []
+        runpaths: list[str] = []
         for segment in elf.iter_segments():
             if segment.header.p_type != "PT_DYNAMIC":
                 continue
 
             for t in segment.iter_tags():
                 if t.entry.d_tag == "DT_RPATH":
                     rpaths = parse_ld_paths(t.rpath, path=path, root=root)
@@ -416,15 +418,15 @@
             log.debug("  ldpaths[rpath]   = %s", rpaths)
             log.debug("  ldpaths[runpath] = %s", runpaths)
         ret["rpath"] = rpaths
         ret["runpath"] = runpaths
         ret["needed"] = libs
 
         # Search for the libs this ELF uses.
-        all_ldpaths = None  # type: Optional[List[str]]
+        all_ldpaths: list[str] | None = None
         for lib in libs:
             if lib in _all_libs:
                 continue
             if all_ldpaths is None:
                 all_ldpaths = (
                     ldpaths["rpath"]
                     + rpaths
```

### Comparing `auditwheel-5.3.0/src/auditwheel/main.py` & `auditwheel-5.4.0/src/auditwheel/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from __future__ import annotations
+
 import argparse
 import logging
 import os
 import pathlib
 import sys
 
 if sys.version_info[:2] >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata
 
-from typing import Optional
-
 import auditwheel
 
 from . import main_addtag, main_lddtree, main_repair, main_show
 
 
-def main() -> Optional[int]:
+def main() -> int | None:
     if sys.platform != "linux":
         print("Error: This tool only supports Linux")
         return 1
 
     location = pathlib.Path(auditwheel.__file__).parent.resolve()
     version = "auditwheel {} installed at {} (python {}.{})".format(
         metadata.version("auditwheel"), location, *sys.version_info
```

### Comparing `auditwheel-5.3.0/src/auditwheel/main_addtag.py` & `auditwheel-5.4.0/src/auditwheel/main_addtag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from os.path import abspath, basename, exists, join
 
 logger = logging.getLogger(__name__)
 
 
 def configure_parser(sub_parsers):
```

### Comparing `auditwheel-5.3.0/src/auditwheel/main_repair.py` & `auditwheel-5.4.0/src/auditwheel/main_repair.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import logging
 from os.path import abspath, basename, exists, isfile
 
 from auditwheel.patcher import Patchelf
 
 from .policy import (
```

### Comparing `auditwheel-5.3.0/src/auditwheel/main_show.py` & `auditwheel-5.4.0/src/auditwheel/main_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from collections import OrderedDict
 
 logger = logging.getLogger(__name__)
 
 
 def configure_parser(sub_parsers):
```

### Comparing `auditwheel-5.3.0/src/auditwheel/musllinux.py` & `auditwheel-5.4.0/src/auditwheel/musllinux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import pathlib
 import re
 import subprocess
 from typing import NamedTuple
 
 from auditwheel.error import InvalidLibc
```

### Comparing `auditwheel-5.3.0/src/auditwheel/patcher.py` & `auditwheel-5.4.0/src/auditwheel/patcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
+
 import re
 from distutils.spawn import find_executable
 from itertools import chain
 from subprocess import CalledProcessError, check_call, check_output
-from typing import Tuple
 
 
 class ElfPatcher:
-    def replace_needed(self, file_name: str, *old_new_pairs: Tuple[str, str]) -> None:
+    def replace_needed(self, file_name: str, *old_new_pairs: tuple[str, str]) -> None:
         raise NotImplementedError
 
     def set_soname(self, file_name: str, new_so_name: str) -> None:
         raise NotImplementedError
 
     def set_rpath(self, file_name: str, rpath: str) -> None:
         raise NotImplementedError
@@ -39,33 +40,31 @@
     )
 
 
 class Patchelf(ElfPatcher):
     def __init__(self) -> None:
         _verify_patchelf()
 
-    def replace_needed(self, file_name: str, *old_new_pairs: Tuple[str, str]) -> None:
+    def replace_needed(self, file_name: str, *old_new_pairs: tuple[str, str]) -> None:
         check_call(
             [
                 "patchelf",
                 *chain.from_iterable(
                     ("--replace-needed", *pair) for pair in old_new_pairs
                 ),
                 file_name,
             ]
         )
 
     def set_soname(self, file_name: str, new_so_name: str) -> None:
         check_call(["patchelf", "--set-soname", new_so_name, file_name])
 
     def set_rpath(self, file_name: str, rpath: str) -> None:
-
         check_call(["patchelf", "--remove-rpath", file_name])
         check_call(["patchelf", "--force-rpath", "--set-rpath", rpath, file_name])
 
     def get_rpath(self, file_name: str) -> str:
-
         return (
             check_output(["patchelf", "--print-rpath", file_name])
             .decode("utf-8")
             .strip()
         )
```

### Comparing `auditwheel-5.3.0/src/auditwheel/policy/__init__.py` & `auditwheel-5.4.0/src/auditwheel/policy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,47 @@
+from __future__ import annotations
+
 import json
 import logging
 import platform as _platform_module
 import sys
 from collections import defaultdict
 from os.path import abspath, dirname, join
 from pathlib import Path
-from typing import Dict, List, Optional, Set
 
 from ..libc import Libc, get_libc
 from ..musllinux import find_musl_libc, get_musl_version
 
 _HERE = Path(__file__).parent
 
 logger = logging.getLogger(__name__)
 
 # https://docs.python.org/3/library/platform.html#platform.architecture
 bits = 8 * (8 if sys.maxsize > 2**32 else 4)
 
 
 def get_arch_name() -> str:
     machine = _platform_module.machine()
-    if machine not in {"x86_64", "i686"}:
-        return machine
-    else:
+    if sys.platform == "darwin" and machine == "arm64":
+        return "aarch64"
+    if machine in {"x86_64", "i686"}:
         return {64: "x86_64", 32: "i686"}[bits]
+    if machine in {"aarch64", "armv8l"}:
+        # use armv7l policy for 64-bit arm kernel in 32-bit mode (armv8l)
+        return {64: "aarch64", 32: "armv7l"}[bits]
+    return machine
 
 
 _ARCH_NAME = get_arch_name()
 _LIBC = get_libc()
 
 
 def _validate_pep600_compliance(policies) -> None:
-    symbol_versions: Dict[str, Dict[str, Set[str]]] = {}
-    lib_whitelist: Set[str] = set()
+    symbol_versions: dict[str, dict[str, set[str]]] = {}
+    lib_whitelist: set[str] = set()
     for policy in sorted(policies, key=lambda x: x["priority"], reverse=True):
         if policy["name"] == "linux":
             continue
         if not lib_whitelist.issubset(set(policy["lib_whitelist"])):
             diff = lib_whitelist - set(policy["lib_whitelist"])
             raise ValueError(
                 'Invalid "policy.json" file. Missing whitelist libraries in '
@@ -127,38 +132,38 @@
 
 def _load_policy_schema():
     with open(join(dirname(abspath(__file__)), "policy-schema.json")) as f_:
         schema = json.load(f_)
     return schema
 
 
-def get_policy_by_name(name: str) -> Optional[Dict]:
+def get_policy_by_name(name: str) -> dict | None:
     matches = [p for p in _POLICIES if p["name"] == name or name in p["aliases"]]
     if len(matches) == 0:
         return None
     if len(matches) > 1:
         raise RuntimeError("Internal error. Policies should be unique")
     return matches[0]
 
 
-def get_policy_name(priority: int) -> Optional[str]:
+def get_policy_name(priority: int) -> str | None:
     matches = [p["name"] for p in _POLICIES if p["priority"] == priority]
     if len(matches) == 0:
         return None
     if len(matches) > 1:
         raise RuntimeError("Internal error. priorities should be unique")
     return matches[0]
 
 
-def get_priority_by_name(name: str) -> Optional[int]:
+def get_priority_by_name(name: str) -> int | None:
     policy = get_policy_by_name(name)
     return None if policy is None else policy["priority"]
 
 
-def get_replace_platforms(name: str) -> List[str]:
+def get_replace_platforms(name: str) -> list[str]:
     """Extract platform tag replacement rules from policy
 
     >>> get_replace_platforms('linux_x86_64')
     []
     >>> get_replace_platforms('linux_i686')
     []
     >>> get_replace_platforms('manylinux1_x86_64')
```

### Comparing `auditwheel-5.3.0/src/auditwheel/policy/external_references.py` & `auditwheel-5.4.0/src/auditwheel/policy/external_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 import logging
 import re
-from typing import Any, Dict, Generator, Set
+from typing import Any, Generator
 
 from ..elfutils import filter_undefined_symbols, is_subdir
 from . import load_policies
 
 log = logging.getLogger(__name__)
-LIBPYTHON_RE = re.compile(r"^libpython\d\.\dm?.so(.\d)*$")
+LIBPYTHON_RE = re.compile(r"^libpython\d+\.\d+m?.so(.\d)*$")
 
 
-def lddtree_external_references(lddtree: Dict, wheel_path: str) -> Dict:
+def lddtree_external_references(lddtree: dict, wheel_path: str) -> dict:
     # XXX: Document the lddtree structure, or put it in something
     # more stable than a big nested dict
     policies = load_policies()
 
-    def filter_libs(libs: Set[str], whitelist: Set[str]) -> Generator[str, None, None]:
+    def filter_libs(libs: set[str], whitelist: set[str]) -> Generator[str, None, None]:
         for lib in libs:
             if "ld-linux" in lib or lib in ["ld64.so.2", "ld64.so.1"]:
                 # always exclude ELF dynamic linker/loader
                 # 'ld64.so.2' on s390x
                 # 'ld64.so.1' on ppc64le
                 # 'ld-linux*' on other platforms
                 continue
@@ -26,29 +28,29 @@
                 # always exclude libpythonXY
                 continue
             if lib in whitelist:
                 # exclude any libs in the whitelist
                 continue
             yield lib
 
-    def get_req_external(libs: Set[str], whitelist: Set[str]) -> Set[str]:
+    def get_req_external(libs: set[str], whitelist: set[str]) -> set[str]:
         # get all the required external libraries
         libs = libs.copy()
         reqs = set()
         while libs:
             lib = libs.pop()
             reqs.add(lib)
             for dep in filter_libs(lddtree["libs"][lib]["needed"], whitelist):
                 if dep not in reqs:
                     libs.add(dep)
         return reqs
 
-    ret = {}  # type: Dict[str, Dict[str, Any]]
+    ret: dict[str, dict[str, Any]] = {}
     for p in policies:
-        needed_external_libs = set()  # type: Set[str]
+        needed_external_libs: set[str] = set()
         blacklist = {}
 
         if not (p["name"] == "linux" and p["priority"] == 0):
             # special-case the generic linux platform here, because it
             # doesn't have a whitelist. or, you could say its
             # whitelist is the complete set of all libraries. so nothing
             # is considered "external" that needs to be copied in.
```

### Comparing `auditwheel-5.3.0/src/auditwheel/policy/manylinux-policy.json` & `auditwheel-5.4.0/src/auditwheel/policy/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/policy/musllinux-policy.json` & `auditwheel-5.4.0/src/auditwheel/policy/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/policy/policy-schema.json` & `auditwheel-5.4.0/src/auditwheel/policy/policy-schema.json`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/src/auditwheel/policy/versioned_symbols.py` & `auditwheel-5.4.0/src/auditwheel/policy/versioned_symbols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 import logging
-from typing import Dict, List, Set
 
 from . import load_policies
 
 log = logging.getLogger(__name__)
 
 
-def versioned_symbols_policy(versioned_symbols: Dict[str, Set[str]]) -> int:
+def versioned_symbols_policy(versioned_symbols: dict[str, set[str]]) -> int:
     def policy_is_satisfied(
-        policy_name: str, policy_sym_vers: Dict[str, Set[str]]
+        policy_name: str, policy_sym_vers: dict[str, set[str]]
     ) -> bool:
         policy_satisfied = True
         for name in set(required_vers) & set(policy_sym_vers):
             if not required_vers[name].issubset(policy_sym_vers[name]):
                 for symbol in required_vers[name] - policy_sym_vers[name]:
                     log.debug(
                         "Package requires %s, incompatible with "
@@ -20,20 +21,20 @@
                         symbol,
                         policy_name,
                         policy_sym_vers[name],
                     )
                 policy_satisfied = False
         return policy_satisfied
 
-    required_vers = {}  # type: Dict[str, Set[str]]
+    required_vers: dict[str, set[str]] = {}
     for symbols in versioned_symbols.values():
         for symbol in symbols:
             sym_name, _, _ = symbol.partition("_")
             required_vers.setdefault(sym_name, set()).add(symbol)
-    matching_policies = []  # type: List[int]
+    matching_policies: list[int] = []
     for p in load_policies():
         policy_sym_vers = {
             sym_name: {sym_name + "_" + version for version in versions}
             for sym_name, versions in p["symbol_versions"].items()
         }
         if policy_is_satisfied(p["name"], policy_sym_vers):
             matching_policies.append(p["priority"])
```

### Comparing `auditwheel-5.3.0/src/auditwheel/repair.py` & `auditwheel-5.4.0/src/auditwheel/repair.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
+
 import itertools
 import logging
 import os
 import platform
 import re
 import shutil
 import stat
 from collections import OrderedDict
 from os.path import abspath, basename, dirname, exists, isabs
 from os.path import join as pjoin
 from subprocess import check_call
-from typing import Dict, Iterable, List, Optional, Tuple
+from typing import Iterable
 
 from auditwheel.patcher import ElfPatcher
 
 from .elfutils import elf_read_dt_needed, elf_read_rpaths, is_subdir
 from .hashfile import hashfile
 from .policy import get_replace_platforms
 from .wheel_abi import get_wheel_elfdata
@@ -28,30 +30,29 @@
      -(?P<pyver>[a-z].+?)-(?P<abi>.+?)-(?P<plat>.+?)(\.whl|\.dist-info)$""",
     re.VERBOSE,
 ).match
 
 
 def repair_wheel(
     wheel_path: str,
-    abis: List[str],
+    abis: list[str],
     lib_sdir: str,
     out_dir: str,
     update_tags: bool,
     patcher: ElfPatcher,
-    exclude: List[str],
+    exclude: list[str],
     strip: bool = False,
-) -> Optional[str]:
-
+) -> str | None:
     external_refs_by_fn = get_wheel_elfdata(wheel_path)[1]
 
     # Do not repair a pure wheel, i.e. has no external refs
     if not external_refs_by_fn:
         return None
 
-    soname_map = {}  # type: Dict[str, Tuple[str, str]]
+    soname_map: dict[str, tuple[str, str]] = {}
     if not isabs(out_dir):
         out_dir = abspath(out_dir)
 
     wheel_fname = basename(wheel_path)
 
     with InWheelCtx(wheel_path) as ctx:
         ctx.out_wheel = pjoin(out_dir, wheel_fname)
@@ -64,18 +65,17 @@
 
         if not exists(dest_dir):
             os.mkdir(dest_dir)
 
         # here, fn is a path to a python extension library in
         # the wheel, and v['libs'] contains its required libs
         for fn, v in external_refs_by_fn.items():
-            ext_libs = v[abis[0]]["libs"]  # type: Dict[str, str]
-            replacements = []  # type: List[Tuple[str, str]]
+            ext_libs: dict[str, str] = v[abis[0]]["libs"]
+            replacements: list[tuple[str, str]] = []
             for soname, src_path in ext_libs.items():
-
                 if soname in exclude:
                     logger.info(f"Excluding {soname}")
                     continue
 
                 if src_path is None:
                     raise ValueError(
                         (
@@ -122,15 +122,15 @@
 
 def strip_symbols(libraries: Iterable[str]) -> None:
     for lib in libraries:
         logger.info("Stripping symbols from %s", lib)
         check_call(["strip", "-s", lib])
 
 
-def copylib(src_path: str, dest_dir: str, patcher: ElfPatcher) -> Tuple[str, str]:
+def copylib(src_path: str, dest_dir: str, patcher: ElfPatcher) -> tuple[str, str]:
     """Graft a shared library from the system into the wheel and update the
     relevant links.
 
     1) Copy the file from src_path to dest_dir/
     2) Rename the shared object from soname to soname.<unique>
     3) If the library has a RUNPATH/RPATH, clear it and set RPATH to point to
     its new location.
```

### Comparing `auditwheel-5.3.0/src/auditwheel/tmpdirs.py` & `auditwheel-5.4.0/src/auditwheel/tmpdirs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Contexts for *with* statement providing temporary directories
 """
+from __future__ import annotations
+
 import os
 from tempfile import TemporaryDirectory
 from types import TracebackType
-from typing import Optional, Type
 
 
 class InTemporaryDirectory:
     """Create, return, and change directory to a temporary directory
 
     Examples
     --------
@@ -33,17 +34,17 @@
     def __enter__(self) -> str:
         self._pwd = os.getcwd()
         os.chdir(self._tmpdir.name)
         return self._tmpdir.__enter__()
 
     def __exit__(
         self,
-        exc: Optional[Type[BaseException]],
-        value: Optional[BaseException],
-        tb: Optional[TracebackType],
+        exc: type[BaseException] | None,
+        value: BaseException | None,
+        tb: TracebackType | None,
     ) -> None:
         os.chdir(self._pwd)
         return self._tmpdir.__exit__(exc, value, tb)
 
 
 class InGivenDirectory:
     """Change directory to given directory for duration of ``with`` block
@@ -65,15 +66,15 @@
     ...     pass
 
     You can then look at the temporary file outputs to debug what is happening,
     fix, and finally replace ``InGivenDirectory`` with ``InTemporaryDirectory``
     again.
     """
 
-    def __init__(self, path: Optional[str] = None) -> None:
+    def __init__(self, path: str | None = None) -> None:
         """Initialize directory context manager
 
         Parameters
         ----------
         path : None or str, optional
             path to change directory to, for duration of ``with`` block.
             Defaults to ``os.getcwd()`` if None
@@ -87,12 +88,12 @@
         if not os.path.isdir(self.name):
             os.mkdir(self.name)
         os.chdir(self.name)
         return self.name
 
     def __exit__(
         self,
-        exc: Optional[Type[BaseException]],
-        value: Optional[BaseException],
-        tb: Optional[TracebackType],
+        exc: type[BaseException] | None,
+        value: BaseException | None,
+        tb: TracebackType | None,
     ) -> None:
         os.chdir(self._pwd)
```

### Comparing `auditwheel-5.3.0/src/auditwheel/tools.py` & `auditwheel-5.4.0/src/auditwheel/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from __future__ import annotations
+
 import argparse
 import os
 import subprocess
 import zipfile
 from datetime import datetime, timezone
-from typing import Any, Iterable, List, Optional
+from typing import Any, Iterable
 
 
-def unique_by_index(sequence: Iterable[Any]) -> List[Any]:
+def unique_by_index(sequence: Iterable[Any]) -> list[Any]:
     """unique elements in `sequence` in the order in which they occur
 
     Parameters
     ----------
     sequence : iterable
 
     Returns
@@ -46,15 +48,15 @@
                 os.chmod(extracted_path, 0o755)
             elif attr != 0:
                 attr &= 511  # only keep permission bits
                 attr |= 6 << 6  # at least read/write for current user
                 os.chmod(extracted_path, attr)
 
 
-def dir2zip(in_dir: str, zip_fname: str, date_time: Optional[datetime] = None) -> None:
+def dir2zip(in_dir: str, zip_fname: str, date_time: datetime | None = None) -> None:
     """Make a zip file `zip_fname` with contents of directory `in_dir`
 
     The recorded filenames are relative to `in_dir`, so doing a standard zip
     unpack of the resulting `zip_fname` in an empty directory will result in
     the original directory contents.
 
     Parameters
```

### Comparing `auditwheel-5.3.0/src/auditwheel/wheel_abi.py` & `auditwheel-5.4.0/src/auditwheel/wheel_abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from __future__ import annotations
+
 import functools
 import itertools
 import json
 import logging
 import os
 from collections import defaultdict, namedtuple
 from collections.abc import Mapping
 from copy import deepcopy
 from os.path import basename
-from typing import Dict, Set
 
 from .elfutils import (
     elf_file_filter,
     elf_find_ucs2_symbols,
     elf_find_versioned_symbols,
     elf_is_python_extension,
     elf_references_PyFPE_jbuf,
@@ -58,15 +59,15 @@
 
 
 @functools.lru_cache()
 def get_wheel_elfdata(wheel_fn: str):
     full_elftree = {}
     nonpy_elftree = {}
     full_external_refs = {}
-    versioned_symbols = defaultdict(lambda: set())  # type: Dict[str, Set[str]]
+    versioned_symbols: dict[str, set[str]] = defaultdict(lambda: set())
     uses_ucs2_symbols = False
     uses_PyFPE_jbuf = False
 
     with InGenericPkgCtx(wheel_fn) as ctx:
         shared_libraries_in_purelib = []
 
         platform_wheel = False
@@ -161,22 +162,22 @@
         full_external_refs,
         versioned_symbols,
         uses_ucs2_symbols,
         uses_PyFPE_jbuf,
     )
 
 
-def get_external_libs(external_refs) -> Dict[str, str]:
+def get_external_libs(external_refs) -> dict[str, str]:
     """Get external library dependencies for all policies excluding the default
     linux policy
     :param external_refs: external references for all policies
     :return: {realpath: soname} e.g.
     {'/path/to/external_ref.so.1.2.3': 'external_ref.so.1'}
     """
-    result: Dict[str, str] = {}
+    result: dict[str, str] = {}
     for policy in external_refs.values():
         # linux tag (priority 0) has no white-list, do not analyze it
         if policy["priority"] == 0:
             continue
         # go through all libs, retrieving their soname and realpath
         for libname, realpath in policy["libs"].items():
             if realpath and realpath not in result.keys():
```

### Comparing `auditwheel-5.3.0/src/auditwheel/wheeltools.py` & `auditwheel-5.4.0/src/auditwheel/wheeltools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """ General tools for working with wheels
 
 Tools that aren't specific to delocation
 """
 
+from __future__ import annotations
+
 import csv
 import glob
 import hashlib
 import logging
 import os
 from base64 import urlsafe_b64encode
 from datetime import datetime, timezone
 from itertools import product
 from os.path import abspath, basename, dirname, exists
 from os.path import join as pjoin
 from os.path import relpath
 from os.path import sep as psep
 from os.path import splitext
 from types import TracebackType
-from typing import Generator, Iterable, List, Optional, Type
+from typing import Generator, Iterable
 
 from ._vendor.wheel.pkginfo import read_pkg_info, write_pkg_info
 from ._vendor.wheel.wheelfile import WHEEL_INFO_RE
 from .tmpdirs import InTemporaryDirectory
 from .tools import dir2zip, unique_by_index, zip2dir
 
 logger = logging.getLogger(__name__)
@@ -97,15 +99,15 @@
     """Context manager for doing things inside wheels
 
     On entering, you'll find yourself in the root tree of the wheel.  If you've
     asked for an output wheel, then on exit we'll rewrite the wheel record and
     pack stuff up for you.
     """
 
-    def __init__(self, in_wheel: str, out_wheel: Optional[str] = None) -> None:
+    def __init__(self, in_wheel: str, out_wheel: str | None = None) -> None:
         """Initialize in-wheel context manager
 
         Parameters
         ----------
         in_wheel : str
             filename of wheel to unpack and work inside
         out_wheel : None or str:
@@ -118,17 +120,17 @@
 
     def __enter__(self) -> str:
         zip2dir(self.in_wheel, self.name)
         return super().__enter__()
 
     def __exit__(
         self,
-        exc: Optional[Type[BaseException]],
-        value: Optional[BaseException],
-        tb: Optional[TracebackType],
+        exc: type[BaseException] | None,
+        value: BaseException | None,
+        tb: TracebackType | None,
     ) -> None:
         if self.out_wheel is not None:
             rewrite_record(self.name)
             date_time = None
             timestamp = os.environ.get("SOURCE_DATE_EPOCH")
             if timestamp:
                 date_time = datetime.fromtimestamp(int(timestamp), tz=timezone.utc)
@@ -148,15 +150,15 @@
     will dicate what the output wheel name is, or whether you want to save at
     all.
 
     The current path of the wheel contents is set in the attribute
     ``wheel_path``.
     """
 
-    def __init__(self, in_wheel: str, out_wheel: Optional[str] = None) -> None:
+    def __init__(self, in_wheel: str, out_wheel: str | None = None) -> None:
         """Init in-wheel context manager returning self from enter
 
         Parameters
         ----------
         in_wheel : str
             filename of wheel to unpack and work inside
         out_wheel : None or str:
@@ -182,15 +184,15 @@
         reader = csv.reader(r for r in record.splitlines())
         for row in reader:
             filename = row[0]
             yield filename
 
 
 def add_platforms(
-    wheel_ctx: InWheelCtx, platforms: List[str], remove_platforms: Iterable[str] = ()
+    wheel_ctx: InWheelCtx, platforms: list[str], remove_platforms: Iterable[str] = ()
 ) -> str:
     """Add platform tags `platforms` to a wheel
 
     Add any platform tags in `platforms` that are missing
     to wheel_ctx's filename and ``WHEEL`` file.
 
     Parameters
```

### Comparing `auditwheel-5.3.0/src/auditwheel.egg-info/PKG-INFO` & `auditwheel-5.4.0/src/auditwheel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: auditwheel
-Version: 5.3.0
+Version: 5.4.0
 Summary: Cross-distribution Linux wheels
 Home-page: https://github.com/pypa/auditwheel
 Author: Robert T. McGibbon
 Author-email: rmcgibbo@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: coverage
 Provides-Extra: develop
 License-File: LICENSE
 
 auditwheel
@@ -66,15 +66,15 @@
 will be picked up at runtime. This accomplishes a similar result as if the libraries had
 been statically linked without requiring changes to the build system. Packagers are
 advised that bundling, like static linking, may implicate copyright concerns.
 
 Requirements
 ------------
 - OS: Linux
-- Python: 3.6+
+- Python: 3.7+
 - `patchelf <https://github.com/NixOS/patchelf>`_: 0.14+
 
 Only systems that use `ELF
 <https://en.wikipedia.org/wiki/Executable_and_Linkable_Format>`_-based linkage
 are supported (this should be essentially every Linux).
 
 In general, building ``manylinux1`` wheels requires running on a CentOS5
@@ -161,19 +161,18 @@
 test dependencies.
 
 Some of the integration tests also require a running and accessible Docker
 daemon. These tests will pull a number of docker images if they are not already
 available on your system, but it won't update existing images.
 To update these images manually, run::
 
-    docker pull python:3.6-slim
+    docker pull python:3.7-slim
     docker pull quay.io/pypa/manylinux1_x86_64
     docker pull quay.io/pypa/manylinux2010_x86_64
     docker pull quay.io/pypa/manylinux2014_x86_64
-    docker pull quay.io/pypa/manylinux_2_24_x86_64
     docker pull quay.io/pypa/manylinux_2_28_x86_64
 
 You may also remove these images using ``docker rmi``.
 
 Code of Conduct
 ---------------
```

### Comparing `auditwheel-5.3.0/src/auditwheel.egg-info/SOURCES.txt` & `auditwheel-5.4.0/src/auditwheel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/cffi-1.5.0-cp27-none-linux_x86_64.whl` & `auditwheel-5.4.0/tests/integration/cffi-1.5.0-cp27-none-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/fpewheel-0.0.0-cp35-cp35m-linux_x86_64.whl` & `auditwheel-5.4.0/tests/integration/fpewheel-0.0.0-cp35-cp35m-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/internal_rpath/setup.py` & `auditwheel-5.4.0/tests/integration/internal_rpath/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from setuptools import Extension, find_packages, setup
 
 package_name = "internal_rpath"
 setup(
     name=package_name,
     version="1.0",
     description="Auditwheel multiple top-level extensions example",
```

### Comparing `auditwheel-5.3.0/tests/integration/multiple_top_level/setup.py` & `auditwheel-5.4.0/tests/integration/multiple_top_level/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from setuptools import Extension, find_packages, setup
 
 setup(
     name="multiple_top_level",
     version="1.0",
     description="Auditwheel multiple top-level extensions example",
     packages=find_packages(where="src"),
```

### Comparing `auditwheel-5.3.0/tests/integration/nonpy_rpath/README.md` & `auditwheel-5.4.0/tests/integration/nonpy_rpath/README.md`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/nonpy_rpath/nonpy_rpath.cpp` & `auditwheel-5.4.0/tests/integration/nonpy_rpath/nonpy_rpath.cpp`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/nonpy_rpath/setup.py` & `auditwheel-5.4.0/tests/integration/nonpy_rpath/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 
 import setuptools.command.build_ext
 from setuptools import Distribution, find_packages, setup
 from setuptools.extension import Extension, Library
 
 # despite its name, setuptools.command.build_ext.link_shared_object won't
```

### Comparing `auditwheel-5.3.0/tests/integration/plumbum-1.6.8-py2.py3-none-any.whl` & `auditwheel-5.4.0/tests/integration/plumbum-1.6.8-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/python_snappy-0.5.2-pp260-pypy_41-linux_x86_64.whl` & `auditwheel-5.4.0/tests/integration/python_snappy-0.5.2-pp260-pypy_41-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/test_bundled_wheels.py` & `auditwheel-5.4.0/tests/integration/test_bundled_wheels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import platform
 import subprocess
 import sys
 import zipfile
 from argparse import Namespace
 from datetime import datetime, timezone
 from pathlib import Path
```

### Comparing `auditwheel-5.3.0/tests/integration/test_glibcxx_3_4_25/testentropy.cpp` & `auditwheel-5.4.0/tests/integration/test_glibcxx_3_4_25/testentropy.cpp`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/test_manylinux.py` & `auditwheel-5.4.0/tests/integration/test_manylinux.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import glob
 import io
 import logging
 import os
 import os.path as op
 import re
 import shutil
@@ -20,36 +22,32 @@
 
 
 ENCODING = "utf-8"
 PLATFORM = get_arch_name()
 MANYLINUX1_IMAGE_ID = f"quay.io/pypa/manylinux1_{PLATFORM}:latest"
 MANYLINUX2010_IMAGE_ID = f"quay.io/pypa/manylinux2010_{PLATFORM}:latest"
 MANYLINUX2014_IMAGE_ID = f"quay.io/pypa/manylinux2014_{PLATFORM}:latest"
-MANYLINUX_2_24_IMAGE_ID = f"quay.io/pypa/manylinux_2_24_{PLATFORM}:latest"
 MANYLINUX_2_28_IMAGE_ID = f"quay.io/pypa/manylinux_2_28_{PLATFORM}:latest"
 if PLATFORM in {"i686", "x86_64"}:
     MANYLINUX_IMAGES = {
         "manylinux_2_5": MANYLINUX1_IMAGE_ID,
         "manylinux_2_12": MANYLINUX2010_IMAGE_ID,
         "manylinux_2_17": MANYLINUX2014_IMAGE_ID,
-        "manylinux_2_24": MANYLINUX_2_24_IMAGE_ID,
         "manylinux_2_28": MANYLINUX_2_28_IMAGE_ID,
     }
     POLICY_ALIASES = {
         "manylinux_2_5": ["manylinux1"],
         "manylinux_2_12": ["manylinux2010"],
         "manylinux_2_17": ["manylinux2014"],
     }
 else:
     MANYLINUX_IMAGES = {
         "manylinux_2_17": MANYLINUX2014_IMAGE_ID,
-        "manylinux_2_24": MANYLINUX_2_24_IMAGE_ID,
+        "manylinux_2_28": MANYLINUX_2_28_IMAGE_ID,
     }
-    if PLATFORM in {"aarch64", "ppc64le"}:
-        MANYLINUX_IMAGES["manylinux_2_28"] = MANYLINUX_2_28_IMAGE_ID
     POLICY_ALIASES = {
         "manylinux_2_17": ["manylinux2014"],
     }
 DOCKER_CONTAINER_NAME = "auditwheel-test-anylinux"
 PYTHON_MAJ_MIN = [str(i) for i in sys.version_info[:2]]
 PYTHON_ABI_MAJ_MIN = "".join(PYTHON_MAJ_MIN)
 PYTHON_ABI_FLAGS = "m" if sys.version_info.minor < 8 else ""
@@ -59,16 +57,15 @@
     "musllinux_1_1": f"quay.io/pypa/musllinux_1_1_{PLATFORM}:latest",
 }
 MUSLLINUX_PYTHON_IMAGE_ID = f'python:{".".join(PYTHON_MAJ_MIN)}-alpine'
 DEVTOOLSET = {
     "manylinux_2_5": "devtoolset-2",
     "manylinux_2_12": "devtoolset-8",
     "manylinux_2_17": "devtoolset-10",
-    "manylinux_2_24": "devtoolset-not-present",
-    "manylinux_2_28": "gcc-toolset-11",
+    "manylinux_2_28": "gcc-toolset-12",
     "musllinux_1_1": "devtoolset-not-present",
 }
 PATH_DIRS = [
     f"/opt/python/{PYTHON_ABI}/bin",
     "/opt/rh/{devtoolset}/root/usr/bin",
     "/usr/local/sbin",
     "/usr/local/bin",
@@ -76,19 +73,19 @@
     "/usr/bin",
     "/sbin",
     "/bin",
 ]
 PATH = {k: ":".join(PATH_DIRS).format(devtoolset=v) for k, v in DEVTOOLSET.items()}
 WHEEL_CACHE_FOLDER = op.expanduser("~/.cache/auditwheel_tests")
 NUMPY_VERSION_MAP = {
-    "36": "1.19.2",
     "37": "1.19.2",
     "38": "1.19.2",
     "39": "1.19.2",
     "310": "1.21.4",
+    "311": "1.23.4",
 }
 NUMPY_VERSION = NUMPY_VERSION_MAP[PYTHON_ABI_MAJ_MIN]
 ORIGINAL_NUMPY_WHEEL = f"numpy-{NUMPY_VERSION}-{PYTHON_ABI}-linux_{PLATFORM}.whl"
 ORIGINAL_SIX_WHEEL = "six-1.11.0-py2.py3-none-any.whl"
 SHOW_RE = re.compile(
     r'[\s](?P<wheel>\S+) is consistent with the following platform tag: "(?P<tag>\S+)"',
     flags=re.DOTALL,
@@ -202,19 +199,14 @@
 
 def build_numpy(container, policy, output_dir):
     """Helper to build numpy from source using the specified container, into
     output_dir."""
 
     if policy.startswith("musllinux_"):
         docker_exec(container, "apk add openblas-dev")
-    elif policy.startswith("manylinux_2_24_"):
-        docker_exec(container, "apt-get update")
-        docker_exec(
-            container, "apt-get install -y --no-install-recommends libatlas-dev"
-        )
     else:
         docker_exec(container, "yum install -y atlas atlas-devel")
 
     if op.exists(op.join(WHEEL_CACHE_FOLDER, policy, ORIGINAL_NUMPY_WHEEL)):
         # If numpy has already been built and put in cache, let's reuse this.
         shutil.copy2(
             op.join(WHEEL_CACHE_FOLDER, policy, ORIGINAL_NUMPY_WHEEL),
@@ -325,15 +317,14 @@
         assert "manylinux" not in orig_wheel
 
         # Exclude libgfortran from grafting into the wheel
         excludes = {
             "manylinux_2_5_x86_64": ["libgfortran.so.1", "libgfortran.so.3"],
             "manylinux_2_12_x86_64": ["libgfortran.so.3", "libgfortran.so.5"],
             "manylinux_2_17_x86_64": ["libgfortran.so.3", "libgfortran.so.5"],
-            "manylinux_2_24_x86_64": ["libgfortran.so.3"],
             "manylinux_2_28_x86_64": ["libgfortran.so.5"],
             "musllinux_1_1_x86_64": ["libgfortran.so.5"],
         }[policy]
 
         repair_command = [
             "auditwheel",
             "repair",
@@ -363,19 +354,14 @@
         self, any_manylinux_container, docker_python, io_folder
     ):
         # Test building a wheel that contains a binary executable (e.g., a program)
 
         policy, tag, manylinux_ctr = any_manylinux_container
         if policy.startswith("musllinux_"):
             docker_exec(manylinux_ctr, "apk add gsl-dev")
-        elif policy.startswith("manylinux_2_24_"):
-            docker_exec(manylinux_ctr, "apt-get update")
-            docker_exec(
-                manylinux_ctr, "apt-get install -y --no-install-recommends libgsl-dev"
-            )
         else:
             docker_exec(manylinux_ctr, "yum install -y gsl-devel")
 
         docker_exec(
             manylinux_ctr,
             [
                 "bash",
@@ -533,15 +519,14 @@
                             ]
                             assert len(rpath_tags) == 1
                             assert rpath_tags[0].rpath == "$ORIGIN/."
 
     def test_build_repair_multiple_top_level_modules_wheel(
         self, any_manylinux_container, docker_python, io_folder
     ):
-
         policy, tag, manylinux_ctr = any_manylinux_container
 
         docker_exec(
             manylinux_ctr,
             [
                 "bash",
                 "-c",
@@ -801,16 +786,22 @@
     @pytest.fixture(scope="session", params=MANYLINUX_IMAGES.keys())
     def any_manylinux_img(self, request):
         """Each manylinux image, with auditwheel installed.
 
         Plus up-to-date pip, setuptools and pytest-cov
         """
         policy = request.param
-        if policy == "manylinux_2_5" and PYTHON_ABI_MAJ_MIN in {"310"}:
-            pytest.skip(f"manylinux_2_5 images do not support cp{PYTHON_ABI_MAJ_MIN}")
+        support_check_map = {
+            "manylinux_2_5": {"37", "38", "39"},
+            "manylinux_2_12": {"37", "38", "39", "310"},
+        }
+        check_set = support_check_map.get(policy, None)
+        if check_set and PYTHON_ABI_MAJ_MIN not in check_set:
+            pytest.skip(f"{policy} images do not support cp{PYTHON_ABI_MAJ_MIN}")
+
         base = MANYLINUX_IMAGES[policy]
         env = {"PATH": PATH[policy]}
         with tmp_docker_image(
             base,
             [
                 'git config --global --add safe.directory "/auditwheel_src"',
                 "pip install -U pip setuptools pytest-cov",
```

### Comparing `auditwheel-5.3.0/tests/integration/test_nonplatform_wheel.py` & `auditwheel-5.4.0/tests/integration/test_nonplatform_wheel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
+
 import pathlib
 import subprocess
 
 import pytest
 
 HERE = pathlib.Path(__file__).parent.resolve()
 
 
 @pytest.mark.parametrize("mode", ["repair", "addtag", "show"])
 def test_non_platform_wheel_repair(mode):
     wheel = HERE / "plumbum-1.6.8-py2.py3-none-any.whl"
     proc = subprocess.run(
         ["auditwheel", mode, str(wheel)],
         stderr=subprocess.PIPE,
-        universal_newlines=True,
+        text=True,
     )
     assert proc.returncode == 1
     assert "This does not look like a platform wheel" in proc.stderr
     assert "AttributeError" not in proc.stderr
```

### Comparing `auditwheel-5.3.0/tests/integration/test_policy_files.py` & `auditwheel-5.4.0/tests/integration/test_policy_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from jsonschema import validate
 
 from auditwheel.policy import (
     POLICY_PRIORITY_HIGHEST,
     POLICY_PRIORITY_LOWEST,
     _load_policy_schema,
     load_policies,
```

### Comparing `auditwheel-5.3.0/tests/integration/testdependencies/dependency.c` & `auditwheel-5.4.0/tests/integration/testdependencies/dependency.c`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/testdependencies/setup.py` & `auditwheel-5.4.0/tests/integration/testdependencies/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 from os import getenv, path
 
 from setuptools import Extension, setup
 
 cmd = "gcc -shared -fPIC -D_GNU_SOURCE dependency.c -o libdependency.so -lm -lc"
 subprocess.check_call(cmd.split())
```

### Comparing `auditwheel-5.3.0/tests/integration/testdependencies/testdependencies.c` & `auditwheel-5.4.0/tests/integration/testdependencies/testdependencies.c`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/testpackage/testpackage/testprogram.c` & `auditwheel-5.4.0/tests/integration/testpackage/testpackage/testprogram.c`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/testrpath/setup.py` & `auditwheel-5.4.0/tests/integration/testrpath/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import subprocess
 
 from setuptools import Extension, setup
 
 cmd = "gcc -fPIC -shared -o b/libb.so b/b.c"
 subprocess.check_call(cmd.split())
```

### Comparing `auditwheel-5.3.0/tests/integration/testrpath/src/testrpath/testrpath.c` & `auditwheel-5.4.0/tests/integration/testrpath/src/testrpath/testrpath.c`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/testsimple/testsimple.c` & `auditwheel-5.4.0/tests/integration/testsimple/testsimple.c`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/integration/testzlib/testzlib.c` & `auditwheel-5.4.0/tests/integration/testzlib/testzlib.c`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/unit/test-permissions.zip.xz` & `auditwheel-5.4.0/tests/unit/test-permissions.zip.xz`

 * *Files identical despite different names*

### Comparing `auditwheel-5.3.0/tests/unit/test_condatools.py` & `auditwheel-5.4.0/tests/unit/test_condatools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest.mock import Mock, patch
 
 from auditwheel.condatools import InCondaPkg, InCondaPkgCtx
 
 
 @patch("auditwheel.condatools.tarbz2todir")
 def test_in_condapkg(tarbz2todir_mock):
```

### Comparing `auditwheel-5.3.0/tests/unit/test_elfpatcher.py` & `auditwheel-5.4.0/tests/unit/test_elfpatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from subprocess import CalledProcessError
 from unittest.mock import call, patch
 
 import pytest
 
 from auditwheel.patcher import Patchelf
```

### Comparing `auditwheel-5.3.0/tests/unit/test_elfutils.py` & `auditwheel-5.4.0/tests/unit/test_elfutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest.mock import Mock, patch
 
 import pytest
 from elftools.common.exceptions import ELFError
 
 from auditwheel.elfutils import (
     elf_file_filter,
```

### Comparing `auditwheel-5.3.0/tests/unit/test_main.py` & `auditwheel-5.4.0/tests/unit/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 
 import pytest
 
 from auditwheel.main import main
 
 on_supported_platform = pytest.mark.skipif(
```

### Comparing `auditwheel-5.3.0/tests/unit/test_musllinux.py` & `auditwheel-5.4.0/tests/unit/test_musllinux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import subprocess
 from unittest.mock import patch
 
 import pytest
 
 from auditwheel.error import InvalidLibc
 from auditwheel.musllinux import find_musl_libc, get_musl_version
```

### Comparing `auditwheel-5.3.0/tests/unit/test_policy.py` & `auditwheel-5.4.0/tests/unit/test_policy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+from __future__ import annotations
+
 from unittest.mock import patch
 
 import pytest
 
 from auditwheel.policy import (
     _validate_pep600_compliance,
     get_arch_name,
     get_policy_name,
     get_priority_by_name,
     get_replace_platforms,
+    lddtree_external_references,
 )
 
 
 @patch("auditwheel.policy._platform_module.machine")
 @patch("auditwheel.policy.bits", 32)
 @pytest.mark.parametrize(
     "reported_arch,expected_arch",
     [
         ("armv6l", "armv6l"),
         ("armv7l", "armv7l"),
+        ("armv8l", "armv7l"),
+        ("aarch64", "armv7l"),
         ("i686", "i686"),
         ("x86_64", "i686"),
     ],
 )
 def test_32bits_arch_name(machine_mock, reported_arch, expected_arch):
     machine_mock.return_value = reported_arch
     machine = get_arch_name()
@@ -29,16 +34,18 @@
 
 
 @patch("auditwheel.policy._platform_module.machine")
 @patch("auditwheel.policy.bits", 64)
 @pytest.mark.parametrize(
     "reported_arch,expected_arch",
     [
+        ("armv8l", "aarch64"),
         ("aarch64", "aarch64"),
         ("ppc64le", "ppc64le"),
+        ("i686", "x86_64"),
         ("x86_64", "x86_64"),
     ],
 )
 def test_64bits_arch_name(machine_mock, reported_arch, expected_arch):
     machine_mock.return_value = reported_arch
     machine = get_arch_name()
     assert machine == expected_arch
@@ -192,7 +199,36 @@
             {"name": "duplicate", "priority": 0},
             {"name": "duplicate", "priority": 0},
         ],
     )
     def test_get_by_name_duplicate(self):
         with pytest.raises(RuntimeError):
             get_priority_by_name("duplicate")
+
+
+class TestLddTreeExternalReferences:
+    """Tests for lddtree_external_references."""
+
+    def test_filter_libs(self):
+        """Test the nested filter_libs function."""
+        filtered_libs = [
+            "ld-linux-x86_64.so.1",
+            "ld64.so.1",
+            "ld64.so.2",
+            "libpython3.7m.so.1.0",
+            "libpython3.9.so.1.0",
+            "libpython3.10.so.1.0",
+            "libpython999.999.so.1.0",
+        ]
+        unfiltered_libs = ["libfoo.so.1.0", "libbar.so.999.999.999"]
+        libs = filtered_libs + unfiltered_libs
+
+        lddtree = {
+            "realpath": "/path/to/lib",
+            "needed": libs,
+            "libs": {lib: {"needed": [], "realpath": "/path/to/lib"} for lib in libs},
+        }
+        full_external_refs = lddtree_external_references(lddtree, "/path/to/wheel")
+
+        # Assert that each policy only has the unfiltered libs.
+        for policy in full_external_refs:
+            assert set(full_external_refs[policy]["libs"]) == set(unfiltered_libs)
```

### Comparing `auditwheel-5.3.0/tests/unit/test_repair.py` & `auditwheel-5.4.0/tests/unit/test_repair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 from unittest.mock import call, patch
 
 from auditwheel.patcher import Patchelf
 from auditwheel.repair import append_rpath_within_wheel
```

### Comparing `auditwheel-5.3.0/tests/unit/test_tmpdirs.py` & `auditwheel-5.4.0/tests/unit/test_tmpdirs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 
 from auditwheel.tmpdirs import InGivenDirectory, InTemporaryDirectory
 
 
 def test_intemporarydirectory():
     cwd = os.getcwd()
```

### Comparing `auditwheel-5.3.0/tests/unit/test_tools.py` & `auditwheel-5.4.0/tests/unit/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import lzma
 from pathlib import Path
 
 import pytest
 
 from auditwheel.tools import EnvironmentDefault, dir2zip, zip2dir
```

### Comparing `auditwheel-5.3.0/tests/unit/test_wheel_abi.py` & `auditwheel-5.4.0/tests/unit/test_wheel_abi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 
 import pretend
 import pytest
 
 from auditwheel import wheel_abi
```

