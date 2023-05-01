# Comparing `tmp/datarobot_early_access-3.2.0.2023.4.3.tar.gz` & `tmp/datarobot_early_access-3.2.0.2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.4.3.tar", last modified: Mon Apr  3 16:47:08 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.1.tar", last modified: Mon May  1 16:47:19 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.4.3.tar` & `datarobot_early_access-3.2.0.2023.5.1.tar`

### file list

```diff
@@ -1,215 +1,168 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   163889 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8482 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5719 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2140 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5320 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13072 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26517 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16695 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23584 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/deployment_monitoring.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94333 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3943 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12505 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27440 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15427 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    82114 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40997 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21197 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8969 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55708 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/datetime_trend_plots.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    92370 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4509 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16677 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10333 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_fit.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21264 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   268121 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33395 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209294 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8203 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4214 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/training_predictions.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69622 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17131 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15333 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7050 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1121 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6404 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/Makefile
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/autodoc/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18051 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/autodoc/api_reference.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10245 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/conf.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/examples/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1958 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/examples/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      415 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/getting_started.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      961 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        2 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/predicted.csv
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3474 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/credentials.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      415 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3688 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/sharing.rst
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7711 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/database_connectivity.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9959 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/dataset.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22218 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/feature_discovery.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      612 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      391 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/index.rst
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    29303 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/custom_model.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26179 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/deployment.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      427 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/index.rst
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4396 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/blueprint.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      570 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/index.rst
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5077 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/automated_documentation.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4033 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/external_testset.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      536 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10234 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/prediction_explanations.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2277 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/rating_table.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5305 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/job.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21949 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/model.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3232 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/model_recommendation.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3385 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/prime.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16205 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/project.rst
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11364 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/binary_data.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7430 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/custom_task.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10036 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/datetime_partition.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      620 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6625 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/monotonic_constraints.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6204 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/segmented_modeling.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    36391 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/time_series.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10392 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/unsupervised_anomaly.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7376 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/unsupervised_clustering.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14760 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/visualai.rst
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39016 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/batch_predictions.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1180 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/index.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9015 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/predict_job.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      319 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3173 2023-04-03 16:46:10.000000 datarobot_early_access-3.2.0.2023.4.3/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-04-03 16:46:10.000000 datarobot_early_access-3.2.0.2023.4.3/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-04-03 16:46:10.000000 datarobot_early_access-3.2.0.2023.4.3/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   167636 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8482 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5638 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2298 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/data_matching.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17252 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1598 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24335 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/deployment_monitoring.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   100246 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4192 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7683 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23045 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    82114 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40817 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    56267 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12528 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12373 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    91264 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16677 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10333 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_fit.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21264 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   268121 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9419 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209294 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6051 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      305 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    20006 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/use_cases/use_case.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17381 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-01 16:46:25.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5622 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1079 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3184 2023-05-01 16:46:26.000000 datarobot_early_access-3.2.0.2023.5.1/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-01 16:47:19.000000 datarobot_early_access-3.2.0.2023.5.1/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-01 16:46:26.000000 datarobot_early_access-3.2.0.2023.5.1/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-01 16:46:26.000000 datarobot_early_access-3.2.0.2023.5.1/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/CHANGES.rst` & `datarobot_early_access-3.2.0.2023.5.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,81 @@
 #########
 Changelog
 #########
 3.2.0b0
 ========
- 
+
 New Features
 ************
- - Added the ability to share deployments. See :ref:`deployment sharing <deployment_sharing>` for more information on sharing deployments.
+- Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
+- Added method :meth:`DatetimePartitioning.datetime_partitioning_log_list <datarobot.DatetimePartitioning.datetime_partitioning_log_list>` to list the datetime partitioning log.
+- Added :meth:`DatetimePartitioning.get_input_data <datarobot.DatetimePartitioning.get_input_data>` to retrieve the input data used to create an optimized datetime partitioning.
+- Added :class:`DatetimePartitioningId <datarobot.helpers.partitioning_methods.DatetimePartitioningId>`, which can be passed as a `partitioning_method` to :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>`.
+- Added the ability to share deployments. See :ref:`deployment sharing <deployment_sharing>` for more information on sharing deployments.
 
- - Added new methods get_bias_and_fairness_settings and update_bias_and_fairness_settings to retrieve or update bias and fairness settings
+- Added new methods get_bias_and_fairness_settings and update_bias_and_fairness_settings to retrieve or update bias and fairness settings.
    :meth:`Deployment.get_bias_and_fairness_settings<datarobot.models.Deployment.get_bias_and_fairness_settings>`
    :meth:`Deployment.update_bias_and_fairness_settings<datarobot.models.Deployment.update_bias_and_fairness_settings>`
 
+- Added a new class :class:`UseCase <datarobot.UseCase>` for interacting with the DataRobot Use Cases API.
+- Added a new class :class:`Notebook <datarobot.Notebook>` for retrieving DataRobot Notebooks available to the user.
+- Added a new class :class:`Application <datarobot.Application>` for retrieving DataRobot Applications available to the user.
+- Added a new class :class:`SharingRole <datarobot.models.sharing.SharingRole>` to hold user or organization access rights.
+- Added a new class :class:`BatchMonitoringJob <datarobot.models.BatchMonitoringJob>` for interacting with batch monitoring jobs.
+- Added a new class :class:`BatchMonitoringJobDefinition <datarobot.models.BatchMonitoringJobDefinition>` for interacting with batch monitoring jobs definitions.
+- Added a new methods for handling monitoring job definitions: list, get, create, update, delete, run_on_schedule and run_once
+  :meth:`BatchMonitoringJobDefinition.list <datarobot.models.BatchMonitoringJobDefinition.list>`
+  :meth:`BatchMonitoringJobDefinition.get <datarobot.models.BatchMonitoringJobDefinition.get>`
+  :meth:`BatchMonitoringJobDefinition.create <datarobot.models.BatchMonitoringJobDefinition.create>`
+  :meth:`BatchMonitoringJobDefinition.update <datarobot.models.BatchMonitoringJobDefinition.update>`
+  :meth:`BatchMonitoringJobDefinition.delete <datarobot.models.BatchMonitoringJobDefinition.delete>`
+  :meth:`BatchMonitoringJobDefinition.run_on_schedule <datarobot.models.BatchMonitoringJobDefinition.run_on_schedule>`
+  :meth:`BatchMonitoringJobDefinition.run_once <datarobot.models.BatchMonitoringJobDefinition.run_once>`
+- Added a new method to retrieve a monitoring job
+  :meth:`BatchMonitoringJob.get <datarobot.models.BatchMonitoringJob.get>`
+- Added the ability to filter return objects by Use Case ID to the following methods:
+  :meth:`Dataset.list <datarobot.models.Dataset.list>`
+  :meth:`Notebook.list <datarobot.Notebook.list>`
+
+- Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set by:
+
+  - invoking `Client(..., use_case = <id>)`, or
+  - setting `use_case: <id>` in drconfig.yaml, or
+  - setting the env var DATAROBOT_DEFAULT_USE_CASE, or
+  - calling `with UseCase.get(<id>):`.
+
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
   correct stage prior to calling this method.
 
 - Extended :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>` by two parameters
   to filter for a target value range in regression projects.
 
-- Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>`
+- Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>` and made sure it is returned in both :py:meth:`datarobot.PredictionExplanations.get_all_as_dataframe`  and :py:meth:`datarobot.PredictionExplanations.get_rows` method.
 
 Bugfixes
 ********
- 
+- Fix incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
+
 API Changes
 ***********
- 
+
 Deprecation Summary
 *******************
- 
+
 Configuration Changes
 *********************
- 
+- Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
+- Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
+
 Documentation Changes
 *********************
+- Fixed in-line documentation of `DataRobotClientConfig`.
 
 Experimental changes
 *********************
 - Added experimental support for data matching:
 
   - :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`
   - :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>`
@@ -49,14 +84,18 @@
 - Changed behavior for returning results in the :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. Instead of saving the results as a file, a pandas dataframe will be returned in the following methods:
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data>`
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_model>`
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_featurelist>`
 
 - Added experimental support for model lineage: :class:`ModelLineage <datarobot._experimental.models.model_lineage.ModelLineage>`
 
+- Changed behavior for methods that search for the closest data points in :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. If the index is missing, instead of throwing the error, methods try to create the index and then query it. This is enabled by default, but if this is not the intended behavior it can be changed by passing `False` to the new `build_index` parameter added to the methods:
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data>`
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_model>`
+    - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_featurelist>`
 
 3.1.0
 =====
 
 New Features
 ************
 
@@ -109,19 +148,14 @@
 - ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead. 
 
 Configuration Changes
 *********************
 
 Experimental changes
 *********************
-- Added :meth:`DatetimePartitioning.datetime_partitioning_log_retrieve <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioning.datetime_partitioning_log_retrieve>` to download the datetime partitioning log.
-
-- Added :meth:`DatetimePartitioning.get_input_data <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioning.get_input_data>` to retrieve the input data used to create an optimized datetime partitioning.
-
-- Added :class:`DatetimePartitioningId <datarobot._experimental.helpers.partitioning_methods.DatetimePartitioningId>`, which can be passed as a `partitioning_method` to :meth:`Project.analyze_and_model <datarobot.models.Project.analyze_and_model>`.
 
 Documentation Changes
 *********************
 - Update the documentation to suggest that setting `use_backtest_start_end_format` of :py:meth:`DatetimePartitioning.to_specification <datarobot.DatetimePartitioning.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 - Update the documentation to suggest setting `use_start_end_format` of :py:meth:`Backtest.to_specification <datarobot.helpers.partitioning_methods.Backtest.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
@@ -1187,15 +1221,15 @@
 - A description can now be added or updated for a project.
   :meth:`Project.set_project_description <datarobot.models.Project.set_project_description>`.
 
 - Added new parameters `read_timeout` and `max_wait` to method :meth:`Dataset.create_from_file<datarobot.models.Dataset.create_from_file>`.
   Values larger than the default can be specified for both to avoid timeouts when uploading large files.
 
 
-- Added new parameter `metric` to :class:`datarobot.models.TargetDrift`, :class:`datarobot.models.FeatureDrift`,
+- Added new parameter `metric` to :class:`datarobot.models.deployment.TargetDrift`, :class:`datarobot.models.deployment.FeatureDrift`,
   :meth:`Deployment.get_target_drift<datarobot.models.Deployment.get_target_drift>`
   and :meth:`Deployment.get_feature_drift<datarobot.models.Deployment.get_feature_drift>`.
 
 - Added new parameter `timeout` to :meth:`BatchPredictionJob.download <datarobot.models.BatchPredictionJob.download>` to indicate
   how many seconds to wait for the download to start (in case the job doesn't start processing immediately).
   Set to ``-1`` to disable.
   This parameter can also be sent as `download_timeout` to :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`
@@ -1337,16 +1371,16 @@
     :class:`ExternalScores<datarobot.ExternalScores>`, :class:`ExternalLiftChart<datarobot.ExternalLiftChart>`, :class:`ExternalRocCurve<datarobot.ExternalRocCurve>`.
 
 - Users can create payoff matrices for generating profit curves for binary classification projects
   using :meth:`PayoffMatrix.create <datarobot.models.PayoffMatrix.create>`.
 
 - Deployment Improvements:
 
-  - :class:`datarobot.models.TargetDrift` can be used to retrieve target drift information.
-  - :class:`datarobot.models.FeatureDrift` can be used to retrieve feature drift information.
+  - :class:`datarobot.models.deployment.TargetDrift` can be used to retrieve target drift information.
+  - :class:`datarobot.models.deployment.FeatureDrift` can be used to retrieve feature drift information.
   - :meth:`Deployment.submit_actuals<datarobot.models.Deployment.submit_actuals>` will submit actuals in batches if the total number of actuals exceeds the limit of one single request.
   - ``Deployment.create_from_custom_model_image`` can be used to create a deployment from a custom model image.
   - Deployments now support predictions data collection that enables prediction requests and results to be saved in Predictions Data Storage. See
     :meth:`Deployment.get_predictions_data_collection_settings<datarobot.models.Deployment.get_predictions_data_collection_settings>`
     and :meth:`Deployment.update_predictions_data_collection_settings<datarobot.models.Deployment.update_predictions_data_collection_settings>` for usage.
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/LICENSE.txt` & `datarobot_early_access-3.2.0.2023.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.2.0.2023.4.3
+Version: 3.2.0.2023.5.1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/README.md` & `datarobot_early_access-3.2.0.2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/common_setup.py` & `datarobot_early_access-3.2.0.2023.5.1/common_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -131,23 +131,20 @@
 ] + images_require
 
 dev_require = (
     tests_require
     + lint_require
     + images_require
     + [
-        "Sphinx==1.8.3",
-        "sphinx_rtd_theme==0.1.9",
-        "nbsphinx>=0.2.9,<1",
-        "mistune==0.8.4",
-        "nbconvert==5.3.1",
-        "numpydoc>=0.6.0",
+        "Sphinx==4.3.2",
+        "sphinx_rtd_theme==1.0.0",
+        "nbsphinx==0.8.9",
+        "numpydoc==1.4.0",
         "jupyter_contrib_nbextensions",
-        "tornado<6.0",
-        "jsonschema<=4.3.1",
+        "sphinx-autodoc-typehints==1.17.1",
     ]
 )
 
 example_require = [
     "jupyter<=5.0",
     "fredapi==0.4.0",
     "matplotlib>=2.1.0",
@@ -177,22 +174,21 @@
     license="DataRobot Tool and Utility Agreement",
     packages=None,
     package_data={"datarobot": ["py.typed"]},
     python_requires=">=3.7",
     long_description=None,
     classifiers=None,
     install_requires=[
-        "contextlib2>=0.5.5",
         "pandas>=0.15",
         "numpy",
         "pyyaml>=3.11",
-        "requests>=2.21",
+        "requests>=2.28.1",
         "requests_toolbelt>=0.6",
         "trafaret>=0.7,<2.2,!=1.1.0",
-        "urllib3>=1.23",
+        "urllib3>=1.23,<2.0.0",
         "typing-extensions==4.3.0",
     ],
     extras_require={
         "dev": dev_require,
         "examples": example_require,
         "release": release_require,
         "lint": lint_require,
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/__init__.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # flake8: noqa
 
 from ._version import __version__
 from .client import Client
+from .context import _context
 from .enums import (
     AUTOPILOT_MODE,
     NETWORK_EGRESS_POLICY,
     QUEUE_STATUS,
     SCORING_TYPE,
     SNAPSHOT_POLICY,
     TARGET_TYPE,
     VERBOSITY_LEVEL,
 )
 from .errors import AppPlatformError
 from .helpers import *
 from .models import (
+    Application,
     AutomatedDocument,
+    BatchMonitoringJob,
+    BatchMonitoringJobDefinition,
     BatchPredictionJob,
     BatchPredictionJobDefinition,
     BlenderModel,
     Blueprint,
     BlueprintChart,
     BlueprintTaskDocument,
     CalendarFile,
@@ -69,14 +73,15 @@
     Job,
     Model,
     ModelBlueprintChart,
     ModelingFeature,
     ModelingFeaturelist,
     ModelJob,
     ModelRecommendation,
+    Notebook,
     PayoffMatrix,
     PredictionDataset,
     PredictionExplanations,
     PredictionExplanationsInitialization,
     Predictions,
     PredictionServer,
     PredictJob,
@@ -92,9 +97,12 @@
     SegmentInfo,
     ShapImpact,
     ShapMatrix,
     ShapMatrixJob,
     SharingAccess,
     TrainingPredictions,
     TrainingPredictionsJob,
+    UseCase,
     UserBlueprint,
 )
+
+Context = _context.get()
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_compat.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
 import logging
 
-from .helpers.partitioning_methods import DatetimePartitioning, DatetimePartitioningId
 from .models.enums import UnsupervisedTypeEnum
 from .models.idiomatic_project import IdiomaticProject
 from .models.model import DatetimeModel, Model
 
 logger = logging.getLogger(__package__)
 
 experimental_warning = (
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/data_matching.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,31 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+import functools
 from io import BytesIO
+import logging
 import os
-from typing import Any, List, Optional
+from typing import Any, Callable, List, Optional
 
 import pandas as pd
 import trafaret as t
 
 from datarobot.enums import DEFAULT_MAX_WAIT
+from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
 from datarobot.utils import get_id_from_location, pagination
 from datarobot.utils.waiters import wait_for_async_resolution
 
+logger = logging.getLogger(__package__)
+
 
 class DataMatching(APIObject):
     """
     Retrieves the closest data points for the input data.
 
     This functionality is more than the simple lookup. In order to retrieve the closest data
     points data matching functionality will leverage DataRobot preprocessing pipeline first
@@ -61,144 +66,180 @@
         return f"DataMatching(project_id={self.project_id})"
 
     def get_query_url(self, url: str, number_of_data: Optional[int] = None) -> str:
         """Returns formatted data matching query url"""
         return f"{url}?numberOfData={number_of_data}" if number_of_data else url
 
     def _execute_data_matching_query(
-        self, url: str, query_file_path: str, max_wait: int
+        self,
+        url: str,
+        query_file_path: str,
+        max_wait: int,
+        build_index_func: Optional[Callable[[], None]] = None,
     ) -> "DataMatchingQuery":
         """Makes the data matching query and returns data matching query instance.
 
         Parameters
         ----------
         url: str
             Data matching query url to make request to
         query_file_path: str
             Path to file with the data point to search closest data points
         max_wait: int
             Number of seconds to wait for the result
+        build_index_func: Callable or None
+            Method to create an index if found to be missing. Default None.
+            If None is specified an error is thrown if the index is missing.
 
         Returns
         -------
         data_matching_query: DataMatchingQuery
             Data matching query instance
         """
         fname = os.path.basename(query_file_path)
-        response = self._client.build_request_with_file(
-            method="POST",
-            url=url,
-            fname=fname,
-            file_path=query_file_path,
-        )
+        try:
+            response = self._client.build_request_with_file(
+                method="POST", url=url, fname=fname, file_path=query_file_path
+            )
+        except ClientError as exc:
+            # If the client error is related to missing index: build it and retry
+            if exc.status_code == 404 and build_index_func:
+                logger.info("Index is missing, index will be built before processing the query")
+                build_index_func()
+                return self._execute_data_matching_query(url, query_file_path, max_wait)
+            raise
+
         location = wait_for_async_resolution(self._client, response.headers["Location"], max_wait)
         data_matching_query = DataMatchingQuery(
             project_id=self.project_id, data_matching_id=get_id_from_location(location)
         )
         return data_matching_query
 
     def get_closest_data(
         self,
         query_file_path: str,
         number_of_data: Optional[int] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
+        build_index_if_missing: bool = True,
     ) -> pd.DataFrame:
-        """Retrieves closest data points to the data point in input file.
+        """Retrieves closest data points to the data point in input file. If the index is missing
+        by default the method will try to build it.
 
         Parameters
         ----------
         query_file_path: str
             Path to file with the data point to search closest data points
         number_of_data: int or None
             Number of results to search for. If no value specified, the default is 10.
         max_wait: int
             Number of seconds to wait for the result. Default is 600.
+        build_index_if_missing: Optional[bool]
+            Should the index be created if it is missing. If False is specified and the index
+            is missing, an exception is thrown. Default True.
 
         Returns
         -------
         df: pd.DataFrame
             Dataframe with query result
         """
         url = self._get_closest_data_path.format(project_id=self.project_id)
+        build_index_func = functools.partial(self.build_index, max_wait)
         data_matching_query = self._execute_data_matching_query(
             url=self.get_query_url(url, number_of_data),
             query_file_path=query_file_path,
             max_wait=max_wait,
+            build_index_func=build_index_func if build_index_if_missing else None,
         )
         df = data_matching_query.get_result()
         return df
 
     def get_closest_data_for_model(
         self,
         model_id: str,
         query_file_path: str,
         number_of_data: Optional[int] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
+        build_index_if_missing: bool = True,
     ) -> pd.DataFrame:
-        """Retrieves closest data points to the data point in input file.
+        """Retrieves closest data points to the data point in input file. If the index is missing
+        by default the method will try to build it.
 
         Parameters
         ----------
         model_id: str
             Id of the model to search for the closest data points
         query_file_path: str
             Path to file with the data point to search closest data points
         number_of_data: int or None
             Number of results to search for. If no value specified, the default is 10.
         max_wait: int
             Number of seconds to wait for the result. Default is 600.
+        build_index_if_missing: Optional[bool]
+            Should the index be created if it is missing. If False is specified and the index
+            is missing, an exception is thrown. Default True.
 
         Returns
         -------
         df: pd.DataFrame
             Dataframe with query result
         """
         url = self._get_closest_data_model_path.format(
             project_id=self.project_id, model_id=model_id
         )
+        build_index_func = functools.partial(self.build_index_for_model, model_id, max_wait)
         data_matching_query = self._execute_data_matching_query(
             url=self.get_query_url(url, number_of_data),
             query_file_path=query_file_path,
             max_wait=max_wait,
+            build_index_func=build_index_func if build_index_if_missing else None,
         )
         df = data_matching_query.get_result()
         return df
 
     def get_closest_data_for_featurelist(
         self,
         featurelist_id: str,
         query_file_path: str,
         number_of_data: Optional[int] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
+        build_index_if_missing: bool = True,
     ) -> pd.DataFrame:
-        """Retrieves closest data points to the data point in input file.
+        """Retrieves closest data points to the data point in input file. If the index is missing
+        by default the method will try to build it.
 
         Parameters
         ----------
         featurelist_id: str
             Id of the featurelist to search for the closest data points
         query_file_path: str
             Path to file with the data point to search closest data points
         number_of_data: int or None
             Number of results to search for. If no value specified, the default is 10.
         max_wait: int
             Number of seconds to wait for the result. Default is 600.
+        build_index_if_missing: bool
+            Should the index be created if it is missing. If False is specified and the index
+            is missing, the exception is thrown. Default True.
 
         Returns
         -------
         df: pd.DataFrame
             Dataframe with query result
         """
         url = self._get_closest_data_featurelist_path.format(
             project_id=self.project_id, featurelist_id=featurelist_id
         )
+        build_index_func = functools.partial(
+            self.build_index_for_featurelist, featurelist_id, max_wait
+        )
         data_matching_query = self._execute_data_matching_query(
             url=self.get_query_url(url, number_of_data),
             query_file_path=query_file_path,
             max_wait=max_wait,
+            build_index_func=build_index_func if build_index_if_missing else None,
         )
         df = data_matching_query.get_result()
         return df
 
     def build_index(self, max_wait: int = DEFAULT_MAX_WAIT) -> None:
         """Builds data matching index and waits for its completion.
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/documentai/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 FeaturesWithSamples = namedtuple(
     "FeaturesWithSamples", ["model_id", "feature_name", "document_task"]
 )
 
 
 if TYPE_CHECKING:
-    from PIL import Image
+    from PIL.Image import Image
     from mypy_extensions import TypedDict
 
     class PredictionType(TypedDict):
         values: Union[float, List[float]]
         labels: NotRequired[List[str]]
 
     class TextLine(TypedDict):
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/client.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -43,14 +43,15 @@
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
+    use_case: Optional[str] = None,
 ) -> RESTClientObject:
     """Return a new `RESTClientObject` with optional configuration.
     Missing configuration will be read from environment variables or a config
     file.
 
     .. note::
         This function is intended for use with the ``client_configuration``
@@ -78,25 +79,28 @@
         Could be set to path with certificates of trusted certification authorities
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools
+    use_case: str, optional
+        The entity ID of the default Use Case to use with any requests made by this Client instance.
     """
     env_config = _get_config_file_from_env()
     if token and endpoint:
         drconfig = DataRobotClientConfig(
             endpoint=endpoint,
             token=token,
             connect_timeout=connect_timeout,
             user_agent_suffix=user_agent_suffix,
             ssl_verify=ssl_verify,
             max_retries=max_retries,
             token_type=token_type,
+            use_case=use_case,
         )
     elif config_path:
         if not _file_exists(config_path):
             raise ValueError(f"Invalid config path - no file at {config_path}")
         drconfig = _config_from_file(config_path)
     elif env_config:
         if not _file_exists(env_config):
@@ -127,14 +131,15 @@
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
+    use_case: Optional[str] = None,
 ) -> RESTClientObject:
     """
     Configures the global API client for the Python SDK with optional
     configuration. Missing configuration will be read from env
     or config file.
 
     Parameters
@@ -158,28 +163,30 @@
         Could be set to path with certificates of trusted certification authorities.
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools.
-
+    use_case: str, optional
+        The entity ID of the default Use Case to use with any requests made by this Client instance.
     Returns
     -------
         The ``RESTClientObject`` instance created.
     """
     new_client = _create_client(
         token,
         endpoint,
         config_path,
         connect_timeout,
         user_agent_suffix,
         ssl_verify,
         max_retries,
         token_type,
+        use_case,
     )
 
     set_client(new_client)
 
     return new_client
 
 
@@ -378,44 +385,50 @@
     """
     Create and return a DataRobotClientConfig from environment variables.
 
     There are two ways this can be used:
     1. Use the environment variable DATAROBOT_CONFIG_FILE to specify the path to a yaml config
        file specifying the configuration to use
     2. Use both the environment variables DATAROBOT_ENDPOINT and DATAROBOT_API_TOKEN to specify
-       the connection parameters. Note that this method only allows for configuration of endpoint,
-       token and user_agent_suffix; any more advanced configuration must be done through a yaml
+       the connection parameters. This method only allows for configuration of endpoint, token,
+       user_agent_suffix, and max retries. More advanced configuration must be done through a yaml
        file
 
     Returns
     -------
     config : DataRobotClientConfig
 
     Raises
     ------
     ValueError
         If either of DATAROBOT_ENDPOINT or DATAROBOT_API_TOKEN is not specified as an environment
         variable
     IOError
         If the config file that DATAROBOT_CONFIG_FILE points to does not exist
     """
-    endpoint = os.environ.get("DATAROBOT_ENDPOINT")
-    token = os.environ.get("DATAROBOT_API_TOKEN")
-    user_agent_suffix = os.environ.get("DATAROBOT_USER_AGENT_SUFFIX")
+    endpoint: Optional[str] = os.environ.get("DATAROBOT_ENDPOINT")
+    token: Optional[str] = os.environ.get("DATAROBOT_API_TOKEN")
+    user_agent_suffix: Optional[str] = os.environ.get("DATAROBOT_USER_AGENT_SUFFIX")
     max_retries: Optional[Union[str, int]] = os.environ.get("DATAROBOT_MAX_RETRIES")
     if max_retries is not None:
         max_retries = int(max_retries)
+    use_case_id: Optional[str] = os.environ.get("DATAROBOT_DEFAULT_USE_CASE")
+
     if endpoint is None or token is None:
         e_msg = (
             "Incomplete DataRobot configuration specified in environment variables; both "
             "DATAROBOT_ENDPOINT and DATAROBOT_API_TOKEN must be specified"
         )
         raise ValueError(e_msg)
     return DataRobotClientConfig(
-        endpoint=endpoint, token=token, user_agent_suffix=user_agent_suffix, max_retries=max_retries
+        endpoint=endpoint,
+        token=token,
+        user_agent_suffix=user_agent_suffix,
+        max_retries=max_retries,
+        use_case=use_case_id,
     )
 
 
 def _config_from_file(config_path: str) -> DataRobotClientConfig:
     """
     Create and return a DataRobotClientConfig from a config path. The file must be
     a yaml formatted file
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/enums.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     REGRESSION = "Regression"
     UNSTRUCTURED = "Unstructured"
     ANOMALY = "Anomaly"
     ALL = [BINARY, MULTICLASS, MULTILABEL, REGRESSION, UNSTRUCTURED, ANOMALY]
 
 
 JOB_TYPE = enum(
+    BATCH_MONITORING="batchMonitoring",
     BATCH_PREDICTIONS="batchPredictions",
     BATCH_PREDICTION_JOB_DEFINITIONS="batchPredictionJobDefinitions",
     FEATURE_IMPACT="featureImpact",
     FEATURE_EFFECTS="featureEffects",
     FEATURE_FIT="featureFit",
     MODEL="model",
     MODEL_EXPORT="modelExport",
@@ -304,22 +305,24 @@
     MULTISERIES_VALUE="multiseriesValue",
     ROW_COUNT="rowCount",
     VALIDATION_SCORE="validationScore",
     BACKTESTING_SCORE="backtestingScore",
     HOLDOUT_SCORE="holdoutScore",
 )
 
-SHARING_ROLE = enum(
-    OWNER="OWNER",
-    READ_WRITE="READ_WRITE",
-    USER="USER",
-    EDITOR="EDITOR",
-    READ_ONLY="READ_ONLY",
-    CONSUMER="CONSUMER",
-)
+
+class SHARING_ROLE(str, Enum):
+    OWNER = ("OWNER",)
+    READ_WRITE = ("READ_WRITE",)
+    USER = ("USER",)
+    EDITOR = ("EDITOR",)
+    READ_ONLY = ("READ_ONLY",)
+    CONSUMER = ("CONSUMER",)
+    NO_ROLE = "NO_ROLE"
+
 
 MODEL_REPLACEMENT_REASON = enum(
     ACCURACY="ACCURACY",
     DATA_DRIFT="DATA_DRIFT",
     ERRORS="ERRORS",
     SCHEDULED_REFRESH="SCHEDULED_REFRESH",
     SCORING_SPEED="SCORING_SPEED",
@@ -344,14 +347,23 @@
     SPEARMAN = "spearman"
     PEARSON = "pearson"
     TAU = "tau"
 
     ALL = [MUTUAL_INFO, CRAMER, SPEARMAN, PEARSON, TAU]
 
 
+class BUCKET_SIZE:
+    PT1H = "PT1H"
+    P1D = "P1D"
+    P7D = "P7D"
+    P1M = "P1M"
+
+    ALL = [PT1H, P1D, P7D, P1M]
+
+
 class SERVICE_STAT_METRIC:  # pylint: disable=missing-class-docstring
     TOTAL_PREDICTIONS = "totalPredictions"
     TOTAL_REQUESTS = "totalRequests"
     SLOW_REQUESTS = "slowRequests"
     EXECUTION_TIME = "executionTime"
     RESPONSE_TIME = "responseTime"
     USER_ERROR_RATE = "userErrorRate"
@@ -862,7 +874,31 @@
     USER = "user"
     CUSTOM = "custom"
 
 
 class ComplianceDocTemplateType(str, Enum):
     NORMAL = "normal"
     TIME_SERIES = "time_series"
+
+
+class UseCaseEntities(str, Enum):
+    PROJECT = "project"
+    DATASET = "dataset"
+    NOTEBOOK = "notebook"
+    APPLICATION = "application"
+    RECIPE = "recipe"
+
+
+class NotebookPermissions(str, Enum):
+    CAN_READ = "CAN_READ"
+    CAN_UPDATE = "CAN_UPDATE"
+    CAN_DELETE = "CAN_DELETE"
+    CAN_SHARE = "CAN_SHARE"
+    CAN_COPY = "CAN_COPY"
+    CAN_EXECUTE = "CAN_EXECUTE"
+
+
+class ApplicationPermissions(str, Enum):
+    CAN_DELETE = "CAN_DELETE"
+    CAN_SHARE = "CAN_SHARE"
+    CAN_UPDATE = "CAN_UPDATE"
+    CAN_VIEW = "CAN_VIEW"
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/errors.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/__init__.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/deployment_monitoring.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/deployment_monitoring.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/helpers/partitioning_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 import abc
 from datetime import datetime
-from typing import Any, cast, Dict, List, Optional, TYPE_CHECKING
+from typing import Any, cast, Dict, List, NoReturn, Optional, TYPE_CHECKING
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.client import get_client, staticproperty
 from datarobot.enums import (
@@ -47,14 +47,15 @@
     "GroupCV",
     "UserCV",
     "RandomTVH",
     "UserTVH",
     "StratifiedTVH",
     "GroupTVH",
     "DatetimePartitioning",
+    "DatetimePartitioningId",
     "DatetimePartitioningSpecification",
     "BacktestSpecification",
     "FeatureSettings",
     "Periodicity",
 )
 
 if TYPE_CHECKING:
@@ -2051,10 +2052,161 @@
             "end_date": {
                 "available_training": self.available_training_end_date,
                 "primary_training": self.primary_training_end_date,
                 "gap": self.gap_end_date,
                 "holdout": self.holdout_end_date,
             },
         }
-        display_df = pd.DataFrame.from_dict(display_dict)
-        final_df = display_df.append([bt.to_dataframe() for bt in self.backtests])
+        display_df_list = [pd.DataFrame.from_dict(display_dict)]
+        display_df_list.extend([bt.to_dataframe() for bt in self.backtests])
+        final_df = pd.concat(display_df_list)
         return final_df
+
+    @classmethod
+    def datetime_partitioning_log_retrieve(
+        cls, project_id: str, datetime_partitioning_id: str
+    ) -> Any:
+        """Retrieve the datetime partitioning log content for an optimized datetime partitioning.
+
+        The datetime partitioning log provides details about the partitioning process for an OTV
+        or time series project.
+
+        Parameters
+        ----------
+        project_id : str
+            The project ID of the project associated with the datetime partitioning.
+        datetime_partitioning_id : str
+            id of the optimized datetime partitioning
+        """
+        url = (
+            f"projects/{project_id}/optimizedDatetimePartitionings/{datetime_partitioning_id}/"
+            "datetimePartitioningLog/file/"
+        )
+        response = cls._client.get(url)
+        return response.text
+
+    @classmethod
+    def datetime_partitioning_log_list(
+        cls,
+        project_id: str,
+        datetime_partitioning_id: str,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> Any:
+        """Retrieve the datetime partitioning log content and log length for an optimized
+        datetime partitioning.
+
+        The Datetime Partitioning Log provides details about the partitioning process for an OTV
+        or Time Series project.
+
+        Parameters
+        ----------
+        project_id : str
+            project id of the project associated with the datetime partitioning.
+        datetime_partitioning_id : str
+            id of the optimized datetime partitioning
+        offset : int or None
+            optional, defaults is 0, this many results will be skipped.
+        limit : int or None
+            optional, defaults to 100, at most this many results are returned. To specify
+            no limit, use 0. The default may change without notice.
+        """
+        url = (
+            f"projects/{project_id}/optimizedDatetimePartitionings/{datetime_partitioning_id}/"
+            "datetimePartitioningLog/"
+        )
+        response = cls._client.get(url, params=dict(offset=offset, limit=limit))
+        return response.json()
+
+    @classmethod
+    def get_input_data(
+        cls, project_id: str, datetime_partitioning_id: str
+    ) -> DatetimePartitioningSpecification:
+        """Retrieve the input used to create an optimized DatetimePartitioning from a project for
+        the specified datetime_partitioning_id. A datetime_partitioning_id is created by using the
+        :meth:`generate_optimized<datarobot.DatetimePartitioning.generate_optimized>` function.
+
+        Parameters
+        ----------
+        project_id : str
+            The ID of the project to retrieve partitioning for.
+        datetime_partitioning_id : ObjectId
+            The ObjectId associated with the project to retrieve from Mongo.
+
+        Returns
+        -------
+        DatetimePartitioningInput : The input to optimized datetime partitioning.
+        """
+        url = "projects/{}/optimizedDatetimePartitionings/{}/datetimePartitioningInput/".format(
+            project_id, datetime_partitioning_id
+        )
+        response = cls._client.get(url)
+        return DatetimePartitioningSpecification.from_server_data(
+            # type: ignore[no-untyped-call, no-any-return]
+            response.json()
+        )
+
+
+class DatetimePartitioningId(PartitioningMethod):
+    """Defines a DatetimePartitioningId used for datetime partitioning.
+
+    This class only includes the datetime_partitioning_id that identifies a previously
+    optimized datetime partitioning and the project_id for the associated project.
+
+    This is the specification that should be passed to :meth:`Project.analyze_and_model
+    <datarobot.models.Project.analyze_and_model>` via the ``partitioning_method`` parameter. To see
+    the full partitioning use :meth:`DatetimePartitioning.get_optimized
+    <datarobot.DatetimePartitioning.get_optimized>`.
+
+    Attributes
+    ----------
+    datetime_partitioning_id : str
+        The ID of the datetime partitioning to use.
+    project_id : str
+        The ID of the project that the datetime partitioning is associated with.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("datetime_partitioning_id"): String(),
+            t.Key("project_id"): String(),
+        }
+    ).ignore_extra("*")
+
+    def __init__(self, datetime_partitioning_id: str, project_id: str):
+        self.datetime_partitioning_id = datetime_partitioning_id
+        self.project_id = project_id
+
+    def _keys_with_defaults(self) -> List[str]:
+        """These keys have default values in the API so they will always be present when starting
+        a project. Make sure these values are set if they are present in the datetime
+        partitioning input."""
+        return [
+            "unsupervised_mode",
+            "treat_as_exponential",
+            "autopilot_data_selection_method",
+            "use_supervised_feature_reduction",
+            "use_time_series",
+            "disable_holdout",
+            "model_splits",
+        ]
+
+    def collect_payload(self) -> Dict[str, Any]:
+        payload = {
+            "datetime_partitioning_id": self.datetime_partitioning_id,
+            "cv_method": CV_METHOD.DATETIME,
+        }
+        datetime_partitioning_input = DatetimePartitioning.get_input_data(
+            self.project_id, self.datetime_partitioning_id
+        )
+        input_payload = datetime_partitioning_input.collect_payload()
+        for key in self._keys_with_defaults():
+            if key in input_payload and input_payload[key] is not None:
+                payload[key] = input_payload[key]
+
+        return payload
+
+    def prep_payload(self, project_id: str, max_wait: int = DEFAULT_MAX_WAIT) -> None:
+        pass
+
+    def update(self, **kwargs: Any) -> NoReturn:
+        raise InvalidUsageError
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/__init__.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
-from .accuracy import Accuracy, AccuracyOverTime
+from .application import Application
 from .automated_documentation import AutomatedDocument
+from .batch_monitoring_job import BatchMonitoringJob, BatchMonitoringJobDefinition
 from .batch_prediction_job import BatchPredictionJob, BatchPredictionJobDefinition
 from .blueprint import Blueprint, BlueprintChart, BlueprintTaskDocument, ModelBlueprintChart
 from .calendar_file import CalendarFile
 from .change_request import ChangeRequest, ChangeRequestReview
 from .cluster import Cluster
 from .cluster_insight import ClusterInsight
 from .compliance_doc_template import ComplianceDocTemplate
@@ -17,15 +18,14 @@
 from .custom_model_version import (
     CustomModelVersion,
     CustomModelVersionConversion,
     CustomModelVersionDependencyBuild,
 )
 from .custom_task import CustomTask
 from .custom_task_version import CustomTaskVersion
-from .data_drift import FeatureDrift, TargetDrift
 from .data_engine_query_generator import DataEngineQueryGenerator
 from .data_source import DataSource, DataSourceParameters
 from .data_store import DataStore
 from .dataset import Dataset, DatasetDetails
 from .deployment import Deployment
 from .driver import DataDriver
 from .execution_environment import ExecutionEnvironment
@@ -78,14 +78,15 @@
     FrozenModel,
     Model,
     ModelParameters,
     PrimeModel,
     RatingTableModel,
 )
 from .modeljob import ModelJob
+from .notebooks import Notebook
 from .pairwise_statistics import (
     PairwiseConditionalProbabilities,
     PairwiseCorrelations,
     PairwiseJointProbabilities,
 )
 from .payoff_matrix import PayoffMatrix
 from .predict_job import PredictJob
@@ -102,14 +103,22 @@
 from .project import Project
 from .rating_table import RatingTable
 from .recommended_model import ModelRecommendation
 from .relationships_configuration import RelationshipsConfiguration
 from .ruleset import Ruleset
 from .secondary_dataset import SecondaryDatasetConfigurations
 from .segmentation import SegmentationTask, SegmentInfo
-from .service_stats import ServiceStats, ServiceStatsOverTime
 from .shap_impact import ShapImpact
 from .shap_matrix import ShapMatrix
 from .shap_matrix_job import ShapMatrixJob
 from .sharing import SharingAccess
 from .training_predictions import TrainingPredictions
+from .types import (
+    AnomalyAssessmentDataPoint,
+    AnomalyAssessmentPreviewBin,
+    AnomalyAssessmentRecordMetadata,
+    RegionExplanationsData,
+    RocCurveEstimatedMetric,
+    ShapleyFeatureContribution,
+)
+from .use_cases import UseCase, UseCaseUser
 from .user_blueprints import UserBlueprint
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/accuracy.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 from typing import Dict, List, Optional, TYPE_CHECKING
 
 import dateutil
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
+from datarobot.enums import ACCURACY_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-
-from ..enums import ACCURACY_METRIC
-from ..helpers.deployment_monitoring import DeploymentQueryBuilderMixin
-from ..utils import from_api
+from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
         end: datetime
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/anomaly_assessment.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,25 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from operator import itemgetter
 from typing import Any, cast, Dict, Iterable, List, Optional, Union
 
 import trafaret as t
-from typing_extensions import Literal, TypedDict, Unpack
+from typing_extensions import Literal, Unpack
 
 from datarobot._compat import Int, String
 from datarobot.enums import AnomalyAssessmentStatus, DATA_SUBSET, SOURCE_TYPE
 from datarobot.models.api_object import APIObject
+from datarobot.models.types import (
+    AnomalyAssessmentDataPoint,
+    AnomalyAssessmentPreviewBin,
+    AnomalyAssessmentRecordMetadata,
+    RegionExplanationsData,
+)
 from datarobot.utils import from_api
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 DEFAULT_BATCH_SIZE = 1000
 
 RecordMetadataTrafaret = t.Dict(
@@ -34,50 +40,16 @@
         t.Key("backtest"): t.Or(String(), Int),
         t.Key("source"): t.Enum(*SOURCE_TYPE.ALL),  # type: ignore[attr-defined]
         t.Key("series_id"): t.Or(String(), t.Null),
     }
 )
 
 
-class RecordMetadata(TypedDict):
-    record_id: str
-    project_id: str
-    model_id: str
-    backtest: Union[str, int]
-    source: SOURCE_TYPE
-    series_id: Optional[str]
-
-
-class PreviewBin(TypedDict):
-    avg_predicted: Optional[float]
-    max_predicted: Optional[float]
-    start_date: str
-    end_date: str
-    frequency: int
-
-
-class RegionExplanationsData(TypedDict):
-    explanations: List[DataPoint]
-    shap_base_value: Optional[float]
-
-
-class ShapleyFeatureContribution(TypedDict):
-    feature_value: str
-    strength: float
-    feature: str
-
-
-class DataPoint(TypedDict):
-    shap_explanation: Optional[List[ShapleyFeatureContribution]]
-    timestamp: str
-    prediction: float
-
-
 class BaseAPIObject(APIObject):  # pylint: disable=missing-class-docstring
-    def __init__(self, **record_kwargs: Unpack[RecordMetadata]) -> None:
+    def __init__(self, **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata]) -> None:
         self.record_id: str = record_kwargs["record_id"]
         self.project_id: str = record_kwargs["project_id"]
         self.model_id: str = record_kwargs["model_id"]
         self.backtest: Union[str, int] = record_kwargs["backtest"]
         self.source: Union[
             Literal[SOURCE_TYPE.TRAINING], Literal[SOURCE_TYPE.VALIDATION]
         ] = record_kwargs["source"]
@@ -218,15 +190,15 @@
         status_details: str,
         start_date: Optional[str],
         end_date: Optional[str],
         prediction_threshold: Optional[float],
         preview_location: Optional[str],
         delete_location: str,
         latest_explanations_location: Optional[str],
-        **record_kwargs: Unpack[RecordMetadata],
+        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
     ) -> None:
         self.status = status
         self.status_details = status_details
         self.start_date = start_date
         self.end_date = end_date
         self.prediction_threshold = prediction_threshold
         self.preview_location = preview_location
@@ -406,15 +378,15 @@
             self.record_id,
             start_date=start_date,
             end_date=end_date,
             points_count=points_count,
         )
 
     def get_explanations_data_in_regions(
-        self, regions: List[PreviewBin], prediction_threshold: float = 0.0
+        self, regions: List[AnomalyAssessmentPreviewBin], prediction_threshold: float = 0.0
     ) -> RegionExplanationsData:
         """Get predictions along with explanations for the specified regions, sorted by
         predictions in descending order.
 
         Parameters
         ----------
         regions: list of preview_bins
@@ -423,15 +395,15 @@
             If specified, only points with score greater or equal to the threshold will be returned.
 
         Returns
         -------
         dict in a form of {'explanations': explanations, 'shap_base_value': shap_base_value}
 
         """
-        explanations: List[DataPoint] = []
+        explanations: List[AnomalyAssessmentDataPoint] = []
         shap_base_value: Optional[float] = None
         for region in regions:
             response = self.get_explanations(
                 start_date=region["start_date"], end_date=region["end_date"]
             )
             shap_base_value = response.shap_base_value
             for item in response.data:
@@ -526,16 +498,16 @@
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         start_date: str,
         end_date: str,
-        preview_bins: List[PreviewBin],
-        **record_kwargs: Unpack[RecordMetadata],
+        preview_bins: List[AnomalyAssessmentPreviewBin],
+        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
     ) -> None:
         self.preview_bins = preview_bins
         self.start_date = start_date
         self.end_date = end_date
         super().__init__(**record_kwargs)
 
     @classmethod
@@ -554,15 +526,17 @@
         AnomalyAssessmentPredictionsPreview
 
         """
         url = cls._path.format(project_id=project_id, record_id=record_id)
         r_data = cls._client.get(url).json()
         return cast("AnomalyAssessmentPredictionsPreview", cls.from_server_data(r_data))
 
-    def find_anomalous_regions(self, max_prediction_threshold: float = 0.0) -> List[PreviewBin]:
+    def find_anomalous_regions(
+        self, max_prediction_threshold: float = 0.0
+    ) -> List[AnomalyAssessmentPreviewBin]:
         """Sort preview bins by max_predicted value and select those with max predicted value
          greater or equal to max prediction threshold.
          Sort the result by max predicted value in descending order.
 
         Parameters
         ----------
         max_prediction_threshold: float, optional
@@ -679,19 +653,19 @@
         .merge(RecordMetadataTrafaret)
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         shap_base_value: float,
-        data: List[DataPoint],
+        data: List[AnomalyAssessmentDataPoint],
         start_date: Optional[str],
         end_date: Optional[str],
         count: int,
-        **record_kwargs: Unpack[RecordMetadata],
+        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
     ) -> None:
         self.shap_base_value = shap_base_value
         self.data = data
         self.count = count
         self.start_date = start_date
         self.end_date = end_date
         super().__init__(**record_kwargs)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/api_object.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/automated_documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
 from typing import cast, List, Optional, Tuple
 
-from requests.models import Response
+from requests import Response
 import trafaret as t
 from typing_extensions import TypedDict
 
 from datarobot._compat import String
 from datarobot.enums import DEFAULT_MAX_WAIT, DocumentType, Locales
 from datarobot.models.api_object import APIObject
 from datarobot.utils import camelize, from_api, get_id_from_location, parse_time
@@ -180,15 +180,15 @@
         """Request generation of an automated document.
 
         Required attributes to request document generation: ``document_type``, ``entity_id``,
         and ``output_format``.
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
 
         Examples
         --------
         .. code-block:: python
 
             import datarobot as dr
 
@@ -227,15 +227,15 @@
     def download(self) -> Response:
         """
         Download a generated Automated Document.
         Document ID is required to download a file.
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
 
         Examples
         --------
 
         Generating and downloading the generated document:
 
         .. code-block:: python
@@ -299,15 +299,15 @@
 
     def delete(self) -> Response:
         """
         Delete a document using its ID.
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
 
         Examples
         --------
 
         .. code-block:: python
 
             import datarobot as dr
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/blueprint.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/calendar_file.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/change_request.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/connector.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/credential.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_model_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
+import contextlib
 import copy
 import json
 import os
 
-import contextlib2
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
 from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
@@ -684,36 +684,32 @@
         network_egress_policy=None,
         maximum_memory=None,
         replicas=None,
         required_metadata_values=None,
     ):
         url = cls._path.format(custom_model_id)
 
-        with contextlib2.ExitStack() as stack:
+        with contextlib.ExitStack() as stack:
             upload_data = [
                 ("isMajorUpdate", str(is_major_update)),
                 ("baseEnvironmentId", base_environment_id),
             ]
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
                     for path in file_paths:
                         file_path = os.path.join(root_path, path)
-                        file = stack.enter_context(
-                            open(file_path, "rb")  # pylint: disable=consider-using-with
-                        )
+                        file = stack.enter_context(open(file_path, "rb"))
 
                         upload_data.append(("file", (os.path.basename(file_path), file)))
                         upload_data.append(("filePath", os.path.relpath(file_path, folder_path)))
 
             if files:
                 for file_path, upload_file_path in files:
-                    file = stack.enter_context(
-                        open(file_path, "rb")  # pylint: disable=consider-using-with
-                    )
+                    file = stack.enter_context(open(file_path, "rb"))
 
                     upload_data.append(("file", (os.path.basename(upload_file_path), file)))
                     upload_data.append(("filePath", upload_file_path))
 
             if extra_upload_data:
                 upload_data += extra_upload_data
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
+import contextlib
 import json
 import os
 
-import contextlib2
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import (
     CustomDependency,
@@ -352,22 +352,20 @@
             )
 
         if maximum_memory:
             upload_data.append(("maximumMemory", str(maximum_memory)))
 
         cls._verify_folder_path(folder_path)
 
-        with contextlib2.ExitStack() as stack:
+        with contextlib.ExitStack() as stack:
             if folder_path:
                 for dir_name, _, file_names in os.walk(folder_path):
                     for file_name in file_names:
                         file_path = os.path.join(dir_name, file_name)
-                        file = stack.enter_context(
-                            open(file_path, "rb")  # pylint: disable=consider-using-with
-                        )
+                        file = stack.enter_context(open(file_path, "rb"))
 
                         upload_data.append(("file", (os.path.basename(file_path), file)))
                         upload_data.append(("filePath", os.path.relpath(file_path, folder_path)))
 
             encoder = MultipartEncoder(fields=upload_data)
             headers = {"Content-Type": encoder.content_type}
             response = cls._client.request(method, url, data=encoder, headers=headers)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_source.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_store.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/dataset.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,14 +581,15 @@
 
     @classmethod
     def list(
         cls: Type[TDataset],
         category: Optional[str] = None,
         filter_failed: Optional[bool] = None,
         order_by: Optional[str] = None,
+        use_case_ids: Optional[Union[str, List[str]]] = None,
     ) -> List[TDataset]:
         """
         List all datasets a user can view.
 
 
         Parameters
         ----------
@@ -603,31 +604,40 @@
             If True invalid datasets will be excluded.
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
-
+        use_case_ids: string or List[string], optional
+            Filter available datasets by a specific Use Case ID or IDs.
         Returns
         -------
         list[Dataset]
             a list of datasets the user can view
 
         """
-        return list(cls.iterate(category=category, order_by=order_by, filter_failed=filter_failed))
+        return list(
+            cls.iterate(
+                category=category,
+                order_by=order_by,
+                filter_failed=filter_failed,
+                use_case_ids=use_case_ids,
+            )
+        )
 
     @classmethod
     def iterate(
         cls: Type[TDataset],
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         category: Optional[str] = None,
         order_by: Optional[str] = None,
         filter_failed: Optional[bool] = None,
+        use_case_ids: Optional[Union[str, List[str]]] = None,
     ) -> Generator[TDataset, None, None]:
         """
         Get an iterator for the requested datasets a user can view.
         This lazily retrieves results. It does not get the next page from the server until the
         current page is exhausted.
 
         Parameters
@@ -651,26 +661,29 @@
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
 
+        use_case_ids: string or List[string], optional
+            Filter available datasets by a specific Use Case ID or IDs.
         Yields
         ------
         Dataset
             An iterator of the datasets the user can view
 
         """
         all_params = {
             "offset": offset,
             "limit": limit,
             "category": category,
             "order_by": order_by,
             "filter_failed": filter_failed,
+            "experiment_container_ids": use_case_ids,
         }
         params = _remove_empty_params(all_params)
         _update_filter_failed(params)
 
         for dataset_json in unpaginate(cls._path, params, cls._client):
             yield cls.from_server_data(dataset_json)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/deployment.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,39 @@
 
 import dateutil
 import pandas as pd
 import pytz
 import trafaret as t
 
 from datarobot._compat import String
-from datarobot.enums import ACCURACY_METRIC, DEFAULT_MAX_WAIT, FileLocationType, LocalSourceType
+from datarobot.enums import (
+    ACCURACY_METRIC,
+    BUCKET_SIZE,
+    DEFAULT_MAX_WAIT,
+    FileLocationType,
+    LocalSourceType,
+)
 from datarobot.errors import InvalidUsageError
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
 from datarobot.models.custom_model_version import CustomModelVersion
+from datarobot.models.deployment.accuracy import Accuracy, AccuracyOverTime
+from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
+from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
+from datarobot.models.deployment.sharing import (
+    DeploymentGrantSharedRoleWithId,
+    DeploymentGrantSharedRoleWithUsername,
+    DeploymentSharedRole,
+)
 from datarobot.utils import deprecated, from_api, get_id_from_location
+from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
-
-from ..helpers.deployment_monitoring import DeploymentQueryBuilderMixin
-from ..utils.pagination import unpaginate
-from ..utils.waiters import wait_for_async_resolution
-from .accuracy import Accuracy, AccuracyOverTime
-from .data_drift import FeatureDrift, TargetDrift
-from .service_stats import ServiceStats, ServiceStatsOverTime
+from datarobot.utils.waiters import wait_for_async_resolution
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     from datarobot.models.batch_prediction_job import IntakeSettings
 
     class FeatureDict(TypedDict):
@@ -116,14 +126,25 @@
         was_acted_on: Optional[bool]
         timestamp: Union[datetime, str]
 
 
 TDeployment = TypeVar("TDeployment", bound="Deployment")
 
 
+def _check(trafaret: t, value: Any, default_to_null: bool = True) -> Any:
+    if default_to_null and value is None:
+        return None
+
+    # Allow users to pass a single value even if a list of values is expected.
+    if isinstance(trafaret, t.List) and not isinstance(value, list):
+        value = [value]
+
+    return trafaret.check(value)
+
+
 class Deployment(APIObject, DeploymentQueryBuilderMixin, BrowserMixin):
     """A deployment created from a DataRobot model.
 
     Attributes
     ----------
     id : str
         the id of the deployment
@@ -1570,15 +1591,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         execution_time_quantile: Optional[float] = None,
         response_time_quantile: Optional[float] = None,
         slow_requests_threshold: Optional[float] = None,
     ) -> ServiceStats:
-        """Retrieve value of service stat metrics over a certain time period.
+        """Retrieves values of many service stat metrics aggregated over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         model_id : str, optional
             the id of the model
@@ -1618,15 +1639,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[str] = None,
         quantile: Optional[float] = None,
         threshold: Optional[int] = None,
     ) -> ServiceStatsOverTime:
-        """Retrieve information about how a service stat metric changes over a certain time period.
+        """Retrieves values of a single service stat metric over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         metric : SERVICE_STAT_METRIC, optional
             the service stat metric to retrieve
@@ -1731,24 +1752,75 @@
         if not self.id:
             raise ValueError("Deployment ID is required to get feature drift.")
 
         return FeatureDrift.list(
             self.id, model_id=model_id, start_time=start_time, end_time=end_time, metric=metric
         )
 
+    def get_predictions_over_time(
+        self,
+        model_ids: Optional[List[str]] = None,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        bucket_size: Optional[BUCKET_SIZE] = None,
+        target_classes: Optional[List[str]] = None,
+    ) -> PredictionsOverTime:
+        """Retrieve stats of deployment's prediction response over a certain time period.
+
+        .. versionadded:: v3.2
+
+        Parameters
+        ----------
+        model_ids : list[str]
+            ID of models to retrieve prediction stats
+        start_time : datetime
+            start of the time period
+        end_time : datetime
+            end of the time period
+        bucket_size : BUCKET_SIZE
+            time duration of each bucket
+        target_classes : list[str]
+            class names of target, only for deployments with multiclass target
+
+        Returns
+        -------
+        predictions_over_time : PredictionsOverTime
+            the queried predictions over time information
+
+        Examples
+        --------
+        .. code-block:: python
+
+            from datarobot import Deployment
+            deployment = Deployment.get(deployment_id='5c939e08962d741e34f609f0')
+            predictions_over_time = deployment.get_predictions_over_time()
+        """
+
+        if not self.id:
+            raise ValueError("Deployment ID is required to get predictions over time.")
+
+        return PredictionsOverTime.get(
+            self.id,
+            model_ids=model_ids,
+            start_time=start_time,
+            end_time=end_time,
+            bucket_size=bucket_size,
+            target_classes=target_classes,
+        )
+
     def get_accuracy(
         self,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         start: Optional[datetime] = None,
         end: Optional[datetime] = None,
         target_classes: Optional[List[str]] = None,
     ) -> Accuracy:
-        """Retrieve values of accuracy metrics over a certain time period.
+        """Retrieves values of many accuracy metrics aggregated over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         model_id : str
             the id of the model
@@ -1785,15 +1857,15 @@
         metric: Optional[ACCURACY_METRIC] = None,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[str] = None,
         target_classes: Optional[List[str]] = None,
     ) -> AccuracyOverTime:
-        """Retrieve information about how an accuracy metric changes over a certain time period.
+        """Retrieves values of a single accuracy metric over a time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         metric : ACCURACY_METRIC
             the accuracy metric to retrieve
@@ -2169,25 +2241,14 @@
                     "DeploymentGrantSharedRoleWithUsername, DeploymentGrantSharedRoleWithId"
                 )
             roles_json.append(role if isinstance(role, dict) else role.to_dict())
 
         self._client.patch(path, data=dict(operation="updateRoles", roles=roles_json))
 
 
-def _check(trafaret: t, value: Any, default_to_null: bool = True) -> Any:
-    if default_to_null and value is None:
-        return None
-
-    # Allow users to pass a single value even if a list of values is expected.
-    if isinstance(trafaret, t.List) and not isinstance(value, list):
-        value = [value]
-
-    return trafaret.check(value)
-
-
 class DeploymentListFilters:  # pylint: disable=missing-class-docstring
     def __init__(
         self,
         role: Optional[str] = None,
         service_health: Optional[List[str]] = None,
         model_health: Optional[List[str]] = None,
         accuracy_health: Optional[List[str]] = None,
@@ -2314,113 +2375,7 @@
     @staticmethod
     def _list_to_comma_separated_string(input_list: List[str]) -> str:
         output_string = ""
         for list_item in input_list:
             output_string += f"{list_item},"
         output_string = output_string[:-1]
         return output_string
-
-
-DeploymentSharedRolesResponseValidator_ = t.Dict(
-    {
-        t.Key("share_recipient_type"): t.Enum("user", "group", "organization"),
-        t.Key("role"): t.Enum("CONSUMER", "USER", "OWNER"),
-        t.Key("id"): String(allow_blank=False, min_length=24, max_length=24),
-        t.Key("name"): String(allow_blank=False),
-    }
-)
-
-
-class DeploymentSharedRole(APIObject):
-    """
-    Parameters
-    ----------
-    share_recipient_type: enum('user', 'group', 'organization')
-        Describes the recipient type, either user, group, or organization.
-    role: str, one of enum('CONSUMER', 'USER', 'OWNER')
-        The role of the org/group/user on this deployment.
-    id: str
-        The ID of the recipient organization, group or user.
-    name: string
-        The name of the recipient organization, group or user.
-    """
-
-    _converter = DeploymentSharedRolesResponseValidator_
-
-    def __init__(
-        self, id: str, name: str, role: str, share_recipient_type: str, **kwargs: Any
-    ) -> None:
-        self.share_recipient_type = share_recipient_type
-        self.role = role
-        self.id = id
-        self.name = name
-
-    def to_dict(self) -> Dict[str, str]:
-        return {
-            "role": self.role,
-            "id": self.id,
-            "share_recipient_type": self.share_recipient_type,
-            "name": self.name,
-        }
-
-
-class DeploymentGrantSharedRoleWithId:
-    """
-
-    Parameters
-    ----------
-    share_recipient_type: enum('user', 'group', 'organization')
-        Describes the recipient type, either user, group, or organization.
-    role: enum('OWNER', 'USER', 'OBSERVER', 'NO_ROLE')
-        The role of the recipient on this entity. One of OWNER, USER, OBSERVER, NO_ROLE.
-        If NO_ROLE is specified, any existing role for the recipient will be removed.
-    id: str
-        The ID of the recipient.
-    """
-
-    def __init__(
-        self,
-        id: str,
-        role: str,
-        share_recipient_type: str = "user",
-        **kwargs: Any,
-    ) -> None:
-        self.share_recipient_type = share_recipient_type
-        self.role = role
-        self.id = id
-
-    def to_dict(self) -> Dict[str, str]:
-        return {
-            "role": self.role,
-            "id": self.id,
-            "share_recipient_type": self.share_recipient_type,
-        }
-
-
-class DeploymentGrantSharedRoleWithUsername:
-    """
-
-    Parameters
-    ----------
-    role: string
-        The role of the recipient on this entity. One of OWNER, USER, CONSUMER, NO_ROLE.
-        If NO_ROLE is specified, any existing role for the user will be removed.
-    username: string
-        Username of the user to update the access role for.
-    """
-
-    def __init__(
-        self,
-        role: str,
-        username: str,
-        **kwargs: Any,
-    ) -> None:
-        self.share_recipient_type = "user"
-        self.role = role
-        self.username = username
-
-    def to_dict(self) -> Dict[str, str]:
-        return {
-            "role": self.role,
-            "username": self.username,
-            "share_recipient_type": self.share_recipient_type,
-        }
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/driver.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from datarobot.models.roc_curve import RocCurveThresholdMixin, RocPointsTrafaret
 from datarobot.utils.pagination import unpaginate
 
 from ..api_object import APIObject
 from .external_scores import DEFAULT_BATCH_SIZE
 
 if TYPE_CHECKING:
-    from datarobot.models.roc_curve import EstimatedMetric
+    from datarobot.models.types import RocCurveEstimatedMetric
 
 
 class ExternalRocCurve(APIObject, RocCurveThresholdMixin):
     """ROC curve data for the model and prediction dataset with target or actual value column in
     unsupervised case.
 
     .. versionadded:: v2.21
@@ -48,15 +48,15 @@
     _path = "projects/{project_id}/models/{model_id}/datasetRocCurves/"
 
     _converter = t.Dict({t.Key("dataset_id"): String}).merge(RocPointsTrafaret).ignore_extra("*")
 
     def __init__(
         self,
         dataset_id: str,
-        roc_points: List[EstimatedMetric],
+        roc_points: List[RocCurveEstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
     ) -> None:
         self.dataset_id = dataset_id
         self.roc_points = roc_points
         self.negative_class_predictions = negative_class_predictions
         self.positive_class_predictions = positive_class_predictions
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_effect.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_fit.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/feature_fit.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/featurelist.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/imported_model.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/job.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/missing_report.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/model.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/modeljob.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pareto_front.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predict_job.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_explanations.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 import abc
 from datetime import datetime
+import json
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import TARGET_TYPE
 from datarobot.models.project_options import ProjectOptions
@@ -24,47 +25,54 @@
 
 int_float_string = t.Type(int) | t.Type(float) | String(allow_blank=True)
 
 prediction_values_trafaret = t.Dict(
     {t.Key("label", optional=True): int_float_string, t.Key("value"): t.Float}
 ).ignore_extra("*")
 
-per_ngram_text_explanations_trafaret = t.Dict(
-    {
-        t.Key("ngrams"): t.List(t.Dict({t.Key("ending_index"): Int, t.Key("starting_index"): Int})),
-        t.Key("is_unknown"): t.Bool,
-        t.Key("qualitative_strength"): String,
-        t.Key("strength"): t.Float,
-    }
+per_ngram_text_explanations_trafaret = t.Or(
+    t.List(
+        t.Dict(
+            {
+                t.Key("ngrams"): t.List(
+                    t.Dict({t.Key("ending_index"): Int, t.Key("starting_index"): Int})
+                ),
+                t.Key("is_unknown"): t.Bool,
+                t.Key("qualitative_strength"): String,
+                t.Key("strength"): t.Float,
+            }
+        )
+    ),
+    t.Null,
 )
 
 prediction_explanations_entry_trafaret = t.Dict(
     {
         t.Key("label", optional=True): int_float_string,
         t.Key("feature"): String,
         t.Key("feature_value"): int_float_string,
         t.Key("strength"): t.Float,
         t.Key("qualitative_strength"): String,
-        t.Key("per_ngram_text_explanations", optional=True): t.List(
-            per_ngram_text_explanations_trafaret
-        ),
+        t.Key("per_ngram_text_explanations", optional=True): per_ngram_text_explanations_trafaret,
     }
 ).ignore_extra("*")
 
 prediction_explanations_trafaret = t.Dict(
     {
         t.Key("row_id"): Int,
         t.Key("prediction"): int_float_string,
         t.Key("adjusted_prediction", optional=True): int_float_string,
         t.Key("prediction_values"): t.List(prediction_values_trafaret),
         t.Key("adjusted_prediction_values", optional=True): t.List(prediction_values_trafaret),
         t.Key("prediction_explanations"): t.List(prediction_explanations_entry_trafaret),
     }
 ).ignore_extra("*")
 
+KEEP_ATTRS = ["data.prediction_explanations.per_ngram_text_explanations"]
+
 
 class PredictionExplanationsMode:
     """Prediction explanations mode for multiclass models"""
 
     @abc.abstractmethod
     def get_api_parameters(self, batch_route=False):
         """Get parameters passed in corresponding API call
@@ -497,25 +505,29 @@
             - explanation_0_feature_value : the value the feature took on
             - explanation_0_label : the output being driven by this explanation.  For regression
               projects, this is the name of the target feature.  For classification projects, this
               is the class label whose probability increasing would correspond to a positive
               strength.
             - explanation_0_qualitative_strength : a human-readable description of how strongly the
               feature affected the prediction (e.g. '+++', '--', '+') for this explanation
+            - explanation_0_per_ngram_text_explanations : Text prediction explanations data in json
+              formatted string.
             - explanation_0_strength : the amount this feature's value affected the prediction
             - ...
             - explanation_N_feature : the name of the feature contributing to the prediction for
               this explanation
             - explanation_N_feature_value : the value the feature took on
             - explanation_N_label : the output being driven by this explanation.  For regression
               projects, this is the name of the target feature.  For classification projects, this
               is the class label whose probability increasing would correspond to a positive
               strength.
             - explanation_N_qualitative_strength : a human-readable description of how strongly the
               feature affected the prediction (e.g. '+++', '--', '+') for this explanation
+            - explanation_N_per_ngram_text_explanations : Text prediction explanations data in json
+              formatted string.
             - explanation_N_strength : the amount this feature's value affected the prediction
 
         For classification projects, the server does not guarantee any ordering on the prediction
         values, however within this function we sort the values so that `class_X` corresponds to
         the same class from row to row.
 
         Parameters
@@ -529,14 +541,18 @@
         dataframe: pandas.DataFrame
         """
         columns = ["row_id", "prediction"]
         rows = self.get_rows(
             batch_size=1, exclude_adjusted_predictions=exclude_adjusted_predictions
         )
         first_row = next(rows)
+        has_text_explanations = (
+            first_row.prediction_explanations
+            and "per_ngram_text_explanations" in first_row.prediction_explanations[0]
+        )
         adjusted_predictions_in_data = first_row.adjusted_prediction is not None
         if adjusted_predictions_in_data:
             columns.append("adjusted_prediction")
         # for regression, length is 1; for classification, length is number of levels in target
         # i.e. 2 for binary classification
         is_classification = len(first_row.prediction_values) > 1
         # include class label/probability for classification project
@@ -552,25 +568,30 @@
                             f"{prefix}_explanation_{i}_feature",
                             f"{prefix}_explanation_{i}_feature_value",
                             f"{prefix}_explanation_{i}_label",
                             f"{prefix}_explanation_{i}_qualitative_strength",
                             f"{prefix}_explanation_{i}_strength",
                         ]
                     )
+                    if has_text_explanations:
+                        columns.append(f"{prefix}_explanation_{i}_per_ngram_text_explanations")
+
         else:
             for i in range(self.max_explanations):
                 columns.extend(
                     [
                         f"explanation_{i}_feature",
                         f"explanation_{i}_feature_value",
                         f"explanation_{i}_label",
                         f"explanation_{i}_qualitative_strength",
                         f"explanation_{i}_strength",
                     ]
                 )
+                if has_text_explanations:
+                    columns.append(f"explanation_{i}_per_ngram_text_explanations")
         pred_expl_list = []
 
         for i, row in enumerate(
             self.get_rows(exclude_adjusted_predictions=exclude_adjusted_predictions)
         ):
             data = [row.row_id, row.prediction]
             if adjusted_predictions_in_data:
@@ -597,26 +618,34 @@
                             pred_expl["feature"],
                             pred_expl["feature_value"],
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
+                    if has_text_explanations:
+                        data.append(
+                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
+                        )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
             else:
                 for pred_expl in row.prediction_explanations:
                     data.extend(
                         [
                             pred_expl["feature"],
                             pred_expl["feature_value"],
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
+                    if has_text_explanations:
+                        data.append(
+                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
+                        )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
 
         return pd.DataFrame(data=pred_expl_list, columns=columns)
 
     def download_to_csv(self, filename, encoding="utf-8", exclude_adjusted_predictions=True):
         """
         Save prediction explanations rows into CSV file.
@@ -833,8 +862,8 @@
         params = {
             "offset": offset,
             "exclude_adjusted_predictions": "true" if exclude_adjusted_predictions else "false",
         }
         if limit:
             params["limit"] = limit
         path = f"{cls._path_template.format(project_id)}{prediction_explanations_id}/"
-        return cls.from_location(path, params=params)
+        return cls.from_location(path, keep_attrs=KEEP_ATTRS, params=params)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_server.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predictions.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prime_file.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/rating_table.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/recommended_model.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/residuals.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/roc_curve.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,43 +16,26 @@
 import numpy as np
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
 
 if TYPE_CHECKING:
-    from mypy_extensions import TypedDict
-
-    class EstimatedMetric(TypedDict):
-        """Typed dict for estimated metric"""
-
-        accuracy: float
-        f1_score: float
-        false_negative_score: int
-        true_negative_score: int
-        true_negative_rate: float
-        matthews_correlation_coefficient: float
-        true_positive_score: int
-        positive_predictive_value: float
-        false_positive_score: int
-        false_positive_rate: float
-        negative_predictive_value: float
-        true_positive_rate: float
-        threshold: float
+    from datarobot.models.types import RocCurveEstimatedMetric
 
 
 class RocCurveThresholdMixin:  # pylint: disable=missing-class-docstring
-    roc_points: Optional[List[EstimatedMetric]] = None
+    roc_points: Optional[List[RocCurveEstimatedMetric]] = None
 
     @staticmethod
     def _validate_threshold(threshold: float) -> None:
         if threshold > 1 or threshold < 0:
             raise ValueError("threshold must be from [0, 1] interval")
 
-    def estimate_threshold(self, threshold: float) -> EstimatedMetric:
+    def estimate_threshold(self, threshold: float) -> RocCurveEstimatedMetric:
         """Return metrics estimation for given threshold.
 
         Parameters
         ----------
         threshold : float from [0, 1] interval
             Threshold we want estimation for
 
@@ -158,15 +141,15 @@
     """
 
     _converter = RocCurveTrafaret
 
     def __init__(
         self,
         source: str,
-        roc_points: List[EstimatedMetric],
+        roc_points: List[RocCurveEstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
         source_model_id: str,
     ) -> None:
         self.source = source
         self.roc_points = roc_points
         self.negative_class_predictions = negative_class_predictions
@@ -212,15 +195,15 @@
         .merge(RocCurveTrafaret)
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         source: str,
-        roc_points: List[EstimatedMetric],
+        roc_points: List[RocCurveEstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
         source_model_id: str,
         label: str,
         kolmogorov_smirnov_metric: float,
         auc: float,
     ) -> None:
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/ruleset.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/segmentation.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/service_stats.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_impact.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/sharing.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/sharing.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import String
+from datarobot.enums import SHARING_ROLE
 from datarobot.models.api_object import APIObject
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class SharingAccessPayload(TypedDict, total=False):
         username: str
@@ -111,7 +112,59 @@
         """
         payload: SharingAccessPayload = {"username": self.username, "role": self.role}
         if self.can_share is not None:
             payload["can_share"] = self.can_share
         if self.can_use_data is not None:
             payload["can_use_data"] = self.can_use_data
         return payload
+
+
+class SharingRole(APIObject):
+    """
+    Represents metadata about a user who has been granted access to an entity.
+
+    Attributes
+    ----------
+    id : str or None
+        The ID of the user.
+    role : str
+        Represents a particular level of access. Should be one of
+        ``datarobot.enums.SHARING_ROLE``.
+    can_share : bool
+        Indicates whether this user is permitted to share with other users. When False, the
+        user has access to the entity, but can only revoke their own access. They cannot not modify
+        any user's access role. When True, the user can share with any other user at an access
+        role up to their own.
+    share_recipient_type : str
+        The type of user for the object of the method. Can be ``user`` or ``organization``.
+    user_full_name : str or None
+        The full name of the user.
+    username : str or None
+        The username (usually the email) of the user.
+    """
+
+    _converter = t.Dict(
+        {
+            t.Key("id", optional=True): t.String,
+            t.Key("user_full_name", optional=True): t.String,
+            t.Key("name", optional=True) >> "username": t.String,
+            t.Key("role"): t.String,
+            t.Key("share_recipient_type"): t.String,
+            t.Key("can_share"): t.Bool,
+        }
+    ).ignore_extra("*")
+
+    def __init__(
+        self,
+        role: SHARING_ROLE,
+        share_recipient_type: str,
+        can_share: bool,
+        id: Optional[str] = None,
+        user_full_name: Optional[str] = None,
+        username: Optional[str] = None,
+    ):
+        self.id = id
+        self.user_full_name = user_full_name
+        self.role = SHARING_ROLE[role]
+        self.share_recipient_type = share_recipient_type
+        self.username = username
+        self.can_share = can_share
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/training_predictions.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
         """
         return cast(
             Response, cls._client.delete(cls._path.format(userBlueprintId=user_blueprint_id))
         )
 
     @classmethod
     def get_input_types(cls) -> UserBlueprintAvailableInput:
@@ -747,15 +747,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
         """
         return UserBlueprintSharingUpdateController.update_shared_roles(
             user_blueprint_id=user_blueprint_id, roles=roles
         )
 
     @classmethod
     def search_catalog(
@@ -1369,15 +1369,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        requests.models.Response
+        :class:`requests.models.Response`
         """
         roles_json = []
         for role in roles:
             if not isinstance(
                 role,
                 (dict, GrantAccessControlWithUsernameValidator, GrantAccessControlWithIdValidator),
             ):
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/validators.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/images.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/word_cloud.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/rest.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -25,14 +25,15 @@
 import trafaret as t
 from urllib3 import Retry
 
 from datarobot.mixins.browser_mixin import BrowserMixin
 
 from ._compat import Int, String
 from ._version import __version__
+from .context import _context
 from .enums import DEFAULT_TIMEOUT
 from .errors import ClientError, JobAlreadyRequested, PlatformDeprecationWarning, ServerError
 from .utils import to_api
 
 if TYPE_CHECKING:
     from io import BufferedReader, IOBase
 
@@ -407,33 +408,39 @@
             t.Key("endpoint"): String(),
             t.Key("token"): String(),
             t.Key("connect_timeout", optional=True): Int(),
             t.Key("ssl_verify", optional=True): t.Or(t.Bool(), String()),
             t.Key("user_agent_suffix", optional=True): String(),
             t.Key("max_retries", optional=True): Int(),
             t.Key("token_type", optional=True): String(),
+            t.Key("use_case", optional=True): String(),
         }
     ).allow_extra("*")
     _fields = {k.to_name or k.name for k in _converter.keys}
 
     def __init__(
         self,
         endpoint: str,
         token: str,
         connect_timeout: Optional[int] = None,
         ssl_verify: bool = True,
         user_agent_suffix: Optional[str] = None,
         max_retries: Optional[Union[int, Retry]] = None,
         token_type: Optional[str] = None,
+        use_case: Optional[str] = None,
     ) -> None:
         self.endpoint = endpoint
         self.token = token
         self.connect_timeout = connect_timeout
         self.ssl_verify = ssl_verify
         self.user_agent_suffix = user_agent_suffix
         self.max_retries = max_retries
         self.token_type = token_type
+        self.use_case = use_case
+
+        if self.use_case is not None:
+            _context.get().use_case = self.use_case
 
     @classmethod
     def from_data(cls, data: Dict[str, Any]) -> DataRobotClientConfig:
         checked = {k: v for k, v in cls._converter.check(data).items() if k in cls._fields}
         return cls(**checked)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/__init__.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module is not considered part of the public interface. As of 2.3, anything here
 may change or be removed without warning."""
 from __future__ import annotations
 
 from collections import defaultdict
+from copy import deepcopy
 from datetime import date, datetime
 import re
 from typing import Any, cast, Dict, Iterable, List, Match, Optional, Tuple, TYPE_CHECKING, Union
 
 from dateutil import parser, tz
 import numpy as np
 import pandas as pd
@@ -70,15 +71,17 @@
     do_recursive: bool = True,
     keep_attrs: Optional[Union[Iterable[str], Iterable[List[str]]]] = None,
     keep_null_keys: bool = False,
 ) -> ServerDataType:
     if type(data) not in (dict, list):
         return data
     if isinstance(data, list):
-        return _from_api_list(data, do_recursive=do_recursive, keep_null_keys=keep_null_keys)
+        return _from_api_list(
+            data, do_recursive=do_recursive, keep_attrs=keep_attrs, keep_null_keys=keep_null_keys
+        )
     return _from_api_dict(
         data, do_recursive=do_recursive, keep_attrs=keep_attrs, keep_null_keys=keep_null_keys
     )
 
 
 # pylint: disable-next=missing-function-docstring
 def _from_api_dict(
@@ -105,30 +108,37 @@
         k_under = underscorize(k)
         if v is None and k_under not in current_level and not keep_null_keys:
             continue
         if do_recursive:
             data_val = from_api(
                 v,
                 do_recursive=do_recursive,
-                keep_attrs=next_level_attrs,
+                keep_attrs=deepcopy(next_level_attrs),
                 keep_null_keys=keep_null_keys,
             )
         else:
             data_val = v
         app_data[k_under] = data_val
     return app_data
 
 
 def _from_api_list(
     data: ServerDataListType,
     do_recursive: bool = True,
+    keep_attrs: Optional[Union[Iterable[str], Iterable[List[str]]]] = None,
     keep_null_keys: bool = False,
 ) -> List[Any]:
     return [
-        from_api(datum, do_recursive=do_recursive, keep_null_keys=keep_null_keys) for datum in data
+        from_api(
+            datum,
+            do_recursive=do_recursive,
+            keep_attrs=deepcopy(keep_attrs),
+            keep_null_keys=keep_null_keys,
+        )
+        for datum in data
     ]
 
 
 def remove_empty_keys(
     metadata: Dict[str, Any],
     keep_attrs: Optional[List[str]] = None,
 ) -> Dict[str, Any]:
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/deprecation.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/pagination.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/retry.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/source.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/waiters.py` & `datarobot_early_access-3.2.0.2023.5.1/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.2.0.2023.4.3
+Version: 3.2.0.2023.5.1
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.2.0.2023.5.1/datarobot_early_access.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-contextlib2>=0.5.5
 pandas>=0.15
 numpy
 pyyaml>=3.11
-requests>=2.21
+requests>=2.28.1
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
-urllib3>=1.23
+urllib3<2.0.0,>=1.23
 typing-extensions==4.3.0
 
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
@@ -23,23 +22,20 @@
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
 types-requests==2.28.11
 types-urllib3==1.26.25
 Pillow==9.2.0
 Pillow==9.2.0
-Sphinx==1.8.3
-sphinx_rtd_theme==0.1.9
-nbsphinx<1,>=0.2.9
-mistune==0.8.4
-nbconvert==5.3.1
-numpydoc>=0.6.0
+Sphinx==4.3.2
+sphinx_rtd_theme==1.0.0
+nbsphinx==0.8.9
+numpydoc==1.4.0
 jupyter_contrib_nbextensions
-tornado<6.0
-jsonschema<=4.3.1
+sphinx-autodoc-typehints==1.17.1
 
 [examples]
 jupyter<=5.0
 fredapi==0.4.0
 matplotlib>=2.1.0
 seaborn<=0.8
 scikit-learn<=0.18.2
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/pyproject.toml` & `datarobot_early_access-3.2.0.2023.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     ### And also we can delete an entry for a file and fix the corresponding errors as we piece-meal annotate the whole repo.
     "datarobot.models.api_object",
     "datarobot.models.batch_prediction_job",
     "datarobot.models.custom_model",
     "datarobot.models.custom_model_test",
     "datarobot.models.custom_model_version",
     "datarobot.models.custom_task_version",
-    "datarobot.models.data_drift",
     "datarobot.models.data_engine_query_generator",
     "datarobot.models.datetime_trend_plots",
     "datarobot.models.execution_environment",
     "datarobot.models.execution_environment_version",
     "datarobot.models.feature",
     "datarobot.models.feature_effect",
     "datarobot.models.feature_fit",
@@ -83,14 +82,15 @@
     "datarobot.models.project",
     "datarobot.models.project_options",
     "datarobot.models.relationships_configuration",
     "datarobot.models.training_predictions",
 
     ### Sub-directories in models
     "datarobot.models.external_dataset_scores_insights.external_confusion_chart",
+    "datarobot.models.deployment.data_drift",
     "datarobot.models.user_blueprints.models",
 
     # Ignore specific files in datarobot sub-directory of repo.
     "datarobot.client",
     "datarobot.enums",
 ]
 ignore_errors = true
```

### Comparing `datarobot_early_access-3.2.0.2023.4.3/setup.py` & `datarobot_early_access-3.2.0.2023.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.3/setup_weekly.py` & `datarobot_early_access-3.2.0.2023.5.1/setup_weekly.py`

 * *Files identical despite different names*

