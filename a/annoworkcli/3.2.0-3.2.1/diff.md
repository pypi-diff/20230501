# Comparing `tmp/annoworkcli-3.2.0.tar.gz` & `tmp/annoworkcli-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkcli-3.2.0.tar", max compression
+gzip compressed data, was "annoworkcli-3.2.1.tar", max compression
```

## Comparing `annoworkcli-3.2.0.tar` & `annoworkcli-3.2.1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     2244 2022-06-03 05:42:00.302116 annoworkcli-3.2.0/README.md
--rw-r--r--   0        0        0       71 2021-11-08 13:55:41.000000 annoworkcli-3.2.0/annoworkcli/__init__.py
--rw-r--r--   0        0        0     2496 2022-06-03 05:42:00.302116 annoworkcli-3.2.0/annoworkcli/__main__.py
--rw-r--r--   0        0        0       22 2023-03-01 16:09:59.301047 annoworkcli-3.2.0/annoworkcli/__version__.py
--rw-r--r--   0        0        0        0 2021-10-22 07:15:52.000000 annoworkcli-3.2.0/annoworkcli/account/__init__.py
--rw-r--r--   0        0        0     2901 2022-05-18 03:17:57.097876 annoworkcli-3.2.0/annoworkcli/account/list_external_linkage_info.py
--rw-r--r--   0        0        0     2398 2022-01-28 05:27:46.263641 annoworkcli-3.2.0/annoworkcli/account/put_external_linkage_info.py
--rw-r--r--   0        0        0      879 2023-03-01 16:10:06.953050 annoworkcli-3.2.0/annoworkcli/account/subcommand.py
--rw-r--r--   0        0        0        0 2021-10-22 07:15:52.000000 annoworkcli-3.2.0/annoworkcli/actual_working_time/__init__.py
--rw-r--r--   0        0        0     7614 2022-05-23 05:57:24.376384 annoworkcli-3.2.0/annoworkcli/actual_working_time/delete_actual_working_time.py
--rw-r--r--   0        0        0    14541 2022-07-29 04:34:41.795672 annoworkcli-3.2.0/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
--rw-r--r--   0        0        0    13292 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    15229 2023-03-01 16:10:07.577050 annoworkcli-3.2.0/annoworkcli/actual_working_time/list_actual_working_time.py
--rw-r--r--   0        0        0     1408 2023-03-01 16:10:06.957050 annoworkcli-3.2.0/annoworkcli/actual_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2021-11-04 02:49:44.000000 annoworkcli-3.2.0/annoworkcli/annofab/__init__.py
--rw-r--r--   0        0        0     8540 2022-07-29 04:49:59.019672 annoworkcli-3.2.0/annoworkcli/annofab/list_job_with_annofab_project.py
--rw-r--r--   0        0        0    21710 2023-03-01 16:10:07.761050 annoworkcli-3.2.0/annoworkcli/annofab/list_working_hours.py
--rw-r--r--   0        0        0     5210 2023-03-01 16:10:07.081050 annoworkcli-3.2.0/annoworkcli/annofab/put_account_external_linkage_info.py
--rw-r--r--   0        0        0     3953 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/annofab/put_job_from_annofab_project.py
--rw-r--r--   0        0        0    51720 2023-03-01 16:10:08.717050 annoworkcli-3.2.0/annoworkcli/annofab/reshape_working_hours.py
--rw-r--r--   0        0        0     1515 2023-03-01 16:10:06.997050 annoworkcli-3.2.0/annoworkcli/annofab/subcommand.py
--rw-r--r--   0        0        0    11287 2022-06-21 08:38:11.740049 annoworkcli-3.2.0/annoworkcli/annofab/visualize_statistics.py
--rw-r--r--   0        0        0        0 2020-10-08 11:25:00.000000 annoworkcli-3.2.0/annoworkcli/common/__init__.py
--rw-r--r--   0        0        0      846 2021-12-02 06:11:59.000000 annoworkcli-3.2.0/annoworkcli/common/annofab.py
--rw-r--r--   0        0        0     9053 2022-08-12 05:58:03.457444 annoworkcli-3.2.0/annoworkcli/common/cli.py
--rw-r--r--   0        0        0       92 2021-03-12 06:36:23.000000 annoworkcli-3.2.0/annoworkcli/common/exeptions.py
--rw-r--r--   0        0        0       78 2021-11-15 16:42:45.000000 annoworkcli-3.2.0/annoworkcli/common/job.py
--rw-r--r--   0        0        0     4364 2022-07-29 04:34:41.799672 annoworkcli-3.2.0/annoworkcli/common/utils.py
--rw-r--r--   0        0        0      923 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/common/workspace_tag.py
--rw-r--r--   0        0        0      829 2022-01-28 07:57:32.319641 annoworkcli-3.2.0/annoworkcli/data/logging.yaml
--rw-r--r--   0        0        0        0 2021-10-22 07:15:52.000000 annoworkcli-3.2.0/annoworkcli/expected_working_time/__init__.py
--rw-r--r--   0        0        0     3858 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/expected_working_time/delete_expected_working_time.py
--rw-r--r--   0        0        0     6739 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/expected_working_time/list_expected_working_time.py
--rw-r--r--   0        0        0     8777 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
--rw-r--r--   0        0        0     5351 2023-02-07 08:53:12.361532 annoworkcli-3.2.0/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
--rw-r--r--   0        0        0     1296 2023-03-01 16:10:07.005050 annoworkcli-3.2.0/annoworkcli/expected_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2021-10-22 07:15:52.000000 annoworkcli-3.2.0/annoworkcli/job/__init__.py
--rw-r--r--   0        0        0     4038 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/job/change_job_properties.py
--rw-r--r--   0        0        0     3326 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/job/delete_job.py
--rw-r--r--   0        0        0     6284 2023-03-01 16:10:07.377050 annoworkcli-3.2.0/annoworkcli/job/list_job.py
--rw-r--r--   0        0        0      885 2023-03-01 16:10:07.041050 annoworkcli-3.2.0/annoworkcli/job/subcommand.py
--rw-r--r--   0        0        0        0 2021-10-22 07:15:52.000000 annoworkcli-3.2.0/annoworkcli/my/__init__.py
--rw-r--r--   0        0        0     1404 2021-11-30 01:58:59.000000 annoworkcli-3.2.0/annoworkcli/my/get_my_account.py
--rw-r--r--   0        0        0     2361 2022-08-12 05:58:03.457444 annoworkcli-3.2.0/annoworkcli/my/list_my_workspace_member.py
--rw-r--r--   0        0        0      816 2023-03-01 16:10:07.065050 annoworkcli-3.2.0/annoworkcli/my/subcommand.py
--rw-r--r--   0        0        0        0 2021-11-04 06:31:02.000000 annoworkcli-3.2.0/annoworkcli/schedule/__init__.py
--rw-r--r--   0        0        0     8172 2023-03-01 16:10:07.653050 annoworkcli-3.2.0/annoworkcli/schedule/list_assigned_hours_daily.py
--rw-r--r--   0        0        0     9204 2023-03-01 16:10:07.441050 annoworkcli-3.2.0/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    11024 2023-03-01 16:10:07.885050 annoworkcli-3.2.0/annoworkcli/schedule/list_schedule.py
--rw-r--r--   0        0        0      995 2023-03-01 16:10:07.465050 annoworkcli-3.2.0/annoworkcli/schedule/subcommand.py
--rw-r--r--   0        0        0     3276 2022-08-12 05:58:03.457444 annoworkcli-3.2.0/annoworkcli/workspace/list_workspace.py
--rw-r--r--   0        0        0     2141 2022-08-12 05:58:03.461446 annoworkcli-3.2.0/annoworkcli/workspace/put_workspace.py
--rw-r--r--   0        0        0      847 2023-03-01 16:10:07.501050 annoworkcli-3.2.0/annoworkcli/workspace/subcommand.py
--rw-r--r--   0        0        0        0 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/workspace_member/__init__.py
--rw-r--r--   0        0        0     5048 2022-08-12 05:58:03.461446 annoworkcli-3.2.0/annoworkcli/workspace_member/append_tag_to_workspace_member.py
--rw-r--r--   0        0        0     4601 2022-08-12 05:58:03.461446 annoworkcli-3.2.0/annoworkcli/workspace_member/change_workspace_member_properties.py
--rw-r--r--   0        0        0     2897 2022-08-12 05:58:03.461446 annoworkcli-3.2.0/annoworkcli/workspace_member/delete_workspace_member.py
--rw-r--r--   0        0        0     6248 2022-08-12 05:58:03.465448 annoworkcli-3.2.0/annoworkcli/workspace_member/list_workspace_member.py
--rw-r--r--   0        0        0     4725 2022-08-12 05:58:03.465448 annoworkcli-3.2.0/annoworkcli/workspace_member/put_workspace_member.py
--rw-r--r--   0        0        0     5079 2022-08-12 05:58:03.465448 annoworkcli-3.2.0/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
--rw-r--r--   0        0        0     1518 2023-03-01 16:10:07.557050 annoworkcli-3.2.0/annoworkcli/workspace_member/subcommand.py
--rw-r--r--   0        0        0        0 2022-05-23 05:57:24.380384 annoworkcli-3.2.0/annoworkcli/workspace_tag/__init__.py
--rw-r--r--   0        0        0     2645 2022-08-12 05:58:03.469450 annoworkcli-3.2.0/annoworkcli/workspace_tag/list_workspace_tag.py
--rw-r--r--   0        0        0     2561 2022-08-12 05:58:03.469450 annoworkcli-3.2.0/annoworkcli/workspace_tag/put_workspace_tag.py
--rw-r--r--   0        0        0      877 2023-03-01 16:10:07.625050 annoworkcli-3.2.0/annoworkcli/workspace_tag/subcommand.py
--rw-r--r--   0        0        0     1961 2023-03-01 16:09:53.329045 annoworkcli-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 annoworkcli-3.2.0/setup.py
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 annoworkcli-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2244 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/README.md
+-rw-r--r--   0        0        0       71 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/list_external_linkage_info.py
+-rw-r--r--   0        0        0     2398 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/put_external_linkage_info.py
+-rw-r--r--   0        0        0      879 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/account/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/__init__.py
+-rw-r--r--   0        0        0     7614 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/delete_actual_working_time.py
+-rw-r--r--   0        0        0    14541 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
+-rw-r--r--   0        0        0    13292 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    15229 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_time.py
+-rw-r--r--   0        0        0     1408 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/actual_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/__init__.py
+-rw-r--r--   0        0        0     8540 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/list_job_with_annofab_project.py
+-rw-r--r--   0        0        0    22039 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/list_working_hours.py
+-rw-r--r--   0        0        0     5210 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/put_account_external_linkage_info.py
+-rw-r--r--   0        0        0     3953 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/put_job_from_annofab_project.py
+-rw-r--r--   0        0        0    51720 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/reshape_working_hours.py
+-rw-r--r--   0        0        0     1515 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/subcommand.py
+-rw-r--r--   0        0        0    11287 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/annofab/visualize_statistics.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/__init__.py
+-rw-r--r--   0        0        0      846 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/annofab.py
+-rw-r--r--   0        0        0     9053 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/cli.py
+-rw-r--r--   0        0        0       92 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/exeptions.py
+-rw-r--r--   0        0        0       78 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/job.py
+-rw-r--r--   0        0        0     4364 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/utils.py
+-rw-r--r--   0        0        0      923 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/common/workspace_tag.py
+-rw-r--r--   0        0        0      829 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/data/logging.yaml
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/__init__.py
+-rw-r--r--   0        0        0     3858 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/delete_expected_working_time.py
+-rw-r--r--   0        0        0     6739 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time.py
+-rw-r--r--   0        0        0     8777 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
+-rw-r--r--   0        0        0     5351 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
+-rw-r--r--   0        0        0     1296 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/expected_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/job/__init__.py
+-rw-r--r--   0        0        0     4038 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/job/change_job_properties.py
+-rw-r--r--   0        0        0     3326 2023-05-01 06:29:38.428616 annoworkcli-3.2.1/annoworkcli/job/delete_job.py
+-rw-r--r--   0        0        0     6284 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/job/list_job.py
+-rw-r--r--   0        0        0      885 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/job/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/get_my_account.py
+-rw-r--r--   0        0        0     2361 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/list_my_workspace_member.py
+-rw-r--r--   0        0        0      816 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/my/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/__init__.py
+-rw-r--r--   0        0        0     8172 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily.py
+-rw-r--r--   0        0        0     9204 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    11024 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/list_schedule.py
+-rw-r--r--   0        0        0      995 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/schedule/subcommand.py
+-rw-r--r--   0        0        0     3276 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace/list_workspace.py
+-rw-r--r--   0        0        0     2141 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace/put_workspace.py
+-rw-r--r--   0        0        0      847 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/__init__.py
+-rw-r--r--   0        0        0     5048 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/append_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     4601 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/change_workspace_member_properties.py
+-rw-r--r--   0        0        0     2897 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/delete_workspace_member.py
+-rw-r--r--   0        0        0     6248 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/list_workspace_member.py
+-rw-r--r--   0        0        0     4725 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/put_workspace_member.py
+-rw-r--r--   0        0        0     5079 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     1518 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_member/subcommand.py
+-rw-r--r--   0        0        0        0 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/__init__.py
+-rw-r--r--   0        0        0     2645 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/list_workspace_tag.py
+-rw-r--r--   0        0        0     2576 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/put_workspace_tag.py
+-rw-r--r--   0        0        0      877 2023-05-01 06:29:38.432616 annoworkcli-3.2.1/annoworkcli/workspace_tag/subcommand.py
+-rw-r--r--   0        0        0     1907 2023-05-01 06:29:38.436617 annoworkcli-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 annoworkcli-3.2.1/PKG-INFO
```

### Comparing `annoworkcli-3.2.0/README.md` & `annoworkcli-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/__main__.py` & `annoworkcli-3.2.1/annoworkcli/__main__.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/account/list_external_linkage_info.py` & `annoworkcli-3.2.1/annoworkcli/account/list_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/account/put_external_linkage_info.py` & `annoworkcli-3.2.1/annoworkcli/account/put_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/account/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/account/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/actual_working_time/delete_actual_working_time.py` & `annoworkcli-3.2.1/annoworkcli/actual_working_time/delete_actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/actual_working_time/list_actual_working_hours_daily.py` & `annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py` & `annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/actual_working_time/list_actual_working_time.py` & `annoworkcli-3.2.1/annoworkcli/actual_working_time/list_actual_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/actual_working_time/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/actual_working_time/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/list_job_with_annofab_project.py` & `annoworkcli-3.2.1/annoworkcli/annofab/list_job_with_annofab_project.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/list_working_hours.py` & `annoworkcli-3.2.1/annoworkcli/annofab/list_working_hours.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,39 @@
 from annoworkcli.common.annofab import TIMEZONE_OFFSET_HOURS, get_annofab_project_id_from_job, isoduration_to_hour
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
-def _get_get_df_working_hours_from_df(
+def _get_df_working_hours_from_df(
     *,
     df_actual_working_hours: pandas.DataFrame,
     df_user_and_af_account: pandas.DataFrame,
     df_job_and_af_project: pandas.DataFrame,
     df_af_working_hours: pandas.DataFrame,
 ) -> pandas.DataFrame:
+    """
+    引数で受け取ったDataFrameをマージしたDataFrameを返します。
+
+    Args:
+        df_actual_working_hours: 実績作業時間情報
+        df_user_and_af_account: ユーザ情報とAnnofabアカウント情報
+        df_job_and_af_project: ジョブ情報とAnnofabプロジェクト情報
+        df_af_working_hours: Annofabの作業時間情報
+    """
     # annowork側の作業時間情報
     df_aw_working_hours = df_actual_working_hours.merge(
         df_user_and_af_account[["user_id", "annofab_account_id"]], how="left", on="user_id"
     ).merge(
         df_job_and_af_project[["job_id", "annofab_project_id"]],
         how="left",
         on="job_id",
     )
 
-    if len(df_af_working_hours) == 0:
-        logger.warning(f"Annofabの作業時間情報が0件でした。")
-        df_aw_working_hours["annofab_working_hours"] = 0
-        return df_aw_working_hours
-
     df_merged = df_aw_working_hours.merge(
         df_af_working_hours, how="outer", on=["date", "annofab_project_id", "annofab_account_id"]
     )
 
     TMP_SUFFIX = "_tmp"
     # df_merged は outer joinしているため、左側にも欠損値ができる。
     # それを埋めるために、以前に user情報, job情報の一意な dataframe を生成して、欠損値を埋める
@@ -80,15 +84,14 @@
     df_merged["job_name"].fillna(df_merged[f"job_name{TMP_SUFFIX}"], inplace=True)
 
     # annofab_project_titleを結合するために、annofab_projectだけのDataFrameを生成する
     df_af_project = df_job_and_af_project.drop_duplicates(subset=["annofab_project_id"])[
         ["annofab_project_id", "annofab_project_title"]
     ]
     df_merged = df_merged.merge(df_af_project, on="annofab_project_id", how="left")
-
     df_merged.fillna(
         {
             "actual_working_hours": 0,
             "annofab_working_hours": 0,
         },
         inplace=True,
     )
@@ -177,19 +180,21 @@
 
         df = df_user.merge(df_af_account, how="inner", on="user_id")
         return df
 
     def _get_df_job_and_af_project(self, job_ids: Collection[str]) -> pandas.DataFrame:
         """
         job_idとAnnofabのプロジェクト情報が格納されたpandas.DataFrameを返します。
-        以下の列を持ちます。
-            * job_id
-            * annofab_project_id
-            * annofab_project_title
 
+        Returns:
+            job_idとAnnofabのプロジェクト情報が格納されたpandas.DataFrame。
+            以下の列が存在します。
+                * job_id
+                * annofab_project_id
+                * annofab_project_title
         """
 
         def get_project_title(project_id: str) -> Optional[str]:
             project = self.annofab_service.wrapper.get_project_or_none(project_id)
             if project is None:
                 return None
             return project["title"]
@@ -242,15 +247,15 @@
         return result
 
     def _get_af_working_hours(
         self, af_project_ids: Collection[str], start_date: Optional[str], end_date: Optional[str]
     ) -> pandas.DataFrame:
         """Annofabの作業時間情報が格納されたDataFrameを返す。
 
-        以下の列がある。
+        返すDataFrameには以下の列が存在します。
         * date
         * annofab_project_id
         * annofab_account_id
         * annofab_working_hours
         """
         result: list[dict[str, Any]] = []
 
@@ -375,21 +380,20 @@
 
         df_af_working_hours = self._get_af_working_hours(
             af_project_ids=af_project_ids,
             start_date=_get_start_date(df_actual_working_hours),
             end_date=_get_end_date(df_actual_working_hours),
         )
 
-        df = _get_get_df_working_hours_from_df(
+        df = _get_df_working_hours_from_df(
             df_actual_working_hours=df_actual_working_hours,
             df_user_and_af_account=df_user_and_af_account,
             df_job_and_af_project=df_job_and_af_project,
             df_af_working_hours=df_af_working_hours,
         )
-
         if user_ids is not None:
             df = df[df["user_id"].isin(set(user_ids))]
 
         if is_show_parent_job:
             df_job_parent_job = self._get_df_job_parent_job()
             df = df.merge(df_job_parent_job, how="left", on="job_id")
```

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/put_account_external_linkage_info.py` & `annoworkcli-3.2.1/annoworkcli/annofab/put_account_external_linkage_info.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/put_job_from_annofab_project.py` & `annoworkcli-3.2.1/annoworkcli/annofab/put_job_from_annofab_project.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/reshape_working_hours.py` & `annoworkcli-3.2.1/annoworkcli/annofab/reshape_working_hours.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/annofab/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/annofab/visualize_statistics.py` & `annoworkcli-3.2.1/annoworkcli/annofab/visualize_statistics.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/common/annofab.py` & `annoworkcli-3.2.1/annoworkcli/common/annofab.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/common/cli.py` & `annoworkcli-3.2.1/annoworkcli/common/cli.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/common/utils.py` & `annoworkcli-3.2.1/annoworkcli/common/utils.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/common/workspace_tag.py` & `annoworkcli-3.2.1/annoworkcli/common/workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/data/logging.yaml` & `annoworkcli-3.2.1/annoworkcli/data/logging.yaml`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/expected_working_time/delete_expected_working_time.py` & `annoworkcli-3.2.1/annoworkcli/expected_working_time/delete_expected_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/expected_working_time/list_expected_working_time.py` & `annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py` & `annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/expected_working_time/list_expected_working_time_weekly.py` & `annoworkcli-3.2.1/annoworkcli/expected_working_time/list_expected_working_time_weekly.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/expected_working_time/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/expected_working_time/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/job/change_job_properties.py` & `annoworkcli-3.2.1/annoworkcli/job/change_job_properties.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/job/delete_job.py` & `annoworkcli-3.2.1/annoworkcli/job/delete_job.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/job/list_job.py` & `annoworkcli-3.2.1/annoworkcli/job/list_job.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/job/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/job/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/my/get_my_account.py` & `annoworkcli-3.2.1/annoworkcli/my/get_my_account.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/my/list_my_workspace_member.py` & `annoworkcli-3.2.1/annoworkcli/my/list_my_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/my/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/my/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/schedule/list_assigned_hours_daily.py` & `annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py` & `annoworkcli-3.2.1/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/schedule/list_schedule.py` & `annoworkcli-3.2.1/annoworkcli/schedule/list_schedule.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/schedule/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/schedule/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace/list_workspace.py` & `annoworkcli-3.2.1/annoworkcli/workspace/list_workspace.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace/put_workspace.py` & `annoworkcli-3.2.1/annoworkcli/workspace/put_workspace.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/workspace/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/append_tag_to_workspace_member.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/append_tag_to_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/change_workspace_member_properties.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/change_workspace_member_properties.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/delete_workspace_member.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/delete_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/list_workspace_member.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/list_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/put_workspace_member.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/put_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/remove_tag_to_workspace_member.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/remove_tag_to_workspace_member.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_member/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/workspace_member/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_tag/list_workspace_tag.py` & `annoworkcli-3.2.1/annoworkcli/workspace_tag/list_workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_tag/put_workspace_tag.py` & `annoworkcli-3.2.1/annoworkcli/workspace_tag/put_workspace_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,14 @@
     )
 
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "put"
-    subcommand_help = "ワークスペースタグを更新します。"
+    subcommand_help = "ワークスペースタグを作成または更新します。"
 
     parser = annoworkcli.common.cli.add_parser(
         subparsers, subcommand_name, subcommand_help, description=subcommand_help
     )
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.2.0/annoworkcli/workspace_tag/subcommand.py` & `annoworkcli-3.2.1/annoworkcli/workspace_tag/subcommand.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.2.0/PKG-INFO` & `annoworkcli-3.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: annoworkcli
-Version: 3.2.0
-Summary: 
+Version: 3.2.1
+Summary: AnnoworkのCLI(Command Line Interface)
 Home-page: https://github.com/kurusugawa-computer/annowork-cli
 License: MIT
 Keywords: annowork,cli
-Author: yuji38kwmt
+Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: annofabapi (>=0.52.4)
 Requires-Dist: annofabcli (>=1.61.2)
 Requires-Dist: annoworkapi (>=3.0.1)
 Requires-Dist: isodate
 Requires-Dist: more-itertools
 Requires-Dist: pandas
```

