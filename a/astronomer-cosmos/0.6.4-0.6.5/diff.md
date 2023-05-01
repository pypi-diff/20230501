# Comparing `tmp/astronomer_cosmos-0.6.4.tar.gz` & `tmp/astronomer_cosmos-0.6.5.tar.gz`

## Comparing `astronomer_cosmos-0.6.4.tar` & `astronomer_cosmos-0.6.5.tar`

### file list

```diff
@@ -1,52 +1,55 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/core/tests/test_airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/__init__.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/constants.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/dag.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/dataset.py
--rw-r--r--   0        0        0    10099 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/render.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/__init__.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/exasol.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/spark.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/trino.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/__init__.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/base.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/docker.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/lazy_load.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/local.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_docker.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_local.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/bigquery.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/databricks.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/postgres.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/redshift.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/snowflake.py
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/profiles_generator.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/__init__.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/project.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/tests/test_project.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_dataset.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_export.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_render.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/cosmos/tests/test_version.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/LICENSE
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/README.rst
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     6665 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/core/tests/test_airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/__init__.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/constants.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/dag.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/dataset.py
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/render.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/__init__.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/exasol.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/spark.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/trino.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/__init__.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/base.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/docker.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/lazy_load.py
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/local.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_docker.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_local.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/bigquery.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/databricks.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/postgres.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/redshift.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/snowflake.py
+-rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/tests/test_profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/__init__.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/adapted_subprocesshook.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/data_aware_scheduling.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/profiles_generator.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/warn_parsing.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_warn_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/project.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/tests/test_project.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_dataset.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_export.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_render.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/cosmos/tests/test_version.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/LICENSE
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/README.rst
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 astronomer_cosmos-0.6.5/PKG-INFO
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/core/airflow.py` & `astronomer_cosmos-0.6.5/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.6.5/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/core/tests/test_airflow.py` & `astronomer_cosmos-0.6.5/cosmos/core/tests/test_airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/__init__.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/dag.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains a function to render a dbt project as an Airflow DAG.
 """
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-from typing import Any, Dict, List
+from typing import Any, Callable, Dict, List, Optional
 
 from cosmos.core.airflow import CosmosDag
 
 from .render import render_project
 
 
 class DbtDag(CosmosDag):
@@ -30,14 +30,16 @@
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param execution_mode: The execution mode in which the dbt project should be run.
         Options are "local", "docker", and "kubernetes".
         Defaults to "local"
+    :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
+        and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         dbt_args: Dict[str, Any] = {},
@@ -46,14 +48,15 @@
         dbt_root_path: str = "/usr/local/airflow/dags/dbt",
         dbt_models_dir: str = "models",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
         execution_mode: Literal["local", "docker", "kubernetes"] = "local",
+        on_warning_callback: Optional[Callable] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         # add additional args to the dbt_args
         dbt_args = {
             **dbt_args,
             "conn_id": conn_id,
@@ -69,11 +72,12 @@
             operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
             select=select,
             exclude=exclude,
             execution_mode=execution_mode,
+            on_warning_callback=on_warning_callback,
         )
 
         # call the airflow DAG constructor
         super().__init__(group, *args, **kwargs)
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/render.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-from typing import Any, Dict, List
+from typing import Any, Callable, Dict, List, Optional
 
 from airflow.exceptions import AirflowException
 
 from cosmos.core.graph.entities import CosmosEntity, Group, Task
 from cosmos.providers.dbt.core.utils.data_aware_scheduling import get_dbt_dataset
 from cosmos.providers.dbt.parser.project import DbtModelType, DbtProject
 
@@ -37,14 +37,15 @@
     operator_args: Dict[str, Any] = {},
     test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
     emit_datasets: bool = True,
     conn_id: str = "default_conn_id",
     select: Dict[str, List[str]] = {},
     exclude: Dict[str, List[str]] = {},
     execution_mode: Literal["local", "docker", "kubernetes"] = "local",
+    on_warning_callback: Optional[Callable] = None,
 ) -> Group:
     """
     Turn a dbt project into a Group
 
     :param dbt_project_name: The name of the dbt project
     :param dbt_root_path: The root path to your dbt folder. Defaults to /usr/local/airflow/dags/dbt
     :param task_args: Arguments to pass to the underlying dbt operators
@@ -55,14 +56,16 @@
     :param emit_datasets: If enabled test nodes emit Airflow Datasets for downstream cross-DAG dependencies
     :param conn_id: The Airflow connection ID to use in Airflow Datasets
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2]}})
     :param execution_mode: The execution mode in which the dbt project should be run.
         Options are "local", "docker", and "kubernetes".
         Defaults to "local"
+     :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
+        and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
     # first, get the dbt project
     project = DbtProject(
         dbt_root_path=dbt_root_path,
         dbt_models_dir=dbt_models_dir,
         dbt_snapshots_dir=dbt_snapshots_dir,
         dbt_seeds_dir=dbt_seeds_dir,
@@ -123,15 +126,16 @@
         if "configs" in exclude:
             # TODO: coverme
             if set(exclude["configs"]).intersection(model.config.config_selectors):
                 continue
 
         run_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
         test_args: Dict[str, Any] = {**task_args, **operator_args, "models": model_name}
-
+        # DbtTestOperator specific arg
+        test_args["on_warning_callback"] = on_warning_callback
         if emit_datasets:
             outlets = [get_dbt_dataset(conn_id, dbt_project_name, model_name)]
 
             if test_behavior == "after_each":
                 test_args["outlets"] = outlets
             else:
                 # TODO: coverme
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/task_group.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/task_group.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains a function to render a dbt project as an Airflow Task Group.
 """
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
-from typing import Any, Dict, List
+from typing import Any, Callable, Dict, List, Optional
 
 from cosmos.core.airflow import CosmosTaskGroup
 
 from .render import render_project
 
 
 class DbtTaskGroup(CosmosTaskGroup):
@@ -31,14 +31,16 @@
     :param test_behavior: The behavior for running tests. Options are "none", "after_each", and "after_all".
         Defaults to "after_each"
     :param select: A dict of dbt selector arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param exclude: A dict of dbt exclude arguments (i.e., {"tags": ["tag_1", "tag_2"]})
     :param execution_mode: The execution mode in which the dbt project should be run.
         Options are "local", "docker", and "kubernetes".
         Defaults to "local"
+    :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
+        and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     def __init__(
         self,
         dbt_project_name: str,
         conn_id: str,
         dbt_args: Dict[str, Any] = {},
@@ -48,14 +50,15 @@
         dbt_models_dir: str = "models",
         dbt_snapshots_dir: str = "snapshots",
         dbt_seeds_dir: str = "seeds",
         test_behavior: Literal["none", "after_each", "after_all"] = "after_each",
         select: Dict[str, List[str]] = {},
         exclude: Dict[str, List[str]] = {},
         execution_mode: Literal["local", "docker", "kubernetes"] = "local",
+        on_warning_callback: Optional[Callable] = None,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         # add additional args to the dbt_args
         dbt_args = {
             **dbt_args,
             "conn_id": conn_id,
@@ -72,11 +75,12 @@
             operator_args=operator_args,
             test_behavior=test_behavior,
             emit_datasets=emit_datasets,
             conn_id=conn_id,
             select=select,
             exclude=exclude,
             execution_mode=execution_mode,
+            on_warning_callback=on_warning_callback,
         )
 
         # call the airflow constructor
         super().__init__(group, *args, **kwargs)
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/exasol.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/exasol.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/spark.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/spark.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/community/profiles/trino.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/community/profiles/trino.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/__init__.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/base.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/docker.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import Sequence
+from typing import Callable, Optional, Sequence
 
 import yaml
 from airflow.utils.context import Context
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
 
 logger = logging.getLogger(__name__)
@@ -133,17 +133,21 @@
 class DbtTestDockerOperator(DbtDockerBaseOperator):
     """
     Executes a dbt core test command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(
+        self, on_warning_callback: Optional[Callable] = None, **kwargs
+    ) -> None:
         super().__init__(**kwargs)
         self.base_cmd = "test"
+        # as of now, on_warning_callback in docker executor does nothing
+        self.on_warning_callback = on_warning_callback
 
     def execute(self, context: Context):
         return self.build_and_run_cmd(context=context)
 
 
 class DbtRunOperationDockerOperator(DbtDockerBaseOperator):
     """
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/kubernetes.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import Sequence
+from typing import Callable, Optional, Sequence
 
 import yaml
 from airflow.utils.context import Context
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
 
 logger = logging.getLogger(__name__)
@@ -143,17 +143,21 @@
 class DbtTestKubernetesOperator(DbtKubernetesBaseOperator):
     """
     Executes a dbt core test command.
     """
 
     ui_color = "#8194E0"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(
+        self, on_warning_callback: Optional[Callable] = None, **kwargs
+    ) -> None:
         super().__init__(**kwargs)
         self.base_cmd = "test"
+        # as of now, on_warning_callback in kubernetes executor does nothing
+        self.on_warning_callback = on_warning_callback
 
     def execute(self, context: Context):
         return self.build_and_run_cmd(context=context)
 
 
 class DbtRunOperationKubernetesOperator(DbtKubernetesBaseOperator):
     """
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/local.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/local.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 import signal
 import tempfile
-from typing import Sequence
+from collections import namedtuple
+from typing import Callable, Optional, Sequence
 
 import yaml
 from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowSkipException
-from airflow.hooks.subprocess import SubprocessHook, SubprocessResult
 from airflow.utils.context import Context
 
 from cosmos.providers.dbt.core.operators.base import DbtBaseOperator
+from cosmos.providers.dbt.core.utils.adapted_subprocesshook import (
+    FullOutputSubprocessHook,
+)
+from cosmos.providers.dbt.core.utils.warn_parsing import (
+    extract_log_issues,
+    parse_output,
+)
 
 logger = logging.getLogger(__name__)
 
+FullOutputSubprocessResult = namedtuple(
+    "FullOutputSubprocessResult", ["exit_code", "output", "full_output"]
+)
+
 
 class DbtLocalBaseOperator(DbtBaseOperator):
     """
     Executes a dbt core cli command locally.
 
     :param install_deps: If true, install dependencies before running the command
     """
@@ -34,31 +45,31 @@
     ) -> None:
         self.install_deps = install_deps
         super().__init__(**kwargs)
 
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
-        return SubprocessHook()
+        return FullOutputSubprocessHook()
 
-    def exception_handling(self, result: SubprocessResult):
+    def exception_handling(self, result: FullOutputSubprocessResult):
         if self.skip_exit_code is not None and result.exit_code == self.skip_exit_code:
             raise AirflowSkipException(
                 f"dbt command returned exit code {self.skip_exit_code}. Skipping."
             )
         elif result.exit_code != 0:
             raise AirflowException(
                 f"dbt command failed. The command returned a non-zero exit code {result.exit_code}."
             )
 
     def run_command(
         self,
         cmd: list[str],
         env: dict[str, str],
-    ) -> SubprocessResult:
+    ) -> FullOutputSubprocessResult:
         """
         Copies the dbt project to a temporary directory and runs the command.
         """
         with tempfile.TemporaryDirectory() as tmp_dir:
             # need a subfolder because shutil.copytree will fail if the destination dir already exists
             tmp_project_dir = os.path.join(tmp_dir, "dbt_project")
             shutil.copytree(
@@ -84,15 +95,15 @@
 
             self.exception_handling(result)
 
             return result
 
     def build_and_run_cmd(
         self, context: Context, cmd_flags: list[str] | None = None
-    ) -> SubprocessResult:
+    ) -> FullOutputSubprocessResult:
         dbt_cmd, env = self.build_cmd(context=context, cmd_flags=cmd_flags)
         return self.run_command(cmd=dbt_cmd, env=env)
 
     def execute(self, context: Context) -> str:
         # TODO is this going to put loads of unnecessary stuff in to xcom?
         return self.build_and_run_cmd(context=context).output
 
@@ -185,24 +196,71 @@
         result = self.build_and_run_cmd(context=context)
         return result.output
 
 
 class DbtTestLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core test command.
+    :param on_warning_callback: A callback function called on warnings with additional Context variables "test_names"
+        and "test_results" of type `List`. Each index in "test_names" corresponds to the same index in "test_results".
     """
 
     ui_color = "#8194E0"
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(
+        self,
+        on_warning_callback: Optional[Callable] = None,
+        **kwargs,
+    ) -> None:
         super().__init__(**kwargs)
         self.base_cmd = "test"
+        self.on_warning_callback = on_warning_callback
+
+    def _should_run_tests(
+        self,
+        result: FullOutputSubprocessResult,
+        no_tests_message: str = "Nothing to do",
+    ) -> bool:
+        """
+        Check if any tests are defined to run in the DAG. If tests are defined
+        and on_warning_callback is set, then function returns True.
+
+        :param result: The output from the build and run command.
+        """
+
+        return self.on_warning_callback and no_tests_message not in result.output
+
+    def _handle_warnings(
+        self, result: FullOutputSubprocessResult, context: Context
+    ) -> None:
+        """
+         Handles warnings by extracting log issues, creating additional context, and calling the
+         on_warning_callback with the updated context.
+
+        :param result: The result object from the build and run command.
+        :param context: The original airflow context in which the build and run command was executed.
+        """
+        test_names, test_results = extract_log_issues(result.full_output)
+
+        warning_context = dict(context)
+        warning_context["test_names"] = test_names
+        warning_context["test_results"] = test_results
+
+        self.on_warning_callback(warning_context)
 
     def execute(self, context: Context):
         result = self.build_and_run_cmd(context=context)
+
+        if not self._should_run_tests(result):
+            return result.output
+
+        warnings = parse_output(result, "WARN")
+        if warnings > 0:
+            self._handle_warnings(result, context)
+
         return result.output
 
 
 class DbtRunOperationLocalOperator(DbtLocalBaseOperator):
     """
     Executes a dbt core run-operation command.
```

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_docker.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/operators/tests/test_local.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/operators/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/__init__.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/bigquery.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/databricks.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/postgres.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/postgres.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/redshift.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/redshift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/snowflake.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/profiles/tests/test_profiles.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/profiles/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/profiles_generator.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/profiles_generator.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/core/utils/tests/test_data_aware_scheduling.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/project.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/parser/tests/test_project.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_dataset.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_export.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/cosmos/providers/dbt/tests/test_render.py` & `astronomer_cosmos-0.6.5/cosmos/providers/dbt/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/.gitignore` & `astronomer_cosmos-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/LICENSE` & `astronomer_cosmos-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/README.rst` & `astronomer_cosmos-0.6.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/astronomer/astronomer-cosmos/main.svg
    :target: https://results.pre-commit.ci/latest/github/astronomer/astronomer-cosmos/main
    :alt: pre-commit.ci status
 
 
 
-.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/cosmos-logo.svg
+.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/_static/cosmos-logo.svg
 
 
 ===========================================================
 
 |fury| |ossrank| |downloads| |pre-commit|
 
 Run your dbt Core projects as `Apache Airflow <https://airflow.apache.org/>`_ DAGs and Task Groups with a few lines of code. Benefits include:
```

### Comparing `astronomer_cosmos-0.6.4/pyproject.toml` & `astronomer_cosmos-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.6.4/PKG-INFO` & `astronomer_cosmos-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.6.4
+Version: 0.6.5
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -86,15 +86,15 @@
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/astronomer/astronomer-cosmos/main.svg
    :target: https://results.pre-commit.ci/latest/github/astronomer/astronomer-cosmos/main
    :alt: pre-commit.ci status
 
 
 
-.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/cosmos-logo.svg
+.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/_static/cosmos-logo.svg
 
 
 ===========================================================
 
 |fury| |ossrank| |downloads| |pre-commit|
 
 Run your dbt Core projects as `Apache Airflow <https://airflow.apache.org/>`_ DAGs and Task Groups with a few lines of code. Benefits include:
```

