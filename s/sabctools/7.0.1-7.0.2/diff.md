# Comparing `tmp/sabctools-7.0.1.tar.gz` & `tmp/sabctools-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabctools-7.0.1.tar", last modified: Mon Apr 17 19:41:01 2023, max compression
+gzip compressed data, was "sabctools-7.0.2.tar", last modified: Mon May  1 19:23:13 2023, max compression
```

## Comparing `sabctools-7.0.1.tar` & `sabctools-7.0.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.580615 sabctools-7.0.1/
--rw-r--r--   0 runner     (501) staff       (20)    17990 2023-04-17 19:40:58.000000 sabctools-7.0.1/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       24 2023-04-17 19:40:58.000000 sabctools-7.0.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2847 2023-04-17 19:41:01.580080 sabctools-7.0.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2073 2023-04-17 19:40:58.000000 sabctools-7.0.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)       90 2023-04-17 19:40:58.000000 sabctools-7.0.1/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.519023 sabctools-7.0.1/sabctools.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2847 2023-04-17 19:41:01.000000 sabctools-7.0.1/sabctools.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2795 2023-04-17 19:41:01.000000 sabctools-7.0.1/sabctools.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-17 19:41:01.000000 sabctools-7.0.1/sabctools.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2023-04-17 19:41:01.000000 sabctools-7.0.1/sabctools.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-17 19:41:01.580751 sabctools-7.0.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)    16137 2023-04-17 19:40:58.000000 sabctools-7.0.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.524831 sabctools-7.0.1/src/
--rw-r--r--   0 runner     (501) staff       (20)      108 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2349 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crc32.cc
--rw-r--r--   0 runner     (501) staff       (20)     1132 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crc32.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.534321 sabctools-7.0.1/src/crcutil-1.0/
--rw-r--r--   0 runner     (501) staff       (20)       54 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/AUTHORS
--rw-r--r--   0 runner     (501) staff       (20)    11358 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/COPYING
--rw-r--r--   0 runner     (501) staff       (20)       58 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/ChangeLog
--rw-r--r--   0 runner     (501) staff       (20)     1700 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/INSTALL
--rw-r--r--   0 runner     (501) staff       (20)    11358 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)    50573 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/Makefile
--rw-r--r--   0 runner     (501) staff       (20)     1210 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/Makefile.am
--rw-r--r--   0 runner     (501) staff       (20)    56163 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/Makefile.in
--rw-r--r--   0 runner     (501) staff       (20)     2076 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/Makefile.win
--rw-r--r--   0 runner     (501) staff       (20)       60 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/NEWS
--rw-r--r--   0 runner     (501) staff       (20)     6669 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/README
--rw-r--r--   0 runner     (501) staff       (20)    34611 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/aclocal.m4
--rw-r--r--   0 runner     (501) staff       (20)     2785 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/autogen.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.544938 sabctools-7.0.1/src/crcutil-1.0/code/
--rw-r--r--   0 runner     (501) staff       (20)     2368 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/base_types.h
--rw-r--r--   0 runner     (501) staff       (20)    12545 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/crc32c_sse4.cc
--rw-r--r--   0 runner     (501) staff       (20)     7511 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/crc32c_sse4.h
--rw-r--r--   0 runner     (501) staff       (20)     3336 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/crc32c_sse4_intrin.h
--rw-r--r--   0 runner     (501) staff       (20)     2223 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/crc_casts.h
--rw-r--r--   0 runner     (501) staff       (20)    21506 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/generic_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     8663 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/gf_util.h
--rw-r--r--   0 runner     (501) staff       (20)     8211 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)     7459 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     8601 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
--rw-r--r--   0 runner     (501) staff       (20)     7945 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     7379 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
--rw-r--r--   0 runner     (501) staff       (20)     7264 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/platform.h
--rw-r--r--   0 runner     (501) staff       (20)     2266 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/protected_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     3417 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/rolling_crc.h
--rw-r--r--   0 runner     (501) staff       (20)     1629 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/std_headers.h
--rw-r--r--   0 runner     (501) staff       (20)     8422 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/code/uint128_sse2.h
--rw-r--r--   0 runner     (501) staff       (20)     2231 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/config.h.in
--rw-r--r--   0 runner     (501) staff       (20)   212367 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/configure
--rw-r--r--   0 runner     (501) staff       (20)      744 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/configure.ac
--rw-r--r--   0 runner     (501) staff       (20)    18615 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/depcomp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.546425 sabctools-7.0.1/src/crcutil-1.0/examples/
--rw-r--r--   0 runner     (501) staff       (20)    10449 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/examples/interface.cc
--rw-r--r--   0 runner     (501) staff       (20)     8820 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/examples/interface.h
--rw-r--r--   0 runner     (501) staff       (20)     6390 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/examples/usage.cc
--rw-r--r--   0 runner     (501) staff       (20)    13663 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/install-sh
--rw-r--r--   0 runner     (501) staff       (20)    11419 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/missing
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.549840 sabctools-7.0.1/src/crcutil-1.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)     2227 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/aligned_alloc.h
--rw-r--r--   0 runner     (501) staff       (20)     2538 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/bob_jenkins_rng.h
--rw-r--r--   0 runner     (501) staff       (20)     1915 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/rdtsc.h
--rw-r--r--   0 runner     (501) staff       (20)     1803 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/set_hi_pri.c
--rw-r--r--   0 runner     (501) staff       (20)     7593 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/unittest.cc
--rw-r--r--   0 runner     (501) staff       (20)    33870 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/unittest.h
--rw-r--r--   0 runner     (501) staff       (20)     1290 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/crcutil-1.0/tests/unittest_helper.h
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/py.typed
--rw-r--r--   0 runner     (501) staff       (20)     2950 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/sabctools.cc
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/sabctools.h
--rw-r--r--   0 runner     (501) staff       (20)      639 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/sabctools.pyi
--rw-r--r--   0 runner     (501) staff       (20)     3254 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/sparse.cc
--rw-r--r--   0 runner     (501) staff       (20)     1028 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/sparse.h
--rw-r--r--   0 runner     (501) staff       (20)     8519 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/unlocked_ssl.cc
--rw-r--r--   0 runner     (501) staff       (20)     1555 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/unlocked_ssl.h
--rw-r--r--   0 runner     (501) staff       (20)     9359 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yenc.cc
--rw-r--r--   0 runner     (501) staff       (20)     1393 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yenc.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-17 19:41:01.579201 sabctools-7.0.1/src/yencode/
--rw-r--r--   0 runner     (501) staff       (20)     9182 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2913 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/crc.cc
--rw-r--r--   0 runner     (501) staff       (20)      413 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/crc.h
--rw-r--r--   0 runner     (501) staff       (20)     7405 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/crc_arm.cc
--rw-r--r--   0 runner     (501) staff       (20)       72 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/crc_common.h
--rw-r--r--   0 runner     (501) staff       (20)    13066 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/crc_folding.cc
--rw-r--r--   0 runner     (501) staff       (20)     8230 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/crc_folding_256.cc
--rw-r--r--   0 runner     (501) staff       (20)     3620 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder.cc
--rw-r--r--   0 runner     (501) staff       (20)     2059 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder.h
--rw-r--r--   0 runner     (501) staff       (20)      754 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_avx.cc
--rw-r--r--   0 runner     (501) staff       (20)      771 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_avx2.cc
--rw-r--r--   0 runner     (501) staff       (20)    31441 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_avx2_base.h
--rw-r--r--   0 runner     (501) staff       (20)    18596 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_common.h
--rw-r--r--   0 runner     (501) staff       (20)    21692 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_neon.cc
--rw-r--r--   0 runner     (501) staff       (20)    22632 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_neon64.cc
--rw-r--r--   0 runner     (501) staff       (20)      644 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)    33901 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_sse_base.h
--rw-r--r--   0 runner     (501) staff       (20)      713 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_ssse3.cc
--rw-r--r--   0 runner     (501) staff       (20)     1429 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/decoder_vbmi2.cc
--rw-r--r--   0 runner     (501) staff       (20)     5383 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder.cc
--rw-r--r--   0 runner     (501) staff       (20)      331 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder.h
--rw-r--r--   0 runner     (501) staff       (20)      342 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_avx.cc
--rw-r--r--   0 runner     (501) staff       (20)      339 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_avx2.cc
--rw-r--r--   0 runner     (501) staff       (20)    26195 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_avx_base.h
--rw-r--r--   0 runner     (501) staff       (20)     3833 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_common.h
--rw-r--r--   0 runner     (501) staff       (20)    21944 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_neon.cc
--rw-r--r--   0 runner     (501) staff       (20)      247 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_sse2.cc
--rw-r--r--   0 runner     (501) staff       (20)    31590 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_sse_base.h
--rw-r--r--   0 runner     (501) staff       (20)      675 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_ssse3.cc
--rw-r--r--   0 runner     (501) staff       (20)      583 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/encoder_vbmi2.cc
--rw-r--r--   0 runner     (501) staff       (20)    72124 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/hedley.h
--rw-r--r--   0 runner     (501) staff       (20)     6010 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/platform.cc
--rw-r--r--   0 runner     (501) staff       (20)     7722 2023-04-17 19:40:58.000000 sabctools-7.0.1/src/yencode/stdint.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.517320 sabctools-7.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    17990 2023-05-01 19:23:12.000000 sabctools-7.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 19:23:12.000000 sabctools-7.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 19:23:13.517320 sabctools-7.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-01 19:23:12.000000 sabctools-7.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 19:23:12.000000 sabctools-7.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.509319 sabctools-7.0.2/sabctools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 19:23:13.000000 sabctools-7.0.2/sabctools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-01 19:23:13.000000 sabctools-7.0.2/sabctools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:23:13.000000 sabctools-7.0.2/sabctools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 19:23:13.000000 sabctools-7.0.2/sabctools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:23:13.517320 sabctools-7.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-01 19:23:12.000000 sabctools-7.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.509319 sabctools-7.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crc32.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crc32.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.513320 sabctools-7.0.2/src/crcutil-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50573 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)    56163 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/Makefile.win
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/README
+-rw-r--r--   0 runner    (1001) docker     (123)    34611 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/aclocal.m4
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/autogen.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.513320 sabctools-7.0.2/src/crcutil-1.0/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/base_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/crc32c_sse4.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/crc32c_sse4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/crc32c_sse4_intrin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/crc_casts.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/generic_crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/gf_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/platform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/protected_crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/rolling_crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/std_headers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/code/uint128_sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)   212367 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/configure
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (123)    18615 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/depcomp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.513320 sabctools-7.0.2/src/crcutil-1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/examples/interface.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/examples/interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/examples/usage.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/install-sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/missing
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.513320 sabctools-7.0.2/src/crcutil-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/aligned_alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/bob_jenkins_rng.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/rdtsc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/set_hi_pri.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/unittest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    33870 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/unittest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/crcutil-1.0/tests/unittest_helper.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/sabctools.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/sabctools.h
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/sabctools.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/sparse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/sparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/unlocked_ssl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/unlocked_ssl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yenc.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yenc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:23:13.517320 sabctools-7.0.2/src/yencode/
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/crc.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/crc_arm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/crc_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13066 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/crc_folding.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/crc_folding_256.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_avx.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_avx2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_avx2_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_neon.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_neon64.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_sse2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    33901 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_sse_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_ssse3.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/decoder_vbmi2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_avx.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_avx2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26195 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_avx_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21944 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_neon.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_sse2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31590 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_sse_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_ssse3.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/encoder_vbmi2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    72124 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/hedley.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/platform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-01 19:23:12.000000 sabctools-7.0.2/src/yencode/stdint.h
```

### Comparing `sabctools-7.0.1/LICENSE.md` & `sabctools-7.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/PKG-INFO` & `sabctools-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 7.0.1
+Version: 7.0.2
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-7.0.1/README.md` & `sabctools-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/sabctools.egg-info/PKG-INFO` & `sabctools-7.0.2/sabctools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabctools
-Version: 7.0.1
+Version: 7.0.2
 Summary: C implementations of functions for use within SABnzbd
 Home-page: https://github.com/sabnzbd/sabctools/
 Author: Safihre
 Author-email: safihre@sabnzbd.org
 License: GPLv2+
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sabctools-7.0.1/sabctools.egg-info/SOURCES.txt` & `sabctools-7.0.2/sabctools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/setup.py` & `sabctools-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crc32.cc` & `sabctools-7.0.2/src/crc32.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crc32.h` & `sabctools-7.0.2/src/crc32.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/COPYING` & `sabctools-7.0.2/src/crcutil-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/INSTALL` & `sabctools-7.0.2/src/crcutil-1.0/INSTALL`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/LICENSE` & `sabctools-7.0.2/src/crcutil-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/Makefile` & `sabctools-7.0.2/src/crcutil-1.0/Makefile`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/Makefile.am` & `sabctools-7.0.2/src/crcutil-1.0/Makefile.am`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/Makefile.in` & `sabctools-7.0.2/src/crcutil-1.0/Makefile.in`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/Makefile.win` & `sabctools-7.0.2/src/crcutil-1.0/Makefile.win`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/README` & `sabctools-7.0.2/src/crcutil-1.0/README`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/aclocal.m4` & `sabctools-7.0.2/src/crcutil-1.0/aclocal.m4`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/autogen.sh` & `sabctools-7.0.2/src/crcutil-1.0/autogen.sh`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/base_types.h` & `sabctools-7.0.2/src/crcutil-1.0/code/base_types.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/crc32c_sse4.cc` & `sabctools-7.0.2/src/crcutil-1.0/code/crc32c_sse4.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/crc32c_sse4.h` & `sabctools-7.0.2/src/crcutil-1.0/code/crc32c_sse4.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/crc32c_sse4_intrin.h` & `sabctools-7.0.2/src/crcutil-1.0/code/crc32c_sse4_intrin.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/crc_casts.h` & `sabctools-7.0.2/src/crcutil-1.0/code/crc_casts.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/generic_crc.h` & `sabctools-7.0.2/src/crcutil-1.0/code/generic_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/gf_util.h` & `sabctools-7.0.2/src/crcutil-1.0/code/gf_util.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc` & `sabctools-7.0.2/src/crcutil-1.0/code/multiword_128_64_gcc_amd64_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc` & `sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_cl_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc` & `sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_gcc_amd64_asm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc` & `sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_gcc_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc` & `sabctools-7.0.2/src/crcutil-1.0/code/multiword_64_64_intrinsic_i386_mmx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/platform.h` & `sabctools-7.0.2/src/crcutil-1.0/code/platform.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/protected_crc.h` & `sabctools-7.0.2/src/crcutil-1.0/code/protected_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/rolling_crc.h` & `sabctools-7.0.2/src/crcutil-1.0/code/rolling_crc.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/std_headers.h` & `sabctools-7.0.2/src/crcutil-1.0/code/std_headers.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/code/uint128_sse2.h` & `sabctools-7.0.2/src/crcutil-1.0/code/uint128_sse2.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/config.h.in` & `sabctools-7.0.2/src/crcutil-1.0/config.h.in`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/configure` & `sabctools-7.0.2/src/crcutil-1.0/configure`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/configure.ac` & `sabctools-7.0.2/src/crcutil-1.0/configure.ac`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/depcomp` & `sabctools-7.0.2/src/crcutil-1.0/depcomp`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/examples/interface.cc` & `sabctools-7.0.2/src/crcutil-1.0/examples/interface.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/examples/interface.h` & `sabctools-7.0.2/src/crcutil-1.0/examples/interface.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/examples/usage.cc` & `sabctools-7.0.2/src/crcutil-1.0/examples/usage.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/install-sh` & `sabctools-7.0.2/src/crcutil-1.0/install-sh`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/missing` & `sabctools-7.0.2/src/crcutil-1.0/missing`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/aligned_alloc.h` & `sabctools-7.0.2/src/crcutil-1.0/tests/aligned_alloc.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/bob_jenkins_rng.h` & `sabctools-7.0.2/src/crcutil-1.0/tests/bob_jenkins_rng.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/rdtsc.h` & `sabctools-7.0.2/src/crcutil-1.0/tests/rdtsc.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/set_hi_pri.c` & `sabctools-7.0.2/src/crcutil-1.0/tests/set_hi_pri.c`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/unittest.cc` & `sabctools-7.0.2/src/crcutil-1.0/tests/unittest.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/unittest.h` & `sabctools-7.0.2/src/crcutil-1.0/tests/unittest.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/crcutil-1.0/tests/unittest_helper.h` & `sabctools-7.0.2/src/crcutil-1.0/tests/unittest_helper.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/sabctools.cc` & `sabctools-7.0.2/src/sabctools.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/sabctools.h` & `sabctools-7.0.2/src/sabctools.h`

 * *Files 9% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 
 #include <Python.h>
 #include <stdio.h>
 #include <fcntl.h>
 #include <string.h>
 
 /* Version information */
-#define SABCTOOLS_VERSION "7.0.1"
+#define SABCTOOLS_VERSION "7.0.2"
 
 PyMODINIT_FUNC PyInit_sabctools(void);
```

### Comparing `sabctools-7.0.1/src/sabctools.pyi` & `sabctools-7.0.2/src/sabctools.pyi`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/sparse.cc` & `sabctools-7.0.2/src/sparse.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/sparse.h` & `sabctools-7.0.2/src/sparse.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/unlocked_ssl.cc` & `sabctools-7.0.2/src/unlocked_ssl.cc`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  * You should have received a copy of the GNU General Public License
  * along with this program; if not, write to the Free Software
  * Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
  */
 
 #include "unlocked_ssl.h"
 
-static int (SABCTOOLS_DLL_CALL *SSL_read_ex)(void*, void*, size_t, size_t*) = NULL;
-static int (SABCTOOLS_DLL_CALL *SSL_get_error)(void*, int) = NULL;
-static int (SABCTOOLS_DLL_CALL *SSL_get_shutdown)(void*) = NULL;
+static int (*SSL_read_ex)(void*, void*, size_t, size_t*) = NULL;
+static int (*SSL_get_error)(void*, int) = NULL;
+static int (*SSL_get_shutdown)(void*) = NULL;
 static PyObject *SSLWantReadError = NULL;
 static PyObject *SSLSocketType = NULL;
 
 typedef struct {
     int ssl; /* last seen error from SSL */
     int c; /* last seen error from libc */
 #ifdef MS_WINDOWS
```

### Comparing `sabctools-7.0.1/src/unlocked_ssl.h` & `sabctools-7.0.2/src/unlocked_ssl.h`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,18 @@
 #include <Python.h>
 #include <stdio.h>
 #include <fcntl.h>
 #include <string.h>
 
 /* OpenSSL link */
 #if defined(_WIN32) || defined(__CYGWIN__)
-# define SABCTOOLS_DLL_CALL __stdcall
 # define WIN32_LEAN_AND_MEAN
 # include <Windows.h>
 # include <winsock2.h>
 #else
-# define SABCTOOLS_DLL_CALL
 # include <dlfcn.h>
 #endif
 
 #ifdef __cplusplus
 extern "C" {
 #endif
```

### Comparing `sabctools-7.0.1/src/yenc.cc` & `sabctools-7.0.2/src/yenc.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yenc.h` & `sabctools-7.0.2/src/yenc.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/common.h` & `sabctools-7.0.2/src/yencode/common.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/crc.cc` & `sabctools-7.0.2/src/yencode/crc.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/crc_arm.cc` & `sabctools-7.0.2/src/yencode/crc_arm.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/crc_folding.cc` & `sabctools-7.0.2/src/yencode/crc_folding.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/crc_folding_256.cc` & `sabctools-7.0.2/src/yencode/crc_folding_256.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder.cc` & `sabctools-7.0.2/src/yencode/decoder.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder.h` & `sabctools-7.0.2/src/yencode/decoder.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_avx.cc` & `sabctools-7.0.2/src/yencode/decoder_avx.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_avx2.cc` & `sabctools-7.0.2/src/yencode/decoder_avx2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_avx2_base.h` & `sabctools-7.0.2/src/yencode/decoder_avx2_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_common.h` & `sabctools-7.0.2/src/yencode/decoder_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_neon.cc` & `sabctools-7.0.2/src/yencode/decoder_neon.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_neon64.cc` & `sabctools-7.0.2/src/yencode/decoder_neon64.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_sse2.cc` & `sabctools-7.0.2/src/yencode/decoder_sse2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_sse_base.h` & `sabctools-7.0.2/src/yencode/decoder_sse_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_ssse3.cc` & `sabctools-7.0.2/src/yencode/decoder_ssse3.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/decoder_vbmi2.cc` & `sabctools-7.0.2/src/yencode/decoder_vbmi2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder.cc` & `sabctools-7.0.2/src/yencode/encoder.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder_avx_base.h` & `sabctools-7.0.2/src/yencode/encoder_avx_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder_common.h` & `sabctools-7.0.2/src/yencode/encoder_common.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder_neon.cc` & `sabctools-7.0.2/src/yencode/encoder_neon.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder_sse_base.h` & `sabctools-7.0.2/src/yencode/encoder_sse_base.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder_ssse3.cc` & `sabctools-7.0.2/src/yencode/encoder_ssse3.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/encoder_vbmi2.cc` & `sabctools-7.0.2/src/yencode/encoder_vbmi2.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/hedley.h` & `sabctools-7.0.2/src/yencode/hedley.h`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/platform.cc` & `sabctools-7.0.2/src/yencode/platform.cc`

 * *Files identical despite different names*

### Comparing `sabctools-7.0.1/src/yencode/stdint.h` & `sabctools-7.0.2/src/yencode/stdint.h`

 * *Files identical despite different names*

