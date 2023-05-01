# Comparing `tmp/windmill_api-1.90.0.tar.gz` & `tmp/windmill_api-1.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.90.0.tar", max compression
+gzip compressed data, was "windmill_api-1.91.0.tar", max compression
```

## Comparing `windmill_api-1.90.0.tar` & `windmill_api-1.91.0.tar`

### file list

```diff
@@ -1,1268 +1,1274 @@
--rw-r--r--   0        0        0    11348 2023-04-29 07:46:49.882179 windmill_api-1.90.0/LICENSE
--rw-r--r--   0        0        0     2952 2023-04-29 07:46:49.886179 windmill_api-1.90.0/README.md
--rw-r--r--   0        0        0      717 2023-04-29 07:46:49.886179 windmill_api-1.90.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-29 07:46:18.189917 windmill_api-1.90.0/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-04-29 07:46:18.673921 windmill_api-1.90.0/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.781921 windmill_api-1.90.0/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-04-29 07:46:29.150005 windmill_api-1.90.0/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-04-29 07:46:29.158005 windmill_api-1.90.0/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-04-29 07:46:29.190005 windmill_api-1.90.0/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-04-29 07:46:29.206005 windmill_api-1.90.0/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-04-29 07:46:29.230005 windmill_api-1.90.0/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3031 2023-04-29 07:46:29.242005 windmill_api-1.90.0/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-04-29 07:46:29.270006 windmill_api-1.90.0/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-04-29 07:46:29.298006 windmill_api-1.90.0/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-04-29 07:46:29.310006 windmill_api-1.90.0/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-04-29 07:46:29.386007 windmill_api-1.90.0/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-04-29 07:46:29.342006 windmill_api-1.90.0/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-04-29 07:46:29.370006 windmill_api-1.90.0/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.713921 windmill_api-1.90.0/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-04-29 07:46:29.414007 windmill_api-1.90.0/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-04-29 07:46:29.490007 windmill_api-1.90.0/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.833922 windmill_api-1.90.0/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-29 07:46:29.442007 windmill_api-1.90.0/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-04-29 07:46:29.470007 windmill_api-1.90.0/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-04-29 07:46:29.502008 windmill_api-1.90.0/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.833922 windmill_api-1.90.0/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-04-29 07:46:29.522008 windmill_api-1.90.0/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-04-29 07:46:29.526008 windmill_api-1.90.0/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.773921 windmill_api-1.90.0/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-04-29 07:46:29.554008 windmill_api-1.90.0/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-04-29 07:46:29.554008 windmill_api-1.90.0/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-04-29 07:46:29.582008 windmill_api-1.90.0/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-04-29 07:46:29.594008 windmill_api-1.90.0/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-04-29 07:46:29.622008 windmill_api-1.90.0/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     4827 2023-04-29 07:46:29.666009 windmill_api-1.90.0/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-04-29 07:46:29.682009 windmill_api-1.90.0/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-04-29 07:46:29.690009 windmill_api-1.90.0/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-04-29 07:46:29.782010 windmill_api-1.90.0/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-04-29 07:46:29.722009 windmill_api-1.90.0/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-04-29 07:46:29.750010 windmill_api-1.90.0/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.825922 windmill_api-1.90.0/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-29 07:46:29.782010 windmill_api-1.90.0/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-04-29 07:46:29.810010 windmill_api-1.90.0/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-04-29 07:46:29.810010 windmill_api-1.90.0/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-04-29 07:46:29.846010 windmill_api-1.90.0/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-04-29 07:46:29.850010 windmill_api-1.90.0/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-04-29 07:46:29.894011 windmill_api-1.90.0/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-04-29 07:46:29.906011 windmill_api-1.90.0/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-04-29 07:46:29.922011 windmill_api-1.90.0/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-04-29 07:46:29.938011 windmill_api-1.90.0/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.829922 windmill_api-1.90.0/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-04-29 07:46:29.970011 windmill_api-1.90.0/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-04-29 07:46:29.990012 windmill_api-1.90.0/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-04-29 07:46:30.002012 windmill_api-1.90.0/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.817922 windmill_api-1.90.0/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-04-29 07:46:30.046012 windmill_api-1.90.0/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-04-29 07:46:30.030012 windmill_api-1.90.0/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-04-29 07:46:30.058012 windmill_api-1.90.0/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-04-29 07:46:30.086012 windmill_api-1.90.0/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-04-29 07:46:30.102012 windmill_api-1.90.0/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-04-29 07:46:30.146013 windmill_api-1.90.0/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-04-29 07:46:30.134013 windmill_api-1.90.0/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-04-29 07:46:30.162013 windmill_api-1.90.0/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.833922 windmill_api-1.90.0/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-29 07:46:30.190013 windmill_api-1.90.0/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-04-29 07:46:30.190013 windmill_api-1.90.0/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-04-29 07:46:30.258014 windmill_api-1.90.0/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-04-29 07:46:30.262014 windmill_api-1.90.0/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-04-29 07:46:30.306014 windmill_api-1.90.0/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.789922 windmill_api-1.90.0/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-04-29 07:46:30.294014 windmill_api-1.90.0/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-04-29 07:46:30.334014 windmill_api-1.90.0/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-29 07:46:30.346014 windmill_api-1.90.0/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-04-29 07:46:30.390015 windmill_api-1.90.0/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-04-29 07:46:30.382015 windmill_api-1.90.0/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-04-29 07:46:30.414015 windmill_api-1.90.0/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-04-29 07:46:30.430015 windmill_api-1.90.0/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:30.438015 windmill_api-1.90.0/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-04-29 07:46:30.470015 windmill_api-1.90.0/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-04-29 07:46:30.494016 windmill_api-1.90.0/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-04-29 07:46:30.526016 windmill_api-1.90.0/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-04-29 07:46:30.546016 windmill_api-1.90.0/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-04-29 07:46:30.670017 windmill_api-1.90.0/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-04-29 07:46:30.706017 windmill_api-1.90.0/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-04-29 07:46:30.842018 windmill_api-1.90.0/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-04-29 07:46:30.734018 windmill_api-1.90.0/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-04-29 07:46:30.762018 windmill_api-1.90.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-04-29 07:46:30.802018 windmill_api-1.90.0/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-29 07:46:30.846019 windmill_api-1.90.0/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-04-29 07:46:30.902019 windmill_api-1.90.0/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-04-29 07:46:30.882019 windmill_api-1.90.0/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-04-29 07:46:30.938019 windmill_api-1.90.0/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-04-29 07:46:30.958020 windmill_api-1.90.0/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-04-29 07:46:31.002020 windmill_api-1.90.0/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-04-29 07:46:30.998020 windmill_api-1.90.0/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-04-29 07:46:31.046020 windmill_api-1.90.0/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-04-29 07:46:31.050020 windmill_api-1.90.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.745921 windmill_api-1.90.0/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-29 07:46:31.118021 windmill_api-1.90.0/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-04-29 07:46:31.078020 windmill_api-1.90.0/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-04-29 07:46:31.106021 windmill_api-1.90.0/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-04-29 07:46:31.134021 windmill_api-1.90.0/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-04-29 07:46:31.146021 windmill_api-1.90.0/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-04-29 07:46:31.158021 windmill_api-1.90.0/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-04-29 07:46:31.182021 windmill_api-1.90.0/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-04-29 07:46:31.190021 windmill_api-1.90.0/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.749921 windmill_api-1.90.0/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-29 07:46:31.214022 windmill_api-1.90.0/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-04-29 07:46:31.218022 windmill_api-1.90.0/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:31.246022 windmill_api-1.90.0/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-04-29 07:46:31.246022 windmill_api-1.90.0/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-04-29 07:46:31.286022 windmill_api-1.90.0/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-04-29 07:46:31.286022 windmill_api-1.90.0/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-04-29 07:46:31.346023 windmill_api-1.90.0/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-04-29 07:46:31.326022 windmill_api-1.90.0/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-04-29 07:46:31.358023 windmill_api-1.90.0/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-04-29 07:46:31.414023 windmill_api-1.90.0/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-04-29 07:46:31.410023 windmill_api-1.90.0/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-04-29 07:46:31.450024 windmill_api-1.90.0/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-04-29 07:46:31.442023 windmill_api-1.90.0/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-04-29 07:46:31.474024 windmill_api-1.90.0/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-04-29 07:46:31.502024 windmill_api-1.90.0/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.813922 windmill_api-1.90.0/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-29 07:46:31.502024 windmill_api-1.90.0/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:31.530024 windmill_api-1.90.0/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-04-29 07:46:31.546024 windmill_api-1.90.0/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-04-29 07:46:31.570025 windmill_api-1.90.0/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-04-29 07:46:31.602025 windmill_api-1.90.0/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-04-29 07:46:31.610025 windmill_api-1.90.0/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-04-29 07:46:31.634025 windmill_api-1.90.0/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-04-29 07:46:31.638025 windmill_api-1.90.0/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.757921 windmill_api-1.90.0/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-04-29 07:46:31.678025 windmill_api-1.90.0/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-04-29 07:46:31.686025 windmill_api-1.90.0/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-29 07:46:31.718026 windmill_api-1.90.0/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-04-29 07:46:31.714026 windmill_api-1.90.0/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-04-29 07:46:31.754026 windmill_api-1.90.0/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-04-29 07:46:31.758026 windmill_api-1.90.0/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-29 07:46:31.790026 windmill_api-1.90.0/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-04-29 07:46:31.798026 windmill_api-1.90.0/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-04-29 07:46:31.826027 windmill_api-1.90.0/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-04-29 07:46:31.842027 windmill_api-1.90.0/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-04-29 07:46:31.862027 windmill_api-1.90.0/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-04-29 07:46:31.882027 windmill_api-1.90.0/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3276 2023-04-29 07:46:31.902027 windmill_api-1.90.0/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-04-29 07:46:31.922027 windmill_api-1.90.0/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-04-29 07:46:31.938028 windmill_api-1.90.0/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-04-29 07:46:31.950028 windmill_api-1.90.0/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-04-29 07:46:32.082029 windmill_api-1.90.0/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-04-29 07:46:31.986028 windmill_api-1.90.0/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:32.014028 windmill_api-1.90.0/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:32.042029 windmill_api-1.90.0/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-04-29 07:46:32.074029 windmill_api-1.90.0/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.689921 windmill_api-1.90.0/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-29 07:46:32.098029 windmill_api-1.90.0/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-04-29 07:46:32.106029 windmill_api-1.90.0/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.717921 windmill_api-1.90.0/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-29 07:46:32.130029 windmill_api-1.90.0/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-04-29 07:46:32.130029 windmill_api-1.90.0/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-04-29 07:46:32.158030 windmill_api-1.90.0/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-04-29 07:46:32.158030 windmill_api-1.90.0/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-04-29 07:46:32.202030 windmill_api-1.90.0/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-04-29 07:46:32.186030 windmill_api-1.90.0/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-04-29 07:46:32.210030 windmill_api-1.90.0/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-04-29 07:46:32.230030 windmill_api-1.90.0/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-04-29 07:46:32.234030 windmill_api-1.90.0/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-04-29 07:46:32.258031 windmill_api-1.90.0/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-04-29 07:46:32.258031 windmill_api-1.90.0/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-04-29 07:46:32.286031 windmill_api-1.90.0/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-04-29 07:46:32.290031 windmill_api-1.90.0/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-04-29 07:46:32.326031 windmill_api-1.90.0/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-04-29 07:46:32.318031 windmill_api-1.90.0/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-04-29 07:46:32.370031 windmill_api-1.90.0/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-04-29 07:46:32.366032 windmill_api-1.90.0/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-04-29 07:46:32.406032 windmill_api-1.90.0/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-04-29 07:46:32.422032 windmill_api-1.90.0/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-04-29 07:46:32.442032 windmill_api-1.90.0/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:32.446032 windmill_api-1.90.0/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-04-29 07:46:32.470032 windmill_api-1.90.0/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-04-29 07:46:32.470032 windmill_api-1.90.0/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-04-29 07:46:32.498033 windmill_api-1.90.0/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-04-29 07:46:32.502033 windmill_api-1.90.0/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-04-29 07:46:32.534033 windmill_api-1.90.0/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-04-29 07:46:32.574033 windmill_api-1.90.0/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.741921 windmill_api-1.90.0/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-29 07:46:32.566033 windmill_api-1.90.0/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-04-29 07:46:32.594034 windmill_api-1.90.0/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-04-29 07:46:32.614034 windmill_api-1.90.0/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-04-29 07:46:32.642034 windmill_api-1.90.0/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-04-29 07:46:32.654034 windmill_api-1.90.0/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-04-29 07:46:32.698034 windmill_api-1.90.0/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-04-29 07:46:32.690034 windmill_api-1.90.0/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.789922 windmill_api-1.90.0/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-04-29 07:46:32.726035 windmill_api-1.90.0/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-04-29 07:46:32.750035 windmill_api-1.90.0/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-04-29 07:46:18.729921 windmill_api-1.90.0/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-29 07:46:32.758035 windmill_api-1.90.0/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-04-29 07:46:32.774035 windmill_api-1.90.0/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-04-29 07:46:32.786035 windmill_api-1.90.0/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-04-29 07:46:32.802035 windmill_api-1.90.0/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-04-29 07:46:32.814036 windmill_api-1.90.0/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-04-29 07:46:32.830036 windmill_api-1.90.0/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-04-29 07:46:32.846036 windmill_api-1.90.0/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-04-29 07:46:32.858036 windmill_api-1.90.0/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-04-29 07:46:32.890036 windmill_api-1.90.0/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-04-29 07:46:32.886036 windmill_api-1.90.0/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-04-29 07:46:32.918037 windmill_api-1.90.0/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-04-29 07:46:32.926036 windmill_api-1.90.0/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-04-29 07:46:32.950037 windmill_api-1.90.0/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-04-29 07:46:32.958037 windmill_api-1.90.0/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-04-29 07:46:32.990037 windmill_api-1.90.0/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-04-29 07:46:32.990037 windmill_api-1.90.0/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-04-29 07:46:33.046038 windmill_api-1.90.0/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-04-29 07:46:33.042038 windmill_api-1.90.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-04-29 07:46:33.066038 windmill_api-1.90.0/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-04-29 07:46:33.074038 windmill_api-1.90.0/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-04-29 07:46:49.878179 windmill_api-1.90.0/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-29 07:46:33.102038 windmill_api-1.90.0/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-04-29 07:46:33.126038 windmill_api-1.90.0/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-04-29 07:46:27.745993 windmill_api-1.90.0/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-04-29 07:46:33.158038 windmill_api-1.90.0/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-04-29 07:46:33.186039 windmill_api-1.90.0/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-04-29 07:46:33.214039 windmill_api-1.90.0/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-04-29 07:46:33.246039 windmill_api-1.90.0/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-04-29 07:46:28.229997 windmill_api-1.90.0/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-04-29 07:46:33.234039 windmill_api-1.90.0/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-04-29 07:46:33.282040 windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-04-29 07:46:28.277997 windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-04-29 07:46:33.270040 windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-04-29 07:46:33.290040 windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-04-29 07:46:33.306040 windmill_api-1.90.0/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7091 2023-04-29 07:46:33.382041 windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-04-29 07:46:33.326040 windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-04-29 07:46:28.518000 windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-04-29 07:46:28.201997 windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-04-29 07:46:33.350040 windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-04-29 07:46:33.410041 windmill_api-1.90.0/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-04-29 07:46:28.265997 windmill_api-1.90.0/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-04-29 07:46:28.161996 windmill_api-1.90.0/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-04-29 07:46:33.406041 windmill_api-1.90.0/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-04-29 07:46:33.450041 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-29 07:46:33.470041 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-29 07:46:28.177997 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-29 07:46:33.482041 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-29 07:46:33.494042 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-29 07:46:33.510042 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-29 07:46:33.530042 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-29 07:46:28.337998 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-29 07:46:33.538042 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-29 07:46:33.566042 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-29 07:46:28.277997 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-29 07:46:33.590042 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-29 07:46:27.593992 windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-04-29 07:46:33.618043 windmill_api-1.90.0/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-04-29 07:46:33.622043 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-29 07:46:33.702043 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-29 07:46:33.662043 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-29 07:46:33.690043 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-29 07:46:33.722044 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-29 07:46:33.730044 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:28.249997 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-29 07:46:33.766044 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:27.861994 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-29 07:46:33.762044 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-29 07:46:33.790044 windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-29 07:46:27.789993 windmill_api-1.90.0/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-04-29 07:46:33.810044 windmill_api-1.90.0/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-04-29 07:46:33.830045 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-29 07:46:33.886045 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-29 07:46:33.870045 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-29 07:46:33.902045 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-29 07:46:33.918045 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-29 07:46:33.934046 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:28.169997 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-29 07:46:33.950046 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:27.729993 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-29 07:46:33.982046 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-29 07:46:33.978046 windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-29 07:46:34.054047 windmill_api-1.90.0/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-04-29 07:46:34.018046 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-29 07:46:34.050047 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-29 07:46:34.082047 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-29 07:46:34.082047 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-29 07:46:27.857994 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-29 07:46:34.142048 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-29 07:46:28.421999 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-29 07:46:34.114047 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-29 07:46:34.146047 windmill_api-1.90.0/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-29 07:46:28.257997 windmill_api-1.90.0/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-04-29 07:46:34.166048 windmill_api-1.90.0/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-29 07:46:34.166048 windmill_api-1.90.0/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-04-29 07:46:34.294049 windmill_api-1.90.0/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-04-29 07:46:34.186048 windmill_api-1.90.0/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-04-29 07:46:34.230048 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-04-29 07:46:34.310049 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-04-29 07:46:34.318049 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-04-29 07:46:34.362049 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-04-29 07:46:28.437999 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-04-29 07:46:34.346049 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-04-29 07:46:34.378049 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-04-29 07:46:27.709993 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-04-29 07:46:34.450050 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-04-29 07:46:34.406050 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-04-29 07:46:34.430050 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-04-29 07:46:27.477991 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-04-29 07:46:34.486050 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-04-29 07:46:34.482051 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-04-29 07:46:28.518000 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-04-29 07:46:34.514051 windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-04-29 07:46:27.937995 windmill_api-1.90.0/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-04-29 07:46:27.465991 windmill_api-1.90.0/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-04-29 07:46:34.534051 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-04-29 07:46:34.590052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-04-29 07:46:34.570051 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-04-29 07:46:34.602052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-29 07:46:34.622052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-29 07:46:34.642052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:28.021995 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-29 07:46:34.650052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:28.017995 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-29 07:46:34.674052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-29 07:46:34.706052 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-04-29 07:46:34.754053 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-04-29 07:46:34.746053 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-04-29 07:46:34.774053 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-04-29 07:46:34.790053 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-04-29 07:46:34.802053 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-04-29 07:46:27.829994 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-04-29 07:46:34.818054 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-04-29 07:46:27.865994 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-04-29 07:46:34.830054 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-04-29 07:46:34.846054 windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-04-29 07:46:34.854054 windmill_api-1.90.0/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-04-29 07:46:34.910054 windmill_api-1.90.0/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-04-29 07:46:34.878054 windmill_api-1.90.0/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-04-29 07:46:34.906054 windmill_api-1.90.0/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-04-29 07:46:34.938055 windmill_api-1.90.0/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2035 2023-04-29 07:46:34.942055 windmill_api-1.90.0/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-29 07:46:34.982055 windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-29 07:46:28.521999 windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-29 07:46:34.970055 windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-29 07:46:34.994055 windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-29 07:46:35.022055 windmill_api-1.90.0/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-29 07:46:35.014055 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-29 07:46:35.058056 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-29 07:46:35.118056 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-29 07:46:35.098056 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-29 07:46:35.126056 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-29 07:46:35.154056 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-29 07:46:35.154056 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:28.365998 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-29 07:46:35.182057 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:27.729993 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-29 07:46:35.182057 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-29 07:46:35.210057 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-29 07:46:35.262057 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-29 07:46:35.270058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-29 07:46:35.294058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-29 07:46:35.306058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-29 07:46:35.322058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-29 07:46:28.405999 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-29 07:46:35.334058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-29 07:46:27.481991 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-29 07:46:35.354058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-29 07:46:35.362058 windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2126 2023-04-29 07:46:35.390059 windmill_api-1.90.0/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-04-29 07:46:35.386059 windmill_api-1.90.0/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-04-29 07:46:35.414059 windmill_api-1.90.0/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-04-29 07:46:35.442059 windmill_api-1.90.0/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-04-29 07:46:35.438059 windmill_api-1.90.0/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-04-29 07:46:35.470059 windmill_api-1.90.0/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-04-29 07:46:27.493991 windmill_api-1.90.0/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     2094 2023-04-29 07:46:35.478059 windmill_api-1.90.0/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-04-29 07:46:35.502060 windmill_api-1.90.0/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-04-29 07:46:35.514060 windmill_api-1.90.0/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-04-29 07:46:35.538060 windmill_api-1.90.0/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-29 07:46:35.534060 windmill_api-1.90.0/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     4829 2023-04-29 07:46:35.606061 windmill_api-1.90.0/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-04-29 07:46:28.521999 windmill_api-1.90.0/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-04-29 07:46:27.469991 windmill_api-1.90.0/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-04-29 07:46:35.562060 windmill_api-1.90.0/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-04-29 07:46:35.598060 windmill_api-1.90.0/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-04-29 07:46:35.650061 windmill_api-1.90.0/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-04-29 07:46:35.642061 windmill_api-1.90.0/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-04-29 07:46:35.678061 windmill_api-1.90.0/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-04-29 07:46:35.690061 windmill_api-1.90.0/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-04-29 07:46:35.718062 windmill_api-1.90.0/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-04-29 07:46:35.714062 windmill_api-1.90.0/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-04-29 07:46:35.746062 windmill_api-1.90.0/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-04-29 07:46:35.738062 windmill_api-1.90.0/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-04-29 07:46:35.906063 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-04-29 07:46:35.762062 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-04-29 07:46:35.806062 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-04-29 07:46:35.890063 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-04-29 07:46:35.914063 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-04-29 07:46:35.938063 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-04-29 07:46:28.053996 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-04-29 07:46:35.942063 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-04-29 07:46:35.974064 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-04-29 07:46:28.253997 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-04-29 07:46:36.050064 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-04-29 07:46:36.002064 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-04-29 07:46:36.030064 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-04-29 07:46:27.633992 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-04-29 07:46:36.058065 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-04-29 07:46:36.086065 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-04-29 07:46:27.645992 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-04-29 07:46:36.098065 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-04-29 07:46:27.473991 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-04-29 07:46:27.997995 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-04-29 07:46:36.130065 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-04-29 07:46:36.182066 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-04-29 07:46:36.170065 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-04-29 07:46:36.198066 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-04-29 07:46:36.250066 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-04-29 07:46:36.226066 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:27.657992 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-29 07:46:36.254066 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.241997 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-04-29 07:46:36.278066 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-04-29 07:46:36.282067 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-04-29 07:46:36.366067 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-04-29 07:46:36.322067 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-04-29 07:46:36.350067 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-04-29 07:46:36.406068 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-04-29 07:46:36.394068 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-29 07:46:28.225997 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-04-29 07:46:36.426068 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-29 07:46:28.037995 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-04-29 07:46:36.438068 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-04-29 07:46:36.454068 windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-04-29 07:46:36.466068 windmill_api-1.90.0/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7065 2023-04-29 07:46:36.546069 windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-04-29 07:46:36.486068 windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-04-29 07:46:28.053996 windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-04-29 07:46:27.557992 windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-04-29 07:46:36.506069 windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-04-29 07:46:36.546069 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-29 07:46:36.642070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-29 07:46:27.645992 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-29 07:46:36.570069 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-29 07:46:36.598070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-29 07:46:36.626070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-29 07:46:36.662070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-29 07:46:28.037995 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-29 07:46:36.670070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-29 07:46:36.694070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-29 07:46:27.961995 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-29 07:46:36.694070 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-29 07:46:27.821994 windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-04-29 07:46:36.722071 windmill_api-1.90.0/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-04-29 07:46:36.730071 windmill_api-1.90.0/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-04-29 07:46:36.754071 windmill_api-1.90.0/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-04-29 07:46:36.790071 windmill_api-1.90.0/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-04-29 07:46:36.802071 windmill_api-1.90.0/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-04-29 07:46:36.818071 windmill_api-1.90.0/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-04-29 07:46:36.838072 windmill_api-1.90.0/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-04-29 07:46:36.842072 windmill_api-1.90.0/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-04-29 07:46:36.870072 windmill_api-1.90.0/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-04-29 07:46:36.890072 windmill_api-1.90.0/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-04-29 07:46:36.890072 windmill_api-1.90.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-04-29 07:46:36.918072 windmill_api-1.90.0/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-04-29 07:46:36.918072 windmill_api-1.90.0/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-04-29 07:46:36.942072 windmill_api-1.90.0/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4633 2023-04-29 07:46:36.982073 windmill_api-1.90.0/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-04-29 07:46:36.962073 windmill_api-1.90.0/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3416 2023-04-29 07:46:37.010073 windmill_api-1.90.0/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-04-29 07:46:37.002073 windmill_api-1.90.0/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-04-29 07:46:37.114074 windmill_api-1.90.0/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-04-29 07:46:37.050073 windmill_api-1.90.0/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-04-29 07:46:37.082074 windmill_api-1.90.0/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-04-29 07:46:37.114074 windmill_api-1.90.0/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-04-29 07:46:37.162074 windmill_api-1.90.0/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-04-29 07:46:28.065996 windmill_api-1.90.0/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-04-29 07:46:37.142074 windmill_api-1.90.0/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-04-29 07:46:27.769993 windmill_api-1.90.0/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-04-29 07:46:37.174075 windmill_api-1.90.0/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-04-29 07:46:37.190075 windmill_api-1.90.0/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-04-29 07:46:37.218075 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-04-29 07:46:37.226075 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-29 07:46:37.250075 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.041996 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-29 07:46:37.254075 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.053996 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-04-29 07:46:27.857994 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-04-29 07:46:28.413999 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-04-29 07:46:37.290076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-04-29 07:46:37.290076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-29 07:46:37.318076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.493999 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-29 07:46:37.322076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.305998 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-04-29 07:46:27.737993 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-04-29 07:46:37.350076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-04-29 07:46:37.362076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-29 07:46:37.382076 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.353998 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-29 07:46:37.398077 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.345998 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-04-29 07:46:27.725993 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-04-29 07:46:37.470077 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-04-29 07:46:37.426077 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-04-29 07:46:27.917995 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-04-29 07:46:37.458077 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-04-29 07:46:28.413999 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-04-29 07:46:37.566078 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-04-29 07:46:37.510078 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-29 07:46:37.538078 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-29 07:46:37.566078 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-29 07:46:37.594078 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:28.501999 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-29 07:46:37.594078 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:27.465991 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-29 07:46:37.626079 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-29 07:46:37.622079 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-04-29 07:46:27.865994 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-04-29 07:46:37.662079 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-04-29 07:46:37.658079 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-29 07:46:37.738080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-29 07:46:37.702079 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-29 07:46:37.730080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-29 07:46:37.762080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-29 07:46:37.766080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:27.881994 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-29 07:46:37.794080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:27.757993 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-29 07:46:37.830080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-29 07:46:37.822080 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-04-29 07:46:37.942082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-04-29 07:46:37.866081 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-29 07:46:37.894081 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-29 07:46:37.926081 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-29 07:46:37.958082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:27.537991 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-29 07:46:37.970082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-29 07:46:27.637992 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-29 07:46:37.986082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-29 07:46:38.002082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-29 07:46:27.541991 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-04-29 07:46:38.022082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-04-29 07:46:38.038082 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-29 07:46:38.106083 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-29 07:46:38.082083 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-29 07:46:38.110083 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-29 07:46:38.138083 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-29 07:46:38.142083 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:27.697993 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-29 07:46:38.198084 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:27.993995 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-29 07:46:38.174084 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-29 07:46:38.202084 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-29 07:46:28.189997 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-04-29 07:46:38.230084 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-04-29 07:46:28.369998 windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-04-29 07:46:38.238084 windmill_api-1.90.0/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-04-29 07:46:38.250084 windmill_api-1.90.0/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-04-29 07:46:38.278084 windmill_api-1.90.0/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-04-29 07:46:38.326085 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-04-29 07:46:38.350085 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-04-29 07:46:38.358085 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-04-29 07:46:38.386085 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-04-29 07:46:38.386085 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:28.061996 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-04-29 07:46:38.410086 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:27.589992 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-04-29 07:46:38.418086 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-04-29 07:46:38.442086 windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-04-29 07:46:38.498087 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-04-29 07:46:38.482086 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-04-29 07:46:38.506086 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-04-29 07:46:38.530087 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-04-29 07:46:38.534087 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-29 07:46:27.677992 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-04-29 07:46:38.562087 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-29 07:46:27.601992 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-04-29 07:46:38.610087 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-04-29 07:46:38.590087 windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-04-29 07:46:38.610087 windmill_api-1.90.0/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-04-29 07:46:38.650088 windmill_api-1.90.0/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-04-29 07:46:38.742089 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-04-29 07:46:38.678088 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-04-29 07:46:38.706088 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-04-29 07:46:27.649992 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-04-29 07:46:38.734089 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-04-29 07:46:38.770089 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-04-29 07:46:28.253997 windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-04-29 07:46:38.822089 windmill_api-1.90.0/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-04-29 07:46:38.794089 windmill_api-1.90.0/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-04-29 07:46:38.826089 windmill_api-1.90.0/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-04-29 07:46:28.309998 windmill_api-1.90.0/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-04-29 07:46:38.850090 windmill_api-1.90.0/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-04-29 07:46:38.862090 windmill_api-1.90.0/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-04-29 07:46:28.333998 windmill_api-1.90.0/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-04-29 07:46:38.934090 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-04-29 07:46:38.886090 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-04-29 07:46:38.914090 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-04-29 07:46:27.977995 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-04-29 07:46:38.942090 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-04-29 07:46:38.970091 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-04-29 07:46:27.837994 windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-04-29 07:46:39.010091 windmill_api-1.90.0/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-04-29 07:46:39.014091 windmill_api-1.90.0/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-04-29 07:46:39.094092 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-04-29 07:46:39.054091 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-04-29 07:46:39.082092 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-29 07:46:39.162092 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-29 07:46:39.122092 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-29 07:46:28.001995 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-29 07:46:39.154092 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-29 07:46:28.221997 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-29 07:46:39.182093 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-29 07:46:39.190093 windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-29 07:46:39.258093 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-04-29 07:46:39.230093 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-29 07:46:39.258093 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-29 07:46:39.294093 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-29 07:46:39.286094 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-29 07:46:27.833994 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-29 07:46:39.314094 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-29 07:46:28.017995 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-29 07:46:39.322094 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-29 07:46:39.398095 windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-04-29 07:46:39.350094 windmill_api-1.90.0/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-04-29 07:46:39.374094 windmill_api-1.90.0/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-04-29 07:46:39.398095 windmill_api-1.90.0/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-04-29 07:46:39.450095 windmill_api-1.90.0/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-04-29 07:46:39.426095 windmill_api-1.90.0/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-04-29 07:46:28.189997 windmill_api-1.90.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-04-29 07:46:39.454095 windmill_api-1.90.0/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-04-29 07:46:28.065996 windmill_api-1.90.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-04-29 07:46:39.578096 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-04-29 07:46:39.494095 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-04-29 07:46:39.522096 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-29 07:46:39.550096 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-29 07:46:39.582096 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-29 07:46:27.501991 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-29 07:46:39.606096 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-29 07:46:28.437999 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-29 07:46:39.606096 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-29 07:46:39.638097 windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-04-29 07:46:27.681993 windmill_api-1.90.0/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-04-29 07:46:39.658097 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-04-29 07:46:28.461999 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-04-29 07:46:39.662097 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-04-29 07:46:39.706097 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-04-29 07:46:27.861994 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-04-29 07:46:39.690097 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-04-29 07:46:39.710097 windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-04-29 07:46:39.794098 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-04-29 07:46:27.925994 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-04-29 07:46:39.734098 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-04-29 07:46:39.778098 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-04-29 07:46:28.225997 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-04-29 07:46:39.806098 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-04-29 07:46:39.814098 windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-04-29 07:46:39.858099 windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-04-29 07:46:28.073996 windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-04-29 07:46:28.353998 windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-04-29 07:46:39.834098 windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-04-29 07:46:39.966099 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-04-29 07:46:39.878099 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-04-29 07:46:39.950099 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-04-29 07:46:40.038100 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-04-29 07:46:39.990100 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-04-29 07:46:40.018100 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-04-29 07:46:27.737993 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-04-29 07:46:40.046100 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-04-29 07:46:40.074100 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-04-29 07:46:27.473991 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-04-29 07:46:40.190101 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-04-29 07:46:40.098101 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-29 07:46:40.142101 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-29 07:46:27.957995 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-29 07:46:40.170101 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-29 07:46:40.206102 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-04-29 07:46:27.737993 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-04-29 07:46:40.226101 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-04-29 07:46:27.753993 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-04-29 07:46:27.901994 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-04-29 07:46:40.250102 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-04-29 07:46:40.310102 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-04-29 07:46:40.290102 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-04-29 07:46:40.374103 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-04-29 07:46:40.342103 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-04-29 07:46:40.366103 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-04-29 07:46:27.757993 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-04-29 07:46:40.398103 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-04-29 07:46:28.381998 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-04-29 07:46:40.406103 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-04-29 07:46:40.426103 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-04-29 07:46:40.490104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-04-29 07:46:40.466104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-04-29 07:46:40.498104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-29 07:46:40.526104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-29 07:46:40.526104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:28.045996 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-29 07:46:40.606105 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:27.925994 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-29 07:46:40.558104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-29 07:46:40.586104 windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5083 2023-04-29 07:46:40.654105 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-04-29 07:46:40.626105 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-04-29 07:46:40.646105 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-04-29 07:46:40.686105 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-04-29 07:46:40.790106 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-04-29 07:46:40.726106 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-04-29 07:46:40.754106 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-29 07:46:40.786106 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-29 07:46:40.814106 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-29 07:46:27.449991 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-29 07:46:40.818107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-29 07:46:27.517991 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-29 07:46:40.846107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-29 07:46:40.846107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-04-29 07:46:40.926107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-04-29 07:46:40.886107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-04-29 07:46:40.918107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-04-29 07:46:40.950107 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-04-29 07:46:41.018108 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-29 07:46:27.461991 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-04-29 07:46:40.982108 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-29 07:46:27.857994 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-04-29 07:46:41.010108 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-04-29 07:46:41.042108 windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-04-29 07:46:41.054108 windmill_api-1.90.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-04-29 07:46:41.066108 windmill_api-1.90.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-04-29 07:46:41.082109 windmill_api-1.90.0/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-04-29 07:46:41.086109 windmill_api-1.90.0/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-04-29 07:46:41.118109 windmill_api-1.90.0/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-04-29 07:46:27.685993 windmill_api-1.90.0/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-04-29 07:46:41.110109 windmill_api-1.90.0/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-04-29 07:46:41.154109 windmill_api-1.90.0/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-04-29 07:46:41.138109 windmill_api-1.90.0/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-04-29 07:46:41.162109 windmill_api-1.90.0/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-04-29 07:46:41.226110 windmill_api-1.90.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-04-29 07:46:41.194110 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-04-29 07:46:41.234110 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-04-29 07:46:41.250110 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-04-29 07:46:41.274110 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-04-29 07:46:41.334111 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-04-29 07:46:41.314110 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-04-29 07:46:41.342111 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-04-29 07:46:41.366111 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-04-29 07:46:41.370111 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-29 07:46:28.221997 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-04-29 07:46:41.394111 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-29 07:46:27.737993 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-04-29 07:46:41.454112 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-04-29 07:46:41.426111 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-04-29 07:46:41.506112 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-04-29 07:46:41.494112 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-04-29 07:46:41.522112 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-04-29 07:46:41.542112 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-04-29 07:46:41.550112 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-04-29 07:46:28.534000 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-04-29 07:46:41.626113 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-04-29 07:46:28.297998 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-04-29 07:46:41.578113 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-04-29 07:46:41.610113 windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-04-29 07:46:41.646113 windmill_api-1.90.0/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-04-29 07:46:28.469999 windmill_api-1.90.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-04-29 07:46:41.666113 windmill_api-1.90.0/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-29 07:46:41.670113 windmill_api-1.90.0/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-04-29 07:46:27.829994 windmill_api-1.90.0/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-04-29 07:46:41.698114 windmill_api-1.90.0/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-04-29 07:46:28.001995 windmill_api-1.90.0/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-04-29 07:46:41.710114 windmill_api-1.90.0/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-04-29 07:46:41.726114 windmill_api-1.90.0/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-04-29 07:46:41.762114 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-04-29 07:46:27.473991 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-04-29 07:46:41.746114 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-04-29 07:46:41.798114 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-04-29 07:46:27.897994 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-04-29 07:46:41.786114 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-04-29 07:46:41.866115 windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-04-29 07:46:41.846115 windmill_api-1.90.0/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-29 07:46:41.870115 windmill_api-1.90.0/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-04-29 07:46:41.902115 windmill_api-1.90.0/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-04-29 07:46:41.898115 windmill_api-1.90.0/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-04-29 07:46:41.958116 windmill_api-1.90.0/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-04-29 07:46:41.922115 windmill_api-1.90.0/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-04-29 07:46:41.942116 windmill_api-1.90.0/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     6987 2023-04-29 07:46:42.026116 windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-29 07:46:41.978116 windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-29 07:46:28.525999 windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-29 07:46:27.989995 windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-29 07:46:42.006116 windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     6987 2023-04-29 07:46:42.150117 windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-29 07:46:42.046116 windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-29 07:46:28.185997 windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-29 07:46:28.001995 windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-29 07:46:42.070117 windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-04-29 07:46:42.102117 windmill_api-1.90.0/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-04-29 07:46:42.158117 windmill_api-1.90.0/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-04-29 07:46:42.182118 windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-04-29 07:46:42.186118 windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-04-29 07:46:42.210118 windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-04-29 07:46:27.525991 windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-04-29 07:46:42.302118 windmill_api-1.90.0/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-29 07:46:42.230118 windmill_api-1.90.0/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-04-29 07:46:42.270118 windmill_api-1.90.0/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-04-29 07:46:27.901994 windmill_api-1.90.0/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-04-29 07:46:42.294119 windmill_api-1.90.0/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-04-29 07:46:42.334119 windmill_api-1.90.0/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:27.629992 windmill_api-1.90.0/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-04-29 07:46:42.342119 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-04-29 07:46:42.394119 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-04-29 07:46:27.965995 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-04-29 07:46:42.370119 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-04-29 07:46:42.398119 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-04-29 07:46:42.422119 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-04-29 07:46:42.434120 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-04-29 07:46:27.481991 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-04-29 07:46:42.446120 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-04-29 07:46:42.470120 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-04-29 07:46:27.657992 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-29 07:46:42.526120 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:27.881994 windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-04-29 07:46:42.514120 windmill_api-1.90.0/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-04-29 07:46:42.538120 windmill_api-1.90.0/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-04-29 07:46:42.554121 windmill_api-1.90.0/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-04-29 07:46:27.769993 windmill_api-1.90.0/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-04-29 07:46:42.574121 windmill_api-1.90.0/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-04-29 07:46:42.578121 windmill_api-1.90.0/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-04-29 07:46:42.602121 windmill_api-1.90.0/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-04-29 07:46:27.905995 windmill_api-1.90.0/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-04-29 07:46:42.606121 windmill_api-1.90.0/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-04-29 07:46:28.361998 windmill_api-1.90.0/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-04-29 07:46:42.686122 windmill_api-1.90.0/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-04-29 07:46:42.634121 windmill_api-1.90.0/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-04-29 07:46:27.913994 windmill_api-1.90.0/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-04-29 07:46:42.666122 windmill_api-1.90.0/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-04-29 07:46:28.397998 windmill_api-1.90.0/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-04-29 07:46:42.718122 windmill_api-1.90.0/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-04-29 07:46:27.609992 windmill_api-1.90.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-04-29 07:46:42.710122 windmill_api-1.90.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-04-29 07:46:28.053996 windmill_api-1.90.0/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-04-29 07:46:42.762122 windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-04-29 07:46:28.473999 windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-04-29 07:46:28.025995 windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-04-29 07:46:42.742122 windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-04-29 07:46:42.874123 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-04-29 07:46:42.782122 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-04-29 07:46:42.826123 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-04-29 07:46:42.910123 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-04-29 07:46:42.962124 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-04-29 07:46:42.938124 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-04-29 07:46:27.721993 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-04-29 07:46:42.966124 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-04-29 07:46:42.998124 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-04-29 07:46:27.901994 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-04-29 07:46:43.114125 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-04-29 07:46:43.022124 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-04-29 07:46:43.050125 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-04-29 07:46:27.809994 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-04-29 07:46:43.082125 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-04-29 07:46:43.118125 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-04-29 07:46:27.977995 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-04-29 07:46:43.146125 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-04-29 07:46:28.357998 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-04-29 07:46:27.973995 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-04-29 07:46:43.166126 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-04-29 07:46:43.230126 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-04-29 07:46:43.206126 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-04-29 07:46:43.234126 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-04-29 07:46:43.262126 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-04-29 07:46:43.262126 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-04-29 07:46:27.441991 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-04-29 07:46:43.290127 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-04-29 07:46:28.097996 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-04-29 07:46:43.294127 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-04-29 07:46:43.318127 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-04-29 07:46:43.378127 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-04-29 07:46:43.358127 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-04-29 07:46:43.442128 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-04-29 07:46:43.410127 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-04-29 07:46:43.502128 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-04-29 07:46:27.461991 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-04-29 07:46:43.470128 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-04-29 07:46:27.777993 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-04-29 07:46:43.502128 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-04-29 07:46:43.530129 windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-04-29 07:46:43.530129 windmill_api-1.90.0/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     5077 2023-04-29 07:46:43.594129 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-29 07:46:43.550129 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     1255 2023-04-29 07:46:43.570129 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_schema.py
--rw-r--r--   0        0        0     3297 2023-04-29 07:46:43.610129 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value.py
--rw-r--r--   0        0        0     7151 2023-04-29 07:46:43.678130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
--rw-r--r--   0        0        0     3318 2023-04-29 07:46:43.650129 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
--rw-r--r--   0        0        0     1985 2023-04-29 07:46:43.678130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2289 2023-04-29 07:46:43.710130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2187 2023-04-29 07:46:43.706130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-29 07:46:28.109996 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2054 2023-04-29 07:46:43.734130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-29 07:46:27.605992 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1978 2023-04-29 07:46:43.738130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2029 2023-04-29 07:46:43.762130 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7049 2023-04-29 07:46:43.878131 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
--rw-r--r--   0        0        0     3284 2023-04-29 07:46:43.802131 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
--rw-r--r--   0        0        0     1975 2023-04-29 07:46:43.830131 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-29 07:46:43.922132 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-29 07:46:43.906132 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-29 07:46:27.829994 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-29 07:46:43.938132 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-29 07:46:28.465999 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-29 07:46:43.954132 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-29 07:46:43.966132 windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2074 2023-04-29 07:46:43.982132 windmill_api-1.90.0/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-29 07:46:43.986132 windmill_api-1.90.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-04-29 07:46:44.026133 windmill_api-1.90.0/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-04-29 07:46:44.006132 windmill_api-1.90.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-04-29 07:46:44.038133 windmill_api-1.90.0/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-04-29 07:46:44.062133 windmill_api-1.90.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-04-29 07:46:44.070133 windmill_api-1.90.0/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-04-29 07:46:44.094133 windmill_api-1.90.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-04-29 07:46:44.102133 windmill_api-1.90.0/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-04-29 07:46:44.134133 windmill_api-1.90.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-04-29 07:46:28.153997 windmill_api-1.90.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-04-29 07:46:44.142134 windmill_api-1.90.0/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-04-29 07:46:44.154134 windmill_api-1.90.0/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-04-29 07:46:28.001995 windmill_api-1.90.0/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-04-29 07:46:44.174134 windmill_api-1.90.0/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-04-29 07:46:27.441991 windmill_api-1.90.0/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-04-29 07:46:44.186134 windmill_api-1.90.0/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-04-29 07:46:44.374135 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-04-29 07:46:44.206134 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-04-29 07:46:44.250134 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-04-29 07:46:44.390136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-04-29 07:46:44.398136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-29 07:46:44.418136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-29 07:46:28.537999 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-29 07:46:44.426136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-29 07:46:44.454136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-04-29 07:46:28.113996 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-04-29 07:46:44.506137 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-04-29 07:46:44.482136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-04-29 07:46:44.510136 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-04-29 07:46:28.341998 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-04-29 07:46:44.534137 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-04-29 07:46:44.546137 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-04-29 07:46:27.857994 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-04-29 07:46:44.566137 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-04-29 07:46:28.550000 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-04-29 07:46:27.997995 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-04-29 07:46:44.590137 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-04-29 07:46:44.646138 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-04-29 07:46:44.698138 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-04-29 07:46:44.674138 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-29 07:46:44.706138 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-29 07:46:44.726138 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:28.205997 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-29 07:46:44.794139 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:27.849994 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-29 07:46:44.754139 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-29 07:46:44.782139 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-04-29 07:46:44.862139 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-04-29 07:46:44.834139 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-04-29 07:46:44.862139 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-29 07:46:44.894140 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-29 07:46:44.894140 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-29 07:46:27.997995 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-29 07:46:44.922140 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-29 07:46:27.741993 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-29 07:46:44.922140 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-29 07:46:44.950140 windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-04-29 07:46:44.986140 windmill_api-1.90.0/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-29 07:46:44.966140 windmill_api-1.90.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-04-29 07:46:45.002141 windmill_api-1.90.0/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-04-29 07:46:45.098141 windmill_api-1.90.0/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-04-29 07:46:45.022141 windmill_api-1.90.0/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-04-29 07:46:45.042141 windmill_api-1.90.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     6980 2023-04-29 07:46:45.134142 windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-29 07:46:45.122141 windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-29 07:46:28.285997 windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-04-29 07:46:28.285997 windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-04-29 07:46:45.146142 windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-04-29 07:46:45.178142 windmill_api-1.90.0/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-04-29 07:46:45.174142 windmill_api-1.90.0/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-04-29 07:46:45.202142 windmill_api-1.90.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-04-29 07:46:45.214142 windmill_api-1.90.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-04-29 07:46:28.305998 windmill_api-1.90.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-04-29 07:46:45.266143 windmill_api-1.90.0/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-04-29 07:46:45.242143 windmill_api-1.90.0/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-04-29 07:46:45.366144 windmill_api-1.90.0/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-29 07:46:45.286143 windmill_api-1.90.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-04-29 07:46:45.322143 windmill_api-1.90.0/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-04-29 07:46:45.354143 windmill_api-1.90.0/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-04-29 07:46:45.386144 windmill_api-1.90.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-04-29 07:46:45.398144 windmill_api-1.90.0/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-04-29 07:46:45.434144 windmill_api-1.90.0/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-04-29 07:46:28.089996 windmill_api-1.90.0/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-04-29 07:46:45.418144 windmill_api-1.90.0/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-04-29 07:46:45.482144 windmill_api-1.90.0/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-04-29 07:46:45.454144 windmill_api-1.90.0/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-04-29 07:46:45.514145 windmill_api-1.90.0/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-04-29 07:46:45.502145 windmill_api-1.90.0/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-04-29 07:46:45.530145 windmill_api-1.90.0/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-04-29 07:46:45.590145 windmill_api-1.90.0/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-04-29 07:46:45.558145 windmill_api-1.90.0/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-04-29 07:46:45.598145 windmill_api-1.90.0/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-04-29 07:46:45.646146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-04-29 07:46:28.117996 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-04-29 07:46:45.622146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-04-29 07:46:45.646146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-04-29 07:46:45.674146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-04-29 07:46:45.686146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-04-29 07:46:27.573992 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-29 07:46:45.702146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-04-29 07:46:45.718146 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-04-29 07:46:27.609992 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-04-29 07:46:45.726147 windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-04-29 07:46:27.573992 windmill_api-1.90.0/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-04-29 07:46:45.758147 windmill_api-1.90.0/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-04-29 07:46:45.746147 windmill_api-1.90.0/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     2108 2023-04-29 07:46:45.782147 windmill_api-1.90.0/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-04-29 07:46:45.794147 windmill_api-1.90.0/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-04-29 07:46:45.810147 windmill_api-1.90.0/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-04-29 07:46:45.834147 windmill_api-1.90.0/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-04-29 07:46:45.898148 windmill_api-1.90.0/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-04-29 07:46:45.874148 windmill_api-1.90.0/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-04-29 07:46:46.018149 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-04-29 07:46:45.938148 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-04-29 07:46:45.966148 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-04-29 07:46:45.998149 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-04-29 07:46:46.030149 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-04-29 07:46:27.757993 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-04-29 07:46:46.046149 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-04-29 07:46:28.377998 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-04-29 07:46:46.062149 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-04-29 07:46:46.074149 windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-04-29 07:46:46.142150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-04-29 07:46:46.114150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-04-29 07:46:46.142150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-04-29 07:46:46.174150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-04-29 07:46:46.170150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-04-29 07:46:28.177997 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-04-29 07:46:46.198150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-04-29 07:46:27.593992 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-04-29 07:46:46.202150 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-04-29 07:46:46.230151 windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-29 07:46:46.246151 windmill_api-1.90.0/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-04-29 07:46:46.246151 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-04-29 07:46:46.286151 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-04-29 07:46:46.326151 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-04-29 07:46:46.326151 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-04-29 07:46:46.410152 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-04-29 07:46:46.358152 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-04-29 07:46:46.458152 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-04-29 07:46:27.677992 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-04-29 07:46:46.438152 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-04-29 07:46:27.641992 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-04-29 07:46:46.470152 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-04-29 07:46:46.486153 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-04-29 07:46:46.550153 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-04-29 07:46:46.526153 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-04-29 07:46:46.554153 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-04-29 07:46:46.582153 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-04-29 07:46:46.582153 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:28.057996 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-04-29 07:46:46.610154 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:28.489999 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-04-29 07:46:46.610154 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-04-29 07:46:46.638154 windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-04-29 07:46:46.638154 windmill_api-1.90.0/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-04-29 07:46:46.674154 windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-04-29 07:46:46.666154 windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:27.713993 windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-04-29 07:46:46.698154 windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:27.569992 windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-04-29 07:46:27.765993 windmill_api-1.90.0/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-04-29 07:46:46.710154 windmill_api-1.90.0/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-04-29 07:46:46.730155 windmill_api-1.90.0/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-04-29 07:46:46.738155 windmill_api-1.90.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-04-29 07:46:28.405999 windmill_api-1.90.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-04-29 07:46:46.758155 windmill_api-1.90.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-04-29 07:46:28.009995 windmill_api-1.90.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-04-29 07:46:28.037995 windmill_api-1.90.0/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-04-29 07:46:46.786155 windmill_api-1.90.0/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-04-29 07:46:28.501999 windmill_api-1.90.0/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-04-29 07:46:46.786155 windmill_api-1.90.0/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-04-29 07:46:46.802155 windmill_api-1.90.0/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-04-29 07:46:46.826156 windmill_api-1.90.0/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-04-29 07:46:46.822155 windmill_api-1.90.0/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-04-29 07:46:28.329998 windmill_api-1.90.0/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-04-29 07:46:46.850156 windmill_api-1.90.0/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-04-29 07:46:46.866156 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-04-29 07:46:46.982157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-04-29 07:46:27.577992 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-04-29 07:46:46.962157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-04-29 07:46:46.986157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-04-29 07:46:47.010157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-04-29 07:46:47.026157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-04-29 07:46:28.253997 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-04-29 07:46:47.038157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-04-29 07:46:47.062157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-04-29 07:46:27.457991 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-04-29 07:46:47.062157 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-04-29 07:46:28.429999 windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-04-29 07:46:47.214159 windmill_api-1.90.0/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-04-29 07:46:47.082157 windmill_api-1.90.0/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-04-29 07:46:47.130158 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-04-29 07:46:47.214159 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-04-29 07:46:47.238159 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-04-29 07:46:47.242159 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-04-29 07:46:28.037995 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-04-29 07:46:47.266159 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-04-29 07:46:47.278159 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-04-29 07:46:28.057996 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-04-29 07:46:47.422160 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-04-29 07:46:47.378160 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-04-29 07:46:47.406160 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-04-29 07:46:27.657992 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-04-29 07:46:47.434160 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-04-29 07:46:47.458160 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-04-29 07:46:27.449991 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-04-29 07:46:47.466161 windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-04-29 07:46:28.313998 windmill_api-1.90.0/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-04-29 07:46:27.793994 windmill_api-1.90.0/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-04-29 07:46:47.502161 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-04-29 07:46:47.546161 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-04-29 07:46:47.542161 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-04-29 07:46:47.570161 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-04-29 07:46:47.578162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-04-29 07:46:47.598162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:28.165997 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-04-29 07:46:47.606162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-29 07:46:28.097996 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-04-29 07:46:47.626162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-04-29 07:46:47.634162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-04-29 07:46:47.706163 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-04-29 07:46:47.670162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-04-29 07:46:47.698162 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-04-29 07:46:47.730163 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-04-29 07:46:47.734163 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-29 07:46:28.305998 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-04-29 07:46:47.754163 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-29 07:46:27.989995 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-04-29 07:46:47.762163 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-04-29 07:46:47.782163 windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-04-29 07:46:47.806163 windmill_api-1.90.0/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-04-29 07:46:47.886164 windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-04-29 07:46:47.834164 windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-04-29 07:46:28.005995 windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-04-29 07:46:47.938164 windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-04-29 07:46:27.949995 windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-04-29 07:46:28.421999 windmill_api-1.90.0/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-04-29 07:46:27.469991 windmill_api-1.90.0/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-04-29 07:46:47.914164 windmill_api-1.90.0/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-04-29 07:46:47.938164 windmill_api-1.90.0/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-04-29 07:46:27.825994 windmill_api-1.90.0/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-04-29 07:46:47.966165 windmill_api-1.90.0/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-04-29 07:46:47.962164 windmill_api-1.90.0/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-04-29 07:46:48.010165 windmill_api-1.90.0/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-04-29 07:46:47.986165 windmill_api-1.90.0/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-04-29 07:46:48.022165 windmill_api-1.90.0/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-04-29 07:46:48.034165 windmill_api-1.90.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-29 07:46:48.042165 windmill_api-1.90.0/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-04-29 07:46:48.070165 windmill_api-1.90.0/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-04-29 07:46:48.070165 windmill_api-1.90.0/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-04-29 07:46:48.102166 windmill_api-1.90.0/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-04-29 07:46:48.090165 windmill_api-1.90.0/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-04-29 07:46:48.122166 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-04-29 07:46:48.118166 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-04-29 07:46:48.162166 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-04-29 07:46:48.202166 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-04-29 07:46:48.198166 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-04-29 07:46:48.230167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-29 07:46:48.234167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-29 07:46:48.258167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-29 07:46:27.617992 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-29 07:46:48.262167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-29 07:46:27.565991 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-29 07:46:48.286167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-29 07:46:48.290167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-04-29 07:46:48.362168 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-04-29 07:46:48.330167 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-04-29 07:46:48.358168 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-04-29 07:46:48.466168 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-04-29 07:46:48.466168 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-04-29 07:46:28.365998 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-04-29 07:46:48.494169 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-04-29 07:46:28.197997 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-04-29 07:46:48.498169 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-04-29 07:46:48.522169 windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-04-29 07:46:48.518169 windmill_api-1.90.0/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-04-29 07:46:48.534169 windmill_api-1.90.0/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-04-29 07:46:48.562169 windmill_api-1.90.0/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-04-29 07:46:48.558169 windmill_api-1.90.0/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-04-29 07:46:28.285997 windmill_api-1.90.0/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-04-29 07:46:48.578169 windmill_api-1.90.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-04-29 07:46:48.582169 windmill_api-1.90.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-04-29 07:46:28.237997 windmill_api-1.90.0/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-04-29 07:46:48.638170 windmill_api-1.90.0/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-04-29 07:46:48.598169 windmill_api-1.90.0/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-04-29 07:46:48.618170 windmill_api-1.90.0/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     6432 2023-04-29 07:46:48.706170 windmill_api-1.90.0/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-04-29 07:46:48.658170 windmill_api-1.90.0/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-04-29 07:46:48.678170 windmill_api-1.90.0/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-04-29 07:46:28.165997 windmill_api-1.90.0/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-04-29 07:46:28.373998 windmill_api-1.90.0/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-04-29 07:46:48.698170 windmill_api-1.90.0/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-04-29 07:46:48.722170 windmill_api-1.90.0/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-04-29 07:46:48.726170 windmill_api-1.90.0/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-04-29 07:46:48.754171 windmill_api-1.90.0/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-04-29 07:46:48.750171 windmill_api-1.90.0/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-04-29 07:46:48.782171 windmill_api-1.90.0/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:28.297998 windmill_api-1.90.0/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-04-29 07:46:48.782171 windmill_api-1.90.0/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-04-29 07:46:28.073996 windmill_api-1.90.0/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-04-29 07:46:48.822171 windmill_api-1.90.0/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-04-29 07:46:48.826171 windmill_api-1.90.0/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-04-29 07:46:48.854171 windmill_api-1.90.0/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-04-29 07:46:28.253997 windmill_api-1.90.0/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-04-29 07:46:48.866171 windmill_api-1.90.0/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-29 07:46:48.898172 windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-29 07:46:27.905995 windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-29 07:46:48.894172 windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-29 07:46:48.914172 windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-29 07:46:48.942172 windmill_api-1.90.0/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-29 07:46:48.934172 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-29 07:46:48.974172 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-29 07:46:49.098173 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-29 07:46:49.014173 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-29 07:46:49.042173 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-29 07:46:49.074173 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-29 07:46:49.102173 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:28.265997 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-29 07:46:49.126174 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-29 07:46:28.413999 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-29 07:46:49.206174 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-29 07:46:49.154174 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-29 07:46:49.230174 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-29 07:46:49.246174 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-29 07:46:49.258175 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-29 07:46:49.278175 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-29 07:46:49.286175 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-29 07:46:27.985995 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-29 07:46:49.306175 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-29 07:46:28.169997 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-29 07:46:49.314175 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-29 07:46:49.334175 windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-04-29 07:46:49.346175 windmill_api-1.90.0/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-04-29 07:46:49.358175 windmill_api-1.90.0/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-04-29 07:46:49.374175 windmill_api-1.90.0/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-04-29 07:46:49.386175 windmill_api-1.90.0/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     2036 2023-04-29 07:46:49.402176 windmill_api-1.90.0/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-04-29 07:46:49.414176 windmill_api-1.90.0/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-04-29 07:46:49.430176 windmill_api-1.90.0/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-04-29 07:46:49.442176 windmill_api-1.90.0/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-29 07:46:49.446176 windmill_api-1.90.0/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-04-29 07:46:49.474176 windmill_api-1.90.0/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-04-29 07:46:49.562177 windmill_api-1.90.0/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-04-29 07:46:49.498176 windmill_api-1.90.0/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-04-29 07:46:49.558177 windmill_api-1.90.0/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-04-29 07:46:49.582177 windmill_api-1.90.0/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-04-29 07:46:49.590177 windmill_api-1.90.0/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-04-29 07:46:49.610177 windmill_api-1.90.0/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-04-29 07:46:49.650178 windmill_api-1.90.0/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-04-29 07:46:49.630177 windmill_api-1.90.0/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-04-29 07:46:49.690178 windmill_api-1.90.0/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-04-29 07:46:49.674178 windmill_api-1.90.0/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-04-29 07:46:49.710178 windmill_api-1.90.0/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-04-29 07:46:49.722178 windmill_api-1.90.0/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-04-29 07:46:49.738178 windmill_api-1.90.0/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-04-29 07:46:18.189917 windmill_api-1.90.0/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-04-29 07:46:49.734178 windmill_api-1.90.0/windmill_api/types.py
--rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 windmill_api-1.90.0/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.90.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-01 17:00:18.173403 windmill_api-1.91.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-01 17:00:18.177403 windmill_api-1.91.0/README.md
+-rw-r--r--   0        0        0      717 2023-05-01 17:00:18.173403 windmill_api-1.91.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-01 16:59:46.784949 windmill_api-1.91.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-01 16:59:47.264956 windmill_api-1.91.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.368957 windmill_api-1.91.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-01 16:59:57.617104 windmill_api-1.91.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-01 16:59:57.617104 windmill_api-1.91.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-01 16:59:57.645104 windmill_api-1.91.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-01 16:59:57.673105 windmill_api-1.91.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-01 16:59:57.685105 windmill_api-1.91.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-01 16:59:57.713105 windmill_api-1.91.0/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-01 16:59:57.721105 windmill_api-1.91.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-01 16:59:57.761106 windmill_api-1.91.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-01 16:59:57.773106 windmill_api-1.91.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-01 16:59:57.789106 windmill_api-1.91.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-01 16:59:57.861107 windmill_api-1.91.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-01 16:59:57.825107 windmill_api-1.91.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-01 16:59:57.853107 windmill_api-1.91.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.300956 windmill_api-1.91.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-01 16:59:57.897108 windmill_api-1.91.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-01 16:59:57.961109 windmill_api-1.91.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.440958 windmill_api-1.91.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-01 16:59:57.925109 windmill_api-1.91.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-01 16:59:57.953109 windmill_api-1.91.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-01 16:59:57.985109 windmill_api-1.91.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.376957 windmill_api-1.91.0/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-01 16:59:57.989109 windmill_api-1.91.0/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.440958 windmill_api-1.91.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-01 16:59:58.017110 windmill_api-1.91.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-01 16:59:58.017110 windmill_api-1.91.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.360957 windmill_api-1.91.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-01 16:59:58.049110 windmill_api-1.91.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-01 16:59:58.049110 windmill_api-1.91.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-01 16:59:58.073111 windmill_api-1.91.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-01 16:59:58.117111 windmill_api-1.91.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-01 16:59:58.125111 windmill_api-1.91.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-01 16:59:58.157112 windmill_api-1.91.0/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-01 16:59:58.185112 windmill_api-1.91.0/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-01 16:59:58.197113 windmill_api-1.91.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-01 16:59:58.209113 windmill_api-1.91.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-01 16:59:58.293114 windmill_api-1.91.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-01 16:59:58.241113 windmill_api-1.91.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-01 16:59:58.269114 windmill_api-1.91.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.432958 windmill_api-1.91.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-01 16:59:58.301114 windmill_api-1.91.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-01 16:59:58.321114 windmill_api-1.91.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-01 16:59:58.333115 windmill_api-1.91.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-01 16:59:58.361115 windmill_api-1.91.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-01 16:59:58.373115 windmill_api-1.91.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-01 16:59:58.405116 windmill_api-1.91.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-01 16:59:58.429116 windmill_api-1.91.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-01 16:59:58.457116 windmill_api-1.91.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-01 16:59:58.493117 windmill_api-1.91.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.436958 windmill_api-1.91.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-01 16:59:58.489117 windmill_api-1.91.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-01 16:59:58.529118 windmill_api-1.91.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-01 16:59:58.525117 windmill_api-1.91.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.424958 windmill_api-1.91.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-01 16:59:58.557118 windmill_api-1.91.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-01 16:59:58.557118 windmill_api-1.91.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-01 16:59:58.585118 windmill_api-1.91.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-01 16:59:58.597119 windmill_api-1.91.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-01 16:59:58.633119 windmill_api-1.91.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-01 16:59:58.653119 windmill_api-1.91.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-01 16:59:58.665120 windmill_api-1.91.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-01 16:59:58.681120 windmill_api-1.91.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.440958 windmill_api-1.91.0/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-01 16:59:58.713120 windmill_api-1.91.0/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-01 16:59:58.705120 windmill_api-1.91.0/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-01 16:59:58.793122 windmill_api-1.91.0/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-01 16:59:58.781121 windmill_api-1.91.0/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-01 16:59:58.833122 windmill_api-1.91.0/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.380957 windmill_api-1.91.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-01 16:59:58.821122 windmill_api-1.91.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-01 16:59:58.857123 windmill_api-1.91.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-01 16:59:58.873123 windmill_api-1.91.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-01 16:59:58.893123 windmill_api-1.91.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-01 16:59:58.913123 windmill_api-1.91.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-01 16:59:58.921124 windmill_api-1.91.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-01 16:59:58.957124 windmill_api-1.91.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-01 16:59:58.949124 windmill_api-1.91.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-01 16:59:58.985124 windmill_api-1.91.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-01 16:59:59.013125 windmill_api-1.91.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-01 16:59:59.037125 windmill_api-1.91.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-01 16:59:59.069126 windmill_api-1.91.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-01 16:59:59.193127 windmill_api-1.91.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-01 16:59:59.225128 windmill_api-1.91.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-01 16:59:59.337130 windmill_api-1.91.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-01 16:59:59.253128 windmill_api-1.91.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-01 16:59:59.285129 windmill_api-1.91.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-01 16:59:59.329130 windmill_api-1.91.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-01 16:59:59.377130 windmill_api-1.91.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-01 16:59:59.413131 windmill_api-1.91.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-01 16:59:59.417131 windmill_api-1.91.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-01 16:59:59.497132 windmill_api-1.91.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-01 16:59:59.469132 windmill_api-1.91.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-01 16:59:59.513132 windmill_api-1.91.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-01 16:59:59.537133 windmill_api-1.91.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-01 16:59:59.581133 windmill_api-1.91.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-01 16:59:59.581133 windmill_api-1.91.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.332957 windmill_api-1.91.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-01 16:59:59.625134 windmill_api-1.91.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-01 16:59:59.609134 windmill_api-1.91.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-01 16:59:59.637134 windmill_api-1.91.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-01 16:59:59.653134 windmill_api-1.91.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-01 16:59:59.661135 windmill_api-1.91.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-01 16:59:59.681135 windmill_api-1.91.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-01 16:59:59.697135 windmill_api-1.91.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-01 16:59:59.713135 windmill_api-1.91.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.336957 windmill_api-1.91.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-01 16:59:59.725136 windmill_api-1.91.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-01 16:59:59.741136 windmill_api-1.91.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-01 16:59:59.753136 windmill_api-1.91.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-01 16:59:59.769136 windmill_api-1.91.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-01 16:59:59.789137 windmill_api-1.91.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-01 16:59:59.821137 windmill_api-1.91.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-01 16:59:59.845137 windmill_api-1.91.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-01 16:59:59.861138 windmill_api-1.91.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-01 16:59:59.873138 windmill_api-1.91.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-01 16:59:59.949139 windmill_api-1.91.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-01 16:59:59.913138 windmill_api-1.91.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-01 16:59:59.953139 windmill_api-1.91.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-01 16:59:59.977139 windmill_api-1.91.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-01 16:59:59.981140 windmill_api-1.91.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-01 17:00:00.009140 windmill_api-1.91.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.420958 windmill_api-1.91.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-01 17:00:00.013140 windmill_api-1.91.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-01 17:00:00.033140 windmill_api-1.91.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-01 17:00:00.053140 windmill_api-1.91.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-01 17:00:00.073141 windmill_api-1.91.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-01 17:00:00.113141 windmill_api-1.91.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-01 17:00:00.113141 windmill_api-1.91.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-01 17:00:00.141142 windmill_api-1.91.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-01 17:00:00.141142 windmill_api-1.91.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.344957 windmill_api-1.91.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-01 17:00:00.205143 windmill_api-1.91.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-01 17:00:00.169142 windmill_api-1.91.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-01 17:00:00.205143 windmill_api-1.91.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-01 17:00:00.233143 windmill_api-1.91.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-01 17:00:00.265144 windmill_api-1.91.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-01 17:00:00.277144 windmill_api-1.91.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-01 17:00:00.301144 windmill_api-1.91.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-01 17:00:00.317144 windmill_api-1.91.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-01 17:00:00.337145 windmill_api-1.91.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-01 17:00:00.345145 windmill_api-1.91.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-01 17:00:00.377145 windmill_api-1.91.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-01 17:00:00.385146 windmill_api-1.91.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-01 17:00:00.417146 windmill_api-1.91.0/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-01 17:00:00.429146 windmill_api-1.91.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-01 17:00:00.453147 windmill_api-1.91.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-01 17:00:00.461147 windmill_api-1.91.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-01 17:00:00.477147 windmill_api-1.91.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-01 17:00:00.613149 windmill_api-1.91.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-01 17:00:00.513147 windmill_api-1.91.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-01 17:00:00.561148 windmill_api-1.91.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-01 17:00:00.589149 windmill_api-1.91.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-01 17:00:00.617149 windmill_api-1.91.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.276956 windmill_api-1.91.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-01 17:00:00.645150 windmill_api-1.91.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-01 17:00:00.641149 windmill_api-1.91.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.304956 windmill_api-1.91.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-01 17:00:00.665150 windmill_api-1.91.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-01 17:00:00.669150 windmill_api-1.91.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-01 17:00:00.693150 windmill_api-1.91.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-01 17:00:00.701150 windmill_api-1.91.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-01 17:00:00.717151 windmill_api-1.91.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-01 17:00:00.729151 windmill_api-1.91.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-01 17:00:00.741151 windmill_api-1.91.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-01 17:00:00.757151 windmill_api-1.91.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-01 17:00:00.765151 windmill_api-1.91.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-01 17:00:00.785152 windmill_api-1.91.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-01 17:00:00.793152 windmill_api-1.91.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-01 17:00:00.813152 windmill_api-1.91.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-01 17:00:00.825152 windmill_api-1.91.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-01 17:00:00.853153 windmill_api-1.91.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-01 17:00:00.849152 windmill_api-1.91.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-01 17:00:00.901153 windmill_api-1.91.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-01 17:00:00.913154 windmill_api-1.91.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-01 17:00:00.941154 windmill_api-1.91.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-01 17:00:00.969154 windmill_api-1.91.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-01 17:00:00.977154 windmill_api-1.91.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-01 17:00:01.009155 windmill_api-1.91.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-01 17:00:01.005155 windmill_api-1.91.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-01 17:00:01.029155 windmill_api-1.91.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-01 17:00:01.037155 windmill_api-1.91.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-01 17:00:01.057156 windmill_api-1.91.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-01 17:00:01.077156 windmill_api-1.91.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-01 17:00:01.097156 windmill_api-1.91.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.328957 windmill_api-1.91.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-01 17:00:01.113156 windmill_api-1.91.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-01 17:00:01.125157 windmill_api-1.91.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-01 17:00:01.157157 windmill_api-1.91.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-01 17:00:01.173157 windmill_api-1.91.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-01 17:00:01.197158 windmill_api-1.91.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-01 17:00:01.229158 windmill_api-1.91.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-01 17:00:01.253159 windmill_api-1.91.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.380957 windmill_api-1.91.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-01 17:00:01.265159 windmill_api-1.91.0/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-01 17:00:01.309159 windmill_api-1.91.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:59:47.316957 windmill_api-1.91.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-01 17:00:01.293159 windmill_api-1.91.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-01 17:00:01.317160 windmill_api-1.91.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-01 17:00:01.337160 windmill_api-1.91.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-01 17:00:01.345160 windmill_api-1.91.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-01 17:00:01.365160 windmill_api-1.91.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-01 17:00:01.373160 windmill_api-1.91.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-01 17:00:01.397161 windmill_api-1.91.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-01 17:00:01.401161 windmill_api-1.91.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-01 17:00:01.425161 windmill_api-1.91.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-01 17:00:01.425161 windmill_api-1.91.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-01 17:00:01.461162 windmill_api-1.91.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-01 17:00:01.461162 windmill_api-1.91.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-01 17:00:01.493162 windmill_api-1.91.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-01 17:00:01.493162 windmill_api-1.91.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-01 17:00:01.533163 windmill_api-1.91.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-01 17:00:01.545163 windmill_api-1.91.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-01 17:00:01.573163 windmill_api-1.91.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-01 17:00:01.593164 windmill_api-1.91.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-01 17:00:01.617164 windmill_api-1.91.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-01 17:00:01.621164 windmill_api-1.91.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-01 17:00:18.169403 windmill_api-1.91.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-01 17:00:01.645165 windmill_api-1.91.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-01 17:00:01.673165 windmill_api-1.91.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-05-01 16:59:56.209083 windmill_api-1.91.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-01 17:00:01.701165 windmill_api-1.91.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-01 17:00:01.729166 windmill_api-1.91.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-01 17:00:01.753166 windmill_api-1.91.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-01 17:00:01.793167 windmill_api-1.91.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-01 16:59:56.705090 windmill_api-1.91.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-01 17:00:01.773167 windmill_api-1.91.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-01 17:00:01.821167 windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-01 16:59:56.753091 windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-01 17:00:01.821167 windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-01 17:00:01.841168 windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-01 17:00:01.845167 windmill_api-1.91.0/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-01 17:00:01.965169 windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-01 17:00:01.865168 windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-01 16:59:56.985094 windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-01 16:59:56.673090 windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-01 17:00:01.901168 windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-01 17:00:01.949169 windmill_api-1.91.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-01 16:59:56.741091 windmill_api-1.91.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-01 16:59:56.633089 windmill_api-1.91.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-01 17:00:01.973169 windmill_api-1.91.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-01 17:00:02.009170 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-01 17:00:02.033170 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-01 16:59:56.649089 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-01 17:00:02.045171 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-01 17:00:02.057171 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-01 17:00:02.073171 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-01 17:00:02.093171 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-01 16:59:56.813092 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-01 17:00:02.101171 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-01 17:00:02.129172 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-01 16:59:56.753091 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-01 17:00:02.129172 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-01 16:59:56.053080 windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-01 17:00:02.165172 windmill_api-1.91.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-01 17:00:02.169172 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-01 17:00:02.261174 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-01 17:00:02.205173 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-01 17:00:02.237173 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-01 17:00:02.269174 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-01 17:00:02.289174 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.725090 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-01 17:00:02.301174 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.325084 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-01 17:00:02.317175 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-01 17:00:02.349175 windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-01 16:59:56.253083 windmill_api-1.91.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-01 17:00:02.357175 windmill_api-1.91.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-01 17:00:02.385176 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-01 17:00:02.433176 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-01 17:00:02.425176 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-01 17:00:02.453177 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-01 17:00:02.465177 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-01 17:00:02.485177 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.637089 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-01 17:00:02.493177 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.193082 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-01 17:00:02.513177 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-01 17:00:02.521178 windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-01 17:00:02.597179 windmill_api-1.91.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-01 17:00:02.561178 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-01 17:00:02.585179 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-01 17:00:02.637179 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-01 17:00:02.625179 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-01 16:59:56.321084 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-01 17:00:02.657180 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-01 16:59:56.897093 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-01 17:00:02.665180 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-01 17:00:02.685180 windmill_api-1.91.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-01 16:59:56.733090 windmill_api-1.91.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-01 17:00:02.689180 windmill_api-1.91.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-01 17:00:02.729181 windmill_api-1.91.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-01 17:00:02.821182 windmill_api-1.91.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-01 17:00:02.749181 windmill_api-1.91.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-01 17:00:02.789182 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-01 17:00:02.877183 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-01 17:00:02.845183 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-01 17:00:02.873183 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-01 16:59:56.913093 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-01 17:00:02.901183 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-01 17:00:02.917183 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-01 16:59:56.173082 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-01 17:00:03.017185 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-01 17:00:02.941184 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-01 17:00:02.969184 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-01 16:59:55.937079 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-01 17:00:02.997185 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-01 17:00:03.037185 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-01 16:59:56.985094 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-01 17:00:03.053186 windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-01 16:59:56.401085 windmill_api-1.91.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-01 16:59:55.925078 windmill_api-1.91.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-01 17:00:03.129187 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-01 17:00:03.129187 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-01 17:00:03.169187 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-01 17:00:03.161187 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-01 17:00:03.193188 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-01 17:00:03.201188 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.489087 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-01 17:00:03.221188 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.485087 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-01 17:00:03.233188 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-01 17:00:03.249188 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-01 17:00:03.313189 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-01 17:00:03.289189 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-01 17:00:03.317189 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-01 17:00:03.345190 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-01 17:00:03.369190 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-01 16:59:56.293084 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-01 17:00:03.373190 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-01 16:59:56.329084 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-01 17:00:03.401191 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-01 17:00:03.405191 windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-01 17:00:03.425191 windmill_api-1.91.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-01 17:00:03.445191 windmill_api-1.91.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-01 17:00:03.449191 windmill_api-1.91.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-01 17:00:03.473192 windmill_api-1.91.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-01 17:00:03.497192 windmill_api-1.91.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-01 17:00:03.509192 windmill_api-1.91.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-01 17:00:03.541193 windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-01 16:59:56.993095 windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-01 17:00:03.537193 windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-01 17:00:03.557193 windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-01 17:00:03.573193 windmill_api-1.91.0/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-01 16:59:56.445086 windmill_api-1.91.0/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-01 17:00:03.581193 windmill_api-1.91.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-01 17:00:03.609194 windmill_api-1.91.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-01 17:00:03.609194 windmill_api-1.91.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-01 17:00:03.637194 windmill_api-1.91.0/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-01 17:00:03.629194 windmill_api-1.91.0/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-01 17:00:03.653194 windmill_api-1.91.0/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-01 17:00:03.661194 windmill_api-1.91.0/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-01 16:59:55.953079 windmill_api-1.91.0/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     2094 2023-05-01 17:00:03.685195 windmill_api-1.91.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-01 17:00:03.689195 windmill_api-1.91.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-01 17:00:03.721195 windmill_api-1.91.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-01 17:00:03.733195 windmill_api-1.91.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-01 17:00:03.765196 windmill_api-1.91.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-01 17:00:03.809197 windmill_api-1.91.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-01 16:59:56.993095 windmill_api-1.91.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-01 16:59:55.929078 windmill_api-1.91.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-01 17:00:03.785196 windmill_api-1.91.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-01 17:00:03.821197 windmill_api-1.91.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-01 17:00:03.841197 windmill_api-1.91.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-01 17:00:03.857197 windmill_api-1.91.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-01 17:00:03.893198 windmill_api-1.91.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-01 17:00:03.897198 windmill_api-1.91.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-01 17:00:03.933198 windmill_api-1.91.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-01 17:00:03.921198 windmill_api-1.91.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-01 17:00:03.949199 windmill_api-1.91.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-01 17:00:03.957199 windmill_api-1.91.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-01 17:00:04.077201 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-01 17:00:03.977199 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-01 17:00:04.017200 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-01 17:00:04.105201 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-01 17:00:04.133201 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-01 17:00:04.133201 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-01 16:59:56.521087 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-01 17:00:04.161202 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-01 17:00:04.181202 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-01 16:59:56.729091 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-01 17:00:04.241203 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-01 17:00:04.209202 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-01 17:00:04.233203 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-01 16:59:56.093081 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-01 17:00:04.289204 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-01 17:00:04.277203 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-01 16:59:56.113081 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-01 17:00:04.309204 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-01 16:59:55.929078 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-01 16:59:56.461086 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-01 17:00:04.337204 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-01 17:00:04.389205 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-01 17:00:04.377205 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-01 17:00:04.409205 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-01 17:00:04.421206 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-01 17:00:04.449206 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.121081 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-01 17:00:04.449206 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.713090 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-01 17:00:04.501207 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-01 17:00:04.477206 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-01 17:00:04.561208 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-01 17:00:04.541207 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-01 17:00:04.569208 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-01 17:00:04.593208 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-01 17:00:04.597208 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.697090 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-01 17:00:04.625208 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.505087 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-01 17:00:04.625208 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-01 17:00:04.673209 windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-01 17:00:04.653209 windmill_api-1.91.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-01 17:00:04.745210 windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-01 17:00:04.693210 windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-01 16:59:56.521087 windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-01 16:59:56.013080 windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-01 17:00:04.717210 windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-01 17:00:04.761211 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-01 17:00:04.801211 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-01 16:59:56.109081 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-01 17:00:04.785211 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-01 17:00:04.809211 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-01 17:00:04.865212 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-01 17:00:04.849212 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-01 16:59:56.505087 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-01 17:00:04.877212 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-01 17:00:04.901213 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-01 16:59:56.429086 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-01 17:00:04.905213 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-01 16:59:56.289084 windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-01 17:00:04.925213 windmill_api-1.91.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-01 17:00:04.937213 windmill_api-1.91.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-01 17:00:04.953213 windmill_api-1.91.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-01 17:00:04.965214 windmill_api-1.91.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-01 17:00:04.973214 windmill_api-1.91.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-01 17:00:04.993214 windmill_api-1.91.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-01 17:00:05.009214 windmill_api-1.91.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-01 17:00:05.017214 windmill_api-1.91.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-01 17:00:05.037215 windmill_api-1.91.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-01 17:00:05.081215 windmill_api-1.91.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-01 17:00:05.061215 windmill_api-1.91.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-01 17:00:05.089215 windmill_api-1.91.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-01 17:00:05.109216 windmill_api-1.91.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-01 17:00:05.109216 windmill_api-1.91.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-01 17:00:05.177217 windmill_api-1.91.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-01 17:00:05.133216 windmill_api-1.91.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-01 17:00:05.181217 windmill_api-1.91.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-01 17:00:05.197217 windmill_api-1.91.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-01 17:00:05.285218 windmill_api-1.91.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-01 17:00:05.237218 windmill_api-1.91.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-01 17:00:05.269218 windmill_api-1.91.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-01 17:00:05.301218 windmill_api-1.91.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-01 17:00:05.317219 windmill_api-1.91.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-01 16:59:56.537088 windmill_api-1.91.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-01 17:00:05.325219 windmill_api-1.91.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-01 16:59:56.233083 windmill_api-1.91.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-01 17:00:05.345219 windmill_api-1.91.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-01 17:00:05.353219 windmill_api-1.91.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-01 17:00:05.393220 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-01 17:00:05.389220 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-01 17:00:05.441221 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.509087 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-01 17:00:05.421220 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.525087 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-01 16:59:56.321084 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-01 16:59:56.889093 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-01 17:00:05.461221 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-01 17:00:05.477221 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-01 17:00:05.493221 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.965094 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-01 17:00:05.505221 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.781091 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-01 16:59:56.201083 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-01 17:00:05.525222 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-01 17:00:05.537222 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-01 17:00:05.557222 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.829092 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-01 17:00:05.569222 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.821092 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-01 16:59:56.189082 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-01 17:00:05.649224 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-01 17:00:05.597223 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-01 16:59:56.381085 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-01 17:00:05.625223 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-01 16:59:56.885093 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-01 17:00:05.705224 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-01 17:00:05.689224 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-01 17:00:05.721225 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-01 17:00:05.733225 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-01 17:00:05.749225 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.973094 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-01 17:00:05.789226 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:55.925078 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-01 17:00:05.777225 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-01 17:00:05.809226 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-01 16:59:56.329084 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-01 17:00:05.825226 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-01 17:00:05.845226 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-01 17:00:05.913227 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-01 17:00:05.889227 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-01 17:00:05.917228 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-01 17:00:05.945228 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-01 17:00:05.949228 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.345085 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-01 17:00:05.973228 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.221083 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-01 17:00:05.981228 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-01 17:00:06.001229 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-01 17:00:06.093230 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-01 17:00:06.041229 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-01 17:00:06.069230 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-01 17:00:06.101230 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-01 17:00:06.125231 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:55.993079 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-01 17:00:06.161231 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-01 16:59:56.105081 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-01 17:00:06.153231 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-01 17:00:06.181231 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-01 16:59:56.001079 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-01 17:00:06.201232 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-01 17:00:06.217232 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-01 17:00:06.281233 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-01 17:00:06.253232 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-01 17:00:06.281233 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-01 17:00:06.313233 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-01 17:00:06.309233 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.165082 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-01 17:00:06.341234 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.457086 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-01 17:00:06.345234 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-01 17:00:06.369234 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-01 16:59:56.657089 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-01 17:00:06.377234 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-01 16:59:56.841092 windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-01 17:00:06.429235 windmill_api-1.91.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-01 17:00:06.397235 windmill_api-1.91.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-01 17:00:06.437235 windmill_api-1.91.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-01 17:00:06.509236 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-01 17:00:06.477236 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-01 17:00:06.537237 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-01 17:00:06.541237 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-01 17:00:06.565237 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.533088 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-01 17:00:06.569237 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.049080 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-01 17:00:06.597237 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-01 17:00:06.597237 windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-01 17:00:06.677239 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-01 17:00:06.633238 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-01 17:00:06.661238 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-01 17:00:06.693239 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-01 17:00:06.705239 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-01 16:59:56.145082 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-01 17:00:06.721239 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-01 16:59:56.061080 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-01 17:00:06.737239 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-01 17:00:06.749240 windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-01 17:00:06.757240 windmill_api-1.91.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-01 17:00:06.821241 windmill_api-1.91.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-01 17:00:06.841241 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-01 17:00:06.845241 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-01 17:00:06.873242 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-01 16:59:56.113081 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-01 17:00:06.873242 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-01 17:00:06.945243 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-01 16:59:56.729091 windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-01 17:00:06.953243 windmill_api-1.91.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-01 17:00:06.973243 windmill_api-1.91.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-01 17:00:06.981243 windmill_api-1.91.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-01 16:59:56.781091 windmill_api-1.91.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-01 17:00:07.001243 windmill_api-1.91.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-01 17:00:07.017244 windmill_api-1.91.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-01 16:59:56.809092 windmill_api-1.91.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-01 17:00:07.085245 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-01 17:00:07.041244 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-01 17:00:07.069244 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-01 16:59:56.441086 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-01 17:00:07.093245 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-01 17:00:07.121245 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-01 16:59:56.301084 windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-01 17:00:07.125245 windmill_api-1.91.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-01 17:00:07.165246 windmill_api-1.91.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-01 17:00:07.245247 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-01 17:00:07.201246 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-01 17:00:07.233247 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-01 17:00:07.265247 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-01 17:00:07.273247 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-01 16:59:56.469087 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-01 17:00:07.325248 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-01 16:59:56.693090 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-01 17:00:07.301248 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-01 17:00:07.329248 windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-01 17:00:07.405249 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-01 17:00:07.369249 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-01 17:00:07.397249 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-01 17:00:07.429250 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-01 17:00:07.433250 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-01 16:59:56.301084 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-01 17:00:07.453250 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-01 16:59:56.485087 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-01 17:00:07.465250 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-01 17:00:07.481250 windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-01 17:00:07.493251 windmill_api-1.91.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-01 17:00:07.501251 windmill_api-1.91.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-01 17:00:07.521251 windmill_api-1.91.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-01 17:00:07.585252 windmill_api-1.91.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-01 17:00:07.549251 windmill_api-1.91.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-01 16:59:56.661090 windmill_api-1.91.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-01 17:00:07.577252 windmill_api-1.91.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-01 16:59:56.537088 windmill_api-1.91.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-01 17:00:07.661253 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-01 17:00:07.625253 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-01 17:00:07.653253 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-01 17:00:07.685253 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-01 17:00:07.733254 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-01 16:59:55.961079 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-01 17:00:07.709254 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-01 16:59:56.913093 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-01 17:00:07.741254 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-01 17:00:07.761254 windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-01 16:59:56.145082 windmill_api-1.91.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-01 17:00:07.789255 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-01 16:59:56.937094 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-01 17:00:07.785255 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-01 17:00:07.833256 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-01 16:59:56.325084 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-01 17:00:07.813255 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-01 17:00:07.833256 windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-01 17:00:07.893257 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-01 16:59:56.773091 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-01 17:00:07.853256 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-01 17:00:07.937257 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-01 16:59:56.353085 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-01 17:00:07.917257 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-01 17:00:07.941257 windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-01 17:00:07.985258 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-01 16:59:56.389085 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-01 17:00:07.961258 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-01 17:00:08.009258 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-01 16:59:56.701090 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-01 17:00:08.009258 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-01 17:00:08.029258 windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-01 17:00:08.057259 windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-01 16:59:56.545088 windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-01 16:59:56.829092 windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-01 17:00:08.053259 windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-01 17:00:08.217261 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-01 17:00:08.077259 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-01 17:00:08.121260 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-01 17:00:08.205261 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-01 17:00:08.233261 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-01 17:00:08.245262 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-01 16:59:56.201083 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-01 17:00:08.261262 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-01 17:00:08.277262 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-01 16:59:55.929078 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-01 17:00:08.397264 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-01 17:00:08.305262 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-01 17:00:08.333263 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-01 16:59:56.425086 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-01 17:00:08.361263 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-01 17:00:08.393264 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-01 16:59:56.201083 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-01 17:00:08.429264 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-01 16:59:56.217083 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-01 16:59:56.369085 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-01 17:00:08.445264 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-01 17:00:08.545266 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-01 17:00:08.485265 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-01 17:00:08.517266 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-01 17:00:08.549266 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-01 17:00:08.573266 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-01 16:59:56.221083 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-01 17:00:08.577267 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-01 16:59:56.857092 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-01 17:00:08.601267 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-01 17:00:08.605267 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-01 17:00:08.681268 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-01 17:00:08.645268 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-01 17:00:08.673268 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-01 17:00:08.749269 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-01 17:00:08.713268 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.513087 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-01 17:00:08.741269 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.393085 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-01 17:00:08.769269 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-01 17:00:08.781269 windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-01 17:00:08.873271 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-01 17:00:08.801270 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-01 17:00:08.821270 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-01 17:00:08.861271 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-01 17:00:08.945272 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-01 17:00:08.909271 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-01 17:00:08.937272 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-01 17:00:08.969272 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-01 17:00:08.973272 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-01 16:59:55.909078 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-01 17:00:09.001273 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-01 16:59:55.977079 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-01 17:00:09.001273 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-01 17:00:09.029273 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-01 17:00:09.121275 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-01 17:00:09.069274 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-01 17:00:09.097274 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-01 17:00:09.129274 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-01 17:00:09.149275 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-01 16:59:55.921078 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-01 17:00:09.161275 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-01 16:59:56.321084 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-01 17:00:09.177275 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-01 17:00:09.189275 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-01 17:00:09.205276 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-01 17:00:09.257276 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-01 17:00:09.225276 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-01 17:00:09.245276 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-01 17:00:09.289277 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-01 17:00:09.377278 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-01 17:00:09.325277 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-01 17:00:09.357278 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-01 17:00:09.389278 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-01 17:00:09.405279 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-01 16:59:56.137081 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-01 17:00:09.421279 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-01 16:59:56.237083 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-01 17:00:09.433279 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-01 17:00:09.449279 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-01 17:00:09.513280 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-01 17:00:09.537281 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-01 17:00:09.541281 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-01 17:00:09.569281 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-01 17:00:09.573281 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-01 16:59:56.089081 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-01 17:00:09.597282 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-01 16:59:56.961094 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-01 17:00:09.601282 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-01 17:00:09.625282 windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-01 17:00:09.641282 windmill_api-1.91.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-01 17:00:09.645282 windmill_api-1.91.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-01 17:00:09.717283 windmill_api-1.91.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-01 17:00:09.665282 windmill_api-1.91.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-01 17:00:09.697283 windmill_api-1.91.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-05-01 16:59:56.149082 windmill_api-1.91.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-01 17:00:09.721283 windmill_api-1.91.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-01 17:00:09.761284 windmill_api-1.91.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-01 17:00:09.741284 windmill_api-1.91.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-01 17:00:09.765284 windmill_api-1.91.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-01 17:00:09.785284 windmill_api-1.91.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-01 17:00:09.805285 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-01 17:00:09.825285 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-01 17:00:09.825285 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-01 17:00:09.869285 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-01 17:00:09.905286 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-01 17:00:09.953287 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-01 17:00:09.937286 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-01 17:00:09.969287 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-01 17:00:09.985287 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.693090 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-01 17:00:09.997287 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.197082 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-01 17:00:10.017288 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-01 17:00:10.025288 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-01 17:00:10.113289 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-01 17:00:10.121289 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-01 17:00:10.145290 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-01 17:00:10.153290 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-01 17:00:10.173290 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-01 16:59:57.001095 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-01 17:00:10.181290 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-01 16:59:56.769091 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-01 17:00:10.205290 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-01 17:00:10.209290 windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-01 17:00:10.245291 windmill_api-1.91.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-01 16:59:56.941094 windmill_api-1.91.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-01 17:00:10.249291 windmill_api-1.91.0/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-01 17:00:10.265291 windmill_api-1.91.0/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-01 16:59:56.293084 windmill_api-1.91.0/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-01 17:00:10.289291 windmill_api-1.91.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-01 16:59:56.469087 windmill_api-1.91.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-01 17:00:10.305292 windmill_api-1.91.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-01 17:00:10.317292 windmill_api-1.91.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-01 17:00:10.401293 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-01 16:59:55.929078 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-01 17:00:10.337292 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-01 17:00:10.385293 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-01 16:59:56.361085 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-01 17:00:10.413293 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-01 17:00:10.425294 windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-01 17:00:10.461294 windmill_api-1.91.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-01 17:00:10.445294 windmill_api-1.91.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-01 17:00:10.481294 windmill_api-1.91.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-01 17:00:10.489294 windmill_api-1.91.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-01 17:00:10.545295 windmill_api-1.91.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-01 17:00:10.509295 windmill_api-1.91.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-01 17:00:10.529295 windmill_api-1.91.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-01 17:00:10.669297 windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-01 17:00:10.561296 windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-01 16:59:56.993095 windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-01 16:59:56.453086 windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-01 17:00:10.589296 windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-01 17:00:10.681297 windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-01 17:00:10.689297 windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-01 16:59:56.657089 windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-01 16:59:56.469087 windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-01 17:00:10.705298 windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-01 17:00:10.773299 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-01 17:00:10.833299 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-01 16:59:56.253083 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-01 16:59:56.969094 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-01 17:00:10.797299 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-01 16:59:56.053080 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-01 16:59:56.957094 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-01 17:00:10.821299 windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-01 17:00:10.849300 windmill_api-1.91.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-01 17:00:10.889300 windmill_api-1.91.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-01 17:00:10.881300 windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-01 17:00:10.905300 windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-01 17:00:10.917301 windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-01 16:59:55.985079 windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-01 17:00:11.021302 windmill_api-1.91.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-01 17:00:10.937301 windmill_api-1.91.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-01 17:00:10.973301 windmill_api-1.91.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-01 16:59:56.369085 windmill_api-1.91.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-01 17:00:10.997302 windmill_api-1.91.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-01 17:00:11.037302 windmill_api-1.91.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-01 16:59:56.093081 windmill_api-1.91.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-01 17:00:11.061303 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-01 17:00:11.097303 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-01 16:59:56.433086 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-01 17:00:11.089303 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-01 17:00:11.117303 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-01 17:00:11.121303 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-01 17:00:11.153304 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-01 16:59:55.937079 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-01 17:00:11.197305 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-01 17:00:11.189304 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-01 16:59:56.121081 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-01 17:00:11.213305 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.345085 windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-01 17:00:11.241305 windmill_api-1.91.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-01 17:00:11.233305 windmill_api-1.91.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-01 17:00:11.261305 windmill_api-1.91.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-01 16:59:56.229083 windmill_api-1.91.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-01 17:00:11.277306 windmill_api-1.91.0/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-01 17:00:11.281306 windmill_api-1.91.0/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-01 17:00:11.305306 windmill_api-1.91.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-01 16:59:56.369085 windmill_api-1.91.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-01 17:00:11.309306 windmill_api-1.91.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-01 16:59:56.837092 windmill_api-1.91.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-01 17:00:11.337306 windmill_api-1.91.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-01 17:00:11.333306 windmill_api-1.91.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-01 16:59:56.381085 windmill_api-1.91.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-01 17:00:11.365307 windmill_api-1.91.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-01 16:59:56.869093 windmill_api-1.91.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-01 17:00:11.385307 windmill_api-1.91.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-01 16:59:56.069080 windmill_api-1.91.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-01 17:00:11.385307 windmill_api-1.91.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-01 16:59:56.521087 windmill_api-1.91.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-01 17:00:11.433308 windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-01 16:59:56.945094 windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-01 16:59:56.493087 windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-01 17:00:11.413308 windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-01 17:00:11.589310 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-01 17:00:11.453308 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-01 17:00:11.497309 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-01 17:00:11.625311 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-01 17:00:11.613310 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-01 17:00:11.645311 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-01 16:59:56.189082 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-01 17:00:11.649311 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-01 17:00:11.677311 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-01 16:59:56.365085 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-01 17:00:11.733312 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-01 17:00:11.701311 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-01 17:00:11.729312 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-01 16:59:56.273084 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-01 17:00:11.757312 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-01 17:00:11.773313 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-01 16:59:56.441086 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-01 17:00:11.789313 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-01 16:59:56.833092 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-01 16:59:56.437086 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-01 17:00:11.817313 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-01 17:00:11.925315 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-01 17:00:11.857314 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-01 17:00:11.885314 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-01 17:00:11.921315 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-01 17:00:12.001316 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-01 16:59:55.897078 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-01 17:00:11.953315 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-01 16:59:56.565088 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-01 17:00:11.985316 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-01 17:00:12.013316 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-01 17:00:12.081317 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-01 17:00:12.053316 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-01 17:00:12.081317 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-01 17:00:12.113317 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-01 17:00:12.109317 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-01 16:59:55.921078 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-01 17:00:12.137318 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-01 16:59:56.241083 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-01 17:00:12.141318 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-01 17:00:12.165318 windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-01 17:00:12.169318 windmill_api-1.91.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-01 17:00:12.193318 windmill_api-1.91.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-01 17:00:12.201319 windmill_api-1.91.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-01 17:00:12.213319 windmill_api-1.91.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-01 17:00:12.245319 windmill_api-1.91.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-01 17:00:12.233319 windmill_api-1.91.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-01 17:00:12.265319 windmill_api-1.91.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-01 17:00:12.281320 windmill_api-1.91.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-01 17:00:12.293320 windmill_api-1.91.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-01 17:00:12.313320 windmill_api-1.91.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-01 17:00:12.373321 windmill_api-1.91.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-01 17:00:12.405321 windmill_api-1.91.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-01 16:59:56.621089 windmill_api-1.91.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-01 17:00:12.409321 windmill_api-1.91.0/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-01 17:00:12.425322 windmill_api-1.91.0/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-01 16:59:56.465087 windmill_api-1.91.0/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-01 17:00:12.441322 windmill_api-1.91.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-01 16:59:55.901078 windmill_api-1.91.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-01 17:00:12.457322 windmill_api-1.91.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-01 17:00:12.593324 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-01 17:00:12.473322 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-01 17:00:12.517323 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-01 17:00:12.601324 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-01 17:00:12.617324 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-01 17:00:12.629325 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-01 16:59:57.005095 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-01 17:00:12.645325 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-01 17:00:12.661325 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-01 16:59:56.581088 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-01 17:00:12.789327 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-01 17:00:12.689325 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-01 17:00:12.713326 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-01 16:59:56.817092 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-01 17:00:12.797327 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-01 17:00:12.825327 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-01 16:59:56.321084 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-01 17:00:12.829327 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-01 16:59:57.013095 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-01 16:59:56.461086 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-01 17:00:12.869328 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-01 17:00:12.909329 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-01 17:00:12.909329 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-01 17:00:12.937329 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-01 17:00:12.941329 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-01 17:00:12.965329 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.677090 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-01 17:00:12.973329 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.313084 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-01 17:00:12.993330 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-01 17:00:13.001330 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-01 17:00:13.073331 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-01 17:00:13.037330 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-01 17:00:13.069331 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-01 17:00:13.101331 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-01 17:00:13.101331 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-01 16:59:56.465087 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-01 17:00:13.177332 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-01 16:59:56.205083 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-01 17:00:13.185332 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-01 17:00:13.205333 windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-05-01 17:00:13.249333 windmill_api-1.91.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-01 17:00:13.225333 windmill_api-1.91.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-01 17:00:13.261334 windmill_api-1.91.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-01 17:00:13.305334 windmill_api-1.91.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-01 17:00:13.277334 windmill_api-1.91.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-01 17:00:13.297334 windmill_api-1.91.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-01 17:00:13.393335 windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-01 17:00:13.325334 windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-01 16:59:56.761091 windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-01 16:59:56.757091 windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-01 17:00:13.349335 windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-01 17:00:13.389335 windmill_api-1.91.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-01 17:00:13.417336 windmill_api-1.91.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-01 17:00:13.421336 windmill_api-1.91.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-01 17:00:13.457336 windmill_api-1.91.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-01 16:59:56.777091 windmill_api-1.91.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-01 17:00:13.481337 windmill_api-1.91.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-01 17:00:13.481337 windmill_api-1.91.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-01 17:00:13.605338 windmill_api-1.91.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-01 17:00:13.501337 windmill_api-1.91.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-01 17:00:13.541337 windmill_api-1.91.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-01 17:00:13.625339 windmill_api-1.91.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-01 17:00:13.637339 windmill_api-1.91.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-01 17:00:13.657339 windmill_api-1.91.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-01 17:00:13.681339 windmill_api-1.91.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-01 16:59:56.561088 windmill_api-1.91.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-01 17:00:13.681339 windmill_api-1.91.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-01 17:00:13.745340 windmill_api-1.91.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-01 17:00:13.701340 windmill_api-1.91.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-01 17:00:13.757341 windmill_api-1.91.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-01 17:00:13.761340 windmill_api-1.91.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-01 17:00:13.785341 windmill_api-1.91.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-01 17:00:13.789341 windmill_api-1.91.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-01 17:00:13.813341 windmill_api-1.91.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-01 17:00:13.825342 windmill_api-1.91.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-01 17:00:13.869342 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-01 16:59:56.585088 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-01 17:00:13.853342 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-01 17:00:13.877342 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-01 17:00:13.897343 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-01 17:00:13.913343 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-01 16:59:56.029080 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-01 17:00:13.973343 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-01 17:00:13.949343 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-01 16:59:56.069080 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-01 17:00:14.029344 windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-01 16:59:56.033080 windmill_api-1.91.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-01 17:00:14.013344 windmill_api-1.91.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-01 17:00:14.033344 windmill_api-1.91.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-01 17:00:14.101345 windmill_api-1.91.0/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-01 16:59:56.625089 windmill_api-1.91.0/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.785091 windmill_api-1.91.0/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-01 17:00:14.053345 windmill_api-1.91.0/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-01 17:00:14.089345 windmill_api-1.91.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-01 17:00:14.125346 windmill_api-1.91.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-01 17:00:14.129346 windmill_api-1.91.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-01 17:00:14.165346 windmill_api-1.91.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-01 17:00:14.149346 windmill_api-1.91.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-01 17:00:14.189347 windmill_api-1.91.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-01 17:00:14.241347 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-01 17:00:14.225347 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-01 17:00:14.257347 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-01 17:00:14.273348 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-01 17:00:14.285348 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-01 16:59:56.221083 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-01 17:00:14.301348 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-01 16:59:56.853092 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-01 17:00:14.313348 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-01 17:00:14.381349 windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-01 17:00:14.393350 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-01 17:00:14.421350 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-01 17:00:14.477351 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-01 17:00:14.453350 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-01 17:00:14.481351 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-01 16:59:56.645089 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-01 17:00:14.505351 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-01 16:59:56.049080 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-01 17:00:14.509351 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-01 17:00:14.533352 windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-01 17:00:14.553352 windmill_api-1.91.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-01 17:00:14.553352 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-01 17:00:14.593352 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-01 17:00:14.633353 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-01 17:00:14.633353 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-01 17:00:14.661353 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-01 17:00:14.665353 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-01 17:00:14.689354 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-01 16:59:56.141082 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-01 17:00:14.693354 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-01 16:59:56.105081 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-01 17:00:14.717354 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-01 17:00:14.721354 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-01 17:00:14.857356 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-01 17:00:14.761355 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-01 17:00:14.789355 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-01 17:00:14.881356 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-01 17:00:14.885356 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.525087 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-01 17:00:14.909357 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.961094 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-01 17:00:14.933357 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-01 17:00:14.937357 windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-01 17:00:14.969358 windmill_api-1.91.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-01 17:00:15.005358 windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-01 17:00:15.033358 windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-01 16:59:56.177082 windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-01 17:00:15.037359 windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-01 16:59:56.029080 windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-01 16:59:56.229083 windmill_api-1.91.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-01 17:00:15.069359 windmill_api-1.91.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-01 17:00:15.069359 windmill_api-1.91.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-01 17:00:15.097359 windmill_api-1.91.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-01 16:59:56.881093 windmill_api-1.91.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-01 17:00:15.101359 windmill_api-1.91.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-01 16:59:56.477087 windmill_api-1.91.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-01 16:59:56.505087 windmill_api-1.91.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-01 17:00:15.149360 windmill_api-1.91.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-01 16:59:56.973094 windmill_api-1.91.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-01 17:00:15.125360 windmill_api-1.91.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-01 17:00:15.145360 windmill_api-1.91.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-01 17:00:15.181361 windmill_api-1.91.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-01 17:00:15.169360 windmill_api-1.91.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-01 16:59:56.805092 windmill_api-1.91.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-01 17:00:15.197361 windmill_api-1.91.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-01 17:00:15.221361 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-01 17:00:15.257362 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-01 16:59:56.037080 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-01 17:00:15.249361 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-01 17:00:15.277362 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-01 17:00:15.349363 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-01 17:00:15.313362 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-01 16:59:56.725090 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-01 17:00:15.341363 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-01 17:00:15.377363 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-01 16:59:55.913078 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-01 17:00:15.373363 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-01 16:59:56.901093 windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-01 17:00:15.525365 windmill_api-1.91.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-01 17:00:15.397364 windmill_api-1.91.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-01 17:00:15.437364 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-01 17:00:15.585366 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-01 17:00:15.549366 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-01 17:00:15.577366 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-01 16:59:56.505087 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-01 17:00:15.605367 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-01 17:00:15.617367 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-01 16:59:56.525087 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-01 17:00:15.765369 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-01 17:00:15.645367 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-01 17:00:15.673367 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-01 16:59:56.121081 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-01 17:00:15.701368 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-01 17:00:15.733368 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-01 16:59:55.905078 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-01 17:00:15.769369 windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-01 16:59:56.789091 windmill_api-1.91.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.253083 windmill_api-1.91.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-01 17:00:15.809369 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-01 17:00:15.849370 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-01 17:00:15.845370 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-01 17:00:15.873370 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-01 17:00:15.881370 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-01 17:00:15.901371 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.637089 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-01 17:00:15.909371 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-01 16:59:56.569088 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-01 17:00:15.933371 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-01 17:00:15.937371 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-01 17:00:16.073373 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-01 17:00:15.973372 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-01 17:00:16.001372 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-01 17:00:16.033372 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-01 17:00:16.061373 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-01 16:59:56.781091 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-01 17:00:16.093373 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-01 16:59:56.453086 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-01 17:00:16.101374 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-01 17:00:16.121374 windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-01 17:00:16.145374 windmill_api-1.91.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-01 17:00:16.153374 windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-01 17:00:16.173375 windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-01 16:59:56.469087 windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-01 17:00:16.181375 windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-01 16:59:56.413086 windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-01 16:59:56.897093 windmill_api-1.91.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-01 16:59:55.929078 windmill_api-1.91.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-01 17:00:16.201375 windmill_api-1.91.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-01 17:00:16.205375 windmill_api-1.91.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-05-01 16:59:56.293084 windmill_api-1.91.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-01 17:00:16.229375 windmill_api-1.91.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-01 17:00:16.229375 windmill_api-1.91.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-01 17:00:16.277376 windmill_api-1.91.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-01 17:00:16.249376 windmill_api-1.91.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-01 17:00:16.281376 windmill_api-1.91.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-01 17:00:16.297376 windmill_api-1.91.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-01 17:00:16.377377 windmill_api-1.91.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-01 17:00:16.333377 windmill_api-1.91.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-01 17:00:16.365377 windmill_api-1.91.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-01 17:00:16.397378 windmill_api-1.91.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-01 17:00:16.393378 windmill_api-1.91.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-01 17:00:16.425378 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-01 17:00:16.413378 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-01 17:00:16.453379 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-01 17:00:16.509379 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-01 17:00:16.493379 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-01 17:00:16.521379 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-01 17:00:16.541380 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-01 17:00:16.549380 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-01 16:59:56.077081 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-01 17:00:16.569380 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-01 16:59:56.021080 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-01 17:00:16.577380 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-01 17:00:16.597380 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-01 17:00:16.717382 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-01 17:00:16.637381 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-01 17:00:16.665382 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-01 17:00:16.697382 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-01 17:00:16.725382 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-01 16:59:56.841092 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-01 17:00:16.745383 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-01 16:59:56.669090 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-01 17:00:16.753383 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-01 17:00:16.773383 windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-01 17:00:16.773383 windmill_api-1.91.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-01 17:00:16.793383 windmill_api-1.91.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-01 17:00:16.809383 windmill_api-1.91.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-01 17:00:16.813383 windmill_api-1.91.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-01 16:59:56.757091 windmill_api-1.91.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-01 17:00:16.829384 windmill_api-1.91.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-01 17:00:16.829384 windmill_api-1.91.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-01 16:59:56.713090 windmill_api-1.91.0/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-01 17:00:16.889385 windmill_api-1.91.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-01 17:00:16.925385 windmill_api-1.91.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-01 17:00:16.909385 windmill_api-1.91.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-01 17:00:16.997386 windmill_api-1.91.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-01 17:00:16.941385 windmill_api-1.91.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-01 17:00:16.961386 windmill_api-1.91.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-01 16:59:56.637089 windmill_api-1.91.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-01 16:59:56.845092 windmill_api-1.91.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-01 17:00:16.985386 windmill_api-1.91.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-01 17:00:17.009386 windmill_api-1.91.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-01 17:00:17.089387 windmill_api-1.91.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-01 17:00:17.037387 windmill_api-1.91.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-01 17:00:17.061387 windmill_api-1.91.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-01 17:00:17.097387 windmill_api-1.91.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-05-01 16:59:56.769091 windmill_api-1.91.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-01 17:00:17.117388 windmill_api-1.91.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-01 16:59:56.541088 windmill_api-1.91.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-01 17:00:17.137388 windmill_api-1.91.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-01 17:00:17.157388 windmill_api-1.91.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-01 17:00:17.169388 windmill_api-1.91.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-05-01 16:59:56.729091 windmill_api-1.91.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-01 17:00:17.201389 windmill_api-1.91.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-01 17:00:17.213389 windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-01 16:59:56.369085 windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-01 17:00:17.229389 windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-01 17:00:17.233389 windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-01 17:00:17.269390 windmill_api-1.91.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-01 17:00:17.253390 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-01 17:00:17.293390 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-01 17:00:17.349391 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-01 17:00:17.333391 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-01 17:00:17.361391 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-01 17:00:17.381391 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-01 17:00:17.389392 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-01 16:59:56.741091 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-01 17:00:17.409392 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-01 16:59:56.885093 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-01 17:00:17.417392 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-01 17:00:17.437392 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-01 17:00:17.585394 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-01 17:00:17.553394 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-01 17:00:17.581394 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-01 17:00:17.613395 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-01 17:00:17.613395 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-01 16:59:56.449086 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-01 17:00:17.637395 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-01 16:59:56.641089 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-01 17:00:17.641395 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-01 17:00:17.665396 windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-01 17:00:17.673395 windmill_api-1.91.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-01 17:00:17.689396 windmill_api-1.91.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-01 17:00:17.701396 windmill_api-1.91.0/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-01 17:00:17.717396 windmill_api-1.91.0/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-01 17:00:17.733396 windmill_api-1.91.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-01 17:00:17.745397 windmill_api-1.91.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-01 17:00:17.757397 windmill_api-1.91.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-01 17:00:17.773397 windmill_api-1.91.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-01 17:00:17.777397 windmill_api-1.91.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-01 17:00:17.805397 windmill_api-1.91.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-01 17:00:17.813398 windmill_api-1.91.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-01 17:00:17.829398 windmill_api-1.91.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-01 17:00:17.869398 windmill_api-1.91.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-01 17:00:17.853398 windmill_api-1.91.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-01 17:00:17.885398 windmill_api-1.91.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-01 17:00:17.897399 windmill_api-1.91.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-01 17:00:17.945399 windmill_api-1.91.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-01 17:00:17.925399 windmill_api-1.91.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-01 17:00:17.985400 windmill_api-1.91.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-01 17:00:17.969400 windmill_api-1.91.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-01 17:00:18.005400 windmill_api-1.91.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-01 17:00:18.017400 windmill_api-1.91.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-01 17:00:18.033401 windmill_api-1.91.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-01 16:59:46.784949 windmill_api-1.91.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-01 17:00:18.029401 windmill_api-1.91.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 windmill_api-1.91.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.91.0/PKG-INFO
```

### Comparing `windmill_api-1.90.0/LICENSE` & `windmill_api-1.91.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/README.md` & `windmill_api-1.91.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/pyproject.toml` & `windmill_api-1.91.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.90.0"
+version = "1.91.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.90.0/windmill_api/api/app/create_app.py` & `windmill_api-1.91.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/delete_app.py` & `windmill_api-1.91.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/execute_component.py` & `windmill_api-1.91.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/exists_app.py` & `windmill_api-1.91.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.91.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.91.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.91.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.91.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.91.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/list_apps.py` & `windmill_api-1.91.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.91.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/app/update_app.py` & `windmill_api-1.91.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.91.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.91.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/capture/create_capture.py` & `windmill_api-1.91.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/capture/get_capture.py` & `windmill_api-1.91.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/capture/update_capture.py` & `windmill_api-1.91.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/favorite/star.py` & `windmill_api-1.91.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/favorite/unstar.py` & `windmill_api-1.91.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.91.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/create_flow.py` & `windmill_api-1.91.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.91.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.91.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.91.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.91.0/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.91.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.91.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/list_flows.py` & `windmill_api-1.91.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.91.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/flow/update_flow.py` & `windmill_api-1.91.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.91.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/create_folder.py` & `windmill_api-1.91.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.91.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/get_folder.py` & `windmill_api-1.91.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.91.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.91.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/list_folders.py` & `windmill_api-1.91.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.91.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/folder/update_folder.py` & `windmill_api-1.91.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.91.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.91.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.91.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.91.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/create_group.py` & `windmill_api-1.91.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/delete_group.py` & `windmill_api-1.91.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/get_group.py` & `windmill_api-1.91.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/list_group_names.py` & `windmill_api-1.91.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/list_groups.py` & `windmill_api-1.91.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.91.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/group/update_group.py` & `windmill_api-1.91.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/input_/create_input.py` & `windmill_api-1.91.0/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/input_/delete_input.py` & `windmill_api-1.91.0/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.91.0/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.91.0/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/input_/update_input.py` & `windmill_api-1.91.0/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.91.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.91.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.91.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.91.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.91.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.91.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.91.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.91.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/get_job.py` & `windmill_api-1.91.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.91.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.91.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.91.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.91.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/list_jobs.py` & `windmill_api-1.91.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/list_queue.py` & `windmill_api-1.91.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/result_by_id.py` & `windmill_api-1.91.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.91.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.91.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.91.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.91.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.91.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.91.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.91.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.91.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.91.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.91.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.91.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/create_account.py` & `windmill_api-1.91.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.91.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.91.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.91.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.91.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.91.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/create_resource.py` & `windmill_api-1.91.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.91.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.91.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.91.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.91.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.91.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/get_resource.py` & `windmill_api-1.91.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.91.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.91.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/list_resource.py` & `windmill_api-1.91.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.91.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.91.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/update_resource.py` & `windmill_api-1.91.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.91.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.91.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.91.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.91.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.91.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.91.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.91.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.91.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.91.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.91.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.91.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.91.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/create_script.py` & `windmill_api-1.91.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.91.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.91.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.91.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.91.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.91.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.91.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.91.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/list_scripts.py` & `windmill_api-1.91.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.91.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.91.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.91.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.91.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/settings/backend_version.py` & `windmill_api-1.91.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.91.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/accept_invite.py` & `windmill_api-1.91.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/create_token.py` & `windmill_api-1.91.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.91.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/create_user.py` & `windmill_api-1.91.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.91.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/decline_invite.py` & `windmill_api-1.91.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/delete_token.py` & `windmill_api-1.91.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/delete_user.py` & `windmill_api-1.91.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/get_current_email.py` & `windmill_api-1.91.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/get_usage.py` & `windmill_api-1.91.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.91.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/global_user_update.py` & `windmill_api-1.91.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/global_whoami.py` & `windmill_api-1.91.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.91.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.91.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/list_tokens.py` & `windmill_api-1.91.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/list_usernames.py` & `windmill_api-1.91.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/list_users.py` & `windmill_api-1.91.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.91.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.91.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/login.py` & `windmill_api-1.91.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.91.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/logout.py` & `windmill_api-1.91.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/set_password.py` & `windmill_api-1.91.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/update_user.py` & `windmill_api-1.91.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/whoami.py` & `windmill_api-1.91.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/user/whois.py` & `windmill_api-1.91.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/create_variable.py` & `windmill_api-1.91.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.91.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.91.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/get_variable.py` & `windmill_api-1.91.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.91.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/list_variable.py` & `windmill_api-1.91.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/variable/update_variable.py` & `windmill_api-1.91.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.91.0/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/worker/list_workers.py` & `windmill_api-1.91.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/add_user.py` & `windmill_api-1.91.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.91.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.91.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.91.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.91.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.91.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.91.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.91.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.91.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.91.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.91.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.91.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.91.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.91.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.91.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.91.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.91.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.91.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.91.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/client.py` & `windmill_api-1.91.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.91.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.91.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.91.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/add_user_json_body.py` & `windmill_api-1.91.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.91.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/app_with_last_version.py` & `windmill_api-1.91.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.91.0/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, ArchiveScriptByHashResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
         tag (Union[Unset, str]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -56,14 +58,16 @@
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, ArchiveScriptByHashResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
     tag: Union[Unset, str] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -89,14 +93,16 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
         tag = self.tag
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -122,14 +128,18 @@
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
         if tag is not UNSET:
             field_dict["tag"] = tag
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -173,14 +183,18 @@
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
         tag = d.pop("tag", UNSET)
 
+        has_draft = d.pop("has_draft", UNSET)
+
+        draft_only = d.pop("draft_only", UNSET)
+
         archive_script_by_hash_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -194,14 +208,16 @@
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
             tag=tag,
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
         archive_script_by_hash_response_200.additional_properties = d
         return archive_script_by_hash_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.91.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/audit_log.py` & `windmill_api-1.91.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/audit_log_operation.py` & `windmill_api-1.91.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.91.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.91.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all.py` & `windmill_api-1.91.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one.py` & `windmill_api-1.91.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.91.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.91.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job.py` & `windmill_api-1.91.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_args.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.91.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.91.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.91.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/contextual_variable.py` & `windmill_api-1.91.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_account_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_app_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_app_json_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,77 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.create_app_json_body_policy import CreateAppJsonBodyPolicy
+from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateAppJsonBody")
 
 
 @attr.s(auto_attribs=True)
 class CreateAppJsonBody:
     """
     Attributes:
         path (str):
         value (Any):
         summary (str):
         policy (CreateAppJsonBodyPolicy):
+        draft_only (Union[Unset, bool]):
     """
 
     path: str
     value: Any
     summary: str
     policy: CreateAppJsonBodyPolicy
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         value = self.value
         summary = self.summary
         policy = self.policy.to_dict()
 
+        draft_only = self.draft_only
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "value": value,
                 "summary": summary,
                 "policy": policy,
             }
         )
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         path = d.pop("path")
 
         value = d.pop("value")
 
         summary = d.pop("summary")
 
         policy = CreateAppJsonBodyPolicy.from_dict(d.pop("policy"))
 
+        draft_only = d.pop("draft_only", UNSET)
+
         create_app_json_body = cls(
             path=path,
             value=value,
             summary=summary,
             policy=policy,
+            draft_only=draft_only,
         )
 
         create_app_json_body.additional_properties = d
         return create_app_json_body
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.91.0/windmill_api/models/open_flow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,83 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_schema import CreateFlowJsonBodySchema
-from ..models.create_flow_json_body_value import CreateFlowJsonBodyValue
+from ..models.open_flow_schema import OpenFlowSchema
+from ..models.open_flow_value import OpenFlowValue
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBody")
+T = TypeVar("T", bound="OpenFlow")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBody:
+class OpenFlow:
     """
     Attributes:
         summary (str):
-        value (CreateFlowJsonBodyValue):
-        path (str):
+        value (OpenFlowValue):
         description (Union[Unset, str]):
-        schema (Union[Unset, CreateFlowJsonBodySchema]):
+        schema (Union[Unset, OpenFlowSchema]):
     """
 
     summary: str
-    value: CreateFlowJsonBodyValue
-    path: str
+    value: OpenFlowValue
     description: Union[Unset, str] = UNSET
-    schema: Union[Unset, CreateFlowJsonBodySchema] = UNSET
+    schema: Union[Unset, OpenFlowSchema] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         summary = self.summary
         value = self.value.to_dict()
 
-        path = self.path
         description = self.description
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "summary": summary,
                 "value": value,
-                "path": path,
             }
         )
         if description is not UNSET:
             field_dict["description"] = description
         if schema is not UNSET:
             field_dict["schema"] = schema
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         summary = d.pop("summary")
 
-        value = CreateFlowJsonBodyValue.from_dict(d.pop("value"))
-
-        path = d.pop("path")
+        value = OpenFlowValue.from_dict(d.pop("value"))
 
         description = d.pop("description", UNSET)
 
         _schema = d.pop("schema", UNSET)
-        schema: Union[Unset, CreateFlowJsonBodySchema]
+        schema: Union[Unset, OpenFlowSchema]
         if isinstance(_schema, Unset):
             schema = UNSET
         else:
-            schema = CreateFlowJsonBodySchema.from_dict(_schema)
+            schema = OpenFlowSchema.from_dict(_schema)
 
-        create_flow_json_body = cls(
+        open_flow = cls(
             summary=summary,
             value=value,
-            path=path,
             description=description,
             schema=schema,
         )
 
-        create_flow_json_body.additional_properties = d
-        return create_flow_json_body
+        open_flow.additional_properties = d
+        return open_flow
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_schema.py` & `windmill_api-1.91.0/windmill_api/models/script_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateFlowJsonBodySchema")
+T = TypeVar("T", bound="ScriptSchema")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodySchema:
+class ScriptSchema:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
@@ -18,18 +18,18 @@
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        create_flow_json_body_schema = cls()
+        script_schema = cls()
 
-        create_flow_json_body_schema.additional_properties = d
-        return create_flow_json_body_schema
+        script_schema.additional_properties = d
+        return script_schema
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_failure_module import CreateFlowJsonBodyValueFailureModule
-from ..models.create_flow_json_body_value_modules_item import CreateFlowJsonBodyValueModulesItem
+from ..models.update_flow_json_body_value_failure_module import UpdateFlowJsonBodyValueFailureModule
+from ..models.update_flow_json_body_value_modules_item import UpdateFlowJsonBodyValueModulesItem
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValue")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValue")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValue:
+class UpdateFlowJsonBodyValue:
     """
     Attributes:
-        modules (List[CreateFlowJsonBodyValueModulesItem]):
-        failure_module (Union[Unset, CreateFlowJsonBodyValueFailureModule]):
+        modules (List[UpdateFlowJsonBodyValueModulesItem]):
+        failure_module (Union[Unset, UpdateFlowJsonBodyValueFailureModule]):
         same_worker (Union[Unset, bool]):
     """
 
-    modules: List[CreateFlowJsonBodyValueModulesItem]
-    failure_module: Union[Unset, CreateFlowJsonBodyValueFailureModule] = UNSET
+    modules: List[UpdateFlowJsonBodyValueModulesItem]
+    failure_module: Union[Unset, UpdateFlowJsonBodyValueFailureModule] = UNSET
     same_worker: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         modules = []
         for modules_item_data in self.modules:
             modules_item = modules_item_data.to_dict()
@@ -52,35 +52,35 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         modules = []
         _modules = d.pop("modules")
         for modules_item_data in _modules:
-            modules_item = CreateFlowJsonBodyValueModulesItem.from_dict(modules_item_data)
+            modules_item = UpdateFlowJsonBodyValueModulesItem.from_dict(modules_item_data)
 
             modules.append(modules_item)
 
         _failure_module = d.pop("failure_module", UNSET)
-        failure_module: Union[Unset, CreateFlowJsonBodyValueFailureModule]
+        failure_module: Union[Unset, UpdateFlowJsonBodyValueFailureModule]
         if isinstance(_failure_module, Unset):
             failure_module = UNSET
         else:
-            failure_module = CreateFlowJsonBodyValueFailureModule.from_dict(_failure_module)
+            failure_module = UpdateFlowJsonBodyValueFailureModule.from_dict(_failure_module)
 
         same_worker = d.pop("same_worker", UNSET)
 
-        create_flow_json_body_value = cls(
+        update_flow_json_body_value = cls(
             modules=modules,
             failure_module=failure_module,
             same_worker=same_worker,
         )
 
-        create_flow_json_body_value.additional_properties = d
-        return create_flow_json_body_value
+        update_flow_json_body_value.additional_properties = d
+        return update_flow_json_body_value
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_failure_module_retry import CreateFlowJsonBodyValueFailureModuleRetry
-from ..models.create_flow_json_body_value_failure_module_sleep_type_0 import (
-    CreateFlowJsonBodyValueFailureModuleSleepType0,
+from ..models.run_flow_preview_json_body_value_failure_module_retry import RunFlowPreviewJsonBodyValueFailureModuleRetry
+from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_0 import (
+    RunFlowPreviewJsonBodyValueFailureModuleSleepType0,
 )
-from ..models.create_flow_json_body_value_failure_module_sleep_type_1 import (
-    CreateFlowJsonBodyValueFailureModuleSleepType1,
+from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_1 import (
+    RunFlowPreviewJsonBodyValueFailureModuleSleepType1,
 )
-from ..models.create_flow_json_body_value_failure_module_stop_after_if import (
-    CreateFlowJsonBodyValueFailureModuleStopAfterIf,
+from ..models.run_flow_preview_json_body_value_failure_module_stop_after_if import (
+    RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf,
+)
+from ..models.run_flow_preview_json_body_value_failure_module_suspend import (
+    RunFlowPreviewJsonBodyValueFailureModuleSuspend,
 )
-from ..models.create_flow_json_body_value_failure_module_suspend import CreateFlowJsonBodyValueFailureModuleSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModule")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModule")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModule:
+class RunFlowPreviewJsonBodyValueFailureModule:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, CreateFlowJsonBodyValueFailureModuleStopAfterIf]):
-        sleep (Union[CreateFlowJsonBodyValueFailureModuleSleepType0, CreateFlowJsonBodyValueFailureModuleSleepType1,
-            Unset]):
+        stop_after_if (Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf]):
+        sleep (Union[RunFlowPreviewJsonBodyValueFailureModuleSleepType0,
+            RunFlowPreviewJsonBodyValueFailureModuleSleepType1, Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, CreateFlowJsonBodyValueFailureModuleSuspend]):
-        retry (Union[Unset, CreateFlowJsonBodyValueFailureModuleRetry]):
+        suspend (Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSuspend]):
+        retry (Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, CreateFlowJsonBodyValueFailureModuleStopAfterIf] = UNSET
+    stop_after_if: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf] = UNSET
     sleep: Union[
-        CreateFlowJsonBodyValueFailureModuleSleepType0, CreateFlowJsonBodyValueFailureModuleSleepType1, Unset
+        RunFlowPreviewJsonBodyValueFailureModuleSleepType0, RunFlowPreviewJsonBodyValueFailureModuleSleepType1, Unset
     ] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, CreateFlowJsonBodyValueFailureModuleSuspend] = UNSET
-    retry: Union[Unset, CreateFlowJsonBodyValueFailureModuleRetry] = UNSET
+    suspend: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSuspend] = UNSET
+    retry: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, CreateFlowJsonBodyValueFailureModuleSleepType0):
+        elif isinstance(self.sleep, RunFlowPreviewJsonBodyValueFailureModuleSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -98,81 +100,83 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, CreateFlowJsonBodyValueFailureModuleStopAfterIf]
+        stop_after_if: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = CreateFlowJsonBodyValueFailureModuleStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
         ) -> Union[
-            CreateFlowJsonBodyValueFailureModuleSleepType0, CreateFlowJsonBodyValueFailureModuleSleepType1, Unset
+            RunFlowPreviewJsonBodyValueFailureModuleSleepType0,
+            RunFlowPreviewJsonBodyValueFailureModuleSleepType1,
+            Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, CreateFlowJsonBodyValueFailureModuleSleepType0]
+                sleep_type_0: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = CreateFlowJsonBodyValueFailureModuleSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = RunFlowPreviewJsonBodyValueFailureModuleSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, CreateFlowJsonBodyValueFailureModuleSleepType1]
+            sleep_type_1: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = CreateFlowJsonBodyValueFailureModuleSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = RunFlowPreviewJsonBodyValueFailureModuleSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, CreateFlowJsonBodyValueFailureModuleSuspend]
+        suspend: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = CreateFlowJsonBodyValueFailureModuleSuspend.from_dict(_suspend)
+            suspend = RunFlowPreviewJsonBodyValueFailureModuleSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, CreateFlowJsonBodyValueFailureModuleRetry]
+        retry: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = CreateFlowJsonBodyValueFailureModuleRetry.from_dict(_retry)
+            retry = RunFlowPreviewJsonBodyValueFailureModuleRetry.from_dict(_retry)
 
-        create_flow_json_body_value_failure_module = cls(
+        run_flow_preview_json_body_value_failure_module = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        create_flow_json_body_value_failure_module.additional_properties = d
-        return create_flow_json_body_value_failure_module
+        run_flow_preview_json_body_value_failure_module.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_failure_module_retry_constant import (
-    CreateFlowJsonBodyValueFailureModuleRetryConstant,
+from ..models.update_flow_json_body_value_failure_module_retry_constant import (
+    UpdateFlowJsonBodyValueFailureModuleRetryConstant,
 )
-from ..models.create_flow_json_body_value_failure_module_retry_exponential import (
-    CreateFlowJsonBodyValueFailureModuleRetryExponential,
+from ..models.update_flow_json_body_value_failure_module_retry_exponential import (
+    UpdateFlowJsonBodyValueFailureModuleRetryExponential,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleRetry")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleRetry")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleRetry:
+class UpdateFlowJsonBodyValueFailureModuleRetry:
     """
     Attributes:
-        constant (Union[Unset, CreateFlowJsonBodyValueFailureModuleRetryConstant]):
-        exponential (Union[Unset, CreateFlowJsonBodyValueFailureModuleRetryExponential]):
+        constant (Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryConstant]):
+        exponential (Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryExponential]):
     """
 
-    constant: Union[Unset, CreateFlowJsonBodyValueFailureModuleRetryConstant] = UNSET
-    exponential: Union[Unset, CreateFlowJsonBodyValueFailureModuleRetryExponential] = UNSET
+    constant: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryConstant] = UNSET
+    exponential: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryExponential] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         constant: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.constant, Unset):
             constant = self.constant.to_dict()
 
@@ -44,34 +44,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, CreateFlowJsonBodyValueFailureModuleRetryConstant]
+        constant: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryConstant]
         if isinstance(_constant, Unset):
             constant = UNSET
         else:
-            constant = CreateFlowJsonBodyValueFailureModuleRetryConstant.from_dict(_constant)
+            constant = UpdateFlowJsonBodyValueFailureModuleRetryConstant.from_dict(_constant)
 
         _exponential = d.pop("exponential", UNSET)
-        exponential: Union[Unset, CreateFlowJsonBodyValueFailureModuleRetryExponential]
+        exponential: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryExponential]
         if isinstance(_exponential, Unset):
             exponential = UNSET
         else:
-            exponential = CreateFlowJsonBodyValueFailureModuleRetryExponential.from_dict(_exponential)
+            exponential = UpdateFlowJsonBodyValueFailureModuleRetryExponential.from_dict(_exponential)
 
-        create_flow_json_body_value_failure_module_retry = cls(
+        update_flow_json_body_value_failure_module_retry = cls(
             constant=constant,
             exponential=exponential,
         )
 
-        create_flow_json_body_value_failure_module_retry.additional_properties = d
-        return create_flow_json_body_value_failure_module_retry
+        update_flow_json_body_value_failure_module_retry.additional_properties = d
+        return update_flow_json_body_value_failure_module_retry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleRetryConstant")
+T = TypeVar("T", bound="OpenFlowValueFailureModuleRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleRetryConstant:
+class OpenFlowValueFailureModuleRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        create_flow_json_body_value_failure_module_retry_constant = cls(
+        open_flow_value_failure_module_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        create_flow_json_body_value_failure_module_retry_constant.additional_properties = d
-        return create_flow_json_body_value_failure_module_retry_constant
+        open_flow_value_failure_module_retry_constant.additional_properties = d
+        return open_flow_value_failure_module_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleRetryExponential")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleRetryExponential:
+class UpdateFlowJsonBodyValueFailureModuleRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        create_flow_json_body_value_failure_module_retry_exponential = cls(
+        update_flow_json_body_value_failure_module_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        create_flow_json_body_value_failure_module_retry_exponential.additional_properties = d
-        return create_flow_json_body_value_failure_module_retry_exponential
+        update_flow_json_body_value_failure_module_retry_exponential.additional_properties = d
+        return update_flow_json_body_value_failure_module_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_failure_module_sleep_type_0_type import (
-    CreateFlowJsonBodyValueFailureModuleSleepType0Type,
+from ..models.update_flow_json_body_value_failure_module_sleep_type_0_type import (
+    UpdateFlowJsonBodyValueFailureModuleSleepType0Type,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleSleepType0")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleSleepType0:
+class UpdateFlowJsonBodyValueFailureModuleSleepType0:
     """
     Attributes:
-        type (CreateFlowJsonBodyValueFailureModuleSleepType0Type):
+        type (UpdateFlowJsonBodyValueFailureModuleSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: CreateFlowJsonBodyValueFailureModuleSleepType0Type
+    type: UpdateFlowJsonBodyValueFailureModuleSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = CreateFlowJsonBodyValueFailureModuleSleepType0Type(d.pop("type"))
+        type = UpdateFlowJsonBodyValueFailureModuleSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        create_flow_json_body_value_failure_module_sleep_type_0 = cls(
+        update_flow_json_body_value_failure_module_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        create_flow_json_body_value_failure_module_sleep_type_0.additional_properties = d
-        return create_flow_json_body_value_failure_module_sleep_type_0
+        update_flow_json_body_value_failure_module_sleep_type_0.additional_properties = d
+        return update_flow_json_body_value_failure_module_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.create_flow_json_body_value_failure_module_sleep_type_1_type import (
-    CreateFlowJsonBodyValueFailureModuleSleepType1Type,
+from ..models.update_flow_json_body_value_failure_module_sleep_type_1_type import (
+    UpdateFlowJsonBodyValueFailureModuleSleepType1Type,
 )
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleSleepType1")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleSleepType1:
+class UpdateFlowJsonBodyValueFailureModuleSleepType1:
     """
     Attributes:
         expr (str):
-        type (CreateFlowJsonBodyValueFailureModuleSleepType1Type):
+        type (UpdateFlowJsonBodyValueFailureModuleSleepType1Type):
     """
 
     expr: str
-    type: CreateFlowJsonBodyValueFailureModuleSleepType1Type
+    type: UpdateFlowJsonBodyValueFailureModuleSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = CreateFlowJsonBodyValueFailureModuleSleepType1Type(d.pop("type"))
+        type = UpdateFlowJsonBodyValueFailureModuleSleepType1Type(d.pop("type"))
 
-        create_flow_json_body_value_failure_module_sleep_type_1 = cls(
+        update_flow_json_body_value_failure_module_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        create_flow_json_body_value_failure_module_sleep_type_1.additional_properties = d
-        return create_flow_json_body_value_failure_module_sleep_type_1
+        update_flow_json_body_value_failure_module_sleep_type_1.additional_properties = d
+        return update_flow_json_body_value_failure_module_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleStopAfterIf")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleStopAfterIf:
+class UpdateFlowJsonBodyValueFailureModuleStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        create_flow_json_body_value_failure_module_stop_after_if = cls(
+        update_flow_json_body_value_failure_module_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        create_flow_json_body_value_failure_module_stop_after_if.additional_properties = d
-        return create_flow_json_body_value_failure_module_stop_after_if
+        update_flow_json_body_value_failure_module_stop_after_if.additional_properties = d
+        return update_flow_json_body_value_failure_module_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueFailureModuleSuspend")
+T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleSuspend")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueFailureModuleSuspend:
+class OpenFlowWPathValueFailureModuleSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        create_flow_json_body_value_failure_module_suspend = cls(
+        open_flow_w_path_value_failure_module_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        create_flow_json_body_value_failure_module_suspend.additional_properties = d
-        return create_flow_json_body_value_failure_module_suspend
+        open_flow_w_path_value_failure_module_suspend.additional_properties = d
+        return open_flow_w_path_value_failure_module_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_modules_item_retry import CreateFlowJsonBodyValueModulesItemRetry
-from ..models.create_flow_json_body_value_modules_item_sleep_type_0 import CreateFlowJsonBodyValueModulesItemSleepType0
-from ..models.create_flow_json_body_value_modules_item_sleep_type_1 import CreateFlowJsonBodyValueModulesItemSleepType1
-from ..models.create_flow_json_body_value_modules_item_stop_after_if import (
-    CreateFlowJsonBodyValueModulesItemStopAfterIf,
+from ..models.run_flow_preview_json_body_value_modules_item_retry import RunFlowPreviewJsonBodyValueModulesItemRetry
+from ..models.run_flow_preview_json_body_value_modules_item_sleep_type_0 import (
+    RunFlowPreviewJsonBodyValueModulesItemSleepType0,
 )
-from ..models.create_flow_json_body_value_modules_item_suspend import CreateFlowJsonBodyValueModulesItemSuspend
+from ..models.run_flow_preview_json_body_value_modules_item_sleep_type_1 import (
+    RunFlowPreviewJsonBodyValueModulesItemSleepType1,
+)
+from ..models.run_flow_preview_json_body_value_modules_item_stop_after_if import (
+    RunFlowPreviewJsonBodyValueModulesItemStopAfterIf,
+)
+from ..models.run_flow_preview_json_body_value_modules_item_suspend import RunFlowPreviewJsonBodyValueModulesItemSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItem")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItem")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItem:
+class RunFlowPreviewJsonBodyValueModulesItem:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, CreateFlowJsonBodyValueModulesItemStopAfterIf]):
-        sleep (Union[CreateFlowJsonBodyValueModulesItemSleepType0, CreateFlowJsonBodyValueModulesItemSleepType1,
+        stop_after_if (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemStopAfterIf]):
+        sleep (Union[RunFlowPreviewJsonBodyValueModulesItemSleepType0, RunFlowPreviewJsonBodyValueModulesItemSleepType1,
             Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, CreateFlowJsonBodyValueModulesItemSuspend]):
-        retry (Union[Unset, CreateFlowJsonBodyValueModulesItemRetry]):
+        suspend (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemSuspend]):
+        retry (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, CreateFlowJsonBodyValueModulesItemStopAfterIf] = UNSET
+    stop_after_if: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemStopAfterIf] = UNSET
     sleep: Union[
-        CreateFlowJsonBodyValueModulesItemSleepType0, CreateFlowJsonBodyValueModulesItemSleepType1, Unset
+        RunFlowPreviewJsonBodyValueModulesItemSleepType0, RunFlowPreviewJsonBodyValueModulesItemSleepType1, Unset
     ] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, CreateFlowJsonBodyValueModulesItemSuspend] = UNSET
-    retry: Union[Unset, CreateFlowJsonBodyValueModulesItemRetry] = UNSET
+    suspend: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemSuspend] = UNSET
+    retry: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, CreateFlowJsonBodyValueModulesItemSleepType0):
+        elif isinstance(self.sleep, RunFlowPreviewJsonBodyValueModulesItemSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -94,79 +98,81 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, CreateFlowJsonBodyValueModulesItemStopAfterIf]
+        stop_after_if: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = CreateFlowJsonBodyValueModulesItemStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = RunFlowPreviewJsonBodyValueModulesItemStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
-        ) -> Union[CreateFlowJsonBodyValueModulesItemSleepType0, CreateFlowJsonBodyValueModulesItemSleepType1, Unset]:
+        ) -> Union[
+            RunFlowPreviewJsonBodyValueModulesItemSleepType0, RunFlowPreviewJsonBodyValueModulesItemSleepType1, Unset
+        ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, CreateFlowJsonBodyValueModulesItemSleepType0]
+                sleep_type_0: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = CreateFlowJsonBodyValueModulesItemSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = RunFlowPreviewJsonBodyValueModulesItemSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, CreateFlowJsonBodyValueModulesItemSleepType1]
+            sleep_type_1: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = CreateFlowJsonBodyValueModulesItemSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = RunFlowPreviewJsonBodyValueModulesItemSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, CreateFlowJsonBodyValueModulesItemSuspend]
+        suspend: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = CreateFlowJsonBodyValueModulesItemSuspend.from_dict(_suspend)
+            suspend = RunFlowPreviewJsonBodyValueModulesItemSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, CreateFlowJsonBodyValueModulesItemRetry]
+        retry: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = CreateFlowJsonBodyValueModulesItemRetry.from_dict(_retry)
+            retry = RunFlowPreviewJsonBodyValueModulesItemRetry.from_dict(_retry)
 
-        create_flow_json_body_value_modules_item = cls(
+        run_flow_preview_json_body_value_modules_item = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        create_flow_json_body_value_modules_item.additional_properties = d
-        return create_flow_json_body_value_modules_item
+        run_flow_preview_json_body_value_modules_item.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_modules_item_retry_constant import (
-    CreateFlowJsonBodyValueModulesItemRetryConstant,
+from ..models.run_flow_preview_json_body_value_modules_item_retry_constant import (
+    RunFlowPreviewJsonBodyValueModulesItemRetryConstant,
 )
-from ..models.create_flow_json_body_value_modules_item_retry_exponential import (
-    CreateFlowJsonBodyValueModulesItemRetryExponential,
+from ..models.run_flow_preview_json_body_value_modules_item_retry_exponential import (
+    RunFlowPreviewJsonBodyValueModulesItemRetryExponential,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemRetry")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemRetry")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemRetry:
+class RunFlowPreviewJsonBodyValueModulesItemRetry:
     """
     Attributes:
-        constant (Union[Unset, CreateFlowJsonBodyValueModulesItemRetryConstant]):
-        exponential (Union[Unset, CreateFlowJsonBodyValueModulesItemRetryExponential]):
+        constant (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryConstant]):
+        exponential (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryExponential]):
     """
 
-    constant: Union[Unset, CreateFlowJsonBodyValueModulesItemRetryConstant] = UNSET
-    exponential: Union[Unset, CreateFlowJsonBodyValueModulesItemRetryExponential] = UNSET
+    constant: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryConstant] = UNSET
+    exponential: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryExponential] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         constant: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.constant, Unset):
             constant = self.constant.to_dict()
 
@@ -44,34 +44,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, CreateFlowJsonBodyValueModulesItemRetryConstant]
+        constant: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryConstant]
         if isinstance(_constant, Unset):
             constant = UNSET
         else:
-            constant = CreateFlowJsonBodyValueModulesItemRetryConstant.from_dict(_constant)
+            constant = RunFlowPreviewJsonBodyValueModulesItemRetryConstant.from_dict(_constant)
 
         _exponential = d.pop("exponential", UNSET)
-        exponential: Union[Unset, CreateFlowJsonBodyValueModulesItemRetryExponential]
+        exponential: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryExponential]
         if isinstance(_exponential, Unset):
             exponential = UNSET
         else:
-            exponential = CreateFlowJsonBodyValueModulesItemRetryExponential.from_dict(_exponential)
+            exponential = RunFlowPreviewJsonBodyValueModulesItemRetryExponential.from_dict(_exponential)
 
-        create_flow_json_body_value_modules_item_retry = cls(
+        run_flow_preview_json_body_value_modules_item_retry = cls(
             constant=constant,
             exponential=exponential,
         )
 
-        create_flow_json_body_value_modules_item_retry.additional_properties = d
-        return create_flow_json_body_value_modules_item_retry
+        run_flow_preview_json_body_value_modules_item_retry.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_retry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemRetryConstant")
+T = TypeVar("T", bound="FlowPreviewValueModulesItemRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemRetryConstant:
+class FlowPreviewValueModulesItemRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        create_flow_json_body_value_modules_item_retry_constant = cls(
+        flow_preview_value_modules_item_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        create_flow_json_body_value_modules_item_retry_constant.additional_properties = d
-        return create_flow_json_body_value_modules_item_retry_constant
+        flow_preview_value_modules_item_retry_constant.additional_properties = d
+        return flow_preview_value_modules_item_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemRetryExponential")
+T = TypeVar("T", bound="OpenFlowValueModulesItemRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemRetryExponential:
+class OpenFlowValueModulesItemRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        create_flow_json_body_value_modules_item_retry_exponential = cls(
+        open_flow_value_modules_item_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        create_flow_json_body_value_modules_item_retry_exponential.additional_properties = d
-        return create_flow_json_body_value_modules_item_retry_exponential
+        open_flow_value_modules_item_retry_exponential.additional_properties = d
+        return open_flow_value_modules_item_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_flow_json_body_value_modules_item_sleep_type_0_type import (
-    CreateFlowJsonBodyValueModulesItemSleepType0Type,
+from ..models.run_flow_preview_json_body_value_modules_item_sleep_type_0_type import (
+    RunFlowPreviewJsonBodyValueModulesItemSleepType0Type,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemSleepType0")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemSleepType0:
+class RunFlowPreviewJsonBodyValueModulesItemSleepType0:
     """
     Attributes:
-        type (CreateFlowJsonBodyValueModulesItemSleepType0Type):
+        type (RunFlowPreviewJsonBodyValueModulesItemSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: CreateFlowJsonBodyValueModulesItemSleepType0Type
+    type: RunFlowPreviewJsonBodyValueModulesItemSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = CreateFlowJsonBodyValueModulesItemSleepType0Type(d.pop("type"))
+        type = RunFlowPreviewJsonBodyValueModulesItemSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        create_flow_json_body_value_modules_item_sleep_type_0 = cls(
+        run_flow_preview_json_body_value_modules_item_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        create_flow_json_body_value_modules_item_sleep_type_0.additional_properties = d
-        return create_flow_json_body_value_modules_item_sleep_type_0
+        run_flow_preview_json_body_value_modules_item_sleep_type_0.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.create_flow_json_body_value_modules_item_sleep_type_1_type import (
-    CreateFlowJsonBodyValueModulesItemSleepType1Type,
+from ..models.run_flow_preview_json_body_value_modules_item_sleep_type_1_type import (
+    RunFlowPreviewJsonBodyValueModulesItemSleepType1Type,
 )
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemSleepType1")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemSleepType1:
+class RunFlowPreviewJsonBodyValueModulesItemSleepType1:
     """
     Attributes:
         expr (str):
-        type (CreateFlowJsonBodyValueModulesItemSleepType1Type):
+        type (RunFlowPreviewJsonBodyValueModulesItemSleepType1Type):
     """
 
     expr: str
-    type: CreateFlowJsonBodyValueModulesItemSleepType1Type
+    type: RunFlowPreviewJsonBodyValueModulesItemSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = CreateFlowJsonBodyValueModulesItemSleepType1Type(d.pop("type"))
+        type = RunFlowPreviewJsonBodyValueModulesItemSleepType1Type(d.pop("type"))
 
-        create_flow_json_body_value_modules_item_sleep_type_1 = cls(
+        run_flow_preview_json_body_value_modules_item_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        create_flow_json_body_value_modules_item_sleep_type_1.additional_properties = d
-        return create_flow_json_body_value_modules_item_sleep_type_1
+        run_flow_preview_json_body_value_modules_item_sleep_type_1.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemStopAfterIf")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemStopAfterIf:
+class UpdateFlowJsonBodyValueModulesItemStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        create_flow_json_body_value_modules_item_stop_after_if = cls(
+        update_flow_json_body_value_modules_item_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        create_flow_json_body_value_modules_item_stop_after_if.additional_properties = d
-        return create_flow_json_body_value_modules_item_stop_after_if
+        update_flow_json_body_value_modules_item_stop_after_if.additional_properties = d
+        return update_flow_json_body_value_modules_item_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFlowJsonBodyValueModulesItemSuspend")
+T = TypeVar("T", bound="OpenFlowWPathValueModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class CreateFlowJsonBodyValueModulesItemSuspend:
+class OpenFlowWPathValueModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        create_flow_json_body_value_modules_item_suspend = cls(
+        open_flow_w_path_value_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        create_flow_json_body_value_modules_item_suspend.additional_properties = d
-        return create_flow_json_body_value_modules_item_suspend
+        open_flow_w_path_value_modules_item_suspend.additional_properties = d
+        return open_flow_w_path_value_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_group_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_input.py` & `windmill_api-1.91.0/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_input_args.py` & `windmill_api-1.91.0/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_input_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.91.0/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_resource.py` & `windmill_api-1.91.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.91.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_script_json_body.py` & `windmill_api-1.91.0/windmill_api/models/listable_variable.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,149 +1,137 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.create_script_json_body_kind import CreateScriptJsonBodyKind
-from ..models.create_script_json_body_language import CreateScriptJsonBodyLanguage
-from ..models.create_script_json_body_schema import CreateScriptJsonBodySchema
+from ..models.listable_variable_extra_perms import ListableVariableExtraPerms
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateScriptJsonBody")
+T = TypeVar("T", bound="ListableVariable")
 
 
 @attr.s(auto_attribs=True)
-class CreateScriptJsonBody:
+class ListableVariable:
     """
     Attributes:
+        workspace_id (str):
         path (str):
-        summary (str):
-        description (str):
-        content (str):
-        language (CreateScriptJsonBodyLanguage):
-        parent_hash (Union[Unset, str]):
-        schema (Union[Unset, CreateScriptJsonBodySchema]):
-        is_template (Union[Unset, bool]):
-        lock (Union[Unset, List[str]]):
-        kind (Union[Unset, CreateScriptJsonBodyKind]):
-        tag (Union[Unset, str]):
+        is_secret (bool):
+        extra_perms (ListableVariableExtraPerms):
+        value (Union[Unset, str]):
+        description (Union[Unset, str]):
+        account (Union[Unset, int]):
+        is_oauth (Union[Unset, bool]):
+        is_expired (Union[Unset, bool]):
+        refresh_error (Union[Unset, str]):
+        is_linked (Union[Unset, bool]):
+        is_refreshed (Union[Unset, bool]):
     """
 
+    workspace_id: str
     path: str
-    summary: str
-    description: str
-    content: str
-    language: CreateScriptJsonBodyLanguage
-    parent_hash: Union[Unset, str] = UNSET
-    schema: Union[Unset, CreateScriptJsonBodySchema] = UNSET
-    is_template: Union[Unset, bool] = UNSET
-    lock: Union[Unset, List[str]] = UNSET
-    kind: Union[Unset, CreateScriptJsonBodyKind] = UNSET
-    tag: Union[Unset, str] = UNSET
+    is_secret: bool
+    extra_perms: ListableVariableExtraPerms
+    value: Union[Unset, str] = UNSET
+    description: Union[Unset, str] = UNSET
+    account: Union[Unset, int] = UNSET
+    is_oauth: Union[Unset, bool] = UNSET
+    is_expired: Union[Unset, bool] = UNSET
+    refresh_error: Union[Unset, str] = UNSET
+    is_linked: Union[Unset, bool] = UNSET
+    is_refreshed: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        workspace_id = self.workspace_id
         path = self.path
-        summary = self.summary
-        description = self.description
-        content = self.content
-        language = self.language.value
-
-        parent_hash = self.parent_hash
-        schema: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.schema, Unset):
-            schema = self.schema.to_dict()
-
-        is_template = self.is_template
-        lock: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.lock, Unset):
-            lock = self.lock
-
-        kind: Union[Unset, str] = UNSET
-        if not isinstance(self.kind, Unset):
-            kind = self.kind.value
+        is_secret = self.is_secret
+        extra_perms = self.extra_perms.to_dict()
 
-        tag = self.tag
+        value = self.value
+        description = self.description
+        account = self.account
+        is_oauth = self.is_oauth
+        is_expired = self.is_expired
+        refresh_error = self.refresh_error
+        is_linked = self.is_linked
+        is_refreshed = self.is_refreshed
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "workspace_id": workspace_id,
                 "path": path,
-                "summary": summary,
-                "description": description,
-                "content": content,
-                "language": language,
+                "is_secret": is_secret,
+                "extra_perms": extra_perms,
             }
         )
-        if parent_hash is not UNSET:
-            field_dict["parent_hash"] = parent_hash
-        if schema is not UNSET:
-            field_dict["schema"] = schema
-        if is_template is not UNSET:
-            field_dict["is_template"] = is_template
-        if lock is not UNSET:
-            field_dict["lock"] = lock
-        if kind is not UNSET:
-            field_dict["kind"] = kind
-        if tag is not UNSET:
-            field_dict["tag"] = tag
+        if value is not UNSET:
+            field_dict["value"] = value
+        if description is not UNSET:
+            field_dict["description"] = description
+        if account is not UNSET:
+            field_dict["account"] = account
+        if is_oauth is not UNSET:
+            field_dict["is_oauth"] = is_oauth
+        if is_expired is not UNSET:
+            field_dict["is_expired"] = is_expired
+        if refresh_error is not UNSET:
+            field_dict["refresh_error"] = refresh_error
+        if is_linked is not UNSET:
+            field_dict["is_linked"] = is_linked
+        if is_refreshed is not UNSET:
+            field_dict["is_refreshed"] = is_refreshed
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        workspace_id = d.pop("workspace_id")
+
         path = d.pop("path")
 
-        summary = d.pop("summary")
+        is_secret = d.pop("is_secret")
 
-        description = d.pop("description")
+        extra_perms = ListableVariableExtraPerms.from_dict(d.pop("extra_perms"))
 
-        content = d.pop("content")
+        value = d.pop("value", UNSET)
 
-        language = CreateScriptJsonBodyLanguage(d.pop("language"))
+        description = d.pop("description", UNSET)
 
-        parent_hash = d.pop("parent_hash", UNSET)
+        account = d.pop("account", UNSET)
 
-        _schema = d.pop("schema", UNSET)
-        schema: Union[Unset, CreateScriptJsonBodySchema]
-        if isinstance(_schema, Unset):
-            schema = UNSET
-        else:
-            schema = CreateScriptJsonBodySchema.from_dict(_schema)
+        is_oauth = d.pop("is_oauth", UNSET)
 
-        is_template = d.pop("is_template", UNSET)
+        is_expired = d.pop("is_expired", UNSET)
 
-        lock = cast(List[str], d.pop("lock", UNSET))
+        refresh_error = d.pop("refresh_error", UNSET)
 
-        _kind = d.pop("kind", UNSET)
-        kind: Union[Unset, CreateScriptJsonBodyKind]
-        if isinstance(_kind, Unset):
-            kind = UNSET
-        else:
-            kind = CreateScriptJsonBodyKind(_kind)
+        is_linked = d.pop("is_linked", UNSET)
 
-        tag = d.pop("tag", UNSET)
+        is_refreshed = d.pop("is_refreshed", UNSET)
 
-        create_script_json_body = cls(
+        listable_variable = cls(
+            workspace_id=workspace_id,
             path=path,
-            summary=summary,
+            is_secret=is_secret,
+            extra_perms=extra_perms,
+            value=value,
             description=description,
-            content=content,
-            language=language,
-            parent_hash=parent_hash,
-            schema=schema,
-            is_template=is_template,
-            lock=lock,
-            kind=kind,
-            tag=tag,
+            account=account,
+            is_oauth=is_oauth,
+            is_expired=is_expired,
+            refresh_error=refresh_error,
+            is_linked=is_linked,
+            is_refreshed=is_refreshed,
         )
 
-        create_script_json_body.additional_properties = d
-        return create_script_json_body
+        listable_variable.additional_properties = d
+        return listable_variable
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.91.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_token_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_user_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_variable.py` & `windmill_api-1.91.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_workspace.py` & `windmill_api-1.91.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.91.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.91.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.91.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, DeleteScriptByHashResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
         tag (Union[Unset, str]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -56,14 +58,16 @@
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, DeleteScriptByHashResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
     tag: Union[Unset, str] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -89,14 +93,16 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
         tag = self.tag
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -122,14 +128,18 @@
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
         if tag is not UNSET:
             field_dict["tag"] = tag
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -173,14 +183,18 @@
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
         tag = d.pop("tag", UNSET)
 
+        has_draft = d.pop("has_draft", UNSET)
+
+        draft_only = d.pop("draft_only", UNSET)
+
         delete_script_by_hash_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -194,14 +208,16 @@
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
             tag=tag,
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
         delete_script_by_hash_response_200.additional_properties = d
         return delete_script_by_hash_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.91.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.91.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.91.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_resource.py` & `windmill_api-1.91.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_resource_type.py` & `windmill_api-1.91.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_schedule.py` & `windmill_api-1.91.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.91.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.91.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_variable.py` & `windmill_api-1.91.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.91.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.91.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.91.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.91.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.91.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.91.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.91.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow.py` & `windmill_api-1.91.0/windmill_api/models/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,28 +24,30 @@
         archived (bool):
         extra_perms (FlowExtraPerms):
         description (Union[Unset, str]):
         schema (Union[Unset, FlowSchema]):
         workspace_id (Union[Unset, str]):
         additional_properties (Union[Unset, bool]):
         starred (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     summary: str
     value: FlowValue
     path: str
     edited_by: str
     edited_at: datetime.datetime
     archived: bool
     extra_perms: FlowExtraPerms
     description: Union[Unset, str] = UNSET
     schema: Union[Unset, FlowSchema] = UNSET
     workspace_id: Union[Unset, str] = UNSET
     additional_properties: Union[Unset, bool] = UNSET
     starred: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         summary = self.summary
         value = self.value.to_dict()
 
         path = self.path
@@ -59,14 +61,15 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         workspace_id = self.workspace_id
         additional_properties = self.additional_properties
         starred = self.starred
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "summary": summary,
                 "value": value,
@@ -83,14 +86,16 @@
             field_dict["schema"] = schema
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if additional_properties is not UNSET:
             field_dict["additionalProperties"] = additional_properties
         if starred is not UNSET:
             field_dict["starred"] = starred
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         summary = d.pop("summary")
@@ -118,27 +123,30 @@
 
         workspace_id = d.pop("workspace_id", UNSET)
 
         additional_properties = d.pop("additionalProperties", UNSET)
 
         starred = d.pop("starred", UNSET)
 
+        draft_only = d.pop("draft_only", UNSET)
+
         flow = cls(
             summary=summary,
             value=value,
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             archived=archived,
             extra_perms=extra_perms,
             description=description,
             schema=schema,
             workspace_id=workspace_id,
             additional_properties=additional_properties,
             starred=starred,
+            draft_only=draft_only,
         )
 
         flow.additional_properties = d
         return flow
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_metadata.py` & `windmill_api-1.91.0/windmill_api/models/flow_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,37 +18,40 @@
         edited_by (str):
         edited_at (datetime.datetime):
         archived (bool):
         extra_perms (FlowMetadataExtraPerms):
         workspace_id (Union[Unset, str]):
         additional_properties (Union[Unset, bool]):
         starred (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     path: str
     edited_by: str
     edited_at: datetime.datetime
     archived: bool
     extra_perms: FlowMetadataExtraPerms
     workspace_id: Union[Unset, str] = UNSET
     additional_properties: Union[Unset, bool] = UNSET
     starred: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         edited_by = self.edited_by
         edited_at = self.edited_at.isoformat()
 
         archived = self.archived
         extra_perms = self.extra_perms.to_dict()
 
         workspace_id = self.workspace_id
         additional_properties = self.additional_properties
         starred = self.starred
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "edited_by": edited_by,
@@ -59,14 +62,16 @@
         )
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if additional_properties is not UNSET:
             field_dict["additionalProperties"] = additional_properties
         if starred is not UNSET:
             field_dict["starred"] = starred
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         path = d.pop("path")
@@ -81,23 +86,26 @@
 
         workspace_id = d.pop("workspace_id", UNSET)
 
         additional_properties = d.pop("additionalProperties", UNSET)
 
         starred = d.pop("starred", UNSET)
 
+        draft_only = d.pop("draft_only", UNSET)
+
         flow_metadata = cls(
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             archived=archived,
             extra_perms=extra_perms,
             workspace_id=workspace_id,
             additional_properties=additional_properties,
             starred=starred,
+            draft_only=draft_only,
         )
 
         flow_metadata.additional_properties = d
         return flow_metadata
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module.py` & `windmill_api-1.91.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.91.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_args.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FlowPreviewValueModulesItemRetryConstant")
+T = TypeVar("T", bound="ForloopFlowModulesItemRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class FlowPreviewValueModulesItemRetryConstant:
+class ForloopFlowModulesItemRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        flow_preview_value_modules_item_retry_constant = cls(
+        forloop_flow_modules_item_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        flow_preview_value_modules_item_retry_constant.additional_properties = d
-        return flow_preview_value_modules_item_retry_constant
+        forloop_flow_modules_item_retry_constant.additional_properties = d
+        return forloop_flow_modules_item_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_schema.py` & `windmill_api-1.91.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status.py` & `windmill_api-1.91.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_module.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value.py` & `windmill_api-1.91.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/folder.py` & `windmill_api-1.91.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.91.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ForloopFlowModulesItemRetryConstant")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItemRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class ForloopFlowModulesItemRetryConstant:
+class ListQueueResponse200ItemRawFlowModulesItemRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        forloop_flow_modules_item_retry_constant = cls(
+        list_queue_response_200_item_raw_flow_modules_item_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        forloop_flow_modules_item_retry_constant.additional_properties = d
-        return forloop_flow_modules_item_retry_constant
+        list_queue_response_200_item_raw_flow_modules_item_retry_constant.additional_properties = d
+        return list_queue_response_200_item_raw_flow_modules_item_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.91.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,30 @@
         archived (bool):
         extra_perms (GetFlowByPathResponse200ExtraPerms):
         description (Union[Unset, str]):
         schema (Union[Unset, GetFlowByPathResponse200Schema]):
         workspace_id (Union[Unset, str]):
         additional_properties (Union[Unset, bool]):
         starred (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     summary: str
     value: GetFlowByPathResponse200Value
     path: str
     edited_by: str
     edited_at: datetime.datetime
     archived: bool
     extra_perms: GetFlowByPathResponse200ExtraPerms
     description: Union[Unset, str] = UNSET
     schema: Union[Unset, GetFlowByPathResponse200Schema] = UNSET
     workspace_id: Union[Unset, str] = UNSET
     additional_properties: Union[Unset, bool] = UNSET
     starred: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         summary = self.summary
         value = self.value.to_dict()
 
         path = self.path
@@ -59,14 +61,15 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         workspace_id = self.workspace_id
         additional_properties = self.additional_properties
         starred = self.starred
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "summary": summary,
                 "value": value,
@@ -83,14 +86,16 @@
             field_dict["schema"] = schema
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if additional_properties is not UNSET:
             field_dict["additionalProperties"] = additional_properties
         if starred is not UNSET:
             field_dict["starred"] = starred
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         summary = d.pop("summary")
@@ -118,27 +123,30 @@
 
         workspace_id = d.pop("workspace_id", UNSET)
 
         additional_properties = d.pop("additionalProperties", UNSET)
 
         starred = d.pop("starred", UNSET)
 
+        draft_only = d.pop("draft_only", UNSET)
+
         get_flow_by_path_response_200 = cls(
             summary=summary,
             value=value,
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             archived=archived,
             extra_perms=extra_perms,
             description=description,
             schema=schema,
             workspace_id=workspace_id,
             additional_properties=additional_properties,
             starred=starred,
+            draft_only=draft_only,
         )
 
         get_flow_by_path_response_200.additional_properties = d
         return get_flow_by_path_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_group_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.91.0/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_job_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.91.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, GetScriptByHashResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
         tag (Union[Unset, str]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -56,14 +58,16 @@
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, GetScriptByHashResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
     tag: Union[Unset, str] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -89,14 +93,16 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
         tag = self.tag
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -122,14 +128,18 @@
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
         if tag is not UNSET:
             field_dict["tag"] = tag
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -173,14 +183,18 @@
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
         tag = d.pop("tag", UNSET)
 
+        has_draft = d.pop("has_draft", UNSET)
+
+        draft_only = d.pop("draft_only", UNSET)
+
         get_script_by_hash_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -194,14 +208,16 @@
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
             tag=tag,
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
         get_script_by_hash_response_200.additional_properties = d
         return get_script_by_hash_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, GetScriptByPathResponse200Schema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
         tag (Union[Unset, str]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -56,14 +58,16 @@
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, GetScriptByPathResponse200Schema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
     tag: Union[Unset, str] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -89,14 +93,16 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
         tag = self.tag
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -122,14 +128,18 @@
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
         if tag is not UNSET:
             field_dict["tag"] = tag
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -173,14 +183,18 @@
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
         tag = d.pop("tag", UNSET)
 
+        has_draft = d.pop("has_draft", UNSET)
+
+        draft_only = d.pop("draft_only", UNSET)
+
         get_script_by_path_response_200 = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -194,14 +208,16 @@
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
             tag=tag,
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
         get_script_by_path_response_200.additional_properties = d
         return get_script_by_path_response_200
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.91.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.91.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/global_user_info.py` & `windmill_api-1.91.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.91.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.91.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.91.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/group.py` & `windmill_api-1.91.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/group_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/identity.py` & `windmill_api-1.91.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/input_.py` & `windmill_api-1.91.0/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/input_args.py` & `windmill_api-1.91.0/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.91.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.91.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.91.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/javascript_transform.py` & `windmill_api-1.91.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/job.py` & `windmill_api-1.91.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.91.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.list_flows_response_200_item_extra_perms import ListFlowsResponse200ItemExtraPerms
-from ..models.list_flows_response_200_item_schema import ListFlowsResponse200ItemSchema
-from ..models.list_flows_response_200_item_value import ListFlowsResponse200ItemValue
+from ..models.get_flow_by_path_with_draft_response_200_draft_extra_perms import (
+    GetFlowByPathWithDraftResponse200DraftExtraPerms,
+)
+from ..models.get_flow_by_path_with_draft_response_200_draft_schema import GetFlowByPathWithDraftResponse200DraftSchema
+from ..models.get_flow_by_path_with_draft_response_200_draft_value import GetFlowByPathWithDraftResponse200DraftValue
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200Item")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200Draft")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200Item:
+class GetFlowByPathWithDraftResponse200Draft:
     """
     Attributes:
         summary (str):
-        value (ListFlowsResponse200ItemValue):
+        value (GetFlowByPathWithDraftResponse200DraftValue):
         path (str):
         edited_by (str):
         edited_at (datetime.datetime):
         archived (bool):
-        extra_perms (ListFlowsResponse200ItemExtraPerms):
+        extra_perms (GetFlowByPathWithDraftResponse200DraftExtraPerms):
         description (Union[Unset, str]):
-        schema (Union[Unset, ListFlowsResponse200ItemSchema]):
+        schema (Union[Unset, GetFlowByPathWithDraftResponse200DraftSchema]):
         workspace_id (Union[Unset, str]):
         additional_properties (Union[Unset, bool]):
         starred (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     summary: str
-    value: ListFlowsResponse200ItemValue
+    value: GetFlowByPathWithDraftResponse200DraftValue
     path: str
     edited_by: str
     edited_at: datetime.datetime
     archived: bool
-    extra_perms: ListFlowsResponse200ItemExtraPerms
+    extra_perms: GetFlowByPathWithDraftResponse200DraftExtraPerms
     description: Union[Unset, str] = UNSET
-    schema: Union[Unset, ListFlowsResponse200ItemSchema] = UNSET
+    schema: Union[Unset, GetFlowByPathWithDraftResponse200DraftSchema] = UNSET
     workspace_id: Union[Unset, str] = UNSET
     additional_properties: Union[Unset, bool] = UNSET
     starred: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         summary = self.summary
         value = self.value.to_dict()
 
         path = self.path
@@ -59,14 +63,15 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         workspace_id = self.workspace_id
         additional_properties = self.additional_properties
         starred = self.starred
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "summary": summary,
                 "value": value,
@@ -83,66 +88,71 @@
             field_dict["schema"] = schema
         if workspace_id is not UNSET:
             field_dict["workspace_id"] = workspace_id
         if additional_properties is not UNSET:
             field_dict["additionalProperties"] = additional_properties
         if starred is not UNSET:
             field_dict["starred"] = starred
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         summary = d.pop("summary")
 
-        value = ListFlowsResponse200ItemValue.from_dict(d.pop("value"))
+        value = GetFlowByPathWithDraftResponse200DraftValue.from_dict(d.pop("value"))
 
         path = d.pop("path")
 
         edited_by = d.pop("edited_by")
 
         edited_at = isoparse(d.pop("edited_at"))
 
         archived = d.pop("archived")
 
-        extra_perms = ListFlowsResponse200ItemExtraPerms.from_dict(d.pop("extra_perms"))
+        extra_perms = GetFlowByPathWithDraftResponse200DraftExtraPerms.from_dict(d.pop("extra_perms"))
 
         description = d.pop("description", UNSET)
 
         _schema = d.pop("schema", UNSET)
-        schema: Union[Unset, ListFlowsResponse200ItemSchema]
+        schema: Union[Unset, GetFlowByPathWithDraftResponse200DraftSchema]
         if isinstance(_schema, Unset):
             schema = UNSET
         else:
-            schema = ListFlowsResponse200ItemSchema.from_dict(_schema)
+            schema = GetFlowByPathWithDraftResponse200DraftSchema.from_dict(_schema)
 
         workspace_id = d.pop("workspace_id", UNSET)
 
         additional_properties = d.pop("additionalProperties", UNSET)
 
         starred = d.pop("starred", UNSET)
 
-        list_flows_response_200_item = cls(
+        draft_only = d.pop("draft_only", UNSET)
+
+        get_flow_by_path_with_draft_response_200_draft = cls(
             summary=summary,
             value=value,
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             archived=archived,
             extra_perms=extra_perms,
             description=description,
             schema=schema,
             workspace_id=workspace_id,
             additional_properties=additional_properties,
             starred=starred,
+            draft_only=draft_only,
         )
 
-        list_flows_response_200_item.additional_properties = d
-        return list_flows_response_200_item
+        get_flow_by_path_with_draft_response_200_draft.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemExtraPerms")
+T = TypeVar("T", bound="ListInputsResponse200ItemArgs")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemExtraPerms:
+class ListInputsResponse200ItemArgs:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
@@ -18,18 +18,18 @@
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        list_flows_response_200_item_extra_perms = cls()
+        list_inputs_response_200_item_args = cls()
 
-        list_flows_response_200_item_extra_perms.additional_properties = d
-        return list_flows_response_200_item_extra_perms
+        list_inputs_response_200_item_args.additional_properties = d
+        return list_inputs_response_200_item_args
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_schema.py` & `windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemSchema")
+T = TypeVar("T", bound="ListScriptsResponse200ItemSchema")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemSchema:
+class ListScriptsResponse200ItemSchema:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
@@ -18,18 +18,18 @@
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        list_flows_response_200_item_schema = cls()
+        list_scripts_response_200_item_schema = cls()
 
-        list_flows_response_200_item_schema.additional_properties = d
-        return list_flows_response_200_item_schema
+        list_scripts_response_200_item_schema.additional_properties = d
+        return list_scripts_response_200_item_schema
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_flows_response_200_item_value_failure_module import ListFlowsResponse200ItemValueFailureModule
-from ..models.list_flows_response_200_item_value_modules_item import ListFlowsResponse200ItemValueModulesItem
+from ..models.open_flow_value_failure_module import OpenFlowValueFailureModule
+from ..models.open_flow_value_modules_item import OpenFlowValueModulesItem
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValue")
+T = TypeVar("T", bound="OpenFlowValue")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValue:
+class OpenFlowValue:
     """
     Attributes:
-        modules (List[ListFlowsResponse200ItemValueModulesItem]):
-        failure_module (Union[Unset, ListFlowsResponse200ItemValueFailureModule]):
+        modules (List[OpenFlowValueModulesItem]):
+        failure_module (Union[Unset, OpenFlowValueFailureModule]):
         same_worker (Union[Unset, bool]):
     """
 
-    modules: List[ListFlowsResponse200ItemValueModulesItem]
-    failure_module: Union[Unset, ListFlowsResponse200ItemValueFailureModule] = UNSET
+    modules: List[OpenFlowValueModulesItem]
+    failure_module: Union[Unset, OpenFlowValueFailureModule] = UNSET
     same_worker: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         modules = []
         for modules_item_data in self.modules:
             modules_item = modules_item_data.to_dict()
@@ -52,35 +52,35 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         modules = []
         _modules = d.pop("modules")
         for modules_item_data in _modules:
-            modules_item = ListFlowsResponse200ItemValueModulesItem.from_dict(modules_item_data)
+            modules_item = OpenFlowValueModulesItem.from_dict(modules_item_data)
 
             modules.append(modules_item)
 
         _failure_module = d.pop("failure_module", UNSET)
-        failure_module: Union[Unset, ListFlowsResponse200ItemValueFailureModule]
+        failure_module: Union[Unset, OpenFlowValueFailureModule]
         if isinstance(_failure_module, Unset):
             failure_module = UNSET
         else:
-            failure_module = ListFlowsResponse200ItemValueFailureModule.from_dict(_failure_module)
+            failure_module = OpenFlowValueFailureModule.from_dict(_failure_module)
 
         same_worker = d.pop("same_worker", UNSET)
 
-        list_flows_response_200_item_value = cls(
+        open_flow_value = cls(
             modules=modules,
             failure_module=failure_module,
             same_worker=same_worker,
         )
 
-        list_flows_response_200_item_value.additional_properties = d
-        return list_flows_response_200_item_value
+        open_flow_value.additional_properties = d
+        return open_flow_value
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_flows_response_200_item_value_failure_module_retry import (
-    ListFlowsResponse200ItemValueFailureModuleRetry,
+from ..models.list_queue_response_200_item_raw_flow_failure_module_retry import (
+    ListQueueResponse200ItemRawFlowFailureModuleRetry,
 )
-from ..models.list_flows_response_200_item_value_failure_module_sleep_type_0 import (
-    ListFlowsResponse200ItemValueFailureModuleSleepType0,
+from ..models.list_queue_response_200_item_raw_flow_failure_module_sleep_type_0 import (
+    ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
 )
-from ..models.list_flows_response_200_item_value_failure_module_sleep_type_1 import (
-    ListFlowsResponse200ItemValueFailureModuleSleepType1,
+from ..models.list_queue_response_200_item_raw_flow_failure_module_sleep_type_1 import (
+    ListQueueResponse200ItemRawFlowFailureModuleSleepType1,
 )
-from ..models.list_flows_response_200_item_value_failure_module_stop_after_if import (
-    ListFlowsResponse200ItemValueFailureModuleStopAfterIf,
+from ..models.list_queue_response_200_item_raw_flow_failure_module_stop_after_if import (
+    ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf,
 )
-from ..models.list_flows_response_200_item_value_failure_module_suspend import (
-    ListFlowsResponse200ItemValueFailureModuleSuspend,
+from ..models.list_queue_response_200_item_raw_flow_failure_module_suspend import (
+    ListQueueResponse200ItemRawFlowFailureModuleSuspend,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModule")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModule")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModule:
+class ListQueueResponse200ItemRawFlowFailureModule:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, ListFlowsResponse200ItemValueFailureModuleStopAfterIf]):
-        sleep (Union[ListFlowsResponse200ItemValueFailureModuleSleepType0,
-            ListFlowsResponse200ItemValueFailureModuleSleepType1, Unset]):
+        stop_after_if (Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf]):
+        sleep (Union[ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
+            ListQueueResponse200ItemRawFlowFailureModuleSleepType1, Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, ListFlowsResponse200ItemValueFailureModuleSuspend]):
-        retry (Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetry]):
+        suspend (Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSuspend]):
+        retry (Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, ListFlowsResponse200ItemValueFailureModuleStopAfterIf] = UNSET
+    stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf] = UNSET
     sleep: Union[
-        ListFlowsResponse200ItemValueFailureModuleSleepType0,
-        ListFlowsResponse200ItemValueFailureModuleSleepType1,
+        ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
+        ListQueueResponse200ItemRawFlowFailureModuleSleepType1,
         Unset,
     ] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, ListFlowsResponse200ItemValueFailureModuleSuspend] = UNSET
-    retry: Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetry] = UNSET
+    suspend: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSuspend] = UNSET
+    retry: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, ListFlowsResponse200ItemValueFailureModuleSleepType0):
+        elif isinstance(self.sleep, ListQueueResponse200ItemRawFlowFailureModuleSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -104,83 +104,83 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, ListFlowsResponse200ItemValueFailureModuleStopAfterIf]
+        stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = ListFlowsResponse200ItemValueFailureModuleStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
         ) -> Union[
-            ListFlowsResponse200ItemValueFailureModuleSleepType0,
-            ListFlowsResponse200ItemValueFailureModuleSleepType1,
+            ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
+            ListQueueResponse200ItemRawFlowFailureModuleSleepType1,
             Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, ListFlowsResponse200ItemValueFailureModuleSleepType0]
+                sleep_type_0: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = ListFlowsResponse200ItemValueFailureModuleSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = ListQueueResponse200ItemRawFlowFailureModuleSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, ListFlowsResponse200ItemValueFailureModuleSleepType1]
+            sleep_type_1: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = ListFlowsResponse200ItemValueFailureModuleSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = ListQueueResponse200ItemRawFlowFailureModuleSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, ListFlowsResponse200ItemValueFailureModuleSuspend]
+        suspend: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = ListFlowsResponse200ItemValueFailureModuleSuspend.from_dict(_suspend)
+            suspend = ListQueueResponse200ItemRawFlowFailureModuleSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetry]
+        retry: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = ListFlowsResponse200ItemValueFailureModuleRetry.from_dict(_retry)
+            retry = ListQueueResponse200ItemRawFlowFailureModuleRetry.from_dict(_retry)
 
-        list_flows_response_200_item_value_failure_module = cls(
+        list_queue_response_200_item_raw_flow_failure_module = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        list_flows_response_200_item_value_failure_module.additional_properties = d
-        return list_flows_response_200_item_value_failure_module
+        list_queue_response_200_item_raw_flow_failure_module.additional_properties = d
+        return list_queue_response_200_item_raw_flow_failure_module
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_flows_response_200_item_value_failure_module_retry_constant import (
-    ListFlowsResponse200ItemValueFailureModuleRetryConstant,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant import (
+    GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryConstant,
 )
-from ..models.list_flows_response_200_item_value_failure_module_retry_exponential import (
-    ListFlowsResponse200ItemValueFailureModuleRetryExponential,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential import (
+    GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryExponential,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleRetry")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetry")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleRetry:
+class GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetry:
     """
     Attributes:
-        constant (Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetryConstant]):
-        exponential (Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetryExponential]):
+        constant (Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryConstant]):
+        exponential (Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryExponential]):
     """
 
-    constant: Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetryConstant] = UNSET
-    exponential: Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetryExponential] = UNSET
+    constant: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryConstant] = UNSET
+    exponential: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryExponential] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         constant: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.constant, Unset):
             constant = self.constant.to_dict()
 
@@ -44,34 +44,36 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetryConstant]
+        constant: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryConstant]
         if isinstance(_constant, Unset):
             constant = UNSET
         else:
-            constant = ListFlowsResponse200ItemValueFailureModuleRetryConstant.from_dict(_constant)
+            constant = GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryConstant.from_dict(_constant)
 
         _exponential = d.pop("exponential", UNSET)
-        exponential: Union[Unset, ListFlowsResponse200ItemValueFailureModuleRetryExponential]
+        exponential: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryExponential]
         if isinstance(_exponential, Unset):
             exponential = UNSET
         else:
-            exponential = ListFlowsResponse200ItemValueFailureModuleRetryExponential.from_dict(_exponential)
+            exponential = GetFlowByPathWithDraftResponse200DraftValueFailureModuleRetryExponential.from_dict(
+                _exponential
+            )
 
-        list_flows_response_200_item_value_failure_module_retry = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry = cls(
             constant=constant,
             exponential=exponential,
         )
 
-        list_flows_response_200_item_value_failure_module_retry.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_retry
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleRetryConstant")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleRetryConstant:
+class RunFlowPreviewJsonBodyValueModulesItemRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        list_flows_response_200_item_value_failure_module_retry_constant = cls(
+        run_flow_preview_json_body_value_modules_item_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        list_flows_response_200_item_value_failure_module_retry_constant.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_retry_constant
+        run_flow_preview_json_body_value_modules_item_retry_constant.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleRetryExponential")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModuleRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleRetryExponential:
+class ListQueueResponse200ItemRawFlowFailureModuleRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        list_flows_response_200_item_value_failure_module_retry_exponential = cls(
+        list_queue_response_200_item_raw_flow_failure_module_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        list_flows_response_200_item_value_failure_module_retry_exponential.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_retry_exponential
+        list_queue_response_200_item_raw_flow_failure_module_retry_exponential.additional_properties = d
+        return list_queue_response_200_item_raw_flow_failure_module_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_flows_response_200_item_value_failure_module_sleep_type_0_type import (
-    ListFlowsResponse200ItemValueFailureModuleSleepType0Type,
+from ..models.open_flow_w_path_value_failure_module_sleep_type_0_type import (
+    OpenFlowWPathValueFailureModuleSleepType0Type,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleSleepType0")
+T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleSleepType0:
+class OpenFlowWPathValueFailureModuleSleepType0:
     """
     Attributes:
-        type (ListFlowsResponse200ItemValueFailureModuleSleepType0Type):
+        type (OpenFlowWPathValueFailureModuleSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: ListFlowsResponse200ItemValueFailureModuleSleepType0Type
+    type: OpenFlowWPathValueFailureModuleSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = ListFlowsResponse200ItemValueFailureModuleSleepType0Type(d.pop("type"))
+        type = OpenFlowWPathValueFailureModuleSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        list_flows_response_200_item_value_failure_module_sleep_type_0 = cls(
+        open_flow_w_path_value_failure_module_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        list_flows_response_200_item_value_failure_module_sleep_type_0.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_sleep_type_0
+        open_flow_w_path_value_failure_module_sleep_type_0.additional_properties = d
+        return open_flow_w_path_value_failure_module_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.list_flows_response_200_item_value_failure_module_sleep_type_1_type import (
-    ListFlowsResponse200ItemValueFailureModuleSleepType1Type,
+from ..models.list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type import (
+    ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type,
 )
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleSleepType1")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModuleSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleSleepType1:
+class ListQueueResponse200ItemRawFlowFailureModuleSleepType1:
     """
     Attributes:
         expr (str):
-        type (ListFlowsResponse200ItemValueFailureModuleSleepType1Type):
+        type (ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type):
     """
 
     expr: str
-    type: ListFlowsResponse200ItemValueFailureModuleSleepType1Type
+    type: ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = ListFlowsResponse200ItemValueFailureModuleSleepType1Type(d.pop("type"))
+        type = ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type(d.pop("type"))
 
-        list_flows_response_200_item_value_failure_module_sleep_type_1 = cls(
+        list_queue_response_200_item_raw_flow_failure_module_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        list_flows_response_200_item_value_failure_module_sleep_type_1.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_sleep_type_1
+        list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.additional_properties = d
+        return list_queue_response_200_item_raw_flow_failure_module_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleStopAfterIf")
+T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleStopAfterIf:
+class OpenFlowWPathValueFailureModuleStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        list_flows_response_200_item_value_failure_module_stop_after_if = cls(
+        open_flow_w_path_value_failure_module_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        list_flows_response_200_item_value_failure_module_stop_after_if.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_stop_after_if
+        open_flow_w_path_value_failure_module_stop_after_if.additional_properties = d
+        return open_flow_w_path_value_failure_module_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueFailureModuleSuspend")
+T = TypeVar("T", bound="QueuedJobRawFlowFailureModuleSuspend")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueFailureModuleSuspend:
+class QueuedJobRawFlowFailureModuleSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        list_flows_response_200_item_value_failure_module_suspend = cls(
+        queued_job_raw_flow_failure_module_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        list_flows_response_200_item_value_failure_module_suspend.additional_properties = d
-        return list_flows_response_200_item_value_failure_module_suspend
+        queued_job_raw_flow_failure_module_suspend.additional_properties = d
+        return queued_job_raw_flow_failure_module_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_flows_response_200_item_value_modules_item_retry import ListFlowsResponse200ItemValueModulesItemRetry
-from ..models.list_flows_response_200_item_value_modules_item_sleep_type_0 import (
-    ListFlowsResponse200ItemValueModulesItemSleepType0,
-)
-from ..models.list_flows_response_200_item_value_modules_item_sleep_type_1 import (
-    ListFlowsResponse200ItemValueModulesItemSleepType1,
-)
-from ..models.list_flows_response_200_item_value_modules_item_stop_after_if import (
-    ListFlowsResponse200ItemValueModulesItemStopAfterIf,
-)
-from ..models.list_flows_response_200_item_value_modules_item_suspend import (
-    ListFlowsResponse200ItemValueModulesItemSuspend,
-)
+from ..models.open_flow_value_modules_item_retry import OpenFlowValueModulesItemRetry
+from ..models.open_flow_value_modules_item_sleep_type_0 import OpenFlowValueModulesItemSleepType0
+from ..models.open_flow_value_modules_item_sleep_type_1 import OpenFlowValueModulesItemSleepType1
+from ..models.open_flow_value_modules_item_stop_after_if import OpenFlowValueModulesItemStopAfterIf
+from ..models.open_flow_value_modules_item_suspend import OpenFlowValueModulesItemSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItem")
+T = TypeVar("T", bound="OpenFlowValueModulesItem")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItem:
+class OpenFlowValueModulesItem:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, ListFlowsResponse200ItemValueModulesItemStopAfterIf]):
-        sleep (Union[ListFlowsResponse200ItemValueModulesItemSleepType0,
-            ListFlowsResponse200ItemValueModulesItemSleepType1, Unset]):
+        stop_after_if (Union[Unset, OpenFlowValueModulesItemStopAfterIf]):
+        sleep (Union[OpenFlowValueModulesItemSleepType0, OpenFlowValueModulesItemSleepType1, Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, ListFlowsResponse200ItemValueModulesItemSuspend]):
-        retry (Union[Unset, ListFlowsResponse200ItemValueModulesItemRetry]):
+        suspend (Union[Unset, OpenFlowValueModulesItemSuspend]):
+        retry (Union[Unset, OpenFlowValueModulesItemRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, ListFlowsResponse200ItemValueModulesItemStopAfterIf] = UNSET
-    sleep: Union[
-        ListFlowsResponse200ItemValueModulesItemSleepType0, ListFlowsResponse200ItemValueModulesItemSleepType1, Unset
-    ] = UNSET
+    stop_after_if: Union[Unset, OpenFlowValueModulesItemStopAfterIf] = UNSET
+    sleep: Union[OpenFlowValueModulesItemSleepType0, OpenFlowValueModulesItemSleepType1, Unset] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, ListFlowsResponse200ItemValueModulesItemSuspend] = UNSET
-    retry: Union[Unset, ListFlowsResponse200ItemValueModulesItemRetry] = UNSET
+    suspend: Union[Unset, OpenFlowValueModulesItemSuspend] = UNSET
+    retry: Union[Unset, OpenFlowValueModulesItemRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, ListFlowsResponse200ItemValueModulesItemSleepType0):
+        elif isinstance(self.sleep, OpenFlowValueModulesItemSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -100,83 +89,79 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, ListFlowsResponse200ItemValueModulesItemStopAfterIf]
+        stop_after_if: Union[Unset, OpenFlowValueModulesItemStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = ListFlowsResponse200ItemValueModulesItemStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = OpenFlowValueModulesItemStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
-        ) -> Union[
-            ListFlowsResponse200ItemValueModulesItemSleepType0,
-            ListFlowsResponse200ItemValueModulesItemSleepType1,
-            Unset,
-        ]:
+        ) -> Union[OpenFlowValueModulesItemSleepType0, OpenFlowValueModulesItemSleepType1, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, ListFlowsResponse200ItemValueModulesItemSleepType0]
+                sleep_type_0: Union[Unset, OpenFlowValueModulesItemSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = ListFlowsResponse200ItemValueModulesItemSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = OpenFlowValueModulesItemSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, ListFlowsResponse200ItemValueModulesItemSleepType1]
+            sleep_type_1: Union[Unset, OpenFlowValueModulesItemSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = ListFlowsResponse200ItemValueModulesItemSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = OpenFlowValueModulesItemSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, ListFlowsResponse200ItemValueModulesItemSuspend]
+        suspend: Union[Unset, OpenFlowValueModulesItemSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = ListFlowsResponse200ItemValueModulesItemSuspend.from_dict(_suspend)
+            suspend = OpenFlowValueModulesItemSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, ListFlowsResponse200ItemValueModulesItemRetry]
+        retry: Union[Unset, OpenFlowValueModulesItemRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = ListFlowsResponse200ItemValueModulesItemRetry.from_dict(_retry)
+            retry = OpenFlowValueModulesItemRetry.from_dict(_retry)
 
-        list_flows_response_200_item_value_modules_item = cls(
+        open_flow_value_modules_item = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        list_flows_response_200_item_value_modules_item.additional_properties = d
-        return list_flows_response_200_item_value_modules_item
+        open_flow_value_modules_item.additional_properties = d
+        return open_flow_value_modules_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItemRetryConstant")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItemRetryConstant:
+class RunFlowPreviewJsonBodyValueFailureModuleRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        list_flows_response_200_item_value_modules_item_retry_constant = cls(
+        run_flow_preview_json_body_value_failure_module_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        list_flows_response_200_item_value_modules_item_retry_constant.additional_properties = d
-        return list_flows_response_200_item_value_modules_item_retry_constant
+        run_flow_preview_json_body_value_failure_module_retry_constant.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItemRetryExponential")
+T = TypeVar("T", bound="OpenFlowWPathValueModulesItemRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItemRetryExponential:
+class OpenFlowWPathValueModulesItemRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        list_flows_response_200_item_value_modules_item_retry_exponential = cls(
+        open_flow_w_path_value_modules_item_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        list_flows_response_200_item_value_modules_item_retry_exponential.additional_properties = d
-        return list_flows_response_200_item_value_modules_item_retry_exponential
+        open_flow_w_path_value_modules_item_retry_exponential.additional_properties = d
+        return open_flow_w_path_value_modules_item_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_flows_response_200_item_value_modules_item_sleep_type_0_type import (
-    ListFlowsResponse200ItemValueModulesItemSleepType0Type,
-)
+from ..models.open_flow_value_modules_item_sleep_type_0_type import OpenFlowValueModulesItemSleepType0Type
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItemSleepType0")
+T = TypeVar("T", bound="OpenFlowValueModulesItemSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItemSleepType0:
+class OpenFlowValueModulesItemSleepType0:
     """
     Attributes:
-        type (ListFlowsResponse200ItemValueModulesItemSleepType0Type):
+        type (OpenFlowValueModulesItemSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: ListFlowsResponse200ItemValueModulesItemSleepType0Type
+    type: OpenFlowValueModulesItemSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +36,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = ListFlowsResponse200ItemValueModulesItemSleepType0Type(d.pop("type"))
+        type = OpenFlowValueModulesItemSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        list_flows_response_200_item_value_modules_item_sleep_type_0 = cls(
+        open_flow_value_modules_item_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        list_flows_response_200_item_value_modules_item_sleep_type_0.additional_properties = d
-        return list_flows_response_200_item_value_modules_item_sleep_type_0
+        open_flow_value_modules_item_sleep_type_0.additional_properties = d
+        return open_flow_value_modules_item_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.list_flows_response_200_item_value_modules_item_sleep_type_1_type import (
-    ListFlowsResponse200ItemValueModulesItemSleepType1Type,
+from ..models.open_flow_w_path_value_failure_module_sleep_type_1_type import (
+    OpenFlowWPathValueFailureModuleSleepType1Type,
 )
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItemSleepType1")
+T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItemSleepType1:
+class OpenFlowWPathValueFailureModuleSleepType1:
     """
     Attributes:
         expr (str):
-        type (ListFlowsResponse200ItemValueModulesItemSleepType1Type):
+        type (OpenFlowWPathValueFailureModuleSleepType1Type):
     """
 
     expr: str
-    type: ListFlowsResponse200ItemValueModulesItemSleepType1Type
+    type: OpenFlowWPathValueFailureModuleSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = ListFlowsResponse200ItemValueModulesItemSleepType1Type(d.pop("type"))
+        type = OpenFlowWPathValueFailureModuleSleepType1Type(d.pop("type"))
 
-        list_flows_response_200_item_value_modules_item_sleep_type_1 = cls(
+        open_flow_w_path_value_failure_module_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        list_flows_response_200_item_value_modules_item_sleep_type_1.additional_properties = d
-        return list_flows_response_200_item_value_modules_item_sleep_type_1
+        open_flow_w_path_value_failure_module_sleep_type_1.additional_properties = d
+        return open_flow_w_path_value_failure_module_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItemStopAfterIf")
+T = TypeVar("T", bound="QueuedJobRawFlowModulesItemStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItemStopAfterIf:
+class QueuedJobRawFlowModulesItemStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        list_flows_response_200_item_value_modules_item_stop_after_if = cls(
+        queued_job_raw_flow_modules_item_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        list_flows_response_200_item_value_modules_item_stop_after_if.additional_properties = d
-        return list_flows_response_200_item_value_modules_item_stop_after_if
+        queued_job_raw_flow_modules_item_stop_after_if.additional_properties = d
+        return queued_job_raw_flow_modules_item_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListFlowsResponse200ItemValueModulesItemSuspend")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class ListFlowsResponse200ItemValueModulesItemSuspend:
+class ListQueueResponse200ItemRawFlowModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        list_flows_response_200_item_value_modules_item_suspend = cls(
+        list_queue_response_200_item_raw_flow_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        list_flows_response_200_item_value_modules_item_suspend.additional_properties = d
-        return list_flows_response_200_item_value_modules_item_suspend
+        list_queue_response_200_item_raw_flow_modules_item_suspend.additional_properties = d
+        return list_queue_response_200_item_raw_flow_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.91.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.91.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.91.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.91.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.91.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.91.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.91.0/windmill_api/models/script_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ListInputsResponse200ItemArgs")
+T = TypeVar("T", bound="ScriptArgs")
 
 
 @attr.s(auto_attribs=True)
-class ListInputsResponse200ItemArgs:
+class ScriptArgs:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
@@ -18,18 +18,18 @@
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        list_inputs_response_200_item_args = cls()
+        script_args = cls()
 
-        list_inputs_response_200_item_args.additional_properties = d
-        return list_inputs_response_200_item_args
+        script_args.additional_properties = d
+        return script_args
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_queue_response_200_item_raw_flow_failure_module_retry import (
-    ListQueueResponse200ItemRawFlowFailureModuleRetry,
+from ..models.list_queue_response_200_item_raw_flow_modules_item_retry import (
+    ListQueueResponse200ItemRawFlowModulesItemRetry,
 )
-from ..models.list_queue_response_200_item_raw_flow_failure_module_sleep_type_0 import (
-    ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
+from ..models.list_queue_response_200_item_raw_flow_modules_item_sleep_type_0 import (
+    ListQueueResponse200ItemRawFlowModulesItemSleepType0,
 )
-from ..models.list_queue_response_200_item_raw_flow_failure_module_sleep_type_1 import (
-    ListQueueResponse200ItemRawFlowFailureModuleSleepType1,
+from ..models.list_queue_response_200_item_raw_flow_modules_item_sleep_type_1 import (
+    ListQueueResponse200ItemRawFlowModulesItemSleepType1,
 )
-from ..models.list_queue_response_200_item_raw_flow_failure_module_stop_after_if import (
-    ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf,
+from ..models.list_queue_response_200_item_raw_flow_modules_item_stop_after_if import (
+    ListQueueResponse200ItemRawFlowModulesItemStopAfterIf,
 )
-from ..models.list_queue_response_200_item_raw_flow_failure_module_suspend import (
-    ListQueueResponse200ItemRawFlowFailureModuleSuspend,
+from ..models.list_queue_response_200_item_raw_flow_modules_item_suspend import (
+    ListQueueResponse200ItemRawFlowModulesItemSuspend,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModule")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItem")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowFailureModule:
+class ListQueueResponse200ItemRawFlowModulesItem:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf]):
-        sleep (Union[ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
-            ListQueueResponse200ItemRawFlowFailureModuleSleepType1, Unset]):
+        stop_after_if (Union[Unset, ListQueueResponse200ItemRawFlowModulesItemStopAfterIf]):
+        sleep (Union[ListQueueResponse200ItemRawFlowModulesItemSleepType0,
+            ListQueueResponse200ItemRawFlowModulesItemSleepType1, Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSuspend]):
-        retry (Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleRetry]):
+        suspend (Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSuspend]):
+        retry (Union[Unset, ListQueueResponse200ItemRawFlowModulesItemRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf] = UNSET
+    stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemStopAfterIf] = UNSET
     sleep: Union[
-        ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
-        ListQueueResponse200ItemRawFlowFailureModuleSleepType1,
+        ListQueueResponse200ItemRawFlowModulesItemSleepType0,
+        ListQueueResponse200ItemRawFlowModulesItemSleepType1,
         Unset,
     ] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSuspend] = UNSET
-    retry: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleRetry] = UNSET
+    suspend: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSuspend] = UNSET
+    retry: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, ListQueueResponse200ItemRawFlowFailureModuleSleepType0):
+        elif isinstance(self.sleep, ListQueueResponse200ItemRawFlowModulesItemSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -104,83 +104,83 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf]
+        stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = ListQueueResponse200ItemRawFlowModulesItemStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
         ) -> Union[
-            ListQueueResponse200ItemRawFlowFailureModuleSleepType0,
-            ListQueueResponse200ItemRawFlowFailureModuleSleepType1,
+            ListQueueResponse200ItemRawFlowModulesItemSleepType0,
+            ListQueueResponse200ItemRawFlowModulesItemSleepType1,
             Unset,
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSleepType0]
+                sleep_type_0: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = ListQueueResponse200ItemRawFlowFailureModuleSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = ListQueueResponse200ItemRawFlowModulesItemSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSleepType1]
+            sleep_type_1: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = ListQueueResponse200ItemRawFlowFailureModuleSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = ListQueueResponse200ItemRawFlowModulesItemSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleSuspend]
+        suspend: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = ListQueueResponse200ItemRawFlowFailureModuleSuspend.from_dict(_suspend)
+            suspend = ListQueueResponse200ItemRawFlowModulesItemSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, ListQueueResponse200ItemRawFlowFailureModuleRetry]
+        retry: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = ListQueueResponse200ItemRawFlowFailureModuleRetry.from_dict(_retry)
+            retry = ListQueueResponse200ItemRawFlowModulesItemRetry.from_dict(_retry)
 
-        list_queue_response_200_item_raw_flow_failure_module = cls(
+        list_queue_response_200_item_raw_flow_modules_item = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        list_queue_response_200_item_raw_flow_failure_module.additional_properties = d
-        return list_queue_response_200_item_raw_flow_failure_module
+        list_queue_response_200_item_raw_flow_modules_item.additional_properties = d
+        return list_queue_response_200_item_raw_flow_modules_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModuleRetryExponential")
+T = TypeVar("T", bound="OpenFlowValueFailureModuleRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowFailureModuleRetryExponential:
+class OpenFlowValueFailureModuleRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        list_queue_response_200_item_raw_flow_failure_module_retry_exponential = cls(
+        open_flow_value_failure_module_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        list_queue_response_200_item_raw_flow_failure_module_retry_exponential.additional_properties = d
-        return list_queue_response_200_item_raw_flow_failure_module_retry_exponential
+        open_flow_value_failure_module_retry_exponential.additional_properties = d
+        return open_flow_value_failure_module_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type import (
-    ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type,
-)
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModuleSleepType1")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowFailureModuleSleepType1:
+class ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf:
     """
     Attributes:
         expr (str):
-        type (ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type):
+        skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
-    type: ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type
+    skip_if_stopped: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
-        type = self.type.value
+        skip_if_stopped = self.skip_if_stopped
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "expr": expr,
-                "type": type,
             }
         )
+        if skip_if_stopped is not UNSET:
+            field_dict["skip_if_stopped"] = skip_if_stopped
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = ListQueueResponse200ItemRawFlowFailureModuleSleepType1Type(d.pop("type"))
+        skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        list_queue_response_200_item_raw_flow_failure_module_sleep_type_1 = cls(
+        list_queue_response_200_item_raw_flow_failure_module_stop_after_if = cls(
             expr=expr,
-            type=type,
+            skip_if_stopped=skip_if_stopped,
         )
 
-        list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.additional_properties = d
-        return list_queue_response_200_item_raw_flow_failure_module_sleep_type_1
+        list_queue_response_200_item_raw_flow_failure_module_stop_after_if.additional_properties = d
+        return list_queue_response_200_item_raw_flow_failure_module_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf")
+T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItemStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowFailureModuleStopAfterIf:
+class ListQueueResponse200ItemRawFlowModulesItemStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        list_queue_response_200_item_raw_flow_failure_module_stop_after_if = cls(
+        list_queue_response_200_item_raw_flow_modules_item_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        list_queue_response_200_item_raw_flow_failure_module_stop_after_if.additional_properties = d
-        return list_queue_response_200_item_raw_flow_failure_module_stop_after_if
+        list_queue_response_200_item_raw_flow_modules_item_stop_after_if.additional_properties = d
+        return list_queue_response_200_item_raw_flow_modules_item_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,55 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.list_queue_response_200_item_raw_flow_modules_item_retry import (
-    ListQueueResponse200ItemRawFlowModulesItemRetry,
-)
-from ..models.list_queue_response_200_item_raw_flow_modules_item_sleep_type_0 import (
-    ListQueueResponse200ItemRawFlowModulesItemSleepType0,
-)
-from ..models.list_queue_response_200_item_raw_flow_modules_item_sleep_type_1 import (
-    ListQueueResponse200ItemRawFlowModulesItemSleepType1,
-)
-from ..models.list_queue_response_200_item_raw_flow_modules_item_stop_after_if import (
-    ListQueueResponse200ItemRawFlowModulesItemStopAfterIf,
-)
-from ..models.list_queue_response_200_item_raw_flow_modules_item_suspend import (
-    ListQueueResponse200ItemRawFlowModulesItemSuspend,
-)
+from ..models.queued_job_raw_flow_modules_item_retry import QueuedJobRawFlowModulesItemRetry
+from ..models.queued_job_raw_flow_modules_item_sleep_type_0 import QueuedJobRawFlowModulesItemSleepType0
+from ..models.queued_job_raw_flow_modules_item_sleep_type_1 import QueuedJobRawFlowModulesItemSleepType1
+from ..models.queued_job_raw_flow_modules_item_stop_after_if import QueuedJobRawFlowModulesItemStopAfterIf
+from ..models.queued_job_raw_flow_modules_item_suspend import QueuedJobRawFlowModulesItemSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItem")
+T = TypeVar("T", bound="QueuedJobRawFlowModulesItem")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowModulesItem:
+class QueuedJobRawFlowModulesItem:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, ListQueueResponse200ItemRawFlowModulesItemStopAfterIf]):
-        sleep (Union[ListQueueResponse200ItemRawFlowModulesItemSleepType0,
-            ListQueueResponse200ItemRawFlowModulesItemSleepType1, Unset]):
+        stop_after_if (Union[Unset, QueuedJobRawFlowModulesItemStopAfterIf]):
+        sleep (Union[QueuedJobRawFlowModulesItemSleepType0, QueuedJobRawFlowModulesItemSleepType1, Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSuspend]):
-        retry (Union[Unset, ListQueueResponse200ItemRawFlowModulesItemRetry]):
+        suspend (Union[Unset, QueuedJobRawFlowModulesItemSuspend]):
+        retry (Union[Unset, QueuedJobRawFlowModulesItemRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemStopAfterIf] = UNSET
-    sleep: Union[
-        ListQueueResponse200ItemRawFlowModulesItemSleepType0,
-        ListQueueResponse200ItemRawFlowModulesItemSleepType1,
-        Unset,
-    ] = UNSET
+    stop_after_if: Union[Unset, QueuedJobRawFlowModulesItemStopAfterIf] = UNSET
+    sleep: Union[QueuedJobRawFlowModulesItemSleepType0, QueuedJobRawFlowModulesItemSleepType1, Unset] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSuspend] = UNSET
-    retry: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemRetry] = UNSET
+    suspend: Union[Unset, QueuedJobRawFlowModulesItemSuspend] = UNSET
+    retry: Union[Unset, QueuedJobRawFlowModulesItemRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, ListQueueResponse200ItemRawFlowModulesItemSleepType0):
+        elif isinstance(self.sleep, QueuedJobRawFlowModulesItemSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -104,83 +89,79 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemStopAfterIf]
+        stop_after_if: Union[Unset, QueuedJobRawFlowModulesItemStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = ListQueueResponse200ItemRawFlowModulesItemStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = QueuedJobRawFlowModulesItemStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
-        ) -> Union[
-            ListQueueResponse200ItemRawFlowModulesItemSleepType0,
-            ListQueueResponse200ItemRawFlowModulesItemSleepType1,
-            Unset,
-        ]:
+        ) -> Union[QueuedJobRawFlowModulesItemSleepType0, QueuedJobRawFlowModulesItemSleepType1, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSleepType0]
+                sleep_type_0: Union[Unset, QueuedJobRawFlowModulesItemSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = ListQueueResponse200ItemRawFlowModulesItemSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = QueuedJobRawFlowModulesItemSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSleepType1]
+            sleep_type_1: Union[Unset, QueuedJobRawFlowModulesItemSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = ListQueueResponse200ItemRawFlowModulesItemSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = QueuedJobRawFlowModulesItemSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemSuspend]
+        suspend: Union[Unset, QueuedJobRawFlowModulesItemSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = ListQueueResponse200ItemRawFlowModulesItemSuspend.from_dict(_suspend)
+            suspend = QueuedJobRawFlowModulesItemSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, ListQueueResponse200ItemRawFlowModulesItemRetry]
+        retry: Union[Unset, QueuedJobRawFlowModulesItemRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = ListQueueResponse200ItemRawFlowModulesItemRetry.from_dict(_retry)
+            retry = QueuedJobRawFlowModulesItemRetry.from_dict(_retry)
 
-        list_queue_response_200_item_raw_flow_modules_item = cls(
+        queued_job_raw_flow_modules_item = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        list_queue_response_200_item_raw_flow_modules_item.additional_properties = d
-        return list_queue_response_200_item_raw_flow_modules_item
+        queued_job_raw_flow_modules_item.additional_properties = d
+        return queued_job_raw_flow_modules_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItemRetryConstant")
+T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowModulesItemRetryConstant:
+class OpenFlowWPathValueFailureModuleRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        list_queue_response_200_item_raw_flow_modules_item_retry_constant = cls(
+        open_flow_w_path_value_failure_module_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        list_queue_response_200_item_raw_flow_modules_item_retry_constant.additional_properties = d
-        return list_queue_response_200_item_raw_flow_modules_item_retry_constant
+        open_flow_w_path_value_failure_module_retry_constant.additional_properties = d
+        return open_flow_w_path_value_failure_module_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItemStopAfterIf")
+T = TypeVar("T", bound="QueuedJobRawFlowFailureModuleStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowModulesItemStopAfterIf:
+class QueuedJobRawFlowFailureModuleStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        list_queue_response_200_item_raw_flow_modules_item_stop_after_if = cls(
+        queued_job_raw_flow_failure_module_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        list_queue_response_200_item_raw_flow_modules_item_stop_after_if.additional_properties = d
-        return list_queue_response_200_item_raw_flow_modules_item_stop_after_if
+        queued_job_raw_flow_failure_module_stop_after_if.additional_properties = d
+        return queued_job_raw_flow_failure_module_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListQueueResponse200ItemRawFlowModulesItemSuspend")
+T = TypeVar("T", bound="OpenFlowValueModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class ListQueueResponse200ItemRawFlowModulesItemSuspend:
+class OpenFlowValueModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        list_queue_response_200_item_raw_flow_modules_item_suspend = cls(
+        open_flow_value_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        list_queue_response_200_item_raw_flow_modules_item_suspend.additional_properties = d
-        return list_queue_response_200_item_raw_flow_modules_item_suspend
+        open_flow_value_modules_item_suspend.additional_properties = d
+        return open_flow_value_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.91.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, ListScriptsResponse200ItemSchema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
         tag (Union[Unset, str]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -56,14 +58,16 @@
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, ListScriptsResponse200ItemSchema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
     tag: Union[Unset, str] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -89,14 +93,16 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
         tag = self.tag
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -122,14 +128,18 @@
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
         if tag is not UNSET:
             field_dict["tag"] = tag
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -173,14 +183,18 @@
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
         tag = d.pop("tag", UNSET)
 
+        has_draft = d.pop("has_draft", UNSET)
+
+        draft_only = d.pop("draft_only", UNSET)
+
         list_scripts_response_200_item = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -194,14 +208,16 @@
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
             tag=tag,
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
         list_scripts_response_200_item.additional_properties = d
         return list_scripts_response_200_item
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.91.0/windmill_api/models/schedule_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ListScriptsResponse200ItemSchema")
+T = TypeVar("T", bound="ScheduleArgs")
 
 
 @attr.s(auto_attribs=True)
-class ListScriptsResponse200ItemSchema:
+class ScheduleArgs:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
@@ -18,18 +18,18 @@
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        list_scripts_response_200_item_schema = cls()
+        schedule_args = cls()
 
-        list_scripts_response_200_item_schema.additional_properties = d
-        return list_scripts_response_200_item_schema
+        schedule_args.additional_properties = d
+        return schedule_args
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.91.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.91.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.91.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.91.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/listable_app.py` & `windmill_api-1.91.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/listable_resource.py` & `windmill_api-1.91.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/listable_variable.py` & `windmill_api-1.91.0/windmill_api/models/schedule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,143 @@
+import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
+from dateutil.parser import isoparse
 
-from ..models.listable_variable_extra_perms import ListableVariableExtraPerms
+from ..models.schedule_args import ScheduleArgs
+from ..models.schedule_extra_perms import ScheduleExtraPerms
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListableVariable")
+T = TypeVar("T", bound="Schedule")
 
 
 @attr.s(auto_attribs=True)
-class ListableVariable:
+class Schedule:
     """
     Attributes:
-        workspace_id (str):
         path (str):
-        is_secret (bool):
-        extra_perms (ListableVariableExtraPerms):
-        value (Union[Unset, str]):
-        description (Union[Unset, str]):
-        account (Union[Unset, int]):
-        is_oauth (Union[Unset, bool]):
-        is_expired (Union[Unset, bool]):
-        refresh_error (Union[Unset, str]):
-        is_linked (Union[Unset, bool]):
-        is_refreshed (Union[Unset, bool]):
+        edited_by (str):
+        edited_at (datetime.datetime):
+        schedule (str):
+        timezone (str):
+        enabled (bool):
+        script_path (str):
+        is_flow (bool):
+        extra_perms (ScheduleExtraPerms):
+        email (str):
+        args (Union[Unset, ScheduleArgs]):
+        error (Union[Unset, str]):
     """
 
-    workspace_id: str
     path: str
-    is_secret: bool
-    extra_perms: ListableVariableExtraPerms
-    value: Union[Unset, str] = UNSET
-    description: Union[Unset, str] = UNSET
-    account: Union[Unset, int] = UNSET
-    is_oauth: Union[Unset, bool] = UNSET
-    is_expired: Union[Unset, bool] = UNSET
-    refresh_error: Union[Unset, str] = UNSET
-    is_linked: Union[Unset, bool] = UNSET
-    is_refreshed: Union[Unset, bool] = UNSET
+    edited_by: str
+    edited_at: datetime.datetime
+    schedule: str
+    timezone: str
+    enabled: bool
+    script_path: str
+    is_flow: bool
+    extra_perms: ScheduleExtraPerms
+    email: str
+    args: Union[Unset, ScheduleArgs] = UNSET
+    error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        workspace_id = self.workspace_id
         path = self.path
-        is_secret = self.is_secret
+        edited_by = self.edited_by
+        edited_at = self.edited_at.isoformat()
+
+        schedule = self.schedule
+        timezone = self.timezone
+        enabled = self.enabled
+        script_path = self.script_path
+        is_flow = self.is_flow
         extra_perms = self.extra_perms.to_dict()
 
-        value = self.value
-        description = self.description
-        account = self.account
-        is_oauth = self.is_oauth
-        is_expired = self.is_expired
-        refresh_error = self.refresh_error
-        is_linked = self.is_linked
-        is_refreshed = self.is_refreshed
+        email = self.email
+        args: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.args, Unset):
+            args = self.args.to_dict()
+
+        error = self.error
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "workspace_id": workspace_id,
                 "path": path,
-                "is_secret": is_secret,
+                "edited_by": edited_by,
+                "edited_at": edited_at,
+                "schedule": schedule,
+                "timezone": timezone,
+                "enabled": enabled,
+                "script_path": script_path,
+                "is_flow": is_flow,
                 "extra_perms": extra_perms,
+                "email": email,
             }
         )
-        if value is not UNSET:
-            field_dict["value"] = value
-        if description is not UNSET:
-            field_dict["description"] = description
-        if account is not UNSET:
-            field_dict["account"] = account
-        if is_oauth is not UNSET:
-            field_dict["is_oauth"] = is_oauth
-        if is_expired is not UNSET:
-            field_dict["is_expired"] = is_expired
-        if refresh_error is not UNSET:
-            field_dict["refresh_error"] = refresh_error
-        if is_linked is not UNSET:
-            field_dict["is_linked"] = is_linked
-        if is_refreshed is not UNSET:
-            field_dict["is_refreshed"] = is_refreshed
+        if args is not UNSET:
+            field_dict["args"] = args
+        if error is not UNSET:
+            field_dict["error"] = error
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        workspace_id = d.pop("workspace_id")
-
         path = d.pop("path")
 
-        is_secret = d.pop("is_secret")
+        edited_by = d.pop("edited_by")
+
+        edited_at = isoparse(d.pop("edited_at"))
 
-        extra_perms = ListableVariableExtraPerms.from_dict(d.pop("extra_perms"))
+        schedule = d.pop("schedule")
 
-        value = d.pop("value", UNSET)
+        timezone = d.pop("timezone")
 
-        description = d.pop("description", UNSET)
+        enabled = d.pop("enabled")
 
-        account = d.pop("account", UNSET)
+        script_path = d.pop("script_path")
 
-        is_oauth = d.pop("is_oauth", UNSET)
+        is_flow = d.pop("is_flow")
 
-        is_expired = d.pop("is_expired", UNSET)
+        extra_perms = ScheduleExtraPerms.from_dict(d.pop("extra_perms"))
 
-        refresh_error = d.pop("refresh_error", UNSET)
+        email = d.pop("email")
 
-        is_linked = d.pop("is_linked", UNSET)
+        _args = d.pop("args", UNSET)
+        args: Union[Unset, ScheduleArgs]
+        if isinstance(_args, Unset):
+            args = UNSET
+        else:
+            args = ScheduleArgs.from_dict(_args)
 
-        is_refreshed = d.pop("is_refreshed", UNSET)
+        error = d.pop("error", UNSET)
 
-        listable_variable = cls(
-            workspace_id=workspace_id,
+        schedule = cls(
             path=path,
-            is_secret=is_secret,
+            edited_by=edited_by,
+            edited_at=edited_at,
+            schedule=schedule,
+            timezone=timezone,
+            enabled=enabled,
+            script_path=script_path,
+            is_flow=is_flow,
             extra_perms=extra_perms,
-            value=value,
-            description=description,
-            account=account,
-            is_oauth=is_oauth,
-            is_expired=is_expired,
-            refresh_error=refresh_error,
-            is_linked=is_linked,
-            is_refreshed=is_refreshed,
+            email=email,
+            args=args,
+            error=error,
         )
 
-        listable_variable.additional_properties = d
-        return listable_variable
+        schedule.additional_properties = d
+        return schedule
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/login.py` & `windmill_api-1.91.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/login_json_body.py` & `windmill_api-1.91.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.91.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.91.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/new_schedule.py` & `windmill_api-1.91.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/new_schedule_args.py` & `windmill_api-1.91.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/new_token.py` & `windmill_api-1.91.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.91.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/new_user.py` & `windmill_api-1.91.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow.py` & `windmill_api-1.91.0/windmill_api/models/create_draft_json_body.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,67 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_schema import OpenFlowSchema
-from ..models.open_flow_value import OpenFlowValue
+from ..models.create_draft_json_body_typ import CreateDraftJsonBodyTyp
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlow")
+T = TypeVar("T", bound="CreateDraftJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlow:
+class CreateDraftJsonBody:
     """
     Attributes:
-        summary (str):
-        value (OpenFlowValue):
-        description (Union[Unset, str]):
-        schema (Union[Unset, OpenFlowSchema]):
+        path (str):
+        typ (CreateDraftJsonBodyTyp):
+        value (Union[Unset, Any]):
     """
 
-    summary: str
-    value: OpenFlowValue
-    description: Union[Unset, str] = UNSET
-    schema: Union[Unset, OpenFlowSchema] = UNSET
+    path: str
+    typ: CreateDraftJsonBodyTyp
+    value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        summary = self.summary
-        value = self.value.to_dict()
+        path = self.path
+        typ = self.typ.value
 
-        description = self.description
-        schema: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.schema, Unset):
-            schema = self.schema.to_dict()
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "summary": summary,
-                "value": value,
+                "path": path,
+                "typ": typ,
             }
         )
-        if description is not UNSET:
-            field_dict["description"] = description
-        if schema is not UNSET:
-            field_dict["schema"] = schema
+        if value is not UNSET:
+            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        summary = d.pop("summary")
+        path = d.pop("path")
 
-        value = OpenFlowValue.from_dict(d.pop("value"))
+        typ = CreateDraftJsonBodyTyp(d.pop("typ"))
 
-        description = d.pop("description", UNSET)
+        value = d.pop("value", UNSET)
 
-        _schema = d.pop("schema", UNSET)
-        schema: Union[Unset, OpenFlowSchema]
-        if isinstance(_schema, Unset):
-            schema = UNSET
-        else:
-            schema = OpenFlowSchema.from_dict(_schema)
-
-        open_flow = cls(
-            summary=summary,
+        create_draft_json_body = cls(
+            path=path,
+            typ=typ,
             value=value,
-            description=description,
-            schema=schema,
         )
 
-        open_flow.additional_properties = d
-        return open_flow
+        create_draft_json_body.additional_properties = d
+        return create_draft_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_schema.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_value_failure_module import OpenFlowValueFailureModule
-from ..models.open_flow_value_modules_item import OpenFlowValueModulesItem
+from ..models.queued_job_raw_flow_failure_module import QueuedJobRawFlowFailureModule
+from ..models.queued_job_raw_flow_modules_item import QueuedJobRawFlowModulesItem
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValue")
+T = TypeVar("T", bound="QueuedJobRawFlow")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValue:
+class QueuedJobRawFlow:
     """
     Attributes:
-        modules (List[OpenFlowValueModulesItem]):
-        failure_module (Union[Unset, OpenFlowValueFailureModule]):
+        modules (List[QueuedJobRawFlowModulesItem]):
+        failure_module (Union[Unset, QueuedJobRawFlowFailureModule]):
         same_worker (Union[Unset, bool]):
     """
 
-    modules: List[OpenFlowValueModulesItem]
-    failure_module: Union[Unset, OpenFlowValueFailureModule] = UNSET
+    modules: List[QueuedJobRawFlowModulesItem]
+    failure_module: Union[Unset, QueuedJobRawFlowFailureModule] = UNSET
     same_worker: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         modules = []
         for modules_item_data in self.modules:
             modules_item = modules_item_data.to_dict()
@@ -52,35 +52,35 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         modules = []
         _modules = d.pop("modules")
         for modules_item_data in _modules:
-            modules_item = OpenFlowValueModulesItem.from_dict(modules_item_data)
+            modules_item = QueuedJobRawFlowModulesItem.from_dict(modules_item_data)
 
             modules.append(modules_item)
 
         _failure_module = d.pop("failure_module", UNSET)
-        failure_module: Union[Unset, OpenFlowValueFailureModule]
+        failure_module: Union[Unset, QueuedJobRawFlowFailureModule]
         if isinstance(_failure_module, Unset):
             failure_module = UNSET
         else:
-            failure_module = OpenFlowValueFailureModule.from_dict(_failure_module)
+            failure_module = QueuedJobRawFlowFailureModule.from_dict(_failure_module)
 
         same_worker = d.pop("same_worker", UNSET)
 
-        open_flow_value = cls(
+        queued_job_raw_flow = cls(
             modules=modules,
             failure_module=failure_module,
             same_worker=same_worker,
         )
 
-        open_flow_value.additional_properties = d
-        return open_flow_value
+        queued_job_raw_flow.additional_properties = d
+        return queued_job_raw_flow
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValueFailureModuleRetryConstant")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValueFailureModuleRetryConstant:
+class UpdateFlowJsonBodyValueFailureModuleRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        open_flow_value_failure_module_retry_constant = cls(
+        update_flow_json_body_value_failure_module_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        open_flow_value_failure_module_retry_constant.additional_properties = d
-        return open_flow_value_failure_module_retry_constant
+        update_flow_json_body_value_failure_module_retry_constant.additional_properties = d
+        return update_flow_json_body_value_failure_module_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValueFailureModuleRetryExponential")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValueFailureModuleRetryExponential:
+class RunFlowPreviewJsonBodyValueFailureModuleRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        open_flow_value_failure_module_retry_exponential = cls(
+        run_flow_preview_json_body_value_failure_module_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        open_flow_value_failure_module_retry_exponential.additional_properties = d
-        return open_flow_value_failure_module_retry_exponential
+        run_flow_preview_json_body_value_failure_module_retry_exponential.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_value_modules_item_retry import OpenFlowValueModulesItemRetry
-from ..models.open_flow_value_modules_item_sleep_type_0 import OpenFlowValueModulesItemSleepType0
-from ..models.open_flow_value_modules_item_sleep_type_1 import OpenFlowValueModulesItemSleepType1
-from ..models.open_flow_value_modules_item_stop_after_if import OpenFlowValueModulesItemStopAfterIf
-from ..models.open_flow_value_modules_item_suspend import OpenFlowValueModulesItemSuspend
+from ..models.open_flow_w_path_value_modules_item_retry import OpenFlowWPathValueModulesItemRetry
+from ..models.open_flow_w_path_value_modules_item_sleep_type_0 import OpenFlowWPathValueModulesItemSleepType0
+from ..models.open_flow_w_path_value_modules_item_sleep_type_1 import OpenFlowWPathValueModulesItemSleepType1
+from ..models.open_flow_w_path_value_modules_item_stop_after_if import OpenFlowWPathValueModulesItemStopAfterIf
+from ..models.open_flow_w_path_value_modules_item_suspend import OpenFlowWPathValueModulesItemSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValueModulesItem")
+T = TypeVar("T", bound="OpenFlowWPathValueModulesItem")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValueModulesItem:
+class OpenFlowWPathValueModulesItem:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, OpenFlowValueModulesItemStopAfterIf]):
-        sleep (Union[OpenFlowValueModulesItemSleepType0, OpenFlowValueModulesItemSleepType1, Unset]):
+        stop_after_if (Union[Unset, OpenFlowWPathValueModulesItemStopAfterIf]):
+        sleep (Union[OpenFlowWPathValueModulesItemSleepType0, OpenFlowWPathValueModulesItemSleepType1, Unset]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, OpenFlowValueModulesItemSuspend]):
-        retry (Union[Unset, OpenFlowValueModulesItemRetry]):
+        suspend (Union[Unset, OpenFlowWPathValueModulesItemSuspend]):
+        retry (Union[Unset, OpenFlowWPathValueModulesItemRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, OpenFlowValueModulesItemStopAfterIf] = UNSET
-    sleep: Union[OpenFlowValueModulesItemSleepType0, OpenFlowValueModulesItemSleepType1, Unset] = UNSET
+    stop_after_if: Union[Unset, OpenFlowWPathValueModulesItemStopAfterIf] = UNSET
+    sleep: Union[OpenFlowWPathValueModulesItemSleepType0, OpenFlowWPathValueModulesItemSleepType1, Unset] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, OpenFlowValueModulesItemSuspend] = UNSET
-    retry: Union[Unset, OpenFlowValueModulesItemRetry] = UNSET
+    suspend: Union[Unset, OpenFlowWPathValueModulesItemSuspend] = UNSET
+    retry: Union[Unset, OpenFlowWPathValueModulesItemRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, OpenFlowValueModulesItemSleepType0):
+        elif isinstance(self.sleep, OpenFlowWPathValueModulesItemSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -89,79 +89,79 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, OpenFlowValueModulesItemStopAfterIf]
+        stop_after_if: Union[Unset, OpenFlowWPathValueModulesItemStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = OpenFlowValueModulesItemStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = OpenFlowWPathValueModulesItemStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
-        ) -> Union[OpenFlowValueModulesItemSleepType0, OpenFlowValueModulesItemSleepType1, Unset]:
+        ) -> Union[OpenFlowWPathValueModulesItemSleepType0, OpenFlowWPathValueModulesItemSleepType1, Unset]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, OpenFlowValueModulesItemSleepType0]
+                sleep_type_0: Union[Unset, OpenFlowWPathValueModulesItemSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = OpenFlowValueModulesItemSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = OpenFlowWPathValueModulesItemSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, OpenFlowValueModulesItemSleepType1]
+            sleep_type_1: Union[Unset, OpenFlowWPathValueModulesItemSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = OpenFlowValueModulesItemSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = OpenFlowWPathValueModulesItemSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, OpenFlowValueModulesItemSuspend]
+        suspend: Union[Unset, OpenFlowWPathValueModulesItemSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = OpenFlowValueModulesItemSuspend.from_dict(_suspend)
+            suspend = OpenFlowWPathValueModulesItemSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, OpenFlowValueModulesItemRetry]
+        retry: Union[Unset, OpenFlowWPathValueModulesItemRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = OpenFlowValueModulesItemRetry.from_dict(_retry)
+            retry = OpenFlowWPathValueModulesItemRetry.from_dict(_retry)
 
-        open_flow_value_modules_item = cls(
+        open_flow_w_path_value_modules_item = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        open_flow_value_modules_item.additional_properties = d
-        return open_flow_value_modules_item
+        open_flow_w_path_value_modules_item.additional_properties = d
+        return open_flow_w_path_value_modules_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValueModulesItemRetryExponential")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValueModulesItemRetryExponential:
+class RunFlowPreviewJsonBodyValueModulesItemRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        open_flow_value_modules_item_retry_exponential = cls(
+        run_flow_preview_json_body_value_modules_item_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        open_flow_value_modules_item_retry_exponential.additional_properties = d
-        return open_flow_value_modules_item_retry_exponential
+        run_flow_preview_json_body_value_modules_item_retry_exponential.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_value_modules_item_sleep_type_0_type import OpenFlowValueModulesItemSleepType0Type
+from ..models.open_flow_w_path_value_modules_item_sleep_type_0_type import OpenFlowWPathValueModulesItemSleepType0Type
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValueModulesItemSleepType0")
+T = TypeVar("T", bound="OpenFlowWPathValueModulesItemSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValueModulesItemSleepType0:
+class OpenFlowWPathValueModulesItemSleepType0:
     """
     Attributes:
-        type (OpenFlowValueModulesItemSleepType0Type):
+        type (OpenFlowWPathValueModulesItemSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: OpenFlowValueModulesItemSleepType0Type
+    type: OpenFlowWPathValueModulesItemSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -36,25 +36,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = OpenFlowValueModulesItemSleepType0Type(d.pop("type"))
+        type = OpenFlowWPathValueModulesItemSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        open_flow_value_modules_item_sleep_type_0 = cls(
+        open_flow_w_path_value_modules_item_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        open_flow_value_modules_item_sleep_type_0.additional_properties = d
-        return open_flow_value_modules_item_sleep_type_0
+        open_flow_w_path_value_modules_item_sleep_type_0.additional_properties = d
+        return open_flow_w_path_value_modules_item_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowValueModulesItemSuspend")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowValueModulesItemSuspend:
+class UpdateFlowJsonBodyValueModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        open_flow_value_modules_item_suspend = cls(
+        update_flow_json_body_value_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        open_flow_value_modules_item_suspend.additional_properties = d
-        return open_flow_value_modules_item_suspend
+        update_flow_json_body_value_modules_item_suspend.additional_properties = d
+        return update_flow_json_body_value_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleRetryConstant")
+T = TypeVar("T", bound="QueuedJobRawFlowFailureModuleRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueFailureModuleRetryConstant:
+class QueuedJobRawFlowFailureModuleRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
+        multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
+    multiplier: Union[Unset, int] = UNSET
     seconds: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         attempts = self.attempts
+        multiplier = self.multiplier
         seconds = self.seconds
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if attempts is not UNSET:
             field_dict["attempts"] = attempts
+        if multiplier is not UNSET:
+            field_dict["multiplier"] = multiplier
         if seconds is not UNSET:
             field_dict["seconds"] = seconds
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
+        multiplier = d.pop("multiplier", UNSET)
+
         seconds = d.pop("seconds", UNSET)
 
-        open_flow_w_path_value_failure_module_retry_constant = cls(
+        queued_job_raw_flow_failure_module_retry_exponential = cls(
             attempts=attempts,
+            multiplier=multiplier,
             seconds=seconds,
         )
 
-        open_flow_w_path_value_failure_module_retry_constant.additional_properties = d
-        return open_flow_w_path_value_failure_module_retry_constant
+        queued_job_raw_flow_failure_module_retry_exponential.additional_properties = d
+        return queued_job_raw_flow_failure_module_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_w_path_value_failure_module_sleep_type_0_type import (
-    OpenFlowWPathValueFailureModuleSleepType0Type,
+from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_0_type import (
+    RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleSleepType0")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueFailureModuleSleepType0:
+class RunFlowPreviewJsonBodyValueFailureModuleSleepType0:
     """
     Attributes:
-        type (OpenFlowWPathValueFailureModuleSleepType0Type):
+        type (RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: OpenFlowWPathValueFailureModuleSleepType0Type
+    type: RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = OpenFlowWPathValueFailureModuleSleepType0Type(d.pop("type"))
+        type = RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        open_flow_w_path_value_failure_module_sleep_type_0 = cls(
+        run_flow_preview_json_body_value_failure_module_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        open_flow_w_path_value_failure_module_sleep_type_0.additional_properties = d
-        return open_flow_w_path_value_failure_module_sleep_type_0
+        run_flow_preview_json_body_value_failure_module_sleep_type_0.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.open_flow_w_path_value_failure_module_sleep_type_1_type import (
-    OpenFlowWPathValueFailureModuleSleepType1Type,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type import (
+    GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType1Type,
 )
 
-T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleSleepType1")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueFailureModuleSleepType1:
+class GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType1:
     """
     Attributes:
         expr (str):
-        type (OpenFlowWPathValueFailureModuleSleepType1Type):
+        type (GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType1Type):
     """
 
     expr: str
-    type: OpenFlowWPathValueFailureModuleSleepType1Type
+    type: GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = OpenFlowWPathValueFailureModuleSleepType1Type(d.pop("type"))
+        type = GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType1Type(d.pop("type"))
 
-        open_flow_w_path_value_failure_module_sleep_type_1 = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        open_flow_w_path_value_failure_module_sleep_type_1.additional_properties = d
-        return open_flow_w_path_value_failure_module_sleep_type_1
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleStopAfterIf")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueFailureModuleStopAfterIf:
+class RunFlowPreviewJsonBodyValueModulesItemStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        open_flow_w_path_value_failure_module_stop_after_if = cls(
+        run_flow_preview_json_body_value_modules_item_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        open_flow_w_path_value_failure_module_stop_after_if.additional_properties = d
-        return open_flow_w_path_value_failure_module_stop_after_if
+        run_flow_preview_json_body_value_modules_item_stop_after_if.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueFailureModuleSuspend")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleSuspend")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueFailureModuleSuspend:
+class UpdateFlowJsonBodyValueFailureModuleSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        open_flow_w_path_value_failure_module_suspend = cls(
+        update_flow_json_body_value_failure_module_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        open_flow_w_path_value_failure_module_suspend.additional_properties = d
-        return open_flow_w_path_value_failure_module_suspend
+        update_flow_json_body_value_failure_module_suspend.additional_properties = d
+        return update_flow_json_body_value_failure_module_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_w_path_value_modules_item_retry import OpenFlowWPathValueModulesItemRetry
-from ..models.open_flow_w_path_value_modules_item_sleep_type_0 import OpenFlowWPathValueModulesItemSleepType0
-from ..models.open_flow_w_path_value_modules_item_sleep_type_1 import OpenFlowWPathValueModulesItemSleepType1
-from ..models.open_flow_w_path_value_modules_item_stop_after_if import OpenFlowWPathValueModulesItemStopAfterIf
-from ..models.open_flow_w_path_value_modules_item_suspend import OpenFlowWPathValueModulesItemSuspend
+from ..models.update_flow_json_body_value_modules_item_retry import UpdateFlowJsonBodyValueModulesItemRetry
+from ..models.update_flow_json_body_value_modules_item_sleep_type_0 import UpdateFlowJsonBodyValueModulesItemSleepType0
+from ..models.update_flow_json_body_value_modules_item_sleep_type_1 import UpdateFlowJsonBodyValueModulesItemSleepType1
+from ..models.update_flow_json_body_value_modules_item_stop_after_if import (
+    UpdateFlowJsonBodyValueModulesItemStopAfterIf,
+)
+from ..models.update_flow_json_body_value_modules_item_suspend import UpdateFlowJsonBodyValueModulesItemSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueModulesItem")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItem")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueModulesItem:
+class UpdateFlowJsonBodyValueModulesItem:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, OpenFlowWPathValueModulesItemStopAfterIf]):
-        sleep (Union[OpenFlowWPathValueModulesItemSleepType0, OpenFlowWPathValueModulesItemSleepType1, Unset]):
+        stop_after_if (Union[Unset, UpdateFlowJsonBodyValueModulesItemStopAfterIf]):
+        sleep (Union[Unset, UpdateFlowJsonBodyValueModulesItemSleepType0,
+            UpdateFlowJsonBodyValueModulesItemSleepType1]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, OpenFlowWPathValueModulesItemSuspend]):
-        retry (Union[Unset, OpenFlowWPathValueModulesItemRetry]):
+        suspend (Union[Unset, UpdateFlowJsonBodyValueModulesItemSuspend]):
+        retry (Union[Unset, UpdateFlowJsonBodyValueModulesItemRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, OpenFlowWPathValueModulesItemStopAfterIf] = UNSET
-    sleep: Union[OpenFlowWPathValueModulesItemSleepType0, OpenFlowWPathValueModulesItemSleepType1, Unset] = UNSET
+    stop_after_if: Union[Unset, UpdateFlowJsonBodyValueModulesItemStopAfterIf] = UNSET
+    sleep: Union[
+        Unset, UpdateFlowJsonBodyValueModulesItemSleepType0, UpdateFlowJsonBodyValueModulesItemSleepType1
+    ] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, OpenFlowWPathValueModulesItemSuspend] = UNSET
-    retry: Union[Unset, OpenFlowWPathValueModulesItemRetry] = UNSET
+    suspend: Union[Unset, UpdateFlowJsonBodyValueModulesItemSuspend] = UNSET
+    retry: Union[Unset, UpdateFlowJsonBodyValueModulesItemRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, OpenFlowWPathValueModulesItemSleepType0):
+        elif isinstance(self.sleep, UpdateFlowJsonBodyValueModulesItemSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -89,79 +94,79 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, OpenFlowWPathValueModulesItemStopAfterIf]
+        stop_after_if: Union[Unset, UpdateFlowJsonBodyValueModulesItemStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = OpenFlowWPathValueModulesItemStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = UpdateFlowJsonBodyValueModulesItemStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
-        ) -> Union[OpenFlowWPathValueModulesItemSleepType0, OpenFlowWPathValueModulesItemSleepType1, Unset]:
+        ) -> Union[Unset, UpdateFlowJsonBodyValueModulesItemSleepType0, UpdateFlowJsonBodyValueModulesItemSleepType1]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, OpenFlowWPathValueModulesItemSleepType0]
+                sleep_type_0: Union[Unset, UpdateFlowJsonBodyValueModulesItemSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = OpenFlowWPathValueModulesItemSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = UpdateFlowJsonBodyValueModulesItemSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, OpenFlowWPathValueModulesItemSleepType1]
+            sleep_type_1: Union[Unset, UpdateFlowJsonBodyValueModulesItemSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = OpenFlowWPathValueModulesItemSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = UpdateFlowJsonBodyValueModulesItemSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, OpenFlowWPathValueModulesItemSuspend]
+        suspend: Union[Unset, UpdateFlowJsonBodyValueModulesItemSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = OpenFlowWPathValueModulesItemSuspend.from_dict(_suspend)
+            suspend = UpdateFlowJsonBodyValueModulesItemSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, OpenFlowWPathValueModulesItemRetry]
+        retry: Union[Unset, UpdateFlowJsonBodyValueModulesItemRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = OpenFlowWPathValueModulesItemRetry.from_dict(_retry)
+            retry = UpdateFlowJsonBodyValueModulesItemRetry.from_dict(_retry)
 
-        open_flow_w_path_value_modules_item = cls(
+        update_flow_json_body_value_modules_item = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        open_flow_w_path_value_modules_item.additional_properties = d
-        return open_flow_w_path_value_modules_item
+        update_flow_json_body_value_modules_item.additional_properties = d
+        return update_flow_json_body_value_modules_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueModulesItemRetryExponential")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueModulesItemRetryExponential:
+class GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        open_flow_w_path_value_modules_item_retry_exponential = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        open_flow_w_path_value_modules_item_retry_exponential.additional_properties = d
-        return open_flow_w_path_value_modules_item_retry_exponential
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.open_flow_w_path_value_modules_item_sleep_type_0_type import OpenFlowWPathValueModulesItemSleepType0Type
+from ..models.raw_script_input_transforms_additional_property_type_0_type import (
+    RawScriptInputTransformsAdditionalPropertyType0Type,
+)
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueModulesItemSleepType0")
+T = TypeVar("T", bound="RawScriptInputTransformsAdditionalPropertyType0")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueModulesItemSleepType0:
+class RawScriptInputTransformsAdditionalPropertyType0:
     """
     Attributes:
-        type (OpenFlowWPathValueModulesItemSleepType0Type):
+        type (RawScriptInputTransformsAdditionalPropertyType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: OpenFlowWPathValueModulesItemSleepType0Type
+    type: RawScriptInputTransformsAdditionalPropertyType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -36,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = OpenFlowWPathValueModulesItemSleepType0Type(d.pop("type"))
+        type = RawScriptInputTransformsAdditionalPropertyType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        open_flow_w_path_value_modules_item_sleep_type_0 = cls(
+        raw_script_input_transforms_additional_property_type_0 = cls(
             type=type,
             value=value,
         )
 
-        open_flow_w_path_value_modules_item_sleep_type_0.additional_properties = d
-        return open_flow_w_path_value_modules_item_sleep_type_0
+        raw_script_input_transforms_additional_property_type_0.additional_properties = d
+        return raw_script_input_transforms_additional_property_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OpenFlowWPathValueModulesItemSuspend")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueFailureModuleSuspend")
 
 
 @attr.s(auto_attribs=True)
-class OpenFlowWPathValueModulesItemSuspend:
+class GetFlowByPathWithDraftResponse200DraftValueFailureModuleSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        open_flow_w_path_value_modules_item_suspend = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        open_flow_w_path_value_modules_item_suspend.additional_properties = d
-        return open_flow_w_path_value_modules_item_suspend
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/path_flow.py` & `windmill_api-1.91.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.91.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_script.py` & `windmill_api-1.91.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.91.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.91.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.91.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/policy.py` & `windmill_api-1.91.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/preview.py` & `windmill_api-1.91.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/preview_args.py` & `windmill_api-1.91.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.91.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.91.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job.py` & `windmill_api-1.91.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_args.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.queued_job_raw_flow_failure_module import QueuedJobRawFlowFailureModule
-from ..models.queued_job_raw_flow_modules_item import QueuedJobRawFlowModulesItem
+from ..models.run_flow_preview_json_body_value_failure_module import RunFlowPreviewJsonBodyValueFailureModule
+from ..models.run_flow_preview_json_body_value_modules_item import RunFlowPreviewJsonBodyValueModulesItem
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="QueuedJobRawFlow")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValue")
 
 
 @attr.s(auto_attribs=True)
-class QueuedJobRawFlow:
+class RunFlowPreviewJsonBodyValue:
     """
     Attributes:
-        modules (List[QueuedJobRawFlowModulesItem]):
-        failure_module (Union[Unset, QueuedJobRawFlowFailureModule]):
+        modules (List[RunFlowPreviewJsonBodyValueModulesItem]):
+        failure_module (Union[Unset, RunFlowPreviewJsonBodyValueFailureModule]):
         same_worker (Union[Unset, bool]):
     """
 
-    modules: List[QueuedJobRawFlowModulesItem]
-    failure_module: Union[Unset, QueuedJobRawFlowFailureModule] = UNSET
+    modules: List[RunFlowPreviewJsonBodyValueModulesItem]
+    failure_module: Union[Unset, RunFlowPreviewJsonBodyValueFailureModule] = UNSET
     same_worker: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         modules = []
         for modules_item_data in self.modules:
             modules_item = modules_item_data.to_dict()
@@ -52,35 +52,35 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         modules = []
         _modules = d.pop("modules")
         for modules_item_data in _modules:
-            modules_item = QueuedJobRawFlowModulesItem.from_dict(modules_item_data)
+            modules_item = RunFlowPreviewJsonBodyValueModulesItem.from_dict(modules_item_data)
 
             modules.append(modules_item)
 
         _failure_module = d.pop("failure_module", UNSET)
-        failure_module: Union[Unset, QueuedJobRawFlowFailureModule]
+        failure_module: Union[Unset, RunFlowPreviewJsonBodyValueFailureModule]
         if isinstance(_failure_module, Unset):
             failure_module = UNSET
         else:
-            failure_module = QueuedJobRawFlowFailureModule.from_dict(_failure_module)
+            failure_module = RunFlowPreviewJsonBodyValueFailureModule.from_dict(_failure_module)
 
         same_worker = d.pop("same_worker", UNSET)
 
-        queued_job_raw_flow = cls(
+        run_flow_preview_json_body_value = cls(
             modules=modules,
             failure_module=failure_module,
             same_worker=same_worker,
         )
 
-        queued_job_raw_flow.additional_properties = d
-        return queued_job_raw_flow
+        run_flow_preview_json_body_value.additional_properties = d
+        return run_flow_preview_json_body_value
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/retry_exponential.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="QueuedJobRawFlowFailureModuleRetryExponential")
+T = TypeVar("T", bound="RetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class QueuedJobRawFlowFailureModuleRetryExponential:
+class RetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        queued_job_raw_flow_failure_module_retry_exponential = cls(
+        retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        queued_job_raw_flow_failure_module_retry_exponential.additional_properties = d
-        return queued_job_raw_flow_failure_module_retry_exponential
+        retry_exponential.additional_properties = d
+        return retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="QueuedJobRawFlowFailureModuleStopAfterIf")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class QueuedJobRawFlowFailureModuleStopAfterIf:
+class RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        queued_job_raw_flow_failure_module_stop_after_if = cls(
+        run_flow_preview_json_body_value_failure_module_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        queued_job_raw_flow_failure_module_stop_after_if.additional_properties = d
-        return queued_job_raw_flow_failure_module_stop_after_if
+        run_flow_preview_json_body_value_failure_module_stop_after_if.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="QueuedJobRawFlowFailureModuleSuspend")
+T = TypeVar("T", bound="QueuedJobRawFlowModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class QueuedJobRawFlowFailureModuleSuspend:
+class QueuedJobRawFlowModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        queued_job_raw_flow_failure_module_suspend = cls(
+        queued_job_raw_flow_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        queued_job_raw_flow_failure_module_suspend.additional_properties = d
-        return queued_job_raw_flow_failure_module_suspend
+        queued_job_raw_flow_modules_item_suspend.additional_properties = d
+        return queued_job_raw_flow_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="QueuedJobRawFlowModulesItemStopAfterIf")
+T = TypeVar("T", bound="UpdateResourceValueJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class QueuedJobRawFlowModulesItemStopAfterIf:
+class UpdateResourceValueJsonBody:
     """
     Attributes:
-        expr (str):
-        skip_if_stopped (Union[Unset, bool]):
+        value (Union[Unset, Any]):
     """
 
-    expr: str
-    skip_if_stopped: Union[Unset, bool] = UNSET
+    value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expr = self.expr
-        skip_if_stopped = self.skip_if_stopped
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "expr": expr,
-            }
-        )
-        if skip_if_stopped is not UNSET:
-            field_dict["skip_if_stopped"] = skip_if_stopped
+        field_dict.update({})
+        if value is not UNSET:
+            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expr = d.pop("expr")
-
-        skip_if_stopped = d.pop("skip_if_stopped", UNSET)
+        value = d.pop("value", UNSET)
 
-        queued_job_raw_flow_modules_item_stop_after_if = cls(
-            expr=expr,
-            skip_if_stopped=skip_if_stopped,
+        update_resource_value_json_body = cls(
+            value=value,
         )
 
-        queued_job_raw_flow_modules_item_stop_after_if.additional_properties = d
-        return queued_job_raw_flow_modules_item_stop_after_if
+        update_resource_value_json_body.additional_properties = d
+        return update_resource_value_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="QueuedJobRawFlowModulesItemSuspend")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class QueuedJobRawFlowModulesItemSuspend:
+class GetFlowByPathWithDraftResponse200DraftValueModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        queued_job_raw_flow_modules_item_suspend = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        queued_job_raw_flow_modules_item_suspend.additional_properties = d
-        return queued_job_raw_flow_modules_item_suspend
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/raw_script.py` & `windmill_api-1.91.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.raw_script_input_transforms_additional_property_type_0_type import (
-    RawScriptInputTransformsAdditionalPropertyType0Type,
+from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_1_type import (
+    RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type,
 )
-from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RawScriptInputTransformsAdditionalPropertyType0")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class RawScriptInputTransformsAdditionalPropertyType0:
+class RunFlowPreviewJsonBodyValueFailureModuleSleepType1:
     """
     Attributes:
-        type (RawScriptInputTransformsAdditionalPropertyType0Type):
-        value (Union[Unset, Any]):
+        expr (str):
+        type (RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type):
     """
 
-    type: RawScriptInputTransformsAdditionalPropertyType0Type
-    value: Union[Unset, Any] = UNSET
+    expr: str
+    type: RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        expr = self.expr
         type = self.type.value
 
-        value = self.value
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "expr": expr,
                 "type": type,
             }
         )
-        if value is not UNSET:
-            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = RawScriptInputTransformsAdditionalPropertyType0Type(d.pop("type"))
+        expr = d.pop("expr")
 
-        value = d.pop("value", UNSET)
+        type = RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type(d.pop("type"))
 
-        raw_script_input_transforms_additional_property_type_0 = cls(
+        run_flow_preview_json_body_value_failure_module_sleep_type_1 = cls(
+            expr=expr,
             type=type,
-            value=value,
         )
 
-        raw_script_input_transforms_additional_property_type_0.additional_properties = d
-        return raw_script_input_transforms_additional_property_type_0
+        run_flow_preview_json_body_value_failure_module_sleep_type_1.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.91.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.91.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.91.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.91.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.91.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/resource.py` & `windmill_api-1.91.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/resource_type.py` & `windmill_api-1.91.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.91.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.91.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/retry.py` & `windmill_api-1.91.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RetryExponential")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemRetryExponential")
 
 
 @attr.s(auto_attribs=True)
-class RetryExponential:
+class UpdateFlowJsonBodyValueModulesItemRetryExponential:
     """
     Attributes:
         attempts (Union[Unset, int]):
         multiplier (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
@@ -43,22 +43,22 @@
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         multiplier = d.pop("multiplier", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        retry_exponential = cls(
+        update_flow_json_body_value_modules_item_retry_exponential = cls(
             attempts=attempts,
             multiplier=multiplier,
             seconds=seconds,
         )
 
-        retry_exponential.additional_properties = d
-        return retry_exponential
+        update_flow_json_body_value_modules_item_retry_exponential.additional_properties = d
+        return update_flow_json_body_value_modules_item_retry_exponential
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_failure_module import RunFlowPreviewJsonBodyValueFailureModule
-from ..models.run_flow_preview_json_body_value_modules_item import RunFlowPreviewJsonBodyValueModulesItem
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_failure_module import (
+    GetFlowByPathWithDraftResponse200DraftValueFailureModule,
+)
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_modules_item import (
+    GetFlowByPathWithDraftResponse200DraftValueModulesItem,
+)
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValue")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValue")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValue:
+class GetFlowByPathWithDraftResponse200DraftValue:
     """
     Attributes:
-        modules (List[RunFlowPreviewJsonBodyValueModulesItem]):
-        failure_module (Union[Unset, RunFlowPreviewJsonBodyValueFailureModule]):
+        modules (List[GetFlowByPathWithDraftResponse200DraftValueModulesItem]):
+        failure_module (Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModule]):
         same_worker (Union[Unset, bool]):
     """
 
-    modules: List[RunFlowPreviewJsonBodyValueModulesItem]
-    failure_module: Union[Unset, RunFlowPreviewJsonBodyValueFailureModule] = UNSET
+    modules: List[GetFlowByPathWithDraftResponse200DraftValueModulesItem]
+    failure_module: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModule] = UNSET
     same_worker: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         modules = []
         for modules_item_data in self.modules:
             modules_item = modules_item_data.to_dict()
@@ -52,35 +56,35 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         modules = []
         _modules = d.pop("modules")
         for modules_item_data in _modules:
-            modules_item = RunFlowPreviewJsonBodyValueModulesItem.from_dict(modules_item_data)
+            modules_item = GetFlowByPathWithDraftResponse200DraftValueModulesItem.from_dict(modules_item_data)
 
             modules.append(modules_item)
 
         _failure_module = d.pop("failure_module", UNSET)
-        failure_module: Union[Unset, RunFlowPreviewJsonBodyValueFailureModule]
+        failure_module: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueFailureModule]
         if isinstance(_failure_module, Unset):
             failure_module = UNSET
         else:
-            failure_module = RunFlowPreviewJsonBodyValueFailureModule.from_dict(_failure_module)
+            failure_module = GetFlowByPathWithDraftResponse200DraftValueFailureModule.from_dict(_failure_module)
 
         same_worker = d.pop("same_worker", UNSET)
 
-        run_flow_preview_json_body_value = cls(
+        get_flow_by_path_with_draft_response_200_draft_value = cls(
             modules=modules,
             failure_module=failure_module,
             same_worker=same_worker,
         )
 
-        run_flow_preview_json_body_value.additional_properties = d
-        return run_flow_preview_json_body_value
+        get_flow_by_path_with_draft_response_200_draft_value.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_failure_module_retry import RunFlowPreviewJsonBodyValueFailureModuleRetry
-from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_0 import (
-    RunFlowPreviewJsonBodyValueFailureModuleSleepType0,
+from ..models.update_flow_json_body_value_failure_module_retry import UpdateFlowJsonBodyValueFailureModuleRetry
+from ..models.update_flow_json_body_value_failure_module_sleep_type_0 import (
+    UpdateFlowJsonBodyValueFailureModuleSleepType0,
 )
-from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_1 import (
-    RunFlowPreviewJsonBodyValueFailureModuleSleepType1,
+from ..models.update_flow_json_body_value_failure_module_sleep_type_1 import (
+    UpdateFlowJsonBodyValueFailureModuleSleepType1,
 )
-from ..models.run_flow_preview_json_body_value_failure_module_stop_after_if import (
-    RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf,
-)
-from ..models.run_flow_preview_json_body_value_failure_module_suspend import (
-    RunFlowPreviewJsonBodyValueFailureModuleSuspend,
+from ..models.update_flow_json_body_value_failure_module_stop_after_if import (
+    UpdateFlowJsonBodyValueFailureModuleStopAfterIf,
 )
+from ..models.update_flow_json_body_value_failure_module_suspend import UpdateFlowJsonBodyValueFailureModuleSuspend
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModule")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModule")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModule:
+class UpdateFlowJsonBodyValueFailureModule:
     """
     Attributes:
         id (str):
         value (Any):
-        stop_after_if (Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf]):
-        sleep (Union[RunFlowPreviewJsonBodyValueFailureModuleSleepType0,
-            RunFlowPreviewJsonBodyValueFailureModuleSleepType1, Unset]):
+        stop_after_if (Union[Unset, UpdateFlowJsonBodyValueFailureModuleStopAfterIf]):
+        sleep (Union[Unset, UpdateFlowJsonBodyValueFailureModuleSleepType0,
+            UpdateFlowJsonBodyValueFailureModuleSleepType1]):
         summary (Union[Unset, str]):
-        suspend (Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSuspend]):
-        retry (Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleRetry]):
+        suspend (Union[Unset, UpdateFlowJsonBodyValueFailureModuleSuspend]):
+        retry (Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetry]):
     """
 
     id: str
     value: Any
-    stop_after_if: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf] = UNSET
+    stop_after_if: Union[Unset, UpdateFlowJsonBodyValueFailureModuleStopAfterIf] = UNSET
     sleep: Union[
-        RunFlowPreviewJsonBodyValueFailureModuleSleepType0, RunFlowPreviewJsonBodyValueFailureModuleSleepType1, Unset
+        Unset, UpdateFlowJsonBodyValueFailureModuleSleepType0, UpdateFlowJsonBodyValueFailureModuleSleepType1
     ] = UNSET
     summary: Union[Unset, str] = UNSET
-    suspend: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSuspend] = UNSET
-    retry: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleRetry] = UNSET
+    suspend: Union[Unset, UpdateFlowJsonBodyValueFailureModuleSuspend] = UNSET
+    retry: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetry] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         value = self.value
         stop_after_if: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.stop_after_if, Unset):
             stop_after_if = self.stop_after_if.to_dict()
 
         sleep: Union[Dict[str, Any], Unset]
         if isinstance(self.sleep, Unset):
             sleep = UNSET
 
-        elif isinstance(self.sleep, RunFlowPreviewJsonBodyValueFailureModuleSleepType0):
+        elif isinstance(self.sleep, UpdateFlowJsonBodyValueFailureModuleSleepType0):
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
                 sleep = self.sleep.to_dict()
 
         else:
             sleep = UNSET
             if not isinstance(self.sleep, Unset):
@@ -100,83 +98,81 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         value = d.pop("value")
 
         _stop_after_if = d.pop("stop_after_if", UNSET)
-        stop_after_if: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf]
+        stop_after_if: Union[Unset, UpdateFlowJsonBodyValueFailureModuleStopAfterIf]
         if isinstance(_stop_after_if, Unset):
             stop_after_if = UNSET
         else:
-            stop_after_if = RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf.from_dict(_stop_after_if)
+            stop_after_if = UpdateFlowJsonBodyValueFailureModuleStopAfterIf.from_dict(_stop_after_if)
 
         def _parse_sleep(
             data: object,
         ) -> Union[
-            RunFlowPreviewJsonBodyValueFailureModuleSleepType0,
-            RunFlowPreviewJsonBodyValueFailureModuleSleepType1,
-            Unset,
+            Unset, UpdateFlowJsonBodyValueFailureModuleSleepType0, UpdateFlowJsonBodyValueFailureModuleSleepType1
         ]:
             if isinstance(data, Unset):
                 return data
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
                 _sleep_type_0 = data
-                sleep_type_0: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSleepType0]
+                sleep_type_0: Union[Unset, UpdateFlowJsonBodyValueFailureModuleSleepType0]
                 if isinstance(_sleep_type_0, Unset):
                     sleep_type_0 = UNSET
                 else:
-                    sleep_type_0 = RunFlowPreviewJsonBodyValueFailureModuleSleepType0.from_dict(_sleep_type_0)
+                    sleep_type_0 = UpdateFlowJsonBodyValueFailureModuleSleepType0.from_dict(_sleep_type_0)
 
                 return sleep_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
             _sleep_type_1 = data
-            sleep_type_1: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSleepType1]
+            sleep_type_1: Union[Unset, UpdateFlowJsonBodyValueFailureModuleSleepType1]
             if isinstance(_sleep_type_1, Unset):
                 sleep_type_1 = UNSET
             else:
-                sleep_type_1 = RunFlowPreviewJsonBodyValueFailureModuleSleepType1.from_dict(_sleep_type_1)
+                sleep_type_1 = UpdateFlowJsonBodyValueFailureModuleSleepType1.from_dict(_sleep_type_1)
 
             return sleep_type_1
 
         sleep = _parse_sleep(d.pop("sleep", UNSET))
 
         summary = d.pop("summary", UNSET)
 
         _suspend = d.pop("suspend", UNSET)
-        suspend: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleSuspend]
+        suspend: Union[Unset, UpdateFlowJsonBodyValueFailureModuleSuspend]
         if isinstance(_suspend, Unset):
             suspend = UNSET
         else:
-            suspend = RunFlowPreviewJsonBodyValueFailureModuleSuspend.from_dict(_suspend)
+            suspend = UpdateFlowJsonBodyValueFailureModuleSuspend.from_dict(_suspend)
 
         _retry = d.pop("retry", UNSET)
-        retry: Union[Unset, RunFlowPreviewJsonBodyValueFailureModuleRetry]
+        retry: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetry]
         if isinstance(_retry, Unset):
             retry = UNSET
         else:
-            retry = RunFlowPreviewJsonBodyValueFailureModuleRetry.from_dict(_retry)
+            retry = UpdateFlowJsonBodyValueFailureModuleRetry.from_dict(_retry)
 
-        run_flow_preview_json_body_value_failure_module = cls(
+        update_flow_json_body_value_failure_module = cls(
             id=id,
             value=value,
             stop_after_if=stop_after_if,
             sleep=sleep,
             summary=summary,
             suspend=suspend,
             retry=retry,
         )
 
-        run_flow_preview_json_body_value_failure_module.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module
+        update_flow_json_body_value_failure_module.additional_properties = d
+        return update_flow_json_body_value_failure_module
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleRetryConstant")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModuleRetryConstant:
+class UpdateFlowJsonBodyValueModulesItemRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        run_flow_preview_json_body_value_failure_module_retry_constant = cls(
+        update_flow_json_body_value_modules_item_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        run_flow_preview_json_body_value_failure_module_retry_constant.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module_retry_constant
+        update_flow_json_body_value_modules_item_retry_constant.additional_properties = d
+        return update_flow_json_body_value_modules_item_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,56 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleRetryExponential")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleSuspend")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModuleRetryExponential:
+class RunFlowPreviewJsonBodyValueFailureModuleSuspend:
     """
     Attributes:
-        attempts (Union[Unset, int]):
-        multiplier (Union[Unset, int]):
-        seconds (Union[Unset, int]):
+        required_events (Union[Unset, int]):
+        timeout (Union[Unset, int]):
     """
 
-    attempts: Union[Unset, int] = UNSET
-    multiplier: Union[Unset, int] = UNSET
-    seconds: Union[Unset, int] = UNSET
+    required_events: Union[Unset, int] = UNSET
+    timeout: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        attempts = self.attempts
-        multiplier = self.multiplier
-        seconds = self.seconds
+        required_events = self.required_events
+        timeout = self.timeout
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if attempts is not UNSET:
-            field_dict["attempts"] = attempts
-        if multiplier is not UNSET:
-            field_dict["multiplier"] = multiplier
-        if seconds is not UNSET:
-            field_dict["seconds"] = seconds
+        if required_events is not UNSET:
+            field_dict["required_events"] = required_events
+        if timeout is not UNSET:
+            field_dict["timeout"] = timeout
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        attempts = d.pop("attempts", UNSET)
+        required_events = d.pop("required_events", UNSET)
 
-        multiplier = d.pop("multiplier", UNSET)
+        timeout = d.pop("timeout", UNSET)
 
-        seconds = d.pop("seconds", UNSET)
-
-        run_flow_preview_json_body_value_failure_module_retry_exponential = cls(
-            attempts=attempts,
-            multiplier=multiplier,
-            seconds=seconds,
+        run_flow_preview_json_body_value_failure_module_suspend = cls(
+            required_events=required_events,
+            timeout=timeout,
         )
 
-        run_flow_preview_json_body_value_failure_module_retry_exponential.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module_retry_exponential
+        run_flow_preview_json_body_value_failure_module_suspend.additional_properties = d
+        return run_flow_preview_json_body_value_failure_module_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_0_type import (
-    RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type,
-)
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleSleepType0")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueFailureModuleStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModuleSleepType0:
+class GetFlowByPathWithDraftResponse200DraftValueFailureModuleStopAfterIf:
     """
     Attributes:
-        type (RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type):
-        value (Union[Unset, Any]):
+        expr (str):
+        skip_if_stopped (Union[Unset, bool]):
     """
 
-    type: RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type
-    value: Union[Unset, Any] = UNSET
+    expr: str
+    skip_if_stopped: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        type = self.type.value
-
-        value = self.value
+        expr = self.expr
+        skip_if_stopped = self.skip_if_stopped
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "type": type,
+                "expr": expr,
             }
         )
-        if value is not UNSET:
-            field_dict["value"] = value
+        if skip_if_stopped is not UNSET:
+            field_dict["skip_if_stopped"] = skip_if_stopped
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = RunFlowPreviewJsonBodyValueFailureModuleSleepType0Type(d.pop("type"))
+        expr = d.pop("expr")
 
-        value = d.pop("value", UNSET)
+        skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        run_flow_preview_json_body_value_failure_module_sleep_type_0 = cls(
-            type=type,
-            value=value,
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if = cls(
+            expr=expr,
+            skip_if_stopped=skip_if_stopped,
         )
 
-        run_flow_preview_json_body_value_failure_module_sleep_type_0.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module_sleep_type_0
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_failure_module_sleep_type_1_type import (
-    RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type import (
+    GetFlowByPathWithDraftResponse200DraftValueModulesItemSleepType1Type,
 )
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleSleepType1")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueModulesItemSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModuleSleepType1:
+class GetFlowByPathWithDraftResponse200DraftValueModulesItemSleepType1:
     """
     Attributes:
         expr (str):
-        type (RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type):
+        type (GetFlowByPathWithDraftResponse200DraftValueModulesItemSleepType1Type):
     """
 
     expr: str
-    type: RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type
+    type: GetFlowByPathWithDraftResponse200DraftValueModulesItemSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = RunFlowPreviewJsonBodyValueFailureModuleSleepType1Type(d.pop("type"))
+        type = GetFlowByPathWithDraftResponse200DraftValueModulesItemSleepType1Type(d.pop("type"))
 
-        run_flow_preview_json_body_value_failure_module_sleep_type_1 = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        run_flow_preview_json_body_value_failure_module_sleep_type_1.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module_sleep_type_1
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,35 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf")
+T = TypeVar("T", bound="GetAppByPathWithDraftResponse200PolicyTriggerablesAdditionalProperty")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModuleStopAfterIf:
-    """
-    Attributes:
-        expr (str):
-        skip_if_stopped (Union[Unset, bool]):
-    """
+class GetAppByPathWithDraftResponse200PolicyTriggerablesAdditionalProperty:
+    """ """
 
-    expr: str
-    skip_if_stopped: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expr = self.expr
-        skip_if_stopped = self.skip_if_stopped
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "expr": expr,
-            }
-        )
-        if skip_if_stopped is not UNSET:
-            field_dict["skip_if_stopped"] = skip_if_stopped
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expr = d.pop("expr")
-
-        skip_if_stopped = d.pop("skip_if_stopped", UNSET)
-
-        run_flow_preview_json_body_value_failure_module_stop_after_if = cls(
-            expr=expr,
-            skip_if_stopped=skip_if_stopped,
-        )
+        get_app_by_path_with_draft_response_200_policy_triggerables_additional_property = cls()
 
-        run_flow_preview_json_body_value_failure_module_stop_after_if.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module_stop_after_if
+        get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.additional_properties = d
+        return get_app_by_path_with_draft_response_200_policy_triggerables_additional_property
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueFailureModuleSuspend")
+T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemSuspend")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueFailureModuleSuspend:
+class RunFlowPreviewJsonBodyValueModulesItemSuspend:
     """
     Attributes:
         required_events (Union[Unset, int]):
         timeout (Union[Unset, int]):
     """
 
     required_events: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         required_events = d.pop("required_events", UNSET)
 
         timeout = d.pop("timeout", UNSET)
 
-        run_flow_preview_json_body_value_failure_module_suspend = cls(
+        run_flow_preview_json_body_value_modules_item_suspend = cls(
             required_events=required_events,
             timeout=timeout,
         )
 
-        run_flow_preview_json_body_value_failure_module_suspend.additional_properties = d
-        return run_flow_preview_json_body_value_failure_module_suspend
+        run_flow_preview_json_body_value_modules_item_suspend.additional_properties = d
+        return run_flow_preview_json_body_value_modules_item_suspend
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_modules_item_retry_constant import (
-    RunFlowPreviewJsonBodyValueModulesItemRetryConstant,
+from ..models.update_flow_json_body_value_modules_item_retry_constant import (
+    UpdateFlowJsonBodyValueModulesItemRetryConstant,
 )
-from ..models.run_flow_preview_json_body_value_modules_item_retry_exponential import (
-    RunFlowPreviewJsonBodyValueModulesItemRetryExponential,
+from ..models.update_flow_json_body_value_modules_item_retry_exponential import (
+    UpdateFlowJsonBodyValueModulesItemRetryExponential,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemRetry")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemRetry")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemRetry:
+class UpdateFlowJsonBodyValueModulesItemRetry:
     """
     Attributes:
-        constant (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryConstant]):
-        exponential (Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryExponential]):
+        constant (Union[Unset, UpdateFlowJsonBodyValueModulesItemRetryConstant]):
+        exponential (Union[Unset, UpdateFlowJsonBodyValueModulesItemRetryExponential]):
     """
 
-    constant: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryConstant] = UNSET
-    exponential: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryExponential] = UNSET
+    constant: Union[Unset, UpdateFlowJsonBodyValueModulesItemRetryConstant] = UNSET
+    exponential: Union[Unset, UpdateFlowJsonBodyValueModulesItemRetryExponential] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         constant: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.constant, Unset):
             constant = self.constant.to_dict()
 
@@ -44,34 +44,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryConstant]
+        constant: Union[Unset, UpdateFlowJsonBodyValueModulesItemRetryConstant]
         if isinstance(_constant, Unset):
             constant = UNSET
         else:
-            constant = RunFlowPreviewJsonBodyValueModulesItemRetryConstant.from_dict(_constant)
+            constant = UpdateFlowJsonBodyValueModulesItemRetryConstant.from_dict(_constant)
 
         _exponential = d.pop("exponential", UNSET)
-        exponential: Union[Unset, RunFlowPreviewJsonBodyValueModulesItemRetryExponential]
+        exponential: Union[Unset, UpdateFlowJsonBodyValueModulesItemRetryExponential]
         if isinstance(_exponential, Unset):
             exponential = UNSET
         else:
-            exponential = RunFlowPreviewJsonBodyValueModulesItemRetryExponential.from_dict(_exponential)
+            exponential = UpdateFlowJsonBodyValueModulesItemRetryExponential.from_dict(_exponential)
 
-        run_flow_preview_json_body_value_modules_item_retry = cls(
+        update_flow_json_body_value_modules_item_retry = cls(
             constant=constant,
             exponential=exponential,
         )
 
-        run_flow_preview_json_body_value_modules_item_retry.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_retry
+        update_flow_json_body_value_modules_item_retry.additional_properties = d
+        return update_flow_json_body_value_modules_item_retry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemRetryConstant")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemRetryConstant:
+class GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant:
     """
     Attributes:
         attempts (Union[Unset, int]):
         seconds (Union[Unset, int]):
     """
 
     attempts: Union[Unset, int] = UNSET
@@ -36,21 +36,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         attempts = d.pop("attempts", UNSET)
 
         seconds = d.pop("seconds", UNSET)
 
-        run_flow_preview_json_body_value_modules_item_retry_constant = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant = cls(
             attempts=attempts,
             seconds=seconds,
         )
 
-        run_flow_preview_json_body_value_modules_item_retry_constant.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_retry_constant
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/update_folder_json_body.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,59 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemRetryExponential")
+T = TypeVar("T", bound="UpdateFolderJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemRetryExponential:
+class UpdateFolderJsonBody:
     """
     Attributes:
-        attempts (Union[Unset, int]):
-        multiplier (Union[Unset, int]):
-        seconds (Union[Unset, int]):
+        owners (Union[Unset, List[str]]):
+        extra_perms (Union[Unset, Any]):
     """
 
-    attempts: Union[Unset, int] = UNSET
-    multiplier: Union[Unset, int] = UNSET
-    seconds: Union[Unset, int] = UNSET
+    owners: Union[Unset, List[str]] = UNSET
+    extra_perms: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        attempts = self.attempts
-        multiplier = self.multiplier
-        seconds = self.seconds
+        owners: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.owners, Unset):
+            owners = self.owners
+
+        extra_perms = self.extra_perms
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if attempts is not UNSET:
-            field_dict["attempts"] = attempts
-        if multiplier is not UNSET:
-            field_dict["multiplier"] = multiplier
-        if seconds is not UNSET:
-            field_dict["seconds"] = seconds
+        if owners is not UNSET:
+            field_dict["owners"] = owners
+        if extra_perms is not UNSET:
+            field_dict["extra_perms"] = extra_perms
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        attempts = d.pop("attempts", UNSET)
-
-        multiplier = d.pop("multiplier", UNSET)
+        owners = cast(List[str], d.pop("owners", UNSET))
 
-        seconds = d.pop("seconds", UNSET)
+        extra_perms = d.pop("extra_perms", UNSET)
 
-        run_flow_preview_json_body_value_modules_item_retry_exponential = cls(
-            attempts=attempts,
-            multiplier=multiplier,
-            seconds=seconds,
+        update_folder_json_body = cls(
+            owners=owners,
+            extra_perms=extra_perms,
         )
 
-        run_flow_preview_json_body_value_modules_item_retry_exponential.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_retry_exponential
+        update_folder_json_body.additional_properties = d
+        return update_folder_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_modules_item_sleep_type_0_type import (
-    RunFlowPreviewJsonBodyValueModulesItemSleepType0Type,
+from ..models.update_flow_json_body_value_modules_item_sleep_type_0_type import (
+    UpdateFlowJsonBodyValueModulesItemSleepType0Type,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemSleepType0")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemSleepType0:
+class UpdateFlowJsonBodyValueModulesItemSleepType0:
     """
     Attributes:
-        type (RunFlowPreviewJsonBodyValueModulesItemSleepType0Type):
+        type (UpdateFlowJsonBodyValueModulesItemSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: RunFlowPreviewJsonBodyValueModulesItemSleepType0Type
+    type: UpdateFlowJsonBodyValueModulesItemSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = RunFlowPreviewJsonBodyValueModulesItemSleepType0Type(d.pop("type"))
+        type = UpdateFlowJsonBodyValueModulesItemSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        run_flow_preview_json_body_value_modules_item_sleep_type_0 = cls(
+        update_flow_json_body_value_modules_item_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        run_flow_preview_json_body_value_modules_item_sleep_type_0.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_sleep_type_0
+        update_flow_json_body_value_modules_item_sleep_type_0.additional_properties = d
+        return update_flow_json_body_value_modules_item_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.run_flow_preview_json_body_value_modules_item_sleep_type_1_type import (
-    RunFlowPreviewJsonBodyValueModulesItemSleepType1Type,
+from ..models.update_flow_json_body_value_modules_item_sleep_type_1_type import (
+    UpdateFlowJsonBodyValueModulesItemSleepType1Type,
 )
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemSleepType1")
+T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemSleepType1")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemSleepType1:
+class UpdateFlowJsonBodyValueModulesItemSleepType1:
     """
     Attributes:
         expr (str):
-        type (RunFlowPreviewJsonBodyValueModulesItemSleepType1Type):
+        type (UpdateFlowJsonBodyValueModulesItemSleepType1Type):
     """
 
     expr: str
-    type: RunFlowPreviewJsonBodyValueModulesItemSleepType1Type
+    type: UpdateFlowJsonBodyValueModulesItemSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         expr = self.expr
         type = self.type.value
 
         field_dict: Dict[str, Any] = {}
@@ -37,23 +37,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
-        type = RunFlowPreviewJsonBodyValueModulesItemSleepType1Type(d.pop("type"))
+        type = UpdateFlowJsonBodyValueModulesItemSleepType1Type(d.pop("type"))
 
-        run_flow_preview_json_body_value_modules_item_sleep_type_1 = cls(
+        update_flow_json_body_value_modules_item_sleep_type_1 = cls(
             expr=expr,
             type=type,
         )
 
-        run_flow_preview_json_body_value_modules_item_sleep_type_1.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_sleep_type_1
+        update_flow_json_body_value_modules_item_sleep_type_1.additional_properties = d
+        return update_flow_json_body_value_modules_item_sleep_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/workspace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemStopAfterIf")
+T = TypeVar("T", bound="Workspace")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemStopAfterIf:
+class Workspace:
     """
     Attributes:
-        expr (str):
-        skip_if_stopped (Union[Unset, bool]):
+        id (str):
+        name (str):
+        owner (str):
+        domain (Union[Unset, str]):
     """
 
-    expr: str
-    skip_if_stopped: Union[Unset, bool] = UNSET
+    id: str
+    name: str
+    owner: str
+    domain: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expr = self.expr
-        skip_if_stopped = self.skip_if_stopped
+        id = self.id
+        name = self.name
+        owner = self.owner
+        domain = self.domain
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "expr": expr,
+                "id": id,
+                "name": name,
+                "owner": owner,
             }
         )
-        if skip_if_stopped is not UNSET:
-            field_dict["skip_if_stopped"] = skip_if_stopped
+        if domain is not UNSET:
+            field_dict["domain"] = domain
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expr = d.pop("expr")
+        id = d.pop("id")
 
-        skip_if_stopped = d.pop("skip_if_stopped", UNSET)
+        name = d.pop("name")
 
-        run_flow_preview_json_body_value_modules_item_stop_after_if = cls(
-            expr=expr,
-            skip_if_stopped=skip_if_stopped,
+        owner = d.pop("owner")
+
+        domain = d.pop("domain", UNSET)
+
+        workspace = cls(
+            id=id,
+            name=name,
+            owner=owner,
+            domain=domain,
         )
 
-        run_flow_preview_json_body_value_modules_item_stop_after_if.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_stop_after_if
+        workspace.additional_properties = d
+        return workspace
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.91.0/windmill_api/models/create_flow_json_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RunFlowPreviewJsonBodyValueModulesItemSuspend")
+T = TypeVar("T", bound="CreateFlowJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class RunFlowPreviewJsonBodyValueModulesItemSuspend:
+class CreateFlowJsonBody:
     """
     Attributes:
-        required_events (Union[Unset, int]):
-        timeout (Union[Unset, int]):
+        draft_only (Union[Unset, bool]):
     """
 
-    required_events: Union[Unset, int] = UNSET
-    timeout: Union[Unset, int] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        required_events = self.required_events
-        timeout = self.timeout
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if required_events is not UNSET:
-            field_dict["required_events"] = required_events
-        if timeout is not UNSET:
-            field_dict["timeout"] = timeout
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        required_events = d.pop("required_events", UNSET)
+        draft_only = d.pop("draft_only", UNSET)
 
-        timeout = d.pop("timeout", UNSET)
-
-        run_flow_preview_json_body_value_modules_item_suspend = cls(
-            required_events=required_events,
-            timeout=timeout,
+        create_flow_json_body = cls(
+            draft_only=draft_only,
         )
 
-        run_flow_preview_json_body_value_modules_item_suspend.additional_properties = d
-        return run_flow_preview_json_body_value_modules_item_suspend
+        create_flow_json_body.additional_properties = d
+        return create_flow_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.91.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.91.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/schedule_args.py` & `windmill_api-1.91.0/windmill_api/models/schedule_extra_perms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ScheduleArgs")
+T = TypeVar("T", bound="ScheduleExtraPerms")
 
 
 @attr.s(auto_attribs=True)
-class ScheduleArgs:
+class ScheduleExtraPerms:
     """ """
 
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, bool] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        schedule_args = cls()
+        schedule_extra_perms = cls()
 
-        schedule_args.additional_properties = d
-        return schedule_args
+        schedule_extra_perms.additional_properties = d
+        return schedule_extra_perms
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: str) -> bool:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: str, value: bool) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `windmill_api-1.90.0/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ScheduleExtraPerms")
+T = TypeVar("T", bound="UpdateScheduleJsonBodyArgs")
 
 
 @attr.s(auto_attribs=True)
-class ScheduleExtraPerms:
+class UpdateScheduleJsonBodyArgs:
     """ """
 
-    additional_properties: Dict[str, bool] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        schedule_extra_perms = cls()
+        update_schedule_json_body_args = cls()
 
-        schedule_extra_perms.additional_properties = d
-        return schedule_extra_perms
+        update_schedule_json_body_args.additional_properties = d
+        return update_schedule_json_body_args
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> bool:
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: bool) -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `windmill_api-1.90.0/windmill_api/models/script.py` & `windmill_api-1.91.0/windmill_api/models/script.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         workspace_id (Union[Unset, str]):
         parent_hashes (Union[Unset, List[str]]): The first element is the direct parent of the script, the second is the
             parent of the first, etc
         schema (Union[Unset, ScriptSchema]):
         lock (Union[Unset, str]):
         lock_error_logs (Union[Unset, str]):
         tag (Union[Unset, str]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
     hash_: str
     path: str
     summary: str
     description: str
     content: str
@@ -56,14 +58,16 @@
     starred: bool
     workspace_id: Union[Unset, str] = UNSET
     parent_hashes: Union[Unset, List[str]] = UNSET
     schema: Union[Unset, ScriptSchema] = UNSET
     lock: Union[Unset, str] = UNSET
     lock_error_logs: Union[Unset, str] = UNSET
     tag: Union[Unset, str] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         hash_ = self.hash_
         path = self.path
         summary = self.summary
         description = self.description
@@ -89,14 +93,16 @@
         schema: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.schema, Unset):
             schema = self.schema.to_dict()
 
         lock = self.lock
         lock_error_logs = self.lock_error_logs
         tag = self.tag
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "hash": hash_,
                 "path": path,
@@ -122,14 +128,18 @@
             field_dict["schema"] = schema
         if lock is not UNSET:
             field_dict["lock"] = lock
         if lock_error_logs is not UNSET:
             field_dict["lock_error_logs"] = lock_error_logs
         if tag is not UNSET:
             field_dict["tag"] = tag
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         hash_ = d.pop("hash")
@@ -173,14 +183,18 @@
 
         lock = d.pop("lock", UNSET)
 
         lock_error_logs = d.pop("lock_error_logs", UNSET)
 
         tag = d.pop("tag", UNSET)
 
+        has_draft = d.pop("has_draft", UNSET)
+
+        draft_only = d.pop("draft_only", UNSET)
+
         script = cls(
             hash_=hash_,
             path=path,
             summary=summary,
             description=description,
             content=content,
             created_by=created_by,
@@ -194,14 +208,16 @@
             starred=starred,
             workspace_id=workspace_id,
             parent_hashes=parent_hashes,
             schema=schema,
             lock=lock,
             lock_error_logs=lock_error_logs,
             tag=tag,
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
         script.additional_properties = d
         return script
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `windmill_api-1.90.0/windmill_api/models/script_args.py` & `windmill_api-1.91.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ScriptArgs")
+T = TypeVar("T", bound="GetAppByPathWithDraftResponse200ExtraPerms")
 
 
 @attr.s(auto_attribs=True)
-class ScriptArgs:
+class GetAppByPathWithDraftResponse200ExtraPerms:
     """ """
 
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, bool] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        script_args = cls()
+        get_app_by_path_with_draft_response_200_extra_perms = cls()
 
-        script_args.additional_properties = d
-        return script_args
+        get_app_by_path_with_draft_response_200_extra_perms.additional_properties = d
+        return get_app_by_path_with_draft_response_200_extra_perms
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: str) -> bool:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: str, value: bool) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `windmill_api-1.90.0/windmill_api/models/script_extra_perms.py` & `windmill_api-1.91.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/script_schema.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ScriptSchema")
+T = TypeVar("T", bound="UpdateFlowJsonBodySchema")
 
 
 @attr.s(auto_attribs=True)
-class ScriptSchema:
+class UpdateFlowJsonBodySchema:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
@@ -18,18 +18,18 @@
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        script_schema = cls()
+        update_flow_json_body_schema = cls()
 
-        script_schema.additional_properties = d
-        return script_schema
+        update_flow_json_body_schema.additional_properties = d
+        return update_flow_json_body_schema
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/set_password_json_body.py` & `windmill_api-1.91.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.91.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/slack_token.py` & `windmill_api-1.91.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/slack_token_bot.py` & `windmill_api-1.91.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/star_json_body.py` & `windmill_api-1.91.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/static_transform.py` & `windmill_api-1.91.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/token_response.py` & `windmill_api-1.91.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/truncated_token.py` & `windmill_api-1.91.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/unstar_json_body.py` & `windmill_api-1.91.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/update_app_json_body.py` & `windmill_api-1.91.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.91.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.91.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.91.0/windmill_api/models/user_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-T = TypeVar("T", bound="UpdateFlowJsonBodySchema")
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="UserUsage")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodySchema:
-    """ """
+class UserUsage:
+    """
+    Attributes:
+        executions (Union[Unset, float]):
+    """
 
+    executions: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        executions = self.executions
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
+        if executions is not UNSET:
+            field_dict["executions"] = executions
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        update_flow_json_body_schema = cls()
+        executions = d.pop("executions", UNSET)
+
+        user_usage = cls(
+            executions=executions,
+        )
 
-        update_flow_json_body_schema.additional_properties = d
-        return update_flow_json_body_schema
+        user_usage.additional_properties = d
+        return user_usage
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.update_flow_json_body_value_failure_module_retry_constant import (
-    UpdateFlowJsonBodyValueFailureModuleRetryConstant,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant import (
+    GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant,
 )
-from ..models.update_flow_json_body_value_failure_module_retry_exponential import (
-    UpdateFlowJsonBodyValueFailureModuleRetryExponential,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential import (
+    GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleRetry")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueModulesItemRetry")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleRetry:
+class GetFlowByPathWithDraftResponse200DraftValueModulesItemRetry:
     """
     Attributes:
-        constant (Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryConstant]):
-        exponential (Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryExponential]):
+        constant (Union[Unset, GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant]):
+        exponential (Union[Unset, GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential]):
     """
 
-    constant: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryConstant] = UNSET
-    exponential: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryExponential] = UNSET
+    constant: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant] = UNSET
+    exponential: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         constant: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.constant, Unset):
             constant = self.constant.to_dict()
 
@@ -44,34 +44,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _constant = d.pop("constant", UNSET)
-        constant: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryConstant]
+        constant: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant]
         if isinstance(_constant, Unset):
             constant = UNSET
         else:
-            constant = UpdateFlowJsonBodyValueFailureModuleRetryConstant.from_dict(_constant)
+            constant = GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryConstant.from_dict(_constant)
 
         _exponential = d.pop("exponential", UNSET)
-        exponential: Union[Unset, UpdateFlowJsonBodyValueFailureModuleRetryExponential]
+        exponential: Union[Unset, GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential]
         if isinstance(_exponential, Unset):
             exponential = UNSET
         else:
-            exponential = UpdateFlowJsonBodyValueFailureModuleRetryExponential.from_dict(_exponential)
+            exponential = GetFlowByPathWithDraftResponse200DraftValueModulesItemRetryExponential.from_dict(_exponential)
 
-        update_flow_json_body_value_failure_module_retry = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry = cls(
             constant=constant,
             exponential=exponential,
         )
 
-        update_flow_json_body_value_failure_module_retry.additional_properties = d
-        return update_flow_json_body_value_failure_module_retry
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,62 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleRetryConstant")
+T = TypeVar("T", bound="UserWorkspaceListWorkspacesItem")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleRetryConstant:
+class UserWorkspaceListWorkspacesItem:
     """
     Attributes:
-        attempts (Union[Unset, int]):
-        seconds (Union[Unset, int]):
+        id (str):
+        name (str):
+        username (str):
     """
 
-    attempts: Union[Unset, int] = UNSET
-    seconds: Union[Unset, int] = UNSET
+    id: str
+    name: str
+    username: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        attempts = self.attempts
-        seconds = self.seconds
+        id = self.id
+        name = self.name
+        username = self.username
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if attempts is not UNSET:
-            field_dict["attempts"] = attempts
-        if seconds is not UNSET:
-            field_dict["seconds"] = seconds
+        field_dict.update(
+            {
+                "id": id,
+                "name": name,
+                "username": username,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        attempts = d.pop("attempts", UNSET)
+        id = d.pop("id")
+
+        name = d.pop("name")
 
-        seconds = d.pop("seconds", UNSET)
+        username = d.pop("username")
 
-        update_flow_json_body_value_failure_module_retry_constant = cls(
-            attempts=attempts,
-            seconds=seconds,
+        user_workspace_list_workspaces_item = cls(
+            id=id,
+            name=name,
+            username=username,
         )
 
-        update_flow_json_body_value_failure_module_retry_constant.additional_properties = d
-        return update_flow_json_body_value_failure_module_retry_constant
+        user_workspace_list_workspaces_item.additional_properties = d
+        return user_workspace_list_workspaces_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/update_input.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,62 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleRetryExponential")
+T = TypeVar("T", bound="UpdateInput")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleRetryExponential:
+class UpdateInput:
     """
     Attributes:
-        attempts (Union[Unset, int]):
-        multiplier (Union[Unset, int]):
-        seconds (Union[Unset, int]):
+        id (str):
+        name (str):
+        is_public (bool):
     """
 
-    attempts: Union[Unset, int] = UNSET
-    multiplier: Union[Unset, int] = UNSET
-    seconds: Union[Unset, int] = UNSET
+    id: str
+    name: str
+    is_public: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        attempts = self.attempts
-        multiplier = self.multiplier
-        seconds = self.seconds
+        id = self.id
+        name = self.name
+        is_public = self.is_public
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if attempts is not UNSET:
-            field_dict["attempts"] = attempts
-        if multiplier is not UNSET:
-            field_dict["multiplier"] = multiplier
-        if seconds is not UNSET:
-            field_dict["seconds"] = seconds
+        field_dict.update(
+            {
+                "id": id,
+                "name": name,
+                "is_public": is_public,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        attempts = d.pop("attempts", UNSET)
+        id = d.pop("id")
 
-        multiplier = d.pop("multiplier", UNSET)
+        name = d.pop("name")
 
-        seconds = d.pop("seconds", UNSET)
+        is_public = d.pop("is_public")
 
-        update_flow_json_body_value_failure_module_retry_exponential = cls(
-            attempts=attempts,
-            multiplier=multiplier,
-            seconds=seconds,
+        update_input = cls(
+            id=id,
+            name=name,
+            is_public=is_public,
         )
 
-        update_flow_json_body_value_failure_module_retry_exponential.additional_properties = d
-        return update_flow_json_body_value_failure_module_retry_exponential
+        update_input.additional_properties = d
+        return update_input
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.update_flow_json_body_value_failure_module_sleep_type_0_type import (
-    UpdateFlowJsonBodyValueFailureModuleSleepType0Type,
+from ..models.get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type import (
+    GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType0Type,
 )
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleSleepType0")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType0")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleSleepType0:
+class GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType0:
     """
     Attributes:
-        type (UpdateFlowJsonBodyValueFailureModuleSleepType0Type):
+        type (GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType0Type):
         value (Union[Unset, Any]):
     """
 
-    type: UpdateFlowJsonBodyValueFailureModuleSleepType0Type
+    type: GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType0Type
     value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         value = self.value
@@ -38,25 +38,25 @@
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = UpdateFlowJsonBodyValueFailureModuleSleepType0Type(d.pop("type"))
+        type = GetFlowByPathWithDraftResponse200DraftValueFailureModuleSleepType0Type(d.pop("type"))
 
         value = d.pop("value", UNSET)
 
-        update_flow_json_body_value_failure_module_sleep_type_0 = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0 = cls(
             type=type,
             value=value,
         )
 
-        update_flow_json_body_value_failure_module_sleep_type_0.additional_properties = d
-        return update_flow_json_body_value_failure_module_sleep_type_0
+        get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,35 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.update_flow_json_body_value_failure_module_sleep_type_1_type import (
-    UpdateFlowJsonBodyValueFailureModuleSleepType1Type,
-)
-
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleSleepType1")
+T = TypeVar("T", bound="GetScriptByPathWithDraftResponse200Schema")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleSleepType1:
-    """
-    Attributes:
-        expr (str):
-        type (UpdateFlowJsonBodyValueFailureModuleSleepType1Type):
-    """
+class GetScriptByPathWithDraftResponse200Schema:
+    """ """
 
-    expr: str
-    type: UpdateFlowJsonBodyValueFailureModuleSleepType1Type
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expr = self.expr
-        type = self.type.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "expr": expr,
-                "type": type,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expr = d.pop("expr")
-
-        type = UpdateFlowJsonBodyValueFailureModuleSleepType1Type(d.pop("type"))
-
-        update_flow_json_body_value_failure_module_sleep_type_1 = cls(
-            expr=expr,
-            type=type,
-        )
+        get_script_by_path_with_draft_response_200_schema = cls()
 
-        update_flow_json_body_value_failure_module_sleep_type_1.additional_properties = d
-        return update_flow_json_body_value_failure_module_sleep_type_1
+        get_script_by_path_with_draft_response_200_schema.additional_properties = d
+        return get_script_by_path_with_draft_response_200_schema
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleStopAfterIf")
+T = TypeVar("T", bound="UpdateResourceTypeJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleStopAfterIf:
+class UpdateResourceTypeJsonBody:
     """
     Attributes:
-        expr (str):
-        skip_if_stopped (Union[Unset, bool]):
+        schema (Union[Unset, str]):
+        description (Union[Unset, str]):
     """
 
-    expr: str
-    skip_if_stopped: Union[Unset, bool] = UNSET
+    schema: Union[Unset, str] = UNSET
+    description: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expr = self.expr
-        skip_if_stopped = self.skip_if_stopped
+        schema = self.schema
+        description = self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "expr": expr,
-            }
-        )
-        if skip_if_stopped is not UNSET:
-            field_dict["skip_if_stopped"] = skip_if_stopped
+        field_dict.update({})
+        if schema is not UNSET:
+            field_dict["schema"] = schema
+        if description is not UNSET:
+            field_dict["description"] = description
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expr = d.pop("expr")
+        schema = d.pop("schema", UNSET)
 
-        skip_if_stopped = d.pop("skip_if_stopped", UNSET)
+        description = d.pop("description", UNSET)
 
-        update_flow_json_body_value_failure_module_stop_after_if = cls(
-            expr=expr,
-            skip_if_stopped=skip_if_stopped,
+        update_resource_type_json_body = cls(
+            schema=schema,
+            description=description,
         )
 
-        update_flow_json_body_value_failure_module_stop_after_if.additional_properties = d
-        return update_flow_json_body_value_failure_module_stop_after_if
+        update_resource_type_json_body.additional_properties = d
+        return update_resource_type_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.91.0/windmill_api/models/update_user_json_body.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueFailureModuleSuspend")
+T = TypeVar("T", bound="UpdateUserJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueFailureModuleSuspend:
+class UpdateUserJsonBody:
     """
     Attributes:
-        required_events (Union[Unset, int]):
-        timeout (Union[Unset, int]):
+        is_admin (Union[Unset, bool]):
+        operator (Union[Unset, bool]):
+        disabled (Union[Unset, bool]):
     """
 
-    required_events: Union[Unset, int] = UNSET
-    timeout: Union[Unset, int] = UNSET
+    is_admin: Union[Unset, bool] = UNSET
+    operator: Union[Unset, bool] = UNSET
+    disabled: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        required_events = self.required_events
-        timeout = self.timeout
+        is_admin = self.is_admin
+        operator = self.operator
+        disabled = self.disabled
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if required_events is not UNSET:
-            field_dict["required_events"] = required_events
-        if timeout is not UNSET:
-            field_dict["timeout"] = timeout
+        if is_admin is not UNSET:
+            field_dict["is_admin"] = is_admin
+        if operator is not UNSET:
+            field_dict["operator"] = operator
+        if disabled is not UNSET:
+            field_dict["disabled"] = disabled
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        required_events = d.pop("required_events", UNSET)
+        is_admin = d.pop("is_admin", UNSET)
 
-        timeout = d.pop("timeout", UNSET)
+        operator = d.pop("operator", UNSET)
 
-        update_flow_json_body_value_failure_module_suspend = cls(
-            required_events=required_events,
-            timeout=timeout,
+        disabled = d.pop("disabled", UNSET)
+
+        update_user_json_body = cls(
+            is_admin=is_admin,
+            operator=operator,
+            disabled=disabled,
         )
 
-        update_flow_json_body_value_failure_module_suspend.additional_properties = d
-        return update_flow_json_body_value_failure_module_suspend
+        update_user_json_body.additional_properties = d
+        return update_user_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.91.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemRetryConstant")
+T = TypeVar("T", bound="ListFlowsResponse200Item")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueModulesItemRetryConstant:
+class ListFlowsResponse200Item:
     """
     Attributes:
-        attempts (Union[Unset, int]):
-        seconds (Union[Unset, int]):
+        has_draft (Union[Unset, bool]):
+        draft_only (Union[Unset, bool]):
     """
 
-    attempts: Union[Unset, int] = UNSET
-    seconds: Union[Unset, int] = UNSET
+    has_draft: Union[Unset, bool] = UNSET
+    draft_only: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        attempts = self.attempts
-        seconds = self.seconds
+        has_draft = self.has_draft
+        draft_only = self.draft_only
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if attempts is not UNSET:
-            field_dict["attempts"] = attempts
-        if seconds is not UNSET:
-            field_dict["seconds"] = seconds
+        if has_draft is not UNSET:
+            field_dict["has_draft"] = has_draft
+        if draft_only is not UNSET:
+            field_dict["draft_only"] = draft_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        attempts = d.pop("attempts", UNSET)
+        has_draft = d.pop("has_draft", UNSET)
 
-        seconds = d.pop("seconds", UNSET)
+        draft_only = d.pop("draft_only", UNSET)
 
-        update_flow_json_body_value_modules_item_retry_constant = cls(
-            attempts=attempts,
-            seconds=seconds,
+        list_flows_response_200_item = cls(
+            has_draft=has_draft,
+            draft_only=draft_only,
         )
 
-        update_flow_json_body_value_modules_item_retry_constant.additional_properties = d
-        return update_flow_json_body_value_modules_item_retry_constant
+        list_flows_response_200_item.additional_properties = d
+        return list_flows_response_200_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.91.0/windmill_api/models/update_group_json_body.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemRetryExponential")
+T = TypeVar("T", bound="UpdateGroupJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueModulesItemRetryExponential:
+class UpdateGroupJsonBody:
     """
     Attributes:
-        attempts (Union[Unset, int]):
-        multiplier (Union[Unset, int]):
-        seconds (Union[Unset, int]):
+        summary (Union[Unset, str]):
     """
 
-    attempts: Union[Unset, int] = UNSET
-    multiplier: Union[Unset, int] = UNSET
-    seconds: Union[Unset, int] = UNSET
+    summary: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        attempts = self.attempts
-        multiplier = self.multiplier
-        seconds = self.seconds
+        summary = self.summary
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if attempts is not UNSET:
-            field_dict["attempts"] = attempts
-        if multiplier is not UNSET:
-            field_dict["multiplier"] = multiplier
-        if seconds is not UNSET:
-            field_dict["seconds"] = seconds
+        if summary is not UNSET:
+            field_dict["summary"] = summary
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        attempts = d.pop("attempts", UNSET)
+        summary = d.pop("summary", UNSET)
 
-        multiplier = d.pop("multiplier", UNSET)
-
-        seconds = d.pop("seconds", UNSET)
-
-        update_flow_json_body_value_modules_item_retry_exponential = cls(
-            attempts=attempts,
-            multiplier=multiplier,
-            seconds=seconds,
+        update_group_json_body = cls(
+            summary=summary,
         )
 
-        update_flow_json_body_value_modules_item_retry_exponential.additional_properties = d
-        return update_flow_json_body_value_modules_item_retry_exponential
+        update_group_json_body.additional_properties = d
+        return update_group_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.91.0/windmill_api/models/update_input_json_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.update_flow_json_body_value_modules_item_sleep_type_0_type import (
-    UpdateFlowJsonBodyValueModulesItemSleepType0Type,
-)
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemSleepType0")
+T = TypeVar("T", bound="UpdateInputJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueModulesItemSleepType0:
+class UpdateInputJsonBody:
     """
     Attributes:
-        type (UpdateFlowJsonBodyValueModulesItemSleepType0Type):
-        value (Union[Unset, Any]):
+        id (str):
+        name (str):
+        is_public (bool):
     """
 
-    type: UpdateFlowJsonBodyValueModulesItemSleepType0Type
-    value: Union[Unset, Any] = UNSET
+    id: str
+    name: str
+    is_public: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        type = self.type.value
-
-        value = self.value
+        id = self.id
+        name = self.name
+        is_public = self.is_public
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "type": type,
+                "id": id,
+                "name": name,
+                "is_public": is_public,
             }
         )
-        if value is not UNSET:
-            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = UpdateFlowJsonBodyValueModulesItemSleepType0Type(d.pop("type"))
+        id = d.pop("id")
+
+        name = d.pop("name")
 
-        value = d.pop("value", UNSET)
+        is_public = d.pop("is_public")
 
-        update_flow_json_body_value_modules_item_sleep_type_0 = cls(
-            type=type,
-            value=value,
+        update_input_json_body = cls(
+            id=id,
+            name=name,
+            is_public=is_public,
         )
 
-        update_flow_json_body_value_modules_item_sleep_type_0.additional_properties = d
-        return update_flow_json_body_value_modules_item_sleep_type_0
+        update_input_json_body.additional_properties = d
+        return update_input_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.91.0/windmill_api/models/update_schedule_json_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.update_flow_json_body_value_modules_item_sleep_type_1_type import (
-    UpdateFlowJsonBodyValueModulesItemSleepType1Type,
-)
+from ..models.update_schedule_json_body_args import UpdateScheduleJsonBodyArgs
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemSleepType1")
+T = TypeVar("T", bound="UpdateScheduleJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueModulesItemSleepType1:
+class UpdateScheduleJsonBody:
     """
     Attributes:
-        expr (str):
-        type (UpdateFlowJsonBodyValueModulesItemSleepType1Type):
+        schedule (str):
+        timezone (str):
+        args (UpdateScheduleJsonBodyArgs):
     """
 
-    expr: str
-    type: UpdateFlowJsonBodyValueModulesItemSleepType1Type
+    schedule: str
+    timezone: str
+    args: UpdateScheduleJsonBodyArgs
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expr = self.expr
-        type = self.type.value
+        schedule = self.schedule
+        timezone = self.timezone
+        args = self.args.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "expr": expr,
-                "type": type,
+                "schedule": schedule,
+                "timezone": timezone,
+                "args": args,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expr = d.pop("expr")
+        schedule = d.pop("schedule")
 
-        type = UpdateFlowJsonBodyValueModulesItemSleepType1Type(d.pop("type"))
+        timezone = d.pop("timezone")
 
-        update_flow_json_body_value_modules_item_sleep_type_1 = cls(
-            expr=expr,
-            type=type,
+        args = UpdateScheduleJsonBodyArgs.from_dict(d.pop("args"))
+
+        update_schedule_json_body = cls(
+            schedule=schedule,
+            timezone=timezone,
+            args=args,
         )
 
-        update_flow_json_body_value_modules_item_sleep_type_1.additional_properties = d
-        return update_flow_json_body_value_modules_item_sleep_type_1
+        update_schedule_json_body.additional_properties = d
+        return update_schedule_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateFlowJsonBodyValueModulesItemStopAfterIf")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftValueModulesItemStopAfterIf")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFlowJsonBodyValueModulesItemStopAfterIf:
+class GetFlowByPathWithDraftResponse200DraftValueModulesItemStopAfterIf:
     """
     Attributes:
         expr (str):
         skip_if_stopped (Union[Unset, bool]):
     """
 
     expr: str
@@ -38,21 +38,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         expr = d.pop("expr")
 
         skip_if_stopped = d.pop("skip_if_stopped", UNSET)
 
-        update_flow_json_body_value_modules_item_stop_after_if = cls(
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if = cls(
             expr=expr,
             skip_if_stopped=skip_if_stopped,
         )
 
-        update_flow_json_body_value_modules_item_stop_after_if.additional_properties = d
-        return update_flow_json_body_value_modules_item_stop_after_if
+        get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,35 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UpdateFolderJsonBody")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftExtraPerms")
 
 
 @attr.s(auto_attribs=True)
-class UpdateFolderJsonBody:
-    """
-    Attributes:
-        owners (Union[Unset, List[str]]):
-        extra_perms (Union[Unset, Any]):
-    """
+class GetFlowByPathWithDraftResponse200DraftExtraPerms:
+    """ """
 
-    owners: Union[Unset, List[str]] = UNSET
-    extra_perms: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        owners: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.owners, Unset):
-            owners = self.owners
-
-        extra_perms = self.extra_perms
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if owners is not UNSET:
-            field_dict["owners"] = owners
-        if extra_perms is not UNSET:
-            field_dict["extra_perms"] = extra_perms
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        owners = cast(List[str], d.pop("owners", UNSET))
-
-        extra_perms = d.pop("extra_perms", UNSET)
-
-        update_folder_json_body = cls(
-            owners=owners,
-            extra_perms=extra_perms,
-        )
+        get_flow_by_path_with_draft_response_200_draft_extra_perms = cls()
 
-        update_folder_json_body.additional_properties = d
-        return update_folder_json_body
+        get_flow_by_path_with_draft_response_200_draft_extra_perms.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_extra_perms
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_group_json_body.py` & `windmill_api-1.91.0/windmill_api/models/update_resource_json_body.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateGroupJsonBody")
+T = TypeVar("T", bound="UpdateResourceJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateGroupJsonBody:
+class UpdateResourceJsonBody:
     """
     Attributes:
-        summary (Union[Unset, str]):
+        path (Union[Unset, str]):
+        description (Union[Unset, str]):
+        value (Union[Unset, Any]):
     """
 
-    summary: Union[Unset, str] = UNSET
+    path: Union[Unset, str] = UNSET
+    description: Union[Unset, str] = UNSET
+    value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        summary = self.summary
+        path = self.path
+        description = self.description
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if summary is not UNSET:
-            field_dict["summary"] = summary
+        if path is not UNSET:
+            field_dict["path"] = path
+        if description is not UNSET:
+            field_dict["description"] = description
+        if value is not UNSET:
+            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        summary = d.pop("summary", UNSET)
+        path = d.pop("path", UNSET)
 
-        update_group_json_body = cls(
-            summary=summary,
+        description = d.pop("description", UNSET)
+
+        value = d.pop("value", UNSET)
+
+        update_resource_json_body = cls(
+            path=path,
+            description=description,
+            value=value,
         )
 
-        update_group_json_body.additional_properties = d
-        return update_group_json_body
+        update_resource_json_body.additional_properties = d
+        return update_resource_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_input.py` & `windmill_api-1.91.0/windmill_api/models/workspace_invite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UpdateInput")
+T = TypeVar("T", bound="WorkspaceInvite")
 
 
 @attr.s(auto_attribs=True)
-class UpdateInput:
+class WorkspaceInvite:
     """
     Attributes:
-        id (str):
-        name (str):
-        is_public (bool):
+        workspace_id (str):
+        email (str):
+        is_admin (bool):
+        operator (bool):
     """
 
-    id: str
-    name: str
-    is_public: bool
+    workspace_id: str
+    email: str
+    is_admin: bool
+    operator: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        name = self.name
-        is_public = self.is_public
+        workspace_id = self.workspace_id
+        email = self.email
+        is_admin = self.is_admin
+        operator = self.operator
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "id": id,
-                "name": name,
-                "is_public": is_public,
+                "workspace_id": workspace_id,
+                "email": email,
+                "is_admin": is_admin,
+                "operator": operator,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id")
+        workspace_id = d.pop("workspace_id")
 
-        name = d.pop("name")
+        email = d.pop("email")
 
-        is_public = d.pop("is_public")
+        is_admin = d.pop("is_admin")
 
-        update_input = cls(
-            id=id,
-            name=name,
-            is_public=is_public,
+        operator = d.pop("operator")
+
+        workspace_invite = cls(
+            workspace_id=workspace_id,
+            email=email,
+            is_admin=is_admin,
+            operator=operator,
         )
 
-        update_input.additional_properties = d
-        return update_input
+        workspace_invite.additional_properties = d
+        return workspace_invite
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_input_json_body.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,35 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UpdateInputJsonBody")
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200DraftSchema")
 
 
 @attr.s(auto_attribs=True)
-class UpdateInputJsonBody:
-    """
-    Attributes:
-        id (str):
-        name (str):
-        is_public (bool):
-    """
-
-    id: str
-    name: str
-    is_public: bool
+class GetFlowByPathWithDraftResponse200DraftSchema:
+    """ """
+
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        name = self.name
-        is_public = self.is_public
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "id": id,
-                "name": name,
-                "is_public": is_public,
-            }
-        )
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id")
-
-        name = d.pop("name")
-
-        is_public = d.pop("is_public")
-
-        update_input_json_body = cls(
-            id=id,
-            name=name,
-            is_public=is_public,
-        )
+        get_flow_by_path_with_draft_response_200_draft_schema = cls()
 
-        update_input_json_body.additional_properties = d
-        return update_input_json_body
+        get_flow_by_path_with_draft_response_200_draft_schema.additional_properties = d
+        return get_flow_by_path_with_draft_response_200_draft_schema
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.91.0/windmill_api/models/update_variable_json_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateResourceJsonBody")
+T = TypeVar("T", bound="UpdateVariableJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class UpdateResourceJsonBody:
+class UpdateVariableJsonBody:
     """
     Attributes:
         path (Union[Unset, str]):
+        value (Union[Unset, str]):
+        is_secret (Union[Unset, bool]):
         description (Union[Unset, str]):
-        value (Union[Unset, Any]):
     """
 
     path: Union[Unset, str] = UNSET
+    value: Union[Unset, str] = UNSET
+    is_secret: Union[Unset, bool] = UNSET
     description: Union[Unset, str] = UNSET
-    value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
-        description = self.description
         value = self.value
+        is_secret = self.is_secret
+        description = self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if path is not UNSET:
             field_dict["path"] = path
-        if description is not UNSET:
-            field_dict["description"] = description
         if value is not UNSET:
             field_dict["value"] = value
+        if is_secret is not UNSET:
+            field_dict["is_secret"] = is_secret
+        if description is not UNSET:
+            field_dict["description"] = description
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         path = d.pop("path", UNSET)
 
-        description = d.pop("description", UNSET)
-
         value = d.pop("value", UNSET)
 
-        update_resource_json_body = cls(
+        is_secret = d.pop("is_secret", UNSET)
+
+        description = d.pop("description", UNSET)
+
+        update_variable_json_body = cls(
             path=path,
-            description=description,
             value=value,
+            is_secret=is_secret,
+            description=description,
         )
 
-        update_resource_json_body.additional_properties = d
-        return update_resource_json_body
+        update_variable_json_body.additional_properties = d
+        return update_variable_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.91.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,35 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="UpdateResourceValueJsonBody")
+T = TypeVar("T", bound="GetScriptByPathWithDraftResponse200DraftSchema")
 
 
 @attr.s(auto_attribs=True)
-class UpdateResourceValueJsonBody:
-    """
-    Attributes:
-        value (Union[Unset, Any]):
-    """
+class GetScriptByPathWithDraftResponse200DraftSchema:
+    """ """
 
-    value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if value is not UNSET:
-            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        value = d.pop("value", UNSET)
-
-        update_resource_value_json_body = cls(
-            value=value,
-        )
+        get_script_by_path_with_draft_response_200_draft_schema = cls()
 
-        update_resource_value_json_body.additional_properties = d
-        return update_resource_value_json_body
+        get_script_by_path_with_draft_response_200_draft_schema.additional_properties = d
+        return get_script_by_path_with_draft_response_200_draft_schema
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.91.0/windmill_api/models/usage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-T = TypeVar("T", bound="UpdateScheduleJsonBodyArgs")
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="Usage")
 
 
 @attr.s(auto_attribs=True)
-class UpdateScheduleJsonBodyArgs:
-    """ """
+class Usage:
+    """
+    Attributes:
+        executions (Union[Unset, float]):
+    """
 
+    executions: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        executions = self.executions
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
+        if executions is not UNSET:
+            field_dict["executions"] = executions
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        update_schedule_json_body_args = cls()
+        executions = d.pop("executions", UNSET)
+
+        usage = cls(
+            executions=executions,
+        )
 
-        update_schedule_json_body_args.additional_properties = d
-        return update_schedule_json_body_args
+        usage.additional_properties = d
+        return usage
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/usage.py` & `windmill_api-1.91.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Usage")
+T = TypeVar("T", bound="WhoamiResponse200Usage")
 
 
 @attr.s(auto_attribs=True)
-class Usage:
+class WhoamiResponse200Usage:
     """
     Attributes:
         executions (Union[Unset, float]):
     """
 
     executions: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -29,20 +29,20 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         executions = d.pop("executions", UNSET)
 
-        usage = cls(
+        whoami_response_200_usage = cls(
             executions=executions,
         )
 
-        usage.additional_properties = d
-        return usage
+        whoami_response_200_usage.additional_properties = d
+        return whoami_response_200_usage
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/user.py` & `windmill_api-1.91.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/user_usage.py` & `windmill_api-1.91.0/windmill_api/models/whois_response_200_usage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UserUsage")
+T = TypeVar("T", bound="WhoisResponse200Usage")
 
 
 @attr.s(auto_attribs=True)
-class UserUsage:
+class WhoisResponse200Usage:
     """
     Attributes:
         executions (Union[Unset, float]):
     """
 
     executions: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -29,20 +29,20 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         executions = d.pop("executions", UNSET)
 
-        user_usage = cls(
+        whois_response_200_usage = cls(
             executions=executions,
         )
 
-        user_usage.additional_properties = d
-        return user_usage
+        whois_response_200_usage.additional_properties = d
+        return whois_response_200_usage
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/user_workspace_list.py` & `windmill_api-1.91.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.91.0/windmill_api/models/worker_ping.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,89 @@
-from typing import Any, Dict, List, Type, TypeVar
+import datetime
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
+from dateutil.parser import isoparse
 
-T = TypeVar("T", bound="UserWorkspaceListWorkspacesItem")
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="WorkerPing")
 
 
 @attr.s(auto_attribs=True)
-class UserWorkspaceListWorkspacesItem:
+class WorkerPing:
     """
     Attributes:
-        id (str):
-        name (str):
-        username (str):
+        worker (str):
+        worker_instance (str):
+        started_at (datetime.datetime):
+        ip (str):
+        jobs_executed (int):
+        last_ping (Union[Unset, float]):
     """
 
-    id: str
-    name: str
-    username: str
+    worker: str
+    worker_instance: str
+    started_at: datetime.datetime
+    ip: str
+    jobs_executed: int
+    last_ping: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        name = self.name
-        username = self.username
+        worker = self.worker
+        worker_instance = self.worker_instance
+        started_at = self.started_at.isoformat()
+
+        ip = self.ip
+        jobs_executed = self.jobs_executed
+        last_ping = self.last_ping
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "id": id,
-                "name": name,
-                "username": username,
+                "worker": worker,
+                "worker_instance": worker_instance,
+                "started_at": started_at,
+                "ip": ip,
+                "jobs_executed": jobs_executed,
             }
         )
+        if last_ping is not UNSET:
+            field_dict["last_ping"] = last_ping
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id")
+        worker = d.pop("worker")
+
+        worker_instance = d.pop("worker_instance")
+
+        started_at = isoparse(d.pop("started_at"))
+
+        ip = d.pop("ip")
 
-        name = d.pop("name")
+        jobs_executed = d.pop("jobs_executed")
 
-        username = d.pop("username")
+        last_ping = d.pop("last_ping", UNSET)
 
-        user_workspace_list_workspaces_item = cls(
-            id=id,
-            name=name,
-            username=username,
+        worker_ping = cls(
+            worker=worker,
+            worker_instance=worker_instance,
+            started_at=started_at,
+            ip=ip,
+            jobs_executed=jobs_executed,
+            last_ping=last_ping,
         )
 
-        user_workspace_list_workspaces_item.additional_properties = d
-        return user_workspace_list_workspaces_item
+        worker_ping.additional_properties = d
+        return worker_ping
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/models/whoami_response_200.py` & `windmill_api-1.91.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/whois_response_200.py` & `windmill_api-1.91.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/windmill_api/models/workspace_invite.py` & `windmill_api-1.91.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,56 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-T = TypeVar("T", bound="WorkspaceInvite")
+from ..models.get_flow_by_path_with_draft_response_200_draft import GetFlowByPathWithDraftResponse200Draft
+from ..types import UNSET, Unset
+
+T = TypeVar("T", bound="GetFlowByPathWithDraftResponse200")
 
 
 @attr.s(auto_attribs=True)
-class WorkspaceInvite:
+class GetFlowByPathWithDraftResponse200:
     """
     Attributes:
-        workspace_id (str):
-        email (str):
-        is_admin (bool):
-        operator (bool):
+        draft (Union[Unset, GetFlowByPathWithDraftResponse200Draft]):
     """
 
-    workspace_id: str
-    email: str
-    is_admin: bool
-    operator: bool
+    draft: Union[Unset, GetFlowByPathWithDraftResponse200Draft] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        workspace_id = self.workspace_id
-        email = self.email
-        is_admin = self.is_admin
-        operator = self.operator
+        draft: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.draft, Unset):
+            draft = self.draft.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "workspace_id": workspace_id,
-                "email": email,
-                "is_admin": is_admin,
-                "operator": operator,
-            }
-        )
+        field_dict.update({})
+        if draft is not UNSET:
+            field_dict["draft"] = draft
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        workspace_id = d.pop("workspace_id")
-
-        email = d.pop("email")
-
-        is_admin = d.pop("is_admin")
-
-        operator = d.pop("operator")
+        _draft = d.pop("draft", UNSET)
+        draft: Union[Unset, GetFlowByPathWithDraftResponse200Draft]
+        if isinstance(_draft, Unset):
+            draft = UNSET
+        else:
+            draft = GetFlowByPathWithDraftResponse200Draft.from_dict(_draft)
 
-        workspace_invite = cls(
-            workspace_id=workspace_id,
-            email=email,
-            is_admin=is_admin,
-            operator=operator,
+        get_flow_by_path_with_draft_response_200 = cls(
+            draft=draft,
         )
 
-        workspace_invite.additional_properties = d
-        return workspace_invite
+        get_flow_by_path_with_draft_response_200.additional_properties = d
+        return get_flow_by_path_with_draft_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.90.0/windmill_api/types.py` & `windmill_api-1.91.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.90.0/setup.py` & `windmill_api-1.91.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 packages = \
 ['windmill_api',
  'windmill_api.api',
  'windmill_api.api.app',
  'windmill_api.api.audit',
  'windmill_api.api.capture',
+ 'windmill_api.api.draft',
  'windmill_api.api.favorite',
  'windmill_api.api.flow',
  'windmill_api.api.folder',
  'windmill_api.api.granular_acl',
  'windmill_api.api.group',
  'windmill_api.api.input_',
  'windmill_api.api.job',
@@ -29,15 +30,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.90.0',
+    'version': '1.91.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.90.0/PKG-INFO` & `windmill_api-1.91.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.90.0
+Version: 1.91.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

