# Comparing `tmp/numpy-flint-0.2.3.tar.gz` & `tmp/numpy-flint-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy-flint-0.2.3.tar", last modified: Wed Apr  5 02:36:15 2023, max compression
+gzip compressed data, was "numpy-flint-0.2.4.tar", last modified: Sun Apr 30 22:18:35 2023, max compression
```

## Comparing `numpy-flint-0.2.3.tar` & `numpy-flint-0.2.4.tar`

### file list

```diff
@@ -1,120 +1,145 @@
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.162395 numpy-flint-0.2.3/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.099395 numpy-flint-0.2.3/.venv/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.099395 numpy-flint-0.2.3/.venv/lib/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.100396 numpy-flint-0.2.3/.venv/lib/python3.9/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.100396 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.107396 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/
--rw-r--r--   0 jef       (1000) jef       (1000)     3908 2023-04-04 22:13:40.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h
--rw-r--r--   0 jef       (1000) jef       (1000)    14800 2023-04-04 22:13:40.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h
--rw-r--r--   0 jef       (1000) jef       (1000)    17680 2023-04-04 22:13:40.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/_embedding.h
--rw-r--r--   0 jef       (1000) jef       (1000)     5976 2023-04-04 22:13:40.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.102395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.101395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.100396 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.128395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/
--rw-r--r--   0 jef       (1000) jef       (1000)    62712 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)    12614 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1877 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h
--rw-r--r--   0 jef       (1000) jef       (1000)      971 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h
--rw-r--r--   0 jef       (1000) jef       (1000)      282 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h
--rw-r--r--   0 jef       (1000) jef       (1000)     3818 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h
--rw-r--r--   0 jef       (1000) jef       (1000)    19943 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1959 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.130396 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/
--rw-r--r--   0 jef       (1000) jef       (1000)    80138 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h
--rw-r--r--   0 jef       (1000) jef       (1000)    10191 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h
--rw-r--r--   0 jef       (1000) jef       (1000)    68688 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h
--rw-r--r--   0 jef       (1000) jef       (1000)     6830 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h
--rw-r--r--   0 jef       (1000) jef       (1000)     4327 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)    15990 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h
--rw-r--r--   0 jef       (1000) jef       (1000)    39015 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h
--rw-r--r--   0 jef       (1000) jef       (1000)     4603 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h
--rw-r--r--   0 jef       (1000) jef       (1000)     2786 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1948 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h
--rw-r--r--   0 jef       (1000) jef       (1000)    19874 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h
--rw-r--r--   0 jef       (1000) jef       (1000)      678 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1120 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h
--rw-r--r--   0 jef       (1000) jef       (1000)     2943 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h
--rw-r--r--   0 jef       (1000) jef       (1000)     6405 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h
--rw-r--r--   0 jef       (1000) jef       (1000)      899 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.132395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/
--rw-r--r--   0 jef       (1000) jef       (1000)      488 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/bitgen.h
--rw-r--r--   0 jef       (1000) jef       (1000)     9865 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h
--rw-r--r--   0 jef       (1000) jef       (1000)    11895 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1185 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.101395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/tests/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.101395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.133396 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/
--rw-r--r--   0 jef       (1000) jef       (1000)      344 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/limited_api.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.102395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.152395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/
--rw-r--r--   0 jef       (1000) jef       (1000)      818 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c
--rw-r--r--   0 jef       (1000) jef       (1000)      432 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimddp.c
--rw-r--r--   0 jef       (1000) jef       (1000)      529 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c
--rw-r--r--   0 jef       (1000) jef       (1000)      379 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdhp.c
--rw-r--r--   0 jef       (1000) jef       (1000)      779 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      749 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      842 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      948 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1004 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c
--rw-r--r--   0 jef       (1000) jef       (1000)      956 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1132 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1010 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      759 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c
--rw-r--r--   0 jef       (1000) jef       (1000)      755 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c
--rw-r--r--   0 jef       (1000) jef       (1000)      868 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c
--rw-r--r--   0 jef       (1000) jef       (1000)      817 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      301 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma4.c
--rw-r--r--   0 jef       (1000) jef       (1000)      600 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c
--rw-r--r--   0 jef       (1000) jef       (1000)      251 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_fp16.c
--rw-r--r--   0 jef       (1000) jef       (1000)      609 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1049 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c
--rw-r--r--   0 jef       (1000) jef       (1000)      686 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c
--rw-r--r--   0 jef       (1000) jef       (1000)      697 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      689 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      675 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c
--rw-r--r--   0 jef       (1000) jef       (1000)      692 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c
--rw-r--r--   0 jef       (1000) jef       (1000)      705 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      478 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      263 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      250 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      305 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx4.c
--rw-r--r--   0 jef       (1000) jef       (1000)      461 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      788 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c
--rw-r--r--   0 jef       (1000) jef       (1000)      624 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      234 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_xop.c
--rw-r--r--   0 jef       (1000) jef       (1000)      636 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c
--rw-r--r--   0 jef       (1000) jef       (1000)      504 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512dq_mask.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1595 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c
--rw-r--r--   0 jef       (1000) jef       (1000)      499 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx4_mma.c
--rw-r--r--   0 jef       (1000) jef       (1000)      945 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c
--rw-r--r--   0 jef       (1000) jef       (1000)       16 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/test_flags.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.152395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/
--rw-r--r--   0 jef       (1000) jef       (1000)       77 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/gfortran_vs2003_hack.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.102395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.154395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/src/
--rw-r--r--   0 jef       (1000) jef       (1000)    46010 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c
--rw-r--r--   0 jef       (1000) jef       (1000)     5835 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.102395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/tests/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.102395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.154395 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/
--rw-r--r--   0 jef       (1000) jef       (1000)     7299 2023-04-02 14:57:18.000000 numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c
--rw-r--r--   0 jef       (1000) jef       (1000)      852 2023-04-02 17:20:31.000000 numpy-flint-0.2.3/MANIFEST.in
--rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-04-05 02:36:15.162395 numpy-flint-0.2.3/PKG-INFO
--rw-r--r--   0 jef       (1000) jef       (1000)     7642 2023-04-02 14:09:32.000000 numpy-flint-0.2.3/copying.lesser.md
--rw-r--r--   0 jef       (1000) jef       (1000)    34916 2023-04-02 14:09:32.000000 numpy-flint-0.2.3/copying.md
--rw-r--r--   0 jef       (1000) jef       (1000)     1507 2023-04-05 00:16:10.000000 numpy-flint-0.2.3/pyproject.toml
--rw-r--r--   0 jef       (1000) jef       (1000)    12282 2023-04-05 01:28:05.000000 numpy-flint-0.2.3/readme.md
--rw-r--r--   0 jef       (1000) jef       (1000)       38 2023-04-05 02:36:15.163396 numpy-flint-0.2.3/setup.cfg
--rw-r--r--   0 jef       (1000) jef       (1000)     1540 2023-04-03 01:00:19.000000 numpy-flint-0.2.3/setup.py
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.156396 numpy-flint-0.2.3/src/
--rw-r--r--   0 jef       (1000) jef       (1000)    36625 2023-04-04 21:55:07.000000 numpy-flint-0.2.3/src/flint.h
--rw-r--r--   0 jef       (1000) jef       (1000)    61811 2023-04-02 15:08:26.000000 numpy-flint-0.2.3/src/numpy_flint.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.160395 numpy-flint-0.2.3/src/numpy_flint.egg-info/
--rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-04-05 02:36:14.000000 numpy-flint-0.2.3/src/numpy_flint.egg-info/PKG-INFO
--rw-r--r--   0 jef       (1000) jef       (1000)     5908 2023-04-05 02:36:15.000000 numpy-flint-0.2.3/src/numpy_flint.egg-info/SOURCES.txt
--rw-r--r--   0 jef       (1000) jef       (1000)        1 2023-04-05 02:36:14.000000 numpy-flint-0.2.3/src/numpy_flint.egg-info/dependency_links.txt
--rw-r--r--   0 jef       (1000) jef       (1000)       12 2023-04-05 02:36:14.000000 numpy-flint-0.2.3/src/numpy_flint.egg-info/requires.txt
--rw-r--r--   0 jef       (1000) jef       (1000)        6 2023-04-05 02:36:14.000000 numpy-flint-0.2.3/src/numpy_flint.egg-info/top_level.txt
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-05 02:36:15.161395 numpy-flint-0.2.3/tests/
--rw-r--r--   0 jef       (1000) jef       (1000)    27588 2023-04-04 21:55:07.000000 numpy-flint-0.2.3/tests/test_flint.py
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.892894 numpy-flint-0.2.4/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.797894 numpy-flint-0.2.4/.venv/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.797894 numpy-flint-0.2.4/.venv/lib/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.798894 numpy-flint-0.2.4/.venv/lib/python3.9/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.807894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.816894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/
+-rw-r--r--   0 jef       (1000) jef       (1000)     3908 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    14800 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    17680 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_embedding.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     5976 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.799894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.799894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.800894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.817894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/
+-rw-r--r--   0 jef       (1000) jef       (1000)  2138822 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_cython.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.825894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/
+-rw-r--r--   0 jef       (1000) jef       (1000)   956390 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c
+-rw-r--r--   0 jef       (1000) jef       (1000)       84 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/release_mem.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.801894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.825894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/
+-rw-r--r--   0 jef       (1000) jef       (1000)    22335 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/python.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.828894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/
+-rw-r--r--   0 jef       (1000) jef       (1000)     1902 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/attach.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1198 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/stdafx.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1035 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/targetver.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.805894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.803894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.802894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.845894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/
+-rw-r--r--   0 jef       (1000) jef       (1000)    62712 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    12614 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1877 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      971 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      282 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     3818 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    19943 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1959 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.845894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/
+-rw-r--r--   0 jef       (1000) jef       (1000)    80138 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    10191 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    68688 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     6830 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     4327 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    15990 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    39015 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     4603 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     2786 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1948 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    19874 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      678 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1120 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     2943 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     6405 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      899 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.847894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/
+-rw-r--r--   0 jef       (1000) jef       (1000)      488 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/bitgen.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     9865 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    11895 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1185 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.803894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.803894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.847894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/
+-rw-r--r--   0 jef       (1000) jef       (1000)      344 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/limited_api.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.804894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.876894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/
+-rw-r--r--   0 jef       (1000) jef       (1000)      818 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      432 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimddp.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      529 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      379 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdhp.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      779 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      749 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      842 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      948 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1004 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      956 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1132 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1010 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      759 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      755 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      868 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      817 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      301 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma4.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      600 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      251 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_fp16.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      609 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1049 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      686 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      697 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      689 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      675 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      692 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      705 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      478 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      263 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      250 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      305 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx4.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      461 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      788 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      624 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      234 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_xop.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      636 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      504 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512dq_mask.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1595 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      499 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx4_mma.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      945 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c
+-rw-r--r--   0 jef       (1000) jef       (1000)       16 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/test_flags.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.877894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/
+-rw-r--r--   0 jef       (1000) jef       (1000)       77 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/gfortran_vs2003_hack.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.805894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.879894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/
+-rw-r--r--   0 jef       (1000) jef       (1000)    46010 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     5835 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.806894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.806894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.880894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/
+-rw-r--r--   0 jef       (1000) jef       (1000)     7299 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.808894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.808894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.880894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/cffi/
+-rw-r--r--   0 jef       (1000) jef       (1000)     2623 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/cffi/_cdefs.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.884894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/
+-rw-r--r--   0 jef       (1000) jef       (1000)      116 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/getpid_compat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      522 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1625 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/mutex.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      284 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/pyversion_compat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     3184 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/zmq_compat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      852 2023-04-02 17:20:31.000000 numpy-flint-0.2.4/MANIFEST.in
+-rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-04-30 22:18:35.891894 numpy-flint-0.2.4/PKG-INFO
+-rw-r--r--   0 jef       (1000) jef       (1000)     7642 2023-04-02 14:09:32.000000 numpy-flint-0.2.4/copying.lesser.md
+-rw-r--r--   0 jef       (1000) jef       (1000)    34916 2023-04-02 14:09:32.000000 numpy-flint-0.2.4/copying.md
+-rw-r--r--   0 jef       (1000) jef       (1000)     1507 2023-04-30 19:41:17.000000 numpy-flint-0.2.4/pyproject.toml
+-rw-r--r--   0 jef       (1000) jef       (1000)    12282 2023-04-05 01:28:05.000000 numpy-flint-0.2.4/readme.md
+-rw-r--r--   0 jef       (1000) jef       (1000)       38 2023-04-30 22:18:35.892894 numpy-flint-0.2.4/setup.cfg
+-rw-r--r--   0 jef       (1000) jef       (1000)     1540 2023-04-03 01:00:19.000000 numpy-flint-0.2.4/setup.py
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.886894 numpy-flint-0.2.4/src/
+-rw-r--r--   0 jef       (1000) jef       (1000)    36625 2023-04-04 21:55:07.000000 numpy-flint-0.2.4/src/flint.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    61889 2023-04-30 18:58:53.000000 numpy-flint-0.2.4/src/numpy_flint.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.890894 numpy-flint-0.2.4/src/numpy_flint.egg-info/
+-rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/PKG-INFO
+-rw-r--r--   0 jef       (1000) jef       (1000)     6947 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/SOURCES.txt
+-rw-r--r--   0 jef       (1000) jef       (1000)        1 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/dependency_links.txt
+-rw-r--r--   0 jef       (1000) jef       (1000)       12 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/requires.txt
+-rw-r--r--   0 jef       (1000) jef       (1000)        6 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/top_level.txt
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.891894 numpy-flint-0.2.4/tests/
+-rw-r--r--   0 jef       (1000) jef       (1000)    30312 2023-04-30 19:40:38.000000 numpy-flint-0.2.4/tests/test_flint.py
```

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/_embedding.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_embedding.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c` & `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/MANIFEST.in` & `numpy-flint-0.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/PKG-INFO` & `numpy-flint-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-flint
-Version: 0.2.3
+Version: 0.2.4
 Summary: Add a rounded floating point interval (flint) dtype to NumPy
 Author-email: Jef Wagner <jefwagner@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: copying.lesser.md
 License-File: copying.md
```

### Comparing `numpy-flint-0.2.3/copying.lesser.md` & `numpy-flint-0.2.4/copying.lesser.md`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/copying.md` & `numpy-flint-0.2.4/copying.md`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/pyproject.toml` & `numpy-flint-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [build-system]
 requires = ["setuptools>=59", "oldest-supported-numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numpy-flint"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{name="Jef Wagner", email="jefwagner@gmail.com"}]
 readme = "readme.md"
 # license = "LGPL-3.0-or-later"
 requires-python = ">=3.7"
 dependencies = ["numpy>=1.17"]
 description = "Add a rounded floating point interval (flint) dtype to NumPy"
```

### Comparing `numpy-flint-0.2.3/readme.md` & `numpy-flint-0.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/setup.py` & `numpy-flint-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/src/flint.h` & `numpy-flint-0.2.4/src/flint.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.3/src/numpy_flint.c` & `numpy-flint-0.2.4/src/numpy_flint.c`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,16 @@
 /// @brief The __setstate__ reads in the data as pickled by __getstate__
 /// @param args A Tuple of object members a PyObjects and a setstate flag
 /// @return NULL on failure or None on success, The value of the `self` is 
 ///         set from the values read in from the args tuple 
 static PyObject* pyflint_setstate(PyObject* self, PyObject* args) {
     flint *f;
     f = &(((PyFlint*) self)->obval);
-    if (PyArg_ParseTuple(args, "ddd:setstate", &(f->a), &(f->b), &(f->v))) {
+    if (!PyArg_ParseTuple(args, "(ddd):setstate", &(f->a), &(f->b), &(f->v))) {
+        PyErr_SetString(PyExc_ValueError, "Could not unpack state tuple");
         return NULL;
     }
     Py_INCREF(Py_None);
     return Py_None;
 }
 
 // ------------------------------------
@@ -925,17 +926,17 @@
     if (dstride == sizeof(flint) && sstride == sizeof(flint)) {
         descr->f->copyswapn(dst, sizeof(double), src, sizeof(double), 
                             n*sizeof(flint)/sizeof(double), swap, arr);
     } else {
         // Else we make a call for each double in the struct
         descr->f->copyswapn(&(_dst->a), dstride, &(_src->a), sstride, 
                             n, swap, arr);
-        descr->f->copyswapn(&(_dst->b), dstride, &(_src->a), sstride, 
+        descr->f->copyswapn(&(_dst->b), dstride, &(_src->b), sstride, 
                             n, swap, arr);
-        descr->f->copyswapn(&(_dst->v), dstride, &(_src->a), sstride, 
+        descr->f->copyswapn(&(_dst->v), dstride, &(_src->v), sstride, 
                             n, swap, arr);
     }
     Py_DECREF(descr);
 }
 
 /// @brief Check if an element of a numpy array is zero
 /// @param data a pointer to the element in a numpy array
```

### Comparing `numpy-flint-0.2.3/src/numpy_flint.egg-info/PKG-INFO` & `numpy-flint-0.2.4/src/numpy_flint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-flint
-Version: 0.2.3
+Version: 0.2.4
 Summary: Add a rounded floating point interval (flint) dtype to NumPy
 Author-email: Jef Wagner <jefwagner@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: copying.lesser.md
 License-File: copying.md
```

### Comparing `numpy-flint-0.2.3/tests/test_flint.py` & `numpy-flint-0.2.4/tests/test_flint.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,14 +85,47 @@
         self.assertEqual(2, x.b)
         self.assertEqual(1.5, x.v)
         x.interval = 1, 2, 1.75
         self.assertEqual(1, x.a)
         self.assertEqual(2, x.b)
         self.assertEqual(1.75, x.v)
 
+class TestState:
+
+    def test_getstate(self):
+        x = flint(1.5)
+        x.interval = 1,2
+        state = x.__getstate__()
+        assert isinstance(state, tuple)
+        assert len(state) == 3
+        assert state[0] == x.a
+        assert state[1] == x.b
+        assert state[2] == x.v
+
+    def test_setstate(self):
+        x = flint(0)
+        x.__setstate__((1.0, 2.0, 1.5))
+        assert x.a == 1.0
+        assert x.b == 2.0
+        assert x.v == 1.5
+
+    def test_reduce(self):
+        x = flint(1.5)
+        x.interval = 1,2
+        r = x.__reduce__()
+        assert isinstance(r, tuple)
+        assert len(r) == 2
+        assert isinstance(r[0], type)
+        assert r[0] == type(x)
+        assert isinstance(r[1], tuple)
+        assert len(r[1]) == 3
+        assert r[1][0] == x.a
+        assert r[1][1] == x.b
+        assert r[1][2] == x.v
+
 
 class TestFloatSpecialValues(unittest.TestCase):
     """Test the query functions for the float special value checks"""
 
     def test_nonzero(self):
         """Validate 0"""
         x = flint(0)
@@ -906,7 +939,65 @@
         self.assertTrue(np.isnan(y.b))
         self.assertTrue(np.isnan(y.v))
         x = flint(1.1)
         y = np.arctanh(x)
         self.assertTrue(np.isnan(y.a))
         self.assertTrue(np.isnan(y.b))
         self.assertTrue(np.isnan(y.v))
+
+
+class TestNumpyArray():
+
+    def test_array(self):
+        a = np.array([1], dtype=flint)
+        assert isinstance(a, np.ndarray)
+        assert a.dtype == flint
+        assert isinstance(a[0], flint)
+        assert a[0].a == np.nextafter(1,-np.inf)
+        assert a[0].b == np.nextafter(1, np.inf)
+        assert a[0].v == 1.0
+
+    def test_zeros(self):
+        a = np.zeros((1,), dtype=flint)
+        assert isinstance(a, np.ndarray)
+        assert a.dtype == flint
+        assert isinstance(a[0], flint)
+        assert a[0].a == 0.0
+        assert a[0].b == 0.0
+        assert a[0].v == 0.0
+
+    def test_fill(self):
+        x = flint(1.5)
+        x.interval = 1,2
+        a = np.full((3,4), x, dtype=flint)
+        assert isinstance(a, np.ndarray)
+        assert a.dtype == flint
+        for val in np.nditer(a):
+            item = val.item()
+            assert isinstance(item, flint)
+            assert item.a == x.a
+            assert item.b == x.b
+            assert item.v == x.v
+
+    def test_copy_row(self):
+        a = np.zeros((3,3), dtype=flint)
+        b = np.arange(1,4, dtype=flint)
+        zero_row = np.zeros((3,))
+        assert np.alltrue( a[0] == zero_row )
+        assert np.alltrue( a[1] == zero_row )
+        assert np.alltrue( a[2] == zero_row )
+        a[1] = b
+        assert np.alltrue( a[0] == zero_row )
+        assert np.alltrue( a[1] == b )
+        assert np.alltrue( a[2] == zero_row )
+
+    def test_copy_col(self):
+        a = np.zeros((3,3), dtype=flint)
+        b = np.arange(1,4, dtype=flint)
+        zero_row = np.zeros((3,))
+        assert np.alltrue( a[:,0] == zero_row )
+        assert np.alltrue( a[:,1] == zero_row )
+        assert np.alltrue( a[:,2] == zero_row )
+        a[:,1] = b
+        assert np.alltrue( a[:,0] == zero_row )
+        assert np.alltrue( a[:,1] == b )
+        assert np.alltrue( a[:,2] == zero_row )
```

