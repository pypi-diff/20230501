# Comparing `tmp/easy_crud_repo_service-0.1.0.tar.gz` & `tmp/easy_crud_repo_service-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_crud_repo_service-0.1.0.tar", max compression
+gzip compressed data, was "easy_crud_repo_service-0.1.1.tar", max compression
```

## Comparing `easy_crud_repo_service-0.1.0.tar` & `easy_crud_repo_service-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,12 @@
--rw-r--r--   0        0        0        0 2023-04-23 19:13:52.339918 easy_crud_repo_service-0.1.0/easy_crud_repo_service/__init__.py
--rw-r--r--   0        0        0      346 2023-04-23 19:13:52.346919 easy_crud_repo_service-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 19:13:52.340970 easy_crud_repo_service-0.1.0/README.md
--rw-r--r--   0        0        0      300 1970-01-01 00:00:00.000000 easy_crud_repo_service-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-23 19:13:52.339918 easy_crud_repo_service-0.1.1/easy_crud_repo_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:59:22.482391 easy_crud_repo_service-0.1.1/easy_crud_repo_service/model/__init__.py
+-rw-r--r--   0        0        0      183 2023-04-23 20:02:18.331784 easy_crud_repo_service-0.1.1/easy_crud_repo_service/model/player.py
+-rw-r--r--   0        0        0      146 2023-04-23 20:02:18.341597 easy_crud_repo_service-0.1.1/easy_crud_repo_service/model/team.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:00:48.714154 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:36:23.143148 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-01 09:50:13.152568 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/builders.py
+-rw-r--r--   0        0        0     1044 2023-05-01 10:25:18.841964 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/get_connection_pool.py
+-rw-r--r--   0        0        0     5106 2023-05-01 11:13:02.644420 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/crud_repo.py
+-rw-r--r--   0        0        0      582 2023-05-01 18:06:47.718354 easy_crud_repo_service-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12849 2023-05-01 15:30:38.823058 easy_crud_repo_service-0.1.1/README.md
+-rw-r--r--   0        0        0    12991 1970-01-01 00:00:00.000000 easy_crud_repo_service-0.1.1/PKG-INFO
```

