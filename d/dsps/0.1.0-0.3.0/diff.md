# Comparing `tmp/dsps-0.1.0.tar.gz` & `tmp/dsps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsps-0.1.0.tar", last modified: Mon Dec 13 19:16:25 2021, max compression
+gzip compressed data, was "dsps-0.3.0.tar", last modified: Mon May  1 19:39:05 2023, max compression
```

## Comparing `dsps-0.1.0.tar` & `dsps-0.3.0.tar`

### file list

```diff
@@ -1,104 +1,183 @@
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2021-12-13 19:16:25.865378 dsps-0.1.0/
--rw-r--r--   0 aphearin   (501) staff       (20)     1521 2021-12-13 19:09:18.000000 dsps-0.1.0/LICENSE
--rw-r--r--   0 aphearin   (501) staff       (20)      303 2021-12-13 19:16:25.865561 dsps-0.1.0/PKG-INFO
--rw-r--r--   0 aphearin   (501) staff       (20)      303 2021-11-30 22:29:55.000000 dsps-0.1.0/README.md
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2021-12-13 19:16:25.832336 dsps-0.1.0/dsps/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3244 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/attenuation_kernels.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2021-12-13 19:16:25.839053 dsps-0.1.0/dsps/data/
--rw-r--r--   0 aphearin   (501) staff       (20)      328 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/fsps_lsst_mags_zobs.npy
--rw-r--r--   0 aphearin   (501) staff       (20)      792 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/fsps_lsst_mags_zobs_imet_20_iage_5.npy
--rw-r--r--   0 aphearin   (501) staff       (20)      792 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/fsps_lsst_mags_zobs_imet_2_iage_90.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    15832 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/fsps_ssp_imet_20_iage_5.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    15832 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/fsps_ssp_imet_2_iage_90.npy
--rw-r--r--   0 aphearin   (501) staff       (20)      880 2021-11-04 22:19:36.000000 dsps-0.1.0/dsps/data/log_age.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    14576 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/lsst_g_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    12688 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/lsst_i_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    13648 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/lsst_r_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)     7216 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/lsst_u_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    15376 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/lsst_y_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    10976 2021-11-04 20:51:58.000000 dsps-0.1.0/dsps/data/lsst_z_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)      304 2021-11-04 22:19:20.000000 dsps-0.1.0/dsps/data/zlegend.npy
--rw-r--r--   0 aphearin   (501) staff       (20)     6787 2021-12-02 15:26:42.000000 dsps-0.1.0/dsps/diffstar_ew_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1518 2021-12-13 18:44:12.000000 dsps-0.1.0/dsps/diffstar_photometry.py
--rw-r--r--   0 aphearin   (501) staff       (20)     7824 2021-12-13 18:44:12.000000 dsps-0.1.0/dsps/diffstar_photometry_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1642 2021-12-02 15:26:42.000000 dsps-0.1.0/dsps/equivalent_width.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3392 2021-11-04 18:06:37.000000 dsps-0.1.0/dsps/flat_wcdm.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4231 2021-12-13 18:44:12.000000 dsps-0.1.0/dsps/load_diffstar_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1847 2021-12-01 16:44:25.000000 dsps-0.1.0/dsps/load_fsps_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6488 2021-12-10 22:04:08.000000 dsps-0.1.0/dsps/mzr.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3402 2021-11-04 23:06:02.000000 dsps-0.1.0/dsps/photometry.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2351 2021-11-04 21:56:44.000000 dsps-0.1.0/dsps/photometry_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1369 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/remnant_mass.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4533 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/sfh_model.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2596 2021-12-01 16:44:25.000000 dsps-0.1.0/dsps/stellar_ages.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1739 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/surviving_mstar.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2021-12-13 19:16:25.847972 dsps-0.1.0/dsps/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3282 2021-11-08 14:32:51.000000 dsps-0.1.0/dsps/tests/retrieve_fake_fsps_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3090 2021-11-16 19:01:00.000000 dsps-0.1.0/dsps/tests/test_attenuation.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2824 2021-12-02 15:26:42.000000 dsps-0.1.0/dsps/tests/test_diffstar_ew_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1166 2021-11-16 17:53:01.000000 dsps-0.1.0/dsps/tests/test_diffstar_photometry.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6101 2021-12-13 18:44:12.000000 dsps-0.1.0/dsps/tests/test_diffstar_photometry_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1132 2021-12-02 15:26:42.000000 dsps-0.1.0/dsps/tests/test_equivalent_width.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3271 2021-11-01 16:31:50.000000 dsps-0.1.0/dsps/tests/test_flat_wcdm.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1370 2021-11-30 22:29:55.000000 dsps-0.1.0/dsps/tests/test_mzr.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1339 2021-11-30 22:29:55.000000 dsps-0.1.0/dsps/tests/test_photometry.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2519 2021-11-04 20:53:12.000000 dsps-0.1.0/dsps/tests/test_photometry_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2830 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/tests/test_remnant_mass.py
--rw-r--r--   0 aphearin   (501) staff       (20)      215 2021-11-08 14:32:51.000000 dsps-0.1.0/dsps/tests/test_retrieve_fake_fsps_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)      393 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/test_sfh_model.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3374 2021-11-05 15:29:54.000000 dsps-0.1.0/dsps/tests/test_stellar_ages.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1917 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/tests/test_surviving_mstar.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1928 2021-12-01 18:55:21.000000 dsps-0.1.0/dsps/tests/test_utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3474 2021-12-10 22:04:08.000000 dsps-0.1.0/dsps/tests/test_weighted_ssps.py
--rw-r--r--   0 aphearin   (501) staff       (20)      643 2021-11-01 15:49:18.000000 dsps-0.1.0/dsps/tests/test_zh_model.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2021-12-13 19:16:25.864991 dsps-0.1.0/dsps/tests/testing_data/
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/calzetti_2000_attenuation.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/calzetti_2000_k_lambda.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/calzetti_2000_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 14:24:13.000000 dsps-0.1.0/dsps/tests/testing_data/chabrier_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/tests/testing_data/chabrier_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)      612 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/galazzi_etal05_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     1340 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/kirby_etal13_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 14:24:13.000000 dsps-0.1.0/dsps/tests/testing_data/kroupa_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/tests/testing_data/kroupa_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)      613 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/kudritzki_etal16_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/leitherer_2002_attenuation.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/leitherer_2002_k_lambda.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/leitherer_2002_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 14:24:13.000000 dsps-0.1.0/dsps/tests/testing_data/lg_ages_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     3799 2021-10-26 18:12:12.000000 dsps-0.1.0/dsps/tests/testing_data/lgageray_myr.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     1010 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/maiolino_etal18_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     2558 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_attenuation1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_attenuation2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2555 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_attenuation3.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2558 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_k_lambda1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_k_lambda2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2555 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_k_lambda3.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/noll_2009_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/salim_2018_attenuation1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2556 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/salim_2018_attenuation2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/salim_2018_k_lambda1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2556 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/salim_2018_k_lambda2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/salim_2018_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 14:24:13.000000 dsps-0.1.0/dsps/tests/testing_data/salpeter_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/tests/testing_data/salpeter_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)    53768 2021-11-08 14:32:51.000000 dsps-0.1.0/dsps/tests/testing_data/ssp_plaw_data_c0.txt
--rw-r--r--   0 aphearin   (501) staff       (20)    53390 2021-11-08 14:32:51.000000 dsps-0.1.0/dsps/tests/testing_data/ssp_plaw_data_c1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)      257 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/trussler_etal20_mzr_all_centrals_sdss_dr7.dat
--rw-r--r--   0 aphearin   (501) staff       (20)      259 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/tests/testing_data/trussler_etal20_mzr_all_sats_sdss_dr7.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 14:24:13.000000 dsps-0.1.0/dsps/tests/testing_data/van_dokkum_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2021-11-17 23:25:46.000000 dsps-0.1.0/dsps/tests/testing_data/van_dokkum_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     4347 2021-12-05 22:03:45.000000 dsps-0.1.0/dsps/utils.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5069 2021-12-10 22:04:08.000000 dsps-0.1.0/dsps/weighted_ssps.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1190 2021-10-25 22:41:03.000000 dsps-0.1.0/dsps/weighted_table_interpolation.py
--rw-r--r--   0 aphearin   (501) staff       (20)      446 2021-11-01 15:49:18.000000 dsps-0.1.0/dsps/zh_model.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2021-12-13 19:16:25.833664 dsps-0.1.0/dsps.egg-info/
--rw-r--r--   0 aphearin   (501) staff       (20)      303 2021-12-13 19:16:25.000000 dsps-0.1.0/dsps.egg-info/PKG-INFO
--rw-r--r--   0 aphearin   (501) staff       (20)     3628 2021-12-13 19:16:25.000000 dsps-0.1.0/dsps.egg-info/SOURCES.txt
--rw-r--r--   0 aphearin   (501) staff       (20)        1 2021-12-13 19:16:25.000000 dsps-0.1.0/dsps.egg-info/dependency_links.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       18 2021-12-13 19:16:25.000000 dsps-0.1.0/dsps.egg-info/requires.txt
--rw-r--r--   0 aphearin   (501) staff       (20)        5 2021-12-13 19:16:25.000000 dsps-0.1.0/dsps.egg-info/top_level.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       95 2021-12-13 19:16:25.866185 dsps-0.1.0/setup.cfg
--rw-r--r--   0 aphearin   (501) staff       (20)      574 2021-12-13 19:14:38.000000 dsps-0.1.0/setup.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.065017 dsps-0.3.0/
+-rw-r--r--   0 aphearin   (501) staff       (20)       90 2022-09-09 13:28:37.000000 dsps-0.3.0/.coveragerc
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:04.982627 dsps-0.3.0/.github/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:04.993908 dsps-0.3.0/.github/workflows/
+-rw-r--r--   0 aphearin   (501) staff       (20)     1089 2023-04-29 18:27:09.000000 dsps-0.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)     1150 2023-04-29 18:27:09.000000 dsps-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)     1489 2023-04-29 18:27:09.000000 dsps-0.3.0/.gitignore
+-rw-r--r--   0 aphearin   (501) staff       (20)      212 2023-04-29 18:27:09.000000 dsps-0.3.0/.readthedocs.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)      741 2023-05-01 18:08:03.000000 dsps-0.3.0/CHANGES.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1521 2023-04-29 18:27:09.000000 dsps-0.3.0/LICENSE.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4069 2023-05-01 19:39:05.064414 dsps-0.3.0/PKG-INFO
+-rw-r--r--   0 aphearin   (501) staff       (20)     1966 2023-04-29 18:27:09.000000 dsps-0.3.0/README.md
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:04.994686 dsps-0.3.0/docs/
+-rw-r--r--   0 aphearin   (501) staff       (20)      638 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/Makefile
+-rw-r--r--   0 aphearin   (501) staff       (20)      804 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/make.bat
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:04.999703 dsps-0.3.0/docs/source/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.000144 dsps-0.3.0/docs/source/_static/
+-rw-r--r--   0 aphearin   (501) staff       (20)   129468 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/_static/fake_ssp_seds.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     1241 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/citation.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1039 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/conf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2171 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/custom_ssps.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2044 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/dsps_data_config.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9494 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/dsps_quickstart.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     1062 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      706 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/installation.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1454 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/quickstart.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      309 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/reference.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)       62 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/requirements.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)      127 2023-04-29 18:27:09.000000 dsps-0.3.0/docs/source/tutorials.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.002554 dsps-0.3.0/dsps/
+-rw-r--r--   0 aphearin   (501) staff       (20)      173 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)       22 2023-05-01 19:39:04.000000 dsps-0.3.0/dsps/_version.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      186 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/constants.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.005946 dsps-0.3.0/dsps/cosmology/
+-rw-r--r--   0 aphearin   (501) staff       (20)      146 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/cosmology/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      198 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/cosmology/defaults.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6618 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/cosmology/flat_wcdm.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.006848 dsps-0.3.0/dsps/cosmology/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/cosmology/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5975 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/cosmology/tests/test_flat_wcdm.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.007418 dsps-0.3.0/dsps/data/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2349 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data/README.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.009712 dsps-0.3.0/dsps/data_loaders/
+-rw-r--r--   0 aphearin   (501) staff       (20)      250 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1165 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/defaults.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2564 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/load_filter_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2252 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/load_ssp_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3412 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/retrieve_fake_fsps_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2097 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/retrieve_fsps_data.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.011055 dsps-0.3.0/dsps/data_loaders/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1707 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/tests/test_load_filter_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      797 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/tests/test_load_ssp_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1042 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/tests/test_retrieve_fake_fsps_data.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.012041 dsps-0.3.0/dsps/data_loaders/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)    53768 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)    53390 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.013999 dsps-0.3.0/dsps/dust/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12142 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/att_curves.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.015727 dsps-0.3.0/dsps/dust/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5152 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/test_att_curves.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      983 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/test_utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.023757 dsps-0.3.0/dsps/dust/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2558 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_attenuation1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_attenuation2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2555 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_attenuation3.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2558 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_k_lambda1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_k_lambda2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2555 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_k_lambda3.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_attenuation1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2556 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_attenuation2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_k_lambda1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2556 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_k_lambda2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)      704 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/dust/utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.024360 dsps-0.3.0/dsps/em_lines/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/em_lines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1699 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/em_lines/equivalent_width.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.025017 dsps-0.3.0/dsps/em_lines/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/em_lines/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1131 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/em_lines/tests/test_equivalent_width.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.025599 dsps-0.3.0/dsps/experimental/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/experimental/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3161 2023-05-01 17:12:20.000000 dsps-0.3.0/dsps/experimental/diffburst.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.026584 dsps-0.3.0/dsps/experimental/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/experimental/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5178 2023-05-01 17:12:20.000000 dsps-0.3.0/dsps/experimental/tests/test_diffburst.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.028063 dsps-0.3.0/dsps/imf/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1463 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/remnant_mass.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1822 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/surviving_mstar.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.029318 dsps-0.3.0/dsps/imf/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2830 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/test_remnant_mass.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1917 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/test_surviving_mstar.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.035521 dsps-0.3.0/dsps/imf/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/chabrier_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/chabrier_mstar_surviving_norem.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/kroupa_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/kroupa_mstar_surviving_norem.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/lg_ages_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/salpeter_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/salpeter_mstar_surviving_norem.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving_norem.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.036510 dsps-0.3.0/dsps/metallicity/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3962 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/mzr.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.037423 dsps-0.3.0/dsps/metallicity/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      842 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/test_mzr.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.040940 dsps-0.3.0/dsps/metallicity/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)      612 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/testing_data/galazzi_etal05_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)     1340 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/testing_data/kirby_etal13_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)      613 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/testing_data/kudritzki_etal16_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)     1010 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/testing_data/maiolino_etal18_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)      257 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/testing_data/trussler_etal20_mzr_all_centrals_sdss_dr7.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)      259 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/metallicity/tests/testing_data/trussler_etal20_mzr_all_sats_sdss_dr7.dat
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.043449 dsps-0.3.0/dsps/photometry/
+-rw-r--r--   0 aphearin   (501) staff       (20)       57 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3312 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/photometry_kernels.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3030 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/photpop.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.045626 dsps-0.3.0/dsps/photometry/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2566 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/tests/test_photometry_kernels.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1646 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/tests/test_photpop.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1449 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/photometry/utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.048110 dsps-0.3.0/dsps/sed/
+-rw-r--r--   0 aphearin   (501) staff       (20)      147 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3624 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/metallicity_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4386 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/ssp_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5636 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/stellar_age_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6139 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/stellar_sed.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.050083 dsps-0.3.0/dsps/sed/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3222 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/tests/test_csp_sed.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2130 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/tests/test_metallicity_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2994 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/tests/test_ssp_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2957 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/sed/tests/test_stellar_age_weights.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.050744 dsps-0.3.0/dsps/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2021-10-25 22:41:03.000000 dsps-0.3.0/dsps/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4234 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/test_utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.059729 dsps-0.3.0/dsps/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)      328 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/fsps_lsst_mags_zobs.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)      792 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_20_iage_5.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)      792 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_2_iage_90.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    15832 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/fsps_ssp_imet_20_iage_5.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    15832 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/fsps_ssp_imet_2_iage_90.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)     3799 2021-10-26 18:12:12.000000 dsps-0.3.0/dsps/tests/testing_data/lgageray_myr.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)    14576 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/lsst_g_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    12688 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/lsst_i_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    13648 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/lsst_r_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)     7216 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/lsst_u_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    15376 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/lsst_y_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    10976 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/tests/testing_data/lsst_z_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    53768 2021-11-08 14:32:51.000000 dsps-0.3.0/dsps/tests/testing_data/ssp_plaw_data_c0.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)    53390 2021-11-08 14:32:51.000000 dsps-0.3.0/dsps/tests/testing_data/ssp_plaw_data_c1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     5458 2023-04-29 18:27:09.000000 dsps-0.3.0/dsps/utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.004969 dsps-0.3.0/dsps.egg-info/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4069 2023-05-01 19:39:04.000000 dsps-0.3.0/dsps.egg-info/PKG-INFO
+-rw-r--r--   0 aphearin   (501) staff       (20)     5635 2023-05-01 19:39:04.000000 dsps-0.3.0/dsps.egg-info/SOURCES.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)        1 2023-05-01 19:39:04.000000 dsps-0.3.0/dsps.egg-info/dependency_links.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       15 2023-05-01 19:39:04.000000 dsps-0.3.0/dsps.egg-info/requires.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       16 2023-05-01 19:39:04.000000 dsps-0.3.0/dsps.egg-info/top_level.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.061559 dsps-0.3.0/notebooks/
+-rw-r--r--   0 aphearin   (501) staff       (20)    72997 2021-11-17 23:25:46.000000 dsps-0.3.0/notebooks/tabulate_mstar_surviving_different_imfs.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    70225 2021-10-27 11:32:35.000000 dsps-0.3.0/notebooks/validate_dsps_attenuation.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     1222 2023-04-29 18:27:09.000000 dsps-0.3.0/pyproject.toml
+-rw-r--r--   0 aphearin   (501) staff       (20)       14 2023-04-29 18:27:09.000000 dsps-0.3.0/requirements.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-01 19:39:05.063735 dsps-0.3.0/scripts/
+-rw-r--r--   0 aphearin   (501) staff       (20)    23049 2023-04-29 18:27:09.000000 dsps-0.3.0/scripts/generate_fsps_photometry_validation_data.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)      436 2023-04-29 18:27:09.000000 dsps-0.3.0/scripts/write_fsps_data_to_disk.py
+-rw-r--r--   0 aphearin   (501) staff       (20)       38 2023-05-01 19:39:05.065161 dsps-0.3.0/setup.cfg
+-rw-r--r--   0 aphearin   (501) staff       (20)       38 2023-04-29 18:27:09.000000 dsps-0.3.0/setup.py
```

### Comparing `dsps-0.1.0/LICENSE` & `dsps-0.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/fsps_lsst_mags_zobs_imet_20_iage_5.npy` & `dsps-0.3.0/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_20_iage_5.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/fsps_lsst_mags_zobs_imet_2_iage_90.npy` & `dsps-0.3.0/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_2_iage_90.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/fsps_ssp_imet_20_iage_5.npy` & `dsps-0.3.0/dsps/tests/testing_data/fsps_ssp_imet_20_iage_5.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/fsps_ssp_imet_2_iage_90.npy` & `dsps-0.3.0/dsps/tests/testing_data/fsps_ssp_imet_2_iage_90.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/lsst_g_transmission.npy` & `dsps-0.3.0/dsps/tests/testing_data/lsst_g_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/lsst_i_transmission.npy` & `dsps-0.3.0/dsps/tests/testing_data/lsst_i_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/lsst_r_transmission.npy` & `dsps-0.3.0/dsps/tests/testing_data/lsst_r_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/lsst_u_transmission.npy` & `dsps-0.3.0/dsps/tests/testing_data/lsst_u_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/lsst_y_transmission.npy` & `dsps-0.3.0/dsps/tests/testing_data/lsst_y_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/data/lsst_z_transmission.npy` & `dsps-0.3.0/dsps/tests/testing_data/lsst_z_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/equivalent_width.py` & `dsps-0.3.0/dsps/em_lines/equivalent_width.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-"""
+"""Kernels used to calculate equivalent width of spectral lines"""
 from jax import jit as jjit
 from jax import numpy as jnp
 
 
 @jjit
 def _get_quadfit_weights(x, x1, x2, x3, x4):
     msk_lo = (x >= x1) & (x <= x2)
@@ -51,15 +50,15 @@
 ):
     quadfit_w = _get_quadfit_weights(
         wave, cont_lo_lo, cont_lo_hi, cont_hi_lo, cont_hi_hi
     )
     c = _weighted_quadratic_fit(wave, flux, quadfit_w)
     c2, c1, c0 = c
 
-    continuum_strength_at_line = c0 + c1 * line_mid + c2 * line_mid ** 2
+    continuum_strength_at_line = c0 + c1 * line_mid + c2 * line_mid**2
 
     int_w = _get_integration_weights(wave, line_lo, line_hi)
     continuum_integrand = int_w * (c0 + c1 * wave + c2 * wave * wave)
     spec_integrand = int_w * flux
 
     continuum_flux_integral = jnp.trapz(continuum_integrand, x=wave)
     spec_flux_integral = jnp.trapz(spec_integrand, x=wave)
```

### Comparing `dsps-0.1.0/dsps/photometry.py` & `dsps-0.3.0/dsps/photometry/photometry_kernels.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,131 +1,119 @@
-"""
-"""
-from jax import vmap as jvmap, jit as jjit
-from .photometry_kernels import _obs_flux_ssp, _calc_obs_mag_no_dimming, _calc_obs_mag
-
-_a = [None, 0, None, None, None]
-_b = [None, None, None, None, 0]
-_obs_flux_ssp_vmap = jjit(
-    jvmap(jvmap(jvmap(_obs_flux_ssp, in_axes=_b), in_axes=_a), in_axes=_a)
-)
-_calc_obs_mag_no_dimming_vmap = jjit(
-    jvmap(jvmap(jvmap(_calc_obs_mag_no_dimming, in_axes=_b), in_axes=_a), in_axes=_a)
-)
-
-_calc_obs_mag_no_dimming_vmap_singlemet = jjit(
-    jvmap(jvmap(_calc_obs_mag_no_dimming, in_axes=_b), in_axes=_a)
-)
-
-_c = [None, 0, None, None, None, None, None]
-_d = [None, None, None, None, 0, None, None]
-_e = [None, None, 0, 0, None, None, None]
-
-_calc_obs_mag_vmap = jjit(
-    jvmap(jvmap(jvmap(_calc_obs_mag, in_axes=_d), in_axes=_c), in_axes=_c)
-)
-
-_a = (*[None] * 4, 0, *[None] * 5)
-_calc_obs_mag_vmap_z = jjit(jvmap(_calc_obs_mag, in_axes=_a))
+"""Kernels of common photometry integrals"""
+from jax import numpy as jnp
+from jax import jit as jjit
+from ..cosmology.flat_wcdm import distance_modulus_to_z
 
-_b = (None, 0, *[None] * 8)
-_calc_obs_mag_vmap_spec = jjit(jvmap(_calc_obs_mag, in_axes=_b))
+AB0 = 1.13492e-13  # 3631 Jansky placed at 10 pc in units of Lsun/Hz
+
+
+__all__ = ("calc_obs_mag", "calc_rest_mag")
 
 
 @jjit
-def calc_obs_mag_history_singlegal(
-    wave_spec, lum_spec, wave_filter, trans_filter, z_obs, Om0, Ode0, w0, wa, h
+def calc_obs_mag(
+    wave_spec_rest, lum_spec, wave_filter, trans_filter, redshift, Om0, w0, wa, h
 ):
-    """Calculate the history of the observed flux of a single galaxy
-    through a particular filter.
+    """Calculate the apparent magnitude of an SED observed through a filter
 
     Parameters
     ----------
-    wave_spec_rest : ndarray of shape (n_wave_spec, )
-        Rest-frame wavelengths of the spectrum
-
-    lum_spec : ndarray of shape (n_wave_spec, )
-        Spectrum of each galaxy in Lsun/Hz
+    wave_spec_rest : ndarray of shape (n_wave, )
 
-    wave_filter : ndarray of shape (n_wave_filter, )
-        Wave length of the filter transmission curve
+    lum_spec : ndarray of shape (n_wave, )
 
-    trans_filter : ndarray of shape (n_wave_filter, )
-        Fraction of the incident flux transmitted through the filter
+    wave_filter : ndarray of shape (n_filter_wave, )
 
-    z_obs : ndarray of shape (n_obs, )
-        Array of redshifts of the observed galaxies
+    trans_filter : ndarray of shape (n_filter_wave, )
 
-    Om0: float
-        Omega matter at z=0
+    redshift : float
 
-    Ode0: float
-        Omega DE at z=0
+    Om0 : float
 
     w0 : float
-        DE eqn of state today
 
     wa : float
-        DE eqn of state deriv
 
     h : float
-        Little h
 
     Returns
     -------
-    obs_mags : ndarray of shape (n_obs, )
+    obs_mag : float
 
     """
-    obs_mags = _calc_obs_mag_vmap_z(
-        wave_spec, lum_spec, wave_filter, trans_filter, z_obs, Om0, Ode0, w0, wa, h
+    flux_source = _obs_flux_ssp(
+        wave_spec_rest, lum_spec, wave_filter, trans_filter, redshift
     )
-    return obs_mags
+    flux_ab0 = _flux_ab0_at_10pc(wave_filter, trans_filter)
+    mag_no_dimming = -2.5 * jnp.log10(flux_source / flux_ab0)
+    dimming = _cosmological_dimming(redshift, Om0, w0, wa, h)
+    obs_mag = mag_no_dimming + dimming
+    return obs_mag
 
 
 @jjit
-def calc_obs_mags_galpop(
-    wave_spec, lum_spec, wave_filter, trans_filter, z_obs, Om0, Ode0, w0, wa, h
-):
-    """Calculate the history of the observed flux of a galaxy population
-    at a single redshift observed through a particular filter.
+def _cosmological_dimming_from_table(z, z_table, distance_modulus_table):
+    distance_modulus = jnp.interp(z, z_table, distance_modulus_table)
+    return distance_modulus - 2.5 * jnp.log10(1 + z)
 
-    Parameters
-    ----------
-    wave_spec_rest : ndarray of shape (n_wave_spec, )
-        Rest-frame wavelengths of the spectrum
 
-    lum_spec : ndarray of shape (n_gals, n_wave_spec)
-        Spectrum of each galaxy in Lsun/Hz
+@jjit
+def _cosmological_dimming(z, Om0, w0, wa, h):
+    dmod = distance_modulus_to_z(z, Om0, w0, wa, h)
+    return dmod - 2.5 * jnp.log10(1 + z)
 
-    wave_filter : ndarray of shape (n_wave_filter, )
-        Wave length of the filter transmission curve
 
-    trans_filter : ndarray of shape (n_wave_filter, )
-        Fraction of the incident flux transmitted through the filter
+@jjit
+def _calc_obs_mag_no_dimming(wave_spec_rest, lum_spec, wave_filter, trans_filter, z):
+    flux_source = _obs_flux_ssp(wave_spec_rest, lum_spec, wave_filter, trans_filter, z)
+    flux_ab0 = _flux_ab0_at_10pc(wave_filter, trans_filter)
+    return -2.5 * jnp.log10(flux_source / flux_ab0)
 
-    z_obs : float
-        Redshift of the observed galaxies
 
-    Om0: float
-        Omega matter at z=0
+@jjit
+def calc_rest_mag(wave_spec_rest, lum_spec, wave_filter, trans_filter):
+    """Calculate the restframe magnitude of an SED observed through a filter
 
-    Ode0: float
-        Omega DE at z=0
+    Parameters
+    ----------
+    wave_spec_rest : ndarray of shape (n_wave, )
 
-    w0 : float
-        DE eqn of state today
+    lum_spec : ndarray of shape (n_wave, )
 
-    wa : float
-        DE eqn of state deriv
+    wave_filter : ndarray of shape (n_filter_wave, )
 
-    h : float
-        Little h
+    trans_filter : ndarray of shape (n_filter_wave, )
 
     Returns
     -------
-    obs_mags : ndarray of shape (n_gals, )
+    rest_mag : float
 
     """
-    obs_mags = _calc_obs_mag_vmap_spec(
-        wave_spec, lum_spec, wave_filter, trans_filter, z_obs, Om0, Ode0, w0, wa, h
+    flux_source = _rest_flux_ssp(wave_spec_rest, lum_spec, wave_filter, trans_filter)
+    flux_ab0 = _flux_ab0_at_10pc(wave_filter, trans_filter)
+    rest_mag = -2.5 * jnp.log10(flux_source / flux_ab0)
+    return rest_mag
+
+
+@jjit
+def _obs_flux_ssp(wave_spec_rest, lum_spec, wave_filter, trans_filter, z):
+    lum_zshift_phot = jnp.interp(
+        wave_filter, wave_spec_rest * (1 + z), lum_spec, left=0, right=0
     )
-    return obs_mags
+    integrand = trans_filter * lum_zshift_phot / wave_filter
+    lum_filter = jnp.trapz(integrand, x=wave_filter)
+    return lum_filter
+
+
+@jjit
+def _rest_flux_ssp(wave_spec_rest, lum_spec, wave_filter, trans_filter):
+    lum_phot = jnp.interp(wave_filter, wave_spec_rest, lum_spec, left=0, right=0)
+    integrand = trans_filter * lum_phot / wave_filter
+    lum_filter = jnp.trapz(integrand, x=wave_filter)
+    return lum_filter
+
+
+@jjit
+def _flux_ab0_at_10pc(wave_filter, trans_filter):
+    integrand = trans_filter * AB0 / wave_filter
+    lum_ab0_filter = jnp.trapz(integrand, x=wave_filter)
+    return lum_ab0_filter
```

### Comparing `dsps-0.1.0/dsps/surviving_mstar.py` & `dsps-0.3.0/dsps/imf/surviving_mstar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""
-"""
+"""Functions calculating the surviving stellar mass as a function of time"""
 from collections import OrderedDict
 from copy import deepcopy
 from jax import jit as jjit
-from .utils import _sigmoid, _sig_slope
+from ..utils import _sigmoid, _sig_slope
 
 
 PARAMS = OrderedDict(x0=2, yhi=0.58)
 DEFAULT_PARAMS = OrderedDict(
     a=0.225,
     b=8.0,
     lgk1=-0.5,
@@ -59,13 +58,14 @@
     """
     frac_returned = _returned_mass(lg_age_yr, a, b, lgk1, d, e, f, lgk2, h)
     return 1 - frac_returned
 
 
 @jjit
 def _returned_mass(lg_age_yr, a, b, lgk1, d, e, f, lgk2, h):
-    k1 = 10 ** lgk1
-    z = _sig_slope(lg_age_yr, a, b, k1, d, e)
+    k1 = 10**lgk1
+    xtp = b
+    z = _sig_slope(lg_age_yr, xtp, a, b, k1, d, e)
 
-    k2 = 10 ** lgk2
+    k2 = 10**lgk2
     h = _sigmoid(lg_age_yr, f, k2, h, z)
     return h
```

### Comparing `dsps-0.1.0/dsps/tests/retrieve_fake_fsps_data.py` & `dsps-0.3.0/dsps/data_loaders/retrieve_fake_fsps_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 """
 """
 import numpy as np
 from scipy.stats import norm
 import os
+from .defaults import SSPData
 
 
 _THIS_DRNAME = os.path.dirname(os.path.abspath(__file__))
 
 
-def load_fake_sps_data():
-    filter_waves = _get_filter_waves()
-    filter_trans = _get_filter_trans()
-    wave_ssp = _get_wave_ssp()
-    spec_ssp = _get_spec_ssp()
-    lgZsun_bin_mids = _get_lgZsun_bin_mids()
-    log_age_gyr = _get_log_age_gyr()
-    ret = filter_waves, filter_trans, wave_ssp, spec_ssp, lgZsun_bin_mids, log_age_gyr
-    return ret
+def load_fake_ssp_data():
+    ssp_lgmet = _get_lgzlegend()
+    ssp_lg_age_gyr = _get_log_age_gyr()
+    ssp_wave = _get_ssp_wave()
+    ssp_flux = _get_spec_ssp()
+    return SSPData(ssp_lgmet, ssp_lg_age_gyr, ssp_wave, ssp_flux)
+
+
+def load_fake_filter_transmission_curves():
+    wave = _get_ssp_wave()
+    lgwave = np.log10(wave)
+    u = _lsst_u_trans(lgwave)
+    g = _lsst_g_trans(lgwave)
+    r = _lsst_r_trans(lgwave)
+    i = _lsst_i_trans(lgwave)
+    z = _lsst_z_trans(lgwave)
+    y = _lsst_y_trans(lgwave)
+    return wave, u, g, r, i, z, y
 
 
 def _get_log_age_gyr():
     log_age_gyr = np.arange(-3.5, 1.2, 0.05)
     return log_age_gyr
 
 
-def _get_lgZsun_bin_mids():
-    lgZsun_bin_mids = np.log10(zlegend / zlegend[-3])
-    return lgZsun_bin_mids
+def _get_lgzlegend():
+    lgzlegend = np.log10(zlegend)
+    return lgzlegend
 
 
-def _get_wave_ssp():
+def _get_ssp_wave():
     n_wave_ssp = 1963
-    x = np.arange(n_wave_ssp)
-    c0, c1 = 2.358, 0.00257
-    lg_wave_ssp = c0 + c1 * x
-    wave_ssp = 10 ** lg_wave_ssp
-    return wave_ssp
+    ssp_wave = np.linspace(100, 20_000, n_wave_ssp)
+    return ssp_wave
 
 
 def _get_spec_ssp():
-    drn = os.path.join(_THIS_DRNAME, "testing_data")
-    wave_ssp = _get_wave_ssp()
-    n_wave_ssp = wave_ssp.size
+    drn = os.path.join(_THIS_DRNAME, "tests", "testing_data")
+    ssp_wave = _get_ssp_wave()
+    n_wave_ssp = ssp_wave.size
     ssp_plaw_data_c0 = np.loadtxt(os.path.join(drn, "ssp_plaw_data_c0.txt"))
     ssp_plaw_data_c1 = np.loadtxt(os.path.join(drn, "ssp_plaw_data_c1.txt"))
     n_met, n_age = ssp_plaw_data_c0.shape
     spec_ssp = np.zeros((n_met, n_age, n_wave_ssp))
     for iz in range(n_met):
         for iage in range(n_age):
             c0 = ssp_plaw_data_c0[iz, iage]
             c1 = ssp_plaw_data_c1[iz, iage]
-            spec_ssp[iz, iage, :] = 10 ** (c0 + c1 * np.log10(wave_ssp))
+            spec_ssp[iz, iage, :] = 10 ** (c0 + c1 * np.log10(ssp_wave))
     return spec_ssp
 
 
 def _lsst_u_trans(x):
     return norm.pdf(x, loc=3.57, scale=0.022) / 80
```

### Comparing `dsps-0.1.0/dsps/tests/test_equivalent_width.py` & `dsps-0.3.0/dsps/em_lines/tests/test_equivalent_width.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 """
 import numpy as np
 from ..equivalent_width import _ew_kernel
-from ..utils import triweight_gaussian
+from ...utils import triweight_gaussian
 
 
 def get_fake_exp_continuum(exp_peak):
     lgpeak = np.log10(exp_peak)
     x = np.logspace(lgpeak - 2, lgpeak + 1, 500)
-    y = 3.2 * np.exp(-0.5 * (x - exp_peak) ** 2 / 10 ** 2)
+    y = 3.2 * np.exp(-0.5 * (x - exp_peak) ** 2 / 10**2)
     return x, y
 
 
 def get_fake_line(x, line, width, area):
     return triweight_gaussian(x, line, width) * area
```

### Comparing `dsps-0.1.0/dsps/tests/test_photometry_kernels.py` & `dsps-0.3.0/dsps/photometry/tests/test_photometry_kernels.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 """
 import numpy as np
 import os
 from jax import jit as jjit, vmap
-from ..photometry_kernels import _calc_obs_mag_no_dimming, _calc_rest_mag, _calc_obs_mag
-from ..flat_wcdm import FSPS_COSMO
+from ..photometry_kernels import _calc_obs_mag_no_dimming, calc_rest_mag, calc_obs_mag
+from ...cosmology.flat_wcdm import FSPS_COSMO
 
 
 _THIS_DRNAME = os.path.dirname(os.path.abspath(__file__))
-DATA_DRN = os.path.join(os.path.dirname(_THIS_DRNAME), "data")
+DATA_DRN = os.path.join(
+    os.path.dirname(os.path.dirname(_THIS_DRNAME)), "tests", "testing_data"
+)
 LSST_BAND_FNPAT = "lsst_{}_transmission.npy"
 
-_a = (*[None] * 4, 0, *[None] * 5)
-_calc_obs_mag_vmap_z = jjit(vmap(_calc_obs_mag, in_axes=_a))
+_a = (*[None] * 4, 0, *[None] * 4)
+_calc_obs_mag_vmap_z = jjit(vmap(calc_obs_mag, in_axes=_a))
 
 
 def test_obs_mag_no_dimming_agrees_with_rest_mag_at_z0():
     z_obs = 0.0
     ssp_bnames = ("fsps_ssp_imet_20_iage_5.npy", "fsps_ssp_imet_2_iage_90.npy")
     ssp_fnames = [os.path.join(DATA_DRN, bn) for bn in ssp_bnames]
 
@@ -29,15 +31,15 @@
             fn = os.path.join(DATA_DRN, LSST_BAND_FNPAT.format(band))
             filter_data = np.load(fn)
             band_wave = filter_data["wave"]
             band_trans = filter_data["transmission"]
             mags_obs = _calc_obs_mag_no_dimming(
                 wave_spec, lum_spec, band_wave, band_trans, z_obs
             )
-            mags_rest = _calc_rest_mag(wave_spec, lum_spec, band_wave, band_trans)
+            mags_rest = calc_rest_mag(wave_spec, lum_spec, band_wave, band_trans)
             assert np.allclose(mags_obs, mags_rest)
 
 
 def test_obs_mag_agrees_with_fsps_across_redshift():
     zobs_ray = np.load(os.path.join(DATA_DRN, "fsps_lsst_mags_zobs.npy"))
     ssp_bnames = ("fsps_ssp_imet_20_iage_5.npy", "fsps_ssp_imet_2_iage_90.npy")
     ssp_fnames = [os.path.join(DATA_DRN, bn) for bn in ssp_bnames]
```

### Comparing `dsps-0.1.0/dsps/tests/test_remnant_mass.py` & `dsps-0.3.0/dsps/imf/tests/test_remnant_mass.py`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/test_surviving_mstar.py` & `dsps-0.3.0/dsps/imf/tests/test_surviving_mstar.py`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/calzetti_2000_attenuation.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/calzetti_2000_k_lambda.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/calzetti_2000_wavelength_microns.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/chabrier_mstar_surviving.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/chabrier_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/chabrier_mstar_surviving_norem.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/chabrier_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/galazzi_etal05_mzr.dat` & `dsps-0.3.0/dsps/metallicity/tests/testing_data/galazzi_etal05_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/kirby_etal13_mzr.dat` & `dsps-0.3.0/dsps/metallicity/tests/testing_data/kirby_etal13_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/kroupa_mstar_surviving.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/kroupa_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/kroupa_mstar_surviving_norem.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/kroupa_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/kudritzki_etal16_mzr.dat` & `dsps-0.3.0/dsps/metallicity/tests/testing_data/kudritzki_etal16_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/leitherer_2002_attenuation.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/leitherer_2002_k_lambda.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/leitherer_2002_wavelength_microns.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/lg_ages_mstar_surviving.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/lg_ages_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/lgageray_myr.txt` & `dsps-0.3.0/dsps/tests/testing_data/lgageray_myr.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/maiolino_etal18_mzr.dat` & `dsps-0.3.0/dsps/metallicity/tests/testing_data/maiolino_etal18_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_attenuation1.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_attenuation1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_attenuation2.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_attenuation2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_attenuation3.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_attenuation3.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_k_lambda1.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_k_lambda1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_k_lambda2.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_k_lambda2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_k_lambda3.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_k_lambda3.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/noll_2009_wavelength_microns.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/noll_2009_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salim_2018_attenuation1.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_attenuation1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salim_2018_attenuation2.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_attenuation2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salim_2018_k_lambda1.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_k_lambda1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salim_2018_k_lambda2.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_k_lambda2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salim_2018_wavelength_microns.txt` & `dsps-0.3.0/dsps/dust/tests/testing_data/salim_2018_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salpeter_mstar_surviving.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/salpeter_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/salpeter_mstar_surviving_norem.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/salpeter_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/ssp_plaw_data_c0.txt` & `dsps-0.3.0/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/ssp_plaw_data_c1.txt` & `dsps-0.3.0/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/van_dokkum_mstar_surviving.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/tests/testing_data/van_dokkum_mstar_surviving_norem.txt` & `dsps-0.3.0/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.1.0/dsps/utils.py` & `dsps-0.3.0/dsps/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 """
 from jax import jit as jjit
 from jax import numpy as jnp
-from jax import ops as jops
 from jax import vmap
+from jax import random as jran
 
 
 @jjit
 def _jax_get_dt_array(t):
     dt = jnp.zeros_like(t)
     tmids = 0.5 * (t[:-1] + t[1:])
     dtmids = jnp.diff(tmids)
-    dt = jops.index_update(dt, jops.index[1:-1], dtmids)
+
+    dt = dt.at[1:-1].set(dtmids)
 
     t_lo = t[0] - (t[1] - t[0]) / 2
     t_hi = t[-1] + dtmids[-1] / 2
 
-    dt = jops.index_update(dt, jops.index[0], tmids[0] - t_lo)
-    dt = jops.index_update(dt, jops.index[-1], t_hi - tmids[-1])
+    dt = dt.at[0].set(tmids[0] - t_lo)
+    dt = dt.at[-1].set(t_hi - tmids[-1])
     return dt
 
 
 @jjit
 def _get_bin_edges(bin_mids, lowest_bin_edge, highest_bin_edge):
     """Calculate the lower and upper bounds on the array.
 
@@ -34,30 +35,30 @@
     bin_edges : ndarray of shape (n+1, )
         Integration bounds on the bins
 
     """
     dbins = _jax_get_dt_array(bin_mids)
 
     bin_edges = jnp.zeros(dbins.size + 1)
-    bin_edges = jops.index_update(bin_edges, jops.index[:-1], bin_mids - dbins / 2)
+    bin_edges = bin_edges.at[:-1].set(bin_mids - dbins / 2)
 
-    bin_edges = jops.index_update(bin_edges, jops.index[0], lowest_bin_edge)
-    bin_edges = jops.index_update(bin_edges, jops.index[-1], highest_bin_edge)
+    bin_edges = bin_edges.at[0].set(lowest_bin_edge)
+    bin_edges = bin_edges.at[-1].set(highest_bin_edge)
 
     return bin_edges
 
 
 @jjit
 def _tw_cuml_kern(x, m, h):
     """Triweight kernel version of an err function."""
     z = (x - m) / h
     val = (
-        -5 * z ** 7 / 69984
-        + 7 * z ** 5 / 2592
-        - 35 * z ** 3 / 864
+        -5 * z**7 / 69984
+        + 7 * z**5 / 2592
+        - 35 * z**3 / 864
         + 35 * z / 96
         + 1 / 2
     )
     val = jnp.where(z < -3, 0, val)
     val = jnp.where(z > 3, 1, val)
     return val
 
@@ -66,19 +67,14 @@
 def _tw_sigmoid(x, x0, tw_h, ymin, ymax):
     height_diff = ymax - ymin
     body = _tw_cuml_kern(x, x0, tw_h)
     return ymin + height_diff * body
 
 
 @jjit
-def _get_tw_h_from_sigmoid_k(k):
-    return 1 / (0.614 * k)
-
-
-@jjit
 def _triweighted_histogram_kernel(x, sig, lo, hi):
     """Triweight kernel integrated across the boundaries of a single bin."""
     a = _tw_cuml_kern(x, lo, sig)
     b = _tw_cuml_kern(x, hi, sig)
     return a - b
 
 
@@ -111,43 +107,30 @@
     z = (x - m) / h
     val = 35 / 96 * (1 - (z / 3) ** 2) ** 3 / h
     msk = (z < -3) | (z > 3)
     return jnp.where(msk, 0, val)
 
 
 @jjit
-def interpolate_transmission_curve(wave, trans, n_out, pcut_lo=0, pcut_hi=1):
-    """ """
-    lowest_bin_edge = wave[0] - (wave[1] - wave[0]) / 2
-    highest_bin_edge = wave[-1] + (wave[-1] - wave[-2]) / 2
-    dwave = jnp.diff(_get_bin_edges(wave, lowest_bin_edge, highest_bin_edge))
-    cuml = jnp.cumsum(dwave * trans)
-    cuml = cuml / cuml[-1]
-
-    msk = cuml >= pcut_lo
-    msk &= cuml <= pcut_hi
-
-    wave_lo, wave_hi = dwave[msk][0], dwave[msk][-1]
-    wave_out = jnp.linspace(wave_lo, wave_hi, n_out)
-    trans_out = jnp.jnp.interp(wave_out, wave, trans)
-
-    return wave_out, trans_out
+def _tw_sig_slope(x, xtp, ytp, x0, tw_h, lo, hi):
+    slope = _tw_sigmoid(x, x0, tw_h, lo, hi)
+    return ytp + slope * (x - xtp)
 
 
 @jjit
 def _fill_empty_weights_singlepoint(x, bin_edges, weights):
     zmsk = jnp.all(weights == 0, axis=0)
     lomsk = x < bin_edges[0]
     himsk = x > bin_edges[-1]
 
     lores = jnp.zeros(bin_edges.size - 1)
     hires = jnp.zeros(bin_edges.size - 1)
 
-    lores = jops.index_update(lores, jops.index[0], 1.0)
-    hires = jops.index_update(hires, jops.index[-1], 1.0)
+    lores = lores.at[0].set(1.0)
+    hires = hires.at[-1].set(1.0)
 
     weights = jnp.where(zmsk & lomsk, lores, weights)
     weights = jnp.where(zmsk & himsk, hires, weights)
     return weights
 
 
 @jjit
@@ -166,10 +149,96 @@
 @jjit
 def _sigmoid(x, x0, k, ylo, yhi):
     height_diff = yhi - ylo
     return ylo + height_diff / (1 + jnp.exp(-k * (x - x0)))
 
 
 @jjit
-def _sig_slope(x, y0, x0, slope_k, lo, hi):
+def _inverse_sigmoid(y, x0, k, ylo, yhi):
+    lnarg = (yhi - ylo) / (y - ylo) - 1
+    return x0 - jnp.log(lnarg) / k
+
+
+@jjit
+def _sig_slope(x, xtp, ytp, x0, slope_k, lo, hi):
     slope = _sigmoid(x, x0, slope_k, lo, hi)
-    return y0 + slope * (x - x0)
+    return ytp + slope * (x - xtp)
+
+
+@jjit
+def _mult_2d(w1, w2):
+    return w1 * w2
+
+
+@jjit
+def _mult_3d(w1, w2, w3):
+    return w1 * w2 * w3
+
+
+_mult_2d_vmap = jjit(vmap(vmap(_mult_2d, in_axes=[None, 0]), in_axes=[0, None]))
+_get_weight_matrices_2d = jjit(vmap(_mult_2d_vmap, in_axes=[0, 0]))
+
+
+_mult_3d_vmap = jjit(
+    vmap(
+        vmap(vmap(_mult_3d, in_axes=[None, None, 0]), in_axes=[None, 0, None]),
+        in_axes=[0, None, None],
+    )
+)
+_get_weight_matrices_3d = jjit(vmap(_mult_3d_vmap, in_axes=[0, 0, 0]))
+
+
+@jjit
+def powerlaw_pdf(x, a, b, g):
+    """pdf(x) propto x^{g-1}. Assumes a<b and g!=0
+
+    Parameters
+    ----------
+    x : ndarray of shape (n, )
+        Points at which to evaluate the powerlaw PDF
+
+    a : ndarray of shape (n, )
+        Lower bound on each powerlaw
+
+    b : ndarray of shape (n, )
+        Upper bound on each powerlaw
+
+    g : ndarray of shape (n, )
+        Index for each powerlaw
+
+    Returns
+    -------
+    pdf : ndarray of shape (n, )
+        Value of the PDF for each powerlaw
+
+    """
+    ag, bg = a**g, b**g
+    return g * x ** (g - 1) / (bg - ag)
+
+
+@jjit
+def powerlaw_rvs(ran_key, a, b, g):
+    """Power-law gen for pdf(x) propto x^{g-1} for a<=x<=b. Assumes a<b and g!=0
+
+    Parameters
+    ----------
+    ran_key : jax.random.PRNGKey
+
+    a : ndarray of shape (n, )
+        Lower bound on each powerlaw
+
+    b : ndarray of shape (n, )
+        Upper bound on each powerlaw
+
+    g : ndarray of shape (n, )
+        Index for each powerlaw
+
+    Returns
+    -------
+    y : ndarray of shape (n, )
+        Monte Carlo realization of the input powerlaws
+
+    """
+    npts = a.shape[0]
+    r = jran.uniform(ran_key, (npts,))
+    ag, bg = a**g, b**g
+    return (ag + (bg - ag) * r) ** (1.0 / g)
```

