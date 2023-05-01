# Comparing `tmp/cloudsmith_api-2.0.1-py2.py3-none-any.whl.zip` & `tmp/cloudsmith_api-2.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,357 +1,409 @@
-Zip file size: 645422 bytes, number of entries: 355
--rw-r--r--  2.0 unx    13188 b- defN 23-Jan-03 10:07 cloudsmith_api/__init__.py
--rw-r--r--  2.0 unx    25067 b- defN 23-Jan-03 10:07 cloudsmith_api/api_client.py
--rw-r--r--  2.0 unx     8390 b- defN 23-Jan-03 10:07 cloudsmith_api/configuration.py
--rw-r--r--  2.0 unx    13166 b- defN 23-Jan-03 10:07 cloudsmith_api/rest.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Jan-03 10:07 cloudsmith_api/api/__init__.py
--rw-r--r--  2.0 unx    11039 b- defN 23-Jan-03 10:07 cloudsmith_api/api/audit_log_api.py
--rw-r--r--  2.0 unx    11425 b- defN 23-Jan-03 10:07 cloudsmith_api/api/badges_api.py
--rw-r--r--  2.0 unx     7978 b- defN 23-Jan-03 10:07 cloudsmith_api/api/distros_api.py
--rw-r--r--  2.0 unx    54786 b- defN 23-Jan-03 10:07 cloudsmith_api/api/entitlements_api.py
--rw-r--r--  2.0 unx    26620 b- defN 23-Jan-03 10:07 cloudsmith_api/api/files_api.py
--rw-r--r--  2.0 unx     7930 b- defN 23-Jan-03 10:07 cloudsmith_api/api/formats_api.py
--rw-r--r--  2.0 unx    19214 b- defN 23-Jan-03 10:07 cloudsmith_api/api/metrics_api.py
--rw-r--r--  2.0 unx     8514 b- defN 23-Jan-03 10:07 cloudsmith_api/api/namespaces_api.py
--rw-r--r--  2.0 unx   129747 b- defN 23-Jan-03 10:07 cloudsmith_api/api/orgs_api.py
--rw-r--r--  2.0 unx   275486 b- defN 23-Jan-03 10:07 cloudsmith_api/api/packages_api.py
--rw-r--r--  2.0 unx    16386 b- defN 23-Jan-03 10:07 cloudsmith_api/api/quota_api.py
--rw-r--r--  2.0 unx     4157 b- defN 23-Jan-03 10:07 cloudsmith_api/api/rates_api.py
--rw-r--r--  2.0 unx    84121 b- defN 23-Jan-03 10:07 cloudsmith_api/api/repos_api.py
--rw-r--r--  2.0 unx     4118 b- defN 23-Jan-03 10:07 cloudsmith_api/api/status_api.py
--rw-r--r--  2.0 unx     8075 b- defN 23-Jan-03 10:07 cloudsmith_api/api/storage_regions_api.py
--rw-r--r--  2.0 unx     7631 b- defN 23-Jan-03 10:07 cloudsmith_api/api/user_api.py
--rw-r--r--  2.0 unx     4706 b- defN 23-Jan-03 10:07 cloudsmith_api/api/users_api.py
--rw-r--r--  2.0 unx    22056 b- defN 23-Jan-03 10:07 cloudsmith_api/api/vulnerabilities_api.py
--rw-r--r--  2.0 unx    26050 b- defN 23-Jan-03 10:07 cloudsmith_api/api/webhooks_api.py
--rw-r--r--  2.0 unx    11991 b- defN 23-Jan-03 10:07 cloudsmith_api/models/__init__.py
--rw-r--r--  2.0 unx     7305 b- defN 23-Jan-03 10:07 cloudsmith_api/models/allocated_limit.py
--rw-r--r--  2.0 unx    58771 b- defN 23-Jan-03 10:07 cloudsmith_api/models/alpine_package_upload.py
--rw-r--r--  2.0 unx     7437 b- defN 23-Jan-03 10:07 cloudsmith_api/models/alpine_package_upload_request.py
--rw-r--r--  2.0 unx     4748 b- defN 23-Jan-03 10:07 cloudsmith_api/models/architecture.py
--rw-r--r--  2.0 unx    58494 b- defN 23-Jan-03 10:07 cloudsmith_api/models/cargo_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-Jan-03 10:07 cloudsmith_api/models/cargo_package_upload_request.py
--rw-r--r--  2.0 unx    59602 b- defN 23-Jan-03 10:07 cloudsmith_api/models/cocoapods_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-Jan-03 10:07 cloudsmith_api/models/cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx     6052 b- defN 23-Jan-03 10:07 cloudsmith_api/models/common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     5636 b- defN 23-Jan-03 10:07 cloudsmith_api/models/common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx     6052 b- defN 23-Jan-03 10:07 cloudsmith_api/models/common_downloads_metrics.py
--rw-r--r--  2.0 unx     3526 b- defN 23-Jan-03 10:07 cloudsmith_api/models/common_downloads_metrics_value.py
--rw-r--r--  2.0 unx     6129 b- defN 23-Jan-03 10:07 cloudsmith_api/models/common_metrics.py
--rw-r--r--  2.0 unx    59325 b- defN 23-Jan-03 10:07 cloudsmith_api/models/composer_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-Jan-03 10:07 cloudsmith_api/models/composer_package_upload_request.py
--rw-r--r--  2.0 unx    61539 b- defN 23-Jan-03 10:07 cloudsmith_api/models/conan_package_upload.py
--rw-r--r--  2.0 unx    14491 b- defN 23-Jan-03 10:07 cloudsmith_api/models/conan_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-Jan-03 10:07 cloudsmith_api/models/conda_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-Jan-03 10:07 cloudsmith_api/models/conda_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jan-03 10:07 cloudsmith_api/models/cran_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jan-03 10:07 cloudsmith_api/models/cran_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jan-03 10:07 cloudsmith_api/models/dart_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jan-03 10:07 cloudsmith_api/models/dart_package_upload_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jan-03 10:07 cloudsmith_api/models/deb_package_upload.py
--rw-r--r--  2.0 unx     9690 b- defN 23-Jan-03 10:07 cloudsmith_api/models/deb_package_upload_request.py
--rw-r--r--  2.0 unx     6159 b- defN 23-Jan-03 10:07 cloudsmith_api/models/distribution.py
--rw-r--r--  2.0 unx     8542 b- defN 23-Jan-03 10:07 cloudsmith_api/models/distribution_full.py
--rw-r--r--  2.0 unx     4497 b- defN 23-Jan-03 10:07 cloudsmith_api/models/distribution_version.py
--rw-r--r--  2.0 unx    58771 b- defN 23-Jan-03 10:07 cloudsmith_api/models/docker_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Jan-03 10:07 cloudsmith_api/models/docker_package_upload_request.py
--rw-r--r--  2.0 unx     3541 b- defN 23-Jan-03 10:07 cloudsmith_api/models/entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     3729 b- defN 23-Jan-03 10:07 cloudsmith_api/models/error_detail.py
--rw-r--r--  2.0 unx     5590 b- defN 23-Jan-03 10:07 cloudsmith_api/models/eula.py
--rw-r--r--  2.0 unx    11287 b- defN 23-Jan-03 10:07 cloudsmith_api/models/format.py
--rw-r--r--  2.0 unx     7319 b- defN 23-Jan-03 10:07 cloudsmith_api/models/format_support.py
--rw-r--r--  2.0 unx     8615 b- defN 23-Jan-03 10:07 cloudsmith_api/models/geo_ip_location.py
--rw-r--r--  2.0 unx    57663 b- defN 23-Jan-03 10:07 cloudsmith_api/models/go_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-Jan-03 10:07 cloudsmith_api/models/go_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jan-03 10:07 cloudsmith_api/models/helm_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jan-03 10:07 cloudsmith_api/models/helm_package_upload_request.py
--rw-r--r--  2.0 unx     7019 b- defN 23-Jan-03 10:07 cloudsmith_api/models/history.py
--rw-r--r--  2.0 unx     5147 b- defN 23-Jan-03 10:07 cloudsmith_api/models/history_fieldset.py
--rw-r--r--  2.0 unx     4150 b- defN 23-Jan-03 10:07 cloudsmith_api/models/inline_response200.py
--rw-r--r--  2.0 unx     4039 b- defN 23-Jan-03 10:07 cloudsmith_api/models/inline_response200_country_code.py
--rw-r--r--  2.0 unx    59325 b- defN 23-Jan-03 10:07 cloudsmith_api/models/luarocks_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-Jan-03 10:07 cloudsmith_api/models/luarocks_package_upload_request.py
--rw-r--r--  2.0 unx    61667 b- defN 23-Jan-03 10:07 cloudsmith_api/models/maven_package_upload.py
--rw-r--r--  2.0 unx    14513 b- defN 23-Jan-03 10:07 cloudsmith_api/models/maven_package_upload_request.py
--rw-r--r--  2.0 unx     5806 b- defN 23-Jan-03 10:07 cloudsmith_api/models/namespace.py
--rw-r--r--  2.0 unx    18223 b- defN 23-Jan-03 10:07 cloudsmith_api/models/namespace_audit_log.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jan-03 10:07 cloudsmith_api/models/npm_package_upload.py
--rw-r--r--  2.0 unx     7663 b- defN 23-Jan-03 10:07 cloudsmith_api/models/npm_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-Jan-03 10:07 cloudsmith_api/models/nuget_package_upload.py
--rw-r--r--  2.0 unx     7272 b- defN 23-Jan-03 10:07 cloudsmith_api/models/nuget_package_upload_request.py
--rw-r--r--  2.0 unx     7918 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization.py
--rw-r--r--  2.0 unx     8617 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_group_sync.py
--rw-r--r--  2.0 unx     8449 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_group_sync_request.py
--rw-r--r--  2.0 unx    10169 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_invite.py
--rw-r--r--  2.0 unx    10519 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_invite_extend.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_invite_request.py
--rw-r--r--  2.0 unx     3821 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_invite_update.py
--rw-r--r--  2.0 unx     3929 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx    12300 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_membership.py
--rw-r--r--  2.0 unx     8110 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_team.py
--rw-r--r--  2.0 unx     3669 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_team_members.py
--rw-r--r--  2.0 unx     4783 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_team_membership.py
--rw-r--r--  2.0 unx     7065 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_team_request.py
--rw-r--r--  2.0 unx     7040 b- defN 23-Jan-03 10:07 cloudsmith_api/models/organization_team_request_patch.py
--rw-r--r--  2.0 unx    57663 b- defN 23-Jan-03 10:07 cloudsmith_api/models/p2_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-Jan-03 10:07 cloudsmith_api/models/p2_package_upload_request.py
--rw-r--r--  2.0 unx    55965 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package.py
--rw-r--r--  2.0 unx    57197 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_copy.py
--rw-r--r--  2.0 unx     4776 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_copy_request.py
--rw-r--r--  2.0 unx     3661 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_dependencies.py
--rw-r--r--  2.0 unx     7227 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_dependency.py
--rw-r--r--  2.0 unx    12968 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_file.py
--rw-r--r--  2.0 unx     6108 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_file_parts_upload.py
--rw-r--r--  2.0 unx     7841 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_file_upload.py
--rw-r--r--  2.0 unx     7815 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_file_upload_request.py
--rw-r--r--  2.0 unx    57195 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_move.py
--rw-r--r--  2.0 unx     3820 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_move_request.py
--rw-r--r--  2.0 unx    58775 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_quarantine.py
--rw-r--r--  2.0 unx     3527 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_quarantine_request.py
--rw-r--r--  2.0 unx    57651 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_resync.py
--rw-r--r--  2.0 unx    15877 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_status.py
--rw-r--r--  2.0 unx    57199 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_tag.py
--rw-r--r--  2.0 unx     4991 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_tag_request.py
--rw-r--r--  2.0 unx     3547 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_usage_metrics.py
--rw-r--r--  2.0 unx     2740 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_version_badge.py
--rw-r--r--  2.0 unx     5707 b- defN 23-Jan-03 10:07 cloudsmith_api/models/package_vulnerability.py
--rw-r--r--  2.0 unx    58771 b- defN 23-Jan-03 10:07 cloudsmith_api/models/python_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Jan-03 10:07 cloudsmith_api/models/python_package_upload_request.py
--rw-r--r--  2.0 unx     3358 b- defN 23-Jan-03 10:07 cloudsmith_api/models/quota.py
--rw-r--r--  2.0 unx     3463 b- defN 23-Jan-03 10:07 cloudsmith_api/models/quota_history.py
--rw-r--r--  2.0 unx     7675 b- defN 23-Jan-03 10:07 cloudsmith_api/models/rate_check.py
--rw-r--r--  2.0 unx    58899 b- defN 23-Jan-03 10:07 cloudsmith_api/models/raw_package_upload.py
--rw-r--r--  2.0 unx    11674 b- defN 23-Jan-03 10:07 cloudsmith_api/models/raw_package_upload_request.py
--rw-r--r--  2.0 unx    66225 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository.py
--rw-r--r--  2.0 unx    14861 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_audit_log.py
--rw-r--r--  2.0 unx    67551 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_create.py
--rw-r--r--  2.0 unx    52992 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_create_request.py
--rw-r--r--  2.0 unx     4272 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_geo_ip_list.py
--rw-r--r--  2.0 unx     8734 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_gpg_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_gpg_key_create.py
--rw-r--r--  2.0 unx     7702 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_privilege_dict.py
--rw-r--r--  2.0 unx     3818 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_privilege_input.py
--rw-r--r--  2.0 unx     3881 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_privilege_input_request.py
--rw-r--r--  2.0 unx     3790 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx    51803 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_request_patch.py
--rw-r--r--  2.0 unx     7753 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_rsa_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_rsa_key_create.py
--rw-r--r--  2.0 unx    40082 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token.py
--rw-r--r--  2.0 unx     2750 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_action.py
--rw-r--r--  2.0 unx    41079 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_refresh.py
--rw-r--r--  2.0 unx    21728 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_refresh_request.py
--rw-r--r--  2.0 unx    22234 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_request.py
--rw-r--r--  2.0 unx    22429 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_request_patch.py
--rw-r--r--  2.0 unx     3505 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_sync.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_token_sync_request.py
--rw-r--r--  2.0 unx    30400 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_webhook.py
--rw-r--r--  2.0 unx    18912 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_webhook_request.py
--rw-r--r--  2.0 unx    18774 b- defN 23-Jan-03 10:07 cloudsmith_api/models/repository_webhook_request_patch.py
--rw-r--r--  2.0 unx     3523 b- defN 23-Jan-03 10:07 cloudsmith_api/models/resources_rate_check.py
--rw-r--r--  2.0 unx     2790 b- defN 23-Jan-03 10:07 cloudsmith_api/models/respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     2825 b- defN 23-Jan-03 10:07 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-Jan-03 10:07 cloudsmith_api/models/rpm_package_upload.py
--rw-r--r--  2.0 unx     7374 b- defN 23-Jan-03 10:07 cloudsmith_api/models/rpm_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-Jan-03 10:07 cloudsmith_api/models/ruby_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-Jan-03 10:07 cloudsmith_api/models/ruby_package_upload_request.py
--rw-r--r--  2.0 unx     8234 b- defN 23-Jan-03 10:07 cloudsmith_api/models/service.py
--rw-r--r--  2.0 unx     6726 b- defN 23-Jan-03 10:07 cloudsmith_api/models/service_request.py
--rw-r--r--  2.0 unx     6701 b- defN 23-Jan-03 10:07 cloudsmith_api/models/service_request_patch.py
--rw-r--r--  2.0 unx     4821 b- defN 23-Jan-03 10:07 cloudsmith_api/models/service_teams.py
--rw-r--r--  2.0 unx     4584 b- defN 23-Jan-03 10:07 cloudsmith_api/models/status_basic.py
--rw-r--r--  2.0 unx     4670 b- defN 23-Jan-03 10:07 cloudsmith_api/models/storage_region.py
--rw-r--r--  2.0 unx     2665 b- defN 23-Jan-03 10:07 cloudsmith_api/models/tags.py
--rw-r--r--  2.0 unx    59602 b- defN 23-Jan-03 10:07 cloudsmith_api/models/terraform_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-Jan-03 10:07 cloudsmith_api/models/terraform_package_upload_request.py
--rw-r--r--  2.0 unx     5738 b- defN 23-Jan-03 10:07 cloudsmith_api/models/usage.py
--rw-r--r--  2.0 unx     4138 b- defN 23-Jan-03 10:07 cloudsmith_api/models/usage_fieldset.py
--rw-r--r--  2.0 unx     4256 b- defN 23-Jan-03 10:07 cloudsmith_api/models/usage_limits.py
--rw-r--r--  2.0 unx     3590 b- defN 23-Jan-03 10:07 cloudsmith_api/models/user_auth_token.py
--rw-r--r--  2.0 unx     4612 b- defN 23-Jan-03 10:07 cloudsmith_api/models/user_auth_token_request.py
--rw-r--r--  2.0 unx     8019 b- defN 23-Jan-03 10:07 cloudsmith_api/models/user_brief.py
--rw-r--r--  2.0 unx    11110 b- defN 23-Jan-03 10:07 cloudsmith_api/models/user_profile.py
--rw-r--r--  2.0 unx    60899 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vagrant_package_upload.py
--rw-r--r--  2.0 unx     9492 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vagrant_package_upload_request.py
--rw-r--r--  2.0 unx    13112 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vulnerability.py
--rw-r--r--  2.0 unx     5400 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vulnerability_scan.py
--rw-r--r--  2.0 unx    10040 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vulnerability_scan_results.py
--rw-r--r--  2.0 unx     9417 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx     8443 b- defN 23-Jan-03 10:07 cloudsmith_api/models/vulnerability_scan_version.py
--rw-r--r--  2.0 unx     4751 b- defN 23-Jan-03 10:07 cloudsmith_api/models/webhook_template.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-03 10:07 test/__init__.py
--rw-r--r--  2.0 unx      900 b- defN 23-Jan-03 10:07 test/test_allocated_limit.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_alpine_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jan-03 10:07 test/test_alpine_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-Jan-03 10:07 test/test_architecture.py
--rw-r--r--  2.0 unx     1083 b- defN 23-Jan-03 10:07 test/test_audit_log_api.py
--rw-r--r--  2.0 unx      883 b- defN 23-Jan-03 10:07 test/test_badges_api.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_cargo_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jan-03 10:07 test/test_cargo_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_cocoapods_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jan-03 10:07 test/test_cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jan-03 10:07 test/test_common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_common_downloads_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jan-03 10:07 test/test_common_downloads_metrics_value.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jan-03 10:07 test/test_common_metrics.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jan-03 10:07 test/test_composer_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-03 10:07 test/test_composer_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_conan_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jan-03 10:07 test/test_conan_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_conda_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jan-03 10:07 test/test_conda_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_cran_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jan-03 10:07 test/test_cran_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_dart_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jan-03 10:07 test/test_dart_package_upload_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jan-03 10:07 test/test_deb_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jan-03 10:07 test/test_deb_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-Jan-03 10:07 test/test_distribution.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jan-03 10:07 test/test_distribution_full.py
--rw-r--r--  2.0 unx      940 b- defN 23-Jan-03 10:07 test/test_distribution_version.py
--rw-r--r--  2.0 unx     1019 b- defN 23-Jan-03 10:07 test/test_distros_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_docker_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jan-03 10:07 test/test_docker_package_upload_request.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jan-03 10:07 test/test_entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     2550 b- defN 23-Jan-03 10:07 test/test_entitlements_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_error_detail.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jan-03 10:07 test/test_eula.py
--rw-r--r--  2.0 unx     1503 b- defN 23-Jan-03 10:07 test/test_files_api.py
--rw-r--r--  2.0 unx      834 b- defN 23-Jan-03 10:07 test/test_format.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jan-03 10:07 test/test_format_support.py
--rw-r--r--  2.0 unx     1022 b- defN 23-Jan-03 10:07 test/test_formats_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-Jan-03 10:07 test/test_geo_ip_location.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jan-03 10:07 test/test_go_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jan-03 10:07 test/test_go_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_helm_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jan-03 10:07 test/test_helm_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jan-03 10:07 test/test_history.py
--rw-r--r--  2.0 unx      908 b- defN 23-Jan-03 10:07 test/test_history_fieldset.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jan-03 10:07 test/test_inline_response200.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-03 10:07 test/test_inline_response200_country_code.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jan-03 10:07 test/test_luarocks_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-03 10:07 test/test_luarocks_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_maven_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jan-03 10:07 test/test_maven_package_upload_request.py
--rw-r--r--  2.0 unx     1335 b- defN 23-Jan-03 10:07 test/test_metrics_api.py
--rw-r--r--  2.0 unx      858 b- defN 23-Jan-03 10:07 test/test_namespace.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_namespace_audit_log.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Jan-03 10:07 test/test_namespaces_api.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jan-03 10:07 test/test_npm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jan-03 10:07 test/test_npm_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_nuget_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jan-03 10:07 test/test_nuget_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-Jan-03 10:07 test/test_organization.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jan-03 10:07 test/test_organization_group_sync.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-03 10:07 test/test_organization_group_sync_request.py
--rw-r--r--  2.0 unx      932 b- defN 23-Jan-03 10:07 test/test_organization_invite.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_organization_invite_extend.py
--rw-r--r--  2.0 unx      990 b- defN 23-Jan-03 10:07 test/test_organization_invite_request.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_organization_invite_update.py
--rw-r--r--  2.0 unx     1082 b- defN 23-Jan-03 10:07 test/test_organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx      964 b- defN 23-Jan-03 10:07 test/test_organization_membership.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jan-03 10:07 test/test_organization_team.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jan-03 10:07 test/test_organization_team_members.py
--rw-r--r--  2.0 unx      998 b- defN 23-Jan-03 10:07 test/test_organization_team_membership.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jan-03 10:07 test/test_organization_team_request.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-03 10:07 test/test_organization_team_request_patch.py
--rw-r--r--  2.0 unx     5914 b- defN 23-Jan-03 10:07 test/test_orgs_api.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jan-03 10:07 test/test_p2_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jan-03 10:07 test/test_p2_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jan-03 10:07 test/test_package.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_package_copy.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_package_copy_request.py
--rw-r--r--  2.0 unx      940 b- defN 23-Jan-03 10:07 test/test_package_dependencies.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jan-03 10:07 test/test_package_dependency.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_package_file.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jan-03 10:07 test/test_package_file_parts_upload.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_package_file_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jan-03 10:07 test/test_package_file_upload_request.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_package_move.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_package_move_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jan-03 10:07 test/test_package_quarantine.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_package_quarantine_request.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jan-03 10:07 test/test_package_resync.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jan-03 10:07 test/test_package_status.py
--rw-r--r--  2.0 unx      868 b- defN 23-Jan-03 10:07 test/test_package_tag.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_package_tag_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_package_usage_metrics.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_package_version_badge.py
--rw-r--r--  2.0 unx      948 b- defN 23-Jan-03 10:07 test/test_package_vulnerability.py
--rw-r--r--  2.0 unx    10990 b- defN 23-Jan-03 10:07 test/test_packages_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_python_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jan-03 10:07 test/test_python_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-Jan-03 10:07 test/test_quota.py
--rw-r--r--  2.0 unx     1364 b- defN 23-Jan-03 10:07 test/test_quota_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-Jan-03 10:07 test/test_quota_history.py
--rw-r--r--  2.0 unx      860 b- defN 23-Jan-03 10:07 test/test_rate_check.py
--rw-r--r--  2.0 unx      862 b- defN 23-Jan-03 10:07 test/test_rates_api.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jan-03 10:07 test/test_raw_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jan-03 10:07 test/test_raw_package_upload_request.py
--rw-r--r--  2.0 unx     3868 b- defN 23-Jan-03 10:07 test/test_repos_api.py
--rw-r--r--  2.0 unx      866 b- defN 23-Jan-03 10:07 test/test_repository.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_repository_audit_log.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jan-03 10:07 test/test_repository_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jan-03 10:07 test/test_repository_create_request.py
--rw-r--r--  2.0 unx      944 b- defN 23-Jan-03 10:07 test/test_repository_geo_ip_list.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jan-03 10:07 test/test_repository_gpg_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jan-03 10:07 test/test_repository_gpg_key_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-Jan-03 10:07 test/test_repository_privilege_dict.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_repository_privilege_input.py
--rw-r--r--  2.0 unx     1040 b- defN 23-Jan-03 10:07 test/test_repository_privilege_input_request.py
--rw-r--r--  2.0 unx     1082 b- defN 23-Jan-03 10:07 test/test_repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_repository_request_patch.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jan-03 10:07 test/test_repository_rsa_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-Jan-03 10:07 test/test_repository_rsa_key_create.py
--rw-r--r--  2.0 unx      908 b- defN 23-Jan-03 10:07 test/test_repository_token.py
--rw-r--r--  2.0 unx      958 b- defN 23-Jan-03 10:07 test/test_repository_token_action.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_repository_token_refresh.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jan-03 10:07 test/test_repository_token_refresh_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_repository_token_request.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jan-03 10:07 test/test_repository_token_request_patch.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_repository_token_sync.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Jan-03 10:07 test/test_repository_token_sync_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jan-03 10:07 test/test_repository_webhook.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_repository_webhook_request.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jan-03 10:07 test/test_repository_webhook_request_patch.py
--rw-r--r--  2.0 unx      934 b- defN 23-Jan-03 10:07 test/test_resources_rate_check.py
--rw-r--r--  2.0 unx     1026 b- defN 23-Jan-03 10:07 test/test_respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     1084 b- defN 23-Jan-03 10:07 test/test_respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-Jan-03 10:07 test/test_rpm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-Jan-03 10:07 test/test_rpm_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-Jan-03 10:07 test/test_ruby_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-Jan-03 10:07 test/test_ruby_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jan-03 10:07 test/test_service.py
--rw-r--r--  2.0 unx      900 b- defN 23-Jan-03 10:07 test/test_service_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jan-03 10:07 test/test_service_request_patch.py
--rw-r--r--  2.0 unx      884 b- defN 23-Jan-03 10:07 test/test_service_teams.py
--rw-r--r--  2.0 unx      864 b- defN 23-Jan-03 10:07 test/test_status_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_status_basic.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jan-03 10:07 test/test_storage_region.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Jan-03 10:07 test/test_storage_regions_api.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jan-03 10:07 test/test_tags.py
--rw-r--r--  2.0 unx      966 b- defN 23-Jan-03 10:07 test/test_terraform_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jan-03 10:07 test/test_terraform_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-Jan-03 10:07 test/test_usage.py
--rw-r--r--  2.0 unx      892 b- defN 23-Jan-03 10:07 test/test_usage_fieldset.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_usage_limits.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Jan-03 10:07 test/test_user_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-Jan-03 10:07 test/test_user_auth_token.py
--rw-r--r--  2.0 unx      952 b- defN 23-Jan-03 10:07 test/test_user_auth_token_request.py
--rw-r--r--  2.0 unx      860 b- defN 23-Jan-03 10:07 test/test_user_brief.py
--rw-r--r--  2.0 unx      876 b- defN 23-Jan-03 10:07 test/test_user_profile.py
--rw-r--r--  2.0 unx      865 b- defN 23-Jan-03 10:07 test/test_users_api.py
--rw-r--r--  2.0 unx      950 b- defN 23-Jan-03 10:07 test/test_vagrant_package_upload.py
--rw-r--r--  2.0 unx     1008 b- defN 23-Jan-03 10:07 test/test_vagrant_package_upload_request.py
--rw-r--r--  2.0 unx     1491 b- defN 23-Jan-03 10:07 test/test_vulnerabilities_api.py
--rw-r--r--  2.0 unx      890 b- defN 23-Jan-03 10:07 test/test_vulnerability.py
--rw-r--r--  2.0 unx      924 b- defN 23-Jan-03 10:07 test/test_vulnerability_scan.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_vulnerability_scan_results.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Jan-03 10:07 test/test_vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jan-03 10:07 test/test_vulnerability_scan_version.py
--rw-r--r--  2.0 unx      908 b- defN 23-Jan-03 10:07 test/test_webhook_template.py
--rw-r--r--  2.0 unx     1557 b- defN 23-Jan-03 10:07 test/test_webhooks_api.py
--rw-r--r--  2.0 unx      457 b- defN 23-Jan-03 10:08 cloudsmith_api-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jan-03 10:08 cloudsmith_api-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jan-03 10:08 cloudsmith_api-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    33818 b- defN 23-Jan-03 10:08 cloudsmith_api-2.0.1.dist-info/RECORD
-355 files, 3916713 bytes uncompressed, 591010 bytes compressed:  84.9%
+Zip file size: 711364 bytes, number of entries: 407
+-rw-r--r--  2.0 unx    15755 b- defN 23-May-01 11:28 cloudsmith_api/__init__.py
+-rw-r--r--  2.0 unx    25067 b- defN 23-May-01 11:28 cloudsmith_api/api_client.py
+-rw-r--r--  2.0 unx     8390 b- defN 23-May-01 11:28 cloudsmith_api/configuration.py
+-rw-r--r--  2.0 unx    13166 b- defN 23-May-01 11:28 cloudsmith_api/rest.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-May-01 11:28 cloudsmith_api/api/__init__.py
+-rw-r--r--  2.0 unx    11039 b- defN 23-May-01 11:28 cloudsmith_api/api/audit_log_api.py
+-rw-r--r--  2.0 unx    11425 b- defN 23-May-01 11:28 cloudsmith_api/api/badges_api.py
+-rw-r--r--  2.0 unx     7978 b- defN 23-May-01 11:28 cloudsmith_api/api/distros_api.py
+-rw-r--r--  2.0 unx    54786 b- defN 23-May-01 11:28 cloudsmith_api/api/entitlements_api.py
+-rw-r--r--  2.0 unx    26620 b- defN 23-May-01 11:28 cloudsmith_api/api/files_api.py
+-rw-r--r--  2.0 unx     7930 b- defN 23-May-01 11:28 cloudsmith_api/api/formats_api.py
+-rw-r--r--  2.0 unx    19214 b- defN 23-May-01 11:28 cloudsmith_api/api/metrics_api.py
+-rw-r--r--  2.0 unx     8514 b- defN 23-May-01 11:28 cloudsmith_api/api/namespaces_api.py
+-rw-r--r--  2.0 unx   195413 b- defN 23-May-01 11:28 cloudsmith_api/api/orgs_api.py
+-rw-r--r--  2.0 unx   275618 b- defN 23-May-01 11:28 cloudsmith_api/api/packages_api.py
+-rw-r--r--  2.0 unx    16386 b- defN 23-May-01 11:28 cloudsmith_api/api/quota_api.py
+-rw-r--r--  2.0 unx     4157 b- defN 23-May-01 11:28 cloudsmith_api/api/rates_api.py
+-rw-r--r--  2.0 unx    98642 b- defN 23-May-01 11:28 cloudsmith_api/api/repos_api.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-May-01 11:28 cloudsmith_api/api/status_api.py
+-rw-r--r--  2.0 unx     8075 b- defN 23-May-01 11:28 cloudsmith_api/api/storage_regions_api.py
+-rw-r--r--  2.0 unx     7631 b- defN 23-May-01 11:28 cloudsmith_api/api/user_api.py
+-rw-r--r--  2.0 unx     4706 b- defN 23-May-01 11:28 cloudsmith_api/api/users_api.py
+-rw-r--r--  2.0 unx    22056 b- defN 23-May-01 11:28 cloudsmith_api/api/vulnerabilities_api.py
+-rw-r--r--  2.0 unx    26050 b- defN 23-May-01 11:28 cloudsmith_api/api/webhooks_api.py
+-rw-r--r--  2.0 unx    14558 b- defN 23-May-01 11:28 cloudsmith_api/models/__init__.py
+-rw-r--r--  2.0 unx     7305 b- defN 23-May-01 11:28 cloudsmith_api/models/allocated_limit.py
+-rw-r--r--  2.0 unx     5410 b- defN 23-May-01 11:28 cloudsmith_api/models/allocated_limit_raw.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-01 11:28 cloudsmith_api/models/alpine_package_upload.py
+-rw-r--r--  2.0 unx     7437 b- defN 23-May-01 11:28 cloudsmith_api/models/alpine_package_upload_request.py
+-rw-r--r--  2.0 unx     4748 b- defN 23-May-01 11:28 cloudsmith_api/models/architecture.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-01 11:28 cloudsmith_api/models/cargo_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-May-01 11:28 cloudsmith_api/models/cargo_package_upload_request.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-May-01 11:28 cloudsmith_api/models/cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-May-01 11:28 cloudsmith_api/models/cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-01 11:28 cloudsmith_api/models/common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     5636 b- defN 23-May-01 11:28 cloudsmith_api/models/common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-01 11:28 cloudsmith_api/models/common_downloads_metrics.py
+-rw-r--r--  2.0 unx     3526 b- defN 23-May-01 11:28 cloudsmith_api/models/common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx     6129 b- defN 23-May-01 11:28 cloudsmith_api/models/common_metrics.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-May-01 11:28 cloudsmith_api/models/composer_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-May-01 11:28 cloudsmith_api/models/composer_package_upload_request.py
+-rw-r--r--  2.0 unx    61539 b- defN 23-May-01 11:28 cloudsmith_api/models/conan_package_upload.py
+-rw-r--r--  2.0 unx    14491 b- defN 23-May-01 11:28 cloudsmith_api/models/conan_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-01 11:28 cloudsmith_api/models/conda_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-May-01 11:28 cloudsmith_api/models/conda_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/cran_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/cran_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/dart_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/dart_package_upload_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-01 11:28 cloudsmith_api/models/deb_package_upload.py
+-rw-r--r--  2.0 unx     9690 b- defN 23-May-01 11:28 cloudsmith_api/models/deb_package_upload_request.py
+-rw-r--r--  2.0 unx     6159 b- defN 23-May-01 11:28 cloudsmith_api/models/distribution.py
+-rw-r--r--  2.0 unx     8542 b- defN 23-May-01 11:28 cloudsmith_api/models/distribution_full.py
+-rw-r--r--  2.0 unx     4497 b- defN 23-May-01 11:28 cloudsmith_api/models/distribution_version.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-01 11:28 cloudsmith_api/models/docker_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-May-01 11:28 cloudsmith_api/models/docker_package_upload_request.py
+-rw-r--r--  2.0 unx     3541 b- defN 23-May-01 11:28 cloudsmith_api/models/entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     3729 b- defN 23-May-01 11:28 cloudsmith_api/models/error_detail.py
+-rw-r--r--  2.0 unx     5590 b- defN 23-May-01 11:28 cloudsmith_api/models/eula.py
+-rw-r--r--  2.0 unx    11287 b- defN 23-May-01 11:28 cloudsmith_api/models/format.py
+-rw-r--r--  2.0 unx     7319 b- defN 23-May-01 11:28 cloudsmith_api/models/format_support.py
+-rw-r--r--  2.0 unx     8615 b- defN 23-May-01 11:28 cloudsmith_api/models/geo_ip_location.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-May-01 11:28 cloudsmith_api/models/go_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-May-01 11:28 cloudsmith_api/models/go_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/helm_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/helm_package_upload_request.py
+-rw-r--r--  2.0 unx     7028 b- defN 23-May-01 11:28 cloudsmith_api/models/history.py
+-rw-r--r--  2.0 unx     5168 b- defN 23-May-01 11:28 cloudsmith_api/models/history_fieldset.py
+-rw-r--r--  2.0 unx     5246 b- defN 23-May-01 11:28 cloudsmith_api/models/history_fieldset_raw.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-May-01 11:28 cloudsmith_api/models/luarocks_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-May-01 11:28 cloudsmith_api/models/luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx    61667 b- defN 23-May-01 11:28 cloudsmith_api/models/maven_package_upload.py
+-rw-r--r--  2.0 unx    14513 b- defN 23-May-01 11:28 cloudsmith_api/models/maven_package_upload_request.py
+-rw-r--r--  2.0 unx     5806 b- defN 23-May-01 11:28 cloudsmith_api/models/namespace.py
+-rw-r--r--  2.0 unx    18223 b- defN 23-May-01 11:28 cloudsmith_api/models/namespace_audit_log.py
+-rw-r--r--  2.0 unx    10461 b- defN 23-May-01 11:28 cloudsmith_api/models/nested_license_policy.py
+-rw-r--r--  2.0 unx    11097 b- defN 23-May-01 11:28 cloudsmith_api/models/nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     9219 b- defN 23-May-01 11:28 cloudsmith_api/models/nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-01 11:28 cloudsmith_api/models/npm_package_upload.py
+-rw-r--r--  2.0 unx     7663 b- defN 23-May-01 11:28 cloudsmith_api/models/npm_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-01 11:28 cloudsmith_api/models/nuget_package_upload.py
+-rw-r--r--  2.0 unx     7272 b- defN 23-May-01 11:28 cloudsmith_api/models/nuget_package_upload_request.py
+-rw-r--r--  2.0 unx     7918 b- defN 23-May-01 11:28 cloudsmith_api/models/organization.py
+-rw-r--r--  2.0 unx     8391 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_group_sync.py
+-rw-r--r--  2.0 unx     8223 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_group_sync_request.py
+-rw-r--r--  2.0 unx    10169 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite.py
+-rw-r--r--  2.0 unx    10519 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_extend.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_request.py
+-rw-r--r--  2.0 unx     3821 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_update.py
+-rw-r--r--  2.0 unx     3929 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx    12300 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_membership.py
+-rw-r--r--  2.0 unx    11008 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_license_policy.py
+-rw-r--r--  2.0 unx     8427 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     8280 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx    11620 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx     8967 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx     8962 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx     8110 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team.py
+-rw-r--r--  2.0 unx     3669 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_members.py
+-rw-r--r--  2.0 unx     4783 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_membership.py
+-rw-r--r--  2.0 unx     7065 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_request.py
+-rw-r--r--  2.0 unx     7040 b- defN 23-May-01 11:28 cloudsmith_api/models/organization_team_request_patch.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-May-01 11:28 cloudsmith_api/models/p2_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-May-01 11:28 cloudsmith_api/models/p2_package_upload_request.py
+-rw-r--r--  2.0 unx    55965 b- defN 23-May-01 11:28 cloudsmith_api/models/package.py
+-rw-r--r--  2.0 unx    57197 b- defN 23-May-01 11:28 cloudsmith_api/models/package_copy.py
+-rw-r--r--  2.0 unx     4776 b- defN 23-May-01 11:28 cloudsmith_api/models/package_copy_request.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-May-01 11:28 cloudsmith_api/models/package_dependencies.py
+-rw-r--r--  2.0 unx     7227 b- defN 23-May-01 11:28 cloudsmith_api/models/package_dependency.py
+-rw-r--r--  2.0 unx    12968 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file.py
+-rw-r--r--  2.0 unx     6108 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file_parts_upload.py
+-rw-r--r--  2.0 unx     7841 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file_upload.py
+-rw-r--r--  2.0 unx     7815 b- defN 23-May-01 11:28 cloudsmith_api/models/package_file_upload_request.py
+-rw-r--r--  2.0 unx     6035 b- defN 23-May-01 11:28 cloudsmith_api/models/package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     5198 b- defN 23-May-01 11:28 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    57195 b- defN 23-May-01 11:28 cloudsmith_api/models/package_move.py
+-rw-r--r--  2.0 unx     3820 b- defN 23-May-01 11:28 cloudsmith_api/models/package_move_request.py
+-rw-r--r--  2.0 unx    58775 b- defN 23-May-01 11:28 cloudsmith_api/models/package_quarantine.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-May-01 11:28 cloudsmith_api/models/package_quarantine_request.py
+-rw-r--r--  2.0 unx    57651 b- defN 23-May-01 11:28 cloudsmith_api/models/package_resync.py
+-rw-r--r--  2.0 unx    15877 b- defN 23-May-01 11:28 cloudsmith_api/models/package_status.py
+-rw-r--r--  2.0 unx    57199 b- defN 23-May-01 11:28 cloudsmith_api/models/package_tag.py
+-rw-r--r--  2.0 unx     5352 b- defN 23-May-01 11:28 cloudsmith_api/models/package_tag_request.py
+-rw-r--r--  2.0 unx     3547 b- defN 23-May-01 11:28 cloudsmith_api/models/package_usage_metrics.py
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-01 11:28 cloudsmith_api/models/package_version_badge.py
+-rw-r--r--  2.0 unx     5707 b- defN 23-May-01 11:28 cloudsmith_api/models/package_vulnerability.py
+-rw-r--r--  2.0 unx     7491 b- defN 23-May-01 11:28 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     5318 b- defN 23-May-01 11:28 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-01 11:28 cloudsmith_api/models/python_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-May-01 11:28 cloudsmith_api/models/python_package_upload_request.py
+-rw-r--r--  2.0 unx     3358 b- defN 23-May-01 11:28 cloudsmith_api/models/quota.py
+-rw-r--r--  2.0 unx     3463 b- defN 23-May-01 11:28 cloudsmith_api/models/quota_history.py
+-rw-r--r--  2.0 unx     7675 b- defN 23-May-01 11:28 cloudsmith_api/models/rate_check.py
+-rw-r--r--  2.0 unx    58899 b- defN 23-May-01 11:28 cloudsmith_api/models/raw_package_upload.py
+-rw-r--r--  2.0 unx    11674 b- defN 23-May-01 11:28 cloudsmith_api/models/raw_package_upload_request.py
+-rw-r--r--  2.0 unx    66229 b- defN 23-May-01 11:28 cloudsmith_api/models/repository.py
+-rw-r--r--  2.0 unx    14861 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_audit_log.py
+-rw-r--r--  2.0 unx    67555 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_create.py
+-rw-r--r--  2.0 unx    52996 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_create_request.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     4488 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx     4424 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     4312 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     3906 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     7359 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx     8734 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_gpg_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_gpg_key_create.py
+-rw-r--r--  2.0 unx     7702 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_dict.py
+-rw-r--r--  2.0 unx     3818 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_input.py
+-rw-r--r--  2.0 unx     3881 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     3790 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx    51807 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_request_patch.py
+-rw-r--r--  2.0 unx     7753 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_rsa_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_rsa_key_create.py
+-rw-r--r--  2.0 unx    40222 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_action.py
+-rw-r--r--  2.0 unx    41219 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_refresh.py
+-rw-r--r--  2.0 unx    21868 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_refresh_request.py
+-rw-r--r--  2.0 unx    22374 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_request.py
+-rw-r--r--  2.0 unx    22569 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_request_patch.py
+-rw-r--r--  2.0 unx     3505 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_sync.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_token_sync_request.py
+-rw-r--r--  2.0 unx    30400 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_webhook.py
+-rw-r--r--  2.0 unx    18912 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_webhook_request.py
+-rw-r--r--  2.0 unx    18774 b- defN 23-May-01 11:28 cloudsmith_api/models/repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-May-01 11:28 cloudsmith_api/models/resources_rate_check.py
+-rw-r--r--  2.0 unx     2790 b- defN 23-May-01 11:28 cloudsmith_api/models/respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     2825 b- defN 23-May-01 11:28 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-01 11:28 cloudsmith_api/models/rpm_package_upload.py
+-rw-r--r--  2.0 unx     7374 b- defN 23-May-01 11:28 cloudsmith_api/models/rpm_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-01 11:28 cloudsmith_api/models/ruby_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-01 11:28 cloudsmith_api/models/ruby_package_upload_request.py
+-rw-r--r--  2.0 unx     8234 b- defN 23-May-01 11:28 cloudsmith_api/models/service.py
+-rw-r--r--  2.0 unx     6726 b- defN 23-May-01 11:28 cloudsmith_api/models/service_request.py
+-rw-r--r--  2.0 unx     6701 b- defN 23-May-01 11:28 cloudsmith_api/models/service_request_patch.py
+-rw-r--r--  2.0 unx     4951 b- defN 23-May-01 11:28 cloudsmith_api/models/service_teams.py
+-rw-r--r--  2.0 unx     4584 b- defN 23-May-01 11:28 cloudsmith_api/models/status_basic.py
+-rw-r--r--  2.0 unx     8478 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_allocated_limit.py
+-rw-r--r--  2.0 unx     6140 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx     4670 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_region.py
+-rw-r--r--  2.0 unx     6847 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_usage.py
+-rw-r--r--  2.0 unx     5048 b- defN 23-May-01 11:28 cloudsmith_api/models/storage_usage_raw.py
+-rw-r--r--  2.0 unx     2665 b- defN 23-May-01 11:28 cloudsmith_api/models/tags.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-May-01 11:28 cloudsmith_api/models/terraform_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-May-01 11:28 cloudsmith_api/models/terraform_package_upload_request.py
+-rw-r--r--  2.0 unx     5738 b- defN 23-May-01 11:28 cloudsmith_api/models/usage.py
+-rw-r--r--  2.0 unx     4147 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_fieldset.py
+-rw-r--r--  2.0 unx     4277 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_limits.py
+-rw-r--r--  2.0 unx     4334 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_limits_raw.py
+-rw-r--r--  2.0 unx     4382 b- defN 23-May-01 11:28 cloudsmith_api/models/usage_raw.py
+-rw-r--r--  2.0 unx     3590 b- defN 23-May-01 11:28 cloudsmith_api/models/user_auth_token.py
+-rw-r--r--  2.0 unx     4612 b- defN 23-May-01 11:28 cloudsmith_api/models/user_auth_token_request.py
+-rw-r--r--  2.0 unx     8019 b- defN 23-May-01 11:28 cloudsmith_api/models/user_brief.py
+-rw-r--r--  2.0 unx    11110 b- defN 23-May-01 11:28 cloudsmith_api/models/user_profile.py
+-rw-r--r--  2.0 unx    60899 b- defN 23-May-01 11:28 cloudsmith_api/models/vagrant_package_upload.py
+-rw-r--r--  2.0 unx     9492 b- defN 23-May-01 11:28 cloudsmith_api/models/vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx    13112 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability.py
+-rw-r--r--  2.0 unx     5400 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan.py
+-rw-r--r--  2.0 unx    10040 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     9417 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx     8443 b- defN 23-May-01 11:28 cloudsmith_api/models/vulnerability_scan_version.py
+-rw-r--r--  2.0 unx     4751 b- defN 23-May-01 11:28 cloudsmith_api/models/webhook_template.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-01 11:28 test/__init__.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-01 11:28 test/test_allocated_limit.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_alpine_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_alpine_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-01 11:28 test/test_architecture.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-01 11:28 test/test_audit_log_api.py
+-rw-r--r--  2.0 unx      883 b- defN 23-May-01 11:28 test/test_badges_api.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_cargo_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_cargo_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_common_downloads_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_common_metrics.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_composer_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_composer_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_conan_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_conan_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_conda_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_conda_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_cran_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_cran_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_dart_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_dart_package_upload_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_deb_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_deb_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-01 11:28 test/test_distribution.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-01 11:28 test/test_distribution_full.py
+-rw-r--r--  2.0 unx      940 b- defN 23-May-01 11:28 test/test_distribution_version.py
+-rw-r--r--  2.0 unx     1019 b- defN 23-May-01 11:28 test/test_distros_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_docker_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_docker_package_upload_request.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-May-01 11:28 test/test_entitlements_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_error_detail.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-01 11:28 test/test_eula.py
+-rw-r--r--  2.0 unx     1503 b- defN 23-May-01 11:28 test/test_files_api.py
+-rw-r--r--  2.0 unx      834 b- defN 23-May-01 11:28 test/test_format.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_format_support.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-May-01 11:28 test/test_formats_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-01 11:28 test/test_geo_ip_location.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-01 11:28 test/test_go_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_go_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_helm_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_helm_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-01 11:28 test/test_history.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-01 11:28 test/test_history_fieldset.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_history_fieldset_raw.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_luarocks_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_maven_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_maven_package_upload_request.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-May-01 11:28 test/test_metrics_api.py
+-rw-r--r--  2.0 unx      858 b- defN 23-May-01 11:28 test/test_namespace.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_namespace_audit_log.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-May-01 11:28 test/test_namespaces_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_nested_license_policy.py
+-rw-r--r--  2.0 unx      990 b- defN 23-May-01 11:28 test/test_nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1032 b- defN 23-May-01 11:28 test/test_nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_npm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_npm_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_nuget_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-01 11:28 test/test_nuget_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-01 11:28 test/test_organization.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_organization_group_sync.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_organization_group_sync_request.py
+-rw-r--r--  2.0 unx      932 b- defN 23-May-01 11:28 test/test_organization_invite.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_organization_invite_extend.py
+-rw-r--r--  2.0 unx      990 b- defN 23-May-01 11:28 test/test_organization_invite_request.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_organization_invite_update.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-May-01 11:28 test/test_organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx      964 b- defN 23-May-01 11:28 test/test_organization_membership.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-May-01 11:28 test/test_organization_package_license_policy.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-May-01 11:28 test/test_organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-May-01 11:28 test/test_organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-May-01 11:28 test/test_organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1154 b- defN 23-May-01 11:28 test/test_organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-May-01 11:28 test/test_organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-01 11:28 test/test_organization_team.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_organization_team_members.py
+-rw-r--r--  2.0 unx      998 b- defN 23-May-01 11:28 test/test_organization_team_membership.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_organization_team_request.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_organization_team_request_patch.py
+-rw-r--r--  2.0 unx     8724 b- defN 23-May-01 11:28 test/test_orgs_api.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-01 11:28 test/test_p2_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_p2_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-01 11:28 test/test_package.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_package_copy.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_package_copy_request.py
+-rw-r--r--  2.0 unx      940 b- defN 23-May-01 11:28 test/test_package_dependencies.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_package_dependency.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_package_file.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_package_file_parts_upload.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_package_file_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_package_file_upload_request.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-01 11:28 test/test_package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-01 11:28 test/test_package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_package_move.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_package_move_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_package_quarantine.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_package_quarantine_request.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_package_resync.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_package_status.py
+-rw-r--r--  2.0 unx      868 b- defN 23-May-01 11:28 test/test_package_tag.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_package_tag_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_package_usage_metrics.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_package_version_badge.py
+-rw-r--r--  2.0 unx      948 b- defN 23-May-01 11:28 test/test_package_vulnerability.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-May-01 11:28 test/test_package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     1182 b- defN 23-May-01 11:28 test/test_package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    11023 b- defN 23-May-01 11:28 test/test_packages_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_python_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_python_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-01 11:28 test/test_quota.py
+-rw-r--r--  2.0 unx     1364 b- defN 23-May-01 11:28 test/test_quota_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-01 11:28 test/test_quota_history.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-01 11:28 test/test_rate_check.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-01 11:28 test/test_rates_api.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_raw_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_raw_package_upload_request.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-01 11:28 test/test_repos_api.py
+-rw-r--r--  2.0 unx      866 b- defN 23-May-01 11:28 test/test_repository.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_repository_audit_log.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-01 11:28 test/test_repository_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_repository_create_request.py
+-rw-r--r--  2.0 unx      944 b- defN 23-May-01 11:28 test/test_repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-01 11:28 test/test_repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-01 11:28 test/test_repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-01 11:28 test/test_repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-May-01 11:28 test/test_repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-01 11:28 test/test_repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-01 11:28 test/test_repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-May-01 11:28 test/test_repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_repository_gpg_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_repository_gpg_key_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-01 11:28 test/test_repository_privilege_dict.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_repository_privilege_input.py
+-rw-r--r--  2.0 unx     1040 b- defN 23-May-01 11:28 test/test_repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-May-01 11:28 test/test_repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_repository_request_patch.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_repository_rsa_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-01 11:28 test/test_repository_rsa_key_create.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-01 11:28 test/test_repository_token.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_repository_token_action.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_repository_token_refresh.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_repository_token_refresh_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_repository_token_request.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_repository_token_request_patch.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_repository_token_sync.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-01 11:28 test/test_repository_token_sync_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_repository_webhook.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_repository_webhook_request.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-01 11:28 test/test_resources_rate_check.py
+-rw-r--r--  2.0 unx     1026 b- defN 23-May-01 11:28 test/test_respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     1084 b- defN 23-May-01 11:28 test/test_respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-01 11:28 test/test_rpm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-01 11:28 test/test_rpm_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-01 11:28 test/test_ruby_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_ruby_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-01 11:28 test/test_service.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-01 11:28 test/test_service_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-01 11:28 test/test_service_request_patch.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-01 11:28 test/test_service_teams.py
+-rw-r--r--  2.0 unx      864 b- defN 23-May-01 11:28 test/test_status_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_status_basic.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-01 11:28 test/test_storage_allocated_limit.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-01 11:28 test/test_storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_storage_region.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-01 11:28 test/test_storage_regions_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-01 11:28 test/test_storage_usage.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-01 11:28 test/test_storage_usage_raw.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-01 11:28 test/test_tags.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-01 11:28 test/test_terraform_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_terraform_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-01 11:28 test/test_usage.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-01 11:28 test/test_usage_fieldset.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_usage_limits.py
+-rw-r--r--  2.0 unx      902 b- defN 23-May-01 11:28 test/test_usage_limits_raw.py
+-rw-r--r--  2.0 unx      852 b- defN 23-May-01 11:28 test/test_usage_raw.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-01 11:28 test/test_user_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-01 11:28 test/test_user_auth_token.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-01 11:28 test/test_user_auth_token_request.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-01 11:28 test/test_user_brief.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-01 11:28 test/test_user_profile.py
+-rw-r--r--  2.0 unx      865 b- defN 23-May-01 11:28 test/test_users_api.py
+-rw-r--r--  2.0 unx      950 b- defN 23-May-01 11:28 test/test_vagrant_package_upload.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-01 11:28 test/test_vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx     1491 b- defN 23-May-01 11:28 test/test_vulnerabilities_api.py
+-rw-r--r--  2.0 unx      890 b- defN 23-May-01 11:28 test/test_vulnerability.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-01 11:28 test/test_vulnerability_scan.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-01 11:28 test/test_vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-01 11:28 test/test_vulnerability_scan_version.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-01 11:28 test/test_webhook_template.py
+-rw-r--r--  2.0 unx     1557 b- defN 23-May-01 11:28 test/test_webhooks_api.py
+-rw-r--r--  2.0 unx      457 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    39488 b- defN 23-May-01 11:29 cloudsmith_api-2.0.2.dist-info/RECORD
+407 files, 4221278 bytes uncompressed, 647576 bytes compressed:  84.7%
```

## zipnote {}

```diff
@@ -72,14 +72,17 @@
 
 Filename: cloudsmith_api/models/__init__.py
 Comment: 
 
 Filename: cloudsmith_api/models/allocated_limit.py
 Comment: 
 
+Filename: cloudsmith_api/models/allocated_limit_raw.py
+Comment: 
+
 Filename: cloudsmith_api/models/alpine_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/alpine_package_upload_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/architecture.py
@@ -195,18 +198,15 @@
 
 Filename: cloudsmith_api/models/history.py
 Comment: 
 
 Filename: cloudsmith_api/models/history_fieldset.py
 Comment: 
 
-Filename: cloudsmith_api/models/inline_response200.py
-Comment: 
-
-Filename: cloudsmith_api/models/inline_response200_country_code.py
+Filename: cloudsmith_api/models/history_fieldset_raw.py
 Comment: 
 
 Filename: cloudsmith_api/models/luarocks_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/luarocks_package_upload_request.py
 Comment: 
@@ -219,14 +219,23 @@
 
 Filename: cloudsmith_api/models/namespace.py
 Comment: 
 
 Filename: cloudsmith_api/models/namespace_audit_log.py
 Comment: 
 
+Filename: cloudsmith_api/models/nested_license_policy.py
+Comment: 
+
+Filename: cloudsmith_api/models/nested_vulnerability_policy.py
+Comment: 
+
+Filename: cloudsmith_api/models/nested_vulnerability_scan_results.py
+Comment: 
+
 Filename: cloudsmith_api/models/npm_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/npm_package_upload_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/nuget_package_upload.py
@@ -258,14 +267,32 @@
 
 Filename: cloudsmith_api/models/organization_invite_update_request_patch.py
 Comment: 
 
 Filename: cloudsmith_api/models/organization_membership.py
 Comment: 
 
+Filename: cloudsmith_api/models/organization_package_license_policy.py
+Comment: 
+
+Filename: cloudsmith_api/models/organization_package_license_policy_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/organization_package_license_policy_request_patch.py
+Comment: 
+
+Filename: cloudsmith_api/models/organization_package_vulnerability_policy.py
+Comment: 
+
+Filename: cloudsmith_api/models/organization_package_vulnerability_policy_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
+Comment: 
+
 Filename: cloudsmith_api/models/organization_team.py
 Comment: 
 
 Filename: cloudsmith_api/models/organization_team_members.py
 Comment: 
 
 Filename: cloudsmith_api/models/organization_team_membership.py
@@ -306,14 +333,20 @@
 
 Filename: cloudsmith_api/models/package_file_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_file_upload_request.py
 Comment: 
 
+Filename: cloudsmith_api/models/package_license_policy_violation_log.py
+Comment: 
+
+Filename: cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
+Comment: 
+
 Filename: cloudsmith_api/models/package_move.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_move_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_quarantine.py
@@ -339,14 +372,20 @@
 
 Filename: cloudsmith_api/models/package_version_badge.py
 Comment: 
 
 Filename: cloudsmith_api/models/package_vulnerability.py
 Comment: 
 
+Filename: cloudsmith_api/models/package_vulnerability_policy_violation_log.py
+Comment: 
+
+Filename: cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
+Comment: 
+
 Filename: cloudsmith_api/models/python_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/python_package_upload_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/quota.py
@@ -372,15 +411,36 @@
 
 Filename: cloudsmith_api/models/repository_create.py
 Comment: 
 
 Filename: cloudsmith_api/models/repository_create_request.py
 Comment: 
 
-Filename: cloudsmith_api/models/repository_geo_ip_list.py
+Filename: cloudsmith_api/models/repository_geo_ip_cidr.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_country_code.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_rules.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_rules_request.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_test_address.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_test_address_response.py
+Comment: 
+
+Filename: cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
 Comment: 
 
 Filename: cloudsmith_api/models/repository_gpg_key.py
 Comment: 
 
 Filename: cloudsmith_api/models/repository_gpg_key_create.py
 Comment: 
@@ -471,17 +531,29 @@
 
 Filename: cloudsmith_api/models/service_teams.py
 Comment: 
 
 Filename: cloudsmith_api/models/status_basic.py
 Comment: 
 
+Filename: cloudsmith_api/models/storage_allocated_limit.py
+Comment: 
+
+Filename: cloudsmith_api/models/storage_allocated_limit_raw.py
+Comment: 
+
 Filename: cloudsmith_api/models/storage_region.py
 Comment: 
 
+Filename: cloudsmith_api/models/storage_usage.py
+Comment: 
+
+Filename: cloudsmith_api/models/storage_usage_raw.py
+Comment: 
+
 Filename: cloudsmith_api/models/tags.py
 Comment: 
 
 Filename: cloudsmith_api/models/terraform_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/terraform_package_upload_request.py
@@ -492,14 +564,20 @@
 
 Filename: cloudsmith_api/models/usage_fieldset.py
 Comment: 
 
 Filename: cloudsmith_api/models/usage_limits.py
 Comment: 
 
+Filename: cloudsmith_api/models/usage_limits_raw.py
+Comment: 
+
+Filename: cloudsmith_api/models/usage_raw.py
+Comment: 
+
 Filename: cloudsmith_api/models/user_auth_token.py
 Comment: 
 
 Filename: cloudsmith_api/models/user_auth_token_request.py
 Comment: 
 
 Filename: cloudsmith_api/models/user_brief.py
@@ -534,14 +612,17 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_allocated_limit.py
 Comment: 
 
+Filename: test/test_allocated_limit_raw.py
+Comment: 
+
 Filename: test/test_alpine_package_upload.py
 Comment: 
 
 Filename: test/test_alpine_package_upload_request.py
 Comment: 
 
 Filename: test/test_architecture.py
@@ -675,18 +756,15 @@
 
 Filename: test/test_history.py
 Comment: 
 
 Filename: test/test_history_fieldset.py
 Comment: 
 
-Filename: test/test_inline_response200.py
-Comment: 
-
-Filename: test/test_inline_response200_country_code.py
+Filename: test/test_history_fieldset_raw.py
 Comment: 
 
 Filename: test/test_luarocks_package_upload.py
 Comment: 
 
 Filename: test/test_luarocks_package_upload_request.py
 Comment: 
@@ -705,14 +783,23 @@
 
 Filename: test/test_namespace_audit_log.py
 Comment: 
 
 Filename: test/test_namespaces_api.py
 Comment: 
 
+Filename: test/test_nested_license_policy.py
+Comment: 
+
+Filename: test/test_nested_vulnerability_policy.py
+Comment: 
+
+Filename: test/test_nested_vulnerability_scan_results.py
+Comment: 
+
 Filename: test/test_npm_package_upload.py
 Comment: 
 
 Filename: test/test_npm_package_upload_request.py
 Comment: 
 
 Filename: test/test_nuget_package_upload.py
@@ -744,14 +831,32 @@
 
 Filename: test/test_organization_invite_update_request_patch.py
 Comment: 
 
 Filename: test/test_organization_membership.py
 Comment: 
 
+Filename: test/test_organization_package_license_policy.py
+Comment: 
+
+Filename: test/test_organization_package_license_policy_request.py
+Comment: 
+
+Filename: test/test_organization_package_license_policy_request_patch.py
+Comment: 
+
+Filename: test/test_organization_package_vulnerability_policy.py
+Comment: 
+
+Filename: test/test_organization_package_vulnerability_policy_request.py
+Comment: 
+
+Filename: test/test_organization_package_vulnerability_policy_request_patch.py
+Comment: 
+
 Filename: test/test_organization_team.py
 Comment: 
 
 Filename: test/test_organization_team_members.py
 Comment: 
 
 Filename: test/test_organization_team_membership.py
@@ -795,14 +900,20 @@
 
 Filename: test/test_package_file_upload.py
 Comment: 
 
 Filename: test/test_package_file_upload_request.py
 Comment: 
 
+Filename: test/test_package_license_policy_violation_log.py
+Comment: 
+
+Filename: test/test_package_license_policy_violation_log_cursor_page.py
+Comment: 
+
 Filename: test/test_package_move.py
 Comment: 
 
 Filename: test/test_package_move_request.py
 Comment: 
 
 Filename: test/test_package_quarantine.py
@@ -828,14 +939,20 @@
 
 Filename: test/test_package_version_badge.py
 Comment: 
 
 Filename: test/test_package_vulnerability.py
 Comment: 
 
+Filename: test/test_package_vulnerability_policy_violation_log.py
+Comment: 
+
+Filename: test/test_package_vulnerability_policy_violation_log_cursor_page.py
+Comment: 
+
 Filename: test/test_packages_api.py
 Comment: 
 
 Filename: test/test_python_package_upload.py
 Comment: 
 
 Filename: test/test_python_package_upload_request.py
@@ -873,15 +990,36 @@
 
 Filename: test/test_repository_create.py
 Comment: 
 
 Filename: test/test_repository_create_request.py
 Comment: 
 
-Filename: test/test_repository_geo_ip_list.py
+Filename: test/test_repository_geo_ip_cidr.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_country_code.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_rules.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_rules_request.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_rules_request_patch.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_test_address.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_test_address_response.py
+Comment: 
+
+Filename: test/test_repository_geo_ip_test_address_response_dict.py
 Comment: 
 
 Filename: test/test_repository_gpg_key.py
 Comment: 
 
 Filename: test/test_repository_gpg_key_create.py
 Comment: 
@@ -975,20 +1113,32 @@
 
 Filename: test/test_status_api.py
 Comment: 
 
 Filename: test/test_status_basic.py
 Comment: 
 
+Filename: test/test_storage_allocated_limit.py
+Comment: 
+
+Filename: test/test_storage_allocated_limit_raw.py
+Comment: 
+
 Filename: test/test_storage_region.py
 Comment: 
 
 Filename: test/test_storage_regions_api.py
 Comment: 
 
+Filename: test/test_storage_usage.py
+Comment: 
+
+Filename: test/test_storage_usage_raw.py
+Comment: 
+
 Filename: test/test_tags.py
 Comment: 
 
 Filename: test/test_terraform_package_upload.py
 Comment: 
 
 Filename: test/test_terraform_package_upload_request.py
@@ -999,14 +1149,20 @@
 
 Filename: test/test_usage_fieldset.py
 Comment: 
 
 Filename: test/test_usage_limits.py
 Comment: 
 
+Filename: test/test_usage_limits_raw.py
+Comment: 
+
+Filename: test/test_usage_raw.py
+Comment: 
+
 Filename: test/test_user_api.py
 Comment: 
 
 Filename: test/test_user_auth_token.py
 Comment: 
 
 Filename: test/test_user_auth_token_request.py
@@ -1047,20 +1203,20 @@
 
 Filename: test/test_webhook_template.py
 Comment: 
 
 Filename: test/test_webhooks_api.py
 Comment: 
 
-Filename: cloudsmith_api-2.0.1.dist-info/METADATA
+Filename: cloudsmith_api-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cloudsmith_api-2.0.1.dist-info/WHEEL
+Filename: cloudsmith_api-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cloudsmith_api-2.0.1.dist-info/top_level.txt
+Filename: cloudsmith_api-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudsmith_api-2.0.1.dist-info/RECORD
+Filename: cloudsmith_api-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudsmith_api/__init__.py

```diff
@@ -37,14 +37,15 @@
 from cloudsmith_api.api.webhooks_api import WebhooksApi
 
 # import ApiClient
 from cloudsmith_api.api_client import ApiClient
 from cloudsmith_api.configuration import Configuration
 # import models into sdk package
 from cloudsmith_api.models.allocated_limit import AllocatedLimit
+from cloudsmith_api.models.allocated_limit_raw import AllocatedLimitRaw
 from cloudsmith_api.models.alpine_package_upload import AlpinePackageUpload
 from cloudsmith_api.models.alpine_package_upload_request import AlpinePackageUploadRequest
 from cloudsmith_api.models.architecture import Architecture
 from cloudsmith_api.models.cargo_package_upload import CargoPackageUpload
 from cloudsmith_api.models.cargo_package_upload_request import CargoPackageUploadRequest
 from cloudsmith_api.models.cocoapods_package_upload import CocoapodsPackageUpload
 from cloudsmith_api.models.cocoapods_package_upload_request import CocoapodsPackageUploadRequest
@@ -78,35 +79,43 @@
 from cloudsmith_api.models.geo_ip_location import GeoIpLocation
 from cloudsmith_api.models.go_package_upload import GoPackageUpload
 from cloudsmith_api.models.go_package_upload_request import GoPackageUploadRequest
 from cloudsmith_api.models.helm_package_upload import HelmPackageUpload
 from cloudsmith_api.models.helm_package_upload_request import HelmPackageUploadRequest
 from cloudsmith_api.models.history import History
 from cloudsmith_api.models.history_fieldset import HistoryFieldset
-from cloudsmith_api.models.inline_response200 import InlineResponse200
-from cloudsmith_api.models.inline_response200_country_code import InlineResponse200CountryCode
+from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw
 from cloudsmith_api.models.luarocks_package_upload import LuarocksPackageUpload
 from cloudsmith_api.models.luarocks_package_upload_request import LuarocksPackageUploadRequest
 from cloudsmith_api.models.maven_package_upload import MavenPackageUpload
 from cloudsmith_api.models.maven_package_upload_request import MavenPackageUploadRequest
 from cloudsmith_api.models.namespace import Namespace
 from cloudsmith_api.models.namespace_audit_log import NamespaceAuditLog
+from cloudsmith_api.models.nested_license_policy import NestedLicensePolicy
+from cloudsmith_api.models.nested_vulnerability_policy import NestedVulnerabilityPolicy
+from cloudsmith_api.models.nested_vulnerability_scan_results import NestedVulnerabilityScanResults
 from cloudsmith_api.models.npm_package_upload import NpmPackageUpload
 from cloudsmith_api.models.npm_package_upload_request import NpmPackageUploadRequest
 from cloudsmith_api.models.nuget_package_upload import NugetPackageUpload
 from cloudsmith_api.models.nuget_package_upload_request import NugetPackageUploadRequest
 from cloudsmith_api.models.organization import Organization
 from cloudsmith_api.models.organization_group_sync import OrganizationGroupSync
 from cloudsmith_api.models.organization_group_sync_request import OrganizationGroupSyncRequest
 from cloudsmith_api.models.organization_invite import OrganizationInvite
 from cloudsmith_api.models.organization_invite_extend import OrganizationInviteExtend
 from cloudsmith_api.models.organization_invite_request import OrganizationInviteRequest
 from cloudsmith_api.models.organization_invite_update import OrganizationInviteUpdate
 from cloudsmith_api.models.organization_invite_update_request_patch import OrganizationInviteUpdateRequestPatch
 from cloudsmith_api.models.organization_membership import OrganizationMembership
+from cloudsmith_api.models.organization_package_license_policy import OrganizationPackageLicensePolicy
+from cloudsmith_api.models.organization_package_license_policy_request import OrganizationPackageLicensePolicyRequest
+from cloudsmith_api.models.organization_package_license_policy_request_patch import OrganizationPackageLicensePolicyRequestPatch
+from cloudsmith_api.models.organization_package_vulnerability_policy import OrganizationPackageVulnerabilityPolicy
+from cloudsmith_api.models.organization_package_vulnerability_policy_request import OrganizationPackageVulnerabilityPolicyRequest
+from cloudsmith_api.models.organization_package_vulnerability_policy_request_patch import OrganizationPackageVulnerabilityPolicyRequestPatch
 from cloudsmith_api.models.organization_team import OrganizationTeam
 from cloudsmith_api.models.organization_team_members import OrganizationTeamMembers
 from cloudsmith_api.models.organization_team_membership import OrganizationTeamMembership
 from cloudsmith_api.models.organization_team_request import OrganizationTeamRequest
 from cloudsmith_api.models.organization_team_request_patch import OrganizationTeamRequestPatch
 from cloudsmith_api.models.p2_package_upload import P2PackageUpload
 from cloudsmith_api.models.p2_package_upload_request import P2PackageUploadRequest
@@ -115,37 +124,48 @@
 from cloudsmith_api.models.package_copy_request import PackageCopyRequest
 from cloudsmith_api.models.package_dependencies import PackageDependencies
 from cloudsmith_api.models.package_dependency import PackageDependency
 from cloudsmith_api.models.package_file import PackageFile
 from cloudsmith_api.models.package_file_parts_upload import PackageFilePartsUpload
 from cloudsmith_api.models.package_file_upload import PackageFileUpload
 from cloudsmith_api.models.package_file_upload_request import PackageFileUploadRequest
+from cloudsmith_api.models.package_license_policy_violation_log import PackageLicensePolicyViolationLog
+from cloudsmith_api.models.package_license_policy_violation_log_cursor_page import PackageLicensePolicyViolationLogCursorPage
 from cloudsmith_api.models.package_move import PackageMove
 from cloudsmith_api.models.package_move_request import PackageMoveRequest
 from cloudsmith_api.models.package_quarantine import PackageQuarantine
 from cloudsmith_api.models.package_quarantine_request import PackageQuarantineRequest
 from cloudsmith_api.models.package_resync import PackageResync
 from cloudsmith_api.models.package_status import PackageStatus
 from cloudsmith_api.models.package_tag import PackageTag
 from cloudsmith_api.models.package_tag_request import PackageTagRequest
 from cloudsmith_api.models.package_usage_metrics import PackageUsageMetrics
 from cloudsmith_api.models.package_version_badge import PackageVersionBadge
 from cloudsmith_api.models.package_vulnerability import PackageVulnerability
+from cloudsmith_api.models.package_vulnerability_policy_violation_log import PackageVulnerabilityPolicyViolationLog
+from cloudsmith_api.models.package_vulnerability_policy_violation_log_cursor_page import PackageVulnerabilityPolicyViolationLogCursorPage
 from cloudsmith_api.models.python_package_upload import PythonPackageUpload
 from cloudsmith_api.models.python_package_upload_request import PythonPackageUploadRequest
 from cloudsmith_api.models.quota import Quota
 from cloudsmith_api.models.quota_history import QuotaHistory
 from cloudsmith_api.models.rate_check import RateCheck
 from cloudsmith_api.models.raw_package_upload import RawPackageUpload
 from cloudsmith_api.models.raw_package_upload_request import RawPackageUploadRequest
 from cloudsmith_api.models.repository import Repository
 from cloudsmith_api.models.repository_audit_log import RepositoryAuditLog
 from cloudsmith_api.models.repository_create import RepositoryCreate
 from cloudsmith_api.models.repository_create_request import RepositoryCreateRequest
-from cloudsmith_api.models.repository_geo_ip_list import RepositoryGeoIPList
+from cloudsmith_api.models.repository_geo_ip_cidr import RepositoryGeoIpCidr
+from cloudsmith_api.models.repository_geo_ip_country_code import RepositoryGeoIpCountryCode
+from cloudsmith_api.models.repository_geo_ip_rules import RepositoryGeoIpRules
+from cloudsmith_api.models.repository_geo_ip_rules_request import RepositoryGeoIpRulesRequest
+from cloudsmith_api.models.repository_geo_ip_rules_request_patch import RepositoryGeoIpRulesRequestPatch
+from cloudsmith_api.models.repository_geo_ip_test_address import RepositoryGeoIpTestAddress
+from cloudsmith_api.models.repository_geo_ip_test_address_response import RepositoryGeoIpTestAddressResponse
+from cloudsmith_api.models.repository_geo_ip_test_address_response_dict import RepositoryGeoIpTestAddressResponseDict
 from cloudsmith_api.models.repository_gpg_key import RepositoryGpgKey
 from cloudsmith_api.models.repository_gpg_key_create import RepositoryGpgKeyCreate
 from cloudsmith_api.models.repository_privilege_dict import RepositoryPrivilegeDict
 from cloudsmith_api.models.repository_privilege_input import RepositoryPrivilegeInput
 from cloudsmith_api.models.repository_privilege_input_request import RepositoryPrivilegeInputRequest
 from cloudsmith_api.models.repository_privilege_input_request_patch import RepositoryPrivilegeInputRequestPatch
 from cloudsmith_api.models.repository_request_patch import RepositoryRequestPatch
@@ -159,32 +179,38 @@
 from cloudsmith_api.models.repository_token_request_patch import RepositoryTokenRequestPatch
 from cloudsmith_api.models.repository_token_sync import RepositoryTokenSync
 from cloudsmith_api.models.repository_token_sync_request import RepositoryTokenSyncRequest
 from cloudsmith_api.models.repository_webhook import RepositoryWebhook
 from cloudsmith_api.models.repository_webhook_request import RepositoryWebhookRequest
 from cloudsmith_api.models.repository_webhook_request_patch import RepositoryWebhookRequestPatch
 from cloudsmith_api.models.resources_rate_check import ResourcesRateCheck
-from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIPEnableDisable
-from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIPEnableDisableRequest
+from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIpEnableDisable
+from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIpEnableDisableRequest
 from cloudsmith_api.models.rpm_package_upload import RpmPackageUpload
 from cloudsmith_api.models.rpm_package_upload_request import RpmPackageUploadRequest
 from cloudsmith_api.models.ruby_package_upload import RubyPackageUpload
 from cloudsmith_api.models.ruby_package_upload_request import RubyPackageUploadRequest
 from cloudsmith_api.models.service import Service
 from cloudsmith_api.models.service_request import ServiceRequest
 from cloudsmith_api.models.service_request_patch import ServiceRequestPatch
 from cloudsmith_api.models.service_teams import ServiceTeams
 from cloudsmith_api.models.status_basic import StatusBasic
+from cloudsmith_api.models.storage_allocated_limit import StorageAllocatedLimit
+from cloudsmith_api.models.storage_allocated_limit_raw import StorageAllocatedLimitRaw
 from cloudsmith_api.models.storage_region import StorageRegion
+from cloudsmith_api.models.storage_usage import StorageUsage
+from cloudsmith_api.models.storage_usage_raw import StorageUsageRaw
 from cloudsmith_api.models.tags import Tags
 from cloudsmith_api.models.terraform_package_upload import TerraformPackageUpload
 from cloudsmith_api.models.terraform_package_upload_request import TerraformPackageUploadRequest
 from cloudsmith_api.models.usage import Usage
 from cloudsmith_api.models.usage_fieldset import UsageFieldset
 from cloudsmith_api.models.usage_limits import UsageLimits
+from cloudsmith_api.models.usage_limits_raw import UsageLimitsRaw
+from cloudsmith_api.models.usage_raw import UsageRaw
 from cloudsmith_api.models.user_auth_token import UserAuthToken
 from cloudsmith_api.models.user_auth_token_request import UserAuthTokenRequest
 from cloudsmith_api.models.user_brief import UserBrief
 from cloudsmith_api.models.user_profile import UserProfile
 from cloudsmith_api.models.vagrant_package_upload import VagrantPackageUpload
 from cloudsmith_api.models.vagrant_package_upload_request import VagrantPackageUploadRequest
 from cloudsmith_api.models.vulnerability import Vulnerability
```

## cloudsmith_api/api_client.py

```diff
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.0.1/python'
+        self.user_agent = 'Swagger-Codegen/2.0.2/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

## cloudsmith_api/configuration.py

```diff
@@ -254,9 +254,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 2.0.1".\
+               "SDK Package Version: 2.0.2".\
                format(env=sys.platform, pyversion=sys.version)
```

## cloudsmith_api/api/orgs_api.py

```diff
@@ -671,14 +671,767 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def orgs_license_policy_create(self, org, **kwargs):  # noqa: E501
+        """Create a package license policy.  # noqa: E501
+
+        Create a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_create(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param OrganizationPackageLicensePolicyRequest data:
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_create_with_http_info(org, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_create_with_http_info(org, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_create_with_http_info(self, org, **kwargs):  # noqa: E501
+        """Create a package license policy.  # noqa: E501
+
+        Create a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_create_with_http_info(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param OrganizationPackageLicensePolicyRequest data:
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageLicensePolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_delete(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Delete a package license policy.  # noqa: E501
+
+        Delete a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_delete(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_delete_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_delete_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_delete_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Delete a package license policy.  # noqa: E501
+
+        Delete a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_delete_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_license_policy_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_list(self, org, **kwargs):  # noqa: E501
+        """Get a list of all package license policies.  # noqa: E501
+
+        Get a list of all package license policies.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_list(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[OrganizationPackageLicensePolicy]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_list_with_http_info(org, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_list_with_http_info(org, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_list_with_http_info(self, org, **kwargs):  # noqa: E501
+        """Get a list of all package license policies.  # noqa: E501
+
+        Get a list of all package license policies.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_list_with_http_info(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[OrganizationPackageLicensePolicy]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[OrganizationPackageLicensePolicy]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_partial_update(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a package license policy.  # noqa: E501
+
+        Partially update a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_partial_update(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageLicensePolicyRequestPatch data:
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_partial_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_partial_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_partial_update_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a package license policy.  # noqa: E501
+
+        Partially update a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_partial_update_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageLicensePolicyRequestPatch data:
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_license_policy_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageLicensePolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_read(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Get a package license policy.  # noqa: E501
+
+        Get a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_read(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_read_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_read_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_read_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Get a package license policy.  # noqa: E501
+
+        Get a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_read_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_license_policy_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageLicensePolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_update(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Update a package license policy.  # noqa: E501
+
+        Update a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_update(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageLicensePolicyRequest data:
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_update_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Update a package license policy.  # noqa: E501
+
+        Update a package license policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_update_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageLicensePolicyRequest data:
+        :return: OrganizationPackageLicensePolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_license_policy_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageLicensePolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_license_policy_violation_list(self, org, **kwargs):  # noqa: E501
+        """List all current license policy violations for this Organization.  # noqa: E501
+
+        List all current license policy violations for this Organization.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_violation_list(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str cursor: The pagination cursor value.
+        :param int page_size: Number of results to return per page.
+        :return: PackageLicensePolicyViolationLogCursorPage
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_license_policy_violation_list_with_http_info(org, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_license_policy_violation_list_with_http_info(org, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_license_policy_violation_list_with_http_info(self, org, **kwargs):  # noqa: E501
+        """List all current license policy violations for this Organization.  # noqa: E501
+
+        List all current license policy violations for this Organization.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_license_policy_violation_list_with_http_info(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str cursor: The pagination cursor value.
+        :param int page_size: Number of results to return per page.
+        :return: PackageLicensePolicyViolationLogCursorPage
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'cursor', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_license_policy_violation_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_license_policy_violation_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+
+        query_params = []
+        if 'cursor' in params:
+            query_params.append(('cursor', params['cursor']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/license-policy-violation/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PackageLicensePolicyViolationLogCursorPage',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def orgs_list(self, **kwargs):  # noqa: E501
         """Get a list of all the organizations you are associated with.  # noqa: E501
 
         Get a list of all the organizations you are associated with.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.orgs_list(async_req=True)
@@ -3115,7 +3868,760 @@
             response_type='OrganizationTeam',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_create(self, org, **kwargs):  # noqa: E501
+        """Create a package vulnerability policy.  # noqa: E501
+
+        Create a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_create(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param OrganizationPackageVulnerabilityPolicyRequest data:
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_create_with_http_info(org, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_create_with_http_info(org, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_create_with_http_info(self, org, **kwargs):  # noqa: E501
+        """Create a package vulnerability policy.  # noqa: E501
+
+        Create a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_create_with_http_info(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param OrganizationPackageVulnerabilityPolicyRequest data:
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageVulnerabilityPolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_delete(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Delete a package vulnerability policy.  # noqa: E501
+
+        Delete a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_delete(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_delete_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_delete_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_delete_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Delete a package vulnerability policy.  # noqa: E501
+
+        Delete a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_delete_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_delete" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_delete`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_vulnerability_policy_delete`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{slug_perm}/', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_list(self, org, **kwargs):  # noqa: E501
+        """Get a list of all package vulnerability policies.  # noqa: E501
+
+        Get a list of all package vulnerability policies.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_list(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[OrganizationPackageVulnerabilityPolicy]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_list_with_http_info(org, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_list_with_http_info(org, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_list_with_http_info(self, org, **kwargs):  # noqa: E501
+        """Get a list of all package vulnerability policies.  # noqa: E501
+
+        Get a list of all package vulnerability policies.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_list_with_http_info(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param int page: A page number within the paginated result set.
+        :param int page_size: Number of results to return per page.
+        :return: list[OrganizationPackageVulnerabilityPolicy]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'page', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+
+        query_params = []
+        if 'page' in params:
+            query_params.append(('page', params['page']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[OrganizationPackageVulnerabilityPolicy]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_partial_update(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a package vulnerability policy.  # noqa: E501
+
+        Partially update a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_partial_update(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageVulnerabilityPolicyRequestPatch data:
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_partial_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_partial_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_partial_update_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Partially update a package vulnerability policy.  # noqa: E501
+
+        Partially update a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_partial_update_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageVulnerabilityPolicyRequestPatch data:
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_partial_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_vulnerability_policy_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{slug_perm}/', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageVulnerabilityPolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_read(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Get a package vulnerability policy.  # noqa: E501
+
+        Get a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_read(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_read_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_read_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_read_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Get a package vulnerability policy.  # noqa: E501
+
+        Get a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_read_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_read" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_read`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_vulnerability_policy_read`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{slug_perm}/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageVulnerabilityPolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_update(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Update a package vulnerability policy.  # noqa: E501
+
+        Update a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_update(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageVulnerabilityPolicyRequest data:
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_update_with_http_info(org, slug_perm, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_update_with_http_info(self, org, slug_perm, **kwargs):  # noqa: E501
+        """Update a package vulnerability policy.  # noqa: E501
+
+        Update a package vulnerability policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_update_with_http_info(org, slug_perm, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str slug_perm: (required)
+        :param OrganizationPackageVulnerabilityPolicyRequest data:
+        :return: OrganizationPackageVulnerabilityPolicy
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'slug_perm', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_update`")  # noqa: E501
+        # verify the required parameter 'slug_perm' is set
+        if self.api_client.client_side_validation and ('slug_perm' not in params or
+                                                       params['slug_perm'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `slug_perm` when calling `orgs_vulnerability_policy_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+        if 'slug_perm' in params:
+            path_params['slug_perm'] = params['slug_perm']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy/{slug_perm}/', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='OrganizationPackageVulnerabilityPolicy',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def orgs_vulnerability_policy_violation_list(self, org, **kwargs):  # noqa: E501
+        """List all current vulnerability policy violations for this Organization.  # noqa: E501
+
+        List all current vulnerability policy violations for this Organization.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_violation_list(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str cursor: The pagination cursor value.
+        :param int page_size: Number of results to return per page.
+        :return: PackageVulnerabilityPolicyViolationLogCursorPage
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.orgs_vulnerability_policy_violation_list_with_http_info(org, **kwargs)  # noqa: E501
+        else:
+            (data) = self.orgs_vulnerability_policy_violation_list_with_http_info(org, **kwargs)  # noqa: E501
+            return data
+
+    def orgs_vulnerability_policy_violation_list_with_http_info(self, org, **kwargs):  # noqa: E501
+        """List all current vulnerability policy violations for this Organization.  # noqa: E501
+
+        List all current vulnerability policy violations for this Organization.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.orgs_vulnerability_policy_violation_list_with_http_info(org, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str org: (required)
+        :param str cursor: The pagination cursor value.
+        :param int page_size: Number of results to return per page.
+        :return: PackageVulnerabilityPolicyViolationLogCursorPage
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['org', 'cursor', 'page_size']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method orgs_vulnerability_policy_violation_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'org' is set
+        if self.api_client.client_side_validation and ('org' not in params or
+                                                       params['org'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `org` when calling `orgs_vulnerability_policy_violation_list`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'org' in params:
+            path_params['org'] = params['org']  # noqa: E501
+
+        query_params = []
+        if 'cursor' in params:
+            query_params.append(('cursor', params['cursor']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('page_size', params['page_size']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/orgs/{org}/vulnerability-policy-violation/', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PackageVulnerabilityPolicyViolationLogCursorPage',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

## cloudsmith_api/api/packages_api.py

```diff
@@ -264,17 +264,17 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def packages_dependencies(self, owner, repo, identifier, **kwargs):  # noqa: E501
-        """Get the direct (non-transitive) dependencies list for a package.  # noqa: E501
+        """Get the list of dependencies for a package. Transitive dependencies are included where supported.  # noqa: E501
 
-        Get the direct (non-transitive) dependencies list for a package.  # noqa: E501
+        Get the list of dependencies for a package. Transitive dependencies are included where supported.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.packages_dependencies(owner, repo, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
@@ -288,17 +288,17 @@
         if kwargs.get('async_req'):
             return self.packages_dependencies_with_http_info(owner, repo, identifier, **kwargs)  # noqa: E501
         else:
             (data) = self.packages_dependencies_with_http_info(owner, repo, identifier, **kwargs)  # noqa: E501
             return data
 
     def packages_dependencies_with_http_info(self, owner, repo, identifier, **kwargs):  # noqa: E501
-        """Get the direct (non-transitive) dependencies list for a package.  # noqa: E501
+        """Get the list of dependencies for a package. Transitive dependencies are included where supported.  # noqa: E501
 
-        Get the direct (non-transitive) dependencies list for a package.  # noqa: E501
+        Get the list of dependencies for a package. Transitive dependencies are included where supported.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.packages_dependencies_with_http_info(owner, repo, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
```

## cloudsmith_api/api/repos_api.py

```diff
@@ -251,15 +251,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_geoip_disable(owner, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str identifier: (required)
-        :param RespositoryGeoIPEnableDisableRequest data:
+        :param RespositoryGeoIpEnableDisableRequest data:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.repos_geoip_disable_with_http_info(owner, identifier, **kwargs)  # noqa: E501
@@ -275,15 +275,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_geoip_disable_with_http_info(owner, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str identifier: (required)
-        :param RespositoryGeoIPEnableDisableRequest data:
+        :param RespositoryGeoIpEnableDisableRequest data:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['owner', 'identifier', 'data']  # noqa: E501
         all_params.append('async_req')
@@ -362,15 +362,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_geoip_enable(owner, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str identifier: (required)
-        :param RespositoryGeoIPEnableDisableRequest data:
+        :param RespositoryGeoIpEnableDisableRequest data:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.repos_geoip_enable_with_http_info(owner, identifier, **kwargs)  # noqa: E501
@@ -386,15 +386,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_geoip_enable_with_http_info(owner, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str identifier: (required)
-        :param RespositoryGeoIPEnableDisableRequest data:
+        :param RespositoryGeoIpEnableDisableRequest data:
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['owner', 'identifier', 'data']  # noqa: E501
         all_params.append('async_req')
@@ -461,50 +461,161 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def repos_geoip_partial_update(self, owner, identifier, **kwargs):  # noqa: E501
+        """Partially update repository geoip rules.  # noqa: E501
+
+        Partially update repository geoip rules.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_geoip_partial_update(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RepositoryGeoIpRulesRequestPatch data:
+        :return: RepositoryGeoIpRules
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_geoip_partial_update_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_geoip_partial_update_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_geoip_partial_update_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Partially update repository geoip rules.  # noqa: E501
+
+        Partially update repository geoip rules.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_geoip_partial_update_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RepositoryGeoIpRulesRequestPatch data:
+        :return: RepositoryGeoIpRules
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_geoip_partial_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_geoip_partial_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_geoip_partial_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/geoip', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RepositoryGeoIpRules',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def repos_geoip_read(self, owner, identifier, **kwargs):  # noqa: E501
-        """List all created GeoIP rules for the repository.  # noqa: E501
+        """List all repository geoip rules.  # noqa: E501
 
-        List all created GeoIP rules for the repository.  # noqa: E501
+        List all repository geoip rules.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_geoip_read(owner, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str identifier: (required)
-        :return: InlineResponse200
+        :return: RepositoryGeoIpRules
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.repos_geoip_read_with_http_info(owner, identifier, **kwargs)  # noqa: E501
         else:
             (data) = self.repos_geoip_read_with_http_info(owner, identifier, **kwargs)  # noqa: E501
             return data
 
     def repos_geoip_read_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
-        """List all created GeoIP rules for the repository.  # noqa: E501
+        """List all repository geoip rules.  # noqa: E501
 
-        List all created GeoIP rules for the repository.  # noqa: E501
+        List all repository geoip rules.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repos_geoip_read_with_http_info(owner, identifier, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str owner: (required)
         :param str identifier: (required)
-        :return: InlineResponse200
+        :return: RepositoryGeoIpRules
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['owner', 'identifier']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -560,15 +671,237 @@
             '/repos/{owner}/{identifier}/geoip', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='InlineResponse200',  # noqa: E501
+            response_type='RepositoryGeoIpRules',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_geoip_test(self, owner, identifier, **kwargs):  # noqa: E501
+        """Test a list of IP addresses against the repository's current GeoIP rules.  # noqa: E501
+
+        Test a list of IP addresses against the repository's current GeoIP rules.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_geoip_test(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RepositoryGeoIpTestAddress data:
+        :return: RepositoryGeoIpTestAddressResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_geoip_test_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_geoip_test_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_geoip_test_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Test a list of IP addresses against the repository's current GeoIP rules.  # noqa: E501
+
+        Test a list of IP addresses against the repository's current GeoIP rules.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_geoip_test_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RepositoryGeoIpTestAddress data:
+        :return: RepositoryGeoIpTestAddressResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_geoip_test" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_geoip_test`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_geoip_test`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/geoip/test/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RepositoryGeoIpTestAddressResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def repos_geoip_update(self, owner, identifier, **kwargs):  # noqa: E501
+        """Replace repository geoip rules.  # noqa: E501
+
+        Replace repository geoip rules.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_geoip_update(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RepositoryGeoIpRulesRequest data:
+        :return: RepositoryGeoIpRules
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.repos_geoip_update_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+        else:
+            (data) = self.repos_geoip_update_with_http_info(owner, identifier, **kwargs)  # noqa: E501
+            return data
+
+    def repos_geoip_update_with_http_info(self, owner, identifier, **kwargs):  # noqa: E501
+        """Replace repository geoip rules.  # noqa: E501
+
+        Replace repository geoip rules.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.repos_geoip_update_with_http_info(owner, identifier, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str identifier: (required)
+        :param RepositoryGeoIpRulesRequest data:
+        :return: RepositoryGeoIpRules
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'identifier', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method repos_geoip_update" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `repos_geoip_update`")  # noqa: E501
+        # verify the required parameter 'identifier' is set
+        if self.api_client.client_side_validation and ('identifier' not in params or
+                                                       params['identifier'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `identifier` when calling `repos_geoip_update`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'identifier' in params:
+            path_params['identifier'] = params['identifier']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/repos/{owner}/{identifier}/geoip', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RepositoryGeoIpRules',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

## cloudsmith_api/models/__init__.py

```diff
@@ -12,14 +12,15 @@
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from cloudsmith_api.models.allocated_limit import AllocatedLimit
+from cloudsmith_api.models.allocated_limit_raw import AllocatedLimitRaw
 from cloudsmith_api.models.alpine_package_upload import AlpinePackageUpload
 from cloudsmith_api.models.alpine_package_upload_request import AlpinePackageUploadRequest
 from cloudsmith_api.models.architecture import Architecture
 from cloudsmith_api.models.cargo_package_upload import CargoPackageUpload
 from cloudsmith_api.models.cargo_package_upload_request import CargoPackageUploadRequest
 from cloudsmith_api.models.cocoapods_package_upload import CocoapodsPackageUpload
 from cloudsmith_api.models.cocoapods_package_upload_request import CocoapodsPackageUploadRequest
@@ -53,35 +54,43 @@
 from cloudsmith_api.models.geo_ip_location import GeoIpLocation
 from cloudsmith_api.models.go_package_upload import GoPackageUpload
 from cloudsmith_api.models.go_package_upload_request import GoPackageUploadRequest
 from cloudsmith_api.models.helm_package_upload import HelmPackageUpload
 from cloudsmith_api.models.helm_package_upload_request import HelmPackageUploadRequest
 from cloudsmith_api.models.history import History
 from cloudsmith_api.models.history_fieldset import HistoryFieldset
-from cloudsmith_api.models.inline_response200 import InlineResponse200
-from cloudsmith_api.models.inline_response200_country_code import InlineResponse200CountryCode
+from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw
 from cloudsmith_api.models.luarocks_package_upload import LuarocksPackageUpload
 from cloudsmith_api.models.luarocks_package_upload_request import LuarocksPackageUploadRequest
 from cloudsmith_api.models.maven_package_upload import MavenPackageUpload
 from cloudsmith_api.models.maven_package_upload_request import MavenPackageUploadRequest
 from cloudsmith_api.models.namespace import Namespace
 from cloudsmith_api.models.namespace_audit_log import NamespaceAuditLog
+from cloudsmith_api.models.nested_license_policy import NestedLicensePolicy
+from cloudsmith_api.models.nested_vulnerability_policy import NestedVulnerabilityPolicy
+from cloudsmith_api.models.nested_vulnerability_scan_results import NestedVulnerabilityScanResults
 from cloudsmith_api.models.npm_package_upload import NpmPackageUpload
 from cloudsmith_api.models.npm_package_upload_request import NpmPackageUploadRequest
 from cloudsmith_api.models.nuget_package_upload import NugetPackageUpload
 from cloudsmith_api.models.nuget_package_upload_request import NugetPackageUploadRequest
 from cloudsmith_api.models.organization import Organization
 from cloudsmith_api.models.organization_group_sync import OrganizationGroupSync
 from cloudsmith_api.models.organization_group_sync_request import OrganizationGroupSyncRequest
 from cloudsmith_api.models.organization_invite import OrganizationInvite
 from cloudsmith_api.models.organization_invite_extend import OrganizationInviteExtend
 from cloudsmith_api.models.organization_invite_request import OrganizationInviteRequest
 from cloudsmith_api.models.organization_invite_update import OrganizationInviteUpdate
 from cloudsmith_api.models.organization_invite_update_request_patch import OrganizationInviteUpdateRequestPatch
 from cloudsmith_api.models.organization_membership import OrganizationMembership
+from cloudsmith_api.models.organization_package_license_policy import OrganizationPackageLicensePolicy
+from cloudsmith_api.models.organization_package_license_policy_request import OrganizationPackageLicensePolicyRequest
+from cloudsmith_api.models.organization_package_license_policy_request_patch import OrganizationPackageLicensePolicyRequestPatch
+from cloudsmith_api.models.organization_package_vulnerability_policy import OrganizationPackageVulnerabilityPolicy
+from cloudsmith_api.models.organization_package_vulnerability_policy_request import OrganizationPackageVulnerabilityPolicyRequest
+from cloudsmith_api.models.organization_package_vulnerability_policy_request_patch import OrganizationPackageVulnerabilityPolicyRequestPatch
 from cloudsmith_api.models.organization_team import OrganizationTeam
 from cloudsmith_api.models.organization_team_members import OrganizationTeamMembers
 from cloudsmith_api.models.organization_team_membership import OrganizationTeamMembership
 from cloudsmith_api.models.organization_team_request import OrganizationTeamRequest
 from cloudsmith_api.models.organization_team_request_patch import OrganizationTeamRequestPatch
 from cloudsmith_api.models.p2_package_upload import P2PackageUpload
 from cloudsmith_api.models.p2_package_upload_request import P2PackageUploadRequest
@@ -90,37 +99,48 @@
 from cloudsmith_api.models.package_copy_request import PackageCopyRequest
 from cloudsmith_api.models.package_dependencies import PackageDependencies
 from cloudsmith_api.models.package_dependency import PackageDependency
 from cloudsmith_api.models.package_file import PackageFile
 from cloudsmith_api.models.package_file_parts_upload import PackageFilePartsUpload
 from cloudsmith_api.models.package_file_upload import PackageFileUpload
 from cloudsmith_api.models.package_file_upload_request import PackageFileUploadRequest
+from cloudsmith_api.models.package_license_policy_violation_log import PackageLicensePolicyViolationLog
+from cloudsmith_api.models.package_license_policy_violation_log_cursor_page import PackageLicensePolicyViolationLogCursorPage
 from cloudsmith_api.models.package_move import PackageMove
 from cloudsmith_api.models.package_move_request import PackageMoveRequest
 from cloudsmith_api.models.package_quarantine import PackageQuarantine
 from cloudsmith_api.models.package_quarantine_request import PackageQuarantineRequest
 from cloudsmith_api.models.package_resync import PackageResync
 from cloudsmith_api.models.package_status import PackageStatus
 from cloudsmith_api.models.package_tag import PackageTag
 from cloudsmith_api.models.package_tag_request import PackageTagRequest
 from cloudsmith_api.models.package_usage_metrics import PackageUsageMetrics
 from cloudsmith_api.models.package_version_badge import PackageVersionBadge
 from cloudsmith_api.models.package_vulnerability import PackageVulnerability
+from cloudsmith_api.models.package_vulnerability_policy_violation_log import PackageVulnerabilityPolicyViolationLog
+from cloudsmith_api.models.package_vulnerability_policy_violation_log_cursor_page import PackageVulnerabilityPolicyViolationLogCursorPage
 from cloudsmith_api.models.python_package_upload import PythonPackageUpload
 from cloudsmith_api.models.python_package_upload_request import PythonPackageUploadRequest
 from cloudsmith_api.models.quota import Quota
 from cloudsmith_api.models.quota_history import QuotaHistory
 from cloudsmith_api.models.rate_check import RateCheck
 from cloudsmith_api.models.raw_package_upload import RawPackageUpload
 from cloudsmith_api.models.raw_package_upload_request import RawPackageUploadRequest
 from cloudsmith_api.models.repository import Repository
 from cloudsmith_api.models.repository_audit_log import RepositoryAuditLog
 from cloudsmith_api.models.repository_create import RepositoryCreate
 from cloudsmith_api.models.repository_create_request import RepositoryCreateRequest
-from cloudsmith_api.models.repository_geo_ip_list import RepositoryGeoIPList
+from cloudsmith_api.models.repository_geo_ip_cidr import RepositoryGeoIpCidr
+from cloudsmith_api.models.repository_geo_ip_country_code import RepositoryGeoIpCountryCode
+from cloudsmith_api.models.repository_geo_ip_rules import RepositoryGeoIpRules
+from cloudsmith_api.models.repository_geo_ip_rules_request import RepositoryGeoIpRulesRequest
+from cloudsmith_api.models.repository_geo_ip_rules_request_patch import RepositoryGeoIpRulesRequestPatch
+from cloudsmith_api.models.repository_geo_ip_test_address import RepositoryGeoIpTestAddress
+from cloudsmith_api.models.repository_geo_ip_test_address_response import RepositoryGeoIpTestAddressResponse
+from cloudsmith_api.models.repository_geo_ip_test_address_response_dict import RepositoryGeoIpTestAddressResponseDict
 from cloudsmith_api.models.repository_gpg_key import RepositoryGpgKey
 from cloudsmith_api.models.repository_gpg_key_create import RepositoryGpgKeyCreate
 from cloudsmith_api.models.repository_privilege_dict import RepositoryPrivilegeDict
 from cloudsmith_api.models.repository_privilege_input import RepositoryPrivilegeInput
 from cloudsmith_api.models.repository_privilege_input_request import RepositoryPrivilegeInputRequest
 from cloudsmith_api.models.repository_privilege_input_request_patch import RepositoryPrivilegeInputRequestPatch
 from cloudsmith_api.models.repository_request_patch import RepositoryRequestPatch
@@ -134,32 +154,38 @@
 from cloudsmith_api.models.repository_token_request_patch import RepositoryTokenRequestPatch
 from cloudsmith_api.models.repository_token_sync import RepositoryTokenSync
 from cloudsmith_api.models.repository_token_sync_request import RepositoryTokenSyncRequest
 from cloudsmith_api.models.repository_webhook import RepositoryWebhook
 from cloudsmith_api.models.repository_webhook_request import RepositoryWebhookRequest
 from cloudsmith_api.models.repository_webhook_request_patch import RepositoryWebhookRequestPatch
 from cloudsmith_api.models.resources_rate_check import ResourcesRateCheck
-from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIPEnableDisable
-from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIPEnableDisableRequest
+from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIpEnableDisable
+from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIpEnableDisableRequest
 from cloudsmith_api.models.rpm_package_upload import RpmPackageUpload
 from cloudsmith_api.models.rpm_package_upload_request import RpmPackageUploadRequest
 from cloudsmith_api.models.ruby_package_upload import RubyPackageUpload
 from cloudsmith_api.models.ruby_package_upload_request import RubyPackageUploadRequest
 from cloudsmith_api.models.service import Service
 from cloudsmith_api.models.service_request import ServiceRequest
 from cloudsmith_api.models.service_request_patch import ServiceRequestPatch
 from cloudsmith_api.models.service_teams import ServiceTeams
 from cloudsmith_api.models.status_basic import StatusBasic
+from cloudsmith_api.models.storage_allocated_limit import StorageAllocatedLimit
+from cloudsmith_api.models.storage_allocated_limit_raw import StorageAllocatedLimitRaw
 from cloudsmith_api.models.storage_region import StorageRegion
+from cloudsmith_api.models.storage_usage import StorageUsage
+from cloudsmith_api.models.storage_usage_raw import StorageUsageRaw
 from cloudsmith_api.models.tags import Tags
 from cloudsmith_api.models.terraform_package_upload import TerraformPackageUpload
 from cloudsmith_api.models.terraform_package_upload_request import TerraformPackageUploadRequest
 from cloudsmith_api.models.usage import Usage
 from cloudsmith_api.models.usage_fieldset import UsageFieldset
 from cloudsmith_api.models.usage_limits import UsageLimits
+from cloudsmith_api.models.usage_limits_raw import UsageLimitsRaw
+from cloudsmith_api.models.usage_raw import UsageRaw
 from cloudsmith_api.models.user_auth_token import UserAuthToken
 from cloudsmith_api.models.user_auth_token_request import UserAuthTokenRequest
 from cloudsmith_api.models.user_brief import UserBrief
 from cloudsmith_api.models.user_profile import UserProfile
 from cloudsmith_api.models.vagrant_package_upload import VagrantPackageUpload
 from cloudsmith_api.models.vagrant_package_upload_request import VagrantPackageUploadRequest
 from cloudsmith_api.models.vulnerability import Vulnerability
```

## cloudsmith_api/models/history.py

```diff
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'days': 'int',
         'display': 'HistoryFieldset',
         'end': 'datetime',
         'plan': 'str',
-        'raw': 'HistoryFieldset',
+        'raw': 'HistoryFieldsetRaw',
         'start': 'datetime'
     }
 
     attribute_map = {
         'days': 'days',
         'display': 'display',
         'end': 'end',
@@ -170,25 +170,25 @@
 
     @property
     def raw(self):
         """Gets the raw of this History.
 
 
         :return: The raw of this History.
-        :rtype: HistoryFieldset
+        :rtype: HistoryFieldsetRaw
         """
         return self._raw
 
     @raw.setter
     def raw(self, raw):
         """Sets the raw of this History.
 
 
         :param raw: The raw of this History.
-        :type: HistoryFieldset
+        :type: HistoryFieldsetRaw
         """
         if self._configuration.client_side_validation and raw is None:
             raise ValueError("Invalid value for `raw`, must not be `None`")  # noqa: E501
 
         self._raw = raw
 
     @property
```

## cloudsmith_api/models/history_fieldset.py

```diff
@@ -30,15 +30,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'downloaded': 'Usage',
-        'storage_used': 'Usage',
+        'storage_used': 'StorageUsage',
         'uploaded': 'Usage'
     }
 
     attribute_map = {
         'downloaded': 'downloaded',
         'storage_used': 'storage_used',
         'uploaded': 'uploaded'
@@ -84,25 +84,25 @@
 
     @property
     def storage_used(self):
         """Gets the storage_used of this HistoryFieldset.
 
 
         :return: The storage_used of this HistoryFieldset.
-        :rtype: Usage
+        :rtype: StorageUsage
         """
         return self._storage_used
 
     @storage_used.setter
     def storage_used(self, storage_used):
         """Sets the storage_used of this HistoryFieldset.
 
 
         :param storage_used: The storage_used of this HistoryFieldset.
-        :type: Usage
+        :type: StorageUsage
         """
         if self._configuration.client_side_validation and storage_used is None:
             raise ValueError("Invalid value for `storage_used`, must not be `None`")  # noqa: E501
 
         self._storage_used = storage_used
 
     @property
```

## cloudsmith_api/models/organization_group_sync.py

```diff
@@ -127,30 +127,35 @@
 
         self._idp_value = idp_value
 
     @property
     def role(self):
         """Gets the role of this OrganizationGroupSync.
 
-         User role within the team.   A `manager` is capable of adding/removing others to/from the team, and  can set the role of other users and other settings pertaining to the  team.   A 'member' is a normal user that inherits the settings and privileges  assigned to the team. 
 
         :return: The role of this OrganizationGroupSync.
         :rtype: str
         """
         return self._role
 
     @role.setter
     def role(self, role):
         """Sets the role of this OrganizationGroupSync.
 
-         User role within the team.   A `manager` is capable of adding/removing others to/from the team, and  can set the role of other users and other settings pertaining to the  team.   A 'member' is a normal user that inherits the settings and privileges  assigned to the team. 
 
         :param role: The role of this OrganizationGroupSync.
         :type: str
         """
+        allowed_values = ["Manager", "Member"]  # noqa: E501
+        if (self._configuration.client_side_validation and
+                role not in allowed_values):
+            raise ValueError(
+                "Invalid value for `role` ({0}), must be one of {1}"  # noqa: E501
+                .format(role, allowed_values)
+            )
 
         self._role = role
 
     @property
     def slug_perm(self):
         """Gets the slug_perm of this OrganizationGroupSync.
```

## cloudsmith_api/models/organization_group_sync_request.py

```diff
@@ -149,30 +149,35 @@
 
         self._organization = organization
 
     @property
     def role(self):
         """Gets the role of this OrganizationGroupSyncRequest.
 
-         User role within the team.   A `manager` is capable of adding/removing others to/from the team, and  can set the role of other users and other settings pertaining to the  team.   A 'member' is a normal user that inherits the settings and privileges  assigned to the team. 
 
         :return: The role of this OrganizationGroupSyncRequest.
         :rtype: str
         """
         return self._role
 
     @role.setter
     def role(self, role):
         """Sets the role of this OrganizationGroupSyncRequest.
 
-         User role within the team.   A `manager` is capable of adding/removing others to/from the team, and  can set the role of other users and other settings pertaining to the  team.   A 'member' is a normal user that inherits the settings and privileges  assigned to the team. 
 
         :param role: The role of this OrganizationGroupSyncRequest.
         :type: str
         """
+        allowed_values = ["Manager", "Member"]  # noqa: E501
+        if (self._configuration.client_side_validation and
+                role not in allowed_values):
+            raise ValueError(
+                "Invalid value for `role` ({0}), must be one of {1}"  # noqa: E501
+                .format(role, allowed_values)
+            )
 
         self._role = role
 
     @property
     def team(self):
         """Gets the team of this OrganizationGroupSyncRequest.
```

## cloudsmith_api/models/package_dependencies.py

```diff
@@ -45,15 +45,16 @@
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._dependencies = None
         self.discriminator = None
 
-        self.dependencies = dependencies
+        if dependencies is not None:
+            self.dependencies = dependencies
 
     @property
     def dependencies(self):
         """Gets the dependencies of this PackageDependencies.
 
 
         :return: The dependencies of this PackageDependencies.
@@ -65,16 +66,14 @@
     def dependencies(self, dependencies):
         """Sets the dependencies of this PackageDependencies.
 
 
         :param dependencies: The dependencies of this PackageDependencies.
         :type: list[PackageDependency]
         """
-        if self._configuration.client_side_validation and dependencies is None:
-            raise ValueError("Invalid value for `dependencies`, must not be `None`")  # noqa: E501
 
         self._dependencies = dependencies
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

## cloudsmith_api/models/package_tag_request.py

```diff
@@ -29,26 +29,26 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'action': 'int',
+        'action': 'str',
         'is_immutable': 'bool',
         'tags': 'list[str]'
     }
 
     attribute_map = {
         'action': 'action',
         'is_immutable': 'is_immutable',
         'tags': 'tags'
     }
 
-    def __init__(self, action=None, is_immutable=False, tags=None, _configuration=None):  # noqa: E501
+    def __init__(self, action='Add', is_immutable=False, tags=None, _configuration=None):  # noqa: E501
         """PackageTagRequest - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._action = None
         self._is_immutable = None
@@ -64,26 +64,33 @@
 
     @property
     def action(self):
         """Gets the action of this PackageTagRequest.
 
 
         :return: The action of this PackageTagRequest.
-        :rtype: int
+        :rtype: str
         """
         return self._action
 
     @action.setter
     def action(self, action):
         """Sets the action of this PackageTagRequest.
 
 
         :param action: The action of this PackageTagRequest.
-        :type: int
+        :type: str
         """
+        allowed_values = ["Add", "Clear", "Replace", "Remove"]  # noqa: E501
+        if (self._configuration.client_side_validation and
+                action not in allowed_values):
+            raise ValueError(
+                "Invalid value for `action` ({0}), must be one of {1}"  # noqa: E501
+                .format(action, allowed_values)
+            )
 
         self._action = action
 
     @property
     def is_immutable(self):
         """Gets the is_immutable of this PackageTagRequest.
```

## cloudsmith_api/models/repository.py

```diff
@@ -824,16 +824,16 @@
         if (self._configuration.client_side_validation and
                 name is not None and len(name) > 50):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 name is not None and len(name) < 1):
             raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self._configuration.client_side_validation and
-                name is not None and not re.search('^\\w[\\w \\-\'\\.\/]+$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/]+$/`")  # noqa: E501
+                name is not None and not re.search('^\\w[\\w \\-\'\\.\/()]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/()]+$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def namespace(self):
         """Gets the namespace of this Repository.
```

## cloudsmith_api/models/repository_create.py

```diff
@@ -824,16 +824,16 @@
         if (self._configuration.client_side_validation and
                 name is not None and len(name) > 50):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 name is not None and len(name) < 1):
             raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self._configuration.client_side_validation and
-                name is not None and not re.search('^\\w[\\w \\-\'\\.\/]+$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/]+$/`")  # noqa: E501
+                name is not None and not re.search('^\\w[\\w \\-\'\\.\/()]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/()]+$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def namespace(self):
         """Gets the namespace of this RepositoryCreate.
```

## cloudsmith_api/models/repository_create_request.py

```diff
@@ -585,16 +585,16 @@
         if (self._configuration.client_side_validation and
                 name is not None and len(name) > 50):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 name is not None and len(name) < 1):
             raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self._configuration.client_side_validation and
-                name is not None and not re.search('^\\w[\\w \\-\'\\.\/]+$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/]+$/`")  # noqa: E501
+                name is not None and not re.search('^\\w[\\w \\-\'\\.\/()]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/()]+$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def proxy_npmjs(self):
         """Gets the proxy_npmjs of this RepositoryCreateRequest.
```

## cloudsmith_api/models/repository_request_patch.py

```diff
@@ -579,16 +579,16 @@
         if (self._configuration.client_side_validation and
                 name is not None and len(name) > 50):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `50`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 name is not None and len(name) < 1):
             raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
         if (self._configuration.client_side_validation and
-                name is not None and not re.search('^\\w[\\w \\-\'\\.\/]+$', name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/]+$/`")  # noqa: E501
+                name is not None and not re.search('^\\w[\\w \\-\'\\.\/()]+$', name)):  # noqa: E501
+            raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^\\w[\\w \\-'\\.\/()]+$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def proxy_npmjs(self):
         """Gets the proxy_npmjs of this RepositoryRequestPatch.
```

## cloudsmith_api/models/repository_token.py

```diff
@@ -780,26 +780,26 @@
 
         self._limit_package_query = limit_package_query
 
     @property
     def limit_path_query(self):
         """Gets the limit_path_query of this RepositoryToken.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :return: The limit_path_query of this RepositoryToken.
         :rtype: str
         """
         return self._limit_path_query
 
     @limit_path_query.setter
     def limit_path_query(self, limit_path_query):
         """Sets the limit_path_query of this RepositoryToken.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :param limit_path_query: The limit_path_query of this RepositoryToken.
         :type: str
         """
         if (self._configuration.client_side_validation and
                 limit_path_query is not None and len(limit_path_query) > 1024):
             raise ValueError("Invalid value for `limit_path_query`, length must be less than or equal to `1024`")  # noqa: E501
```

## cloudsmith_api/models/repository_token_refresh.py

```diff
@@ -781,26 +781,26 @@
 
         self._limit_package_query = limit_package_query
 
     @property
     def limit_path_query(self):
         """Gets the limit_path_query of this RepositoryTokenRefresh.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :return: The limit_path_query of this RepositoryTokenRefresh.
         :rtype: str
         """
         return self._limit_path_query
 
     @limit_path_query.setter
     def limit_path_query(self, limit_path_query):
         """Sets the limit_path_query of this RepositoryTokenRefresh.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :param limit_path_query: The limit_path_query of this RepositoryTokenRefresh.
         :type: str
         """
         if (self._configuration.client_side_validation and
                 limit_path_query is not None and len(limit_path_query) > 1024):
             raise ValueError("Invalid value for `limit_path_query`, length must be less than or equal to `1024`")  # noqa: E501
```

## cloudsmith_api/models/repository_token_refresh_request.py

```diff
@@ -350,26 +350,26 @@
 
         self._limit_package_query = limit_package_query
 
     @property
     def limit_path_query(self):
         """Gets the limit_path_query of this RepositoryTokenRefreshRequest.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :return: The limit_path_query of this RepositoryTokenRefreshRequest.
         :rtype: str
         """
         return self._limit_path_query
 
     @limit_path_query.setter
     def limit_path_query(self, limit_path_query):
         """Sets the limit_path_query of this RepositoryTokenRefreshRequest.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :param limit_path_query: The limit_path_query of this RepositoryTokenRefreshRequest.
         :type: str
         """
         if (self._configuration.client_side_validation and
                 limit_path_query is not None and len(limit_path_query) > 1024):
             raise ValueError("Invalid value for `limit_path_query`, length must be less than or equal to `1024`")  # noqa: E501
```

## cloudsmith_api/models/repository_token_request.py

```diff
@@ -354,26 +354,26 @@
 
         self._limit_package_query = limit_package_query
 
     @property
     def limit_path_query(self):
         """Gets the limit_path_query of this RepositoryTokenRequest.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :return: The limit_path_query of this RepositoryTokenRequest.
         :rtype: str
         """
         return self._limit_path_query
 
     @limit_path_query.setter
     def limit_path_query(self, limit_path_query):
         """Sets the limit_path_query of this RepositoryTokenRequest.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :param limit_path_query: The limit_path_query of this RepositoryTokenRequest.
         :type: str
         """
         if (self._configuration.client_side_validation and
                 limit_path_query is not None and len(limit_path_query) > 1024):
             raise ValueError("Invalid value for `limit_path_query`, length must be less than or equal to `1024`")  # noqa: E501
```

## cloudsmith_api/models/repository_token_request_patch.py

```diff
@@ -355,26 +355,26 @@
 
         self._limit_package_query = limit_package_query
 
     @property
     def limit_path_query(self):
         """Gets the limit_path_query of this RepositoryTokenRequestPatch.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :return: The limit_path_query of this RepositoryTokenRequestPatch.
         :rtype: str
         """
         return self._limit_path_query
 
     @limit_path_query.setter
     def limit_path_query(self, limit_path_query):
         """Sets the limit_path_query of this RepositoryTokenRequestPatch.
 
-        The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
+        THIS WILL SOON BE DEPRECATED, please use limit_package_query instead. The path-based search query to apply to restrict downloads to. This supports boolean logic operators such as OR/AND/NOT and parentheses for grouping. The path evaluated does not include the domain name, the namespace, the entitlement code used, the package format, etc. and it always starts with a forward slash.
 
         :param limit_path_query: The limit_path_query of this RepositoryTokenRequestPatch.
         :type: str
         """
         if (self._configuration.client_side_validation and
                 limit_path_query is not None and len(limit_path_query) > 1024):
             raise ValueError("Invalid value for `limit_path_query`, length must be less than or equal to `1024`")  # noqa: E501
```

## cloudsmith_api/models/respository_geo_ip_enable_disable.py

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from cloudsmith_api.configuration import Configuration
 
 
-class RespositoryGeoIPEnableDisable(object):
+class RespositoryGeoIpEnableDisable(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """RespositoryGeoIPEnableDisable - a model defined in Swagger"""  # noqa: E501
+        """RespositoryGeoIpEnableDisable - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RespositoryGeoIPEnableDisable, dict):
+        if issubclass(RespositoryGeoIpEnableDisable, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,19 +78,19 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RespositoryGeoIPEnableDisable):
+        if not isinstance(other, RespositoryGeoIpEnableDisable):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RespositoryGeoIPEnableDisable):
+        if not isinstance(other, RespositoryGeoIpEnableDisable):
             return True
 
         return self.to_dict() != other.to_dict()
```

## cloudsmith_api/models/respository_geo_ip_enable_disable_request.py

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from cloudsmith_api.configuration import Configuration
 
 
-class RespositoryGeoIPEnableDisableRequest(object):
+class RespositoryGeoIpEnableDisableRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """RespositoryGeoIPEnableDisableRequest - a model defined in Swagger"""  # noqa: E501
+        """RespositoryGeoIpEnableDisableRequest - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RespositoryGeoIPEnableDisableRequest, dict):
+        if issubclass(RespositoryGeoIpEnableDisableRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,19 +78,19 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RespositoryGeoIPEnableDisableRequest):
+        if not isinstance(other, RespositoryGeoIpEnableDisableRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RespositoryGeoIPEnableDisableRequest):
+        if not isinstance(other, RespositoryGeoIpEnableDisableRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

## cloudsmith_api/models/service_teams.py

```diff
@@ -50,16 +50,15 @@
 
         self._role = None
         self._slug = None
         self.discriminator = None
 
         if role is not None:
             self.role = role
-        if slug is not None:
-            self.slug = slug
+        self.slug = slug
 
     @property
     def role(self):
         """Gets the role of this ServiceTeams.
 
         The team role associated with the service
 
@@ -103,14 +102,16 @@
         """Sets the slug of this ServiceTeams.
 
         The teams associated with the service
 
         :param slug: The slug of this ServiceTeams.
         :type: str
         """
+        if self._configuration.client_side_validation and slug is None:
+            raise ValueError("Invalid value for `slug`, must not be `None`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 slug is not None and len(slug) < 1):
             raise ValueError("Invalid value for `slug`, length must be greater than or equal to `1`")  # noqa: E501
         if (self._configuration.client_side_validation and
                 slug is not None and not re.search('^[-a-zA-Z0-9_]+$', slug)):  # noqa: E501
             raise ValueError(r"Invalid value for `slug`, must be a follow pattern or equal to `/^[-a-zA-Z0-9_]+$/`")  # noqa: E501
```

## cloudsmith_api/models/status_basic.py

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'detail': 'detail',
         'version': 'version'
     }
 
-    def __init__(self, detail='Cloudsmith API is operational.', version='1.190.1', _configuration=None):  # noqa: E501
+    def __init__(self, detail='Cloudsmith API is operational.', version='1.249.4', _configuration=None):  # noqa: E501
         """StatusBasic - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._detail = None
         self._version = None
```

## cloudsmith_api/models/usage_fieldset.py

```diff
@@ -30,15 +30,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'display': 'UsageLimits',
-        'raw': 'UsageLimits'
+        'raw': 'UsageLimitsRaw'
     }
 
     attribute_map = {
         'display': 'display',
         'raw': 'raw'
     }
 
@@ -80,25 +80,25 @@
 
     @property
     def raw(self):
         """Gets the raw of this UsageFieldset.
 
 
         :return: The raw of this UsageFieldset.
-        :rtype: UsageLimits
+        :rtype: UsageLimitsRaw
         """
         return self._raw
 
     @raw.setter
     def raw(self, raw):
         """Sets the raw of this UsageFieldset.
 
 
         :param raw: The raw of this UsageFieldset.
-        :type: UsageLimits
+        :type: UsageLimitsRaw
         """
         if self._configuration.client_side_validation and raw is None:
             raise ValueError("Invalid value for `raw`, must not be `None`")  # noqa: E501
 
         self._raw = raw
 
     def to_dict(self):
```

## cloudsmith_api/models/usage_limits.py

```diff
@@ -30,15 +30,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'bandwidth': 'AllocatedLimit',
-        'storage': 'AllocatedLimit'
+        'storage': 'StorageAllocatedLimit'
     }
 
     attribute_map = {
         'bandwidth': 'bandwidth',
         'storage': 'storage'
     }
 
@@ -80,25 +80,25 @@
 
     @property
     def storage(self):
         """Gets the storage of this UsageLimits.
 
 
         :return: The storage of this UsageLimits.
-        :rtype: AllocatedLimit
+        :rtype: StorageAllocatedLimit
         """
         return self._storage
 
     @storage.setter
     def storage(self, storage):
         """Sets the storage of this UsageLimits.
 
 
         :param storage: The storage of this UsageLimits.
-        :type: AllocatedLimit
+        :type: StorageAllocatedLimit
         """
         if self._configuration.client_side_validation and storage is None:
             raise ValueError("Invalid value for `storage`, must not be `None`")  # noqa: E501
 
         self._storage = storage
 
     def to_dict(self):
```

## test/test_orgs_api.py

```diff
@@ -67,14 +67,63 @@
     def test_orgs_invites_resend(self):
         """Test case for orgs_invites_resend
 
         Resend an organization invite.  # noqa: E501
         """
         pass
 
+    def test_orgs_license_policy_create(self):
+        """Test case for orgs_license_policy_create
+
+        Create a package license policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_delete(self):
+        """Test case for orgs_license_policy_delete
+
+        Delete a package license policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_list(self):
+        """Test case for orgs_license_policy_list
+
+        Get a list of all package license policies.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_partial_update(self):
+        """Test case for orgs_license_policy_partial_update
+
+        Partially update a package license policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_read(self):
+        """Test case for orgs_license_policy_read
+
+        Get a package license policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_update(self):
+        """Test case for orgs_license_policy_update
+
+        Update a package license policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_license_policy_violation_list(self):
+        """Test case for orgs_license_policy_violation_list
+
+        List all current license policy violations for this Organization.  # noqa: E501
+        """
+        pass
+
     def test_orgs_list(self):
         """Test case for orgs_list
 
         Get a list of all the organizations you are associated with.  # noqa: E501
         """
         pass
 
@@ -228,10 +277,59 @@
     def test_orgs_teams_read(self):
         """Test case for orgs_teams_read
 
         Get the details of a specific team within an organization.  # noqa: E501
         """
         pass
 
+    def test_orgs_vulnerability_policy_create(self):
+        """Test case for orgs_vulnerability_policy_create
+
+        Create a package vulnerability policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_delete(self):
+        """Test case for orgs_vulnerability_policy_delete
+
+        Delete a package vulnerability policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_list(self):
+        """Test case for orgs_vulnerability_policy_list
+
+        Get a list of all package vulnerability policies.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_partial_update(self):
+        """Test case for orgs_vulnerability_policy_partial_update
+
+        Partially update a package vulnerability policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_read(self):
+        """Test case for orgs_vulnerability_policy_read
+
+        Get a package vulnerability policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_update(self):
+        """Test case for orgs_vulnerability_policy_update
+
+        Update a package vulnerability policy.  # noqa: E501
+        """
+        pass
+
+    def test_orgs_vulnerability_policy_violation_list(self):
+        """Test case for orgs_vulnerability_policy_violation_list
+
+        List all current vulnerability policy violations for this Organization.  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

## test/test_packages_api.py

```diff
@@ -42,15 +42,15 @@
         Delete a specific package in a repository.  # noqa: E501
         """
         pass
 
     def test_packages_dependencies(self):
         """Test case for packages_dependencies
 
-        Get the direct (non-transitive) dependencies list for a package.  # noqa: E501
+        Get the list of dependencies for a package. Transitive dependencies are included where supported.  # noqa: E501
         """
         pass
 
     def test_packages_list(self):
         """Test case for packages_list
 
         Get a list of all packages associated with repository.  # noqa: E501
```

## test/test_repos_api.py

```diff
@@ -53,18 +53,39 @@
     def test_repos_geoip_enable(self):
         """Test case for repos_geoip_enable
 
         Enable GeoIP for this repository.  # noqa: E501
         """
         pass
 
+    def test_repos_geoip_partial_update(self):
+        """Test case for repos_geoip_partial_update
+
+        Partially update repository geoip rules.  # noqa: E501
+        """
+        pass
+
     def test_repos_geoip_read(self):
         """Test case for repos_geoip_read
 
-        List all created GeoIP rules for the repository.  # noqa: E501
+        List all repository geoip rules.  # noqa: E501
+        """
+        pass
+
+    def test_repos_geoip_test(self):
+        """Test case for repos_geoip_test
+
+        Test a list of IP addresses against the repository's current GeoIP rules.  # noqa: E501
+        """
+        pass
+
+    def test_repos_geoip_update(self):
+        """Test case for repos_geoip_update
+
+        Replace repository geoip rules.  # noqa: E501
         """
         pass
 
     def test_repos_gpg_create(self):
         """Test case for repos_gpg_create
 
         Set the active GPG key for the Repository.  # noqa: E501
```

## test/test_respository_geo_ip_enable_disable.py

```diff
@@ -12,29 +12,29 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cloudsmith_api
-from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIPEnableDisable  # noqa: E501
+from cloudsmith_api.models.respository_geo_ip_enable_disable import RespositoryGeoIpEnableDisable  # noqa: E501
 from cloudsmith_api.rest import ApiException
 
 
-class TestRespositoryGeoIPEnableDisable(unittest.TestCase):
-    """RespositoryGeoIPEnableDisable unit test stubs"""
+class TestRespositoryGeoIpEnableDisable(unittest.TestCase):
+    """RespositoryGeoIpEnableDisable unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRespositoryGeoIPEnableDisable(self):
-        """Test RespositoryGeoIPEnableDisable"""
+    def testRespositoryGeoIpEnableDisable(self):
+        """Test RespositoryGeoIpEnableDisable"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cloudsmith_api.models.respository_geo_ip_enable_disable.RespositoryGeoIPEnableDisable()  # noqa: E501
+        # model = cloudsmith_api.models.respository_geo_ip_enable_disable.RespositoryGeoIpEnableDisable()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

## test/test_respository_geo_ip_enable_disable_request.py

```diff
@@ -12,29 +12,29 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cloudsmith_api
-from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIPEnableDisableRequest  # noqa: E501
+from cloudsmith_api.models.respository_geo_ip_enable_disable_request import RespositoryGeoIpEnableDisableRequest  # noqa: E501
 from cloudsmith_api.rest import ApiException
 
 
-class TestRespositoryGeoIPEnableDisableRequest(unittest.TestCase):
-    """RespositoryGeoIPEnableDisableRequest unit test stubs"""
+class TestRespositoryGeoIpEnableDisableRequest(unittest.TestCase):
+    """RespositoryGeoIpEnableDisableRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRespositoryGeoIPEnableDisableRequest(self):
-        """Test RespositoryGeoIPEnableDisableRequest"""
+    def testRespositoryGeoIpEnableDisableRequest(self):
+        """Test RespositoryGeoIpEnableDisableRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cloudsmith_api.models.respository_geo_ip_enable_disable_request.RespositoryGeoIPEnableDisableRequest()  # noqa: E501
+        # model = cloudsmith_api.models.respository_geo_ip_enable_disable_request.RespositoryGeoIpEnableDisableRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `cloudsmith_api/models/inline_response200.py` & `cloudsmith_api/models/repository_geo_ip_rules_request_patch.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,93 +15,93 @@
 import re  # noqa: F401
 
 import six
 
 from cloudsmith_api.configuration import Configuration
 
 
-class InlineResponse200(object):
+class RepositoryGeoIpRulesRequestPatch(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'country_code': 'InlineResponse200CountryCode',
-        'cidr': 'InlineResponse200CountryCode'
+        'cidr': 'RepositoryGeoIpCidr',
+        'country_code': 'RepositoryGeoIpCountryCode'
     }
 
     attribute_map = {
-        'country_code': 'country_code',
-        'cidr': 'cidr'
+        'cidr': 'cidr',
+        'country_code': 'country_code'
     }
 
-    def __init__(self, country_code=None, cidr=None, _configuration=None):  # noqa: E501
-        """InlineResponse200 - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, cidr=None, country_code=None, _configuration=None):  # noqa: E501
+        """RepositoryGeoIpRulesRequestPatch - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
-        self._country_code = None
         self._cidr = None
+        self._country_code = None
         self.discriminator = None
 
-        if country_code is not None:
-            self.country_code = country_code
         if cidr is not None:
             self.cidr = cidr
+        if country_code is not None:
+            self.country_code = country_code
 
     @property
-    def country_code(self):
-        """Gets the country_code of this InlineResponse200.
+    def cidr(self):
+        """Gets the cidr of this RepositoryGeoIpRulesRequestPatch.
 
 
-        :return: The country_code of this InlineResponse200.
-        :rtype: InlineResponse200CountryCode
+        :return: The cidr of this RepositoryGeoIpRulesRequestPatch.
+        :rtype: RepositoryGeoIpCidr
         """
-        return self._country_code
+        return self._cidr
 
-    @country_code.setter
-    def country_code(self, country_code):
-        """Sets the country_code of this InlineResponse200.
+    @cidr.setter
+    def cidr(self, cidr):
+        """Sets the cidr of this RepositoryGeoIpRulesRequestPatch.
 
 
-        :param country_code: The country_code of this InlineResponse200.
-        :type: InlineResponse200CountryCode
+        :param cidr: The cidr of this RepositoryGeoIpRulesRequestPatch.
+        :type: RepositoryGeoIpCidr
         """
 
-        self._country_code = country_code
+        self._cidr = cidr
 
     @property
-    def cidr(self):
-        """Gets the cidr of this InlineResponse200.
+    def country_code(self):
+        """Gets the country_code of this RepositoryGeoIpRulesRequestPatch.
 
 
-        :return: The cidr of this InlineResponse200.
-        :rtype: InlineResponse200CountryCode
+        :return: The country_code of this RepositoryGeoIpRulesRequestPatch.
+        :rtype: RepositoryGeoIpCountryCode
         """
-        return self._cidr
+        return self._country_code
 
-    @cidr.setter
-    def cidr(self, cidr):
-        """Sets the cidr of this InlineResponse200.
+    @country_code.setter
+    def country_code(self, country_code):
+        """Sets the country_code of this RepositoryGeoIpRulesRequestPatch.
 
 
-        :param cidr: The cidr of this InlineResponse200.
-        :type: InlineResponse200CountryCode
+        :param country_code: The country_code of this RepositoryGeoIpRulesRequestPatch.
+        :type: RepositoryGeoIpCountryCode
         """
 
-        self._cidr = cidr
+        self._country_code = country_code
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -116,15 +116,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(InlineResponse200, dict):
+        if issubclass(RepositoryGeoIpRulesRequestPatch, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,19 +132,19 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse200):
+        if not isinstance(other, RepositoryGeoIpRulesRequestPatch):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineResponse200):
+        if not isinstance(other, RepositoryGeoIpRulesRequestPatch):
             return True
 
         return self.to_dict() != other.to_dict()
```

## Comparing `cloudsmith_api/models/inline_response200_country_code.py` & `cloudsmith_api/models/repository_geo_ip_country_code.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from cloudsmith_api.configuration import Configuration
 
 
-class InlineResponse200CountryCode(object):
+class RepositoryGeoIpCountryCode(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -39,67 +39,73 @@
 
     attribute_map = {
         'allow': 'allow',
         'deny': 'deny'
     }
 
     def __init__(self, allow=None, deny=None, _configuration=None):  # noqa: E501
-        """InlineResponse200CountryCode - a model defined in Swagger"""  # noqa: E501
+        """RepositoryGeoIpCountryCode - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._allow = None
         self._deny = None
         self.discriminator = None
 
-        if allow is not None:
-            self.allow = allow
-        if deny is not None:
-            self.deny = deny
+        self.allow = allow
+        self.deny = deny
 
     @property
     def allow(self):
-        """Gets the allow of this InlineResponse200CountryCode.
+        """Gets the allow of this RepositoryGeoIpCountryCode.
 
+        The allowed country codes for this repository
 
-        :return: The allow of this InlineResponse200CountryCode.
+        :return: The allow of this RepositoryGeoIpCountryCode.
         :rtype: list[str]
         """
         return self._allow
 
     @allow.setter
     def allow(self, allow):
-        """Sets the allow of this InlineResponse200CountryCode.
+        """Sets the allow of this RepositoryGeoIpCountryCode.
 
+        The allowed country codes for this repository
 
-        :param allow: The allow of this InlineResponse200CountryCode.
+        :param allow: The allow of this RepositoryGeoIpCountryCode.
         :type: list[str]
         """
+        if self._configuration.client_side_validation and allow is None:
+            raise ValueError("Invalid value for `allow`, must not be `None`")  # noqa: E501
 
         self._allow = allow
 
     @property
     def deny(self):
-        """Gets the deny of this InlineResponse200CountryCode.
+        """Gets the deny of this RepositoryGeoIpCountryCode.
 
+        The denied country codes for this repository
 
-        :return: The deny of this InlineResponse200CountryCode.
+        :return: The deny of this RepositoryGeoIpCountryCode.
         :rtype: list[str]
         """
         return self._deny
 
     @deny.setter
     def deny(self, deny):
-        """Sets the deny of this InlineResponse200CountryCode.
+        """Sets the deny of this RepositoryGeoIpCountryCode.
 
+        The denied country codes for this repository
 
-        :param deny: The deny of this InlineResponse200CountryCode.
+        :param deny: The deny of this RepositoryGeoIpCountryCode.
         :type: list[str]
         """
+        if self._configuration.client_side_validation and deny is None:
+            raise ValueError("Invalid value for `deny`, must not be `None`")  # noqa: E501
 
         self._deny = deny
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -116,15 +122,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(InlineResponse200CountryCode, dict):
+        if issubclass(RepositoryGeoIpCountryCode, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,19 +138,19 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, InlineResponse200CountryCode):
+        if not isinstance(other, RepositoryGeoIpCountryCode):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, InlineResponse200CountryCode):
+        if not isinstance(other, RepositoryGeoIpCountryCode):
             return True
 
         return self.to_dict() != other.to_dict()
```

## Comparing `cloudsmith_api/models/repository_geo_ip_list.py` & `cloudsmith_api/models/repository_geo_ip_rules.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,95 +15,93 @@
 import re  # noqa: F401
 
 import six
 
 from cloudsmith_api.configuration import Configuration
 
 
-class RepositoryGeoIPList(object):
+class RepositoryGeoIpRules(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'cidr': 'str',
-        'country_code': 'str'
+        'cidr': 'RepositoryGeoIpCidr',
+        'country_code': 'RepositoryGeoIpCountryCode'
     }
 
     attribute_map = {
         'cidr': 'cidr',
         'country_code': 'country_code'
     }
 
     def __init__(self, cidr=None, country_code=None, _configuration=None):  # noqa: E501
-        """RepositoryGeoIPList - a model defined in Swagger"""  # noqa: E501
+        """RepositoryGeoIpRules - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._cidr = None
         self._country_code = None
         self.discriminator = None
 
-        if cidr is not None:
-            self.cidr = cidr
-        if country_code is not None:
-            self.country_code = country_code
+        self.cidr = cidr
+        self.country_code = country_code
 
     @property
     def cidr(self):
-        """Gets the cidr of this RepositoryGeoIPList.
+        """Gets the cidr of this RepositoryGeoIpRules.
 
-        List all CIDR geographic rules within the repository
 
-        :return: The cidr of this RepositoryGeoIPList.
-        :rtype: str
+        :return: The cidr of this RepositoryGeoIpRules.
+        :rtype: RepositoryGeoIpCidr
         """
         return self._cidr
 
     @cidr.setter
     def cidr(self, cidr):
-        """Sets the cidr of this RepositoryGeoIPList.
+        """Sets the cidr of this RepositoryGeoIpRules.
 
-        List all CIDR geographic rules within the repository
 
-        :param cidr: The cidr of this RepositoryGeoIPList.
-        :type: str
+        :param cidr: The cidr of this RepositoryGeoIpRules.
+        :type: RepositoryGeoIpCidr
         """
+        if self._configuration.client_side_validation and cidr is None:
+            raise ValueError("Invalid value for `cidr`, must not be `None`")  # noqa: E501
 
         self._cidr = cidr
 
     @property
     def country_code(self):
-        """Gets the country_code of this RepositoryGeoIPList.
+        """Gets the country_code of this RepositoryGeoIpRules.
 
-        List all GeoIP geographic rules within the repository
 
-        :return: The country_code of this RepositoryGeoIPList.
-        :rtype: str
+        :return: The country_code of this RepositoryGeoIpRules.
+        :rtype: RepositoryGeoIpCountryCode
         """
         return self._country_code
 
     @country_code.setter
     def country_code(self, country_code):
-        """Sets the country_code of this RepositoryGeoIPList.
+        """Sets the country_code of this RepositoryGeoIpRules.
 
-        List all GeoIP geographic rules within the repository
 
-        :param country_code: The country_code of this RepositoryGeoIPList.
-        :type: str
+        :param country_code: The country_code of this RepositoryGeoIpRules.
+        :type: RepositoryGeoIpCountryCode
         """
+        if self._configuration.client_side_validation and country_code is None:
+            raise ValueError("Invalid value for `country_code`, must not be `None`")  # noqa: E501
 
         self._country_code = country_code
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -120,15 +118,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RepositoryGeoIPList, dict):
+        if issubclass(RepositoryGeoIpRules, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -136,19 +134,19 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RepositoryGeoIPList):
+        if not isinstance(other, RepositoryGeoIpRules):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RepositoryGeoIPList):
+        if not isinstance(other, RepositoryGeoIpRules):
             return True
 
         return self.to_dict() != other.to_dict()
```

## Comparing `test/test_inline_response200.py` & `test/test_repository_geo_ip_cidr.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cloudsmith_api
-from cloudsmith_api.models.inline_response200 import InlineResponse200  # noqa: E501
+from cloudsmith_api.models.repository_geo_ip_cidr import RepositoryGeoIpCidr  # noqa: E501
 from cloudsmith_api.rest import ApiException
 
 
-class TestInlineResponse200(unittest.TestCase):
-    """InlineResponse200 unit test stubs"""
+class TestRepositoryGeoIpCidr(unittest.TestCase):
+    """RepositoryGeoIpCidr unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInlineResponse200(self):
-        """Test InlineResponse200"""
+    def testRepositoryGeoIpCidr(self):
+        """Test RepositoryGeoIpCidr"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cloudsmith_api.models.inline_response200.InlineResponse200()  # noqa: E501
+        # model = cloudsmith_api.models.repository_geo_ip_cidr.RepositoryGeoIpCidr()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `test/test_inline_response200_country_code.py` & `test/test_history_fieldset_raw.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import cloudsmith_api
-from cloudsmith_api.models.inline_response200_country_code import InlineResponse200CountryCode  # noqa: E501
+from cloudsmith_api.models.history_fieldset_raw import HistoryFieldsetRaw  # noqa: E501
 from cloudsmith_api.rest import ApiException
 
 
-class TestInlineResponse200CountryCode(unittest.TestCase):
-    """InlineResponse200CountryCode unit test stubs"""
+class TestHistoryFieldsetRaw(unittest.TestCase):
+    """HistoryFieldsetRaw unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInlineResponse200CountryCode(self):
-        """Test InlineResponse200CountryCode"""
+    def testHistoryFieldsetRaw(self):
+        """Test HistoryFieldsetRaw"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = cloudsmith_api.models.inline_response200_country_code.InlineResponse200CountryCode()  # noqa: E501
+        # model = cloudsmith_api.models.history_fieldset_raw.HistoryFieldsetRaw()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `cloudsmith_api-2.0.1.dist-info/RECORD` & `cloudsmith_api-2.0.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-cloudsmith_api/__init__.py,sha256=5asZMabU9KNw_CNMG8a23rpW_vD3P0EvjUmd6-k8nPs,13188
-cloudsmith_api/api_client.py,sha256=cwcc-FOPl5jX26THVYVgn8FdK6ig4mqyxYrN0InTAXc,25067
-cloudsmith_api/configuration.py,sha256=-3E9IJb1tMZORbb9yUI7eSjgr5qvHidU9Za5s7uxLbA,8390
+cloudsmith_api/__init__.py,sha256=NxNLPzjHYTWxaurn7a1Nfg_JJyveMWwEhOIExubwtGk,15755
+cloudsmith_api/api_client.py,sha256=db62D6KBLLKVV2yJOrvjoUgs3WiiLzAcaLDH7j9mkls,25067
+cloudsmith_api/configuration.py,sha256=rhBZacb4NPqOHLKnZN0uQeZmQriesFXzTSlRSHOiym4,8390
 cloudsmith_api/rest.py,sha256=IVGz52ALLAOqfC3YGAkqFfFjiLz5mAB_R0mIs51372Y,13166
 cloudsmith_api/api/__init__.py,sha256=oHMaETBtdkm77g6ZMGgBaWJb1Q3a8jlD8Nh02VKZd2U,1131
 cloudsmith_api/api/audit_log_api.py,sha256=cDN0Rsgck9w4qB19hpWzsTETl41Zsm-pk8Wrr14EDGs,11039
 cloudsmith_api/api/badges_api.py,sha256=PF8u5FZiEm1BFP8e52ZEDjzMo9skZVM9Qc7arsPk4vc,11425
 cloudsmith_api/api/distros_api.py,sha256=44C2sU3C43GkhRNPLK-jxlB8KrS8-KFe7Bj7KxAc-cU,7978
 cloudsmith_api/api/entitlements_api.py,sha256=Ao8Zk99xiIDEf-5GTz9YbgyaVig05QDGN0Pc2TpZmmo,54786
 cloudsmith_api/api/files_api.py,sha256=lsuhZ5M3ugbdQoqeci23QCYe15g2zVmJ3nF_nRsljZM,26620
 cloudsmith_api/api/formats_api.py,sha256=7Bv_EKqHBEnSHJIbtQ_oh-5laVu5EmofmZwBJo9h4og,7930
 cloudsmith_api/api/metrics_api.py,sha256=cTqkKtutQn2u-zNS7FHVTkxX-LSc3xRpjgbLDIqsWWc,19214
 cloudsmith_api/api/namespaces_api.py,sha256=2qCN92-asz_tZyASYgXE7gpAPBfL6W13khfmuOYV8CA,8514
-cloudsmith_api/api/orgs_api.py,sha256=3JW-xyvoBCmLNQjUrQ2_rDIQeY5w7wpSVukJ0zOO_ZI,129747
-cloudsmith_api/api/packages_api.py,sha256=j7MggT220fNCExNExrynJMMcNXxj6xMyPKBvJg5fy14,275486
+cloudsmith_api/api/orgs_api.py,sha256=mPEe7pszQCmE63DPPsc6HUXj3Z_5Awgh8gPRqTacNKQ,195413
+cloudsmith_api/api/packages_api.py,sha256=KbZCkscS-6aoPYiEIiexa_zTKRN0l_62iNsjOkLn3QQ,275618
 cloudsmith_api/api/quota_api.py,sha256=cLljkIY1w8-urDPf5Zi31YdaoWsyVrzKKz1t3Qasm_w,16386
 cloudsmith_api/api/rates_api.py,sha256=iVavoIQtWfbFE6C_jPnTQP8uG8wk0YS-ejHztrajZdY,4157
-cloudsmith_api/api/repos_api.py,sha256=2LN4M1rz6dHCsPe2AHAAasdVUOm1E_OsR3OSgyyn1eg,84121
+cloudsmith_api/api/repos_api.py,sha256=9IYStNbWWFqBnTEQfDnB14Dfp4-jrVfMG7Ea0FBnKUo,98642
 cloudsmith_api/api/status_api.py,sha256=Y7fJjz1UeBzgC2y7F8EcnBuJIFUh553zQDdk1oLGOIQ,4118
 cloudsmith_api/api/storage_regions_api.py,sha256=27lr9PVQ8G84depb-1M7z1dJ5srWscFsU776W7SRVpc,8075
 cloudsmith_api/api/user_api.py,sha256=B2_HoP2ZNBYI-2GfmmSEmucylTZV_VhU7GnnP4aYPpE,7631
 cloudsmith_api/api/users_api.py,sha256=fjOMJWnFJ8qx5i5WkiR4cdpsKR2RzdoUT_V0w-TIZVM,4706
 cloudsmith_api/api/vulnerabilities_api.py,sha256=jW4-4p0G9a31UiJZZ0Bm6Iz0gQxNLSjGSS3oNVbAQjw,22056
 cloudsmith_api/api/webhooks_api.py,sha256=RsnHyob8BKBLbqKHq3U7TizhcFJF-VCkgzJllmTZliw,26050
-cloudsmith_api/models/__init__.py,sha256=oI6AqiCuKPQX7E5eLzmlKKDHG7M1PKIZx9HI8wMbPSA,11991
+cloudsmith_api/models/__init__.py,sha256=WxCGgbJ71FAPYLFkhb2Olerq1BEGcLrhhy-yAJUS8cc,14558
 cloudsmith_api/models/allocated_limit.py,sha256=1SlEiDZ2Ozouu8Gg6CrYf47I7pJjyxUOCFtJd7Q0yzA,7305
+cloudsmith_api/models/allocated_limit_raw.py,sha256=p6vlL-y9gGwoER9aLnDeexcM0Ci6W5as9765n74SfRE,5410
 cloudsmith_api/models/alpine_package_upload.py,sha256=IUVVXR1YrQt0d52V93rFkdkHGg5YkymjC4pjUKpcxrQ,58771
 cloudsmith_api/models/alpine_package_upload_request.py,sha256=jrzolgP1mvgRKgLiDfWe6J2VS9hywOudnbpg-8zM3lk,7437
 cloudsmith_api/models/architecture.py,sha256=bzGmeP8O7tYFZfdkboF5_E34LlX-NyN2HU4W9T1Bkds,4748
 cloudsmith_api/models/cargo_package_upload.py,sha256=y6a8rNJxe9H4GWMv72MJkqnCPP-7L3YfGALtFbn8RvI,58494
 cloudsmith_api/models/cargo_package_upload_request.py,sha256=RmfIq722CsU9jPUpsofwJRXdTzjwZ0OG8js66XFUPpQ,6177
 cloudsmith_api/models/cocoapods_package_upload.py,sha256=enyJ9XU_WgEiiHzD10ac8PjUaF08pIjb7Su0bpXlLFk,59602
 cloudsmith_api/models/cocoapods_package_upload_request.py,sha256=eDvFWdZ8c7uOw8ywMucI5bDWIzVIK0LASue-PVEiLUc,6245
@@ -59,129 +60,155 @@
 cloudsmith_api/models/format.py,sha256=w9JIldZS2mRBRKo-4tYyPP9ve-4wdF-xTf9gEBvJMuI,11287
 cloudsmith_api/models/format_support.py,sha256=-TbnGczxma_ziAuD4ss-jwdHSPhE6cAI_za52K_Gbpg,7319
 cloudsmith_api/models/geo_ip_location.py,sha256=w5oOjWMH_GcOQtcUwVo0gWk_dDkPVGwmHJ2IC0RxURY,8615
 cloudsmith_api/models/go_package_upload.py,sha256=Slt7_6-PvfajmCK0wHQOKjbdwBA9qs4EgZf__MtSvFE,57663
 cloudsmith_api/models/go_package_upload_request.py,sha256=UgLfJ7yrqfuch7bEjriI8c151CWwStC21nsgOl3Hw4g,6126
 cloudsmith_api/models/helm_package_upload.py,sha256=1AwH6eg9iLHxOf-VK1lzNuWqof7zGa3D1YXjhx7YnrA,58217
 cloudsmith_api/models/helm_package_upload_request.py,sha256=QNb20d7lYd1U1y7gJ_Q5Htm5NMphVtry4U12Mcmfbas,6160
-cloudsmith_api/models/history.py,sha256=8Zk4Fe-VljaTZHVysrhfcRqJ9HKcn1odWr_hjX24E0A,7019
-cloudsmith_api/models/history_fieldset.py,sha256=QkrxDRSHrqG5X9_Eg0XIzHu0zXjX4iZ38TvuBG8ZY_8,5147
-cloudsmith_api/models/inline_response200.py,sha256=qdlp9ZCksfT7taapJWXURt2PwkfD89ekUjG8XVF0oKo,4150
-cloudsmith_api/models/inline_response200_country_code.py,sha256=kRtzWu2dE3_xVyhXNaL-TFJ92T6--PzPQtSjwSPIO3Q,4039
+cloudsmith_api/models/history.py,sha256=17AfMvcTcXVi0L8gkqSdytdMeVbNRrLVSToP9SnWsxE,7028
+cloudsmith_api/models/history_fieldset.py,sha256=Cng-daGoLVr2Hc2tlZ7_lktiEllkIGUcKjcTKG0pU-Q,5168
+cloudsmith_api/models/history_fieldset_raw.py,sha256=EV7mi9q3pTap9fsh1cVuSpTUrHrQxcmUreT-EFoUcq0,5246
 cloudsmith_api/models/luarocks_package_upload.py,sha256=D8VMxUWsIKi-evMg-AJW0r89t3hVfhrlSfa6jDNYMjM,59325
 cloudsmith_api/models/luarocks_package_upload_request.py,sha256=FQc8EpOCyRHBRBOmLC9xAl0TlZihGUnLhCE-hUlnIjk,6228
 cloudsmith_api/models/maven_package_upload.py,sha256=I68w-cFKGv_d_7h2GU_lVbq28iQbyNJiuaPezLTG9JY,61667
 cloudsmith_api/models/maven_package_upload_request.py,sha256=tEVqdFfD9sdGz6R2radMCadKIh6ReRxFktJ2ZOEjBv8,14513
 cloudsmith_api/models/namespace.py,sha256=pPo1q6hL3GaOyfeMuz85jZtPvZ7NZ5pM7GKt4VQPFfw,5806
 cloudsmith_api/models/namespace_audit_log.py,sha256=WRKsSuHhPThpTFC9aQLbWMIjxXpimne5yzQkxK-VtkU,18223
+cloudsmith_api/models/nested_license_policy.py,sha256=FDeCtx5VoWOI73YslB3z6eQa_Bloc093a6WYc94YRBc,10461
+cloudsmith_api/models/nested_vulnerability_policy.py,sha256=QfFboFfy2trv7bZe9-6I1u4eE88lQHaCmfi-6g-RUKo,11097
+cloudsmith_api/models/nested_vulnerability_scan_results.py,sha256=skZp2mjRwEh9khje1YHLN7njmZZNEiiZlQhzL_3ByJA,9219
 cloudsmith_api/models/npm_package_upload.py,sha256=IEPmH7bgimdDPVNzVZDpKI03DNtqQYnJW5qFXI1SUHw,57940
 cloudsmith_api/models/npm_package_upload_request.py,sha256=xpqvQTM7dP6S81Ztl89g0PoQoVCTg8QJr1hlZ5wZmR4,7663
 cloudsmith_api/models/nuget_package_upload.py,sha256=eExC3CDlMs3F_LvmunNevVqw3H6pTrpz-Bfoc17uW5c,58494
 cloudsmith_api/models/nuget_package_upload_request.py,sha256=_V5hSUOnLmqhcbTKRgYQIaAINNMxtcx2oYRSOXQP4No,7272
 cloudsmith_api/models/organization.py,sha256=BzOVB7ziaUvwmW8387INoJtf90stbPfxkBZ-XYqhKvQ,7918
-cloudsmith_api/models/organization_group_sync.py,sha256=AwwgftlZnvLAOgSB6heC21sNMcWbwWC7Y4HVN_jcyig,8617
-cloudsmith_api/models/organization_group_sync_request.py,sha256=j2W4WCc2eghCvTsjwgA6a0P3LRRoBS9_sfVSpeK2qfs,8449
+cloudsmith_api/models/organization_group_sync.py,sha256=Z-_Ia7wrql-e4T2lJBQVP1KZs0-9XbXQyEMXOqJV8ZM,8391
+cloudsmith_api/models/organization_group_sync_request.py,sha256=KBOHy5g1JAfcqBqvZRPupOF9huDSiJ2e_p3ZS9M0nfc,8223
 cloudsmith_api/models/organization_invite.py,sha256=Az2o6U-T9A-J39v5rDu-IIVHXkMxypHl79A0llK3_CM,10169
 cloudsmith_api/models/organization_invite_extend.py,sha256=cnrSWvGjyFgoOCYxQls0Zv0ExztcXez-XCT8aJ6mhWY,10519
 cloudsmith_api/models/organization_invite_request.py,sha256=xJLQdrXDXsAeTOKsgenEY5HGpqi18xsAAjRXbv2KA8w,5661
 cloudsmith_api/models/organization_invite_update.py,sha256=xnY-FGOU6_nI4ZRJQoYINB9OlTx8pSc07SxnwzaEVHQ,3821
 cloudsmith_api/models/organization_invite_update_request_patch.py,sha256=LzGXkpzloxzgfKYHWoO8nMYzX6yLs785T3LASWmMG1M,3929
 cloudsmith_api/models/organization_membership.py,sha256=5Y9s4HF4xVgK1CINFIpfUd7mLS9ZpmfdD8eAKpM5bXU,12300
+cloudsmith_api/models/organization_package_license_policy.py,sha256=5jempFC6tp8UaT4xJ-v35YIFAK_uBRvjz5TWiV6x3PE,11008
+cloudsmith_api/models/organization_package_license_policy_request.py,sha256=R3oBRZjcac_ebmLaKqo9iZzc9iF6SB1fpNWaIhmW6TI,8427
+cloudsmith_api/models/organization_package_license_policy_request_patch.py,sha256=Ca5Ozz45VIxKamxUJmayH3NBcD6EzRrLxmpnUAJWKhw,8280
+cloudsmith_api/models/organization_package_vulnerability_policy.py,sha256=9P8wK_nBFdib9GvgHyquELcR4k4N0Z-YGeYUbnx3c90,11620
+cloudsmith_api/models/organization_package_vulnerability_policy_request.py,sha256=2TFyV4TBreOH7DSGH62t57GCjVO_iRCrow0ayPzaf_0,8967
+cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py,sha256=DirhztKtbU7ZfyDFhmAZ8G01h-3bA3suinUW_3ElOsw,8962
 cloudsmith_api/models/organization_team.py,sha256=SJl-c2DybDkjhh99Z6I5HhAmUqoRsTISKn74VqG2pKs,8110
 cloudsmith_api/models/organization_team_members.py,sha256=erGYU0Ld15obQdUSnPRUEuqHuZiKdbM_sJIZ8cxfZu0,3669
 cloudsmith_api/models/organization_team_membership.py,sha256=yKw8jnDGeZnGe5gHOn4qOELSE54Vy4rE8CvHLKUIjTI,4783
 cloudsmith_api/models/organization_team_request.py,sha256=acFbvl-oZo00j8PszeTWbJef-gmHQi4t6t2uR3d0D1w,7065
 cloudsmith_api/models/organization_team_request_patch.py,sha256=Bh6jE5bFOQ9DH_ZFCXlvFxp_g7mMlxNFLOl_W2Z6OGs,7040
 cloudsmith_api/models/p2_package_upload.py,sha256=3YHZTGVGfMkvsY679eDd2WrekadM_KaVI2YyYe7BPmg,57663
 cloudsmith_api/models/p2_package_upload_request.py,sha256=VOEHo4ToZzZAt5m_XCSv7RcJLB7moanktYqidGoXPdw,6126
 cloudsmith_api/models/package.py,sha256=qpyCFReWWKOvnxP29gqdqlexhsN1wLkqTgcE3WugHBU,55965
 cloudsmith_api/models/package_copy.py,sha256=DWOABmICpB0_IRBUm7RGxvzA4_gKGyDGUNw-YUyBjcM,57197
 cloudsmith_api/models/package_copy_request.py,sha256=WiROah7GuiROyF-AE7I3O1bZojVOaqL8XqgDckQAdjY,4776
-cloudsmith_api/models/package_dependencies.py,sha256=ckdTxFYXpMD_iNvFI-8iw2pBxAs4Ruj36-qRy-resbw,3661
+cloudsmith_api/models/package_dependencies.py,sha256=V20LNJxN8_tUTFEBj6ygX4xzwPjtKRePbXOeRmB_C7g,3523
 cloudsmith_api/models/package_dependency.py,sha256=NB7Ok5msL8gr7b_D9YmdPOdO-YAeho4YnoIOpaFJPEE,7227
 cloudsmith_api/models/package_file.py,sha256=VRhis2DJ8H7yWL0V6Mx5WcD87HphFE5BpnEkGdVt06E,12968
 cloudsmith_api/models/package_file_parts_upload.py,sha256=NUgpfiMxAN2qU6k-gxJigd3e4pxP_XfZaJsK1reiriE,6108
 cloudsmith_api/models/package_file_upload.py,sha256=kLsYBDgujzwrcWa1D5mYSLdizqpu7kfoCrHhpp2xSxI,7841
 cloudsmith_api/models/package_file_upload_request.py,sha256=XJAVe2imaUG-kIOtIvP19RO9yktTFM_Nvcb8SmYaSTk,7815
+cloudsmith_api/models/package_license_policy_violation_log.py,sha256=LqfpVo013EdCh4gzs5TJCitgo3vEfqpOOFfDnGmktC8,6035
+cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py,sha256=tx7lA-BDmJ4aEvkhb1HDjOp1M0pll_RWK6cPKBYjpIw,5198
 cloudsmith_api/models/package_move.py,sha256=5Rf9FVxaLol6bIG7DZqNSrMasyx2SkoHWDCrTul0KsM,57195
 cloudsmith_api/models/package_move_request.py,sha256=rH-8TsDTwTLPmwOgJcc51yfyeVSqmFDNggKd0LjPciQ,3820
 cloudsmith_api/models/package_quarantine.py,sha256=lnt1g478Z7cMFBRaPlGwPqyZOBU_WCvrwt2ZApoSR6k,58775
 cloudsmith_api/models/package_quarantine_request.py,sha256=JMaDWKZ7DYOGy3lg8vYQLvIDCeMhIu8rDUiBSZ1LdSY,3527
 cloudsmith_api/models/package_resync.py,sha256=2txwMHIR-tb3jFuODLgE9BFmYKSY1i4KLODsGc-4Lvk,57651
 cloudsmith_api/models/package_status.py,sha256=MnQTlZLtSd-cGfgdjyq-QFVsKiwBeO651RKutDAoGok,15877
 cloudsmith_api/models/package_tag.py,sha256=LCUM6nMFNv5EGbfqKWa_QdygV21WO-KxXpEZK7W1CdY,57199
-cloudsmith_api/models/package_tag_request.py,sha256=I18HlbvFeeOMRvLewQJggPBNM-AEQSk4n3CupoaU3t8,4991
+cloudsmith_api/models/package_tag_request.py,sha256=VTbLpaU8j_MKE7pjZsusCAHFhRHEpyKg3pUCGioAdU8,5352
 cloudsmith_api/models/package_usage_metrics.py,sha256=M7j46JbJloiqe2D4leVEZIaksx5ftwF6OmQNd0WZs5E,3547
 cloudsmith_api/models/package_version_badge.py,sha256=yhpRbr5Mp1Zs6ZLqP0YvF3ihtT8I5-Srzmy0R2_8Ff8,2740
 cloudsmith_api/models/package_vulnerability.py,sha256=7-UFtdgFtceJ5YClNjsCtknJoYu8QlJ3Q3PGjGdC9XA,5707
+cloudsmith_api/models/package_vulnerability_policy_violation_log.py,sha256=kyMrjsBjqZ9ag-he0Rq1Lv_gqfsS1h0F2XwzNbGwK_g,7491
+cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py,sha256=FZC3S0q3ZrWXGzdifdBbze_CzGkQQ7NRDAmNm9Y0_TU,5318
 cloudsmith_api/models/python_package_upload.py,sha256=iJw8R4hVX64k8m-OGklH4z-YTFTzj7kdTJW2IJf19Nc,58771
 cloudsmith_api/models/python_package_upload_request.py,sha256=QeQVyHNe16XOY39n5OTJTJ-Nte6XyhIAlycR77VKBu4,6194
 cloudsmith_api/models/quota.py,sha256=ylCUfeFqiG_jJVYGuYWgN-Hyrx2jsoYPSjiFraD4H6k,3358
 cloudsmith_api/models/quota_history.py,sha256=MbgL9kyGqCmUugExMsdFuoYxT8UWSY6PqtyfrLDB-G0,3463
 cloudsmith_api/models/rate_check.py,sha256=oZn08kE-_pCwt5X2PapC4Mw6-rG_U6u54UnrOQdLV6w,7675
 cloudsmith_api/models/raw_package_upload.py,sha256=o4zSr0dezpZIB4hJFgJxxTT-IJpwa9j0ArMjoRkOars,58899
 cloudsmith_api/models/raw_package_upload_request.py,sha256=ZZnWmMeBiU6RZs_fmzUoe2S9EXSDwJZQgtK3VDIxwHA,11674
-cloudsmith_api/models/repository.py,sha256=8RDnlFy7MQDSntFDiHzaNBcoFgm_vE4d4qY6vbKYKYY,66225
+cloudsmith_api/models/repository.py,sha256=w8bfh1EDaJWgHOKiQI4n1pO5TxlbcoXPcXKkd0qIwvg,66229
 cloudsmith_api/models/repository_audit_log.py,sha256=MUOn8hqKio0KTSVvFCfh6eKoOoCzuj7RMiM6hWGWR6Y,14861
-cloudsmith_api/models/repository_create.py,sha256=0W_BcPKegAAidC0LPfXTg-Hm6y8psBqIdochiQDiAyY,67551
-cloudsmith_api/models/repository_create_request.py,sha256=Se5COrw_DlcLMupRFPIPMehfl8Uy3mKBFY4uYDVkfWU,52992
-cloudsmith_api/models/repository_geo_ip_list.py,sha256=2CMCDtrHcKbGYXdzDA_IBkzUPSKSbEVT8GXJRHvnWwg,4272
+cloudsmith_api/models/repository_create.py,sha256=A6e8jKpxjVEESj_uYAqvuY7ORYupPHm-kJXTXfN5faE,67555
+cloudsmith_api/models/repository_create_request.py,sha256=C5JZwvjqgaK6R7VHuFmBRPO-XHjJ3DEJfLOApe2Bwfg,52996
+cloudsmith_api/models/repository_geo_ip_cidr.py,sha256=7wJQwEwVVu0qcsvKSjnRFwAgD7n49xpVGbdJdkGwwMQ,4365
+cloudsmith_api/models/repository_geo_ip_country_code.py,sha256=kdT6ScF276kzwql9IiF5CJ7MEkDIvXiRQvuhJlVF6qE,4488
+cloudsmith_api/models/repository_geo_ip_rules.py,sha256=JIol8diaP2PNjGuasPcqB5BBf8zZ3la0e7fNEMYn4G0,4424
+cloudsmith_api/models/repository_geo_ip_rules_request.py,sha256=xsafnZmrBUr45VwlP36uBgXrG_O_a-TWW48CfkB0nKo,4515
+cloudsmith_api/models/repository_geo_ip_rules_request_patch.py,sha256=vBkRqXQnfLLwsfgaigA-nrqMmxbXi6pGQiYqFYwwz1w,4312
+cloudsmith_api/models/repository_geo_ip_test_address.py,sha256=grst-YoYiJj2oQPig3HqYqK_2kpLr38gzf3tUl_8Ytw,3733
+cloudsmith_api/models/repository_geo_ip_test_address_response.py,sha256=Nsclvv3BE136evwTnNixX_RYhOU4KNLY9pvI_Cj8rjE,3906
+cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py,sha256=7BKCqna2erKMRCPUGUugi9FQYP9JMEP8JjMruu4dAP8,7359
 cloudsmith_api/models/repository_gpg_key.py,sha256=cMQMspdP0UvOwPCDCHcEOcNky9QGuGvYO8xmN91wP-E,8734
 cloudsmith_api/models/repository_gpg_key_create.py,sha256=fXt8XT2_tGgfNkpYvLT3sFyAHSumKifCpAILQVK8CpE,5133
 cloudsmith_api/models/repository_privilege_dict.py,sha256=ZzruAgyQiiIBB5qBFag4El1tWR4-QHqDe66-r57LiA0,7702
 cloudsmith_api/models/repository_privilege_input.py,sha256=H1uipl0JCqgrB-Ea-F2WOV0U-YOZenD_wgViKq-c5yc,3818
 cloudsmith_api/models/repository_privilege_input_request.py,sha256=SbVMKEhvmAAapeV3o1yK-hE9L8yiErCuda8dgMnQ83w,3881
 cloudsmith_api/models/repository_privilege_input_request_patch.py,sha256=gRV-R-eAcfYqAKbE6bAR1hlIsfe99hJwQMps5gN2e-A,3790
-cloudsmith_api/models/repository_request_patch.py,sha256=er5JfxdV_rMgRqvsR9CFeDYsaXhBcD5hC5qmhCioGHg,51803
+cloudsmith_api/models/repository_request_patch.py,sha256=EQwQuihT-MvPt83hsuoT-25Q4Gs6kg8cPa26uahzYz0,51807
 cloudsmith_api/models/repository_rsa_key.py,sha256=m5HzgFF21eCDsik255LryTsadctALhkq3LqD2SaskZc,7753
 cloudsmith_api/models/repository_rsa_key_create.py,sha256=4QsWN17vYUeiCVIDr548BPRJPEOCR3a8UTP2vlMVoKo,5133
-cloudsmith_api/models/repository_token.py,sha256=_7pihk09MEdFvb5_l0t9_HPeC6sj0-SFfrVxe2aaybk,40082
+cloudsmith_api/models/repository_token.py,sha256=DIiQ5ZIwzMHLwKo-fPQ7ZkovCZov5RPjgo6anj2-evU,40222
 cloudsmith_api/models/repository_token_action.py,sha256=M6nBZsDLWOtqs2nGoiOsTtEpcDVLb_24REhGQDeZoPk,2750
-cloudsmith_api/models/repository_token_refresh.py,sha256=dWkNlRTfwem6QK4Y-gsfG0OF7pVN0T_N-qn5RNXkhPc,41079
-cloudsmith_api/models/repository_token_refresh_request.py,sha256=AGe7qmcQGES6K6kbULs4C2ZXMswQRtzKCSbRlExIcK4,21728
-cloudsmith_api/models/repository_token_request.py,sha256=mBptBei28dprJjPxjnom6MgeW7jvRwLBWVSo_3xZ_xc,22234
-cloudsmith_api/models/repository_token_request_patch.py,sha256=TBL-eRGIP6D28Gff5OE44ixuuvUHdUIgsHz6OZflPNc,22429
+cloudsmith_api/models/repository_token_refresh.py,sha256=l_XUV2lnvb9JOwh4xeN9tTD25TIfpkWXPFx0IIw2cXw,41219
+cloudsmith_api/models/repository_token_refresh_request.py,sha256=hX1_e-Q1jtVb-QTr_AkgESElIX_tNcHnf68qL5w2tFE,21868
+cloudsmith_api/models/repository_token_request.py,sha256=WIV-TiYm7Qq625QDyc1Kvs0d5Rh-_I6PhdVhIUllQwE,22374
+cloudsmith_api/models/repository_token_request_patch.py,sha256=8A3H75DvnqyU1-fVmE54O1hyAOtijUjNz7SYv0MeGA8,22569
 cloudsmith_api/models/repository_token_sync.py,sha256=heyuf6pEUaCNhTyZHhBb5ktOXKZ_nTuJ9zMY9BzW3ME,3505
 cloudsmith_api/models/repository_token_sync_request.py,sha256=AhwroLUUylZJlQvCxYFaOdLI0vt9m3GIep9781xu9Sg,3904
 cloudsmith_api/models/repository_webhook.py,sha256=bGH-t5dC3wTnAqV60GTX3gGfaQhTEFqMb4H--RtyXpk,30400
 cloudsmith_api/models/repository_webhook_request.py,sha256=FbkfdGvrZn7yS2PVFpgxgWDnqpfbknuJZfXluVxu9jk,18912
 cloudsmith_api/models/repository_webhook_request_patch.py,sha256=TbujXUmPBjgatch193r4wqhdoofPhWVrkfZh01GvPj8,18774
 cloudsmith_api/models/resources_rate_check.py,sha256=7LlUfH6WkOYY9J1O26LYHbK0jXnXCPyL206-G19VtWs,3523
-cloudsmith_api/models/respository_geo_ip_enable_disable.py,sha256=Na7vk3yBuaeY76FH48cZeSJ6Fyg6NfmuQGoCF5u0rrM,2790
-cloudsmith_api/models/respository_geo_ip_enable_disable_request.py,sha256=QLp6KVsIMZI5bJSSE4WyAMa76g3s94hJq76gC2HtauQ,2825
+cloudsmith_api/models/respository_geo_ip_enable_disable.py,sha256=oSzM7HSHfh7875ZOr9wbap9ciy2zFeooAVd4ceT1-7w,2790
+cloudsmith_api/models/respository_geo_ip_enable_disable_request.py,sha256=h5cWc3qwFHoh5ckaXmbIdDVAyxBu1xWTtC6hr3LxxZ4,2825
 cloudsmith_api/models/rpm_package_upload.py,sha256=EzTFVTqVaif9B17_0HZMz9sB1n-oQcxT0ng23Mbsl4U,57940
 cloudsmith_api/models/rpm_package_upload_request.py,sha256=dI7_B02n2f4DhzcTl_dClukOTFHbuL2ITWwnTEyZrOM,7374
 cloudsmith_api/models/ruby_package_upload.py,sha256=cLi1WS4JxzNIRkDjUAMtIM_Fx12s_-Th51ysO_t08Bk,58217
 cloudsmith_api/models/ruby_package_upload_request.py,sha256=pA2MIcN9TvnQBQdh-W3VsQRgkB2VkQg4lWuFalrmHmw,6160
 cloudsmith_api/models/service.py,sha256=lhEXDlJBEf2h_uhqlb0gLo9fPePbEi9Ayo4aC6Zyo6w,8234
 cloudsmith_api/models/service_request.py,sha256=JOv9I8cUiQqTFOBomiwC3KVnewi8x2Rc6NUpp4wg42g,6726
 cloudsmith_api/models/service_request_patch.py,sha256=G3Kyh4R5MA_qsdxaqygbWco5zFqdRmklQGaW0MfAKGQ,6701
-cloudsmith_api/models/service_teams.py,sha256=VFPyr1rVXB-9ovSvzJSQdyc68sr4IVaUGO8wA4c_I5U,4821
-cloudsmith_api/models/status_basic.py,sha256=dUR7U8xzLHwb7jlXE_ZDUuQybVGYyBObqL6v0PSjZBk,4584
+cloudsmith_api/models/service_teams.py,sha256=JVUDlli2nc2oVtCGZQo29lHNQRuRuEsGKei-ShRyYlA,4951
+cloudsmith_api/models/status_basic.py,sha256=cjAe5Y4FhS9avgP5LGAQwTHTjv41S29jVpkuO4aeC-c,4584
+cloudsmith_api/models/storage_allocated_limit.py,sha256=NkE1HLffx1kwuA0GamS5COBvOE3I0CyNa44Ox2vkTcQ,8478
+cloudsmith_api/models/storage_allocated_limit_raw.py,sha256=EZ2PZeIOBGfue8u0HVjurLNClceuFc5wH2UKoBqdtyQ,6140
 cloudsmith_api/models/storage_region.py,sha256=dx_5FJDAJmHrcNI4cBWiZJ6Jr06fFCA5TWYxGob9BTc,4670
+cloudsmith_api/models/storage_usage.py,sha256=EfRE_skvZ85zdc57ZKXwpacL85QGDSrMiYKf2sBQxMQ,6847
+cloudsmith_api/models/storage_usage_raw.py,sha256=fFnveEKU771hbXtZXfCV262Tm3B3RNJH6-4JPC4QFqA,5048
 cloudsmith_api/models/tags.py,sha256=p-1Zwln_mYSv2tQ3naimZtoRiFgntVOAOd9phO2zuDw,2665
 cloudsmith_api/models/terraform_package_upload.py,sha256=hXd--8XCuyh1gj9XMwmAytVoKt9zIE3qsKTYhG5H-Ws,59602
 cloudsmith_api/models/terraform_package_upload_request.py,sha256=BNrLwg_Oo0D8SE3y2I-R_ZNFyV82NtzTnQiFu0mtsyY,6245
 cloudsmith_api/models/usage.py,sha256=Ul0g37TGK2PyaL52ktLDl_nHRtrM4VQ4C9FUdW1Grt8,5738
-cloudsmith_api/models/usage_fieldset.py,sha256=5m4Nu5YlG8727B0m0wH8MfWUulLydG6QsdAWRpQH0-Y,4138
-cloudsmith_api/models/usage_limits.py,sha256=l7XbIGrUtA0BCvwg0R7KEFyhPpf7fx6WZJ1ggOg3U-0,4256
+cloudsmith_api/models/usage_fieldset.py,sha256=FtRfgLJlKKco4fH0BMrrVTUNUqYX5J3cpVPcOOaH3fA,4147
+cloudsmith_api/models/usage_limits.py,sha256=5SkxEF-RFwCFMb02sVRNU6h0ulk_L5tTpEiNshh5gL0,4277
+cloudsmith_api/models/usage_limits_raw.py,sha256=xgqXqPYTufrxi7kSW505N0TWxA8gV1lNs3IfTp9FRzU,4334
+cloudsmith_api/models/usage_raw.py,sha256=PF8QF-dzTyHU5rg3KCL7y0UNomF3ptX3MO1bdywBbss,4382
 cloudsmith_api/models/user_auth_token.py,sha256=7aTKRUgN-b4kV25CPCRXMFO8NuMbqB7j63f8KR_ERVE,3590
 cloudsmith_api/models/user_auth_token_request.py,sha256=_mi1GgiNsLkMMFONOpRemg1SD8DPbJxQvmNIEWDg214,4612
 cloudsmith_api/models/user_brief.py,sha256=FjY-e7q8d3O3pE43TuR0Oi3SzihNVkmLvjMCluJH-RE,8019
 cloudsmith_api/models/user_profile.py,sha256=R7MrOiT5xeTjkw9W2oo0S0Jr15FoyoWts6ACWJHUNrE,11110
 cloudsmith_api/models/vagrant_package_upload.py,sha256=YHZRrw8Fx5owKP2IxNKjyTgGW7G3iziRUrTkQ0xsExc,60899
 cloudsmith_api/models/vagrant_package_upload_request.py,sha256=QCeUkKr6NXB6wAEbFS5prYiv_2BCHyOpHOd0QNM3gTQ,9492
 cloudsmith_api/models/vulnerability.py,sha256=EhiEvjqjau_YWOJQvHUx8ez_iNK0L62OsooXqlYOe6s,13112
 cloudsmith_api/models/vulnerability_scan.py,sha256=l_c1Fi1f5yWuFpkZJ8b9fnoUT24mR-GymVyOXhyStr4,5400
 cloudsmith_api/models/vulnerability_scan_results.py,sha256=kIfT6aN_ptfQP7yCPym3o8Ep9PdvYYgELikIQojP1Es,10040
 cloudsmith_api/models/vulnerability_scan_results_list.py,sha256=TQ3ed-Bwh6Y9GSbs8wXqWZwN9m9YSAiYlB0IvRk6o7E,9417
 cloudsmith_api/models/vulnerability_scan_version.py,sha256=iEIDkLWfEL7Xh6wKKm7-DGY2vzbrrJNiMDzSHOKpKwM,8443
 cloudsmith_api/models/webhook_template.py,sha256=7gckCqIgyXL1qtzgJ_ShilhjC4OAj0E5dmfS6bt0MEM,4751
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_allocated_limit.py,sha256=Z9YkpJvxvcybMcK7lhy2w5WWUnB3sqf4g2YiZOZe11g,900
+test/test_allocated_limit_raw.py,sha256=do3JYGvEItmUtaw3jvSXDqtZZPFq4d8aA-FuB6e6jvE,926
 test/test_alpine_package_upload.py,sha256=WsaGcAtKxDgIqI52TuiTekpdFxTKZPUHXg-AgFcoi7A,942
 test/test_alpine_package_upload_request.py,sha256=uHCsktTOkhnw99LhXnMYfqSIapL_CZk5Bue7JBtPUW0,1000
 test/test_architecture.py,sha256=GWlvnskp29WARHM89Iuobu_NH3Ke-F_UtsQcnvwMXps,882
 test/test_audit_log_api.py,sha256=OUzS5LWdmGnr9yjGlDXuJFneGM7jGV4KdBdAwEBt2PY,1083
 test/test_badges_api.py,sha256=UvGeoUP9p9TolfcD1mCN6g4elqPC4OXQ8kK2ys_Hq84,883
 test/test_cargo_package_upload.py,sha256=XD2Ry2ZHKZxBvmcINX6WtGkBy7sgPYmX6LV-P7ta968,934
 test/test_cargo_package_upload_request.py,sha256=ROlhQn4yqG2g0oTJ2A-uI22ggJu0cCz5LlSsmeTyshI,992
@@ -221,81 +248,100 @@
 test/test_geo_ip_location.py,sha256=emR0Gn9O08c3hIq3Z0AHl1I3lrGFDQtD5xEjbEuI5GM,894
 test/test_go_package_upload.py,sha256=-JNWeb4MtT6zYxdaJ4hSnx3_YnSeF1zLUx-Z1rUCSC4,910
 test/test_go_package_upload_request.py,sha256=NkySpOxmeCFPIQaf6mSFxuE6u1-jSAuGc2do4S46I08,968
 test/test_helm_package_upload.py,sha256=10o8yyxk6c5dgU7c-XUAqtFhyB1xjZaAYxmFgXF6g2U,926
 test/test_helm_package_upload_request.py,sha256=nnG38-2Bl3noBV6PGpbmtF5FagtEUasLwd01B8oO9DM,984
 test/test_history.py,sha256=KcfXovwetcML_pfkqu-mXgjfORWPwk1RaK8YwkdQWsA,842
 test/test_history_fieldset.py,sha256=Bm7FOpV8w9-Whk32HtjzdUtzYZv4DJARQ6DhczdDmn4,908
-test/test_inline_response200.py,sha256=0jRPrjPyxTR41hw-QBskBOL1RVsc1t0qQpUqNjZzycg,924
-test/test_inline_response200_country_code.py,sha256=-TvrsWr7omnjgDrnGiNhT22K6DlKSzsqRnNAztgCZ4I,1016
+test/test_history_fieldset_raw.py,sha256=47wxdjeecweq3QtbNu6SBptW_MLpYI7q1KM2YLjwMks,934
 test/test_luarocks_package_upload.py,sha256=GYj_FvW7CbegzPRB19VjteBuCeLK5S-TVhN5cSnTkFg,958
 test/test_luarocks_package_upload_request.py,sha256=6xLeA8NDCWrRdfLFtOS3ohBNh0xzJ58CUoJvSB-XusU,1016
 test/test_maven_package_upload.py,sha256=5jSiC-GuZ3BSqByMsDRoi9iGbuOdOlkpycLiY_WFITQ,934
 test/test_maven_package_upload_request.py,sha256=2SF-gjJYFmlNinfiCRDCj0AASmwzr2AsbxluOJTpMkA,992
 test/test_metrics_api.py,sha256=crXuZZhSRBWaJ_3jrZ05GSwQhPBpNEAnvQwkX-cjFX8,1335
 test/test_namespace.py,sha256=r3GlqY-TttleCmnpyM7WyrJ1F_QadGhWBmPdcrkGK_E,858
 test/test_namespace_audit_log.py,sha256=ltgG_bIAYUT6UCiRVIOpv3lUt6JRbCNEiOgC9hTOg58,926
 test/test_namespaces_api.py,sha256=ptdTesyF3xWhFm5tcSL2dcLbKvTA7DgNwgRfyK5Q9vU,1051
+test/test_nested_license_policy.py,sha256=C-n4QFeKPfmApUwzED3FkxQrLAQarQ2JH4lIq-i9taQ,942
+test/test_nested_vulnerability_policy.py,sha256=0lXonQei5aKyKfEPyLEnmXeQ06fg9s2c7t3QFnOSCN8,990
+test/test_nested_vulnerability_scan_results.py,sha256=twIYeQF19uD1pK4KjW_flIOSLaKoMR9gRAaYNFSrBX8,1032
 test/test_npm_package_upload.py,sha256=CGaT4uu2xrFDMbp7JetsB3uQmo0NDUiIBLOUvI1PJMk,918
 test/test_npm_package_upload_request.py,sha256=8IuRpjFC9dU6fOYr_SMkZxWLknG9qCxjl-6GPmUAiW8,976
 test/test_nuget_package_upload.py,sha256=Bk_B3BFm21nP3R3l3uz-l7IwsfX9F3VwqgP3izBybRQ,934
 test/test_nuget_package_upload_request.py,sha256=cZQpVTJ5-tNAp8kpjjaTNqdeQBLf7xjowOsaxOOCIRU,992
 test/test_organization.py,sha256=eREcOoymQehUxcZOAmmDWXJ9qN9G1R-aerZwO-5JVJo,882
 test/test_organization_group_sync.py,sha256=5-NQtopJCdf8MdUgY1seiJoOIK1fRk-4_fBKy_xRf3A,958
 test/test_organization_group_sync_request.py,sha256=8CV8MJv9lNU3DyYtWDLnR7SwxP-qfxPMhqLvUGXOP9Q,1016
 test/test_organization_invite.py,sha256=s2ZxogC6P1ci60k7B1GtGC7YBkKbu7RuXyqEi3Vb_Bg,932
 test/test_organization_invite_extend.py,sha256=QDT6q7fE4jTbQxEcSiWCo6D0p1eG1unzAH2LsyAAnzs,982
 test/test_organization_invite_request.py,sha256=Ixuvzod4-_UWPMJQEA-bUI8acmvlNzz0b5W5MWphnPI,990
 test/test_organization_invite_update.py,sha256=O0CmoZVVF0HKps7DfvFM4ZJ_FmgbIO-9LDAQb4LpyNo,982
 test/test_organization_invite_update_request_patch.py,sha256=QDT8CeDnQFmuzjltXlcr43cMNtal5e4nqUxDjAXoCmo,1082
 test/test_organization_membership.py,sha256=dBHixEQ7vGdeZRJtkdAcq6peQR0V4Qk5m9j8Jbb5hqM,964
+test/test_organization_package_license_policy.py,sha256=MVJKIGkXB_sGdL8XOYReAxDNqK-iVBoI-JRF1gHuzRU,1048
+test/test_organization_package_license_policy_request.py,sha256=-34ltfWIWIi0Mzuu6SMxxw5HqU5thhHPg-N1f12-EE4,1106
+test/test_organization_package_license_policy_request_patch.py,sha256=yRop2JFxfySttOW3CC0W2Qrmmn2jo4TOEQWVjrLmgII,1148
+test/test_organization_package_vulnerability_policy.py,sha256=WrMT5cn2ylyuYpCDh4XrKRJsOPzVzqptCmwUB2xpOnE,1096
+test/test_organization_package_vulnerability_policy_request.py,sha256=p--_Ps1cJTbDGxlK1_GhLQTFn-g9NkYvk53hKY1Lpvk,1154
+test/test_organization_package_vulnerability_policy_request_patch.py,sha256=tEx5i9iLkznzWqfZVmNaE2ktVVvL4IeAPm2mzBsidXc,1196
 test/test_organization_team.py,sha256=2v-a-O2QGZHyCKwnQjQZWKpobLK2aZsu_RF7F-CHjq8,916
 test/test_organization_team_members.py,sha256=16WGRziNyDblKTBlhuN-YfFUdPunCbMxC9YrfUg8C1Q,974
 test/test_organization_team_membership.py,sha256=670Vtv_P694fq5RuOXDh_2LjIjL2aVGlUpNWFbGjcFk,998
 test/test_organization_team_request.py,sha256=1C36jTrtUkDS_L8boAIALBiDasZkbjml4-1aikC-dik,974
 test/test_organization_team_request_patch.py,sha256=YkTZUinXN-kN1CZdVD-1vW6ePQYxbLdQw_RpShRsbRg,1016
-test/test_orgs_api.py,sha256=pU-mlbWx7B4NxIS7UQr8vXvFyg0Wde8pWF9_k8tbqhQ,5914
+test/test_orgs_api.py,sha256=h2brxMBbDssctD0qJWJREnSDnndFqQatcPo6qqydOKE,8724
 test/test_p2_package_upload.py,sha256=aoiFoPo_ShLLp5GwCfICouWaC-3NBkTE0eJ0qfKU9QM,910
 test/test_p2_package_upload_request.py,sha256=KL2bMTridhweBkiuQBMU2R-fi6B6-3-hT0hthD_JxaI,968
 test/test_package.py,sha256=OulQtuNamdW7P2IH8V4-ZQcUEUrReNgVKsBYQ-jFmMs,842
 test/test_package_copy.py,sha256=7-auHuSlNVA4DGNrhbOOm6-F7URvNpcxh34RJ5Ux4wQ,876
 test/test_package_copy_request.py,sha256=wQeTnFexOXdPjNtBJ2Yiz9FTprSfCNhdDBdPfJ6MrGw,934
 test/test_package_dependencies.py,sha256=ouRcYsVryLKrIk7BKQYTQKlDnh06nPUmvxZ7htW4Uk0,940
 test/test_package_dependency.py,sha256=WJIUENn8yrmhTxuHLDPSmkWu6YFPldabbVGW7CQOvX0,924
 test/test_package_file.py,sha256=A-K2ibsMHN4ozvs1JdZq2sQb7AsDqr3epbt5uMJ_tRc,876
 test/test_package_file_parts_upload.py,sha256=BZ2T1wVk51Duk4Pgf-_83CauVnDWKy-FeUbzyHSgi2w,968
 test/test_package_file_upload.py,sha256=PUZhEifW8GiZTkzK4NRyTRErHlNhvnfhTuzIDGD0irs,926
 test/test_package_file_upload_request.py,sha256=F3XinFmLzOR9Spss5VQ73DSVqGax7J6i1fvSXJoha-c,984
+test/test_package_license_policy_violation_log.py,sha256=yTsnfWMCqpZmfEnxckU92rfcJ5CvlFE1aTUVzYVti24,1050
+test/test_package_license_policy_violation_log_cursor_page.py,sha256=2iPxBe6NCMEhqs6BqZRUeInrUUi1NHguRVShnzB-kIg,1134
 test/test_package_move.py,sha256=-wzLMgw5zxCPEdO5WTve6qX7YkSlUwq3DUIlukolLi0,876
 test/test_package_move_request.py,sha256=2NnjT9qkQWbsh5LtNoetHeiNiFx5Hvri_ZBZSLCSa9k,934
 test/test_package_quarantine.py,sha256=sb3rngGqkA1jWOnnAflSwNITyOq7IsjZWHOdMA9MUkk,924
 test/test_package_quarantine_request.py,sha256=DPj9Y30Lb6gpWpZptdZKpbbaHS4mHgYtnAwMDFAIn4s,982
 test/test_package_resync.py,sha256=c5B1GBugA9YkeASHf9mwkICAeTw7Qj5g0olVC1XvzkI,892
 test/test_package_status.py,sha256=rkTkhQpbnl9gIPoyRTILzKl5i0gSnQcmp4t8LiykOd4,892
 test/test_package_tag.py,sha256=BkcYyKWhYR0zx_a940tYo5Pm4bguJW6fnpnIboBQBi4,868
 test/test_package_tag_request.py,sha256=HXsOuuK6Tfv6fqZw8r5-PihQTJekhC5_L8kfmyh2F0w,926
 test/test_package_usage_metrics.py,sha256=SA2_RAqLdmvnXrhKq4rFEMb6jJ0uj1sIZO-WjwU9NrE,942
 test/test_package_version_badge.py,sha256=FceEfshIzpn-tZWImTMJWnhpiHObWejQv2syqoOFJ4s,942
 test/test_package_vulnerability.py,sha256=mTIkCXM1qjoanj2t0zdhGxV6TUzo9mhNmUqI1hzMlTs,948
-test/test_packages_api.py,sha256=7HQAj0Oxf24FLM-Id78p6wWWzmY8PkJUKT4PlpX-YOQ,10990
+test/test_package_vulnerability_policy_violation_log.py,sha256=iIrZ6ABnEq_AmAr3jUd9vR_FQh66W1xB7ztdstyFMY4,1098
+test/test_package_vulnerability_policy_violation_log_cursor_page.py,sha256=W5uSYYF6ZzUruutsT4Jj78KOEnNqzN-HZaIzB2IEn2Y,1182
+test/test_packages_api.py,sha256=2PIK8EGrIouF2dUQoIodbgOmw0mrRx69qCQLSvJIX_E,11023
 test/test_python_package_upload.py,sha256=9TqfbGmuNwLq5E3K2DW3jSTsj3NIUlgmQwPLQWcH3YY,942
 test/test_python_package_upload_request.py,sha256=I2Si5Gxo2QZcYiqnG9rJoKD3_uwa58Kj5XUDVS-IUpw,1000
 test/test_quota.py,sha256=MBDyrqP8f-c-sfrwseJSKhJr8n-CHk_RdVWKnzXQVeY,826
 test/test_quota_api.py,sha256=9s116ymseG0AEs5GjlYvA6sZQt3TA8314jiigYyHQ8I,1364
 test/test_quota_history.py,sha256=He4i2YAkLW9vikiNV6RkUOQvs5gUqjRUxgHihqriPAw,884
 test/test_rate_check.py,sha256=3chA15laHCwLu0QXKOyTCdiJKJbOzAQOeUTftcsaGCg,860
 test/test_rates_api.py,sha256=eEs-UjEVTAr5b40hueduthNROAGZfwy6pEx2VQaRaHM,862
 test/test_raw_package_upload.py,sha256=IOnVbqK50WyDhWqIWzscOznwL142-YLa8zv-RnAHZzM,918
 test/test_raw_package_upload_request.py,sha256=p6me4NBLN_3QVoZa8EFCiAgr21KwH2aZeJrKge1TmjQ,976
-test/test_repos_api.py,sha256=Biw3e7OePLENRRKYUYexq1xmtxaZod9o31Ay1VBCpr8,3868
+test/test_repos_api.py,sha256=qfQT2t-Y-rh6IfjXYb-Sh5IMeBubJTqU_ozmxzJDlYI,4407
 test/test_repository.py,sha256=Khjg77HHFEGxqCWDfPPU-y1Jb1dzDKdGOMm00kmWBt0,866
 test/test_repository_audit_log.py,sha256=9F9aBPgSLwK34UJrdoduvWAjo4IJpm9GPbxJbxyYJn8,934
 test/test_repository_create.py,sha256=LIA13KpeHw57CGXAXDf3-a3qCdVeM_DnG7aGIzAxwNs,916
 test/test_repository_create_request.py,sha256=egKIFHRgD_DBdb9SFbqrSfw9Y1KDiguii_YMXFIaGEY,974
-test/test_repository_geo_ip_list.py,sha256=FZKAY2MMAuu-O0Nj2WQCwScKm8QegslbUSmDPDuCwKw,944
+test/test_repository_geo_ip_cidr.py,sha256=xejx6E_I_DBzag-DFMUn_9X1q5AfT4uToDeXernxNAc,944
+test/test_repository_geo_ip_country_code.py,sha256=ump9BL4aEShFETmaRX5L2K7ECne-mn98-aBR7NpmipI,1002
+test/test_repository_geo_ip_rules.py,sha256=psSkqPoHGXWi54gPNHX8qp3404Q6iK_LYbClWlUpOQo,952
+test/test_repository_geo_ip_rules_request.py,sha256=yQ3XkaDBo4gna3jyCzK-mLS6Nd6SY3KrrlQAXf_436E,1010
+test/test_repository_geo_ip_rules_request_patch.py,sha256=SkdmcVqGaO6lL9i9x0MrBpD7rTKqfh-oO8N9EBOVzu8,1052
+test/test_repository_geo_ip_test_address.py,sha256=UGARr2LX6oY4ndFNh5cDYv59MrrE6FQiJrE6lNDj10E,1002
+test/test_repository_geo_ip_test_address_response.py,sha256=nny9RsK3VthWL7rZeBN9v1MCthdQ-AKosRpF2nswDHo,1068
+test/test_repository_geo_ip_test_address_response_dict.py,sha256=bau0pz3d807_SFu6qxpsccEB8noc_wZDPfyDHjaKP6M,1102
 test/test_repository_gpg_key.py,sha256=2nupyeqvh4tHaqI6GBTjgi4gXlAOvjT2rirl64eXOHw,918
 test/test_repository_gpg_key_create.py,sha256=KRso5DAwbUfsUf73Xj6BY1inzuuvjm2sC_DPBhnmDjo,968
 test/test_repository_privilege_dict.py,sha256=ht38XFL2qeUlkAupLexn90sRleaatJX-bJSUN9euKW8,974
 test/test_repository_privilege_input.py,sha256=iBmABbgsB-6TEHSsEccMaDZYLZCtCEiZwyY6yqJU7aY,982
 test/test_repository_privilege_input_request.py,sha256=1_C9P_3asQKdPHky-naJPN0S2AO4zsJynaT3W2qNo3M,1040
 test/test_repository_privilege_input_request_patch.py,sha256=cDrMvglJMav6bwdZzypm5VqoJMjBNvX0emxy6CGGzNs,1082
 test/test_repository_request_patch.py,sha256=EWtNLU8BLlAPGBW-zjeCexFQ6U0SESkI-_dIU9f4MeE,966
@@ -309,34 +355,40 @@
 test/test_repository_token_request_patch.py,sha256=WkvSHNBVbGlErx2t5-sJfAJbhTlSjyDiY4TADbrIu6Y,1008
 test/test_repository_token_sync.py,sha256=50jMOX3aDCHNkfP_-VOghKpz7rrr7yIESlI0ZATdjWU,942
 test/test_repository_token_sync_request.py,sha256=vY_hc4VxNdHKtdjSNFPHEoJydU3RYGATyhSd_xdeLrE,1000
 test/test_repository_webhook.py,sha256=JU-EbkiusSFl0BgNKfRlYiWYRw_5XIr_AkyBrsRD9l0,924
 test/test_repository_webhook_request.py,sha256=GoFwoKftbPU5ww8tsZwCxxAsbAcylooblPHsVeqtoB4,982
 test/test_repository_webhook_request_patch.py,sha256=T26xKDug4PM3DybormpBPr-6bxAC09_pZvFcSkDvprM,1024
 test/test_resources_rate_check.py,sha256=6sKARN2PzI439zKMj5LwExw1mYii3oWGJ15H1W8smCc,934
-test/test_respository_geo_ip_enable_disable.py,sha256=Iy0qGumdkLpr_MB8JXqF2mJsG_f3z8zI--wkwrgm5mY,1026
-test/test_respository_geo_ip_enable_disable_request.py,sha256=cpBTiHQCYEIIDWbvFRMi_AHPNhHPfThqgsXXQqdikoA,1084
+test/test_respository_geo_ip_enable_disable.py,sha256=oKirww-aJ5PVYFwMOI3_RnwNyk0yMRjc97sHqlYCy0U,1026
+test/test_respository_geo_ip_enable_disable_request.py,sha256=DcpIiUwxt_1cwIh7Qu4vypyc7jBziNAc0AbdOUn-PCE,1084
 test/test_rpm_package_upload.py,sha256=oPTf9f7iJZXSMEUnftoUWrQcj5YH7KWLoa6AlKSApy8,918
 test/test_rpm_package_upload_request.py,sha256=BKwOqvJsWd1DVkQXw64hTFXariDx7Uo_w0pi4aDwV-M,976
 test/test_ruby_package_upload.py,sha256=8qAZf0Z3nwNudKh0vwbvS0fgETivNi1zilPS4S97Ips,926
 test/test_ruby_package_upload_request.py,sha256=M-3rRvlmDDCTKDCZ1F5JakVks4tLxDzZBt9uWK7eams,984
 test/test_service.py,sha256=5iblPOypOwC59YMu85MUON5Xo2_A6C-ZDLtY7H-CPdQ,842
 test/test_service_request.py,sha256=ax3v4nmwXOMukqNVWVS8BVfnpcmsH105c4tw8YeZxyA,900
 test/test_service_request_patch.py,sha256=Hb93XIoaLRDaUF6vKxI4_ZgYPOSFmecMXa96Zio7wFs,942
 test/test_service_teams.py,sha256=gpukM2U7PtF3qbZtbBMyeTvgt6bexCsbpV-UkMSEZYs,884
 test/test_status_api.py,sha256=FQG73VMU1KsBNF9u3wPmBzlbw6AmlN3Sn9uaaAJUMec,864
 test/test_status_basic.py,sha256=PbQ_cv693ykgjTXcdivquHSHITNicdB8fhxIcsmNsM0,876
+test/test_storage_allocated_limit.py,sha256=bWe-Ylveo3nl-qyRFA8QI3Dy_eZviX22ZU0LrGKeQHQ,958
+test/test_storage_allocated_limit_raw.py,sha256=B-ee2fuKpZK5Qrhw1w0zxH0iYkg0VmBEn4wTmbp5QGc,984
 test/test_storage_region.py,sha256=BjZSa-EkFeefRy-ZR9RBS5nXBtzp8APmMTJd6XdNJOk,892
 test/test_storage_regions_api.py,sha256=I1kmxtq2MflgNeyAUr09oEQvqpbatAEECihtdJOB5_E,1088
+test/test_storage_usage.py,sha256=6Eum1n3K6FDcPHGnSqrdeyr7-A_41WsFQj9rnfzLo1c,884
+test/test_storage_usage_raw.py,sha256=2K1DanJXtZiDRZnntbL0-dkkX23jEcwa8GLe8uCa4e0,910
 test/test_tags.py,sha256=d-lPTWDjFN_G7ihzyC3EIr-EmIQdODPGQ72x-l-yOBI,818
 test/test_terraform_package_upload.py,sha256=ynJhz-h8TJ0H89EvJA1TRodUKg-QFjyVQZdCwjEcz_I,966
 test/test_terraform_package_upload_request.py,sha256=P26Jc367hdg2hhMxMhdQvJsTHkoRgeCbgiWn_cytolM,1024
 test/test_usage.py,sha256=ncymPsT2Ld4xusH3JLtDA_ZsS5-z99JiWqC5p_HIl5g,826
 test/test_usage_fieldset.py,sha256=I1IrPs87hGgH63yJVzUJd_ALI0nhrlcbUao5S_-uF2g,892
 test/test_usage_limits.py,sha256=FRrQS2vtHdBYdO2Kw3UJYyNtOHSfcyNWrfcHQiPDlIQ,876
+test/test_usage_limits_raw.py,sha256=St3yDuTIv_4qFY6gHTbsNKpSXoWJEvQVbc2d2Av_TJA,902
+test/test_usage_raw.py,sha256=7wO8ycFrqjRplqm5GaLBuR2fivxjF0Vv-yWbtDZ_9p4,852
 test/test_user_api.py,sha256=82n8RsQnK0YXob2MjQ_iJ7UhbhNO5hOeZUl1_Pv2jIM,1024
 test/test_user_auth_token.py,sha256=D19JwH469XeJEaLc9DicTHHIeM0BQySBP8crk4IpSMA,894
 test/test_user_auth_token_request.py,sha256=IsMDmx2fIeyniPMtzj5ZRwGalAbJmHB9mqQnWQfVz0Q,952
 test/test_user_brief.py,sha256=i4HR1YTMkN_un1wqpCxJVffgDkK_An3kChIUexVNklg,860
 test/test_user_profile.py,sha256=xhUpzGSJMXEfH36iBJYMfNnK6Q0eg4-Xc_7gPSIZMkI,876
 test/test_users_api.py,sha256=LQ-S4lEkFqRvv97Dz9y8AZfbSGVIr8PMV4g8Omw1vwI,865
 test/test_vagrant_package_upload.py,sha256=epUVY08Iq5IbuL7Ww5WqGUYrncdM6SIK79xA78B5BgQ,950
@@ -345,11 +397,11 @@
 test/test_vulnerability.py,sha256=4QDPIFWXKuHg_oy9PTRqFhO8yvsur5VyUFhDVkQ-Dnc,890
 test/test_vulnerability_scan.py,sha256=mGc0AETJ-UP30jb32rN5LvHeP8KFteXB8afWUED2mfI,924
 test/test_vulnerability_scan_results.py,sha256=8-nfCw6UiVWIOsTyge5XETxWxfCkB4hQf4km2lQ3pVI,982
 test/test_vulnerability_scan_results_list.py,sha256=dtcBvhUgGr6LluGnjA6x7dqQ7bkeSbCuPJpKSdHm1kQ,1016
 test/test_vulnerability_scan_version.py,sha256=hgxu72nwZ8rfEgverNQQ9_DF1A-cxa0kIBXPkEEknuk,982
 test/test_webhook_template.py,sha256=kCtiNGZ65WVUpB0an-VxzQ6-F1k-w7kTmHqdgQLSKDU,908
 test/test_webhooks_api.py,sha256=ujU1QfkYPe4MwlMR0M-p2rEfSVTzPO1Q3uB8VLiDbOg,1557
-cloudsmith_api-2.0.1.dist-info/METADATA,sha256=ZkLwSIoeAThtk-OWQAd20e5NqmKMphdZJH4ox0RJn7w,457
-cloudsmith_api-2.0.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-cloudsmith_api-2.0.1.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
-cloudsmith_api-2.0.1.dist-info/RECORD,,
+cloudsmith_api-2.0.2.dist-info/METADATA,sha256=la8ps_jKiBQ1_cDuF0kpYVCiZF7Ndt9b7xNZ68xVFhk,457
+cloudsmith_api-2.0.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+cloudsmith_api-2.0.2.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
+cloudsmith_api-2.0.2.dist-info/RECORD,,
```

