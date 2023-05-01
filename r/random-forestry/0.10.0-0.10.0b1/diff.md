# Comparing `tmp/random-forestry-0.10.0.tar.gz` & `tmp/random-forestry-0.10.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random-forestry-0.10.0.tar", last modified: Mon May  1 14:32:24 2023, max compression
+gzip compressed data, was "random-forestry-0.10.0b1.tar", last modified: Fri Mar 31 02:43:04 2023, max compression
```

## Comparing `random-forestry-0.10.0.tar` & `random-forestry-0.10.0b1.tar`

### file list

```diff
@@ -1,742 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.034510 random-forestry-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-01 14:31:58.000000 random-forestry-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 14:31:58.000000 random-forestry-0.10.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-01 14:32:24.034510 random-forestry-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-01 14:31:58.000000 random-forestry-0.10.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.894507 random-forestry-0.10.0/extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 14:31:58.000000 random-forestry-0.10.0/extension/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.894507 random-forestry-0.10.0/extension/armadillo/
--rw-r--r--   0 runner    (1001) docker     (123)    25518 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.890507 random-forestry-0.10.0/extension/armadillo/cmake_aux/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.894507 random-forestry-0.10.0/extension/armadillo/cmake_aux/InstallFiles/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/InstallFiles/ArmadilloConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/InstallFiles/ArmadilloConfigVersion.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.894507 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindARPACK.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindATLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindBLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindFlexiBLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindLAPACK.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindMKL.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindOpenBLAS.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/cmake_aux/Modules/ARMA_FindSuperLU5.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.894507 random-forestry-0.10.0/extension/armadillo/include/
--rw-r--r--   0 runner    (1001) docker     (123)    32439 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.010509 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/BaseCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/BaseCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Base_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20269 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Base_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Col_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    37783 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Col_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/CubeToMatOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/CubeToMatOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28720 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Cube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   127221 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Cube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/GenCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/GenCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Gen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Gen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/GlueCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/GlueCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Glue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Glue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/MapMat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    33757 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/MapMat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    45408 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   203280 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/OpCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/OpCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Op_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Op_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    92960 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Proxy.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20131 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/ProxyCube.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Row_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    37727 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/Row_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SizeCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SizeCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SizeMat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SizeMat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpBase_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17596 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpBase_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpCol_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpCol_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    35836 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpMat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpMat_iterators_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   148166 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpMat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpRow_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpRow_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpSubview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpSubview_col_list_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpSubview_col_list_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31949 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpSubview_iterators_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    40563 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpSubview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpToDOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpToDOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpValProxy_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/SpValProxy_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_cmath.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_config.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_forward.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_ostream_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28965 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_ostream_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_rel_comparators.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_rng.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_rng_cxx03.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_static_check.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_str.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arma_version.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arrayops_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/arrayops_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/auxlib_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   196845 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/auxlib_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/band_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/compiler_check.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/compiler_setup.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/compiler_setup_post.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/cond_rel_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/cond_rel_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/config.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/config.hpp.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/constants_old.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/csv_name.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    35701 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/def_arpack.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/def_atlas.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/def_blas.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/def_fftw3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   115263 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/def_lapack.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/def_superlu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/diagmat_proxy.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/diagview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/diagview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/diskio_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   129573 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/diskio_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/distr_param.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eGlueCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eGlueCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eOpCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eOpCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eglue_core_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    46921 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eglue_core_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eop_aux.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eop_core_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30632 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/eop_core_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fft_engine_fftw3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fft_engine_kissfft.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/field_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    62071 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/field_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fill.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_accu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_all.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_any.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_approx_equal.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_as_scalar.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_chi2rnd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_chol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_clamp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_cond_rcond.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_conv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18097 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_conv_to.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_cor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_cross.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_cumprod.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_cumsum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_det.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_diagmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_diagvec.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_diff.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_dot.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eig_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eig_pair.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eig_sym.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eigs_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eigs_sym.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_elem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eps.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_expmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_eye.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_fft.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_fft2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_find.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_find_unique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_flip.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_hess.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_hist.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_histc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_index_max.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_index_min.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_inplace_strans.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_inplace_trans.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_interp1.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_interp2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_intersect.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_inv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_inv_sympd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_join.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_kmeans.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_kron.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_log_det.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_log_normpdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_logmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_lu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_max.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_mean.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_median.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_min.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_mvnrnd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_n_unique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_nonzeros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_norm.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_normalise.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_normcdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_normpdf.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_numel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_ones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_orth_null.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_pinv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_polyfit.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_polyval.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_powext.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_powmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_princomp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_prod.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_qr.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_quantile.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_qz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_randg.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_randi.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_randn.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_randperm.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_randu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_range.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_rank.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_regspace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_repelem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_repmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_reshape.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_resize.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_reverse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_roots.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_schur.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_shift.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_shuffle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_size.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_solve.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sort_index.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_speye.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_spones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sprandn.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sprandu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_spsolve.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sqrtmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_stddev.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_strans.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_svd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_svds.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_sylvester.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_symmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_toeplitz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trace.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trans.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trapz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trig.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trimat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trimat_ind.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trunc_exp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_trunc_log.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_unique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_var.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_vectorise.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_wishrnd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/fn_zeros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_affmul_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_affmul_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_atan2_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_atan2_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_conv_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_conv_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_cor_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_cor_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_cov_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_cov_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_cross_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_cross_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_hist_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_hist_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_histc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_histc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_hypot_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_hypot_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_intersect_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_intersect_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_join_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_join_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_kron_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_kron_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_mixed_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_mixed_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_mvnrnd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_mvnrnd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_polyfit_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_polyfit_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_polyval_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_polyval_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_powext_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_powext_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_quantile_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_quantile_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_relational_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_relational_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_solve_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20198 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_solve_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_times_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34564 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_times_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_toeplitz_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_toeplitz_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_trapz_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/glue_trapz_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/gmm_diag_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    66029 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/gmm_diag_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/gmm_full_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    68513 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/gmm_full_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/gmm_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/gmm_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19941 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/hdf5_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/hdf5_name.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/include_hdf5.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/include_superlu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/injector_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/injector_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/memory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mp_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtGlueCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtGlueCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtOpCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtOpCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtSpGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtSpGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtSpOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mtSpOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mul_gemm.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mul_gemm_mixed.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mul_gemv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mul_herk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/mul_syrk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_EigsSelect.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_GenEigsSolver_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_GenEigsSolver_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SortEigenvalue.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SparseGenRealShiftSolve_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SparseGenRealShiftSolve_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SymEigsShiftSolver_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SymEigsShiftSolver_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SymEigsSolver_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_SymEigsSolver_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_TridiagEigen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_TridiagEigen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/newarp_cx_attrib.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_all_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_all_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_any_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_any_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_chi2rnd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_chi2rnd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_chol_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_chol_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_clamp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_clamp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_col_as_mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_col_as_mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cond_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cond_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cor_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cor_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cov_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cov_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cumprod_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cumprod_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cumsum_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cumsum_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cx_scalar_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_cx_scalar_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_det_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_det_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_diagmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20265 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_diagmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_diagvec_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_diagvec_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_diff_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_diff_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_dot_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_dot_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_dotext_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_dotext_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_expmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_expmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_fft_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_fft_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_find_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18411 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_find_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_find_unique_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_find_unique_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_flip_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_flip_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_hist_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_hist_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_htrans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_htrans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_index_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_index_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_index_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_index_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_inv_gen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_inv_gen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_inv_spd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_inv_spd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_log_det_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_log_det_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_logmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_logmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_mean_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_mean_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_median_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_median_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_nonzeros_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_nonzeros_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_norm_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18015 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_norm_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_normalise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_normalise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_orth_null_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_orth_null_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_pinv_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_pinv_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_powmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_powmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_princomp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_princomp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_prod_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_prod_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_range_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_range_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_rank_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_rank_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_rcond_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_rcond_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_relational_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_relational_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_repelem_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_repelem_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_repmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_repmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_reshape_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_reshape_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_resize_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_resize_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_reverse_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_reverse_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_roots_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_roots_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_row_as_mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_row_as_mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_shift_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_shift_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_shuffle_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_shuffle_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sort_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sort_index_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sort_index_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sort_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sp_minus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sp_minus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sp_plus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sp_plus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sqrtmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sqrtmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_stddev_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_stddev_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_strans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_strans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sum_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_sum_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_symmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_symmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_toeplitz_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_toeplitz_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_trimat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_trimat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_unique_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_unique_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_var_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_var_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_vectorise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_vectorise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_wishrnd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/op_wishrnd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_cube_div.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_cube_minus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_cube_plus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_cube_relational.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_cube_schur.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_cube_times.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_div.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_minus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_ostream.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_plus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_relational.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_schur.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/operator_times.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/podarray_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/podarray_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/promote_type.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/restrictors.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/running_stat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/running_stat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/running_stat_vec_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/running_stat_vec_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/sp_auxlib_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    86448 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/sp_auxlib_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/span.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spdiagview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23126 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spdiagview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_join_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_join_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_kron_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_kron_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_merge_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_merge_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_minus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_minus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_plus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_plus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_relational_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_relational_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_schur_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_schur_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_times_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18636 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spglue_times_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_diagmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_diagmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_htrans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_htrans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_mean_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_mean_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_norm_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_norm_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_normalise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_normalise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_repmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_repmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_reverse_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_reverse_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_strans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_strans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_sum_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_sum_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_symmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_symmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_trimat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_trimat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_var_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_var_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_vectorise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spop_vectorise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spsolve_factoriser_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/spsolve_factoriser_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/strip.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_cube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_cube_each_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22790 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_cube_each_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    67156 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_cube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_cube_slices_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_cube_slices_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_each_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_each_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_elem1_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23405 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_elem1_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_elem2_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_elem2_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_field_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_field_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   108796 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/subview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/sym_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/translate_arpack.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/translate_atlas.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/translate_blas.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/translate_fftw3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    84711 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/translate_lapack.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/translate_superlu.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/trimat_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/typedef_elem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/typedef_elem_check.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/typedef_mat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/typedef_mat_fixed.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    77808 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/unwrap.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/unwrap_cube.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/unwrap_spmat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/upgrade_val.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/wall_clock_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/wall_clock_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/xtrans_mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/xtrans_mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/xvec_htrans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/include/armadillo_bits/xvec_htrans_meat.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.010509 random-forestry-0.10.0/extension/armadillo/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/misc/armadillo.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/misc/armadillo.spec
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/misc/blank_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/misc/doxygen.config
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/misc/main.doxy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.014509 random-forestry-0.10.0/extension/armadillo/src/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/src/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)    94890 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/src/wrapper1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    89530 2023-05-01 14:32:03.000000 random-forestry-0.10.0/extension/armadillo/src/wrapper2.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.018509 random-forestry-0.10.0/extension/include/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/Makevars
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/Makevars.makefile
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/Makevars.win
--rw-r--r--   0 runner    (1001) docker     (123)    23493 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/RFNode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/RFNode.h
--rw-r--r--   0 runner    (1001) docker     (123)    22904 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/RcppExports.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/dataFrame.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/dataFrame.h
--rw-r--r--   0 runner    (1001) docker     (123)    38308 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/forestry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/forestry.h
--rw-r--r--   0 runner    (1001) docker     (123)    56845 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/forestryTree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/forestryTree.h
--rw-r--r--   0 runner    (1001) docker     (123)    36352 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/rcpp_cppBuildInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/sampling.h
--rw-r--r--   0 runner    (1001) docker     (123)    59695 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/treeSplitting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/treeSplitting.h
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-01 14:31:59.000000 random-forestry-0.10.0/extension/include/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.018509 random-forestry-0.10.0/extension/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:23.890507 random-forestry-0.10.0/extension/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.022509 random-forestry-0.10.0/extension/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65638 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.026509 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    50369 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    25057 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    32147 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79524 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125761 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    93848 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.026509 random-forestry-0.10.0/extension/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.030509 random-forestry-0.10.0/extension/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-01 14:32:05.000000 random-forestry-0.10.0/extension/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.030509 random-forestry-0.10.0/extension/src/
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-05-01 14:31:58.000000 random-forestry-0.10.0/extension/src/api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-01 14:31:58.000000 random-forestry-0.10.0/extension/src/api.h
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-05-01 14:31:58.000000 random-forestry-0.10.0/extension/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-01 14:31:58.000000 random-forestry-0.10.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.030509 random-forestry-0.10.0/random_forestry/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63383 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/forestry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/processed_dta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.034510 random-forestry-0.10.0/random_forestry/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/validators/base_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/validators/fit_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-01 14:31:58.000000 random-forestry-0.10.0/random_forestry/validators/predict_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:32:24.030509 random-forestry-0.10.0/random_forestry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-01 14:32:23.000000 random-forestry-0.10.0/random_forestry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    41990 2023-05-01 14:32:23.000000 random-forestry-0.10.0/random_forestry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:32:23.000000 random-forestry-0.10.0/random_forestry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:32:23.000000 random-forestry-0.10.0/random_forestry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 14:32:23.000000 random-forestry-0.10.0/random_forestry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 14:32:23.000000 random-forestry-0.10.0/random_forestry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:32:24.034510 random-forestry-0.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-01 14:31:58.000000 random-forestry-0.10.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.693841 random-forestry-0.10.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-31 02:43:04.693841 random-forestry-0.10.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.673841 random-forestry-0.10.0b1/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.677841 random-forestry-0.10.0b1/extension/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/Makevars
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/Makevars.makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/Makevars.win
+-rw-r--r--   0 runner    (1001) docker     (123)    23493 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/RFNode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/RFNode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22904 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/RcppExports.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/dataFrame.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/dataFrame.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38308 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/forestry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/forestry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56845 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/forestryTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/forestryTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36352 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/rcpp_cppBuildInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    59695 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/treeSplitting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/treeSplitting.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/include/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.677841 random-forestry-0.10.0b1/extension/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.669841 random-forestry-0.10.0b1/extension/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.681841 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65638 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.685841 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50369 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25057 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42266 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32147 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79524 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125761 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93848 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.685841 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.689841 random-forestry-0.10.0b1/extension/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-31 02:42:38.000000 random-forestry-0.10.0b1/extension/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.689841 random-forestry-0.10.0b1/extension/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/src/api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/src/api.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/extension/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.689841 random-forestry-0.10.0b1/random_forestry/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60437 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/forestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/processed_dta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.693841 random-forestry-0.10.0b1/random_forestry/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/validators/base_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/validators/fit_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/random_forestry/validators/predict_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:43:04.689841 random-forestry-0.10.0b1/random_forestry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-31 02:43:04.000000 random-forestry-0.10.0b1/random_forestry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-31 02:43:04.000000 random-forestry-0.10.0b1/random_forestry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 02:43:04.000000 random-forestry-0.10.0b1/random_forestry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 02:43:04.000000 random-forestry-0.10.0b1/random_forestry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-31 02:43:04.000000 random-forestry-0.10.0b1/random_forestry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 02:43:04.000000 random-forestry-0.10.0b1/random_forestry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 02:43:04.693841 random-forestry-0.10.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-31 02:42:36.000000 random-forestry-0.10.0b1/setup.py
```

### Comparing `random-forestry-0.10.0/LICENSE` & `random-forestry-0.10.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/PKG-INFO` & `random-forestry-0.10.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-forestry
-Version: 0.10.0
+Version: 0.10.0b1
 Summary: Random forest estimator
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `random-forestry-0.10.0/README.md` & `random-forestry-0.10.0b1/README.md`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/CMakeLists.txt` & `random-forestry-0.10.0b1/extension/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,39 +2,51 @@
 
 set(CMAKE_CXX_COMPILER clang++)
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -O3 -ftemplate-depth=1024")
 
 project(forestry)
 
+#### Armadillo
 
-#### PyBind11
-
-add_subdirectory(pybind11)
+find_path(ARMADILLO_INCLUDE_DIR armadillo
+        HINTS $ENV{ARMADILLO_DIR}
+        PATH_SUFFIXES include
+        REQUIRED
+        )
+message(STATUS "ARMADILLO_INCLUDE_DIR => ${ARMADILLO_INCLUDE_DIR}")
 
+find_library(ARMADILLO_LIBRARY armadillo
+        HINTS $ENV{ARMADILLO_DIR}
+        PATH_SUFFIXES lib${LIB_SUFFIX} lib64 lib
+        REQUIRED
+        )
+message(STATUS "ARMADILLO_LIBRARY => ${ARMADILLO_LIBRARY}")
 
-#### Armadillo
 
-option(BUILD_SHARED_LIBS "build shared library" OFF)
-option(BUILD_SMOKE_TEST "build smoke test" OFF)
-add_subdirectory(armadillo)
 
 
+message(STATUS "ARMADILLO_LIBRARY_DIR => ${Armadillo_LIBRARY_DIR}")
+include_directories("include" ${Armadillo_LIBRARY_DIR})
 
+add_subdirectory(pybind11)
+#pybind11_add_module(extension src/main.cpp include/forestry.cpp include/forestryTree.cpp include/dataFrame.cpp include/sampling.cpp)
 
 add_library(extension MODULE src/main.cpp src/api.cpp include/forestry.cpp include/forestryTree.cpp include/dataFrame.cpp include/treeSplitting.cpp include/RFNode.cpp include/sampling.cpp include/utils.cpp)
 
-target_link_libraries(extension PRIVATE pybind11::module pybind11::lto pybind11::windows_extras PUBLIC armadillo)
+target_link_libraries(extension PRIVATE pybind11::module pybind11::lto pybind11::windows_extras PUBLIC ${ARMADILLO_LIBRARY})
 
 pybind11_extension(extension)
 if(NOT MSVC AND NOT ${CMAKE_BUILD_TYPE} MATCHES Debug|RelWithDebInfo)
     # Strip unnecessary sections of the binary on Linux/macOS
     pybind11_strip(extension)
 endif()
 
 set_target_properties(extension PROPERTIES CXX_VISIBILITY_PRESET "hidden" CUDA_VISIBILITY_PRESET "hidden")
 
-target_include_directories(extension PUBLIC include)
+###
+
+target_include_directories(extension PUBLIC ${ARMADILLO_INCLUDE_DIR})
 
-# VERSION_INFO is defined by setup.py and passed into the C++ code as a
+# EXAMPLE_VERSION_INFO is defined by setup.py and passed into the C++ code as a
 # define (VERSION_INFO) here.
 target_compile_definitions(extension PRIVATE VERSION_INFO=${VERSION_INFO})
```

### Comparing `random-forestry-0.10.0/extension/include/RFNode.cpp` & `random-forestry-0.10.0b1/extension/include/RFNode.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/RFNode.h` & `random-forestry-0.10.0b1/extension/include/RFNode.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/RcppExports.cpp` & `random-forestry-0.10.0b1/extension/include/RcppExports.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/dataFrame.cpp` & `random-forestry-0.10.0b1/extension/include/dataFrame.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/dataFrame.h` & `random-forestry-0.10.0b1/extension/include/dataFrame.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/forestry.cpp` & `random-forestry-0.10.0b1/extension/include/forestry.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/forestry.h` & `random-forestry-0.10.0b1/extension/include/forestry.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/forestryTree.cpp` & `random-forestry-0.10.0b1/extension/include/forestryTree.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/forestryTree.h` & `random-forestry-0.10.0b1/extension/include/forestryTree.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/rcpp_cppBuildInterface.cpp` & `random-forestry-0.10.0b1/extension/include/rcpp_cppBuildInterface.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/sampling.cpp` & `random-forestry-0.10.0b1/extension/include/sampling.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #include "utils.h"
 #include <vector>
 #include <string>
 #include <iostream>
 #include <random>
 #include <algorithm>
 #include <cmath>
-#include <unordered_set>
 
 // Given a number of groups, we assign each group to a
 // fold of size foldSize (if numGroups % foldSize != 0, one
 // fold may have a smaller number of groups).
 // Returns a vector of vectors where the ith vector holds the
 // indices of the groups in the ith fold.
 void assign_groups_to_folds(
@@ -117,24 +116,14 @@
     std::vector <size_t> sampleIndex;
 
     // If the forest is to be constructed with minTreesPerFold, we want to
     // use that sampling method instead of the sampling methods we have
     size_t currentFold;
     std::vector <size_t> groups_to_remove;
 
-    // See if the weights are uniform or not
-    std::unordered_set<double> uniqueWeights;
-    std::vector<double>* sampleWeights = (trainingData->getobservationWeights());
-    // Iterate through the vector and insert each value into the unordered_set
-    for (const auto& value : (*sampleWeights)) {
-        uniqueWeights.insert(value);
-    }
-
-    // use weights if multiple unique values
-    bool use_weights = uniqueWeights.size() != 1;
 
     // If using groups with honesty, we split the groups into either splitting or
     // averaging groups before taking the bootstrap sample
     if (((*trainingData->getGroups())[0] != 0) && (oobHonest || ((splitratio != 1) && (splitratio != 0)))) {
 
         // If we are combining honesty with groups, first partition the groups of the tree into
         // splitting and averaging groups.
@@ -359,84 +348,16 @@
         }
 
         // Set the indices and return
         splitSampleIndexReturn = splitSampleIndex_;
         averageSampleIndexReturn = averageSampleIndex_;
         return;
 
-    } else if (replacement && oobHonest && use_weights) {
-
-        // Now we generate a weighted distribution using observationWeights
-        std::vector<double>* sampleWeights = (trainingData->getobservationWeights());
-
-        // First assign the unique observations into the splitting set, averaging set, or double OOB set for the tree
-        // With the ratios:
-        //  - Splitting set = .632
-        //  - Averaging set = .233
-        //  - Double OOB set = .135
-        std::vector<size_t> all_unique_indices(sampleSize);
-
-        // Create a random partition with the correct sizes by shuffling and taking the first
-        // .135 for doob, next .233 for averaging, and next .632 for splitting
-        std::iota(all_unique_indices.begin(), all_unique_indices.end(), 0);
-        std::shuffle(all_unique_indices.begin(), all_unique_indices.end(), random_number_generator);
-
-        size_t doob_count = std::max((size_t) 1, (size_t) std::floor(.135 * (double) sampleSize));
-        size_t avg_count = std::max((size_t) 1, (size_t) std::floor(.233 * (double) sampleSize));
-        size_t spl_count = sampleSize - doob_count - avg_count;
-
-        // Create a vector of the unique avging + splitting indices for this tree
-        std::vector<size_t> unique_avg_indices(all_unique_indices.begin() + doob_count,
-                                               all_unique_indices.begin() + doob_count + avg_count);
-
-        std::vector<size_t> unique_spl_indices(all_unique_indices.begin() + doob_count + avg_count,
-                                               all_unique_indices.end());
-
-        // Get the weights from the original weights vector and assign them to the unique averaging + splitting observations
-        std::vector<double> potential_avg_weights(unique_avg_indices.size());
-        for (size_t i = 0; i < unique_avg_indices.size(); i++) {
-            potential_avg_weights[i] = sampleWeights->at(unique_avg_indices[i]);
-        }
-        std::vector<double> potential_spl_weights(unique_spl_indices.size());
-        for (size_t i = 0; i < unique_spl_indices.size(); i++) {
-            potential_spl_weights[i] = sampleWeights->at(unique_spl_indices[i]);
-        }
-
-        // Create weighted distribution over the potential averaging and splitting indices
-        // Note it is okay not to explicitly normalize the weights since std::discrete_distribution does this already
-        std::discrete_distribution<size_t> potential_avg_dist(
-                potential_avg_weights.begin(), potential_avg_weights.end()
-        );
-        std::discrete_distribution<size_t> potential_spl_dist(
-                potential_spl_weights.begin(), potential_spl_weights.end()
-        );
-
-        // Now carry out the sampling from the two partitions
-        std::vector <size_t> splitSampleIndex_;
-        std::vector <size_t> averageSampleIndex_;
-
-        // Generate index with replacement for averaging set
-        for (size_t j = 0; j < avg_count; j++) {
-            size_t randomIndex = potential_avg_dist(random_number_generator);
-            averageSampleIndex_.push_back(unique_avg_indices[randomIndex]);
-        }
-
-        // Generate index with replacement for averaging set
-        for (size_t j = 0; j < spl_count; j++) {
-            size_t randomIndex = potential_spl_dist(random_number_generator);
-            splitSampleIndex_.push_back(unique_spl_indices[randomIndex]);
-        }
-
-        // Set the indices and return
-        splitSampleIndexReturn = splitSampleIndex_;
-        averageSampleIndexReturn = averageSampleIndex_;
-        return;
-
-        // Standard replacement sampling
     } else if (replacement) {
+
         // Now we generate a weighted distribution using observationWeights
         std::vector<double>* sampleWeights = (trainingData->getobservationWeights());
         std::discrete_distribution<size_t> sample_dist(
                 sampleWeights->begin(), sampleWeights->end()
         );
 
         // Generate index with replacement
```

### Comparing `random-forestry-0.10.0/extension/include/sampling.h` & `random-forestry-0.10.0b1/extension/include/sampling.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/treeSplitting.cpp` & `random-forestry-0.10.0b1/extension/include/treeSplitting.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/treeSplitting.h` & `random-forestry-0.10.0b1/extension/include/treeSplitting.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/utils.cpp` & `random-forestry-0.10.0b1/extension/include/utils.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/include/utils.h` & `random-forestry-0.10.0b1/extension/include/utils.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/CMakeLists.txt` & `random-forestry-0.10.0b1/extension/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/LICENSE` & `random-forestry-0.10.0b1/extension/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/attr.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/buffer_info.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/cast.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/chrono.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/complex.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/class.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/common.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/descr.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/init.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/internals.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/type_caster_base.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/detail/typeid.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/eigen.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/embed.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/eval.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/functional.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/gil.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/iostream.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/numpy.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/operators.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/options.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/pybind11.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/pytypes.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/stl/filesystem.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/stl.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/include/pybind11/stl_bind.h` & `random-forestry-0.10.0b1/extension/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/FindCatch.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/FindEigen3.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/FindPythonLibsNew.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/JoinPaths.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/check-style.sh` & `random-forestry-0.10.0b1/extension/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/cmake_uninstall.cmake.in` & `random-forestry-0.10.0b1/extension/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/codespell_ignore_lines_from_errors.py` & `random-forestry-0.10.0b1/extension/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/libsize.py` & `random-forestry-0.10.0b1/extension/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/make_changelog.py` & `random-forestry-0.10.0b1/extension/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/pybind11Common.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/pybind11Config.cmake.in` & `random-forestry-0.10.0b1/extension/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/pybind11NewTools.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/pybind11Tools.cmake` & `random-forestry-0.10.0b1/extension/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/setup_global.py.in` & `random-forestry-0.10.0b1/extension/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/pybind11/tools/setup_main.py.in` & `random-forestry-0.10.0b1/extension/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/src/api.cpp` & `random-forestry-0.10.0b1/extension/src/api.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     
         // Create outcome data
         std::unique_ptr< std::vector<double> > outcomeData {
                 new std::vector<double>(numRows)
         };
     
         for (size_t i = 0; i < numRows; i++) {
-            outcomeData->at(i) = arr[numColumns*(i+1)-1];
+            outcomeData->at(i) = arr[numColumns*i-1];
         }
     
         numColumns--;
     
     
         // Categorical features column
         std::unique_ptr< std::vector<size_t> > categoricalFeatureCols (
@@ -404,20 +404,19 @@
         }
     
         // Initialize the weightMatrix
         arma::Mat<double> weightMatrix;
     
         if (returnWeightMatrix) {
             weightMatrix.zeros(dta_frame->getNumRows(), dta_frame->getNumRows());
-            std::vector<size_t> treeCounts(dta_frame->getNumRows(), 0);
-
+    
             predictions = forest->predictOOB(
                 predi_data,
                 &weightMatrix,
-                &treeCounts,
+                nullptr,
                 doubleOOB,
                 exact,
                 training_idx_use
             );
     
             size_t idx = 0;
             for (size_t i = 0; i < dta_frame->getNumRows(); i++){
```

### Comparing `random-forestry-0.10.0/extension/src/api.h` & `random-forestry-0.10.0b1/extension/src/api.h`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/extension/src/main.cpp` & `random-forestry-0.10.0b1/extension/src/main.cpp`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/pyproject.toml` & `random-forestry-0.10.0b1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 [build-system]
 requires = ["setuptools >= 65.6.3, < 66", "wheel >=0.34.2, < 1", "cmake >= 3.26, < 4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "random-forestry"
-version = "0.10.0"
+version = "0.10.0-b1"
 description = "Random forest estimator"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "numpy >= 1.23.5, < 2",
-    "pandas >= 1.4, < 1.5",
+    "numpy >= 1.24.2, < 2",
+    "pandas >= 1.5.3, < 2",
     "statsmodels >= 0.13.5, < 1",
     "pydantic >= 1.10.6, < 2",
-    "scikit-learn == 1.2.2, < 2",
 
     # Conditional dependencies
     'typing_extensions; python_version < "3.11"'
 ]
 requires-python = ">=3.8"
 
 [tool.setuptools]
 packages = ["random_forestry", "random_forestry.validators"]
 zip-safe = false
 
 [project.optional-dependencies]
-dev = ["bumpver >= 2022.1120", "pip-tools >= 6.12.3"]
-test = ["pytest >= 7.2.2"]
+dev = ["bumpver >= 2022.1120, < 2023", "pip-tools >= 6.12.3, < 7"]
+test = ["pytest >= 7.2.2, < 8", "scikit-learn == 1.2.2, < 2"]
 
 [project.urls]
 Homepage = "https://github.com/forestry-labs/Rforestry#readme"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.10.0"
+current_version = "0.10.0-b1"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `random-forestry-0.10.0/random_forestry/forestry.py` & `random-forestry-0.10.0b1/random_forestry/forestry.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import math
 import os
 import pickle  # nosec B403 - 'Consider possible security implications associated with pickle'
 import sys
 import warnings
 from pathlib import Path
 from random import randrange
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
+import statsmodels.api as sm
 from pydantic import (  # pylint: disable=no-name-in-module
     ConfigDict,
     StrictBool,
     StrictFloat,
     StrictInt,
     confloat,
     conint,
@@ -132,15 +133,15 @@
      which are not in a group in the current fold. The folds form a random partition of
      all of the possible groups, each of size foldSize. This means we create at
      least # folds * min_trees_per_fold trees for the forest.
      If ntree > # folds * min_trees_per_fold, we create
      max(# folds * min_trees_per_fold, ntree) total trees, in which at least min_trees_per_fold
      are created leaving out each fold.
     :type min_trees_per_fold: *int, optional, default=0*
-    :param fold_size: The number of groups that are selected randomly for each fold to be
+    :param fold_size The number of groups that are selected randomly for each fold to be
      left out when using minTreesPerFold. When minTreesPerFold is set and foldSize is
      set, all possible groups will be partitioned into folds, each containing foldSize unique groups
      (if foldSize doesn't evenly divide the number of groups, a single fold will be smaller,
      as it will contain the remaining groups). Then minTreesPerFold are grown with each
      entire fold of groups left out.
     :type fold_size: *int, optional, default=1*
     :param monotone_avg: This is a flag that indicates whether or not monotonic
@@ -193,15 +194,15 @@
         * unique_feature_values (*list*) - The categories of the current categorical feature.
 
         * numeric_feature_values (*numpy.array*) - The categories of the current categorical feature encoded
           into numeric represetation.
 
      * feature_weights (*numpy.array of shape[ncols]*) - an array of sampling probabilities/weights for each feature
        used when subsampling *mtry* features at each node.
-       Check out :meth:`fit() <random_forestry.RandomForest.fit>` fot more details.
+       Check out :meth:`fit() <Rforestry.RandomForest.fit>` fot more details.
 
      * feature_weights_variables (*numpy.array*) - Indices of the features which weight
        more than ``max(feature_weights)*0.001`` .
 
      * deep_feature_weights (*numpy.array of shape[ncols]*) - Used in place of *feature_weights* for splits
        below *interaction_depth*. Check out :meth:`fit() <forestry.RandomForest.fit>` fot more details.
 
@@ -213,19 +214,27 @@
        Check out :meth:`fit() <forestry.RandomForest.fit>` fot more details.
 
      * monotonic_constraints (*numpy.array of shape[ncols]*) - An array of size *ncol* specifying monotonic
        relationships between the continuous features and the outcome. Its entries are in -1, 0, 1, in which
        1 indicates an increasing monotonic relationship, -1 indicates a decreasing monotonic relationship, and
        0 indicates no constraint. Check out :meth:`fit() <forestry.RandomForest.fit>` fot more details.
 
-     * group_memberships(*numpy.array of shape[nrows]*) - Factorized group membership of each training observation.
-
      * linear_feature_cols (*numpy.array*) - An array containing the indices of which features to split linearly on
        when using linear penalized splits. Check out :meth:`fit() <forestry.RandomForest.fit>` fot more details.
 
+     * groups_mapping (*dict*) - Contains informtion about the groups of the training observations.
+       Has the following entries:
+
+        * group_value (*pandas.Index*) - The categories of the groups.
+
+        * group_numeric_value (*numpy.array*) - The categories of the groups encoded into numeric represetation
+
+     * groups (*pandas.Series(..., dtype='category')*) - Specifies the group membership of each training observation.
+       Check out :meth:`fit() <forestry.RandomForest.fit>` fot more details.
+
      * col_means (*numpy.array of shape[ncols]*) - The mean value of each column.
 
      * col_sd (*numpy.array of shape[ncols]*) - The standard deviation of each column.
 
      * has_nas (*bool*) - Specifies whether the feature matrix contains missing observations or not.
 
      * na_direction (*bool*) - Sets a default direction for missing values in each split node during training
@@ -238,16 +247,16 @@
 
      Note that **all** of the entries in processed_dta are set to ``None`` or empty containers during initialization.
      They are only assigned a value after :meth:`fit() <forestry.RandomForest.fit>` is called.
     :vartype processed_dta: ProcessedDta
 
      .. _translate-label:
 
-    :ivar saved_forest: For any tree *i* in the forest, *saved_forest[i]* is a dictionary which gives access to the
-     underlying structrure of that tree. *saved_forest[i]* has the following entries:
+    :ivar saved_forest: For any tree *i* in the forest, *saved_forest[i]* is a dictionary which gives access to the underlying
+     structrure of that tree. *saved_forest[i]* has the following entries:
 
      * children_right (*numpy.array of shape[number of nodes in the tree,]*) - For a node with a given *id*,
        *children_right[id]* gives the id of the right child of that node. If leaf node, *children_right[id]* is *-1*.
 
      * children_left (*numpy.array of shape[number of nodes in the tree,]*) - For a node with a given *id*,
        *children_left[id]* gives the id of the left child of that node. If leaf node, *children_left[id]* is *-1*.
 
@@ -262,16 +271,16 @@
        gives the splitting point (threshold) of the split in that node. If leaf node, *threshold[id]* is *0.0*.
 
      * values (*numpy.array of shape[number of nodes in the tree,]*) - For a node with a given *id*, if that node is
        a leaf node, *values[id]* gives the prediction made by that node. Otherwise, *values[id]* is *0.0*.
 
      .. note::
         When a *RandomForest* is initialized, *saved_forest* is set to a list of *ntree* empty dictionaries. In order to
-        populate those dictionaries, the :meth:`translate_tree() <random_forestry.RandomForest.translate_tree>` method
-        must be used.
+        populate those dictionaries, one must use the :meth:`translate_tree() <Rforestry.RandomForest.translate_tree>`
+        method.
 
     :vartype saved_forest: list[dict]
     :ivar forest: A ctypes pointer to the *forestry* object in C++. It is initially set to *None* and updated only
      after :meth:`fit() <forestry.RandomForest.fit>` is called.
     :vartype forest: ctypes.c_void_p
     :ivar dataframe: A ctypes pointer to the *DataFrame* object in C++. It is initially set to *None* and updated only
      after :meth:`fit() <forestry.RandomForest.fit>` is called.
@@ -350,14 +359,15 @@
         if seed is None:
             return self.seed
         if (not isinstance(seed, int)) or seed < 0:
             raise ValueError("seed must be a nonnegative integer.")
         return seed
 
     def _set_nodesize_strict(self) -> None:
+
         # if the splitratio is 1, then we use adaptive rf and avgSampleSize is
         # equal to the total sampsize
 
         if self.splitratio in (0, 1):
             split_sample_size = self.sampsize
             avg_sample_size = self.sampsize
         else:
@@ -397,35 +407,38 @@
         weights_variables = [i for i in range(weights.size) if weights[i] > max(weights) * 0.001]
         if len(weights_variables) < self.mtry:
             raise ValueError("mtry is too large. Given the feature weights, can't select that many features.")
 
         weights_variables = np.array(weights_variables, dtype=np.ulonglong)
         return weights_variables
 
-    def _get_group_memberships(self, nrow: int, groups: Optional[pd.Series]) -> np.ndarray:
-        if groups is None:
-            return np.zeros(nrow, dtype=np.ulonglong)
-        codes, levels = pd.factorize(groups)
-        # Increment array to avoid having 0s
-        codes += 1
+    def _get_groups_mapping_and_vector(self, x: pd.DataFrame, groups: Optional[pd.Series]) -> Tuple[dict, pd.Series]:
+        nrow, _ = x.shape
+        groups_mapping = {}
+        if groups is not None:
+            groups_mapping["groupValue"] = groups.cat.categories
+            groups_mapping["groupNumericValue"] = np.arange(len(groups.cat.categories))
 
-        # Print warning if the group number and minTreesPerFold results in a large forest
-        if self.min_trees_per_fold > 0 and (-(len(levels) // -self.fold_size)) * self.min_trees_per_fold > 2000:
-            warnings.warn(
-                "Using "
-                + str(len(levels))
-                + " groups with fold size "
-                + str(self.fold_size)
-                + " and "
-                + str(self.min_trees_per_fold)
-                + " trees per fold will train "
-                + str(len(levels) * self.min_trees_per_fold)
-                + " trees in the forest"
-            )
-        return codes
+            group_vector = pd.to_numeric(groups)
+
+            # Print warning if the group number and minTreesPerFold results in a large forest
+            if self.min_trees_per_fold > 0 and len(groups.cat.categories) * self.min_trees_per_fold > 2000:
+                warnings.warn(
+                    "Using "
+                    + str(len(groups.cat.categories))
+                    + " groups with "
+                    + str(self.min_trees_per_fold)
+                    + " trees per group will train "
+                    + str(len(groups.cat.categories) * self.min_trees_per_fold)
+                    + " trees in the forest"
+                )
+
+        else:
+            group_vector = np.zeros(nrow, dtype=np.ulonglong)
+        return groups_mapping, group_vector
 
     @FitValidator
     def fit(
         self,
         x: Union[pd.DataFrame, pd.Series, List],
         y: np.ndarray,
         *,
@@ -464,22 +477,22 @@
         :type linFeats: *array_like, optional*
         :param monotonicConstraints: Specifies monotonic relationships between the continuous
          features and the outcome. Supplied as a list of length *ncol* with entries in
          1, 0, -1, with 1 indicating an increasing monotonic relationship, -1 indicating
          a decreasing monotonic relationship, and 0 indicating no constraint.
          Constraints supplied for categorical variable will be ignored. Defaults to all 0-s (no constraints).
         :type monotonicConstraints: *array_like of shape [ncols,], optional*
-        :param groups: A pandas series specifying the group membership of each training observation.
+        :param groups: A pandas categorical Seires specifying the group membership of each training observation.
          These groups are used in the aggregation when doing out of bag predictions in
          order to predict with only trees where the entire group was not used for aggregation.
          This allows the user to specify custom subgroups which will be used to create
          predictions which do not use any data from a common group to make predictions for
          any observation in the group. This can be used to create general custom
          resampling schemes, and provide predictions consistent with the Out-of-Group set.
-        :type groups: *pandas.Series, optional*,
+        :type groups: *pandas.Categorical(...), pandas.Series(..., dtype="category"),
          or other pandas categorical dtypes, optional, default=None*
         :param seed: Random number generator seed. The default value is the *RandomForest* seed.
         :type seed: *int, optional*
         :rtype: None
         """
 
         # Make sure that all the parameters exist when passed to RandomForest
@@ -509,15 +522,15 @@
         deep_feature_weights_variables = self._get_weights_variables(deep_feature_weights)
 
         feature_weights /= np.sum(feature_weights)
         deep_feature_weights /= np.sum(deep_feature_weights)
         if self.replace:
             observation_weights /= np.sum(observation_weights)
 
-        group_memberships = self._get_group_memberships(nrow, groups)
+        groups_mapping, group_vector = self._get_groups_mapping_and_vector(x, groups)
 
         (
             processed_x,
             categorical_feature_cols,
             categorical_feature_mapping,
         ) = preprocessing.preprocess_training(x, y)
 
@@ -541,15 +554,15 @@
             feature_weights_variables,
             feature_weights_variables.size,
             deep_feature_weights,
             deep_feature_weights_variables,
             deep_feature_weights_variables.size,
             observation_weights,
             monotonic_constraints,
-            group_memberships,
+            group_vector,
             self.monotone_avg,
             nrow,
             ncol + 1,
             self._get_seed(seed),
         )
 
         self.forest: pd.DataFrame = extension.train_forest(
@@ -591,15 +604,16 @@
             feature_weights=feature_weights,
             feature_weights_variables=feature_weights_variables,
             deep_feature_weights=deep_feature_weights,
             deep_feature_weights_variables=deep_feature_weights_variables,
             observation_weights=observation_weights,
             monotonic_constraints=monotonic_constraints,
             linear_feature_cols=lin_feats,
-            groups=group_memberships,
+            groups_mapping=groups_mapping,
+            groups=groups,
             col_means=col_means,
             col_sd=col_sd,
             has_nas=x.isnull().values.any(),
             n_observations=nrow,
             num_columns=ncol,
             feat_names=feat_names,
         )
@@ -622,154 +636,99 @@
         processed_x = preprocessing.preprocess_testing(
             newdata,
             self.processed_dta.categorical_feature_cols,
             self.processed_dta.categorical_feature_mapping,
         )
         return len(processed_x.index)
 
-    def _scale_ret_values(
-        self, ret_values: Optional[Tuple[np.ndarray, np.ndarray]], include_coefficients: bool = False
-    ) -> Optional[Tuple[np.ndarray, np.ndarray]]:
-        if include_coefficients:
-            return (
-                ret_values[0] * self.processed_dta.col_sd[-1] + self.processed_dta.col_means[-1],
-                ret_values[1],
-                ret_values[2],
-            )
-        return (ret_values[0] * self.processed_dta.col_sd[-1] + self.processed_dta.col_means[-1], ret_values[1])
-
     def _aggregation_oob(
         self,
         newdata: Optional[pd.DataFrame],
         exact: bool,
         return_weight_matrix: bool,
-        training_idx: Optional[np.ndarray],
+        training_idx: Optional[np.ndarray]
     ) -> Optional[Tuple[np.ndarray, np.ndarray]]:
-        if newdata is not None:
-            processed_x = preprocessing.preprocess_testing(
-                newdata,
-                self.processed_dta.categorical_feature_cols,
-                self.processed_dta.categorical_feature_mapping,
-            )
-            if len(processed_x.index) != self.processed_dta.n_observations and training_idx is None:
-                raise ValueError("Attempting to do OOB predictions on a dataset which doesn't match the training data!")
-            if training_idx and len(training_idx) != len(newdata.index):
-                raise ValueError("Training Indices must be of the same length as newdata")
-            if self.scale:
-                processed_x = preprocessing.scale_center(
-                    processed_x,
-                    self.processed_dta.categorical_feature_cols,
-                    self.processed_dta.col_means,
-                    self.processed_dta.col_sd,
-                )
+        if newdata is not None and self.processed_dta.n_observations != len(newdata.index) and training_idx is None:
+            warnings.warn("Attempting to do OOB predictions on a dataset which doesn't match the training data!")
+            return None
+        elif len(training_idx) != len(newdata.index):
+            raise ValueError("Training Indices must be of the same length as newdata")
 
-        if training_idx and (
-            not np.issubdtype(training_idx.dtype, np.integer)
-            or np.any((training_idx < 0) | (training_idx >= self.processed_dta.n_observations))
-        ):
-            raise ValueError(
-                "Training Indices must contain integers between 0 and the number of training observations - 1"
-            )
+        if training_idx is not None and (not np.issubdtype(training_idx.dtype, np.integer) or np.any((training_idx < 0) | (training_idx >= self.processed_dta.n_observations))):
+            raise ValueError("Training Indices must contain integers between 0 and the number of training observations - 1")
 
         n_preds = self._get_n_preds(newdata)
         n_weight_matrix = n_preds * self.processed_dta.n_observations if return_weight_matrix else 0
 
-        ret_values = extension.predict_oob_forest(
+        return extension.predict_oob_forest(
             self.forest,
             self.dataframe,
-            self._get_test_data(processed_x),
+            self._get_test_data(newdata),
             False,
             exact,
             return_weight_matrix,
             self.verbose,
             training_idx is not None,
             n_preds,
             n_weight_matrix,
-            training_idx if training_idx else [],
+            training_idx
         )
-        # If the forest was trained with scaled values we need to rescale + re center the predictions
-        if self.scale:
-            return self._scale_ret_values(ret_values)
-        else:
-            return ret_values
 
     def _aggregation_double_oob(
         self,
         newdata: Optional[pd.DataFrame],
         exact: bool,
         return_weight_matrix: bool,
-        training_idx: Optional[np.ndarray],
+        training_idx: Optional[np.ndarray]
     ) -> Tuple[np.ndarray, np.ndarray]:
-        if newdata is not None:
+        if newdata is None:
+            double_oob = True
+        else:
+            double_oob = False
             processed_x = preprocessing.preprocess_testing(
                 newdata,
                 self.processed_dta.categorical_feature_cols,
                 self.processed_dta.categorical_feature_mapping,
             )
             if len(processed_x.index) != self.processed_dta.n_observations and training_idx is None:
                 raise ValueError("Attempting to do OOB predictions on a dataset which doesn't match the training data!")
-            if training_idx and len(training_idx) != len(newdata.index):
+            elif len(training_idx) != len(newdata.index):
                 raise ValueError("Training Indices must be of the same length as newdata")
-            if self.scale:
-                processed_x = preprocessing.scale_center(
-                    processed_x,
-                    self.processed_dta.categorical_feature_cols,
-                    self.processed_dta.col_means,
-                    self.processed_dta.col_sd,
-                )
 
-        if training_idx and (
-            not np.issubdtype(training_idx.dtype, np.integer)
-            or np.any((training_idx < 0) | (training_idx >= self.processed_dta.n_observations))
-        ):
-            raise ValueError(
-                "Training Indices must contain integers between 0 and the number of training observations - 1"
-            )
+        if training_idx is not None and (not np.issubdtype(training_idx.dtype, np.integer) or np.any((training_idx < 0) | (training_idx >= self.processed_dta.n_observations))):
+            raise ValueError("Training Indices must contain integers between 0 and the number of training observations - 1")
+
 
         n_preds = self._get_n_preds(newdata)
         n_weight_matrix = n_preds * self.processed_dta.n_observations if return_weight_matrix else 0
 
-        ret_values = extension.predict_oob_forest(
+        return extension.predict_oob_forest(
             self.forest,
             self.dataframe,
-            self._get_test_data(processed_x),
-            True,
+            self._get_test_data(newdata),
+            double_oob,
             exact,
             return_weight_matrix,
             self.verbose,
             training_idx is not None,
             n_preds,
             n_weight_matrix,
-            training_idx if training_idx else [],
+            training_idx
         )
 
-        # If the forest was trained with scaled values we need to rescale + re center the predictions
-        if self.scale:
-            return self._scale_ret_values(ret_values)
-        else:
-            return ret_values
-
     def _aggregation_coefs(
         self, newdata: pd.DataFrame, exact: bool, seed: int, nthread: int
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         processed_x = preprocessing.preprocess_testing(
             newdata,
             self.processed_dta.categorical_feature_cols,
             self.processed_dta.categorical_feature_mapping,
         )
 
-        if self.scale:
-            processed_x = preprocessing.scale_center(
-                processed_x,
-                self.processed_dta.categorical_feature_cols,
-                self.processed_dta.col_means,
-                self.processed_dta.col_sd,
-            )
-
-        ret_values = extension.predict_forest(
+        return extension.predict_forest(
             self.forest,
             self.dataframe,
             np.ascontiguousarray(processed_x.values[:, :], np.double).ravel(),
             seed,
             nthread,
             exact,
             False,
@@ -778,55 +737,41 @@
             np.zeros(self.ntree, dtype=np.ulonglong),
             len(processed_x.index),
             self._get_n_preds(newdata),
             0,
             self.processed_dta.n_observations * (self.processed_dta.linear_feature_cols.size + 1),
         )
 
-        # If the forest was trained with scaled values we need to rescale + re center the predictions
-        if self.scale:
-            return self._scale_ret_values(ret_values, include_coefficients=True)
-        else:
-            return ret_values
-
     def _aggregation_fallback(
         self,
         newdata: pd.DataFrame,
         exact: bool,
         seed: int,
         nthread: int,
         return_weight_matrix: bool,
         trees: Optional[np.ndarray],
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         processed_x = preprocessing.preprocess_testing(
             newdata,
             self.processed_dta.categorical_feature_cols,
             self.processed_dta.categorical_feature_mapping,
         )
-        if self.scale:
-            processed_x = preprocessing.scale_center(
-                processed_x,
-                self.processed_dta.categorical_feature_cols,
-                self.processed_dta.col_means,
-                self.processed_dta.col_sd,
-            )
-
         tree_weights = np.zeros(self.ntree, dtype=np.ulonglong)
         if trees is not None:
             # If trees are being used, we need to convert them into a weight vector
             for tree in trees:
                 tree_weights[tree] += 1
             use_weights = True
         else:
             use_weights = False
 
         n_preds = self._get_n_preds(newdata)
         n_weight_matrix = n_preds * self.processed_dta.n_observations if return_weight_matrix else 0
 
-        ret_values = extension.predict_forest(
+        return extension.predict_forest(
             self.forest,
             self.dataframe,
             np.ascontiguousarray(processed_x.values[:, :], np.double).ravel(),
             seed,
             nthread,
             exact,
             return_weight_matrix,
@@ -835,39 +780,32 @@
             tree_weights,
             len(processed_x.index),
             n_preds,
             n_weight_matrix,
             0,
         )
 
-        # If the forest was trained with scaled values we need to rescale + re center the predictions
-        if self.scale:
-            return self._scale_ret_values(ret_values, include_coefficients=True)
-        else:
-            return ret_values
-
     @PredictValidator
     def predict(
         self,
         newdata: Optional[Union[pd.DataFrame, pd.Series, List]] = PredictValidator.DEFAULT_NEWDATA,
         *,
         aggregation: str = PredictValidator.DEFAULT_AGGREGATION,
         seed: Optional[int] = None,
         nthread: Optional[int] = None,
-        exact: bool = True,
+        exact: Optional[bool] = None,
         trees: Optional[np.ndarray] = None,
         training_idx: Optional[np.ndarray] = None,
         return_weight_matrix: bool = False,
     ) -> Union[np.ndarray, dict]:
         """
         Return the prediction from the forest.
 
         :param newdata: Testing predictors.
-        :type newdata: *pandas.DataFrame, pandas.Series, numpy.ndarray, 2d list of shape [nsamples, ncols],
-         default=None*
+        :type newdata: *pandas.DataFrame, pandas.Series, numpy.ndarray, 2d list of shape [nsamples, ncols], deffault=None*
         :param aggregation: How the individual tree predictions are aggregated:
          'average' returns the mean of all trees in the forest; 'terminalNodes' also returns
          the weightMatrix, as well as "terminalNodes" - a matrix where
          the i-th entry of the j-th column is the index of the leaf node to which the
          i-th observation is assigned in the j-th tree; and "sparse" - a matrix
          where the ioth entry in the j-th column is 1 if the ith observation in
          newdata is assigned to the j-th leaf and 0 otherwise. In each tree the
@@ -904,44 +842,44 @@
          varied orders as different threads finish at different times.
          By default, exact is *True* unless ``N>100,000`` or a custom aggregation
          function is used.
         :type exact: *bool, optional*
         :param trees: A list of indices in the range *[0, ntree)*, which tells
          predict which trees in the forest to use for the prediction. Predict will by
          default take the average of all trees in the forest, although this flag
-         can be used to get single tree predictions, or averages of different trees
-         with different weightings.
-             .. note::
-                 Duplicate entries are allowed, so if ``trees = [0,1,1]``
-                 this will predict the weighted average prediction of only trees 0 and 1 weighted by:
-                 ``predict(..., trees = [0,1,1]) = (predict(..., trees = [0]) + 2*predict(..., trees = [1])) / 3``
-                 we must have ``exact = True`` , and ``aggregation = "average"`` to use tree indices.
-         Defaults to using all trees equally weighted.
+         can be used to get single tree predictions, or averages of diffferent trees
+         with different weightings. Duplicate entries are allowed, so if ``trees = [0,1,1]``
+         this will predict the weighted average prediction of only trees 0 and 1 weighted by::
+
+            predict(..., trees = [0,1,1]) = (predict(..., trees = [0]) +
+                                            2*predict(..., trees = [1])) / 3
+
+         note we must have ``exact = True`` , and ``aggregation = "average"`` to use tree indices. Defaults to using
+         all trees equally weighted.
         :type trees: *array_like, optional*
         :param training_idx: When doing OOB predictions with a data set that is of a different size than the
-         training data, training_idx holds the indices of the training observations that should be used for
-         determining the out-of-bag set for each observation in newdata. Entries must be between 1 and the number
-         of training observations, and the length must be equal to the number of observations in newdata.
+        training data, training_idx holds the indices of the training observations that should be used for
+        determining the out-of-bag set for each observation in newdata. Entries must be between 1 and the number
+        of training observations, and the length must be equal to the number of observations in newdata.
         :type training_idx: *array_like, optional*
         :param weightMatrix: An indicator of whether or not we should also return a
          matrix of the weights given to each training observation when making each
          prediction. When getting the weight matrix, aggregation must be one of
          'average', 'oob', and 'doubleOOB'. his is a normal text paragraph.
         :type weightMatrix: *bool, optional, default=False*
         :return: An array of predicted responses.
         :rtype: numpy.array
+
         """
 
         if aggregation == "oob":
-            predictions, weight_matrix = self._aggregation_oob(newdata, exact, return_weight_matrix, training_idx)
+            predictions, weight_matrix = self._aggregation_oob(newdata, exact, return_weight_matrix)
 
         elif aggregation == "doubleOOB":
-            predictions, weight_matrix = self._aggregation_double_oob(
-                newdata, exact, return_weight_matrix, training_idx
-            )
+            predictions, weight_matrix = self._aggregation_double_oob(newdata, exact, return_weight_matrix)
 
         elif aggregation == "coefs":
             predictions, weight_matrix, coefficients = self._aggregation_coefs(
                 newdata, exact, self._get_seed(seed), nthread
             )
             return {
                 "predictions": predictions,
@@ -1058,18 +996,18 @@
         """
         from sklearn.metrics import r2_score
 
         return r2_score(y, self.predict(newdata=X, aggregation="average"), sample_weight=sample_weight)
 
     def translate_tree(self, tree_ids: Optional[Union[int, np.ndarray]] = None) -> None:
         """
-        Given a trained forest, translates the selected trees by allowing access to its underlying structure. After
-        translating tree *i*, its structure will be stored as a dictionary in :ref:`saved_forest <translate-label>`
-        and can be accessed by ``[RandomForest object].saved_forest[i]``. Check out the
-        :ref:`saved_forest <translate-label>` attribute for more details about its structure.
+        Given a trained forest, translates the selected trees by allowing access to its underlying structure.
+        After translating tree *i*, its structure will be stored as a dictionary in :ref:`saved_forest <translate-label>`
+        and can be accessed by ``[RandomForest object].saved_forest[i]`` . Check out the :ref:`saved_forest <translate-label>`
+        attribute for more details about its structure.
 
         :param tree_ids: The indices of the trees to be translated. By default, all the trees in the forest
          are translated.
         :type tree_ids: *int/array_like, optional*
         :rtype: None
         """
 
@@ -1081,46 +1019,45 @@
         else:
             if isinstance(tree_ids, (int, np.integer)):
                 idx = np.array([tree_ids])
             else:
                 idx = np.array(tree_ids)
 
         for cur_id in idx:
+
             if self.saved_forest[cur_id]:
                 continue
 
             num_nodes = extension.get_tree_node_count(self.forest, cur_id)
             num_leaf_nodes = extension.get_tree_leaf_count(self.forest, cur_id)
 
             # Initialize arrays to pass to C
             split_info = np.empty(self.sampsize + 1, dtype=np.intc)
-            averaging_info = np.empty(self.sampsize + 1, dtype=np.intc)
+            averaging_info = split_info
 
             tree_info = np.empty(num_nodes * 5 + num_leaf_nodes * 2 + 1, dtype=np.double)
 
             extension.fill_tree_info(self.forest, cur_id, tree_info, split_info, averaging_info)
 
-            self.saved_forest[cur_id]["feature"] = np.empty(num_nodes + num_leaf_nodes, dtype=np.intc)
+            self.saved_forest[cur_id]["feature"] = np.empty(num_nodes+num_leaf_nodes, dtype=np.intc)
             self.saved_forest[cur_id]["threshold"] = np.empty(num_nodes, dtype=np.double)
             self.saved_forest[cur_id]["values"] = np.empty(num_leaf_nodes, dtype=np.double)
             self.saved_forest[cur_id]["na_left_count"] = np.empty(num_nodes, dtype=np.intc)
             self.saved_forest[cur_id]["na_right_count"] = np.empty(num_nodes, dtype=np.intc)
             self.saved_forest[cur_id]["na_default_direction"] = np.empty(num_nodes, dtype=np.intc)
 
-            for i in range(num_nodes + num_leaf_nodes):
+            for i in range(num_nodes+num_leaf_nodes):
                 self.saved_forest[cur_id]["feature"][i] = int(tree_info[i])
             for i in range(num_leaf_nodes):
-                self.saved_forest[cur_id]["values"][i] = tree_info[num_nodes + num_leaf_nodes + i]
+                self.saved_forest[cur_id]["values"][i] = tree_info[num_nodes+num_leaf_nodes + i]
             for i in range(num_nodes):
                 self.saved_forest[cur_id]["threshold"][i] = tree_info[num_nodes + num_leaf_nodes * 2 + i]
                 self.saved_forest[cur_id]["na_left_count"][i] = int(tree_info[num_nodes * 2 + num_leaf_nodes * 2 + i])
                 self.saved_forest[cur_id]["na_right_count"][i] = int(tree_info[num_nodes * 3 + num_leaf_nodes * 2 + i])
-                self.saved_forest[cur_id]["na_default_direction"][i] = int(
-                    tree_info[num_nodes * 4 + num_leaf_nodes * 2 + i]
-                )
+                self.saved_forest[cur_id]["na_default_direction"][i] = int(tree_info[num_nodes * 4 + num_leaf_nodes * 2 + i])
 
             num_split_idx = int(split_info[0])
             self.saved_forest[cur_id]["splitting_sample_idx"] = np.empty(num_split_idx, dtype=np.intc)
             for i in range(num_split_idx):
                 self.saved_forest[cur_id]["splitting_sample_idx"][i] = int(split_info[i + 1])
 
             num_av_idx = int(averaging_info[0])
@@ -1149,15 +1086,15 @@
         Set the parameters of the *RandomForest*.
 
         :param **params: Forestry parameters.
         :type **params: *dict*
         :return: A new *RandomForest* object with the given parameters.
          Note: this reinitializes the *RandomForest* object,
          so fit must be called on the new estimator.
-        :rtype: *RandomForest*
+        :rtype: *RandomForest* -- MIGHT CHANGE THE NAME
         """
 
         if not new_parameters:
             return self
 
         current_parameters = self.get_parameters()
         for parameter in new_parameters:
@@ -1174,14 +1111,19 @@
         state = self.__dict__.copy()
         del state["dataframe"]
         del state["forest"]
         return state
 
     def __setstate__(self, state: dict) -> None:
         self.__dict__ = state
+        group_vector = (
+            pd.to_numeric(state["processed_dta"].groups)
+            if state["processed_dta"].groups is not None
+            else np.repeat(0, state["processed_dta"].n_observations)
+        )
         state["dataframe"] = extension.get_data(
             np.ascontiguousarray(
                 pd.concat(
                     [
                         state["processed_dta"].processed_x,
                         pd.Series(state["processed_dta"].y),
                     ],
@@ -1197,15 +1139,15 @@
             state["processed_dta"].feature_weights_variables,
             state["processed_dta"].feature_weights_variables.size,
             state["processed_dta"].deep_feature_weights,
             state["processed_dta"].deep_feature_weights_variables,
             state["processed_dta"].deep_feature_weights_variables.size,
             state["processed_dta"].observation_weights,
             state["processed_dta"].monotonic_constraints,
-            state["processed_dta"].group_memberships,
+            group_vector,
             state["monotone_avg"],
             state["processed_dta"].n_observations,
             state["processed_dta"].num_columns + 1,
             state["seed"],
         )
 
         tree_counts = np.empty(state["ntree"] * 4, dtype=np.intc)
@@ -1219,15 +1161,15 @@
 
             tree_counts[3 * i + 2] = state["saved_forest"][i]["averaging_sample_idx"].size
             total_av_idx += tree_counts[3 * i + 2]
 
             tree_counts[3 * i + 3] = state["saved_forest"][i]["values"].size
             total_leaf_nodes += tree_counts[3 * i + 3]
 
-        features = np.empty(total_nodes + total_leaf_nodes, dtype=np.intc)
+        features = np.empty(total_nodes+total_leaf_nodes, dtype=np.intc)
 
         thresholds = np.empty(total_nodes, dtype=np.double)
         na_left_counts = np.empty(total_nodes, dtype=np.intc)
         na_right_counts = np.empty(total_nodes, dtype=np.intc)
         na_default_direction = np.empty(total_nodes, dtype=np.intc)
 
         sample_split_idx = np.empty(total_split_idx, dtype=np.intc)
@@ -1252,15 +1194,15 @@
                 ind_s += 1
 
             for j in range(tree_counts[3 * i + 2]):
                 sample_av_idx[ind_a] = state["saved_forest"][i]["averaging_sample_idx"][j]
                 ind_a += 1
 
             for j in range(tree_counts[3 * i + 3]):
-                features[tree_counts[3 * i] + ind_val] = state["saved_forest"][i]["feature"][j]
+                features[tree_counts[3 * i]+ind_val] = state["saved_forest"][i]["feature"][j]
                 predict_weights[ind_val] = state["saved_forest"][i]["values"][j]
                 ind_val += 1
 
             tree_seeds[i] = state["saved_forest"][i]["seed"]
 
         state["forest"] = extension.reconstruct_tree(
             state["dataframe"],
@@ -1300,37 +1242,20 @@
             sample_av_idx,
             predict_weights,
             tree_seeds,
         )
 
     # Saving and loading
     def save_forestry(self, filename: Path) -> None:
-        """
-        Given a trained forest, saves the forest using pickle in the file given by *filename*. This can be used
-        to save a model for future analysis or share a model after training.
-
-        :param filename: The name of the file to save the forest model to
-        :type Path: *char/array_like, optional*
-        :rtype: None
-        """
         self.translate_tree()
 
         with open(filename, "wb") as output_file:  # Overwrites any existing file.
             pickle.dump(self, output_file, pickle.HIGHEST_PROTOCOL)
 
     @staticmethod
     def load_forestry(filename: Path) -> Self:
-        """
-        Loads a forest that has been saved using *save_forestry*. Since the forest contains a pointer to the
-        C++ object, it is necessary to rebuild this object and relink the pointer before the forest can
-        be used to make predictions etc.
-
-        :param filename: The name of the file to save the
-        :type Path: *char/array_like, optional*
-        :rtype: None
-        """
         with open(filename, "rb") as input_file:
             return pickle.load(input_file)  # nosec B301
 
     def __del__(self):
         # Free the pointers to foretsry and dataframe
         extension.delete_forestry(self.forest, self.dataframe)
```

### Comparing `random-forestry-0.10.0/random_forestry/preprocessing.py` & `random-forestry-0.10.0b1/random_forestry/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     return x.isnull().values.any()
 
 
 def get_sampsize(forest, x: pd.DataFrame) -> int:
     nrows, _ = x.shape
     if forest.sampsize is None:
         sampsize = nrows if forest.replace else math.ceil(0.632 * nrows)
-    else:
-        sampsize = forest.sampsize
 
     # only if sample.fraction is given, update sampsize
     if forest.sample_fraction is not None:
         sampsize = math.ceil(forest.sample_fraction * nrows)
 
     return sampsize
 
@@ -76,14 +74,15 @@
     if (not forest.dataframe) or (not forest.forest):
         raise ValueError("The RandomForest object has invalid ctypes pointers.")
 
 
 # Given a dataframe with Y and Y.hat at least, fits an OLS and gives the LOO
 # predictions on the sample
 def loo_pred_helper(data_frame: pd.DataFrame) -> dict:
+
     Y = data_frame["Y"]
     X = data_frame.loc[:, data_frame.columns != "Y"]
     X = sm.add_constant(X)
 
     adjust_lm = sm.OLS(Y, X).fit()
 
     cv = LeaveOneOut()
```

### Comparing `random-forestry-0.10.0/random_forestry/processed_dta.py` & `random-forestry-0.10.0b1/random_forestry/processed_dta.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     feature_weights: Optional[np.ndarray] = None
     feature_weights_variables: Optional[np.ndarray] = None
     deep_feature_weights: Optional[np.ndarray] = None
     deep_feature_weights_variables: Optional[str] = None
     observation_weights: Optional[str] = None
     monotonic_constraints: Optional[str] = None
     linear_feature_cols: np.ndarray = field(default_factory=lambda: np.array(0))
-    group_memberships: np.ndarray = field(default_factory=lambda: np.array(0))
+    groups_mapping: Optional[Dict[str, Any]] = None
+    groups: Optional[str] = None
     col_means: np.ndarray = field(default_factory=lambda: np.array(0))
     col_sd: np.ndarray = field(default_factory=lambda: np.array(0))
     has_nas: bool = False
     na_direction: bool = False
     n_observations: int = 0
     num_columns: int = 0
     feat_names: Optional[np.ndarray] = None
```

### Comparing `random-forestry-0.10.0/random_forestry/test.py` & `random-forestry-0.10.0b1/random_forestry/test.py`

 * *Files identical despite different names*

### Comparing `random-forestry-0.10.0/random_forestry/validators/fit_validator.py` & `random-forestry-0.10.0b1/random_forestry/validators/fit_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 
 from .. import preprocessing
 from .base_validator import BaseValidator
 
 
 class FitValidator(BaseValidator):
+
     def validate_monotonic_constraints(self, *args, **kwargs):
         _self = args[0]
 
         x = pd.DataFrame(kwargs.get("x", args[1])).copy()
         _, ncols = x.shape
 
         if "monotonic_constraints" not in kwargs:
@@ -103,17 +104,24 @@
             raise ValueError("There must be at least one non-zero weight in deep_feature_weights")
 
         return deep_feature_weights
 
     def validate_groups(self, *_, **kwargs):
         if "groups" in kwargs:
             groups = kwargs["groups"]
+            if not pd.api.types.is_categorical_dtype(groups):
+                raise ValueError(
+                    "groups must have a data dtype of categorical. ",
+                    'Try using pd.Categorical(...) or pd.Series(..., dtype="category").',
+                )
             if len(groups.unique()) == 1:
                 raise ValueError("groups must have more than 1 level to be left out from sampling.")
-            return groups
+
+            return pd.Series(groups, dtype="category")
+
         return None
 
     def __call__(self, *args, **kwargs):
         _self = args[0]
 
         x = pd.DataFrame(kwargs.get("x", args[1])).copy()
         y = np.array(kwargs.get("y", args[1] if "x" in kwargs else args[2]), dtype=np.double).copy()
```

### Comparing `random-forestry-0.10.0/random_forestry/validators/predict_validator.py` & `random-forestry-0.10.0b1/random_forestry/validators/predict_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 
 from .. import preprocessing
 from .base_validator import BaseValidator
 
 
 class PredictValidator(BaseValidator):
+
     DEFAULT_NEWDATA: Final = None
     DEFAULT_AGGREGATION: Final[str] = "average"
 
     def get_newdata(self, *args, **kwargs) -> Union[pd.DataFrame, pd.Series, List, None]:
         if len(args) > 2:
             raise TypeError(f"predict() takes from 1 to 2 positional arguments but {len(args)} were given")
         if len(args) == 2:
```

### Comparing `random-forestry-0.10.0/random_forestry.egg-info/PKG-INFO` & `random-forestry-0.10.0b1/random_forestry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-forestry
-Version: 0.10.0
+Version: 0.10.0b1
 Summary: Random forest estimator
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `random-forestry-0.10.0/setup.py` & `random-forestry-0.10.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,19 @@
                 # CMake 3.12+ only.
                 build_args += [f"-j{self.parallel}"]
 
         build_temp = Path(self.build_temp) / ext.name
         if not build_temp.exists():
             build_temp.mkdir(parents=True)
 
-        subprocess.run(["cmake", ext.sourcedir] + cmake_args, cwd=build_temp, check=True)
-        subprocess.run(["cmake", "--build", ".", "-v"] + build_args, cwd=build_temp, check=True)
+        subprocess.run(
+            ["cmake", ext.sourcedir] + cmake_args, cwd=build_temp, check=True
+        )
+        subprocess.run(
+            ["cmake", "--build", ".", "-v"] + build_args, cwd=build_temp, check=True
+        )
 
 
 setup(
     ext_modules=[CMakeExtension("random_forestry.extension", sourcedir="extension")],
     cmdclass={"build_ext": CMakeBuild},
 )
```

