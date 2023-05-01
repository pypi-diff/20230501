# Comparing `tmp/types-passlib-1.7.7.8.tar.gz` & `tmp/types-passlib-1.7.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-passlib-1.7.7.8.tar", last modified: Tue Feb  7 01:21:45 2023, max compression
+gzip compressed data, was "types-passlib-1.7.7.9.tar", last modified: Wed Feb 15 12:35:43 2023, max compression
```

## Comparing `types-passlib-1.7.7.8.tar` & `types-passlib-1.7.7.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.796643 types-passlib-1.7.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-07 01:21:44.000000 types-passlib-1.7.7.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-07 01:21:45.000000 types-passlib-1.7.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-07 01:21:45.792643 types-passlib-1.7.7.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.788643 types-passlib-1.7.7.8/passlib-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-07 01:21:44.000000 types-passlib-1.7.7.8/passlib-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/apache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/apps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.788643 types-passlib-1.7.7.8/passlib-stubs/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.788643 types-passlib-1.7.7.8/passlib-stubs/crypto/_blowfish/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/_blowfish/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/_blowfish/_gen_files.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/_blowfish/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/_blowfish/unrolled.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/_md4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/des.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/digest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.788643 types-passlib-1.7.7.8/passlib-stubs/crypto/scrypt/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/scrypt/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/scrypt/_builtin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/scrypt/_gen_files.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/crypto/scrypt/_salsa.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/exc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.788643 types-passlib-1.7.7.8/passlib-stubs/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/ext/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.788643 types-passlib-1.7.7.8/passlib-stubs/ext/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/ext/django/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/ext/django/models.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/ext/django/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.792643 types-passlib-1.7.7.8/passlib-stubs/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/argon2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/bcrypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/cisco.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/des_crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/digests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/django.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/fshp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/ldap_digests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/md5_crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/misc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/mssql.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/oracle.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/pbkdf2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/phpass.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/postgres.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/roundup.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/scram.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/scrypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/sha1_crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/sha2_crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/sun_md5_crypt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/handlers/windows.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/hash.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/hosts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/ifc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/pwd.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/registry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/totp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.792643 types-passlib-1.7.7.8/passlib-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/binary.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.792643 types-passlib-1.7.7.8/passlib-stubs/utils/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/compat/_ordered_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/decor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/des.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/md4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/utils/pbkdf2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-07 01:20:33.000000 types-passlib-1.7.7.8/passlib-stubs/win32.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 01:21:45.796643 types-passlib-1.7.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-07 01:21:44.000000 types-passlib-1.7.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:45.792643 types-passlib-1.7.7.8/types_passlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-07 01:21:45.000000 types-passlib-1.7.7.8/types_passlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-02-07 01:21:45.000000 types-passlib-1.7.7.8/types_passlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 01:21:45.000000 types-passlib-1.7.7.8/types_passlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-07 01:21:45.000000 types-passlib-1.7.7.8/types_passlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.896848 types-passlib-1.7.7.9/passlib-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/passlib-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/apache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/apps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.896848 types-passlib-1.7.7.9/passlib-stubs/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.896848 types-passlib-1.7.7.9/passlib-stubs/crypto/_blowfish/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/_blowfish/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/_blowfish/_gen_files.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/_blowfish/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/_blowfish/unrolled.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/_md4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/des.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/digest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.896848 types-passlib-1.7.7.9/passlib-stubs/crypto/scrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/scrypt/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/scrypt/_builtin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/scrypt/_gen_files.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/crypto/scrypt/_salsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/exc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.896848 types-passlib-1.7.7.9/passlib-stubs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/ext/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.896848 types-passlib-1.7.7.9/passlib-stubs/ext/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/ext/django/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/ext/django/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/ext/django/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/passlib-stubs/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/argon2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/bcrypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/cisco.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/des_crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/digests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/django.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/fshp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/ldap_digests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/md5_crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/misc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/mssql.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/oracle.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/pbkdf2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/phpass.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/postgres.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/roundup.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/scram.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/scrypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/sha1_crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/sha2_crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/sun_md5_crypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/handlers/windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/hash.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/hosts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/ifc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/pwd.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/registry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/totp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/passlib-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/binary.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/passlib-stubs/utils/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/compat/_ordered_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/decor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/des.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/md4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/utils/pbkdf2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-15 12:33:40.000000 types-passlib-1.7.7.9/passlib-stubs/win32.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 12:35:43.900848 types-passlib-1.7.7.9/types_passlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/types_passlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/types_passlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/types_passlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-15 12:35:43.000000 types-passlib-1.7.7.9/types_passlib.egg-info/top_level.txt
```

### Comparing `types-passlib-1.7.7.8/CHANGELOG.md` & `types-passlib-1.7.7.9/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.7.7.9 (2023-02-15)
+
+Use `typing_extensions.Self` instead of `_typeshed.Self` (#9702)
+
 ## 1.7.7.8 (2023-02-07)
 
 Bump mypy to 1.0 (#9684)
 
 ## 1.7.7.7 (2023-02-02)
 
 Manual changes of `Any` union to `Incomplete` in stubs folder (#9566)
```

### Comparing `types-passlib-1.7.7.8/PKG-INFO` & `types-passlib-1.7.7.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-passlib
-Version: 1.7.7.8
+Version: 1.7.7.9
 Summary: Typing stubs for passlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/passlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `passlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/passlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c4c4bee8aa368b8c05d06559904531596e8a7be6`.
+This package was generated from typeshed commit `7180d0223b3cfb0275bdc4dff902439536dd4e3d`.
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/apache.pyi` & `types-passlib-1.7.7.9/passlib-stubs/apache.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/apps.pyi` & `types-passlib-1.7.7.9/passlib-stubs/apps.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/context.pyi` & `types-passlib-1.7.7.9/passlib-stubs/context.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from _typeshed import Incomplete, Self, StrOrBytesPath, SupportsItems
+from _typeshed import Incomplete, StrOrBytesPath, SupportsItems
 from typing import Any
+from typing_extensions import Self
 
 class CryptPolicy:
     @classmethod
     def from_path(cls, path, section: str = ..., encoding: str = ...): ...
     @classmethod
     def from_string(cls, source, section: str = ..., encoding: str = ...): ...
     @classmethod
@@ -22,17 +23,17 @@
     def iter_config(self, ini: bool = ..., resolve: bool = ...): ...
     def to_dict(self, resolve: bool = ...): ...
     def to_file(self, stream, section: str = ...) -> None: ...
     def to_string(self, section: str = ..., encoding: Incomplete | None = ...): ...
 
 class CryptContext:
     @classmethod
-    def from_string(cls: type[Self], source: str | bytes, section: str = ..., encoding: str = ...) -> Self: ...
+    def from_string(cls, source: str | bytes, section: str = ..., encoding: str = ...) -> Self: ...
     @classmethod
-    def from_path(cls: type[Self], path: StrOrBytesPath, section: str = ..., encoding: str = ...) -> Self: ...
+    def from_path(cls, path: StrOrBytesPath, section: str = ..., encoding: str = ...) -> Self: ...
     def copy(self, **kwds: Any) -> CryptContext: ...
     def using(self, **kwds: Any) -> CryptContext: ...
     def replace(self, **kwds): ...
     def __init__(self, schemes: Incomplete | None = ..., policy=..., _autoload: bool = ..., **kwds) -> None: ...
     policy: CryptPolicy
     def load_path(self, path: StrOrBytesPath, update: bool = ..., section: str = ..., encoding: str = ...) -> None: ...
     def load(
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/crypto/digest.pyi` & `types-passlib-1.7.7.9/passlib-stubs/crypto/digest.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/exc.pyi` & `types-passlib-1.7.7.9/passlib-stubs/exc.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/ext/django/utils.pyi` & `types-passlib-1.7.7.9/passlib-stubs/ext/django/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/argon2.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/argon2.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/bcrypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/bcrypt.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/cisco.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/cisco.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/des_crypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/des_crypt.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/digests.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/digests.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/django.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/django.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/fshp.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/fshp.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/ldap_digests.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/ldap_digests.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/md5_crypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/md5_crypt.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/misc.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/misc.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/mssql.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/mssql.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/oracle.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/oracle.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/pbkdf2.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/pbkdf2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from _typeshed import Self
 from typing import ClassVar
+from typing_extensions import Self
 
 import passlib.utils.handlers as uh
 from passlib.utils.handlers import PrefixWrapper
 
 class Pbkdf2DigestHandler(uh.HasRounds, uh.HasRawSalt, uh.HasRawChecksum, uh.GenericHandler):  # type: ignore[misc]
     checksum_chars: ClassVar[str]
     default_salt_size: ClassVar[int]
     max_salt_size: ClassVar[int]
     default_rounds: ClassVar[int]
     min_rounds: ClassVar[int]
     max_rounds: ClassVar[int]
     rounds_cost: ClassVar[str]
     @classmethod
-    def from_string(cls: type[Self], hash: str | bytes) -> Self: ...  # type: ignore[override]
+    def from_string(cls, hash: str | bytes) -> Self: ...  # type: ignore[override]
 
 # dynamically created by create_pbkdf2_hash()
 class pbkdf2_sha1(Pbkdf2DigestHandler):
     name: ClassVar[str]
     ident: ClassVar[str]
     checksum_size: ClassVar[int]
     encoded_checksum_size: ClassVar[int]
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/phpass.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/phpass.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from _typeshed import Self
 from typing import ClassVar
+from typing_extensions import Self
 
 import passlib.utils.handlers as uh
 
 class phpass(uh.HasManyIdents, uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
     name: ClassVar[str]
     checksum_chars: ClassVar[str]
     min_salt_size: ClassVar[int]
@@ -13,8 +13,8 @@
     min_rounds: ClassVar[int]
     max_rounds: ClassVar[int]
     rounds_cost: ClassVar[str]
     default_ident: ClassVar[str]
     ident_values: ClassVar[tuple[str, ...]]
     ident_aliases: ClassVar[dict[str, str]]
     @classmethod
-    def from_string(cls: type[Self], hash: str | bytes) -> Self: ...  # type: ignore[override]
+    def from_string(cls, hash: str | bytes) -> Self: ...  # type: ignore[override]
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/scram.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/scram.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/scrypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/scrypt.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/sha1_crypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/sha2_crypt.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from _typeshed import Self
-from typing import Any, ClassVar
+from typing import ClassVar
+from typing_extensions import Self
 
 import passlib.utils.handlers as uh
 
-log: Any
-
-class sha1_crypt(uh.HasManyBackends, uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
-    name: ClassVar[str]
-    ident: ClassVar[str]
-    checksum_size: ClassVar[int]
+class _SHA2_Common(uh.HasManyBackends, uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
     checksum_chars: ClassVar[str]
-    default_salt_size: ClassVar[int]
     max_salt_size: ClassVar[int]
     salt_chars: ClassVar[str]
-    default_rounds: ClassVar[int]
     min_rounds: ClassVar[int]
     max_rounds: ClassVar[int]
     rounds_cost: ClassVar[str]
+    implicit_rounds: bool
+    def __init__(self, implicit_rounds: bool | None = ..., **kwds) -> None: ...
     @classmethod
-    def from_string(cls: type[Self], hash: str | bytes) -> Self: ...  # type: ignore[override]
-    def to_string(self, config: bool = ...) -> str: ...
+    def from_string(cls, hash: str | bytes) -> Self: ...  # type: ignore[override]
     backends: ClassVar[tuple[str, ...]]
+
+class sha256_crypt(_SHA2_Common):
+    name: ClassVar[str]
+    ident: ClassVar[str]
+    checksum_size: ClassVar[int]
+    default_rounds: ClassVar[int]
+
+class sha512_crypt(_SHA2_Common):
+    name: ClassVar[str]
+    ident: ClassVar[str]
+    checksum_size: ClassVar[int]
+    default_rounds: ClassVar[int]
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/sha2_crypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/sun_md5_crypt.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-from _typeshed import Self
 from typing import ClassVar
+from typing_extensions import Self
 
 import passlib.utils.handlers as uh
 
-class _SHA2_Common(uh.HasManyBackends, uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
+class sun_md5_crypt(uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
+    name: ClassVar[str]
     checksum_chars: ClassVar[str]
-    max_salt_size: ClassVar[int]
+    checksum_size: ClassVar[int]
+    default_salt_size: ClassVar[int]
+    max_salt_size: ClassVar[int | None]
     salt_chars: ClassVar[str]
+    default_rounds: ClassVar[int]
     min_rounds: ClassVar[int]
     max_rounds: ClassVar[int]
     rounds_cost: ClassVar[str]
-    implicit_rounds: bool
-    def __init__(self, implicit_rounds: bool | None = ..., **kwds) -> None: ...
+    ident_values: ClassVar[tuple[str, ...]]
+    bare_salt: bool
+    def __init__(self, bare_salt: bool = ..., **kwds) -> None: ...
     @classmethod
-    def from_string(cls: type[Self], hash: str | bytes) -> Self: ...  # type: ignore[override]
-    backends: ClassVar[tuple[str, ...]]
-
-class sha256_crypt(_SHA2_Common):
-    name: ClassVar[str]
-    ident: ClassVar[str]
-    checksum_size: ClassVar[int]
-    default_rounds: ClassVar[int]
-
-class sha512_crypt(_SHA2_Common):
-    name: ClassVar[str]
-    ident: ClassVar[str]
-    checksum_size: ClassVar[int]
-    default_rounds: ClassVar[int]
+    def identify(cls, hash): ...
+    @classmethod
+    def from_string(cls, hash: str | bytes) -> Self: ...  # type: ignore[override]
+    def to_string(self, _withchk: bool = ...) -> str: ...
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/sun_md5_crypt.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/sha1_crypt.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from _typeshed import Self
-from typing import ClassVar
+from typing import Any, ClassVar
+from typing_extensions import Self
 
 import passlib.utils.handlers as uh
 
-class sun_md5_crypt(uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
+log: Any
+
+class sha1_crypt(uh.HasManyBackends, uh.HasRounds, uh.HasSalt, uh.GenericHandler):  # type: ignore[misc]
     name: ClassVar[str]
-    checksum_chars: ClassVar[str]
+    ident: ClassVar[str]
     checksum_size: ClassVar[int]
+    checksum_chars: ClassVar[str]
     default_salt_size: ClassVar[int]
-    max_salt_size: ClassVar[int | None]
+    max_salt_size: ClassVar[int]
     salt_chars: ClassVar[str]
     default_rounds: ClassVar[int]
     min_rounds: ClassVar[int]
     max_rounds: ClassVar[int]
     rounds_cost: ClassVar[str]
-    ident_values: ClassVar[tuple[str, ...]]
-    bare_salt: bool
-    def __init__(self, bare_salt: bool = ..., **kwds) -> None: ...
-    @classmethod
-    def identify(cls, hash): ...
     @classmethod
-    def from_string(cls: type[Self], hash: str | bytes) -> Self: ...  # type: ignore[override]
-    def to_string(self, _withchk: bool = ...) -> str: ...
+    def from_string(cls, hash: str | bytes) -> Self: ...  # type: ignore[override]
+    def to_string(self, config: bool = ...) -> str: ...
+    backends: ClassVar[tuple[str, ...]]
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/handlers/windows.pyi` & `types-passlib-1.7.7.9/passlib-stubs/handlers/windows.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/hash.pyi` & `types-passlib-1.7.7.9/passlib-stubs/hash.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/ifc.pyi` & `types-passlib-1.7.7.9/passlib-stubs/ifc.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from _typeshed import Self
 from abc import ABCMeta, abstractmethod
 from typing import Any, ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, Self
 
 class PasswordHash(metaclass=ABCMeta):
     is_disabled: ClassVar[bool]
     truncate_size: ClassVar[int | None]
     truncate_error: ClassVar[bool]
     truncate_verify_reject: ClassVar[bool]
     @classmethod
@@ -14,15 +13,15 @@
     @classmethod
     def encrypt(cls, secret: str | bytes, **kwds) -> str: ...
     @classmethod
     @abstractmethod
     def verify(cls, secret: str | bytes, hash: str | bytes, **context_kwds): ...
     @classmethod
     @abstractmethod
-    def using(cls: type[Self], relaxed: bool = ..., **kwds: Any) -> type[Self]: ...
+    def using(cls, relaxed: bool = ..., **kwds: Any) -> type[Self]: ...
     @classmethod
     def needs_update(cls, hash: str, secret: str | bytes | None = ...) -> bool: ...
     @classmethod
     @abstractmethod
     def identify(cls, hash: str | bytes) -> bool: ...
     @classmethod
     def genconfig(cls, **setting_kwds: Any) -> str: ...
```

### Comparing `types-passlib-1.7.7.8/passlib-stubs/pwd.pyi` & `types-passlib-1.7.7.9/passlib-stubs/pwd.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/totp.pyi` & `types-passlib-1.7.7.9/passlib-stubs/totp.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/utils/__init__.pyi` & `types-passlib-1.7.7.9/passlib-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/utils/binary.pyi` & `types-passlib-1.7.7.9/passlib-stubs/utils/binary.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/utils/compat/_ordered_dict.pyi` & `types-passlib-1.7.7.9/passlib-stubs/utils/compat/_ordered_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/utils/decor.pyi` & `types-passlib-1.7.7.9/passlib-stubs/utils/decor.pyi`

 * *Files identical despite different names*

### Comparing `types-passlib-1.7.7.8/passlib-stubs/utils/handlers.pyi` & `types-passlib-1.7.7.9/passlib-stubs/utils/handlers.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
-from _typeshed import Incomplete, Self
+from _typeshed import Incomplete
 from typing import Any, ClassVar
+from typing_extensions import Self
 
 from passlib.ifc import PasswordHash
 from passlib.utils.binary import BASE64_CHARS, HASH64_CHARS, LOWER_HEX_CHARS, PADDED_BASE64_CHARS, UPPER_HEX_CHARS
 
 H64_CHARS = HASH64_CHARS
 B64_CHARS = BASE64_CHARS
 PADDED_B64_CHARS = PADDED_BASE64_CHARS
@@ -16,35 +17,35 @@
     hash, prefix, sep=..., rounds_base: int = ..., default_rounds: Incomplete | None = ..., handler: Incomplete | None = ...
 ): ...
 def render_mc2(ident, salt, checksum, sep=...): ...
 def render_mc3(ident, rounds, salt, checksum, sep=..., rounds_base: int = ...): ...
 
 class MinimalHandler(PasswordHash, metaclass=abc.ABCMeta):
     @classmethod
-    def using(cls: Self, relaxed: bool = ...) -> type[Self]: ...  # type: ignore[override]
+    def using(cls, relaxed: bool = ...) -> type[Self]: ...  # type: ignore[override]
 
 class TruncateMixin(MinimalHandler, metaclass=abc.ABCMeta):
     truncate_error: ClassVar[bool]
     truncate_verify_reject: ClassVar[bool]
     @classmethod
-    def using(cls: type[Self], truncate_error: object = ..., *, relaxed: bool = ...) -> type[Self]: ...  # type: ignore[override]
+    def using(cls, truncate_error: object = ..., *, relaxed: bool = ...) -> type[Self]: ...  # type: ignore[override]
 
 class GenericHandler(MinimalHandler):
     setting_kwds: ClassVar[tuple[str, ...]]
     context_kwds: ClassVar[tuple[str, ...]]
     ident: ClassVar[str | None]
     checksum_size: ClassVar[int | None]
     checksum_chars: ClassVar[str | None]
     checksum: str | None
     use_defaults: bool
     def __init__(self, checksum: str | None = ..., use_defaults: bool = ...) -> None: ...
     @classmethod
     def identify(cls, hash: str | bytes) -> bool: ...
     @classmethod
-    def from_string(cls: type[Self], hash: str | bytes, **context: Any) -> Self: ...
+    def from_string(cls, hash: str | bytes, **context: Any) -> Self: ...
     def to_string(self) -> str: ...
     @classmethod
     def hash(cls, secret: str | bytes, **kwds: Any) -> str: ...
     @classmethod
     def verify(cls, secret: str | bytes, hash: str | bytes, **context: Any) -> bool: ...
     @classmethod
     def genconfig(cls, **kwds: Any) -> str: ...
```

### Comparing `types-passlib-1.7.7.8/setup.py` & `types-passlib-1.7.7.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `passlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/passlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c4c4bee8aa368b8c05d06559904531596e8a7be6`.
+This package was generated from typeshed commit `7180d0223b3cfb0275bdc4dff902439536dd4e3d`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.7.7.8",
+      version="1.7.7.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/passlib.md",
```

### Comparing `types-passlib-1.7.7.8/types_passlib.egg-info/PKG-INFO` & `types-passlib-1.7.7.9/types_passlib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-passlib
-Version: 1.7.7.8
+Version: 1.7.7.9
 Summary: Typing stubs for passlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/passlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `passlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/passlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c4c4bee8aa368b8c05d06559904531596e8a7be6`.
+This package was generated from typeshed commit `7180d0223b3cfb0275bdc4dff902439536dd4e3d`.
```

### Comparing `types-passlib-1.7.7.8/types_passlib.egg-info/SOURCES.txt` & `types-passlib-1.7.7.9/types_passlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

