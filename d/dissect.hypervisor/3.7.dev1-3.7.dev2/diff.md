# Comparing `tmp/dissect.hypervisor-3.7.dev1.tar.gz` & `tmp/dissect.hypervisor-3.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.hypervisor-3.7.dev1.tar", last modified: Wed Apr 19 19:22:12 2023, max compression
+gzip compressed data, was "dissect.hypervisor-3.7.dev2.tar", last modified: Mon May  1 11:38:37 2023, max compression
```

## Comparing `dissect.hypervisor-3.7.dev1.tar` & `dissect.hypervisor-3.7.dev2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.790526 dissect.hypervisor-3.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-19 19:22:12.790526 dissect.hypervisor-3.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.774526 dissect.hypervisor-3.7.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.774526 dissect.hypervisor-3.7.dev1/dissect/hypervisor/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.778526 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/c_vma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/c_wim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/vma.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/wim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/xva.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.778526 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/c_hyperv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/hyperv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/ovf.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/pvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/vbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/vmx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.782526 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_hdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_qcow2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vhdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/hdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/qcow2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vhd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vhdx.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vmdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.782526 dissect.hypervisor-3.7.dev1/dissect/hypervisor/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/tools/envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/tools/vma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.782526 dissect.hypervisor-3.7.dev1/dissect/hypervisor/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/util/envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/dissect/hypervisor/util/vmtar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.774526 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-19 19:22:12.000000 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-19 19:22:12.000000 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:22:12.000000 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-19 19:22:12.000000 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 19:22:12.000000 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 19:22:12.000000 dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-19 19:22:03.000000 dissect.hypervisor-3.7.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:22:12.790526 dissect.hypervisor-3.7.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.782526 dissect.hypervisor-3.7.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.786526 dissect.hypervisor-3.7.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   325934 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/differencing.avhdx.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   145940 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/dynamic.vhd.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   184563 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/dynamic.vhdx.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/encrypted.vmx
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/encryption.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.786526 dissect.hypervisor-3.7.dev1/tests/data/expanding.hdd/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/expanding.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/expanding.hdd/expanding.hdd
--rw-r--r--   0 runner    (1001) docker     (123)   115232 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   151327 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/fixed.vhd.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   162126 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/fixed.vhdx.gz
--rw-r--r--   0 runner    (1001) docker     (123)   110592 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/local.tgz.ve
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.786526 dissect.hypervisor-3.7.dev1/tests/data/plain.hdd/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/plain.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/plain.hdd/plain.hdd
--rw-r--r--   0 runner    (1001) docker     (123)   114982 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)    54881 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/sesparse.vmdk.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:22:12.790526 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)    45092 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/test.VMRS
--rw-r--r--   0 runner    (1001) docker     (123)    16897 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/test.vgz
--rw-r--r--   0 runner    (1001) docker     (123)    65107 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/test.vma.gz
--rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/data/test.vmcx
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_hdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_hyperv.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_pvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vhdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vma.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vmtar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tests/test_vmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-19 19:21:59.000000 dissect.hypervisor-3.7.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.422645 dissect.hypervisor-3.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 11:38:37.422645 dissect.hypervisor-3.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.406645 dissect.hypervisor-3.7.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.410645 dissect.hypervisor-3.7.dev2/dissect/hypervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.410645 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/c_vma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/c_wim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/vma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/wim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/xva.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.410645 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/c_hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/ovf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/vbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/vmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.414645 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_qcow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/qcow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.414645 dissect.hypervisor-3.7.dev2/dissect/hypervisor/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/tools/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/tools/vma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.414645 dissect.hypervisor-3.7.dev2/dissect/hypervisor/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/util/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/dissect/hypervisor/util/vmtar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.410645 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 11:38:37.000000 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-01 11:38:37.000000 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:38:37.000000 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 11:38:37.000000 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-01 11:38:37.000000 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 11:38:37.000000 dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 11:38:27.000000 dissect.hypervisor-3.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 11:38:37.422645 dissect.hypervisor-3.7.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.414645 dissect.hypervisor-3.7.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.418645 dissect.hypervisor-3.7.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   325934 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/differencing.avhdx.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   145940 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/dynamic.vhd.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   184563 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/dynamic.vhdx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/encrypted.vmx
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/encryption.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.418645 dissect.hypervisor-3.7.dev2/tests/data/expanding.hdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/expanding.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/tests/data/expanding.hdd/expanding.hdd
+-rw-r--r--   0 runner    (1001) docker     (123)   115232 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   151327 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/fixed.vhd.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   162126 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/fixed.vhdx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   110592 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/local.tgz.ve
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.418645 dissect.hypervisor-3.7.dev2/tests/data/plain.hdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/plain.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/tests/data/plain.hdd/plain.hdd
+-rw-r--r--   0 runner    (1001) docker     (123)   114982 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    54881 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/sesparse.vmdk.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:37.422645 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:38:23.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    45092 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/test.VMRS
+-rw-r--r--   0 runner    (1001) docker     (123)    16897 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/test.vgz
+-rw-r--r--   0 runner    (1001) docker     (123)    65107 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/test.vma.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/data/test.vmcx
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_pvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vmtar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tests/test_vmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-01 11:38:22.000000 dissect.hypervisor-3.7.dev2/tox.ini
```

### Comparing `dissect.hypervisor-3.7.dev1/LICENSE` & `dissect.hypervisor-3.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/PKG-INFO` & `dissect.hypervisor-3.7.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.hypervisor
-Version: 3.7.dev1
+Version: 3.7.dev2
 Summary: A Dissect module implementing parsers for various hypervisor disk, backup and configuration files
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.hypervisor
 Project-URL: repository, https://github.com/fox-it/dissect.hypervisor
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.hypervisor-3.7.dev1/README.md` & `dissect.hypervisor-3.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/c_vma.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/c_vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/c_wim.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/c_wim.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/vma.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/vma.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         self._devices = {}
         for dev_id, dev_info in enumerate(self.header.dev_info):
             if dev_id == 0 or dev_info.devname_ptr == 0:
                 continue
 
             self._devices[dev_id] = Device(self, dev_id, self.blob_string(dev_info.devname_ptr), dev_info.size)
 
+        self._extent = lru_cache(65536)(self._extent)
+
     @property
     def creation_time(self):
         return ts.from_unix(self.header.ctime)
 
     def blob_data(self, offset):
         if offset not in self._blob_data:
             raise KeyError(f"No blob data for offset {offset}")
@@ -88,15 +90,14 @@
 
     def device(self, dev_id):
         return self._devices[dev_id]
 
     def devices(self):
         return list(self._devices.values())
 
-    @lru_cache(65536)
     def _extent(self, offset):
         return Extent(self.fh, offset)
 
     def extents(self):
         offset = self.header.header_size
         while True:
             try:
@@ -144,14 +145,15 @@
 
         # Keep track of the lowest and highest cluster we have for any device
         # We can use this to speed up extent lookup later on
         # There are at most 59 entries, so safe to parse ahead of use
         self._min = {}
         self._max = {}
         self.blocks = defaultdict(list)
+        block_offset = self.data_offset
         for block_info in self.header.blockinfo:
             cluster_num = block_info & 0xFFFFFFFF
             dev_id = (block_info >> 32) & 0xFF
             mask = block_info >> (32 + 16)
 
             if dev_id == 0:
                 continue
@@ -160,15 +162,22 @@
                 self._min[dev_id] = cluster_num
                 self._max[dev_id] = cluster_num
             elif cluster_num < self._min[dev_id]:
                 self._min[dev_id] = cluster_num
             elif cluster_num > self._max[dev_id]:
                 self._max[dev_id] = cluster_num
 
-            self.blocks[dev_id].append((dev_id, cluster_num, mask))
+            self.blocks[dev_id].append((cluster_num, mask, block_offset))
+
+            if mask == 0xFFFF:
+                block_offset += 16 * c_vma.VMA_BLOCK_SIZE
+            elif mask == 0:
+                pass
+            else:
+                block_offset += bin(mask).count("1") * c_vma.VMA_BLOCK_SIZE
 
     def __repr__(self):
         return f"<Extent offset=0x{self.offset:x} size=0x{self.size:x}>"
 
 
 class DeviceDataStream(AlignedStream):
     def __init__(self, device):
@@ -214,34 +223,26 @@
     for extent in vma.extents():
         if dev_id not in extent.blocks:
             continue
 
         if end < extent._min[dev_id] or cluster > extent._max[dev_id]:
             continue
 
-        block_offset = extent.data_offset
-        for _, cluster_num, mask in extent.blocks[dev_id]:
+        for cluster_num, mask, block_offset in extent.blocks[dev_id]:
             if cluster_num == cluster:
                 yield cluster_num, mask, block_offset
                 cluster += 1
 
                 while cluster in temp:
                     yield temp[cluster]
                     del temp[cluster]
                     cluster += 1
             elif cluster < cluster_num <= end:
                 temp[cluster_num] = (cluster_num, mask, block_offset)
 
-            if mask == 0xFFFF:
-                block_offset += 16 * c_vma.VMA_BLOCK_SIZE
-            elif mask == 0:
-                pass
-            else:
-                block_offset += bin(mask).count("1") * c_vma.VMA_BLOCK_SIZE
-
             if cluster == end:
                 break
 
         if cluster == end:
             break
 
     while cluster in temp:
```

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/backup/xva.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/backup/xva.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/c_hyperv.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/c_hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/hyperv.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/ovf.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/ovf.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/pvs.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/pvs.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/vbox.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/vbox.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/descriptor/vmx.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/descriptor/vmx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_hdd.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_qcow2.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_qcow2.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vdi.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vdi.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vhd.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vhdx.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/c_vmdk.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/c_vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/hdd.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/qcow2.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/qcow2.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vdi.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vdi.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vhd.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vhdx.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/disk/vmdk.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/disk/vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/tools/envelope.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/tools/envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/tools/vma.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/tools/vma.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     logger.addHandler(handler)
     logger.setLevel(level)
 
 
 def main():
     parser = argparse.ArgumentParser(description="VMA extractor")
     parser.add_argument("input", type=Path, help="path to vma file")
-    parser.add_argument("-o", "--output", type=Path, help="path to output directory")
+    parser.add_argument("-o", "--output", type=Path, required=True, help="path to output directory")
     parser.add_argument("-v", "--verbose", action="count", default=3, help="increase output verbosity")
     args = parser.parse_args()
 
     setup_logging(log, args.verbose)
 
     in_file = args.input.resolve()
     if not in_file.exists():
@@ -131,27 +131,26 @@
             task_id = progress.add_task("extract", filename=device.name, total=device.size)
             tasks[device.id] = task_id
             handles[device.id] = out_dir.joinpath(device.name).open("wb")
 
         with progress:
             try:
                 for extent in vma.extents():
-                    data_offset = extent.data_offset
+                    vma.fh.seek(extent.data_offset)
                     for block_info in extent.header.blockinfo:
                         cluster_num = block_info & 0xFFFFFFFF
                         dev_id = (block_info >> 32) & 0xFF
                         mask = block_info >> (32 + 16)
 
                         if dev_id == 0:
                             continue
 
                         fh_out = handles[dev_id]
                         fh_out.seek(cluster_num * c_vma.VMA_CLUSTER_SIZE)
 
-                        vma.fh.seek(data_offset)
                         if mask == 0xFFFF:
                             fh_out.write(vma.fh.read(c_vma.VMA_CLUSTER_SIZE))
                         elif mask == 0:
                             fh_out.write(b"\x00" * c_vma.VMA_CLUSTER_SIZE)
                         else:
                             for allocated, count in _iter_mask(mask, 16):
                                 if allocated:
```

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/util/envelope.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/util/envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect/hypervisor/util/vmtar.py` & `dissect.hypervisor-3.7.dev2/dissect/hypervisor/util/vmtar.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/PKG-INFO` & `dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.hypervisor
-Version: 3.7.dev1
+Version: 3.7.dev2
 Summary: A Dissect module implementing parsers for various hypervisor disk, backup and configuration files
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.hypervisor
 Project-URL: repository, https://github.com/fox-it/dissect.hypervisor
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dissect.hypervisor-3.7.dev1/dissect.hypervisor.egg-info/SOURCES.txt` & `dissect.hypervisor-3.7.dev2/dissect.hypervisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/pyproject.toml` & `dissect.hypervisor-3.7.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/conftest.py` & `dissect.hypervisor-3.7.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/differencing.avhdx.gz` & `dissect.hypervisor-3.7.dev2/tests/data/differencing.avhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/dynamic.vhd.gz` & `dissect.hypervisor-3.7.dev2/tests/data/dynamic.vhd.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/dynamic.vhdx.gz` & `dissect.hypervisor-3.7.dev2/tests/data/dynamic.vhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/encrypted.vmx` & `dissect.hypervisor-3.7.dev2/tests/data/encrypted.vmx`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/expanding.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.7.dev2/tests/data/expanding.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/fixed.vhd.gz` & `dissect.hypervisor-3.7.dev2/tests/data/fixed.vhd.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/fixed.vhdx.gz` & `dissect.hypervisor-3.7.dev2/tests/data/fixed.vhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/local.tgz.ve` & `dissect.hypervisor-3.7.dev2/tests/data/local.tgz.ve`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/plain.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.7.dev2/tests/data/plain.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/sesparse.vmdk.gz` & `dissect.hypervisor-3.7.dev2/tests/data/sesparse.vmdk.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev2/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/test.VMRS` & `dissect.hypervisor-3.7.dev2/tests/data/test.VMRS`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/test.vgz` & `dissect.hypervisor-3.7.dev2/tests/data/test.vgz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/test.vma.gz` & `dissect.hypervisor-3.7.dev2/tests/data/test.vma.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/data/test.vmcx` & `dissect.hypervisor-3.7.dev2/tests/data/test.vmcx`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_envelope.py` & `dissect.hypervisor-3.7.dev2/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_hdd.py` & `dissect.hypervisor-3.7.dev2/tests/test_hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_hyperv.py` & `dissect.hypervisor-3.7.dev2/tests/test_hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_pvs.py` & `dissect.hypervisor-3.7.dev2/tests/test_pvs.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vbox.py` & `dissect.hypervisor-3.7.dev2/tests/test_vbox.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vhd.py` & `dissect.hypervisor-3.7.dev2/tests/test_vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vhdx.py` & `dissect.hypervisor-3.7.dev2/tests/test_vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vma.py` & `dissect.hypervisor-3.7.dev2/tests/test_vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vmdk.py` & `dissect.hypervisor-3.7.dev2/tests/test_vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vmtar.py` & `dissect.hypervisor-3.7.dev2/tests/test_vmtar.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tests/test_vmx.py` & `dissect.hypervisor-3.7.dev2/tests/test_vmx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev1/tox.ini` & `dissect.hypervisor-3.7.dev2/tox.ini`

 * *Files identical despite different names*

