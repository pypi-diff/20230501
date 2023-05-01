# Comparing `tmp/google-cloud-automlops-1.0.5.tar.gz` & `tmp/google-cloud-automlops-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-automlops-1.0.5.tar", last modified: Mon Mar  6 21:46:28 2023, max compression
+gzip compressed data, was "google-cloud-automlops-1.1.0.tar", last modified: Mon May  1 20:18:52 2023, max compression
```

## Comparing `google-cloud-automlops-1.0.5.tar` & `google-cloud-automlops-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-03-06 21:46:28.012391 google-cloud-automlops-1.0.5/
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-03-06 21:46:28.011219 google-cloud-automlops-1.0.5/AutoMLOps/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    43140 2023-03-06 21:44:05.000000 google-cloud-automlops-1.0.5/AutoMLOps/AutoMLOps.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-02-07 20:59:28.000000 google-cloud-automlops-1.0.5/AutoMLOps/AutoMLOps_test.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    12078 2023-02-07 20:51:34.000000 google-cloud-automlops-1.0.5/AutoMLOps/BuilderUtils.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    19460 2023-03-06 19:29:22.000000 google-cloud-automlops-1.0.5/AutoMLOps/CloudRunBuilder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     8507 2023-02-07 19:52:13.000000 google-cloud-automlops-1.0.5/AutoMLOps/ComponentBuilder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     2444 2023-02-07 20:41:39.000000 google-cloud-automlops-1.0.5/AutoMLOps/JupyterUtilsMagic.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14800 2023-03-06 16:10:04.000000 google-cloud-automlops-1.0.5/AutoMLOps/PipelineBuilder.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-03-06 21:46:10.000000 google-cloud-automlops-1.0.5/AutoMLOps/__init__.py
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.0.5/LICENSE
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13984 2023-03-06 21:46:28.012218 google-cloud-automlops-1.0.5/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13115 2023-03-06 21:28:52.000000 google-cloud-automlops-1.0.5/README.md
-drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-03-06 21:46:28.012007 google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13984 2023-03-06 21:46:28.000000 google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/PKG-INFO
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      473 2023-03-06 21:46:28.000000 google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/SOURCES.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-03-06 21:46:28.000000 google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/dependency_links.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)      105 2023-03-06 21:46:28.000000 google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/requires.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       10 2023-03-06 21:46:28.000000 google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/top_level.txt
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-03-06 21:46:28.012438 google-cloud-automlops-1.0.5/setup.cfg
--rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1986 2023-03-06 21:46:17.000000 google-cloud-automlops-1.0.5/setup.py
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-01 20:18:52.525854 google-cloud-automlops-1.1.0/
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-01 20:18:52.524621 google-cloud-automlops-1.1.0/AutoMLOps/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    43608 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      702 2023-02-07 20:59:28.000000 google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps_test.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     9741 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/BuilderUtils.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    19465 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/CloudRunBuilder.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    10765 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/ComponentBuilder.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13155 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/PipelineBuilder.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1199 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/AutoMLOps/__init__.py
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    11357 2023-01-13 20:01:02.000000 google-cloud-automlops-1.1.0/LICENSE
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14181 2023-05-01 20:18:52.525651 google-cloud-automlops-1.1.0/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    13312 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/README.md
+drwxr-xr-x   0 srastatter (1006147) primarygroup (89939)        0 2023-05-01 20:18:52.525435 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)    14181 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/PKG-INFO
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)      442 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/SOURCES.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)        1 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/dependency_links.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       79 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/requires.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       10 2023-05-01 20:18:52.000000 google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/top_level.txt
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)       38 2023-05-01 20:18:52.525910 google-cloud-automlops-1.1.0/setup.cfg
+-rw-r--r--   0 srastatter (1006147) primarygroup (89939)     1910 2023-05-01 20:16:21.000000 google-cloud-automlops-1.1.0/setup.py
```

### Comparing `google-cloud-automlops-1.0.5/AutoMLOps/AutoMLOps.py` & `google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,45 +12,43 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """AutoMLOps is a tool that generates a production-style MLOps pipeline
    from Jupyter Notebooks."""
 
 # pylint: disable=C0103
-# pylint: disable=unused-import
 # pylint: disable=line-too-long
 
+import functools
 import logging
 import os
 import re
+import sys
 import subprocess
-from typing import Dict, List
+from typing import Callable, Dict, List, Optional
 
 from AutoMLOps import BuilderUtils
 from AutoMLOps import ComponentBuilder
 from AutoMLOps import PipelineBuilder
 from AutoMLOps import CloudRunBuilder
-from AutoMLOps import JupyterUtilsMagic
 
+logging.basicConfig(stream=sys.stdout, level=logging.INFO, format='%(message)s')
 logger = logging.getLogger()
-log_level = os.environ.get('LOG_LEVEL', 'INFO')
-logger.setLevel(log_level)
 
 TOP_LVL_NAME = 'AutoMLOps/'
 DEFAULTS_FILE = TOP_LVL_NAME + 'configs/defaults.yaml'
 PIPELINE_SPEC_SH_FILE = TOP_LVL_NAME + 'scripts/build_pipeline_spec.sh'
 BUILD_COMPONENTS_SH_FILE = TOP_LVL_NAME + 'scripts/build_components.sh'
 RUN_PIPELINE_SH_FILE = TOP_LVL_NAME + 'scripts/run_pipeline.sh'
 RUN_ALL_SH_FILE = TOP_LVL_NAME + 'scripts/run_all.sh'
 RESOURCES_SH_FILE = TOP_LVL_NAME + 'scripts/create_resources.sh'
 SUBMIT_JOB_FILE = TOP_LVL_NAME + 'scripts/submit_to_runner_svc.sh'
 CLOUDBUILD_FILE = TOP_LVL_NAME + 'cloudbuild.yaml'
 PIPELINE_FILE = TOP_LVL_NAME + 'pipelines/pipeline.py'
-IMPORTS_FILE = '.imports.py'
-DEFAULT_IMAGE = 'python:3.9'
+DEFAULT_IMAGE = 'python:3.9-slim'
 COMPONENT_BASE = TOP_LVL_NAME + 'components/component_base'
 COMPONENT_BASE_SRC = TOP_LVL_NAME + 'components/component_base/src'
 OUTPUT_DIR = BuilderUtils.TMPFILES_DIR
 DIRS = [
     TOP_LVL_NAME,
     TOP_LVL_NAME + 'components',
     TOP_LVL_NAME + 'components/component_base',
@@ -60,34 +58,34 @@
     TOP_LVL_NAME + 'pipelines',
     TOP_LVL_NAME + 'pipelines/runtime_parameters',
     TOP_LVL_NAME + 'scripts',
     TOP_LVL_NAME + 'scripts/pipeline_spec']
 
 def go(project_id: str,
        pipeline_params: Dict,
-       af_registry_location: str = 'us-central1',
-       af_registry_name: str = 'vertex-mlops-af',
-       cb_trigger_location: str = 'us-central1',
-       cb_trigger_name: str = 'automlops-trigger',
-       cloud_run_location: str = 'us-central1',
-       cloud_run_name: str = 'run-pipeline',
-       cloud_tasks_queue_location: str = 'us-central1',
-       cloud_tasks_queue_name: str = 'queueing-svc',
-       csr_branch_name: str = 'automlops',
-       csr_name: str = 'AutoMLOps-repo',
-       custom_training_job_specs: List[Dict] = None,
-       gs_bucket_location: str = 'us-central1',
-       gs_bucket_name: str = None,
-       pipeline_runner_sa: str = None,
-       run_local: bool = True,
-       schedule_location: str = 'us-central1',
-       schedule_name: str = 'AutoMLOps-schedule',
-       schedule_pattern: str = 'No Schedule Specified',
-       use_kfp_spec: bool = False,
-       vpc_connector: str = 'No VPC Specified'):
+       af_registry_location: Optional[str] = 'us-central1',
+       af_registry_name: Optional[str] = 'vertex-mlops-af',
+       cb_trigger_location: Optional[str] = 'us-central1',
+       cb_trigger_name: Optional[str] = 'automlops-trigger',
+       cloud_run_location: Optional[str] = 'us-central1',
+       cloud_run_name: Optional[str] = 'run-pipeline',
+       cloud_tasks_queue_location: Optional[str] = 'us-central1',
+       cloud_tasks_queue_name: Optional[str] = 'queueing-svc',
+       csr_branch_name: Optional[str] = 'automlops',
+       csr_name: Optional[str] = 'AutoMLOps-repo',
+       custom_training_job_specs: Optional[List[Dict]] = None,
+       gs_bucket_location: Optional[str] = 'us-central1',
+       gs_bucket_name: Optional[str] = None,
+       pipeline_runner_sa: Optional[str] = None,
+       run_local: Optional[bool] = True,
+       schedule_location: Optional[str] = 'us-central1',
+       schedule_name: Optional[str] = 'AutoMLOps-schedule',
+       schedule_pattern: Optional[str] = 'No Schedule Specified',
+       use_kfp_spec: Optional[bool] = False,
+       vpc_connector: Optional[str] = 'No VPC Specified'):
     """Generates relevant pipeline and component artifacts,
        then builds, compiles, and submits the PipelineJob.
 
     Args:
         project_id: The project ID.
         pipeline_params: Dictionary containing runtime pipeline parameters.
         af_registry_location: Region of the Artifact Registry.
@@ -119,75 +117,76 @@
              pipeline_runner_sa, run_local, schedule_location,
              schedule_name, schedule_pattern, use_kfp_spec,
              vpc_connector)
     run(run_local)
 
 def generate(project_id: str,
              pipeline_params: Dict,
-             af_registry_location: str = 'us-central1',
-             af_registry_name: str = 'vertex-mlops-af',
-             cb_trigger_location: str = 'us-central1',
-             cb_trigger_name: str = 'automlops-trigger',
-             cloud_run_location: str = 'us-central1',
-             cloud_run_name: str = 'run-pipeline',
-             cloud_tasks_queue_location: str = 'us-central1',
-             cloud_tasks_queue_name: str = 'queueing-svc',
-             csr_branch_name: str = 'automlops',
-             csr_name: str = 'AutoMLOps-repo',
-             custom_training_job_specs: List[Dict] = None,
-             gs_bucket_location: str = 'us-central1',
-             gs_bucket_name: str = None,
-             pipeline_runner_sa: str = None,
-             run_local: bool = True,
-             schedule_location: str = 'us-central1',
-             schedule_name: str = 'AutoMLOps-schedule',
-             schedule_pattern: str = 'No Schedule Specified',
-             use_kfp_spec: bool = False,
-             vpc_connector: str = 'No VPC Specified'):
+             af_registry_location: Optional[str] = 'us-central1',
+             af_registry_name: Optional[str] = 'vertex-mlops-af',
+             cb_trigger_location: Optional[str] = 'us-central1',
+             cb_trigger_name: Optional[str] = 'automlops-trigger',
+             cloud_run_location: Optional[str] = 'us-central1',
+             cloud_run_name: Optional[str] = 'run-pipeline',
+             cloud_tasks_queue_location: Optional[str] = 'us-central1',
+             cloud_tasks_queue_name: Optional[str] = 'queueing-svc',
+             csr_branch_name: Optional[str] = 'automlops',
+             csr_name: Optional[str] = 'AutoMLOps-repo',
+             custom_training_job_specs: Optional[List[Dict]] = None,
+             gs_bucket_location: Optional[str] = 'us-central1',
+             gs_bucket_name: Optional[str] = None,
+             pipeline_runner_sa: Optional[str] = None,
+             run_local: Optional[bool] = True,
+             schedule_location: Optional[str] = 'us-central1',
+             schedule_name: Optional[str] = 'AutoMLOps-schedule',
+             schedule_pattern: Optional[str] = 'No Schedule Specified',
+             use_kfp_spec: Optional[bool] = False,
+             vpc_connector: Optional[str] = 'No VPC Specified'):
     """Generates relevant pipeline and component artifacts.
 
     Args: See go() function.
     """
     BuilderUtils.validate_schedule(schedule_pattern, run_local)
     default_bucket_name = f'{project_id}-bucket' if gs_bucket_name is None else gs_bucket_name
     default_pipeline_runner_sa = f'vertex-pipelines@{project_id}.iam.gserviceaccount.com' if pipeline_runner_sa is None else pipeline_runner_sa
     BuilderUtils.make_dirs(DIRS)
     _create_default_config(af_registry_location, af_registry_name, cb_trigger_location,
                            cb_trigger_name, cloud_run_location, cloud_run_name,
                            cloud_tasks_queue_location, cloud_tasks_queue_name, csr_branch_name,
                            csr_name, gs_bucket_location, default_bucket_name,
                            default_pipeline_runner_sa, project_id, schedule_location,
                            schedule_name, schedule_pattern, vpc_connector)
-
     _create_scripts(run_local)
     _create_cloudbuild_config(run_local)
     # copy tmp pipeline file over to AutoMLOps dir
     BuilderUtils.execute_process(f'cp {BuilderUtils.PIPELINE_TMPFILE} {PIPELINE_FILE}', to_null=False)
     # Create components and pipelines
     components_path_list = BuilderUtils.get_components_list()
     for path in components_path_list:
         ComponentBuilder.formalize(path, TOP_LVL_NAME, DEFAULTS_FILE, use_kfp_spec)
     PipelineBuilder.formalize(custom_training_job_specs, DEFAULTS_FILE, pipeline_params, TOP_LVL_NAME)
-    if not use_kfp_spec:
-        _autoflake_srcfiles()
-    _create_requirements(use_kfp_spec)
+    _create_requirements()
     _create_dockerfile()
     if not run_local:
         CloudRunBuilder.formalize(TOP_LVL_NAME, DEFAULTS_FILE)
 
 def run(run_local: bool):
     """Builds, compiles, and submits the PipelineJob.
 
     Args:
         run_local: Flag that determines whether to use Cloud Run CI/CD.
     """
     BuilderUtils.execute_process('./'+RESOURCES_SH_FILE, to_null=False)
     if run_local:
         os.chdir(TOP_LVL_NAME)
-        BuilderUtils.execute_process('./scripts/run_all.sh', to_null=False)
+        try:
+            subprocess.run(['./scripts/run_all.sh'], shell=True, check=True,
+                stderr=subprocess.STDOUT)
+        except subprocess.CalledProcessError as e:
+            logging.info(e)
         os.chdir('../')
     else:
         _push_to_csr()
     _resources_generation_manifest(run_local)
 
 def _resources_generation_manifest(run_local: bool):
     """Logs urls of generated resources.
@@ -584,49 +583,49 @@
             f'           "--vpc-connector", "{vpc_connector}",\n'
             f'           "--vpc-egress", "all-traffic"')
     vpc_connector_tail += ']\n'
 
     cloudbuild_comp_config = (BuilderUtils.LICENSE +
         f'steps:\n'
         f'# ==============================================================================\n'
-        f'# BUILD & PUSH CUSTOM COMPONENT IMAGES\n'
+        f'# BUILD CUSTOM IMAGES\n'
         f'# ==============================================================================\n'
         f'\n'
         f'''  # build the component_base image\n'''
         f'''  - name: "gcr.io/cloud-builders/docker"\n'''
         f'''    args: [ "build", "-t", "{defaults['gcp']['af_registry_location']}-docker.pkg.dev/{defaults['gcp']['project_id']}/{defaults['gcp']['af_registry_name']}/components/component_base:latest", "." ]\n'''
         f'''    dir: "{TOP_LVL_NAME}components/component_base"\n'''
         f'''    id: "build_component_base"\n'''
         f'''    waitFor: ["-"]\n'''
         f'\n'
-        f'''  # push the component_base image\n'''
-        f'''  - name: "gcr.io/cloud-builders/docker"\n'''
-        f'''    args: ["push", "{defaults['gcp']['af_registry_location']}-docker.pkg.dev/{defaults['gcp']['project_id']}/{defaults['gcp']['af_registry_name']}/components/component_base:latest"]\n'''
-        f'''    dir: "{TOP_LVL_NAME}components/component_base"\n'''
-        f'''    id: "push_component_base"\n'''
-        f'''    waitFor: ["build_component_base"]\n''')
-    cloudbuild_cloudrun_config = (
-        f'\n'
-        f'# ==============================================================================\n'
-        f'# BUILD & PUSH CLOUD RUN IMAGES\n'
-        f'# ==============================================================================\n'
-        f'\n'
         f'''  # build the run_pipeline image\n'''
         f'''  - name: 'gcr.io/cloud-builders/docker'\n'''
         f'''    args: [ "build", "-t", "{defaults['gcp']['af_registry_location']}-docker.pkg.dev/{defaults['gcp']['project_id']}/{defaults['gcp']['af_registry_name']}/run_pipeline:latest", "-f", "cloud_run/run_pipeline/Dockerfile", "." ]\n'''
         f'''    dir: "{TOP_LVL_NAME}"\n'''
         f'''    id: "build_pipeline_runner_svc"\n'''
-        f'''    waitFor: ['push_component_base']\n'''
+        f'''    waitFor: ['build_component_base']\n''')
+    cloudbuild_cloudrun_config = (
+        f'\n'
+        f'# ==============================================================================\n'
+        f'# PUSH & DEPLOY CUSTOM IMAGES\n'
+        f'# ==============================================================================\n'
+        f'\n'
+        f'''  # push the component_base image\n'''
+        f'''  - name: "gcr.io/cloud-builders/docker"\n'''
+        f'''    args: ["push", "{defaults['gcp']['af_registry_location']}-docker.pkg.dev/{defaults['gcp']['project_id']}/{defaults['gcp']['af_registry_name']}/components/component_base:latest"]\n'''
+        f'''    dir: "{TOP_LVL_NAME}components/component_base"\n'''
+        f'''    id: "push_component_base"\n'''
+        f'''    waitFor: ["build_pipeline_runner_svc"]\n'''
         f'\n'
         f'''  # push the run_pipeline image\n'''
         f'''  - name: "gcr.io/cloud-builders/docker"\n'''
         f'''    args: ["push", "{defaults['gcp']['af_registry_location']}-docker.pkg.dev/{defaults['gcp']['project_id']}/{defaults['gcp']['af_registry_name']}/run_pipeline:latest"]\n'''
         f'''    dir: "{TOP_LVL_NAME}"\n'''
         f'''    id: "push_pipeline_runner_svc"\n'''
-        f'''    waitFor: ["build_pipeline_runner_svc"]\n'''
+        f'''    waitFor: ["push_component_base"]\n'''
         f'\n'
         f'''  # deploy the cloud run service\n'''
         f'''  - name: "gcr.io/google.com/cloudsdktool/cloud-sdk"\n'''
         f'''    entrypoint: gcloud\n'''
         f'''    args: ["run",\n'''
         f'''           "deploy",\n'''
         f'''           "{defaults['gcp']['cloud_run_name']}",\n'''
@@ -685,77 +684,72 @@
     else:
         if defaults['gcp']['cloud_schedule_pattern'] == 'No Schedule Specified':
             cb_file_contents = cloudbuild_comp_config + cloudbuild_cloudrun_config + custom_comp_image + cloudrun_image
         else:
             cb_file_contents = cloudbuild_comp_config + cloudbuild_cloudrun_config + cloudbuild_scheduler_config + custom_comp_image + cloudrun_image
     BuilderUtils.write_file(CLOUDBUILD_FILE, cb_file_contents, 'w+')
 
-def _autoflake_srcfiles():
-    """Removes unused imports from the python srcfiles. By default,
-       all imports listed in the imports cell will be written to
-       each srcfile. Autoflake removes the ones not being used."""
-    BuilderUtils.execute_process(f'python3 -m autoflake --in-place --remove-all-unused-imports {COMPONENT_BASE_SRC}/*.py', to_null=False)
-
-def _create_requirements(use_kfp_spec: bool):
+def _create_requirements():
     """Writes a requirements.txt to the component_base directory.
-       If not using kfp spec, infers pip requirements from the
-       python srcfiles using pipreqs. Some default gcp packages
-       are included, as well as packages that are often missing
+       Infers pip requirements from the python srcfiles using 
+       pipreqs. Takes user-inputted requirements, and addes some 
+       default gcp packages as well as packages that are often missing
        in setup.py files (e.g db_types, pyarrow, gcsfs, fsspec).
-
-    Args:
-        use_kfp_spec: Flag that determines the format of the component yamls.
     """
     reqs_filename = f'{COMPONENT_BASE}/requirements.txt'
-    if use_kfp_spec:
-        BuilderUtils.delete_file(reqs_filename)
-        components_path_list = BuilderUtils.get_components_list()
-        for component_path in components_path_list:
-            component_spec = BuilderUtils.read_yaml_file(component_path)
-            reqs = component_spec['implementation']['container']['command'][2]
-            formatted_reqs = re.findall('\'([^\']*)\'', reqs)
-            reqs_str = ''.join(r+'\n' for r in formatted_reqs)
-            BuilderUtils.write_file(reqs_filename, reqs_str, 'a+')
-    else:
-        gcp_reqs = (
-            'google-cloud-aiplatform\n'
-            'google-cloud-appengine-logging\n'
-            'google-cloud-audit-log\n'
-            'google-cloud-bigquery\n'
-            'google-cloud-bigquery-storage\n'
-            'google-cloud-bigtable\n'
-            'google-cloud-core\n'
-            'google-cloud-dataproc\n'
-            'google-cloud-datastore\n'
-            'google-cloud-dlp\n'
-            'google-cloud-firestore\n'
-            'google-cloud-kms\n'
-            'google-cloud-language\n'
-            'google-cloud-logging\n'
-            'google-cloud-monitoring\n'
-            'google-cloud-notebooks\n'
-            'google-cloud-pipeline-components\n'
-            'google-cloud-pubsub\n'
-            'google-cloud-pubsublite\n'
-            'google-cloud-recommendations-ai\n'
-            'google-cloud-resource-manager\n'
-            'google-cloud-scheduler\n'
-            'google-cloud-spanner\n'
-            'google-cloud-speech\n'
-            'google-cloud-storage\n'
-            'google-cloud-tasks\n'
-            'google-cloud-translate\n'
-            'google-cloud-videointelligence\n'
-            'google-cloud-vision\n'
-            'db_dtypes\n'
-            'pyarrow\n'
-            'gcsfs\n'
-            'fsspec\n')
-        BuilderUtils.execute_process(f'python3 -m pipreqs.pipreqs {COMPONENT_BASE} --mode no-pin --force', to_null=False)
-        BuilderUtils.write_file(reqs_filename, gcp_reqs, 'a')
+    default_gcp_reqs = [
+        'google-cloud-aiplatform',
+        'google-cloud-appengine-logging',
+        'google-cloud-audit-log',
+        'google-cloud-bigquery',
+        'google-cloud-bigquery-storage',
+        'google-cloud-bigtable',
+        'google-cloud-core',
+        'google-cloud-dataproc',
+        'google-cloud-datastore',
+        'google-cloud-dlp',
+        'google-cloud-firestore',
+        'google-cloud-kms',
+        'google-cloud-language',
+        'google-cloud-logging',
+        'google-cloud-monitoring',
+        'google-cloud-notebooks',
+        'google-cloud-pipeline-components',
+        'google-cloud-pubsub',
+        'google-cloud-pubsublite',
+        'google-cloud-recommendations-ai',
+        'google-cloud-resource-manager',
+        'google-cloud-scheduler',
+        'google-cloud-spanner',
+        'google-cloud-speech',
+        'google-cloud-storage',
+        'google-cloud-tasks',
+        'google-cloud-translate',
+        'google-cloud-videointelligence',
+        'google-cloud-vision',
+        'db_dtypes',
+        'pyarrow',
+        'gcsfs',
+        'fsspec']
+    # Infer reqs using pipreqs
+    BuilderUtils.execute_process(f'python3 -m pipreqs.pipreqs {COMPONENT_BASE} --mode no-pin --force', to_null=False)
+    pipreqs = BuilderUtils.read_file(reqs_filename).splitlines()
+    # Get user-inputted requirements from .tmpfiles dir
+    user_inp_reqs = []
+    components_path_list = BuilderUtils.get_components_list()
+    for component_path in components_path_list:
+        component_spec = BuilderUtils.read_yaml_file(component_path)
+        reqs = component_spec['implementation']['container']['command'][2]
+        formatted_reqs = re.findall('\'([^\']*)\'', reqs)
+        user_inp_reqs.extend(formatted_reqs)
+    # Remove duplicates
+    set_of_requirements = set(user_inp_reqs) if user_inp_reqs else set(pipreqs + default_gcp_reqs)
+    reqs_str = ''.join(r+'\n' for r in sorted(set_of_requirements))
+    BuilderUtils.delete_file(reqs_filename)
+    BuilderUtils.write_file(reqs_filename, reqs_str, 'w')
 
 def _create_dockerfile():
     """Writes a Dockerfile to the component_base directory."""
     # pylint: disable=anomalous-backslash-in-string
     dockerfile = (BuilderUtils.LICENSE +
         f'FROM {DEFAULT_IMAGE}\n'
         f'RUN python -m pip install --upgrade pip\n'
@@ -763,50 +757,71 @@
         f'RUN python -m pip install -r \ \n'
         f'    requirements.txt --quiet --no-cache-dir \ \n'
         f'    && rm -f requirements.txt\n'
         f'COPY ./src /pipelines/component/src\n'
         f'ENTRYPOINT ["/bin/bash"]\n')
     BuilderUtils.write_file(f'{COMPONENT_BASE}/Dockerfile', dockerfile, 'w')
 
-def makeComponent(name: str,
-                  params: list,
-                  description: str = None):
-    """Wrapper function that creates a tmp component scaffold
-       which will be used by the ComponentBuilder formalize function.
-
+def component(func: Optional[Callable] = None,
+              *,
+              packages_to_install: Optional[List[str]] = None):
+    """Decorator for Python-function based components in AutoMLOps.
+
+    Example usage:
+    from AutoMLOps import AutoMLOps
+    @AutoMLOps.component
+    def my_function_one(input: str, output: Output[Model]):
+      ...
     Args:
-        name: Component name.
-        params: Component parameters. A list of dictionaries,
-            each param is a dict containing keys:
-                'name': required, str param name.
-                'type': required, python primitive type.
-                'description': optional, str param desc.
-        description: Optional description of the component.
-    """
-    ComponentBuilder.create_component_scaffold(name,
-        params, description)
-
-def makePipeline(name: str,
-                 params: list,
-                 pipeline: list,
-                 description: str = None):
-    """Wrapper function that creates a tmp pipeline scaffold
-       which will be used by the PipelineBuilder formalize function.
-
+        func: The python function to create a component from. The function
+            should have type annotations for all its arguments, indicating how
+            it is intended to be used (e.g. as an input/output Artifact object,
+            a plain parameter, or a path to a file).
+        packages_to_install: A list of optional packages to install before
+            executing func. These will always be installed at component runtime.
+  """
+    if func is None:
+        return functools.partial(
+            component,
+            packages_to_install=packages_to_install)
+    else:
+        return ComponentBuilder.create_component_scaffold(
+            func=func,
+            packages_to_install=packages_to_install)
+
+def pipeline(func: Optional[Callable] = None,
+             *,
+             name: Optional[str] = None,
+             description: Optional[str] = None):
+    """Decorator for Python-function based pipelines in AutoMLOps.
+
+    Example usage:
+    from AutoMLOps import AutoMLOps
+    @AutoMLOps.pipeline
+    def pipeline(bq_table: str,
+                output_model_directory: str,
+                project: str,
+                region: str,
+                ):
+
+        dataset_task = create_dataset(
+            bq_table=bq_table, 
+            project=project)
+      ...
     Args:
-        name: Pipeline name.
-        params: Pipeline parameters. A list of dictionaries,
-            each param is a dict containing keys:
-                'name': required, str param name.
-                'type': required, python primitive type.
-                'description': optional, str param desc.
-        pipeline: Defines the components to use in the pipeline,
-            their order, and a mapping of component params to
-            pipeline params. A list of dictionaries, each dict
-            specifies a custom component and contains keys:
-                'component_name': name of the component
-                'param_mapping': a list of tuples mapping ->
-                    (component_param_name, pipeline_param_name)
-        description: Optional description of the pipeline.
-    """
-    PipelineBuilder.create_pipeline_scaffold(name,
-        params, pipeline, description)
+        func: The python function to create a pipeline from. The function
+            should have type annotations for all its arguments, indicating how
+            it is intended to be used (e.g. as an input/output Artifact object,
+            a plain parameter, or a path to a file).
+        name: The name of the pipeline.
+        description: Short description of what the pipeline does.
+  """
+    if func is None:
+        return functools.partial(
+            pipeline,
+            name=name,
+            description=description)
+    else:
+        return PipelineBuilder.create_pipeline_scaffold(
+            func=func,
+            name=name,
+            description=description)
```

### Comparing `google-cloud-automlops-1.0.5/AutoMLOps/AutoMLOps_test.py` & `google-cloud-automlops-1.1.0/AutoMLOps/AutoMLOps_test.py`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.0.5/AutoMLOps/BuilderUtils.py` & `google-cloud-automlops-1.1.0/AutoMLOps/BuilderUtils.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 
 """Utility functions and globals to be used by all
    other modules in this directory."""
 
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
+import inspect
 import os
 import subprocess
+
+import itertools
+import textwrap
+from typing import Callable
 import yaml
 
 TMPFILES_DIR = '.tmpfiles'
 IMPORTS_TMPFILE = f'{TMPFILES_DIR}/imports.py'
 CELL_TMPFILE = f'{TMPFILES_DIR}/cell.py'
 PIPELINE_TMPFILE = f'{TMPFILES_DIR}/pipeline_scaffold.py'
 PARAMETER_VALUES_PATH = 'pipelines/runtime_parameters/pipeline_parameter_values.json'
@@ -93,17 +98,17 @@
         raise yaml.YAMLError(f'Error writing to file. {err}') from err
 
 def read_file(filepath: str) -> str:
     """Reads a file and returns contents as a string.
        Defaults to utf-8 encoding.
 
     Args:
-        filepath: Path to the yaml.
+        filepath: Path to the file.
     Returns:
-        dict: Contents of the yaml.
+        str: Contents of the file.
     Raises:
         Exception: If an error is encountered reading the file.
     """
     try:
         with open(filepath, 'r', encoding='utf-8') as file:
             contents = file.read()
         file.close()
@@ -214,96 +219,14 @@
         run_local: Flag that determines whether to use Cloud Run CI/CD.
     Raises:
         Exception: If schedule is not cron formatted or run_local validation fails.
     """
     if schedule_pattern != 'No Schedule Specified' and run_local:
         raise ValueError('run_local must be set to False to use Cloud Scheduler.')
 
-def validate_name(name: str):
-    """Validates that the inputted name parameter is of type str.
-
-    Args:
-        name: The name of a component or pipeline.
-    Raises:
-        Exception: If the name is not of type str.
-    """
-    if not isinstance(name, str):
-        raise TypeError('Pipeline and Component names must be of type string.')
-
-def validate_params(params: list):
-    """Verifies that the inputted params follow the correct
-       specification.
-
-    Args:
-        params: Pipeline parameters. A list of dictionaries,
-            each param is a dict containing keys:
-                'name': required, str param name.
-                'type': required, python primitive type.
-                'description': optional, str param desc.
-    Raises:
-        Exception: If incorrect params specification.
-    """
-    s = set()
-    for param in params:
-        try:
-            name = param['name']
-            if not isinstance(name, str):
-                raise TypeError('Parameter name must be of type string.')
-            param_type = param['type']
-            if not isinstance(param_type, type):
-                raise TypeError('Parameter type must be a valid python type.')
-        except KeyError as err:
-            raise ValueError(f'Parameter {param} does not contain '
-                             f'required keys. {err}') from err
-        if param['name'] in s:
-            raise ValueError(f'''Duplicate parameter {param['name']} found.''')
-        else:
-            s.add(param['name'])
-        if 'description' not in param.keys():
-            param['description'] = 'No description provided.'
-
-def validate_pipeline_structure(pipeline: list):
-    """Verifies that the pipeline follows the correct
-       specification.
-
-    Args:
-        pipeline: Defines the components to use in the pipeline,
-            their order, and a mapping of component params to
-            pipeline params. A list of dictionaries, each dict
-            specifies a custom component and contains keys:
-                'component_name': name of the component
-                'param_mapping': a list of tuples mapping ->
-                    (component_param, pipeline_param)
-    Raises:
-        Exception: If incorrect pipeline specification.
-    """
-    components_list = get_components_list(full_path=False)
-    for component in pipeline:
-        try:
-            component_name = component['component_name']
-            if component_name not in components_list:
-                raise ValueError(f'Component {component_name} not found - '
-                    f'No matching yaml definition in tmpfiles directory.')
-            param_mapping = component['param_mapping']
-        except KeyError as err:
-            raise ValueError(f'Component {component} does not contain '
-                f'required keys. {err}') from err
-        for param_tuple in param_mapping:
-            if not isinstance(param_tuple, tuple):
-                raise TypeError(f'Mapping contains a non-tuple '
-                                f'element {param_tuple}')
-            elif len(param_tuple) != 2:
-                raise TypeError(f'Mapping must contain only 2 elements, '
-                                f'tuple {param_tuple} is invalid.')
-            else:
-                for item in param_tuple:
-                    if not isinstance(item, str):
-                        raise TypeError(f'Mapping must be str-str, '
-                                        f'tuple {param_tuple} is invalid.')
-
 def update_params(params: list) -> list:
     """Converts the parameter types from Python types
        to Kubeflow types. Currently only supports
        Python primitive types.
 
     Args:
         params: Pipeline parameters. A list of dictionaries,
@@ -325,9 +248,34 @@
         dict: 'Dict'
     }
     for param in params:
         try:
             param['type'] = python_kfp_types_mapper[param['type']]
         except KeyError as err:
             raise ValueError(f'Unsupported python type - we only support '
-                             f'primitive types at this time. {err}') from err
+                            f'primitive types at this time. {err}') from err
     return params
+
+def get_function_source_definition(func: Callable) -> str:
+    """Returns a formatted list of parameters.
+
+    Args:
+        func: The python function to create a component from. The function
+            should have type annotations for all its arguments, indicating how
+            it is intended to be used (e.g. as an input/output Artifact object,
+            a plain parameter, or a path to a file).
+    Returns:
+        str: The source code from the inputted function.
+    Raises:
+        Exception: If the preprocess operates failed.
+    """
+    source_code = inspect.getsource(func)
+    source_code = textwrap.dedent(source_code)
+    source_code_lines = source_code.split('\n')
+    source_code_lines = itertools.dropwhile(lambda x: not x.startswith('def'),
+                                            source_code_lines)
+    if not source_code_lines:
+        raise ValueError(
+            f'Failed to dedent and clean up the source of function "{func.__name__}". '
+            f'It is probably not properly indented.')
+
+    return '\n'.join(source_code_lines)
```

### Comparing `google-cloud-automlops-1.0.5/AutoMLOps/CloudRunBuilder.py` & `google-cloud-automlops-1.1.0/AutoMLOps/CloudRunBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """Writes a Dockerfile to the cloud_run/run_pipeline directory.
 
     Args:
         top_lvl_name: Top directory name.
     """
     cloudrun_base = top_lvl_name + 'cloud_run/run_pipeline'
     dockerfile = (BuilderUtils.LICENSE +
-        'FROM python:3.9\n'
+        'FROM python:3.9-slim\n'
         '\n'
         '# Allow statements and log messages to immediately appear in the Knative logs\n'
         'ENV PYTHONUNBUFFERED True\n'
         '\n'
         '# Copy local code to the container image.\n'
         'ENV APP_HOME /app\n'
         'WORKDIR $APP_HOME\n'
```

### Comparing `google-cloud-automlops-1.0.5/AutoMLOps/PipelineBuilder.py` & `google-cloud-automlops-1.1.0/AutoMLOps/PipelineBuilder.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 
 """Builds pipeline files."""
 
 # pylint: disable=C0103
 # pylint: disable=line-too-long
 
 import json
-from typing import Dict, List
+from typing import Callable, Dict, List, Optional
 
 from AutoMLOps import BuilderUtils
 
+DEFAULT_PIPELINE_NAME = 'automlops-pipeline'
+
 def formalize(custom_training_job_specs: List[Dict],
               defaults_file: str,
               pipeline_parameter_values: dict,
               top_lvl_name: str):
     """Constructs and writes pipeline.py, pipeline_runner.py, and pipeline_parameter_values.json files.
         pipeline.py: Generates a Kubeflow pipeline spec from custom components.
         pipeline_runner.py: Sends a PipelineJob to Vertex AI using pipeline spec.
@@ -81,15 +83,16 @@
     newline_tab = '\n    '
     return (
         f'''import argparse\n'''
         f'''import os\n'''
         f'''{gcpc_imports if custom_training_job_specs else ''}'''
         f'''import kfp\n'''
         f'''from kfp.v2 import compiler, dsl\n'''
-        f'''from kfp.v2.dsl import pipeline, component, Artifact, Dataset, Input, Metrics, Model, Output, InputPath, OutputPath\n'''
+        f'''from kfp.v2.dsl import *\n'''
+        f'''from typing import *\n'''
         f'''import yaml\n'''
         f'\n'
         f'''def load_custom_component(component_name: str):\n'''
         f'''    component_path = os.path.join('components',\n'''
         f'''                                component_name,\n'''
         f'''                              'component.yaml')\n'''
         f'''    return kfp.components.load_component_from_file(component_path)\n'''
@@ -143,19 +146,14 @@
 def get_pipeline_argparse() -> str:
     """Generates python code that loads default pipeline parameters from the defaults config_file.
 
     Returns:
         str: Python pipeline_argparse code.
     """
     return (
-        '''\n'''
-        '''    compiler.Compiler().compile(\n'''
-        '''        pipeline_func=pipeline,\n'''
-        '''        package_path=pipeline_job_spec_path)\n'''
-        '\n'
         '''if __name__ == '__main__':\n'''
         '''    parser = argparse.ArgumentParser()\n'''
         '''    parser.add_argument('--config', type=str,\n'''
         '''                       help='The config file for setting default values.')\n'''
         '\n'
         '''    args = parser.parse_args()\n'''
         '\n'
@@ -233,86 +231,61 @@
         '\n'
         '''    run_pipeline(project_id=config['gcp']['project_id'],\n'''
         '''                 pipeline_root=config['pipelines']['pipeline_storage_path'],\n'''
         '''                 pipeline_runner_sa=config['gcp']['pipeline_runner_service_account'],\n'''
         '''                 parameter_values_path=config['pipelines']['parameter_values_path'],\n'''
         '''                 pipeline_spec_path=config['pipelines']['pipeline_job_spec_path']) \n''')
 
-def create_pipeline_scaffold(name: str,
-                             params: list,
-                             pipeline: list,
-                             description: str = None):
+def create_pipeline_scaffold(func: Optional[Callable] = None,
+                             *,
+                             name: Optional[str] = None,
+                             description: Optional[str] = None):
     """Creates a temporary pipeline scaffold which will
        be used by the formalize function.
 
     Args:
-        name: Pipeline name.
-        params: Pipeline parameters. A list of dictionaries,
-            each param is a dict containing keys:
-                'name': required, str param name.
-                'type': required, python primitive type.
-                'description': optional, str param desc.
-        pipeline: Defines the components to use in the pipeline,
-            their order, and a mapping of component params to
-            pipeline params. A list of dictionaries, each dict
-            specifies a custom component and contains keys:
-                'component_name': name of the component
-                'param_mapping': a list of tuples mapping ->
-                    (component_param, pipeline_param)
-        description: Optional description of the pipeline.
+        func: The python function to create a pipeline from. The function
+            should have type annotations for all its arguments, indicating how
+            it is intended to be used (e.g. as an input/output Artifact object,
+            a plain parameter, or a path to a file).
+        name: The name of the pipeline.
+        description: Short description of what the pipeline does.
     """
-    BuilderUtils.validate_name(name)
-    BuilderUtils.validate_params(params)
-    BuilderUtils.validate_pipeline_structure(pipeline)
+    pipeline_scaffold = (get_pipeline_decorator(name, description) +
+                         BuilderUtils.get_function_source_definition(func) +
+                         get_compile_step(func.__name__))
     BuilderUtils.make_dirs([BuilderUtils.TMPFILES_DIR]) # if it doesn't already exist
-    pipeline_scaffold = get_pipeline_scaffold(name, params, pipeline, description)
     BuilderUtils.write_file(BuilderUtils.PIPELINE_TMPFILE, pipeline_scaffold, 'w')
 
-def get_pipeline_scaffold(name: str,
-                          params: list,
-                          pipeline: list,
-                          description: str):
-    """Generates the Kubeflow pipeline definition. Uses a
-       queue to define .after() ordering in the pipeline.
+def get_pipeline_decorator(name: Optional[str] = None,
+                           description: Optional[str] = None):
+    """Creates the kfp pipeline decorator.
 
     Args:
-        name: Pipeline name.
-        params: Pipeline parameters. A list of dictionaries,
-            each param is a dict containing keys:
-                'name': required, str param name.
-                'type': required, python primitive type.
-                'description': optional, str param desc.
-        pipeline: Defines the components to use in the pipeline,
-            their order, and a mapping of component params to
-            pipeline params. A list of dictionaries, each dict
-            specifies a custom component and contains keys:
-                'component_name': name of the component
-                'param_mapping': a list of tuples mapping ->
-                    (component_param, pipeline_param)
-        description: Optional description of the pipeline.
+        name: The name of the pipeline.
+        description: Short description of what the pipeline does.
+
+    Returns:
+        str: Python compile function call.
+    """
+    default_name = DEFAULT_PIPELINE_NAME if not name else name
+    name_str = f'''(\n    name='{default_name}',\n'''
+    desc_str = f'''    description='{description}',\n''' if description else ''
+    ending_str = ')\n'
+    return '@dsl.pipeline' + name_str + desc_str + ending_str
+
+def get_compile_step(func_name: str):
+    """Creates the compile function call.
+
+    Args:
+        func_name: The name of the pipeline function.
+
+    Returns:
+        str: Python compile function call.
     """
-    newline = '\n'
-    queue = ['']
-    for idx, component in enumerate(pipeline):
-        if idx != len(pipeline)-1:
-            queue.append(f'''.after({component['component_name']}_task)''')
     return (
         f'\n'
-        f'@dsl.pipeline(\n'
-        f'''    name='{name}',\n'''
-        f'''    description='{description}')\n'''
-        f'def pipeline(\n'
-        f'''{newline.join(f"    {param['name']}: {param['type'].__name__}," for param in params)}\n'''
-        f'):\n'
-        f'''    """{description}\n'''
-        f'\n'
-        f'    Args:\n'
-        f'''{newline.join(f"        {param['name']}: {param['description']}," for param in params)}\n'''
-        f'    """\n'
-        f"""{newline.join(
-        f'''    {component['component_name']}_task = {component['component_name']}({newline}'''
-        f'''    {f'{newline}    '.join(f"   {param[0]}={param[1]}," for param in component['param_mapping'])}{newline}'''
-        f'''    ){queue.pop(0)}{newline}'''
-        for component in pipeline
-        )}"""
+        f'compiler.Compiler().compile(\n'
+        f'    pipeline_func={func_name},\n'
+        f'    package_path=pipeline_job_spec_path)\n'
         f'\n'
     )
```

### Comparing `google-cloud-automlops-1.0.5/AutoMLOps/__init__.py` & `google-cloud-automlops-1.1.0/AutoMLOps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 import, with the end goal of becoming a Jupyter plugin to Vertex
 Workbench managed notebooks. The tool will generate yaml-component
 definitions, complete with Dockerfiles and requirements.txts for all
 Kubeflow components defined in a notebook. It will also generate a
 series of directories to support the creation of Vertex Pipelines.
 """
 # pylint: disable=invalid-name
-__version__ = '1.0.5'
+__version__ = '1.1.0'
 __author__ = 'Sean Rastatter'
 __credits__ = 'Google'
```

### Comparing `google-cloud-automlops-1.0.5/LICENSE` & `google-cloud-automlops-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-automlops-1.0.5/PKG-INFO` & `google-cloud-automlops-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.0.5
+Version: 1.1.0
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,16 +23,14 @@
 
 AutoMLOps is a service that generates a production ready MLOps pipeline from Jupyter Notebooks, bridging the gap between Data Science and DevOps and accelerating the adoption and use of Vertex AI. The service generates an MLOps codebase for users to customize, and provides a way to build and manage a CI/CD integrated MLOps pipeline from the notebook. AutoMLOps automatically builds a source repo for versioning, cloudbuild configs and triggers, an artifact registry for storing custom components, gs buckets, service accounts and updated IAM privs for running pipelines, enables APIs (cloud Run, Cloud Build, Artifact Registry, etc.), creates a runner service API in Cloud Run for submitting PipelineJobs to Vertex AI, and a Cloud Scheduler job for submitting PipelineJobs on a recurring basis. These automatic integrations empower data scientists to take their experiments to production more quickly, allowing them to focus on what they do best: providing actionable insights through data.
 
 # Prerequisites
 
 In order to use AutoMLOps, the following are required:
 
-- Jupyter (or Jupyter-compatible) notebook environment
-- [Notebooks API](https://console.cloud.google.com/marketplace/product/google/notebooks.googleapis.com) enabled
 - Python 3.7 - 3.10
 - [Google Cloud SDK 407.0.0](https://cloud.google.com/sdk/gcloud/reference)
 - [beta 2022.10.21](https://cloud.google.com/sdk/gcloud/reference/beta)
 - `git` installed
 - `git` logged-in:
 ```
   git config --global user.email "you@example.com"
@@ -47,19 +45,17 @@
 # Install
 
 Install AutoMLOps from [PyPI](https://pypi.org/project/google-cloud-automlops/): `pip install google-cloud-automlops` 
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
-- `autoflake==2.0.0`,
 - `docopt==0.6.2`,
-- `ipython==7.34.0`,
+- `docstring-parser==0.15`,
 - `pipreqs==0.4.11`,
-- `pyflakes==3.0.1`,
 - `PyYAML==5.4.1`,
 - `yarg==0.1.9`
 
 # GCP Services
 AutoMLOps makes use of the following products by default:
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction)
 - [Artifact Registry](https://cloud.google.com/artifact-registry/docs/overview)
@@ -168,18 +164,37 @@
 **Use a VPC connector:**
 
 Use the `vpc_connector` parameter to specify a vpc connector. 
 ```
 vpc_connector = 'example-vpc'
 ```
 
+**Specify package versions:**
+
+Use the `packages_to_install` parameter of `@AutoMLOps.component` to explicitly specify packages and versions. 
+```
+@AutoMLOps.component(
+    packages_to_install=[
+        "google-cloud-bigquery==2.34.4", 
+        "pandas",
+        "pyarrow",
+        "db_dtypes"
+    ]
+)
+def create_dataset(
+    bq_table: str,
+    data_path: str,
+    project_id: str
+):
+...
+```
 
 # Layout
 
-Included in the repository is an [example notebook](./example/automlops_example_notebook.ipynb) that demonstrates the usage of AutoMLOps. Upon running `AutoMLOps.go(project_id='automlops-sandbox',pipeline_params=pipeline_params)`, a series of directories will be generated automatically, and a pipelineJob will be submitted using the setup below:
+Included in the repository is an [example notebook](./examples/training/00_training_example.ipynb) that demonstrates the usage of AutoMLOps. Upon running `AutoMLOps.go(project_id='automlops-sandbox',pipeline_params=pipeline_params)`, a series of directories will be generated automatically, and a pipelineJob will be submitted using the setup below:
 
 ```bash
 .
 ├── cloud_run                                      : Cloud Runner service for submitting PipelineJobs.
     ├──run_pipeline                                : Contains main.py file, Dockerfile and requirements.txt
     ├──queueing_svc                                : Contains files for scheduling and queueing jobs to runner service
 ├── components                                     : Custom vertex pipeline components.
@@ -209,15 +224,15 @@
 
 <p align="center">
     <img src="./CICD.png" alt="CICD" width="1000"/>
 </p>
 
 # Pipeline Components
 
-The [example notebook](example/automlops_example_notebook.ipynb) comes with 3 components as part of the pipeline. Additional sample code for commonly used services can be found below:
+The [example notebook](./examples/training/00_training_example.ipynb) comes with 3 components as part of the pipeline. Additional sample code for commonly used services can be found below:
 
 - [Feature Store](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/feature_store)
 - [BigQuery ML](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/bigquery_ml)
 - [Model Registry](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/model_registry)
 - [Experiments](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/experiments)
 - [ExplainableAI](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/explainable_ai)
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/notebooks)
```

### Comparing `google-cloud-automlops-1.0.5/README.md` & `google-cloud-automlops-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 AutoMLOps is a service that generates a production ready MLOps pipeline from Jupyter Notebooks, bridging the gap between Data Science and DevOps and accelerating the adoption and use of Vertex AI. The service generates an MLOps codebase for users to customize, and provides a way to build and manage a CI/CD integrated MLOps pipeline from the notebook. AutoMLOps automatically builds a source repo for versioning, cloudbuild configs and triggers, an artifact registry for storing custom components, gs buckets, service accounts and updated IAM privs for running pipelines, enables APIs (cloud Run, Cloud Build, Artifact Registry, etc.), creates a runner service API in Cloud Run for submitting PipelineJobs to Vertex AI, and a Cloud Scheduler job for submitting PipelineJobs on a recurring basis. These automatic integrations empower data scientists to take their experiments to production more quickly, allowing them to focus on what they do best: providing actionable insights through data.
 
 # Prerequisites
 
 In order to use AutoMLOps, the following are required:
 
-- Jupyter (or Jupyter-compatible) notebook environment
-- [Notebooks API](https://console.cloud.google.com/marketplace/product/google/notebooks.googleapis.com) enabled
 - Python 3.7 - 3.10
 - [Google Cloud SDK 407.0.0](https://cloud.google.com/sdk/gcloud/reference)
 - [beta 2022.10.21](https://cloud.google.com/sdk/gcloud/reference/beta)
 - `git` installed
 - `git` logged-in:
 ```
   git config --global user.email "you@example.com"
@@ -26,19 +24,17 @@
 # Install
 
 Install AutoMLOps from [PyPI](https://pypi.org/project/google-cloud-automlops/): `pip install google-cloud-automlops` 
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
-- `autoflake==2.0.0`,
 - `docopt==0.6.2`,
-- `ipython==7.34.0`,
+- `docstring-parser==0.15`,
 - `pipreqs==0.4.11`,
-- `pyflakes==3.0.1`,
 - `PyYAML==5.4.1`,
 - `yarg==0.1.9`
 
 # GCP Services
 AutoMLOps makes use of the following products by default:
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction)
 - [Artifact Registry](https://cloud.google.com/artifact-registry/docs/overview)
@@ -147,18 +143,37 @@
 **Use a VPC connector:**
 
 Use the `vpc_connector` parameter to specify a vpc connector. 
 ```
 vpc_connector = 'example-vpc'
 ```
 
+**Specify package versions:**
+
+Use the `packages_to_install` parameter of `@AutoMLOps.component` to explicitly specify packages and versions. 
+```
+@AutoMLOps.component(
+    packages_to_install=[
+        "google-cloud-bigquery==2.34.4", 
+        "pandas",
+        "pyarrow",
+        "db_dtypes"
+    ]
+)
+def create_dataset(
+    bq_table: str,
+    data_path: str,
+    project_id: str
+):
+...
+```
 
 # Layout
 
-Included in the repository is an [example notebook](./example/automlops_example_notebook.ipynb) that demonstrates the usage of AutoMLOps. Upon running `AutoMLOps.go(project_id='automlops-sandbox',pipeline_params=pipeline_params)`, a series of directories will be generated automatically, and a pipelineJob will be submitted using the setup below:
+Included in the repository is an [example notebook](./examples/training/00_training_example.ipynb) that demonstrates the usage of AutoMLOps. Upon running `AutoMLOps.go(project_id='automlops-sandbox',pipeline_params=pipeline_params)`, a series of directories will be generated automatically, and a pipelineJob will be submitted using the setup below:
 
 ```bash
 .
 ├── cloud_run                                      : Cloud Runner service for submitting PipelineJobs.
     ├──run_pipeline                                : Contains main.py file, Dockerfile and requirements.txt
     ├──queueing_svc                                : Contains files for scheduling and queueing jobs to runner service
 ├── components                                     : Custom vertex pipeline components.
@@ -188,15 +203,15 @@
 
 <p align="center">
     <img src="./CICD.png" alt="CICD" width="1000"/>
 </p>
 
 # Pipeline Components
 
-The [example notebook](example/automlops_example_notebook.ipynb) comes with 3 components as part of the pipeline. Additional sample code for commonly used services can be found below:
+The [example notebook](./examples/training/00_training_example.ipynb) comes with 3 components as part of the pipeline. Additional sample code for commonly used services can be found below:
 
 - [Feature Store](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/feature_store)
 - [BigQuery ML](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/bigquery_ml)
 - [Model Registry](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/model_registry)
 - [Experiments](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/experiments)
 - [ExplainableAI](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/explainable_ai)
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/notebooks)
```

### Comparing `google-cloud-automlops-1.0.5/google_cloud_automlops.egg-info/PKG-INFO` & `google-cloud-automlops-1.1.0/google_cloud_automlops.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-automlops
-Version: 1.0.5
+Version: 1.1.0
 Summary: AutoMLOps is a service that generates a production-style         MLOps pipeline from Jupyter Notebooks.
 Home-page: https://github.com/GoogleCloudPlatform/automlops
 Author: Sean Rastatter
 Author-email: srastatter@google.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,16 +23,14 @@
 
 AutoMLOps is a service that generates a production ready MLOps pipeline from Jupyter Notebooks, bridging the gap between Data Science and DevOps and accelerating the adoption and use of Vertex AI. The service generates an MLOps codebase for users to customize, and provides a way to build and manage a CI/CD integrated MLOps pipeline from the notebook. AutoMLOps automatically builds a source repo for versioning, cloudbuild configs and triggers, an artifact registry for storing custom components, gs buckets, service accounts and updated IAM privs for running pipelines, enables APIs (cloud Run, Cloud Build, Artifact Registry, etc.), creates a runner service API in Cloud Run for submitting PipelineJobs to Vertex AI, and a Cloud Scheduler job for submitting PipelineJobs on a recurring basis. These automatic integrations empower data scientists to take their experiments to production more quickly, allowing them to focus on what they do best: providing actionable insights through data.
 
 # Prerequisites
 
 In order to use AutoMLOps, the following are required:
 
-- Jupyter (or Jupyter-compatible) notebook environment
-- [Notebooks API](https://console.cloud.google.com/marketplace/product/google/notebooks.googleapis.com) enabled
 - Python 3.7 - 3.10
 - [Google Cloud SDK 407.0.0](https://cloud.google.com/sdk/gcloud/reference)
 - [beta 2022.10.21](https://cloud.google.com/sdk/gcloud/reference/beta)
 - `git` installed
 - `git` logged-in:
 ```
   git config --global user.email "you@example.com"
@@ -47,19 +45,17 @@
 # Install
 
 Install AutoMLOps from [PyPI](https://pypi.org/project/google-cloud-automlops/): `pip install google-cloud-automlops` 
 
 Or Install locally by cloning the repo and running `pip install .`
 
 # Dependencies
-- `autoflake==2.0.0`,
 - `docopt==0.6.2`,
-- `ipython==7.34.0`,
+- `docstring-parser==0.15`,
 - `pipreqs==0.4.11`,
-- `pyflakes==3.0.1`,
 - `PyYAML==5.4.1`,
 - `yarg==0.1.9`
 
 # GCP Services
 AutoMLOps makes use of the following products by default:
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction)
 - [Artifact Registry](https://cloud.google.com/artifact-registry/docs/overview)
@@ -168,18 +164,37 @@
 **Use a VPC connector:**
 
 Use the `vpc_connector` parameter to specify a vpc connector. 
 ```
 vpc_connector = 'example-vpc'
 ```
 
+**Specify package versions:**
+
+Use the `packages_to_install` parameter of `@AutoMLOps.component` to explicitly specify packages and versions. 
+```
+@AutoMLOps.component(
+    packages_to_install=[
+        "google-cloud-bigquery==2.34.4", 
+        "pandas",
+        "pyarrow",
+        "db_dtypes"
+    ]
+)
+def create_dataset(
+    bq_table: str,
+    data_path: str,
+    project_id: str
+):
+...
+```
 
 # Layout
 
-Included in the repository is an [example notebook](./example/automlops_example_notebook.ipynb) that demonstrates the usage of AutoMLOps. Upon running `AutoMLOps.go(project_id='automlops-sandbox',pipeline_params=pipeline_params)`, a series of directories will be generated automatically, and a pipelineJob will be submitted using the setup below:
+Included in the repository is an [example notebook](./examples/training/00_training_example.ipynb) that demonstrates the usage of AutoMLOps. Upon running `AutoMLOps.go(project_id='automlops-sandbox',pipeline_params=pipeline_params)`, a series of directories will be generated automatically, and a pipelineJob will be submitted using the setup below:
 
 ```bash
 .
 ├── cloud_run                                      : Cloud Runner service for submitting PipelineJobs.
     ├──run_pipeline                                : Contains main.py file, Dockerfile and requirements.txt
     ├──queueing_svc                                : Contains files for scheduling and queueing jobs to runner service
 ├── components                                     : Custom vertex pipeline components.
@@ -209,15 +224,15 @@
 
 <p align="center">
     <img src="./CICD.png" alt="CICD" width="1000"/>
 </p>
 
 # Pipeline Components
 
-The [example notebook](example/automlops_example_notebook.ipynb) comes with 3 components as part of the pipeline. Additional sample code for commonly used services can be found below:
+The [example notebook](./examples/training/00_training_example.ipynb) comes with 3 components as part of the pipeline. Additional sample code for commonly used services can be found below:
 
 - [Feature Store](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/feature_store)
 - [BigQuery ML](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/bigquery_ml)
 - [Model Registry](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/model_registry)
 - [Experiments](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/experiments)
 - [ExplainableAI](https://github.com/GoogleCloudPlatform/vertex-ai-samples/tree/main/notebooks/official/explainable_ai)
 - [Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/notebooks)
```

### Comparing `google-cloud-automlops-1.0.5/setup.py` & `google-cloud-automlops-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as file:
     readme_contents = file.read()
 
 setup(
     name='google-cloud-automlops',
-    version='1.0.5',
+    version='1.1.0',
     description='AutoMLOps is a service that generates a production-style \
         MLOps pipeline from Jupyter Notebooks.',
     long_description=readme_contents,
     long_description_content_type='text/markdown',
     url='https://github.com/GoogleCloudPlatform/automlops',
     author='Sean Rastatter',
     author_email='srastatter@google.com',
     license='Apache-2.0',
     packages=['AutoMLOps'],
-    install_requires=['autoflake==2.0.0',
-                      'docopt==0.6.2',
-                      'ipython==7.34.0',
+    install_requires=['docopt==0.6.2',
+                      'docstring-parser==0.15',
                       'pipreqs==0.4.11',
-                      'pyflakes==3.0.1',
                       'PyYAML==5.4.1',
                       'yarg==0.1.9'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
```

