# Comparing `tmp/incydr-1.0.1.tar.gz` & `tmp/incydr-1.1.0.tar.gz`

## Comparing `incydr-1.0.1.tar` & `incydr-1.1.0.tar`

### file list

```diff
@@ -1,102 +1,106 @@
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/__init__.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/core.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cursor.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/exceptions.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/file_readers.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/render.py
--rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/rich_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/utils.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/alert_rules.py
--rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/alerts.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/audit_log.py
--rw-r--r--   0        0        0    17742 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/cases.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/departments.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/devices.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/directory_groups.py
--rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/file_events.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/models.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/trusted_activities.py
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/user_risk_profiles.py
--rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/users.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/utils.py
--rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/watchlists.py
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/alert_filter_options.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/audit_log_filter_options.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/event_filter_options.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/output_options.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/profile_filter_options.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/cmds/options/utils.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/logger/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/logger/enums.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_cli/logger/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/__version__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/exceptions.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/utils.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alert_rules/client.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alert_rules/models/request.py
--rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alert_rules/models/response.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/__init__.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/alert.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/enums.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/request.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/alerts/models/response.py
--rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/audit_log/client.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/audit_log/models.py
--rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/cases/client.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/cases/models.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/auth.py
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/client.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/models.py
--rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/core/utils.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/customer/client.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/customer/models.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/departments/client.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/departments/models.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/devices/client.py
--rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/devices/models.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/directory_groups/client.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/directory_groups/models.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/__init__.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/alerts.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/cases.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/devices.py
--rw-r--r--   0        0        0    17648 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/file_events.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/trusted_activities.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/enums/watchlists.py
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/enums.py
--rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/event.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/file_events/models/response.py
--rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/queries/alerts.py
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/queries/file_events.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/queries/utils.py
--rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/trusted_activities/client.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/trusted_activities/models.py
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/user_risk_profiles/client.py
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/user_risk_profiles/models.py
--rw-r--r--   0        0        0    14022 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/users/client.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/users/models.py
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/models/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/models/requests.py
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 incydr-1.0.1/_incydr_sdk/watchlists/models/responses.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/__main__.py
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/models.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/alerts.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/cases.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/devices.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/file_events.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/trusted_activities.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 incydr-1.0.1/incydr/enums/watchlists.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 incydr-1.0.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 incydr-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 incydr-1.0.1/README.md
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 incydr-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 incydr-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/__init__.py
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/core.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cursor.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/exceptions.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/file_readers.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/render.py
+-rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/rich_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/utils.py
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/agents.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/alert_rules.py
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/alerts.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/audit_log.py
+-rw-r--r--   0        0        0    17742 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/cases.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/departments.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/devices.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/directory_groups.py
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/file_events.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/models.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/trusted_activities.py
+-rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/user_risk_profiles.py
+-rw-r--r--   0        0        0    15938 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/users.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/utils.py
+-rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/watchlists.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/options/alert_filter_options.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/options/audit_log_filter_options.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/options/event_filter_options.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/options/output_options.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/options/profile_filter_options.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/cmds/options/utils.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/logger/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/logger/enums.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_cli/logger/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/__version__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/exceptions.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/utils.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/agents/client.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/agents/models.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alert_rules/client.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alert_rules/models/request.py
+-rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alert_rules/models/response.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alerts/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alerts/models/__init__.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alerts/models/alert.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alerts/models/enums.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alerts/models/request.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/alerts/models/response.py
+-rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/audit_log/client.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/audit_log/models.py
+-rw-r--r--   0        0        0    15787 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/cases/client.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/cases/models.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/core/auth.py
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/core/client.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/core/models.py
+-rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/core/settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/core/utils.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/customer/client.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/customer/models.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/departments/client.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/departments/models.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/devices/client.py
+-rw-r--r--   0        0        0     7898 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/devices/models.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/directory_groups/client.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/directory_groups/models.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/__init__.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/alerts.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/cases.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/devices.py
+-rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/file_events.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/trusted_activities.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/enums/watchlists.py
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/file_events/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/file_events/models/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/file_events/models/enums.py
+-rw-r--r--   0        0        0    32082 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/file_events/models/event.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/file_events/models/response.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/queries/alerts.py
+-rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/queries/file_events.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/queries/utils.py
+-rw-r--r--   0        0        0    15252 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/trusted_activities/client.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/trusted_activities/models.py
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/user_risk_profiles/client.py
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/user_risk_profiles/models.py
+-rw-r--r--   0        0        0    14133 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/users/client.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/users/models.py
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/watchlists/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/watchlists/models/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/watchlists/models/requests.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 incydr-1.1.0/_incydr_sdk/watchlists/models/responses.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/__main__.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/models.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/agents.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/alerts.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/cases.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/devices.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/file_events.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/trusted_activities.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 incydr-1.1.0/incydr/enums/watchlists.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 incydr-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 incydr-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 incydr-1.1.0/README.md
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 incydr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 incydr-1.1.0/PKG-INFO
```

### Comparing `incydr-1.0.1/_incydr_cli/__init__.py` & `incydr-1.1.0/_incydr_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/core.py` & `incydr-1.1.0/_incydr_cli/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import re
 
 import click
 from requests import HTTPError
 
 from _incydr_cli.exceptions import IncydrCLIException
 from _incydr_cli.exceptions import LoggedCLIError
-from _incydr_sdk.core.client import Client
+from _incydr_sdk.core.settings import IncydrSettings
+from _incydr_sdk.exceptions import AuthMissingError
 from _incydr_sdk.exceptions import IncydrException
 
 _DIFFLIB_CUT_OFF = 0.6
 
 
 try:
     import rich
@@ -60,40 +61,49 @@
     def make_context(self, info_name, args, parent=None, **extra):
         # grab the original command line arguments for logging purposes
         self._original_args = " ".join(args)
 
         return super().make_context(info_name, args, parent=parent, **extra)
 
     def invoke(self, ctx):
+        settings = IncydrSettings(url="", api_client_id="", api_client_secret="")
         try:
             return super().invoke(ctx)
         except click.UsageError as err:
             self._suggest_cmd(err)
         except LoggedCLIError:
             raise
         except click.exceptions.Exit:
             raise
+        except AuthMissingError as err:
+            missing_vars = "\n".join(
+                f"  - INCYDR_{key.upper()}" for key in err.error_keys
+            )
+            msg = (
+                f"Missing authentication variables in environment.\n\n{missing_vars}"
+                "\n\nSee https://developer.code42.com/cli/getting_started/#authentication"
+            )
+            settings.logger.error(msg)
+            raise IncydrCLIException(msg)
+
         except IncydrException as err:
             # log error and raise custom error to print error message to console
-            client = Client(skip_auth=True)
-            client._log_error(err, self._original_args)
+            settings._log_error(err, self._original_args)
             raise IncydrCLIException(err.args[0])
         except click.ClickException:
             raise
         except HTTPError as err:
             # log error with traceback and print error code with brief error message to console
-            client = Client(skip_auth=True)
-            client._log_verbose_error(self._original_args, err.request)
+            settings._log_verbose_error(self._original_args, err.request)
             raise LoggedCLIError(err.args[0])
         except OSError:
             raise
         except Exception:
             # log error with traceback and print message pointing user to logs
-            client = Client(skip_auth=True)
-            client._log_verbose_error(self._original_args)
+            settings._log_verbose_error(self._original_args)
             raise LoggedCLIError("Unknown problem occurred.")
 
     @staticmethod
     def _suggest_cmd(usage_err):
         """Handles fuzzy suggestion of commands that are close to the bad command entered."""
         if usage_err.message is not None:
             match = re.match("No such command '(.*)'.", usage_err.message)
```

### Comparing `incydr-1.0.1/_incydr_cli/cursor.py` & `incydr-1.1.0/_incydr_cli/cursor.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/exceptions.py` & `incydr-1.1.0/_incydr_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/file_readers.py` & `incydr-1.1.0/_incydr_cli/file_readers.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/main.py` & `incydr-1.1.0/_incydr_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 
 import click
 from requests.exceptions import HTTPError
 
 from _incydr_cli import console
 from _incydr_cli import logging_options
+from _incydr_cli.cmds.agents import agents
 from _incydr_cli.cmds.alert_rules import alert_rules
 from _incydr_cli.cmds.alerts import alerts
 from _incydr_cli.cmds.audit_log import audit_log
 from _incydr_cli.cmds.cases import cases
 from _incydr_cli.cmds.departments import departments
 from _incydr_cli.cmds.devices import devices
 from _incydr_cli.cmds.directory_groups import directory_groups
@@ -62,14 +63,15 @@
 
         for root, _dirs, files in os.walk(site.USER_BASE):
             if "incydr" in files or "incydr.exe" in files:
                 console.print(root, highlight=False)
                 sys.exit(0)
 
 
+incydr.add_command(agents)
 incydr.add_command(alerts)
 incydr.add_command(alert_rules)
 incydr.add_command(audit_log)
 incydr.add_command(departments)
 incydr.add_command(devices)
 incydr.add_command(directory_groups)
 incydr.add_command(file_events)
```

### Comparing `incydr-1.0.1/_incydr_cli/render.py` & `incydr-1.1.0/_incydr_cli/render.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/rich_utils.py` & `incydr-1.1.0/_incydr_cli/rich_utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/utils.py` & `incydr-1.1.0/_incydr_cli/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/alert_rules.py` & `incydr-1.1.0/_incydr_cli/cmds/alert_rules.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/alerts.py` & `incydr-1.1.0/_incydr_cli/cmds/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/audit_log.py` & `incydr-1.1.0/_incydr_cli/cmds/audit_log.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/cases.py` & `incydr-1.1.0/_incydr_cli/cmds/cases.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/departments.py` & `incydr-1.1.0/_incydr_cli/cmds/departments.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/devices.py` & `incydr-1.1.0/_incydr_cli/cmds/devices.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/directory_groups.py` & `incydr-1.1.0/_incydr_cli/cmds/directory_groups.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/file_events.py` & `incydr-1.1.0/_incydr_cli/cmds/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/models.py` & `incydr-1.1.0/_incydr_cli/cmds/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,7 +20,30 @@
         if "username" not in values and "userId" not in values:
             raise ValueError("A json key of 'username' or 'userId' is required")
         return values
 
     @property
     def user(self):
         return self.userId or self.username
+
+
+class AgentCSV(CSVModel):
+    agent_id: str = Field(csv_aliases=["agent_id", "agentId", "guid"])
+
+
+class AgentJSON(Model):
+    agent_id: Optional[str]
+
+    @root_validator(pre=True)
+    def _validate(cls, values):  # noqa
+        if "agent_id" in values:
+            return values
+        elif "agentId" in values:
+            values["agent_id"] = values["agentId"]
+            return values
+        elif "guid" in values:
+            values["agent_id"] = values["guid"]
+            return values
+        else:
+            raise ValueError(
+                "A json key of 'agent_id', 'agentId', or 'guid' is required"
+            )
```

### Comparing `incydr-1.0.1/_incydr_cli/cmds/trusted_activities.py` & `incydr-1.1.0/_incydr_cli/cmds/trusted_activities.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/user_risk_profiles.py` & `incydr-1.1.0/_incydr_cli/cmds/user_risk_profiles.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/users.py` & `incydr-1.1.0/_incydr_cli/cmds/users.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/utils.py` & `incydr-1.1.0/_incydr_cli/cmds/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/watchlists.py` & `incydr-1.1.0/_incydr_cli/cmds/watchlists.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/options/alert_filter_options.py` & `incydr-1.1.0/_incydr_cli/cmds/options/alert_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/options/audit_log_filter_options.py` & `incydr-1.1.0/_incydr_cli/cmds/options/audit_log_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/options/event_filter_options.py` & `incydr-1.1.0/_incydr_cli/cmds/options/event_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/options/output_options.py` & `incydr-1.1.0/_incydr_cli/cmds/options/output_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/options/profile_filter_options.py` & `incydr-1.1.0/_incydr_cli/cmds/options/profile_filter_options.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/cmds/options/utils.py` & `incydr-1.1.0/_incydr_cli/cmds/options/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/logger/__init__.py` & `incydr-1.1.0/_incydr_cli/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_cli/logger/handlers.py` & `incydr-1.1.0/_incydr_cli/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/utils.py` & `incydr-1.1.0/_incydr_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alert_rules/client.py` & `incydr-1.1.0/_incydr_sdk/alert_rules/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alert_rules/models/response.py` & `incydr-1.1.0/_incydr_sdk/alert_rules/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alerts/client.py` & `incydr-1.1.0/_incydr_sdk/alerts/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alerts/models/alert.py` & `incydr-1.1.0/_incydr_sdk/alerts/models/alert.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alerts/models/enums.py` & `incydr-1.1.0/_incydr_sdk/alerts/models/enums.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alerts/models/request.py` & `incydr-1.1.0/_incydr_sdk/alerts/models/request.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/alerts/models/response.py` & `incydr-1.1.0/_incydr_sdk/alerts/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/audit_log/client.py` & `incydr-1.1.0/_incydr_sdk/audit_log/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/audit_log/models.py` & `incydr-1.1.0/_incydr_sdk/audit_log/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/cases/client.py` & `incydr-1.1.0/_incydr_sdk/cases/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/cases/models.py` & `incydr-1.1.0/_incydr_sdk/cases/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/core/auth.py` & `incydr-1.1.0/_incydr_sdk/core/auth.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/core/client.py` & `incydr-1.1.0/_incydr_sdk/core/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import base64
 import json
 import logging
-import re
-import traceback
 from collections import deque
-from textwrap import indent
 
+import pydantic
 from requests_toolbelt import user_agent
 from requests_toolbelt.sessions import BaseUrlSession
-from requests_toolbelt.utils.dump import dump_response
 
 from _incydr_sdk.__version__ import __version__
+from _incydr_sdk.agents.client import AgentsClient
 from _incydr_sdk.alert_rules.client import AlertRulesClient
 from _incydr_sdk.alerts.client import AlertsClient
 from _incydr_sdk.audit_log.client import AuditLogClient
 from _incydr_sdk.cases.client import CasesClient
 from _incydr_sdk.core.auth import APIClientAuth
 from _incydr_sdk.core.settings import IncydrSettings
 from _incydr_sdk.customer.client import CustomerClient
 from _incydr_sdk.departments.client import DepartmentsClient
 from _incydr_sdk.devices.client import DevicesClient
 from _incydr_sdk.directory_groups.client import DirectoryGroupsClient
+from _incydr_sdk.exceptions import AuthMissingError
 from _incydr_sdk.file_events.client import FileEventsClient
 from _incydr_sdk.trusted_activities.client import TrustedActivitiesClient
 from _incydr_sdk.user_risk_profiles.client import UserRiskProfiles
 from _incydr_sdk.users.client import UsersClient
 from _incydr_sdk.watchlists.client import WatchlistsClient
 
 _base_user_agent = user_agent("incydr", __version__)
-_auth_header_regex = re.compile(r"Authorization: (Bearer|Basic) \S+")
 
 
 class Client:
     """
     An HTTP client for interacting with the Code42 Incydr API.
 
     **Parameters**:
@@ -53,20 +51,28 @@
         self,
         url: str = None,
         api_client_id: str = None,
         api_client_secret: str = None,
         skip_auth: bool = False,
         **settings_kwargs,
     ):
-        self._settings = IncydrSettings(
-            url=url,
-            api_client_id=api_client_id,
-            api_client_secret=api_client_secret,
-            **settings_kwargs,
-        )
+        try:
+            self._settings = IncydrSettings(
+                url=url,
+                api_client_id=api_client_id,
+                api_client_secret=api_client_secret,
+                **settings_kwargs,
+            )
+        except pydantic.ValidationError as err:
+            auth_keys = {"api_client_id", "api_client_secret", "url"}
+            error_keys = {e["loc"][0] for e in err.errors()}
+            if auth_keys & error_keys:
+                raise AuthMissingError(err)
+            else:
+                raise
         self._request_history = deque(maxlen=self._settings.max_response_history)
 
         self._session = BaseUrlSession(base_url=self._settings.url)
         self._session.headers["User-Agent"] = (
             self._settings.user_agent_prefix or "" + _base_user_agent
         )
         self._session.auth = APIClientAuth(
@@ -74,23 +80,24 @@
             api_client_id=self._settings.api_client_id,
             api_client_secret=self._settings.api_client_secret,
         )
 
         def response_hook(response, *args, **kwargs):
             level = self._settings.log_level
             if level == logging.INFO:
-                self._log_response_info(response)
+                self.settings._log_response_info(response)
             if level == logging.DEBUG:
-                self._log_response_debug(response)
+                self.settings._log_response_debug(response)
 
             self._request_history.appendleft(response)
             response.raise_for_status()
 
         self._session.hooks["response"] = [response_hook]
 
+        self._agents = AgentsClient(self)
         self._alerts = AlertsClient(self)
         self._alert_rules = AlertRulesClient(self)
         self._audit_log = AuditLogClient(self)
         self._cases = CasesClient(self)
         self._customer = CustomerClient(self)
         self._departments = DepartmentsClient(self)
         self._devices = DevicesClient(self)
@@ -146,14 +153,24 @@
             <Response [200]>
             >>> response.url
             'https://api.us.code42.com/v1/users'
         """
         return self._session
 
     @property
+    def agents(self):
+        """
+        Property returning an [`AgentsClient`](../agents) for interacting with
+        `/v*/agents` API endpoints.
+        Usage:
+            >>> client.agents.v1.get_page()
+        """
+        return self._agents
+
+    @property
     def alerts(self):
         """
         Property returning an [`AlertsClient`](../alerts) for interacting with
         `/v*/alerts` API endpoints.
         Usage:
             >>> client.alerts.v1.get_page()
         """
@@ -294,50 +311,7 @@
         """
         Property returning a [`WatchlistsClient`](../watchlists) for interacting with `/v*/watchlists` API endpoints.
         Usage:
 
             >>> client.watchlists.v1.get_page()
         """
         return self._watchlists
-
-    def _log_response_info(self, response):
-        self._settings.logger.info(
-            f"{response.request.method} {response.request.url} status_code={response.status_code}"
-        )
-
-    def _log_response_debug(self, response):
-        try:
-            dumped = dump_response(
-                response, request_prefix=b"", response_prefix=b""
-            ).decode("utf-8")
-            dumped = re.sub(
-                _auth_header_regex,
-                "Authorization: <token_redacted>",
-                dumped,
-            )
-            if not self._settings.use_rich:
-                dumped = indent(dumped, prefix="\t")
-            self._settings.logger.debug(dumped)
-        except Exception as err:
-            self._settings.logger.debug(f"Error dumping request/response info: {err}")
-            self._settings.logger.debug(response)
-
-    def _log_error(self, err, invocation_str=None):
-        message = str(err) if err else None
-        if invocation_str:
-            message = f"Exception occurred from input: '{invocation_str}'.\n" + message
-        if message:
-            self._settings.logger.error(message)
-
-    def _log_verbose_error(self, invocation_str=None, http_request=None):
-        """For logging traces, invocation strs, and request parameters during exceptions to the
-        error log file."""
-        prefix = (
-            "Exception occurred."
-            if not invocation_str
-            else f"Exception occurred from input: '{invocation_str}'."
-        )
-        message = f"{prefix}. See error below."
-        self._log_error(message)
-        self._log_error(traceback.format_exc())
-        if http_request:
-            self._log_error(f"Request parameters: {http_request.body}")
```

### Comparing `incydr-1.0.1/_incydr_sdk/core/models.py` & `incydr-1.1.0/_incydr_sdk/core/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/core/settings.py` & `incydr-1.1.0/_incydr_sdk/core/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
+import re
 import sys
 import warnings
 from io import IOBase
 from pathlib import Path
+from textwrap import indent
 from typing import Union
 
 from pydantic import BaseSettings
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import SecretStr
 from pydantic import validator
+from requests_toolbelt.utils.dump import dump_response
 from rich import pretty
 from rich.console import Console
 from rich.logging import RichHandler
 
 from _incydr_sdk.enums import _Enum
 
 # capture default displayhook so we can "uninstall" rich
@@ -33,14 +36,16 @@
 
 
 _std_log_formatter = logging.Formatter(
     fmt="%(asctime)s - %(name)s:%(levelname)s - %(message)s", datefmt="[%x %X]"
 )
 _rich_log_formatter = logging.Formatter(fmt="%(message)s", datefmt="[%x %X]")
 
+_auth_header_regex = re.compile(r"Authorization: (Bearer|Basic) \S+")
+
 
 class IncydrSettings(BaseSettings):
     """
     Configure settings on the `incydr.Client`.
 
     Usage:
 
@@ -149,15 +154,15 @@
             return logger
         if isinstance(value, logging.Logger):
             return value
         else:
             raise ValueError(f"{value} is not a `logging.Logger`.")
 
     @root_validator(skip_on_failure=True)
-    def configure_logging(cls, values):  # noqa
+    def _configure_logging(cls, values):  # noqa
         use_rich = values["use_rich"]
         log_file = values["log_file"]
         log_stderr = values["log_stderr"]
         log_level = values["log_level"]
         logger = values["logger"]
 
         if not hasattr(logger, "_incydr"):
@@ -196,7 +201,48 @@
                 std_file_handler = logging.StreamHandler(stream=log_file)
             std_file_handler.setFormatter(_std_log_formatter)
             logger.addHandler(std_file_handler)
 
         logger.setLevel(log_level)
         values["logger"] = logger
         return values
+
+    def _log_response_info(self, response):
+        self.logger.info(
+            f"{response.request.method} {response.request.url} status_code={response.status_code}"
+        )
+
+    def _log_response_debug(self, response):
+        try:
+            dumped = dump_response(
+                response, request_prefix=b"", response_prefix=b""
+            ).decode("utf-8")
+            dumped = re.sub(
+                _auth_header_regex,
+                "Authorization: <token_redacted>",
+                dumped,
+            )
+            if not self.use_rich:
+                dumped = indent(dumped, prefix="\t")
+            self.logger.debug(dumped)
+        except Exception as err:
+            self.logger.debug(f"Error dumping request/response info: {err}")
+            self.logger.debug(response)
+
+    def _log_error(self, err, invocation_str=None):
+        message = str(err) if err else None
+        if invocation_str:
+            message = f"Exception occurred from input: '{invocation_str}'.\n" + message
+        if message:
+            self.logger.error(message)
+
+    def _log_verbose_error(self, invocation_str=None, http_request=None):
+        """For logging traces, invocation strs, and request parameters during exceptions to the
+        error log file."""
+        prefix = (
+            "Exception occurred."
+            if not invocation_str
+            else f"Exception occurred from input: '{invocation_str}'."
+        )
+        self.logger.exception(f"{prefix}. See error below.")
+        if http_request:
+            self._log_error(f"Request parameters: {http_request.body}")
```

### Comparing `incydr-1.0.1/_incydr_sdk/customer/client.py` & `incydr-1.1.0/_incydr_sdk/customer/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/customer/models.py` & `incydr-1.1.0/_incydr_sdk/customer/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/departments/client.py` & `incydr-1.1.0/_incydr_sdk/departments/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/departments/models.py` & `incydr-1.1.0/_incydr_sdk/departments/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/devices/client.py` & `incydr-1.1.0/_incydr_sdk/devices/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def __init__(self, parent):
         self._parent = parent
 
     def get_device(self, device_id: str) -> Device:
         """Get a single device.
 
-        **Parameters:**
+        **Parameters**:
 
         * **device_id**: `str` (required) - The unique ID for the device.
 
         **Returns**: A [`Device`][device-model] object representing the device.
 
         """
         response = self._parent.session.get(f"/v1/devices/{device_id}")
```

### Comparing `incydr-1.0.1/_incydr_sdk/devices/models.py` & `incydr-1.1.0/_incydr_sdk/devices/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/directory_groups/client.py` & `incydr-1.1.0/_incydr_sdk/directory_groups/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/directory_groups/models.py` & `incydr-1.1.0/_incydr_sdk/directory_groups/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/enums/__init__.py` & `incydr-1.1.0/_incydr_sdk/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/enums/alerts.py` & `incydr-1.1.0/_incydr_sdk/enums/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/enums/file_events.py` & `incydr-1.1.0/_incydr_sdk/enums/file_events.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     DESTINATION_IP = "destination.ip"
     DESTINATION_NAME = "destination.name"
     DESTINATION_OPERATING_SYSTEM = "destination.operatingSystem"
     DESTINATION_PRINT_JOB_NAME = "destination.printJobName"
     DESTINATION_PRINTED_FILES_BACKUP_PATH = "destination.printedFilesBackupPath"
     DESTINATION_PRINTER_NAME = "destination.printerName"
     DESTINATION_PRIVATE_IP = "destination.privateIp"
+    DESTINATION_REMOTE_HOSTNAME = "destination.remoteHostname"
     DESTINATION_REMOVABLE_MEDIA_BUS_TYPE = "destination.removableMedia.busType"
     DESTINATION_REMOVABLE_MEDIA_CAPACITY = "destination.removableMedia.capacity"
     DESTINATION_REMOVABLE_MEDIA_MEDIA_NAME = "destination.removableMedia.mediaName"
     DESTINATION_REMOVABLE_MEDIA_NAME = "destination.removableMedia.name"
     DESTINATION_REMOVABLE_MEDIA_PARTITION_ID = "destination.removableMedia.partitionId"
     DESTINATION_REMOVABLE_MEDIA_SERIAL_NUMBER = (
         "destination.removableMedia.serialNumber"
@@ -61,17 +62,39 @@
     EVENT_RELATED_EVENTS_SOURCE_NAME = "event.relatedEvents.sourceName"
     EVENT_RELATED_EVENTS_TABS_TITLE = "event.relatedEvents.tabs.title"
     EVENT_RELATED_EVENTS_TABS_TITLE_ERROR = "event.relatedEvents.tabs.titleError"
     EVENT_RELATED_EVENTS_TABS_URL = "event.relatedEvents.tabs.url"
     EVENT_RELATED_EVENTS_TABS_URL_ERROR = "event.relatedEvents.tabs.urlError"
     EVENT_RELATED_EVENTS_USER_EMAIL = "event.relatedEvents.userEmail"
     EVENT_SHARE_TYPE = "event.shareType"
+    EVENT_DETECTOR_DISPLAY_NAME = "event.detectorDisplayName"
+    EVENT_VECTOR = "event.vector"
+    FILE_ACQUIRED_FROM_GIT_REPOSITORY_EMAIL = "file.acquiredFrom.git.repositoryEmail"
+    FILE_ACQUIRED_FROM_GIT_REPOSITORY_URI = "file.acquiredFrom.git.repositoryUri"
+    FILE_ACQUIRED_FROM_GIT_REPOSITORY_USER = "file.acquiredFrom.git.repositoryUser"
+    FILE_ACQUIRED_FROM_TABS_URL_ERROR = "file.acquiredFrom.tabs.urlError"
+    FILE_ACQUIRED_FROM_SOURCE_DOMAINS = "file.acquiredFrom.sourceDomains"
+    FILE_ACQUIRED_FROM_USER_EMAIL = "file.acquiredFrom.userEmail"
+    FILE_ACQUIRED_FROM_SOURCE_USER_EMAIL = "file.acquiredFrom.sourceUser.email"
+    FILE_ACQUIRED_FROM_TABS_URL = "file.acquiredFrom.tabs.url"
+    FILE_ACQUIRED_FROM_EVENT_ID = "file.acquiredFrom.eventId"
+    FILE_ACQUIRED_FROM_FILE_NAME = "file.acquiredFrom.fileName"
+    FILE_ACQUIRED_FROM_SOURCE_CATEGORY = "file.acquiredFrom.sourceCategory"
+    FILE_ACQUIRED_FROM_SOURCE_ACCOUNT_NAME = "file.acquiredFrom.sourceAccountName"
+    FILE_ACQUIRED_FROM_SOURCE_NAME = "file.acquiredFrom.sourceName"
+    FILE_ACQUIRED_FROM_AGENT_TIMESTAMP = "file.acquiredFrom.agentTimestamp"
+    FILE_ACQUIRED_FROM_EVENT_ACTION = "file.acquiredFrom.eventAction"
+    FILE_ACQUIRED_FROM_TABS_TITLE_ERROR = "file.acquiredFrom.tabs.titleError"
+    FILE_ACQUIRED_FROM_TABS_TITLE = "file.acquiredFrom.tabs.title"
+    FILE_ACQUIRED_FROM_SOURCE_ACCOUNT_TYPE = "file.acquiredFrom.sourceAccountType"
+    FILE_ACQUIRED_FROM_MD5 = "file.acquiredFrom.md5"
     FILE_CATEGORY = "file.category"
     FILE_CATEGORY_BY_BYTES = "file.categoryByBytes"
     FILE_CATEGORY_BY_EXTENSION = "file.categoryByExtension"
+    FILE_CHANGE_TYPE = "file.changeType"
     FILE_CLASSIFICATIONS_VALUE = "file.classifications.value"
     FILE_CLASSIFICATIONS_VENDOR = "file.classifications.vendor"
     FILE_CLOUD_DRIVE_ID = "file.cloudDriveId"
     FILE_CREATED = "file.created"
     FILE_DIRECTORY = "file.directory"
     FILE_DIRECTORY_ID = "file.directoryId"
     FILE_HASH_MD5 = "file.hash.md5"
@@ -79,31 +102,47 @@
     FILE_HASH_SHA256 = "file.hash.sha256"
     FILE_HASH_SHA256_ERROR = "file.hash.sha256Error"
     FILE_ID = "file.id"
     FILE_MIME_TYPE_BY_BYTES = "file.mimeTypeByBytes"
     FILE_MIME_TYPE_BY_EXTENSION = "file.mimeTypeByExtension"
     FILE_MODIFIED = "file.modified"
     FILE_NAME = "file.name"
+    FILE_ORIGINAL_NAME = "file.originalName"
+    FILE_ORIGINAL_DIRECTORY = "file.originalDirectory"
     FILE_OWNER = "file.owner"
     FILE_SIZE_IN_BYTES = "file.sizeInBytes"
     FILE_URL = "file.url"
+    GIT_REPOSITORY_URI = "git.repositoryUri"
+    GIT_LAST_COMMIT_HASH = "git.lastCommitHash"
+    GIT_EVENT_ID = "git.eventId"
+    GIT_REPOSITORY_ENDPOINT_PATH = "git.repositoryEndpointPath"
+    GIT_REPOSITORY_USER = "git.repositoryUser"
+    GIT_REPOSITORY_EMAIL = "git.repositoryEmail"
     PROCESS_EXECUTABLE = "process.executable"
     PROCESS_OWNER = "process.owner"
     REPORT_COUNT = "report.count"
     REPORT_DESCRIPTION = "report.description"
     REPORT_HEADERS = "report.headers"
     REPORT_ID = "report.id"
     REPORT_NAME = "report.name"
     REPORT_TYPE = "report.type"
     RISK_INDICATORS_NAME = "risk.indicators.name"
     RISK_INDICATORS_WEIGHT = "risk.indicators.weight"
+    RISK_INDICATORS_ID = "risk.indicators.id"
     RISK_SCORE = "risk.score"
     RISK_SEVERITY = "risk.severity"
     RISK_TRUST_REASON = "risk.trustReason"
     RISK_TRUSTED = "risk.trusted"
+    RISK_UNTRUSTED_VALUES_GIT_REPOSITORY_URIS = "risk.untrustedValues.gitRepositoryUris"
+    RISK_UNTRUSTED_VALUES_URL_PATHS = "risk.untrustedValues.urlPaths"
+    RISK_UNTRUSTED_VALUES_DOMAINS = "risk.untrustedValues.domains"
+    RISK_UNTRUSTED_VALUES_SLACK_WORKSPACES = "risk.untrustedValues.slackWorkspaces"
+    RISK_UNTRUSTED_VALUES_ACCOUNT_NAMES = "risk.untrustedValues.accountNames"
+    SOURCE_ACCOUNT_TYPE = "source.accountType"
+    SOURCE_ACCOUNT_NAME = "source.accountName"
     SOURCE_CATEGORY = "source.category"
     SOURCE_DOMAIN = "source.domain"
     SOURCE_DOMAINS = "source.domains"
     SOURCE_EMAIL_FROM = "source.email.from"
     SOURCE_EMAIL_SENDER = "source.email.sender"
     SOURCE_IP = "source.ip"
     SOURCE_NAME = "source.name"
@@ -117,14 +156,15 @@
     SOURCE_REMOVABLE_MEDIA_SERIAL_NUMBER = "source.removableMedia.serialNumber"
     SOURCE_REMOVABLE_MEDIA_VENDOR = "source.removableMedia.vendor"
     SOURCE_REMOVABLE_MEDIA_VOLUME_NAME = "source.removableMedia.volumeName"
     SOURCE_TABS_TITLE = "source.tabs.title"
     SOURCE_TABS_TITLE_ERROR = "source.tabs.titleError"
     SOURCE_TABS_URL = "source.tabs.url"
     SOURCE_TABS_URL_ERROR = "source.tabs.urlError"
+    SOURCE_USER_EMAIL = "source.user.email"
     USER_DEVICE_UID = "user.deviceUid"
     USER_EMAIL = "user.email"
     USER_ID = "user.id"
 
 
 class FileCategory(_Enum):
     """Available file categories for filtering file events."""
```

### Comparing `incydr-1.0.1/_incydr_sdk/enums/trusted_activities.py` & `incydr-1.1.0/_incydr_sdk/enums/trusted_activities.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/enums/watchlists.py` & `incydr-1.1.0/_incydr_sdk/enums/watchlists.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/file_events/client.py` & `incydr-1.1.0/_incydr_sdk/file_events/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/file_events/models/event.py` & `incydr-1.1.0/_incydr_sdk/file_events/models/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,67 @@
 from pydantic import Field
 
 from _incydr_sdk.core.models import Model
 from _incydr_sdk.core.models import ResponseModel
 from _incydr_sdk.enums.file_events import ReportType
 
 
+class AcquiredFromGit(Model):
+    repository_email: Optional[str] = Field(
+        None,
+        alias="repositoryEmail",
+        title="The email address specified by the user who performed the Git event. This is a user-defined value and may differ from the credentials used to sign in to Git.",
+    )
+    repository_uri: Optional[str] = Field(
+        None,
+        alias="repositoryUri",
+        title="Uniform Resource Identifier (URI) for the Git repository.",
+    )
+    repository_user: Optional[str] = Field(
+        None,
+        alias="repositoryUser",
+        title="The username specified by the user who performed the Git event. This is a user-defined value and may differ from the credentials used to sign in to Git.",
+    )
+
+
+class AcquiredFromSourceUser(Model):
+    email: Optional[List[str]] = Field(
+        None,
+        example=["first.last@example.com", "first_last_example_com"],
+        title="For endpoint events where a file in cloud storage is synced to a device, the email address of the user logged in to the cloud storage provider.",
+    )
+
+
+class UntrustedValues(Model):
+    account_names: List[str] = Field(
+        ...,
+        alias="accountNames",
+        title="Account names that do not match an entry in your list of Trusted activity. Values are obtained from the account name metadata for the event. Only applies to event types that are evaluated for trust.",
+    )
+    domains: List[str] = Field(
+        ...,
+        title="Domains that do not match an entry in your list of Trusted activity. Values are obtained from the domain section of related metadata for the event. Only applies to event types that are evaluated for trust.",
+    )
+    git_repository_uris: List[str] = Field(
+        ...,
+        alias="gitRepositoryUris",
+        title="Git URIs that do not match an entry in your list of Trusted activity. Values are obtained from the Git URI metadata for the event. Only applies to event types that are evaluated for trust.",
+    )
+    slack_workspaces: List[str] = Field(
+        ...,
+        alias="slackWorkspaces",
+        title="Slack workspaces that do not match an entry in your list of Trusted activity. Values are obtained from the Slack metadata for the event. Only applies to event types that are evaluated for trust.",
+    )
+    url_paths: List[str] = Field(
+        ...,
+        alias="urlPaths",
+        title="URL paths that do not match an entry in your list of Trusted activity. Values are obtained from the URL metadata for the event. Only applies to event types that are evaluated for trust.",
+    )
+
+
 class DestinationEmail(Model):
     recipients: Optional[List[str]] = Field(
         description="The email addresses of those who received the email. Includes the To, Cc, and Bcc recipients.",
         example=["cody@example.com", "theboss@example.com"],
     )
     subject: Optional[str] = Field(
         description="The subject of the email message.",
@@ -140,14 +193,17 @@
 
 
 class RiskIndicator(Model):
     name: Optional[str] = Field(
         description="Name of the risk indicator.",
         example="Browser upload",
     )
+    id: Optional[str] = Field(
+        None, title="The unique identifier for the risk indicator."
+    )
     weight: Optional[int] = Field(
         description="Configured weight of the risk indicator at the time this event was seen.",
         example=5,
     )
 
 
 class SourceEmail(Model):
@@ -204,71 +260,82 @@
     id: Optional[str] = Field(
         description="Unique identifier for the user of the Code42 app on the device. Null if the file event occurred on a cloud provider.",
         example=1138,
     )
 
 
 class AcquiredFrom(Model):
-    agent_timestamp: Optional[datetime] = Field(
-        None,
-        alias="agentTimestamp",
-        description="Date and time that the Code42 service on the device detected an event; based on the device’s system clock and reported in Coordinated Universal Time (UTC).",
-        example="2020-10-27T15:16:05.369203Z",
-    )
-    event_action: Optional[str] = Field(
-        None,
-        alias="eventAction",
-        description="The type of file event observed. For example: file-modified, application-read, removable-media-created.",
-        example="file-downloaded",
-    )
     event_id: Optional[str] = Field(
         None,
         alias="eventId",
-        description="The unique identifier for the event.",
         example="0_147e9445-2f30-4a91-8b2a-9455332e880a_973435567569502913_986467523038446097_163",
+        title="The unique identifier for the event.",
     )
-    file_name: Optional[str] = Field(
+    tabs: Optional[List[Tab]] = Field(
+        None, title="Metadata about the browser tab source."
+    )
+    source_account_name: Optional[str] = Field(
         None,
-        alias="fileName",
-        description="The name of the file, including the file extension.",
-        example="example.txt",
+        alias="sourceAccountName",
+        title="For cloud sync apps installed on user devices, the name of the cloud account where the event was observed. This can help identify if the activity occurred in a business or personal account.",
     )
-    md5: Optional[str] = Field(
+    source_account_type: Optional[str] = Field(
         None,
-        description="The MD5 hash of the file contents.",
-        example="6123bbce7f3937667a368bbb9f3d79ce",
+        alias="sourceAccountType",
+        title="For cloud sync apps installed on user devices, the type of account where the event was observed. For example, 'BUSINESS' or 'PERSONAL'.",
     )
     source_category: Optional[str] = Field(
         None,
         alias="sourceCategory",
-        description="General category of where the file originated. For example: Cloud Storage, Email, Social Media.",
         example="Social Media",
-    )
-    source_domains: Optional[List[str]] = Field(
-        None,
-        alias="sourceDomains",
-        description="The domain section of the URLs reported in file.acquiredFrom.tabs.url.",
-        example="example.com",
+        title="General category of where the file originated. For example: Cloud Storage, Email, Social Media.",
     )
     source_name: Optional[str] = Field(
         None,
         alias="sourceName",
-        description="The name reported by the device's operating system.  This may be different than the device name in the Code42 console.",
         example="Mari's MacBook",
+        title="The name reported by the device's operating system.  This may be different than the device name in the Code42 console.",
     )
-    tabs: Optional[List[Tab]] = Field(
+    source_user: Optional[AcquiredFromSourceUser] = Field(None, alias="sourceUser")
+    agent_timestamp: Optional[datetime] = Field(
         None,
-        description="Metadata about the browser tab source.",
+        alias="agentTimestamp",
+        example="2020-10-27T15:16:05.369203Z",
+        title="Date and time that the Code42 service on the device detected an event; based on the device’s system clock and reported in Coordinated Universal Time (UTC).",
     )
     user_email: Optional[str] = Field(
         None,
         alias="userEmail",
-        description="The Code42 username used to sign in to the Code42 app on the device (for endpoint events) or the cloud service username of the person who caused the event (for cloud events).",
         example="cody@example.com",
+        title="The Code42 username used to sign in to the Code42 app on the device (for endpoint events) or the cloud service username of the person who caused the event (for cloud events).",
+    )
+    event_action: Optional[str] = Field(
+        None,
+        alias="eventAction",
+        example="file-downloaded",
+        title="The type of file event observed. For example: file-modified, application-read, removable-media-created.",
     )
+    source_domains: Optional[List[str]] = Field(
+        None,
+        alias="sourceDomains",
+        example="example.com",
+        title="The domain section of the URLs reported in file.acquiredFrom.tabs.url.",
+    )
+    file_name: Optional[str] = Field(
+        None,
+        alias="fileName",
+        example="example.txt",
+        title="The name of the file, including the file extension.",
+    )
+    md5: Optional[str] = Field(
+        None,
+        example="6123bbce7f3937667a368bbb9f3d79ce",
+        title="The MD5 hash of the file contents.",
+    )
+    git: Optional[AcquiredFromGit] = None
 
 
 class Destination(Model):
     account_name: Optional[str] = Field(
         alias="accountName",
         description="For cloud sync apps installed on user devices, the name of the cloud account where the event was observed. This can help identify if the activity occurred in a business or personal account.",
     )
@@ -322,14 +389,19 @@
     )
     tabs: Optional[List[Tab]] = Field(
         description="Metadata about the browser tab destination.",
     )
     user: Optional[DestinationUser] = Field(
         description="Metadata about the destination user."
     )
+    remote_hostname: Optional[str] = Field(
+        None,
+        alias="remoteHostname",
+        title="For events where a file transfer tool was used, the destination hostname.",
+    )
 
 
 class File(Model):
     acquired_from: Optional[List[AcquiredFrom]] = Field(None, alias="acquiredFrom")
     category: Optional[str] = Field(
         description="A categorization of the file that is inferred from MIME type.",
         example="Audio",
@@ -362,14 +434,20 @@
         description="File creation timestamp as reported by the device's operating system in Coordinated Universal Time (UTC); available for Mac and Windows NTFS devices only.",
         example="2020-10-27T15:16:05.369203Z",
     )
     directory: Optional[str] = Field(
         description="The file location on the user's device; a forward or backslash must be included at the end of the filepath. Possibly null if the file event occurred on a cloud provider.",
         example="/Users/alix/Documents/",
     )
+    original_directory: Optional[str] = Field(
+        None,
+        alias="originalDirectory",
+        example="/Users/alix/Documents/",
+        title="The original file location on the user’s device or cloud service location; a forward or backslash must be included at the end of the filepath. Possibly null if the file event occurred on a cloud provider.",
+    )
     directory_id: Optional[List[str]] = Field(
         alias="directoryId",
         description="Unique identifiers of the parent drives that contain the file; searching on directoryId will return events for all of the files contained in the parent drive.",
         example=["1234", "56d78"],
     )
     hash: Optional[Hash] = Field(description="Hash values of the file.")
     id: Optional[str] = Field(
@@ -390,14 +468,20 @@
         description="File modification timestamp as reported by the device's operating system.  This only indicates changes to file contents.  Changes to file permissions, file owner, or other metadata are not reflected in this timestamp.  Date is reported in Coordinated Universal Time (UTC).",
         example="2020-10-27T15:16:05.369203Z",
     )
     name: Optional[str] = Field(
         description="The name of the file, including the file extension.",
         example="ReadMe.md",
     )
+    original_name: Optional[str] = Field(
+        None,
+        alias="originalName",
+        example="ReadMe.md",
+        title="The original name of the file, including the file extension.",
+    )
     owner: Optional[str] = Field(
         description="The name of the user who owns the file as reported by the device's file system.",
         example="ari.example",
     )
     size_in_bytes: Optional[int] = Field(
         alias="sizeInBytes", description="Size of the file in bytes.", example=256
     )
@@ -424,14 +508,15 @@
         description="The reason the event is trusted. trustReason is only populated if trusted is true for this event.",
         example="TRUSTED_DOMAIN_BROWSER_URL",
     )
     trusted: Optional[bool] = Field(
         description="Indicates whether or not the file activity is trusted based on your Data Preferences settings.",
         example=True,
     )
+    untrusted_values: UntrustedValues = Field(..., alias="untrustedValues")
 
 
 class Source(Model):
     account_name: Optional[str] = Field(
         None,
         alias="accountName",
         description="For cloud sync apps installed on user devices, the name of the cloud account where the event was observed. This can help identify if the activity occurred in a business or personal account.",
@@ -535,14 +620,19 @@
         description="Date and time the event processing is completed by Code42; timestamp is based on the Code42 server system clock and reported in Coordinated Universal Time (UTC). Typically occurs very soon after the event.ingested time.",
         example="2020-10-27T15:16:05.369203Z",
     )
     observer: Optional[str] = Field(
         description="The data source that captured the file event. For example: GoogleDrive, Office365, Salesforce.",
         example="Endpoint",
     )
+    detector_display_name: Optional[str] = Field(
+        None,
+        alias="detectorDisplayName",
+        title="Indicates the name you provided when the cloud data connection was initially configured in the Code42 console.",
+    )
     related_events: Optional[List[RelatedEvent]] = Field(
         alias="relatedEvents",
         description="List of other events associated with this file. This can help determine the origin of the file.",
     )
     share_type: Optional[List[str]] = Field(
         alias="shareType",
         description="Sharing types added by this event.",
```

### Comparing `incydr-1.0.1/_incydr_sdk/file_events/models/response.py` & `incydr-1.1.0/_incydr_sdk/file_events/models/response.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/queries/alerts.py` & `incydr-1.1.0/_incydr_sdk/queries/alerts.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/queries/file_events.py` & `incydr-1.1.0/_incydr_sdk/queries/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/queries/utils.py` & `incydr-1.1.0/_incydr_sdk/queries/utils.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/trusted_activities/client.py` & `incydr-1.1.0/_incydr_sdk/trusted_activities/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/trusted_activities/models.py` & `incydr-1.1.0/_incydr_sdk/trusted_activities/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/user_risk_profiles/client.py` & `incydr-1.1.0/_incydr_sdk/user_risk_profiles/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/user_risk_profiles/models.py` & `incydr-1.1.0/_incydr_sdk/user_risk_profiles/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/users/client.py` & `incydr-1.1.0/_incydr_sdk/users/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,16 @@
         """
         Remove a role, or multiple roles, from a user's current roles.
 
         **Parameters**:
 
         * **user_id**: `str` (required) - The unique ID for the user.
         * **roles**: `str | List[str]` The roles to remove from the user. Accepts either role IDs or role names."
+
+        **Returns**: A `requests.Response` indicating success.
         """
         roles = self._update_role_ids_for_user(roles, user_id, add=False)
         response = self._parent.session.put(
             f"/v1/users/{user_id}/roles", json={"roleIds": roles}
         )
         return UpdateRolesResponse.parse_response(response)
 
@@ -264,49 +266,49 @@
         Activate a user.
 
         **Parameters:**
 
         * **user_id**: `str` (required) - The unique ID for the user.
 
         **Returns**: A `requests.Response` indicating success.
-
         """
         return self._parent.session.post(f"/v1/users/{user_id}/activate")
 
     def deactivate(self, user_id: str) -> Response:
         """
         Deactivate a user.
 
         **Parameters:**
 
         * **user_id**: `str` (required) - The unique ID for the user.
 
         **Returns**: A `requests.Response` indicating success.
-
         """
         return self._parent.session.post(f"/v1/users/{user_id}/deactivate")
 
     def list_roles(self) -> List[Role]:
         """
         Get a list of all available roles that can be assigned by the current user.
 
         **Parameters**:
 
-        **Returns**: A list of [`UserRole`][role-model] objects.
+        **Returns**: A list of [`Role`][role-model] objects.
         """
         response = self._parent.session.get("/v1/users/roles")
         return parse_obj_as(List[Role], response.json())
 
     def get_role(self, role: str) -> Role:
         """
         Get details for a single role.
 
         **Parameters**:
 
         * **role**: `str` (required) - Role ID or role name (case-sensitive).
+
+        **Returns**: A [`Role`](role-model) object.
         """
         response = self._parent.session.get(
             f"/v1/users/roles/{self._get_id_by_name(role)}"
         )
         return Role.parse_response(response)
 
     def _get_id_by_name(self, role_name: str):
```

### Comparing `incydr-1.0.1/_incydr_sdk/users/models.py` & `incydr-1.1.0/_incydr_sdk/users/models.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/watchlists/client.py` & `incydr-1.1.0/_incydr_sdk/watchlists/client.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/watchlists/models/requests.py` & `incydr-1.1.0/_incydr_sdk/watchlists/models/requests.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/_incydr_sdk/watchlists/models/responses.py` & `incydr-1.1.0/_incydr_sdk/watchlists/models/responses.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/incydr/__init__.py` & `incydr-1.1.0/incydr/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 # SPDX-FileCopyrightText: 2022-present Code42 Software <integrations@code42.com>
 #
 # SPDX-License-Identifier: MIT
+from . import enums
 from . import models
+from _incydr_sdk import exceptions
 from _incydr_sdk.__version__ import __version__
 from _incydr_sdk.core.client import Client
 from _incydr_sdk.queries.alerts import AlertQuery
 from _incydr_sdk.queries.file_events import EventQuery
 
-__all__ = ["__version__", "Client", "AlertQuery", "EventQuery", "models"]
+__all__ = [
+    "__version__",
+    "Client",
+    "AlertQuery",
+    "EventQuery",
+    "models",
+    "exceptions",
+]
 
 __locals = locals()
 for __name in __all__:
     if not __name.startswith("__"):
         setattr(__locals[__name], "__module__", "incydr")  # noqa
```

### Comparing `incydr-1.0.1/incydr/models.py` & `incydr-1.1.0/incydr/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from _incydr_sdk.agents.models import Agent
+from _incydr_sdk.agents.models import AgentsPage
 from _incydr_sdk.alert_rules.models.response import RuleDetails
 from _incydr_sdk.alert_rules.models.response import RuleUser
 from _incydr_sdk.alert_rules.models.response import RuleUsersList
 from _incydr_sdk.alerts.models.alert import AlertDetails
 from _incydr_sdk.alerts.models.alert import AlertSummary
 from _incydr_sdk.alerts.models.response import AlertQueryPage
 from _incydr_sdk.audit_log.models import AuditEventsPage
@@ -34,14 +36,16 @@
 from _incydr_sdk.watchlists.models.responses import IncludedUsersList
 from _incydr_sdk.watchlists.models.responses import Watchlist
 from _incydr_sdk.watchlists.models.responses import WatchlistMembersList
 from _incydr_sdk.watchlists.models.responses import WatchlistsPage
 from _incydr_sdk.watchlists.models.responses import WatchlistUser
 
 __all__ = [
+    "Agent",
+    "AgentsPage",
     "AlertDetails",
     "AlertSummary",
     "AlertQueryPage",
     "Case",
     "CaseFileEvents",
     "CasesPage",
     "Customer",
```

### Comparing `incydr-1.0.1/incydr/enums/file_events.py` & `incydr-1.1.0/incydr/enums/file_events.py`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/LICENSE.txt` & `incydr-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/README.md` & `incydr-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/pyproject.toml` & `incydr-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `incydr-1.0.1/PKG-INFO` & `incydr-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incydr
-Version: 1.0.1
+Version: 1.1.0
 Summary: Code42's Incydr Python SDK
 Project-URL: Documentation, https://github.com/code42/incydr_python#readme
 Project-URL: Issues, https://github.com/code42/incydr_python/issues
 Project-URL: Source, https://github.com/code42/incydr_python/incydr
 Author-email: Code42 <integrations@code42.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

