# Comparing `tmp/pDESy-0.4.9.tar.gz` & `tmp/pDESy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pDESy-0.4.9.tar", max compression
+gzip compressed data, was "pDESy-0.5.0.tar", max compression
```

## Comparing `pDESy-0.4.9.tar` & `pDESy-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,19 @@
--rw-r--r--   0        0        0     1071 2022-07-12 06:34:46.069426 pDESy-0.4.9/LICENSE
--rw-r--r--   0        0        0     1931 2022-07-12 06:34:46.069426 pDESy-0.4.9/README.md
--rw-r--r--   0        0        0       85 2022-07-29 08:57:44.549688 pDESy-0.4.9/pDESy/__init__.py
--rw-r--r--   0        0        0       62 2022-07-12 06:34:46.069426 pDESy-0.4.9/pDESy/model/__init__.py
--rw-r--r--   0        0        0    21702 2022-07-21 08:45:29.633647 pDESy-0.4.9/pDESy/model/base_component.py
--rw-r--r--   0        0        0    16468 2022-07-21 08:30:11.532761 pDESy-0.4.9/pDESy/model/base_facility.py
--rw-r--r--   0        0        0    56754 2022-07-21 08:30:11.532761 pDESy-0.4.9/pDESy/model/base_organization.py
--rw-r--r--   0        0        0     6612 2022-07-12 06:34:46.073426 pDESy-0.4.9/pDESy/model/base_priority_rule.py
--rw-r--r--   0        0        0    31459 2022-07-29 07:23:24.958392 pDESy-0.4.9/pDESy/model/base_product.py
--rw-r--r--   0        0        0    77268 2022-07-29 08:57:45.821695 pDESy-0.4.9/pDESy/model/base_project.py
--rw-r--r--   0        0        0    15163 2022-07-21 08:45:29.633647 pDESy-0.4.9/pDESy/model/base_resource.py
--rw-r--r--   0        0        0    32461 2022-07-21 08:45:29.633647 pDESy-0.4.9/pDESy/model/base_task.py
--rw-r--r--   0        0        0    32413 2022-07-21 08:30:11.536761 pDESy-0.4.9/pDESy/model/base_team.py
--rw-r--r--   0        0        0     6151 2022-07-21 08:45:29.633647 pDESy-0.4.9/pDESy/model/base_worker.py
--rw-r--r--   0        0        0    52284 2022-07-29 07:05:36.780585 pDESy-0.4.9/pDESy/model/base_workflow.py
--rw-r--r--   0        0        0    40407 2022-07-21 08:30:11.536761 pDESy-0.4.9/pDESy/model/base_workplace.py
--rw-r--r--   0        0        0     3796 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/component.py
--rw-r--r--   0        0        0     1035 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/organization.py
--rw-r--r--   0        0        0      551 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/product.py
--rw-r--r--   0        0        0    19251 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/project.py
--rw-r--r--   0        0        0    10816 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/task.py
--rw-r--r--   0        0        0     1586 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/team.py
--rw-r--r--   0        0        0     5213 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/worker.py
--rw-r--r--   0        0        0     1648 2022-07-21 08:45:29.637647 pDESy-0.4.9/pDESy/model/workflow.py
--rw-r--r--   0        0        0     1123 2022-07-29 08:57:44.157686 pDESy-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     2923 2022-07-29 09:06:59.980044 pDESy-0.4.9/setup.py
--rw-r--r--   0        0        0     3010 2022-07-29 09:06:59.980307 pDESy-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:35:41.240517 pDESy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1930 2023-04-30 23:35:41.240517 pDESy-0.5.0/README.md
+-rw-r--r--   0        0        0       85 2023-04-30 23:35:41.240517 pDESy-0.5.0/pDESy/__init__.py
+-rw-r--r--   0        0        0       62 2022-07-12 06:34:46.069426 pDESy-0.5.0/pDESy/model/__init__.py
+-rw-r--r--   0        0        0    23875 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_component.py
+-rw-r--r--   0        0        0    16574 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_facility.py
+-rw-r--r--   0        0        0    57975 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_organization.py
+-rw-r--r--   0        0        0     9224 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_priority_rule.py
+-rw-r--r--   0        0        0    31417 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_product.py
+-rw-r--r--   0        0        0    87964 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_project.py
+-rw-r--r--   0        0        0     7063 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_subproject_task.py
+-rw-r--r--   0        0        0    35480 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_task.py
+-rw-r--r--   0        0        0    32536 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_team.py
+-rw-r--r--   0        0        0    19968 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_worker.py
+-rw-r--r--   0        0        0    59279 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_workflow.py
+-rw-r--r--   0        0        0    40514 2023-04-30 23:35:41.244517 pDESy-0.5.0/pDESy/model/base_workplace.py
+-rw-r--r--   0        0        0     1103 2023-04-30 23:35:41.244517 pDESy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2895 2023-04-30 23:51:31.147988 pDESy-0.5.0/setup.py
+-rw-r--r--   0        0        0     2968 2023-04-30 23:51:31.148328 pDESy-0.5.0/PKG-INFO
```

### Comparing `pDESy-0.4.9/LICENSE` & `pDESy-0.5.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 MITSUYUKI Taiga
+Copyright (c) 2023 MITSUYUKI Taiga
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pDESy-0.4.9/README.md` & `pDESy-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pDESy: Discrete-Event Simulator in Python
 
-[![PyPi version](https://pypip.in/v/pDESy/badge.png)](https://pypi.org/project/pDESy/)
+[![PyPI version](https://badge.fury.io/py/pDESy.svg)](https://badge.fury.io/py/pDESy)
 [![Anaconda-Server Badge](https://anaconda.org/taiga4112/pdesy/badges/version.svg)](https://anaconda.org/taiga4112/pdesy)
 ![test](https://github.com/pDESy/pDESy/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/pDESy/pDESy/branch/master/graph/badge.svg)](https://codecov.io/gh/pDESy/pDESy)
 
 ## What is it?
 
 **pDESy** is a Python package of Discrete-Event Simulator (DES). It aims to be the fundamental high-level building block for doing practical, real world engineering project management by using DES and other DES modeling tools. **pDESy** has only the function of discrete-event simulation, does not include the function of visual modeling.
```

### Comparing `pDESy-0.4.9/pDESy/model/base_component.py` & `pDESy-0.5.0/pDESy/model/base_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """base_component."""
 
 import abc
 import datetime
 import uuid
 from enum import IntEnum
 
+import numpy as np
+
 from .base_task import BaseTaskState
 
 
 class BaseComponentState(IntEnum):
     """BaseComponentState."""
 
     NONE = 0
@@ -23,17 +25,18 @@
 class BaseComponent(object, metaclass=abc.ABCMeta):
     """BaseComponent.
 
     BaseComponent class for expressing target product.
     This class can be used as template.
 
     Args:
-        name (str):
+        name (str, optional):
             Basic parameter.
             Name of this component.
+            Defaults to None -> "New Component"
         ID (str, optional):
             Basic parameter.
             ID will be defined automatically.
         parent_component_list(List[BaseComponent], optional):
             Basic parameter.
             List of parent BaseComponents.
             Defaults to None -> [].
@@ -45,14 +48,18 @@
             Basic parameter.
             List of targeted tasks.
             Defaults to None -> [].
         space_size (float, optional):
             Basic parameter.
             Space size related to base_workplace's max_space_size.
             Default to None -> 1.0.
+        parent_product(BaseProduct, optional):
+            Basic parameter.
+            Parent product.
+            Defaults to None.
         state (BaseComponentState, optional):
             Basic variable.
             State of this task in simulation.
             Defaults to BaseComponentState.NONE.
         state_record_list (List[BaseComponentState], optional):
             Basic variable.
             Record list of state.
@@ -61,37 +68,46 @@
             Basic variable.
             A workplace which this componetnt is placed in simulation.
             Defaults to None.
         placed_workplace_id_record (List[str], optional):
             Basic variable.
             Record of placed workplace ID in simulation.
             Defaults to None -> [].
+        error_tolerance (float, optional):
+            Advanced parameter.
+        error (float, optional):
+            Advanced variables.
     """
 
     def __init__(
         self,
         # Basic parameters
-        name: str,
+        name=None,
         ID=None,
         parent_component_list=None,
         child_component_list=None,
         targeted_task_list=None,
         space_size=None,
+        parent_product=None,
         # Basic variables
         state=BaseComponentState.NONE,
         state_record_list=None,
         placed_workplace=None,
         placed_workplace_id_record=None,
+        # Advanced parameters for customized simulation
+        error_tolerance=None,
+        # Advanced variables for customized simulation
+        error=None,
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.name = name
+        self.name = name if name is not None else "New Component"
         self.ID = ID if ID is not None else str(uuid.uuid4())
 
         if parent_component_list is not None:
             self.parent_component_list = parent_component_list
         else:
             self.parent_component_list = []
 
@@ -106,14 +122,16 @@
             self.targeted_task_list = []
 
         if space_size is not None:
             self.space_size = space_size
         else:
             self.space_size = 1.0
 
+        self.parent_product = parent_product if parent_product is not None else None
+
         if state is not BaseComponentState.NONE:
             self.state = state
         else:
             self.state = BaseComponentState.NONE
 
         if state_record_list is not None:
             self.state_record_list = state_record_list
@@ -126,14 +144,26 @@
             self.placed_workplace = None
 
         if placed_workplace_id_record is not None:
             self.placed_workplace_id_record = placed_workplace_id_record
         else:
             self.placed_workplace_id_record = []
 
+        # --
+        # Advanced parameter for customized simulation
+        if error_tolerance is not None:
+            self.error_tolerance = error_tolerance
+        else:
+            self.error_tolerance = 0.0
+        # Advanced variables for customized simulation
+        if error is not None:
+            self.error = error
+        else:
+            self.error = 0.0
+
     def extend_child_component_list(self, child_component_list):
         """
         Extend the list of child components.
 
         Args:
             child_component_list (List[BaseComponent]):
                 List of BaseComponents which are children of this component.
@@ -164,14 +194,15 @@
             >>> print([child_c.name for child_c in c.child_component_list])
             ['c1']
             >>> print([parent_c.name for parent_c in c1.parent_component_list])
             ['c']
         """
         self.child_component_list.append(child_component)
         child_component.parent_component_list.append(self)
+        child_component.parent_product = self.parent_product
 
     def set_placed_workplace(self, placed_workplace, set_to_all_children=True):
         """
         Set the `placed_workplace`.
 
         Args:
             placed_workplace (BaseWorkplace):
@@ -268,14 +299,16 @@
         """
         Initialize the following changeable basic variables of BaseComponent.
 
         If `state_info` is True, the following attributes are initialized.
 
           - `state`
           - `placed_workplace`
+          - `error`
+
 
         If `log_info` is True, the following attributes are initialized.
 
           - `state_record_list`
           - `placed_workplace_id_record`
 
         Args:
@@ -292,18 +325,47 @@
         if log_info:
             self.state_record_list = []
             self.placed_workplace_id_record = []
 
         if state_info:
             self.state = BaseComponentState.NONE
             self.placed_workplace = None
+            self.error = 0.0
 
             if check_task_state:
                 self.check_state()
 
+    def update_error_value(
+        self, no_error_prob: float, error_increment: float, seed=None
+    ):
+        """
+        Update error value randomly.
+
+        If no_error_prob >=1.0, error = error + error_increment.
+
+        Args:
+            no_error_prob (float): Probability of no error (0.0~1.0)
+            error_increment (float): Increment of error variables if error has occurred.
+            seed (int, optional): seed of creating random.rand(). Defaults to None.
+        Examples:
+            >>> c = Component("c")
+            >>> c.update_error_value(0.9, 1.0, seed=32)
+            >>> print(c.error)
+            0.0
+            >>> c.update_error_value(0.4, 1.0, seed=32)
+            >>> print(c.error) # Random 1.0 or 0.0
+            1.0
+        Note:
+            This method is developed for customized simulation.
+        """
+        if seed is not None:
+            np.random.seed(seed=seed)
+        if np.random.rand() > no_error_prob:
+            self.error = self.error + error_increment
+
     def reverse_log_information(self):
         """Reverse log information of all."""
         self.state_record_list = self.state_record_list[::-1]
         self.placed_workplace_id_record = self.placed_workplace_id_record[::-1]
 
     def check_state(self):
         """Check and update the `state` of this component."""
@@ -467,15 +529,15 @@
         Export the information of this component to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseComponent",
+            type=self.__class__.__name__,
             name=self.name,
             ID=self.ID,
             parent_component_list=[c.ID for c in self.parent_component_list],
             child_component_list=[c.ID for c in self.child_component_list],
             targeted_task_list=[t.ID for t in self.targeted_task_list],
             space_size=self.space_size,
             state=int(self.state),
```

### Comparing `pDESy-0.4.9/pDESy/model/base_facility.py` & `pDESy-0.5.0/pDESy/model/base_facility.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 class BaseFacility(object, metaclass=abc.ABCMeta):
     """BaseFacility.
 
     BaseFacility class for expressing a workplace.
     This class will be used as template.
 
     Args:
-        name (str):
+        name (str, optional):
             Basic parameter.
             Name of this facility.
+            Defaults to None -> "New Facility"
         ID (str, optional):
             Basic parameter.
             ID will be defined automatically.
             Defaults to None -> str(uuid.uuid4()).
         workplace_id (str, optional):
             Basic parameter.
             ID of Workplace which this facility is belonged.
@@ -77,15 +78,15 @@
             Record of his or her assigned tasks' id in simulation.
             Defaults to None -> [].
     """
 
     def __init__(
         self,
         # Basic parameters
-        name: str,
+        name=None,
         ID=None,
         workplace_id=None,
         cost_per_time=0.0,
         solo_working=False,
         workamount_skill_mean_map={},
         workamount_skill_sd_map={},
         absence_time_list=None,
@@ -97,15 +98,15 @@
         assigned_task_id_record=None,
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.name = name
+        self.name = name if name is not None else "New Facility"
         self.ID = ID if ID is not None else str(uuid.uuid4())
         self.workplace_id = workplace_id if workplace_id is not None else None
         self.cost_per_time = cost_per_time if cost_per_time != 0.0 else 0.0
         self.solo_working = solo_working if solo_working is not None else False
         self.workamount_skill_mean_map = (
             workamount_skill_mean_map if workamount_skill_mean_map != {} else {}
         )
@@ -162,15 +163,15 @@
         Export the information of this facility to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseFacility",
+            type=self.__class__.__name__,
             name=self.name,
             ID=self.ID,
             workplace_id=self.workplace_id if self.workplace_id is not None else None,
             cost_per_time=self.cost_per_time,
             solo_working=self.solo_working,
             workamount_skill_mean_map=self.workamount_skill_mean_map,
             workamount_skill_sd_map=self.workamount_skill_sd_map,
```

### Comparing `pDESy-0.4.9/pDESy/model/base_organization.py` & `pDESy-0.5.0/pDESy/model/base_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """base_organization."""
 
 import abc
 import datetime
 import warnings
-from typing import List
 
 import matplotlib.pyplot as plt
 
 import networkx as nx
 
 import plotly.figure_factory as ff
 import plotly.graph_objects as go
@@ -24,41 +23,42 @@
     """BaseOrganization.
 
     BaseOrganization class for expressing organization in target project.
     BaseOrganization is consist of multiple BaseTeam and BaseWorkplace.
     This class will be used as template.
 
     Args:
-        team_list (List[BaseTeam]):
+        team_list (List[BaseTeam], optional):
             Basic parameter.
             List of BaseTeam in this organization.
+            Default to None -> []
         workplace_list (List[BaseWorkplace], optional):
             Basic parameter.
             List of BaseWorkplace in this organization.
             Default to None -> []
         cost_list (List[float], optional):
             Basic variable.
             History or record of this organization's cost in simulation.
             Defaults to None -> [].
     """
 
     def __init__(
         self,
         # Basic parameters
-        team_list: List[BaseTeam],
+        team_list=None,
         workplace_list=None,
         # Basic variables
         cost_list=None,
     ):
         """init."""
         # ----
         # Constraint parameters on simulation
         # --
         # Basic parameter
-        self.team_list = team_list
+        self.team_list = team_list if team_list is not None else []
         self.workplace_list = workplace_list if workplace_list is not None else []
         # --
         # Advanced parameter for customized simulation
 
         # ----
         # Changeable variables on simulation
         # --
@@ -84,15 +84,15 @@
         Export the information of this organization to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseOrganization",
+            type=self.__class__.__name__,
             team_list=[t.export_dict_json_data() for t in self.team_list],
             workplace_list=[t.export_dict_json_data() for t in self.workplace_list],
             cost_list=self.cost_list,
         )
         return dict_json_data
 
     def read_json_data(self, json_data):
@@ -506,14 +506,40 @@
         """Reverse log information of all."""
         self.cost_list = self.cost_list[::-1]
         for team in self.team_list:
             team.reverse_log_information()
         for workplace in self.workplace_list:
             workplace.reverse_log_information()
 
+    def reverse_dependencies(self):
+        """
+        Reverse all workplace dependencies in workplace_list.
+
+        Note:
+            This method is developed only for backward simulation.
+        """
+        # 1.
+        # Register the input_workplace_list to dummy_output_workplace_list
+        # Register the output_workplace_list to dummy_input_workplace_list
+        for workplace in self.workplace_list:
+            workplace.dummy_output_workplace_list = workplace.input_workplace_list
+            workplace.dummy_input_workplace_list = workplace.output_workplace_list
+
+        # 2.
+        # Register the dummy_output_workplace_list to output_workplace_list
+        # Register the dummy_input_workplace_list to input_workplace_list
+        # Delete the dummy_output_workplace_list, dummy_input_workplace_list
+        for workplace in self.workplace_list:
+            workplace.output_workplace_list = workplace.dummy_output_workplace_list
+            workplace.input_workplace_list = workplace.dummy_input_workplace_list
+            del (
+                workplace.dummy_output_workplace_list,
+                workplace.dummy_input_workplace_list,
+            )
+
     def add_labor_cost(
         self,
         only_working=True,
         add_zero_to_all_workers=False,
         add_zero_to_all_facilities=False,
     ):
         """
```

### Comparing `pDESy-0.4.9/pDESy/model/base_priority_rule.py` & `pDESy-0.5.0/pDESy/model/base_priority_rule.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     FSS = 0  # Free Space Size
     SSP = 1  # Sum Skill Points of targeted task
 
 
 class ResourcePriorityRuleMode(IntEnum):
     """ResourcePriorityRuleMode."""
 
-    SSP = 0
-    VC = 1
-    HSV = 2
+    MW = -1  # a worker whose main workplace is equal to target has high priority
+    SSP = 0  # a worker which amount of skillpoint is lower has high priority
+    VC = 1  # a worker which cost is lower has high priority
+    HSV = 2  # a worker which target skillpoint is higher has high priority
 
 
 class TaskPriorityRuleMode(IntEnum):
     """TaskPriorityRuleMode."""
 
     TSLACK = 0
     EST = 1  # Earliest Start Time
@@ -75,55 +76,119 @@
             workplace_list,
             key=lambda workplace: count_sum_skill_point(workplace, kwargs["name"]),
             reverse=True,
         )
     return workplace_list
 
 
-def sort_resource_list(
-    resource_list, priority_rule_mode=ResourcePriorityRuleMode.SSP, **kwargs
+def sort_worker_list(
+    worker_list, priority_rule_mode=ResourcePriorityRuleMode.SSP, **kwargs
 ):
     """
-    Sort resource_list as priority_rule_mode.
+    Sort worker_list as priority_rule_mode.
 
     Args:
-        resource_list (List[BaseResource]):
-            Target resource list of sorting.
-            BaseWorker and BaseFacility are one of resource type in this repository.
+        worker_list (List[BaseWorker]):
+            Target worker list of sorting.
         priority_rule_mode (ResourcePriorityRuleMode, optional):
             Mode of priority rule for sorting.
             Defaults to ResourcePriorityRuleMode.SSP
         args:
             Other information of each rule.
     Returns:
-        List[BaseResource]: resource_list after sorted
+        List[BaseWorker]: worker_list after sorted
     """
-    # SSP: a resource which amount of skillpoint is lower has high priority
+    target_workplace_id = None
+    if "workplace_id" in kwargs:
+        target_workplace_id = kwargs["workplace_id"]
+
+    # MW: a worker whose main workplace is equal to target has high priority
+    if priority_rule_mode == ResourcePriorityRuleMode.MW:
+        worker_list = sorted(
+            worker_list,
+            key=lambda worker: (
+                worker.main_workplace_id is not target_workplace_id,  # MW1
+                worker.main_workplace_id is not None,  # MW2
+                sum(worker.workamount_skill_mean_map.values()),  # SSP (additional)
+            ),
+        )
+    # SSP: a worker which amount of skillpoint is lower has high priority
+    elif priority_rule_mode == ResourcePriorityRuleMode.SSP:
+        worker_list = sorted(
+            worker_list,
+            key=lambda worker: (
+                sum(worker.workamount_skill_mean_map.values()),
+                worker.main_workplace_id is not target_workplace_id,
+                worker.main_workplace_id is not None,
+            ),
+        )
+    # VC: a worker which cost is lower has high priority
+    elif priority_rule_mode == ResourcePriorityRuleMode.VC:
+        worker_list = sorted(
+            worker_list,
+            key=lambda worker: (
+                worker.cost_per_time,
+                worker.main_workplace_id is not target_workplace_id,
+                worker.main_workplace_id is not None,
+            ),
+        )
+    # HSV: a worker which target skillpoint is higher has high priority
+    elif priority_rule_mode == ResourcePriorityRuleMode.HSV:
+        worker_list = sorted(
+            worker_list,
+            key=lambda worker: (
+                -worker.workamount_skill_mean_map.get(kwargs["name"], -float("inf")),
+                worker.main_workplace_id is not target_workplace_id,
+                worker.main_workplace_id is not None,
+            ),
+        )
+
+    return worker_list
+
+
+def sort_facility_list(
+    facility_list, priority_rule_mode=ResourcePriorityRuleMode.SSP, **kwargs
+):
+    """
+    Sort facility_list as priority_rule_mode.
+
+    Args:
+        facility_list (List[BaseFacility]):
+            Target facility list of sorting.
+        priority_rule_mode (ResourcePriorityRuleMode, optional):
+            Mode of priority rule for sorting.
+            Defaults to ResourcePriorityRuleMode.SSP
+        args:
+            Other information of each rule.
+    Returns:
+        List[BaseFacility]: facility_list after sorted
+    """
+    # SSP: a facility which amount of skillpoint is lower has high priority
     if priority_rule_mode == ResourcePriorityRuleMode.SSP:
-        resource_list = sorted(
-            resource_list,
-            key=lambda resource: sum(resource.workamount_skill_mean_map.values()),
+        facility_list = sorted(
+            facility_list,
+            key=lambda facility: sum(facility.workamount_skill_mean_map.values()),
         )
-    # VC :a resource which cost is lower has high priority
+    # VC :a facility which cost is lower has high priority
     elif priority_rule_mode == ResourcePriorityRuleMode.VC:
-        resource_list = sorted(
-            resource_list,
-            key=lambda resource: (resource.cost_per_time),
+        facility_list = sorted(
+            facility_list,
+            key=lambda facility: (facility.cost_per_time),
         )
-    # HSV: a resource which target skillpoint is higher has high priority
+    # HSV: a facility which target skillpoint is higher has high priority
     elif priority_rule_mode == ResourcePriorityRuleMode.HSV:
-        resource_list = sorted(
-            resource_list,
-            key=lambda resource: resource.workamount_skill_mean_map.get(
+        facility_list = sorted(
+            facility_list,
+            key=lambda facility: facility.workamount_skill_mean_map.get(
                 kwargs["name"], -float("inf")
             ),
             reverse=True,
         )
 
-    return resource_list
+    return facility_list
 
 
 def sort_task_list(task_list, priority_rule_mode=TaskPriorityRuleMode.TSLACK):
     """
     Sort task_list as priority_rule_mode.
 
     Args:
```

### Comparing `pDESy-0.4.9/pDESy/model/base_product.py` & `pDESy-0.5.0/pDESy/model/base_product.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """base_product."""
 
 import abc
 import datetime
 import warnings
-from typing import List
 
 import matplotlib.pyplot as plt
 
 import networkx as nx
 
 import plotly.figure_factory as ff
 import plotly.graph_objects as go
@@ -22,25 +21,27 @@
     """BaseProduct.
 
     BaseProduct class for expressing target product in a project.
     BaseProduct is consist of multiple BaseComponents.
     This class will be used as template.
 
     Args:
-        component_list (List[BaseComponent]):
+        component_list (List[BaseComponent], optional):
             List of BaseComponents
     """
 
-    def __init__(self, component_list: List[BaseComponent]):
+    def __init__(self, component_list=None):
         """init."""
         # ----
         # Constraint parameters on simulation
         # --
         # Basic parameter
-        self.component_list = component_list
+        self.component_list = []
+        if component_list is not None:
+            self.extend_child_component_list(component_list)
 
     def initialize(self, state_info=True, log_info=True):
         """
         Initialize the following changeable variables of BaseProduct.
 
         BaseComponent in `component_list` are also initialized by this function.
 
@@ -63,24 +64,42 @@
         Examples:
             >>> p = BaseProduct([BaseComponent('c')])
             >>> print([c.name for c in p.component_list])
             ['c']
         """
         return "{}".format(list(map(lambda c: str(c), self.component_list)))
 
+    def append_child_component(self, component):
+        """
+        Append target component to this workflow.
+        Args:
+            component (BaseComponent): target component
+        """
+        self.component_list.append(component)
+        component.parent_product = self
+
+    def extend_child_component_list(self, component_list):
+        """
+        Extend target component_list to this product.
+        Args:
+            component_list (List[BaseComponent]): target component list
+        """
+        for component in component_list:
+            self.append_child_component(component)
+
     def export_dict_json_data(self):
         """
         Export the information of this product to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseProduct",
+            type=self.__class__.__name__,
             component_list=[c.export_dict_json_data() for c in self.component_list],
         )
         return dict_json_data
 
     def read_json_data(self, json_data):
         """
         Read the JSON data for creating BaseOrganization instance.
@@ -379,36 +398,14 @@
         if len(self.component_list) > 0:
             for t in range(len(self.component_list[0].state_record_list)):
                 print("TIME: ", t)
                 if backward:
                     t = len(self.component_list[0].state_record_list) - 1 - t
                 self.print_log(t)
 
-    def remove_absence_time_list(self, absence_time_list):
-        """
-        Remove record information on `absence_time_list`.
-
-        Args:
-            absence_time_list (List[int]):
-                List of absence step time in simulation.
-        """
-        for c in self.component_list:
-            c.remove_absence_time_list(absence_time_list)
-
-    def insert_absence_time_list(self, absence_time_list):
-        """
-        Insert record information on `absence_time_list`.
-
-        Args:
-            absence_time_list (List[int]):
-                List of absence step time in simulation.
-        """
-        for c in self.component_list:
-            c.insert_absence_time_list(absence_time_list)
-
     def plot_simple_gantt(
         self,
         finish_margin=1.0,
         view_ready=True,
         component_color="#FF6600",
         ready_color="#C0C0C0",
         figsize=[6.4, 4.8],
```

### Comparing `pDESy-0.4.9/pDESy/model/base_project.py` & `pDESy-0.5.0/pDESy/model/base_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 import matplotlib.pyplot as plt
 
 import networkx as nx
 
 import plotly.figure_factory as ff
 import plotly.graph_objects as go
 
-from .base_component import BaseComponent
+from .base_component import BaseComponent, BaseComponentState
 from .base_facility import BaseFacility, BaseFacilityState
 from .base_organization import BaseOrganization
 from .base_priority_rule import (
     TaskPriorityRuleMode,
-    sort_resource_list,
+    sort_worker_list,
+    sort_facility_list,
     sort_task_list,
     sort_workplace_list,
 )
 from .base_product import BaseProduct
 from .base_task import BaseTask, BaseTaskDependency, BaseTaskState
 from .base_team import BaseTeam
 from .base_worker import BaseWorker, BaseWorkerState
@@ -53,17 +54,14 @@
     """BaseProject.
 
     BaseProject class for expressing target project
     including product, organization and workflow.
     This class will be used as template.
 
     Args:
-        file_path (str, optional):
-            File path of this project data for reading.
-            Defaults to None. (New Project)
         init_datetime (datetime.datetime, optional):
             Start datetime of project.
             Defaults to None -> datetime.datetime.now().
         unit_timedelta (datetime.timedelta, optional):
             Unit time of simulation.
             Defaults to None -> datetime.timedelta(minutes=1).
         absence_time_list (List[int], optional):
@@ -71,21 +69,21 @@
             Defaults to None -> [].
         perform_auto_task_while_absence_time (bool, optional):
             Perform auto_task while absence time or not.
             Defaults to None -> False.
             This means that auto_task does not be performed while absence time.
         product (BaseProduct, optional):
             BaseProduct in this project.
-            Defaults to None. (New Project)
+            Defaults to None. -> BaseProduct()
         organization (BaseOrganization, optional):
             BaseOrganization in this project.
-            Defaults to None. (New Project)
+            Defaults to None. -> BaseOrganization()
         workflow (BaseWorkflow, optional):
             BaseWorkflow in this project.
-            Defaults to None. (New Project)
+            Defaults to None. -> BaseWorkflow()
         time (int, optional):
             Simulation time executing this method.
             Defaults to 0.
         cost_list (List[float], optional):
             Basic variable.
             History or record of this project's cost in simulation.
             Defaults to None -> [].
@@ -97,15 +95,14 @@
             Basic variable.
             Project status.
             Defaults to None -> BaseProjectStatus.NONE
     """
 
     def __init__(
         self,
-        file_path=None,
         # Basic parameters
         init_datetime=None,
         unit_timedelta=None,
         absence_time_list=None,
         perform_auto_task_while_absence_time=None,
         # Basic variables
         product=None,
@@ -143,25 +140,25 @@
 
         # Changeable variable on simulation
         # --
         # Basic variables
         if product is not None:
             self.product = product
         else:
-            self.product = None
+            self.product = BaseProduct()
 
         if organization is not None:
             self.organization = organization
         else:
-            self.organization = None
+            self.organization = BaseOrganization()
 
         if workflow is not None:
             self.workflow = workflow
         else:
-            self.workflow = None
+            self.workflow = BaseWorkflow()
 
         if time != int(0):
             self.time = time
         else:
             self.time = int(0)
 
         if cost_list is not None:
@@ -189,20 +186,19 @@
             self.time, str(self.product), str(self.organization), str(self.workflow)
         )
 
     def initialize(self, state_info=True, log_info=True):
         """
         Initialize the following changeable variables of BaseProject.
 
-        If `state_info` is True, the following attributes are initialized.
-
-          - `time`
+        If `state_info` is True, the attributes of this class are not initialized.
 
         If `log_info` is True, the following attributes are initialized.
 
+          - `time`
           - `cost_list`
           - `simulation_mode`
           - `status`
 
         BaseProduct in `product`, BaseOrganization in `organization` and BaseWorkflow in `workflow`
         are also initialized by this function.
 
@@ -210,17 +206,17 @@
             state_info (bool):
                 State information are initialized or not.
                 Defaluts to True.
             log_info (bool):
                 Log information are initialized or not.
                 Defaults to True.
         """
-        if state_info:
-            self.time = 0
+
         if log_info:
+            self.time = 0
             self.cost_list = []
             self.simulation_mode = SimulationMode.NONE
             self.status = BaseProjectStatus.NONE
         self.organization.initialize(state_info=state_info, log_info=log_info)
         self.workflow.initialize(state_info=state_info, log_info=log_info)
         self.product.initialize(state_info=state_info, log_info=log_info)
         # product should be initialized after initializing workflow
@@ -294,25 +290,31 @@
         self.simulation_mode = SimulationMode.FOWARD
 
         self.absence_time_list = absence_time_list
 
         self.perform_auto_task_while_absence_time = perform_auto_task_while_absence_time
 
         while True:
+
+            # 0. Update status
+            self.__update()
+
             # 1. Check finished or not
             state_list = list(map(lambda task: task.state, self.workflow.task_list))
             if all(state == BaseTaskState.FINISHED for state in state_list):
                 self.status = BaseProjectStatus.FINISHED_SUCCESS
                 return
 
-            # Error check
+            # Time over check
             if self.time >= max_time:
-                text = "Time Over! Please check your simulation model or increase max_time value"
                 self.status = BaseProjectStatus.FINISHED_FAILURE
-                raise Exception(text)
+                warnings.warn(
+                    "Time Over! Please check your simulation model or increase max_time value"
+                )
+                return
 
             # check now is business time or not
             working = True
 
             if self.time in absence_time_list:
                 working = False
 
@@ -342,16 +344,16 @@
                 if mode == 1:
                     self.__perform()
             elif perform_auto_task_while_absence_time:
                 self.workflow.perform(self.time, only_auto_task=True)
 
             # 5. Record
             self.__record(working=working)
-            # 6. Update
-            self.__update()
+
+            # 6. Update time
             self.time = self.time + unit_time
 
     def backward_simulate(
         self,
         task_performed_mode="multi-workers",
         task_priority_rule=TaskPriorityRuleMode.TSLACK,
         error_tol=1e-10,
@@ -412,14 +414,15 @@
                 Defaults to True.
 
         Note:
             This function is only for research and still in progress.
             Especially, this function is not suitable for simulation considering rework.
         """
         self.workflow.reverse_dependencies()
+        self.organization.reverse_dependencies()
 
         autotask_removing_after_simulation = set()
         try:
             if considering_due_time_of_tail_tasks:
                 # Add dummy task for considering the difference of due_time
                 tail_task_list = list(
                     filter(
@@ -458,14 +461,15 @@
             for autotask in autotask_removing_after_simulation:
                 for task, dependency in autotask.output_task_list:
                     task.input_task_list.remove([autotask, dependency])
                 self.workflow.task_list.remove(autotask)
             if reverse_log_information:
                 self.reverse_log_information()
             self.workflow.reverse_dependencies()
+            self.organization.reverse_dependencies()
 
     def reverse_log_information(self):
         """Reverse log information of all."""
         self.cost_list = self.cost_list[::-1]
         total_step_length = len(self.cost_list)
         self.absence_time_list = sorted(
             list(
@@ -523,19 +527,14 @@
             filter(
                 lambda task: task.state == BaseTaskState.READY
                 or task.state == BaseTaskState.WORKING,
                 self.workflow.task_list,
             )
         )
 
-        # Candidate allocating task list (auto_task=False)
-        ready_and_working_task_list = list(
-            filter(lambda task: not task.auto_task, ready_and_working_task_list)
-        )
-
         worker_list = list(
             itertools.chain.from_iterable(
                 list(map(lambda team: team.worker_list, self.organization.team_list))
             )
         )
 
         free_worker_list = list(
@@ -547,127 +546,162 @@
             ready_and_working_task_list, task_priority_rule
         )
 
         # 3. Allocate ready tasks to free workers and facilities
         target_workplace_id_list = [wp.ID for wp in self.organization.workplace_list]
 
         for task in ready_and_working_task_list:
-            # 3-1. Set target component of workplace if target component is ready
-            component = task.target_component
-            if component.is_ready():
-                candidate_workplace_list = task.allocated_workplace_list
-                candidate_workplace_list = sort_workplace_list(
-                    candidate_workplace_list,
-                    task.workplace_priority_rule,
-                    name=task.name,
-                )
-                for workplace in candidate_workplace_list:
-                    if workplace.ID in target_workplace_id_list:
-                        conveyor_condition = True
-                        if len(workplace.input_workplace_list) > 0:
-                            if component.placed_workplace is None:
-                                conveyor_condition = True
-                            elif not (
-                                component.placed_workplace
-                                in workplace.input_workplace_list
+            if task.target_component is not None:
+                # 3-1. Set target component of workplace if target component is ready
+                component = task.target_component
+                if component.is_ready():
+                    candidate_workplace_list = task.allocated_workplace_list
+                    candidate_workplace_list = sort_workplace_list(
+                        candidate_workplace_list,
+                        task.workplace_priority_rule,
+                        name=task.name,
+                    )
+                    for workplace in candidate_workplace_list:
+                        if workplace.ID in target_workplace_id_list:
+                            conveyor_condition = True
+                            if len(workplace.input_workplace_list) > 0:
+                                if component.placed_workplace is None:
+                                    conveyor_condition = True
+                                elif not (
+                                    component.placed_workplace
+                                    in workplace.input_workplace_list
+                                ):
+                                    conveyor_condition = False
+
+                            if (
+                                conveyor_condition
+                                and workplace.can_put(component)
+                                and workplace.get_total_workamount_skill(task.name)
+                                > 1e-10
                             ):
-                                conveyor_condition = False
+                                # 3-1-1. move ready_component
+                                pre_workplace = component.placed_workplace
 
-                        if (
-                            conveyor_condition
-                            and workplace.can_put(component)
-                            and workplace.get_total_workamount_skill(task.name) > 1e-10
-                        ):
-                            # 3-1-1. move ready_component
-                            pre_workplace = component.placed_workplace
-
-                            # 3-1-1-1. remove
-                            if pre_workplace is None:
-                                for child_c in component.child_component_list:
-                                    wp = child_c.placed_workplace
-                                    if wp is not None:
-                                        for c_wp in wp.placed_component_list:
-                                            if task.target_component.ID in [
-                                                c.ID for c in c_wp.parent_component_list
-                                            ]:
-                                                wp.remove_placed_component(c_wp)
-
-                            elif pre_workplace is not None:
-                                pre_workplace.remove_placed_component(component)
-
-                            component.set_placed_workplace(None)
-
-                            # 3-1-1-2. regsister
-                            component.set_placed_workplace(workplace)
-                            workplace.set_placed_component(component)
-                            break
-
-            # 3-2. Allocate ready tasks to free workers and facilities
-            # Worker sorting
-            free_worker_list = sort_resource_list(
-                free_worker_list, task.worker_priority_rule, name=task.name
-            )
+                                # 3-1-1-1. remove
+                                if pre_workplace is None:
+                                    for child_c in component.child_component_list:
+                                        wp = child_c.placed_workplace
+                                        if wp is not None:
+                                            for c_wp in wp.placed_component_list:
+                                                if task.target_component.ID in [
+                                                    c.ID
+                                                    for c in c_wp.parent_component_list
+                                                ]:
+                                                    wp.remove_placed_component(c_wp)
+
+                                elif pre_workplace is not None:
+                                    pre_workplace.remove_placed_component(component)
+
+                                component.set_placed_workplace(None)
+
+                                # 3-1-1-2. regsister
+                                component.set_placed_workplace(workplace)
+                                workplace.set_placed_component(component)
+                                break
 
-            allocating_workers = list(
-                filter(
-                    lambda worker: worker.has_workamount_skill(task.name)
-                    and self.__is_allocated_worker(worker, task),
-                    free_worker_list,
-                )
-            )
+            if not task.auto_task:
 
-            if task.need_facility:
+                # 3-2. Allocate ready tasks to free workers and facilities
 
-                # Search candidate facilities from the list of placed_workplace
-                placed_workplace = task.target_component.placed_workplace
+                if task.need_facility:
 
-                if placed_workplace is not None:
+                    # Search candidate facilities from the list of placed_workplace
+                    placed_workplace = task.target_component.placed_workplace
 
-                    free_facility_list = list(
-                        filter(
-                            lambda facility: facility.state == BaseFacilityState.FREE,
-                            placed_workplace.facility_list,
+                    if placed_workplace is not None:
+
+                        free_facility_list = list(
+                            filter(
+                                lambda facility: facility.state
+                                == BaseFacilityState.FREE,
+                                placed_workplace.facility_list,
+                            )
                         )
-                    )
 
-                    # Facility sorting
-                    free_facility_list = sort_resource_list(
-                        free_facility_list, task.facility_priority_rule
-                    )
+                        # Facility sorting
+                        free_facility_list = sort_facility_list(
+                            free_facility_list, task.facility_priority_rule
+                        )
 
-                    # candidate facilities
-                    allocating_facilities = list(
-                        filter(
-                            lambda facility: facility.has_workamount_skill(task.name)
-                            and self.__is_allocated_facility(facility, task),
-                            free_facility_list,
+                        # candidate facilities
+                        allocating_facilities = list(
+                            filter(
+                                lambda facility: facility.has_workamount_skill(
+                                    task.name
+                                )
+                                and self.__is_allocated_facility(facility, task),
+                                free_facility_list,
+                            )
                         )
-                    )
 
-                    for facility in allocating_facilities:
-                        for worker in allocating_workers:
-                            if task.can_add_resources(worker=worker, facility=facility):
+                        for facility in allocating_facilities:
+
+                            # Extract only candidate workers
+                            allocating_workers = list(
+                                filter(
+                                    lambda worker: worker.has_workamount_skill(
+                                        task.name
+                                    )
+                                    and self.__is_allocated_worker(worker, task)
+                                    and task.can_add_resources(
+                                        worker=worker, facility=facility
+                                    ),
+                                    free_worker_list,
+                                )
+                            )
+
+                            # Sort workers
+                            allocating_workers = sort_worker_list(
+                                allocating_workers,
+                                task.worker_priority_rule,
+                                name=task.name,
+                                workplace_id=placed_workplace.ID,
+                            )
+
+                            # Allocate
+                            for worker in allocating_workers:
                                 task.allocated_worker_list.append(worker)
                                 worker.assigned_task_list.append(task)
                                 task.allocated_facility_list.append(facility)
                                 facility.assigned_task_list.append(task)
                                 allocating_workers.remove(worker)
                                 free_worker_list = [
                                     w for w in free_worker_list if w.ID != worker.ID
                                 ]
                                 break
 
-            else:
-                for worker in allocating_workers:
-                    if task.can_add_resources(worker=worker):
-                        task.allocated_worker_list.append(worker)
-                        worker.assigned_task_list.append(task)
-                        free_worker_list = [
-                            w for w in free_worker_list if w.ID != worker.ID
-                        ]
+                else:
+
+                    # Worker sorting
+                    free_worker_list = sort_worker_list(
+                        free_worker_list, task.worker_priority_rule, name=task.name
+                    )
+
+                    # Extract only candidate workers
+                    allocating_workers = list(
+                        filter(
+                            lambda worker: worker.has_workamount_skill(task.name)
+                            and self.__is_allocated_worker(worker, task),
+                            free_worker_list,
+                        )
+                    )
+
+                    # Allocate free workers to tasks
+                    for worker in allocating_workers:
+                        if task.can_add_resources(worker=worker):
+                            task.allocated_worker_list.append(worker)
+                            worker.assigned_task_list.append(task)
+                            free_worker_list = [
+                                w for w in free_worker_list if w.ID != worker.ID
+                            ]
 
         # 4. Update state of task newly allocated workers and facilities (READY -> WORKING)
         self.workflow.check_state(self.time, BaseTaskState.WORKING)
         self.product.check_state()  # product should be checked after checking workflow state
 
     def remove_absence_time_list(self):
         """
@@ -1531,15 +1565,15 @@
         Args:
             file_path (str):
                 File path for saving this project data.
         """
         dict_data = {"pDESy": []}
         dict_data["pDESy"].append(
             {
-                "type": "BaseProject",
+                "type": self.__class__.__name__,
                 "init_datetime": self.init_datetime.strftime("%Y-%m-%d %H:%M:%S"),
                 "unit_timedelta": str(self.unit_timedelta.total_seconds()),
                 "absence_time_list": self.absence_time_list,
                 "perform_auto_task_while_absence_time": self.perform_auto_task_while_absence_time,
                 "time": self.time,
                 "cost_list": self.cost_list,
                 "simulation_mode": int(self.simulation_mode),
@@ -1686,14 +1720,225 @@
                 for ID in x.placed_component_list
             ]
             for f in x.facility_list:
                 f.assigned_task_list = [
                     self.workflow.get_task_list(ID=ID)[0] for ID in f.assigned_task_list
                 ]
 
+    def append_project_log_from_simple_json(self, file_path, encoding="utf-8"):
+        """
+        Append project log information from json file which is created by BaseProject.write_simple_json().
+        TODO: This function is not yet verified sufficiently.
+
+        Args:
+            file_path (str):
+                File path for reading targeted extended project data.
+        """
+        pdes_json = open(file_path, "r", encoding=encoding)
+        json_data = json.load(pdes_json)
+        data = json_data["pDESy"]
+        project_json = list(filter(lambda node: node["type"] == "BaseProject", data))[0]
+
+        target_absence_time_list = [
+            self.time + t for t in project_json["absence_time_list"]
+        ]
+        self.absence_time_list.extend(target_absence_time_list)
+
+        self.time = self.time + int(project_json["time"])
+        self.cost_list.extend(project_json["cost_list"])
+
+        # product
+        product_json = list(filter(lambda node: node["type"] == "BaseProduct", data))[0]
+        for c_json in product_json["component_list"]:
+            c = list(
+                filter(
+                    lambda component: component.ID == c_json["ID"],
+                    self.product.component_list,
+                )
+            )[0]
+            c.state = BaseComponentState(c_json["state"])
+            c.state_record_list.extend(
+                [BaseComponentState(num) for num in c_json["state_record_list"]]
+            )
+            c.placed_workplace = c_json["placed_workplace"]
+            c.placed_workplace_id_record.extend(c_json["placed_workplace_id_record"])
+
+        # workflow
+        workflow_j = list(filter(lambda node: node["type"] == "BaseWorkflow", data))[0]
+        for j in workflow_j["task_list"]:
+            task = list(
+                filter(
+                    lambda task: task.ID == j["ID"],
+                    self.workflow.task_list,
+                )
+            )[0]
+            task.est = j["est"]
+            task.eft = j["eft"]
+            task.lst = j["lst"]
+            task.lft = j["lft"]
+            task.remaining_work_amount = j["remaining_work_amount"]
+            task.state = BaseTaskState(j["state"])
+            task.state_record_list.extend(
+                [BaseTaskState(num) for num in j["state_record_list"]],
+            )
+            task.allocated_worker_list = j["allocated_worker_list"]
+            task.allocated_worker_id_record.extend(j["allocated_worker_id_record"])
+            task.allocated_facility_list = j["allocated_facility_list"]
+            task.allocated_facility_id_record.extend(j["allocated_facility_id_record"])
+
+        # organization
+        o_json = list(filter(lambda node: node["type"] == "BaseOrganization", data))[0]
+        # team
+        team_list_j = o_json["team_list"]
+        for team_j in team_list_j:
+            team = list(
+                filter(
+                    lambda team: team.ID == team_j["ID"],
+                    self.organization.team_list,
+                )
+            )[0]
+            team.cost_list.extend(team_j["cost_list"])
+            for j in team_j["worker_list"]:
+                worker = list(
+                    filter(
+                        lambda worker: worker.ID == j["ID"],
+                        team.worker_list,
+                    )
+                )[0]
+                worker.state = BaseWorkerState(j["state"])
+                worker.state_record_list.extend(
+                    [BaseWorkerState(num) for num in j["state_record_list"]],
+                )
+                worker.cost_list.extend(j["cost_list"])
+                worker.assigned_task_list = j["assigned_task_list"]
+                worker.assigned_task_id_record.extend(j["assigned_task_id_record"])
+
+        # workplace
+        workplace_list_j = o_json["workplace_list"]
+        for workplace_j in workplace_list_j:
+            workplace = list(
+                filter(
+                    lambda workplace: workplace.ID == workplace_j["ID"],
+                    self.organization.workplace_list,
+                )
+            )[0]
+            workplace.cost_list.extend(workplace_j["cost_list"])
+            workplace.placed_component_list = workplace_j["placed_component_list"]
+            workplace.placed_component_id_record.extend(
+                workplace_j["placed_component_id_record"]
+            )
+            for j in workplace_j["facility_list"]:
+                facility = list(
+                    filter(
+                        lambda worker: worker.ID == j["ID"],
+                        workplace.facility_list,
+                    )
+                )[0]
+                facility.state = BaseWorkerState(j["state"])
+                facility.state_record_list.extend(
+                    [BaseWorkerState(num) for num in j["state_record_list"]],
+                )
+                facility.cost_list.extend(j["cost_list"])
+                facility.assigned_task_list = j["assigned_task_list"]
+                facility.assigned_task_id_record.extend(j["assigned_task_id_record"])
+        # organization = BaseOrganization(team_list=[], workplace_list=[])
+        # organization.read_json_data(organization_json)
+        # self.organization = organization
+
+        # # 2. update ID info to instance info
+        # # 2-1. component
+        # for c in self.product.component_list:
+        #     c.parent_component_list = [
+        #         self.product.get_component_list(ID=ID)[0]
+        #         for ID in c.parent_component_list
+        #     ]
+        #     c.child_component_list = [
+        #         self.product.get_component_list(ID=ID)[0]
+        #         for ID in c.child_component_list
+        #     ]
+        #     c.targeted_task_list = [
+        #         self.workflow.get_task_list(ID=ID)[0] for ID in c.targeted_task_list
+        #     ]
+        #     c.placed_workplace = (
+        #         self.organization.get_workplace_list(ID=c.placed_workplace)[0]
+        #         if c.placed_workplace is not None
+        #         else None
+        #     )
+        # # 2-2. task
+        # for t in self.workflow.task_list:
+        #     t.input_task_list = [
+        #         [
+        #             self.workflow.get_task_list(ID=ID)[0],
+        #             BaseTaskDependency(dependency_number),
+        #         ]
+        #         for (ID, dependency_number) in t.input_task_list
+        #     ]
+        #     t.output_task_list = [
+        #         [
+        #             self.workflow.get_task_list(ID=ID)[0],
+        #             BaseTaskDependency(dependency_number),
+        #         ]
+        #         for (ID, dependency_number) in t.output_task_list
+        #     ]
+        #     t.allocated_team_list = [
+        #         self.organization.get_team_list(ID=ID)[0]
+        #         for ID in t.allocated_team_list
+        #     ]
+        #     t.allocated_workplace_list = [
+        #         self.organization.get_workplace_list(ID=ID)[0]
+        #         for ID in t.allocated_workplace_list
+        #     ]
+        #     t.target_component = (
+        #         self.product.get_component_list(ID=t.target_component)[0]
+        #         if t.target_component is not None
+        #         else None
+        #     )
+        #     t.allocated_worker_list = [
+        #         self.organization.get_worker_list(ID=ID)[0]
+        #         for ID in t.allocated_worker_list
+        #     ]
+        #     t.allocated_facility_list = [
+        #         self.organization.get_facility_list(ID=ID)[0]
+        #         for ID in t.allocated_facility_list
+        #     ]
+        # # 2-3. organziation
+        # # 2-3-1. team
+        # for x in self.organization.team_list:
+        #     x.targeted_task_list = [
+        #         self.workflow.get_task_list(ID=ID)[0] for ID in x.targeted_task_list
+        #     ]
+        #     x.parent_team = (
+        #         self.organization.get_team_list(ID=x.parent_team)[0]
+        #         if x.parent_team is not None
+        #         else None
+        #     )
+        #     for w in x.worker_list:
+        #         w.assigned_task_list = [
+        #             self.workflow.get_task_list(ID=ID)[0] for ID in w.assigned_task_list
+        #         ]
+
+        # # 2-3-2. workplace
+        # for x in self.organization.workplace_list:
+        #     x.targeted_task_list = [
+        #         self.workflow.get_task_list(ID=ID)[0] for ID in x.targeted_task_list
+        #     ]
+        #     x.parent_workplace = (
+        #         self.organization.get_workplace_list(ID=x.parent_workplace)[0]
+        #         if x.parent_workplace is not None
+        #         else None
+        #     )
+        #     x.placed_component_list = [
+        #         self.product.get_component_list(ID=ID)[0]
+        #         for ID in x.placed_component_list
+        #     ]
+        #     for f in x.facility_list:
+        #         f.assigned_task_list = [
+        #             self.workflow.get_task_list(ID=ID)[0] for ID in f.assigned_task_list
+        #         ]
+
     # ---
     # READ FUNCTION
     # ---
 
     # def read_pDESy_web_json(self, file_path: str, encoding=None):
     #     """
     #     Read json file from pDESy.org.
```

### Comparing `pDESy-0.4.9/pDESy/model/base_resource.py` & `pDESy-0.5.0/pDESy/model/base_worker.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,75 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-"""base_resource."""
+"""base_worker."""
 
 import abc
 import uuid
-import warnings
 from enum import IntEnum
-
 import numpy as np
 
 from .base_task import BaseTaskState
 
 
-class BaseResourceState(IntEnum):
-    """BaseResourceState.
-
-    Note:
-        DEPRICATED from v0.3.
-        Use BaseWorkerState or BaseFacilityState as instead.
-    """
-
-    warnings.warn(
-        "DEPRICATED from v1.3. Use BaseWorkerState or BaseFacilityState as instead.",
-        DeprecationWarning,
-    )
+class BaseWorkerState(IntEnum):
+    """BaseWorkerState."""
 
     FREE = 0
     WORKING = 1
     ABSENCE = -1
 
 
-class BaseResource(object, metaclass=abc.ABCMeta):
-    """BaseResource.
-
-    Note:
-        DEPRICATED from v0.3.
-        Use BaseWorkerState or BaseFacilityState as instead.
-
+class BaseWorker(object, metaclass=abc.ABCMeta):
+    """BaseWorker.
 
-    BaseResource class for expressing a team.
+    BaseWorker class for expressing a worker.
     This class will be used as template.
 
     Args:
-        name (str):
-            Basic parameter. Name of this resource.
+        name (str, optional):
+            Basic parameter.
+            Name of this worker.
+            Defaults to None -> "New Worker"
         ID (str, optional):
             Basic parameter.
             ID will be defined automatically.
-            Defaults to None.
+            Defaults to None -> str(uuid.uuid4()).
         team_id (str, optional):
             Basic parameter.
-            Team ID will be defined automatically on adding team.
+            Defaults to None.
+        main_workplace_id (str, optional):
+            Basic parameter.
             Defaults to None.
         cost_per_time (float, optional):
             Basic parameter.
-            Cost of this resource per unit time.
+            Cost of this worker per unit time.
             Defaults to 0.0.
         solo_working (bool, optional):
             Basic parameter.
-            Flag whether this resource can work with other resources or not.
+            Flag whether this worker can work with other workers or not.
             Defaults to False.
         workamount_skill_mean_map (Dict[str, float], optional):
             Basic parameter.
             Skill for expressing progress in unit time.
             Defaults to {}.
         workamount_skill_sd_map (Dict[str, float], optional):
             Basic parameter.
             Standard deviation of skill for expressing progress in unit time.
             Defaults to {}.
+        facility_skill_map (Dict[str, float], optional):
+            Basic parameter.
+            Skill for operating facility in unit time.
+            Defaults to {}.
         absence_time_list (List[int], optional):
             List of absence time of simulation.
             Defaults to None -> [].
-        state (BaseResourceState, optional):
+        state (BaseWorkerState, optional):
             Basic variable.
-            State of this resource in simulation.
-            Defaults to BaseResourceState.FREE.
+            State of this worker in simulation.
+            Defaults to BaseWorkerState.FREE.
         state_record_list (List[BaseWorkerState], optional):
             Basic variable.
             Record list of state.
             Defaults to None -> [].
         cost_list (List[float], optional):
             Basic variable.
             History or record of his or her cost in simulation.
@@ -87,47 +78,58 @@
             Basic variable.
             State of his or her assigned tasks in simulation.
             Defaults to None -> [].
         assigned_task_id_record (List[List[str]], optional):
             Basic variable.
             Record of his or her assigned tasks' id in simulation.
             Defaults to None -> [].
+        quality_skill_mean_map (Dict[str, float], optional):
+            Advanced parameter.
+            Skill for expressing quality in unit time.
+            Defaults to {}.
+        quality_skill_sd_map (Dict[str, float], optional):
+            Advanced parameter.
+            Standard deviation of skill for expressing quality in unit time.
+            Defaults to {}.
     """
 
-    warnings.warn(
-        "DEPRICATED from v1.3. Use BaseWorker or BaseFacility as instead.",
-        DeprecationWarning,
-    )
-
     def __init__(
         self,
         # Basic parameters
-        name: str,
+        name=None,
         ID=None,
         team_id=None,
+        main_workplace_id=None,
         cost_per_time=0.0,
         solo_working=False,
         workamount_skill_mean_map={},
         workamount_skill_sd_map={},
+        facility_skill_map={},
         absence_time_list=None,
         # Basic variables
-        state=BaseResourceState.FREE,
+        state=BaseWorkerState.FREE,
         state_record_list=None,
         cost_list=None,
         assigned_task_list=None,
         assigned_task_id_record=None,
+        # Advanced parameters for customized simulation
+        quality_skill_mean_map={},
+        quality_skill_sd_map={},
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.name = name
+        self.name = name if name is not None else "New Worker"
         self.ID = ID if ID is not None else str(uuid.uuid4())
         self.team_id = team_id if team_id is not None else None
+        self.main_workplace_id = (
+            main_workplace_id if main_workplace_id is not None else None
+        )
         self.cost_per_time = cost_per_time if cost_per_time != 0.0 else 0.0
         self.solo_working = solo_working if solo_working is not None else False
         self.workamount_skill_mean_map = (
             workamount_skill_mean_map if workamount_skill_mean_map != {} else {}
         )
         self.workamount_skill_sd_map = (
             workamount_skill_sd_map if workamount_skill_sd_map is not None else {}
@@ -136,18 +138,18 @@
             absence_time_list if absence_time_list is not None else []
         )
 
         # ----
         # Changeable variable on simulation
         # --
         # Basic variables
-        if state is not BaseResourceState.FREE:
+        if state is not BaseWorkerState.FREE:
             self.state = state
         else:
-            self.state = BaseResourceState.FREE
+            self.state = BaseWorkerState.FREE
 
         if state_record_list is not None:
             self.state_record_list = state_record_list
         else:
             self.state_record_list = []
 
         if cost_list is not None:
@@ -161,14 +163,112 @@
             self.assigned_task_list = []
 
         if assigned_task_id_record is not None:
             self.assigned_task_id_record = assigned_task_id_record
         else:
             self.assigned_task_id_record = []
 
+        self.facility_skill_map = (
+            facility_skill_map if facility_skill_map is not None else {}
+        )
+
+        # --
+        # Advanced parameter for customized simulation
+        self.quality_skill_mean_map = (
+            quality_skill_mean_map if quality_skill_mean_map is not None else {}
+        )
+        self.quality_skill_sd_map = (
+            quality_skill_sd_map if quality_skill_sd_map is not None else {}
+        )
+
+    def has_facility_skill(self, facility_name, error_tol=1e-10):
+        """
+        Check whether he or she has facility skill or not.
+
+        By checking facility_skill_map.
+
+        Args:
+            facility_name (str):
+                Facility name
+            error_tol (float, optional):
+                Measures against numerical error.
+                Defaults to 1e-10.
+
+        Returns:
+            bool: whether he or she has workamount skill of task_name or not
+        """
+        if facility_name in self.facility_skill_map:
+            if self.facility_skill_map[facility_name] > 0.0 + error_tol:
+                return True
+        return False
+
+    def has_quality_skill(self, task_name, error_tol=1e-10):
+        """
+        Check whether he or she has quality skill or not.
+
+        By checking quality_skill_mean_map.
+
+        Args:
+            task_name (str):
+                Task name
+            error_tol (float, optional):
+                Measures against numerical error.
+                Defaults to 1e-10.
+
+        Returns:
+            bool: whether he or she has quality skill of task_name or not
+        """
+        if task_name in self.quality_skill_mean_map:
+            if self.quality_skill_mean_map[task_name] > 0.0 + error_tol:
+                return True
+        return False
+
+    def get_quality_skill_point(self, task_name, seed=None):
+        """
+        Get point of quality by his or her contribution in this time.
+
+        Args:
+            task_name (str):
+                Task name
+            error_tol (float, optional):
+                Countermeasures against numerical error.
+                Defaults to 1e-10.
+
+        Returns:
+            float: Point of quality by his or her contribution in this time
+        """
+        if seed is not None:
+            np.random.seed(seed=seed)
+        if not self.has_quality_skill(task_name):
+            return 0.0
+        skill_mean = self.quality_skill_mean_map[task_name]
+
+        if task_name not in self.quality_skill_sd_map:
+            skill_sd = 0
+        else:
+            skill_sd = self.quality_skill_sd_map[task_name]
+        base_quality = np.random.normal(skill_mean, skill_sd)
+        return base_quality  # / float(sum_of_working_task_in_this_time)
+
+    def check_update_state_from_absence_time_list(self, step_time):
+        """
+        Check and Update state of all resources to ABSENCE or FREE or WORKING.
+
+        Args:
+            step_time (int):
+                Target step time of checking and updating state of workers and facilities.
+        """
+        if step_time in self.absence_time_list:
+            self.state = BaseWorkerState.ABSENCE
+        else:
+            if len(self.assigned_task_list) == 0:
+                self.state = BaseWorkerState.FREE
+            else:
+                self.state = BaseWorkerState.WORKING
+
     def __str__(self):
         """str.
 
         Returns:
             str: name of BaseResource
         Examples:
             >>> r = BaseResource("r")
@@ -197,15 +297,15 @@
                 State information are initialized or not.
                 Defaluts to True.
             log_info (bool):
                 Log information are initialized or not.
                 Defaults to True.
         """
         if state_info:
-            self.state = BaseResourceState.FREE
+            self.state = BaseWorkerState.FREE
             self.assigned_task_list = []
 
         if log_info:
             self.state_record_list = []
             self.cost_list = []
             self.assigned_task_id_record = []
 
@@ -222,19 +322,19 @@
         )
 
     def record_state(self, working=True):
         """Record current 'state' in 'state_record_list'."""
         if working:
             self.state_record_list.append(self.state)
         else:
-            # if self.state == BaseResourceState.WORKING:
-            #     self.state_record_list.append(BaseResourceState.FREE)
+            # if self.state == BaseWorkerState.WORKING:
+            #     self.state_record_list.append(BaseWorkerState.FREE)
             # else:
             #     self.state_record_list.append(self.state)
-            self.state_record_list.append(BaseResourceState.ABSENCE)
+            self.state_record_list.append(BaseWorkerState.ABSENCE)
 
     def remove_absence_time_list(self, absence_time_list):
         """
         Remove record information on `absence_time_list`.
 
         Args:
             absence_time_list (List[int]):
@@ -255,21 +355,21 @@
                 List of absence step time in simulation.
         """
         for step_time in sorted(absence_time_list):
             if step_time < len(self.state_record_list):
                 if step_time == 0:
                     self.assigned_task_id_record.insert(step_time, None)
                     self.cost_list.insert(step_time, 0.0)
-                    self.state_record_list.insert(step_time, BaseResourceState.FREE)
+                    self.state_record_list.insert(step_time, BaseWorkerState.FREE)
                 else:
                     self.assigned_task_id_record.insert(
                         step_time, self.assigned_task_id_record[step_time - 1]
                     )
                     self.cost_list.insert(step_time, 0.0)
-                    self.state_record_list.insert(step_time, BaseResourceState.FREE)
+                    self.state_record_list.insert(step_time, BaseWorkerState.FREE)
 
     def print_log(self, target_step_time):
         """
         Print log in `target_step_time` as follows:
 
         - ID
         - name
@@ -317,52 +417,52 @@
         to_time = -1
         for time, state in enumerate(self.state_record_list):
             if state != previous_state:
                 if from_time == -1:
                     from_time = time
                 elif to_time == -1:
                     to_time = time
-                    if state == BaseResourceState.FREE:
-                        if previous_state == BaseResourceState.WORKING:
+                    if state == BaseWorkerState.FREE:
+                        if previous_state == BaseWorkerState.WORKING:
                             working_time_list.append(
                                 (from_time, (to_time - 1) - from_time + finish_margin)
                             )
-                        elif previous_state == BaseResourceState.ABSENCE:
+                        elif previous_state == BaseWorkerState.ABSENCE:
                             absence_time_list.append(
                                 (from_time, (to_time - 1) - from_time + finish_margin)
                             )
-                    if state == BaseResourceState.WORKING:
-                        if previous_state == BaseResourceState.FREE:
+                    if state == BaseWorkerState.WORKING:
+                        if previous_state == BaseWorkerState.FREE:
                             ready_time_list.append(
                                 (from_time, (to_time - 1) - from_time + finish_margin)
                             )
-                        elif previous_state == BaseResourceState.ABSENCE:
+                        elif previous_state == BaseWorkerState.ABSENCE:
                             absence_time_list.append(
                                 (from_time, (to_time - 1) - from_time + finish_margin)
                             )
-                    if state == BaseResourceState.ABSENCE:
-                        if previous_state == BaseResourceState.FREE:
+                    if state == BaseWorkerState.ABSENCE:
+                        if previous_state == BaseWorkerState.FREE:
                             ready_time_list.append(
                                 (from_time, (to_time - 1) - from_time + finish_margin)
                             )
-                        elif previous_state == BaseResourceState.WORKING:
+                        elif previous_state == BaseWorkerState.WORKING:
                             working_time_list.append(
                                 (from_time, (to_time - 1) - from_time + finish_margin)
                             )
                     from_time = time
                     to_time = -1
             previous_state = state
 
         # Suspended because of max time limitation
         if from_time > -1 and to_time == -1:
-            if previous_state == BaseResourceState.WORKING:
+            if previous_state == BaseWorkerState.WORKING:
                 working_time_list.append((from_time, time - from_time + finish_margin))
-            elif previous_state == BaseResourceState.FREE:
+            elif previous_state == BaseWorkerState.FREE:
                 ready_time_list.append((from_time, time - from_time + finish_margin))
-            elif previous_state == BaseResourceState.ABSENCE:
+            elif previous_state == BaseWorkerState.ABSENCE:
                 absence_time_list.append((from_time, time - from_time + finish_margin))
 
         return ready_time_list, working_time_list, absence_time_list
 
     def has_workamount_skill(self, task_name, error_tol=1e-10):
         """
         Check whether he or she has workamount skill or not.
@@ -407,15 +507,15 @@
         Returns:
             float: Progress of workamount by his or her contribution in this time
         """
         if seed is not None:
             np.random.seed(seed=seed)
         if not self.has_workamount_skill(task_name):
             return 0.0
-        if self.state == BaseResourceState.ABSENCE:
+        if self.state == BaseWorkerState.ABSENCE:
             return 0.0
         skill_mean = self.workamount_skill_mean_map[task_name]
         if task_name not in self.workamount_skill_sd_map:
             skill_sd = 0
         else:
             skill_sd = self.workamount_skill_sd_map[task_name]
         base_progress = np.random.normal(skill_mean, skill_sd)
@@ -423,7 +523,34 @@
             map(
                 lambda task: task.state == BaseTaskState.WORKING
                 or task.state == BaseTaskState.WORKING_ADDITIONALLY,
                 self.assigned_task_list,
             )
         )
         return base_progress / float(sum_of_working_task_in_this_time)
+
+    def export_dict_json_data(self):
+        """
+        Export the information of this worker to JSON data.
+
+        Returns:
+            dict: JSON format data.
+        """
+        dict_json_data = {}
+        dict_json_data.update(
+            type=self.__class__.__name__,
+            name=self.name,
+            ID=self.ID,
+            team_id=self.team_id if self.team_id is not None else None,
+            cost_per_time=self.cost_per_time,
+            solo_working=self.solo_working,
+            workamount_skill_mean_map=self.workamount_skill_mean_map,
+            workamount_skill_sd_map=self.workamount_skill_sd_map,
+            facility_skill_map=self.facility_skill_map,
+            absence_time_list=self.absence_time_list,
+            state=int(self.state),
+            state_record_list=[int(state) for state in self.state_record_list],
+            cost_list=self.cost_list,
+            assigned_task_list=[t.ID for t in self.assigned_task_list],
+            assigned_task_id_record=self.assigned_task_id_record,
+        )
+        return dict_json_data
```

### Comparing `pDESy-0.4.9/pDESy/model/base_task.py` & `pDESy-0.5.0/pDESy/model/base_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,29 @@
 class BaseTask(object, metaclass=abc.ABCMeta):
     """BaseTask.
 
     BaseTask class for expressing target workflow.
     This class will be used as template.
 
     Args:
-        name (str):
+        name (str, optional):
             Basic parameter.
             Name of this task.
+            Defaults to None -> "New Task".
         ID (str, optional):
             Basic parameter.
             ID will be defined automatically.
-            Defaults to None.
+            Defaults to None -> str(uuid.uuid4()).
         default_work_amount (float, optional):
             Basic parameter.
             Defalt workamount of this BaseTask.
             Defaults to None -> 10.0.
+        work_amount_progress_of_unit_step_time (float, optional)
+            Baseline of work amount progress of unit step time.
+            Default to None -> 1.0.
         input_task_list (List[BaseTask,BaseTaskDependency], optional):
             Basic parameter.
             List of input BaseTask and type of dependency(FS, SS, SF, F/F).
             Defaults to None -> [].
         output_task_list (List[BaseTask,BaseTaskDependency], optional):
             Basic parameter.
             List of input BaseTask and type of dependency(FS, SS, SF, F/F).
@@ -148,29 +152,39 @@
             Basic variable.
             State of allocating facility list in simulation.
             Defaults to None -> [].
         allocated_facility_id_record (List[List[str]], optional):
             Basic variable.
             State of allocating facility id list in simulation.
             Defaults to None -> [].
+        additional_work_amount (float, optional):
+            Advanced parameter.
+            Defaults to None.
+        additional_task_flag (bool, optional):
+            Advanced variable.
+            Defaults to False.
+        actual_work_amount (float, optional):
+            Advanced variable.
+            Default to None -> default_work_amount*(1.0-default_progress)
     """
 
     def __init__(
         self,
         # Basic parameters
-        name: str,
+        name=None,
         ID=None,
         default_work_amount=None,
+        work_amount_progress_of_unit_step_time=None,
         input_task_list=None,
         output_task_list=None,
         allocated_team_list=None,
         allocated_workplace_list=None,
         parent_workflow=None,
         workplace_priority_rule=WorkplacePriorityRuleMode.FSS,
-        worker_priority_rule=ResourcePriorityRuleMode.SSP,
+        worker_priority_rule=ResourcePriorityRuleMode.MW,
         facility_priority_rule=ResourcePriorityRuleMode.SSP,
         need_facility=False,
         target_component=None,
         default_progress=None,
         due_time=None,
         auto_task=False,
         fixing_allocating_worker_id_list=None,
@@ -184,25 +198,35 @@
         remaining_work_amount_record_list=None,
         state=BaseTaskState.NONE,
         state_record_list=None,
         allocated_worker_list=None,
         allocated_worker_id_record=None,
         allocated_facility_list=None,
         allocated_facility_id_record=None,
+        # Advanced parameters for customized simulation
+        additional_work_amount=None,
+        # Advanced variables for customized simulation
+        additional_task_flag=False,
+        actual_work_amount=None,
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.name = name
+        self.name = name if name is not None else "New Task"
         self.ID = ID if ID is not None else str(uuid.uuid4())
         self.default_work_amount = (
             default_work_amount if default_work_amount is not None else 10.0
         )
+        self.work_amount_progress_of_unit_step_time = (
+            work_amount_progress_of_unit_step_time
+            if work_amount_progress_of_unit_step_time is not None
+            else 1.0
+        )
         self.input_task_list = input_task_list if input_task_list is not None else []
         self.output_task_list = output_task_list if output_task_list is not None else []
         self.allocated_team_list = (
             allocated_team_list if allocated_team_list is not None else []
         )
         self.allocated_workplace_list = (
             allocated_workplace_list if allocated_workplace_list is not None else []
@@ -288,14 +312,29 @@
             self.allocated_facility_list = []
 
         if allocated_facility_id_record is not None:
             self.allocated_facility_id_record = allocated_facility_id_record
         else:
             self.allocated_facility_id_record = []
 
+        # --
+        # Advanced parameter for customized simulation
+        self.additional_work_amount = (
+            additional_work_amount if additional_work_amount is not None else 0.0
+        )
+        # --
+        # Advanced variables for customized simulation
+        if additional_task_flag is not False:
+            self.additional_task_flag = additional_task_flag
+        else:
+            self.additional_task_flag = False
+        self.actual_work_amount = self.default_work_amount * (
+            1.0 - self.default_progress
+        )
+
     def __str__(self):
         """str.
 
         Returns:
             str: name of BaseTask
         Examples:
             >>> task = BaseTask("task1")
@@ -309,18 +348,19 @@
         Export the information of this task to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseTask",
+            type=self.__class__.__name__,
             name=self.name,
             ID=self.ID,
             default_work_amount=self.default_work_amount,
+            work_amount_progress_of_unit_step_time=self.work_amount_progress_of_unit_step_time,
             input_task_list=[
                 (task.ID, int(dependency)) for task, dependency in self.input_task_list
             ],
             output_task_list=[
                 (task.ID, int(dependency)) for task, dependency in self.output_task_list
             ],
             allocated_team_list=[team.ID for team in self.allocated_team_list],
@@ -374,14 +414,15 @@
             >>> print([input_t.name for input_t in task.input_task_list])
             ['task1']
             >>> print([parent_t.name for parent_t in task1.output_task_list])
             ['task']
         """
         self.input_task_list.append([input_task, task_dependency_mode])
         input_task.output_task_list.append([self, task_dependency_mode])
+        input_task.parent_workflow = self.parent_workflow
 
     def extend_input_task_list(
         self, input_task_list, task_dependency_mode=BaseTaskDependency.FS
     ):
         """
         Extend the list of input tasks to `input_task_list`.
 
@@ -400,14 +441,15 @@
             ['task1']
             >>> print([parent_t.name for parent_t in task1.output_task_list])
             ['task']
         """
         for input_task in input_task_list:
             self.input_task_list.append([input_task, task_dependency_mode])
             input_task.output_task_list.append([self, task_dependency_mode])
+            input_task.parent_workflow = self.parent_workflow
 
     def initialize(self, error_tol=1e-10, state_info=True, log_info=True):
         """
         Initialize the following changeable variables of BaseTask.
 
         If `state_info` is True, the following attributes are initialized.
 
@@ -415,14 +457,16 @@
           - `eft`
           - `lst`
           - `lft`
           - `remaining_work_amount`
           - `state`
           - `allocated_worker_list`
           - `allocated_facility_list`
+          - `additional_task_flag`
+          - `actual_work_amount`
 
         If `log_info` is True the following attributes are initialized.
 
             - `remaining_work_amount_record_list`
             - `state_record_list`
             - `allocated_worker_id_record`
             - `allocated_facility_id_record`
@@ -445,44 +489,51 @@
             self.lft = -1.0  # Latest finish time
             self.remaining_work_amount = self.default_work_amount * (
                 1.0 - self.default_progress
             )
             self.state = BaseTaskState.NONE
             self.allocated_worker_list = []
             self.allocated_facility_list = []
+            self.additional_task_flag = False
+            self.actual_work_amount = self.default_work_amount * (
+                1.0 - self.default_progress
+            )
         if log_info:
             self.remaining_work_amount_record_list = []
             self.state_record_list = []
             self.allocated_worker_id_record = []
             self.allocated_facility_id_record = []
 
         if state_info and log_info:
-            if (0.00 + error_tol) < self.default_progress and self.default_progress < (
-                1.00 - error_tol
-            ):
-                self.state = BaseTaskState.READY
-            elif self.default_progress >= (1.00 - error_tol):
+            if self.default_progress >= (1.00 - error_tol):
                 self.state = BaseTaskState.FINISHED
 
-    def perform(self, time: int, seed=None):
+    def perform(self, time: int, seed=None, increase_component_error=1.0):
         """
         Perform this BaseTask in this simulation.
 
         Args:
             time (int):
                 Simulation time executing this method.
             seed (int, optional):
                 Random seed for describing deviation of progress.
                 Defaults to None.
+            increase_component_error (float, optional):
+                For advanced simulation.
+                Increment error value when error has occurred.
+                Defaults to 1.0.
+        Note:
+            This method includes advanced code of custom simulation.
+            We have to separete basic code and advanced code in the future.
         """
         if self.state == BaseTaskState.WORKING:
             work_amount_progress = 0.0
-
+            noErrorProbability = 1.0
             if self.auto_task:
-                work_amount_progress = 1.0
+                work_amount_progress = self.work_amount_progress_of_unit_step_time
             else:
                 if self.need_facility:
                     min_length = min(
                         len(self.allocated_worker_list),
                         len(self.allocated_facility_list),
                     )
                     for i in range(min_length):
@@ -491,26 +542,40 @@
                             self.name, seed=seed
                         )
                         facility = self.allocated_facility_list[i]
                         f_progress = facility.get_work_amount_skill_progress(
                             self.name, seed=seed
                         )
                         work_amount_progress += w_progress * f_progress
+                        noErrorProbability = (
+                            noErrorProbability
+                            - worker.get_quality_skill_point(self.name, seed=seed)
+                        )
                 else:
                     for worker in self.allocated_worker_list:
                         work_amount_progress = (
                             work_amount_progress
                             + worker.get_work_amount_skill_progress(
                                 self.name, seed=seed
                             )
                         )
+                        noErrorProbability = (
+                            noErrorProbability
+                            - worker.get_quality_skill_point(self.name, seed=seed)
+                        )
+
             self.remaining_work_amount = (
                 self.remaining_work_amount - work_amount_progress
             )
 
+            if self.target_component is not None:
+                self.target_component.update_error_value(
+                    noErrorProbability, increase_component_error, seed=seed
+                )
+
     def can_add_resources(self, worker=None, facility=None):
         """
         Judge whether this task can be assigned another resources or not.
 
         Args:
             worker (BaseWorker):
                 Target worker for allocating.
```

### Comparing `pDESy-0.4.9/pDESy/model/base_team.py` & `pDESy-0.5.0/pDESy/model/base_team.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 class BaseTeam(object, metaclass=abc.ABCMeta):
     """BaseTeam.
 
     BaseTeam class for expressing team in a project.
     This class will be used as template.
 
     Args:
-        name (str):
+        name (str, optional):
             Basic parameter.
             Name of this team.
+            Defaults to None -> "New Team"
         ID (str, optional):
             Basic parameter.
             ID will be defined automatically.
-            Defaults to None.
+            Defaults to None -> str(uuid.uuid4()).
         worker_list (List[BaseWorker], optional):
             Basic parameter.
             List of BaseWorkers who belong to this team.
             Defaults to None -> [].
         targeted_task_list (List[BaseTask], optional):
             Basic parameter.
             List of targeted BaseTasks.
@@ -46,28 +47,28 @@
             History or record of this team's cost in simulation.
             Defaults to None -> [].
     """
 
     def __init__(
         self,
         # Basic parameters
-        name: str,
+        name=None,
         ID=None,
         worker_list=None,
         targeted_task_list=None,
         parent_team=None,
         # Basic variables
         cost_list=None,
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.name = name
+        self.name = name if name is not None else "New Team"
         self.ID = ID if ID is not None else str(uuid.uuid4())
 
         self.worker_list = worker_list if worker_list is not None else []
         for worker in self.worker_list:
             if worker.team_id is None:
                 worker.team_id = self.ID
 
@@ -248,15 +249,15 @@
         Export the information of this team to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseTeam",
+            type=self.__class__.__name__,
             name=self.name,
             ID=self.ID,
             worker_list=[w.export_dict_json_data() for w in self.worker_list],
             targeted_task_list=[t.ID for t in self.targeted_task_list],
             parent_team=self.parent_team.ID if self.parent_team is not None else None,
             # Basic variables
             cost_list=self.cost_list,
```

### Comparing `pDESy-0.4.9/pDESy/model/base_workflow.py` & `pDESy-0.5.0/pDESy/model/base_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """base_workflow."""
 
 import abc
 import datetime
 import warnings
-from typing import List
 
 import matplotlib.pyplot as plt
 
 import networkx as nx
 
 import plotly.figure_factory as ff
 import plotly.graph_objects as go
 
 from .base_facility import BaseFacilityState
 from .base_task import BaseTask, BaseTaskDependency, BaseTaskState
 from .base_worker import BaseWorkerState
+from .base_subproject_task import BaseSubProjectTask
 
 
 class BaseWorkflow(object, metaclass=abc.ABCMeta):
     """BaseWorkflow.
 
     BaseWorkflow class for expressing workflow in a project.
     BaseWorkflow is consist of multiple BaseTasks.
     This class will be used as template.
 
     Args:
-        task_list (List[BaseTask]):
+        task_list (List[BaseTask], optional):
             Basic parameter.
             List of BaseTask in this BaseWorkflow.
+            Default to None -> [].
         critical_path_length (float, optional):
             Basic variable.
             Critical path length of PERT/CPM.
             Defaults to 0.0.
     """
 
     def __init__(
         self,
         # Basic parameters
-        task_list: List[BaseTask],
+        task_list=None,
         # Basic variables
         critical_path_length=0.0,
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.task_list = task_list
-
+        self.task_list = []
+        if task_list is not None:
+            self.extend_child_task_list(task_list)
         # ----
         # Changeable variable on simulation
         # --
         # Basic variables
         self.critical_path_length = (
             critical_path_length if critical_path_length != 0.0 else 0.0
         )
@@ -66,72 +68,188 @@
         Examples:
             >>> w = BaseWorkflow([BaseTask('t1')])
             >>> print([t.name for t in w.task_list])
             ['t1']
         """
         return "{}".format(list(map(lambda task: str(task), self.task_list)))
 
+    def append_child_task(self, task):
+        """
+        Append target task to this workflow.
+        Args:
+            task (BaseTask): target task
+        """
+        self.task_list.append(task)
+        task.parent_workflow = self
+
+    def extend_child_task_list(self, task_list):
+        """
+        Extend target task_list to this workflow.
+        Args:
+            task_list (List[BaseTask]): target task list
+        """
+        for task in task_list:
+            self.append_child_task(task)
+
     def export_dict_json_data(self):
         """
         Export the information of this workflow to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseWorkflow",
+            type=self.__class__.__name__,
             task_list=[t.export_dict_json_data() for t in self.task_list],
             critical_path_length=self.critical_path_length,
         )
         return dict_json_data
 
     def read_json_data(self, json_data):
         """
         Read the JSON data for creating BaseOrganization instance.
 
         Args:
             json_data (dict): JSON data.
         """
+        self.task_list = []
         j_list = json_data["task_list"]
-        self.task_list = [
-            BaseTask(
-                name=j["name"],
-                ID=j["ID"],
-                default_work_amount=j["default_work_amount"],
-                input_task_list=j["input_task_list"],
-                output_task_list=j["output_task_list"],
-                allocated_team_list=j["allocated_team_list"],
-                allocated_workplace_list=j["allocated_workplace_list"],
-                need_facility=j["need_facility"],
-                target_component=j["target_component"],
-                default_progress=j["default_progress"],
-                due_time=j["due_time"],
-                auto_task=j["auto_task"],
-                fixing_allocating_worker_id_list=j["fixing_allocating_worker_id_list"],
-                fixing_allocating_facility_id_list=j[
-                    "fixing_allocating_facility_id_list"
-                ],
-                # Basic variables
-                est=j["est"],
-                eft=j["eft"],
-                lst=j["lst"],
-                lft=j["lft"],
-                remaining_work_amount=j["remaining_work_amount"],
-                state=BaseTaskState(j["state"]),
-                state_record_list=[
-                    BaseTaskState(num) for num in j["state_record_list"]
-                ],
-                allocated_worker_list=j["allocated_worker_list"],
-                allocated_worker_id_record=j["allocated_worker_id_record"],
-                allocated_facility_list=j["allocated_facility_list"],
-                allocated_facility_id_record=j["allocated_facility_id_record"],
-            )
-            for j in j_list
-        ]
+        for j in j_list:
+            if j["type"] == "BaseTask":
+                self.task_list.append(
+                    BaseTask(
+                        name=j["name"],
+                        ID=j["ID"],
+                        default_work_amount=j["default_work_amount"],
+                        work_amount_progress_of_unit_step_time=j[
+                            "work_amount_progress_of_unit_step_time"
+                        ],
+                        input_task_list=j["input_task_list"],
+                        output_task_list=j["output_task_list"],
+                        allocated_team_list=j["allocated_team_list"],
+                        allocated_workplace_list=j["allocated_workplace_list"],
+                        need_facility=j["need_facility"],
+                        target_component=j["target_component"],
+                        default_progress=j["default_progress"],
+                        due_time=j["due_time"],
+                        auto_task=j["auto_task"],
+                        fixing_allocating_worker_id_list=j[
+                            "fixing_allocating_worker_id_list"
+                        ],
+                        fixing_allocating_facility_id_list=j[
+                            "fixing_allocating_facility_id_list"
+                        ],
+                        # Basic variables
+                        est=j["est"],
+                        eft=j["eft"],
+                        lst=j["lst"],
+                        lft=j["lft"],
+                        remaining_work_amount=j["remaining_work_amount"],
+                        remaining_work_amount_record_list=j[
+                            "remaining_work_amount_record_list"
+                        ],
+                        state=BaseTaskState(j["state"]),
+                        state_record_list=[
+                            BaseTaskState(num) for num in j["state_record_list"]
+                        ],
+                        allocated_worker_list=j["allocated_worker_list"],
+                        allocated_worker_id_record=j["allocated_worker_id_record"],
+                        allocated_facility_list=j["allocated_facility_list"],
+                        allocated_facility_id_record=j["allocated_facility_id_record"],
+                    )
+                )
+            elif j["type"] == "BaseSubProjectTask":
+                self.task_list.append(
+                    BaseSubProjectTask(
+                        file_path=j["file_path"],
+                        unit_timedelta=j["unit_timedelta"],
+                        read_json_file=j["read_json_file"],
+                        remove_absence_time_list=j["remove_absence_time_list"],
+                        name=j["name"],
+                        ID=j["ID"],
+                        default_work_amount=j["default_work_amount"],
+                        work_amount_progress_of_unit_step_time=j[
+                            "work_amount_progress_of_unit_step_time"
+                        ],
+                        input_task_list=j["input_task_list"],
+                        output_task_list=j["output_task_list"],
+                        allocated_team_list=j["allocated_team_list"],
+                        allocated_workplace_list=j["allocated_workplace_list"],
+                        need_facility=j["need_facility"],
+                        target_component=j["target_component"],
+                        default_progress=j["default_progress"],
+                        due_time=j["due_time"],
+                        auto_task=j["auto_task"],
+                        fixing_allocating_worker_id_list=j[
+                            "fixing_allocating_worker_id_list"
+                        ],
+                        fixing_allocating_facility_id_list=j[
+                            "fixing_allocating_facility_id_list"
+                        ],
+                        # Basic variables
+                        est=j["est"],
+                        eft=j["eft"],
+                        lst=j["lst"],
+                        lft=j["lft"],
+                        remaining_work_amount=j["remaining_work_amount"],
+                        remaining_work_amount_record_list=j[
+                            "remaining_work_amount_record_list"
+                        ],
+                        state=BaseTaskState(j["state"]),
+                        state_record_list=[
+                            BaseTaskState(num) for num in j["state_record_list"]
+                        ],
+                        allocated_worker_list=j["allocated_worker_list"],
+                        allocated_worker_id_record=j["allocated_worker_id_record"],
+                        allocated_facility_list=j["allocated_facility_list"],
+                        allocated_facility_id_record=j["allocated_facility_id_record"],
+                    )
+                )
+        # self.task_list = [
+        #     BaseTask(
+        #         name=j["name"],
+        #         ID=j["ID"],
+        #         default_work_amount=j["default_work_amount"],
+        #         work_amount_progress_of_unit_step_time=j[
+        #             "work_amount_progress_of_unit_step_time"
+        #         ],
+        #         input_task_list=j["input_task_list"],
+        #         output_task_list=j["output_task_list"],
+        #         allocated_team_list=j["allocated_team_list"],
+        #         allocated_workplace_list=j["allocated_workplace_list"],
+        #         need_facility=j["need_facility"],
+        #         target_component=j["target_component"],
+        #         default_progress=j["default_progress"],
+        #         due_time=j["due_time"],
+        #         auto_task=j["auto_task"],
+        #         fixing_allocating_worker_id_list=j["fixing_allocating_worker_id_list"],
+        #         fixing_allocating_facility_id_list=j[
+        #             "fixing_allocating_facility_id_list"
+        #         ],
+        #         # Basic variables
+        #         est=j["est"],
+        #         eft=j["eft"],
+        #         lst=j["lst"],
+        #         lft=j["lft"],
+        #         remaining_work_amount=j["remaining_work_amount"],
+        #         remaining_work_amount_record_list=j[
+        #             "remaining_work_amount_record_list"
+        #         ],
+        #         state=BaseTaskState(j["state"]),
+        #         state_record_list=[
+        #             BaseTaskState(num) for num in j["state_record_list"]
+        #         ],
+        #         allocated_worker_list=j["allocated_worker_list"],
+        #         allocated_worker_id_record=j["allocated_worker_id_record"],
+        #         allocated_facility_list=j["allocated_facility_list"],
+        #         allocated_facility_id_record=j["allocated_facility_id_record"],
+        #     )
+        #     for j in j_list
+        # ]
 
         self.critical_path_length = json_data["critical_path_length"]
 
     def extract_none_task_list(self, target_time_list):
         """
         Extract NONE task list from simulation result.
 
@@ -557,32 +675,46 @@
             filter(
                 lambda task: task.state == BaseTaskState.READY
                 and len(task.allocated_worker_list) > 0,
                 self.task_list,
             )
         )
 
-        ready_auto_task_set = set(
+        ready_auto_task_without_component_set = set(
             filter(
-                lambda task: task.state == BaseTaskState.READY and task.auto_task,
+                lambda task: task.state == BaseTaskState.READY
+                and task.auto_task
+                and task.target_component is None,
+                self.task_list,
+            )
+        )
+
+        ready_auto_task_with_component_set = set(
+            filter(
+                lambda task: task.state == BaseTaskState.READY
+                and task.auto_task
+                and task.target_component is not None
+                and task.target_component.placed_workplace
+                in task.allocated_workplace_list,
                 self.task_list,
             )
         )
 
         working_and_assigned_task_set = set(
             filter(
                 lambda task: task.state == BaseTaskState.WORKING
                 and len(task.allocated_worker_list) > 0,
                 self.task_list,
             )
         )
 
         target_task_set = set()
         target_task_set.update(ready_and_assigned_task_set)
-        target_task_set.update(ready_auto_task_set)
+        target_task_set.update(ready_auto_task_without_component_set)
+        target_task_set.update(ready_auto_task_with_component_set)
         target_task_set.update(working_and_assigned_task_set)
 
         for task in target_task_set:
             if task.state == BaseTaskState.READY:
                 task.state = BaseTaskState.WORKING
                 for worker in task.allocated_worker_list:
                     worker.state = BaseWorkerState.WORKING
@@ -634,29 +766,29 @@
                         finished = False
                         break
             if finished:
                 task.state = BaseTaskState.FINISHED
                 task.remaining_work_amount = 0.0
 
                 for worker in task.allocated_worker_list:
-                    if all(
+                    if len(worker.assigned_task_list) > 0 and all(
                         list(
                             map(
                                 lambda task: task.state == BaseTaskState.FINISHED,
                                 worker.assigned_task_list,
                             )
                         )
                     ):
                         worker.state = BaseWorkerState.FREE
                         worker.assigned_task_list.remove(task)
                 task.allocated_worker_list = []
 
                 if task.need_facility:
                     for facility in task.allocated_facility_list:
-                        if all(
+                        if len(facility.assigned_task_list) > 0 and all(
                             list(
                                 map(
                                     lambda task: task.state == BaseTaskState.FINISHED,
                                     facility.assigned_task_list,
                                 )
                             )
                         ):
@@ -777,34 +909,45 @@
         # Register the dummy_input_task_list to input_task_list
         # Delete the dummy_output_task_list, dummy_input_task_list
         for task in self.task_list:
             task.output_task_list = task.dummy_output_task_list
             task.input_task_list = task.dummy_input_task_list
             del task.dummy_output_task_list, task.dummy_input_task_list
 
-    def perform(self, time: int, only_auto_task=False, seed=None):
+    def perform(
+        self, time: int, only_auto_task=False, seed=None, increase_component_error=1.0
+    ):
         """
         Perform BaseTask in task_list in simulation.
 
         Args:
             time (int):
                 Simulation time.
             only_auto_task (bool, optional):
                 Perform only auto task or not.
                 Defaults to False.
             seed (int, optional):
                 Random seed for describing deviation of progress.
                 Defaults to None.
+            increase_component_error (float, optional):
+                For advanced simulation.
+                Increment error value when error has occurred.
+                Defaults to 1.0.
+        Note:
+            This method includes advanced code of custom simulation.
+            We have to separete basic code and advanced code in the future.
         """
         for task in self.task_list:
             if only_auto_task:
                 if task.auto_task:
                     task.perform(time, seed=seed)
             else:
-                task.perform(time, seed=seed)
+                task.perform(
+                    time, seed=seed, increase_component_error=increase_component_error
+                )
 
     def remove_absence_time_list(self, absence_time_list):
         """
         Remove record information on `absence_time_list`.
 
         Args:
             absence_time_list (List[int]):
```

### Comparing `pDESy-0.4.9/pDESy/model/base_workplace.py` & `pDESy-0.5.0/pDESy/model/base_workplace.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 class BaseWorkplace(object, metaclass=abc.ABCMeta):
     """BaseWorkplace.
 
     BaseWorkplace class for expressing workplace including facilities in a project.
     This class will be used as template.
 
     Args:
-        name (str):
+        name (str, optional):
             Basic parameter.
             Name of this workplace.
+            Defaults to None -> "New Workplace"
         ID (str, optional):
             Basic parameter.
             ID will be defined automatically.
             Defaults to None -> str(uuid.uuid4()).
         facility_list (List[BaseFacility], optional):
             Basic parameter.
             List of BaseFacility who belong to this workplace.
@@ -66,15 +67,15 @@
             History or record of this workplace's cost in simulation.
             Defaults to None -> [].
     """
 
     def __init__(
         self,
         # Basic parameters
-        name: str,
+        name=None,
         ID=None,
         facility_list=None,
         targeted_task_list=None,
         parent_workplace=None,
         max_space_size=None,
         input_workplace_list=None,
         output_workplace_list=None,
@@ -84,15 +85,15 @@
         placed_component_id_record=None,
     ):
         """init."""
         # ----
         # Constraint parameter on simulation
         # --
         # Basic parameter
-        self.name = name
+        self.name = name if name is not None else "New Workplace"
         self.ID = ID if ID is not None else str(uuid.uuid4())
 
         self.facility_list = facility_list if facility_list is not None else []
         for facility in self.facility_list:
             if facility.workplace_id is None:
                 facility.workplace_id = self.ID
 
@@ -406,15 +407,15 @@
         Export the information of this workplace to JSON data.
 
         Returns:
             dict: JSON format data.
         """
         dict_json_data = {}
         dict_json_data.update(
-            type="BaseWorkplace",
+            type=self.__class__.__name__,
             name=self.name,
             ID=self.ID,
             facility_list=[f.export_dict_json_data() for f in self.facility_list],
             targeted_task_list=[t.ID for t in self.targeted_task_list],
             parent_workplace=self.parent_workplace.ID
             if self.parent_workplace is not None
             else None,
```

### Comparing `pDESy-0.4.9/pyproject.toml` & `pDESy-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pDESy"
-version = "0.4.9"
+version = "0.5.0"
 description = "pDESy: Discrete Event Simulation of Python"
 authors = ["Taiga MITSUYUKI <mitsuyuki-taiga-my@ynu.ac.jp>"]
 maintainers = ["Taiga MITSUYUKI <mitsuyuki-taiga-my@ynu.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pDESy/pDESy"
 packages = [
@@ -16,15 +16,14 @@
 python = "^3.8"
 numpy = "^1.22.4"
 networkx = "^2.8"
 plotly = "^5.8.2"
 pytest-cov = "^3.0.0"
 matplotlib = "^3.5.1"
 coverage = "^6.3.2"
-codecov = "^2.1.12"
 poetry = "^1.1.13"
 Pillow = "^9.1.0"
 decorator = "^5.1.1"
 
 [tool.poetry.dev-dependencies]
 black = "^19.10b0"
 flake8 = "^3.8.2"
```

### Comparing `pDESy-0.4.9/setup.py` & `pDESy-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 ['pDESy', 'pDESy.model']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.1.0,<10.0.0',
- 'codecov>=2.1.12,<3.0.0',
  'coverage>=6.3.2,<7.0.0',
  'decorator>=5.1.1,<6.0.0',
  'matplotlib>=3.5.1,<4.0.0',
  'networkx>=2.8,<3.0',
  'numpy>=1.22.4,<2.0.0',
  'plotly>=5.8.2,<6.0.0',
  'poetry>=1.1.13,<2.0.0',
  'pytest-cov>=3.0.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'pdesy',
-    'version': '0.4.9',
+    'version': '0.5.0',
     'description': 'pDESy: Discrete Event Simulation of Python',
-    'long_description': "# pDESy: Discrete-Event Simulator in Python\n\n[![PyPi version](https://pypip.in/v/pDESy/badge.png)](https://pypi.org/project/pDESy/)\n[![Anaconda-Server Badge](https://anaconda.org/taiga4112/pdesy/badges/version.svg)](https://anaconda.org/taiga4112/pdesy)\n![test](https://github.com/pDESy/pDESy/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/pDESy/pDESy/branch/master/graph/badge.svg)](https://codecov.io/gh/pDESy/pDESy)\n\n## What is it?\n\n**pDESy** is a Python package of Discrete-Event Simulator (DES). It aims to be the fundamental high-level building block for doing practical, real world engineering project management by using DES and other DES modeling tools. **pDESy** has only the function of discrete-event simulation, does not include the function of visual modeling.\n\n\n## Where to get it\nThe source code is currently hosted on GitHub at: [https://github.com/pDESy/pDESy](https://github.com/pDESy/pDESy)\n\nBinary installers for the latest released version will be available at the Python package index. Now, please install pDESy as following.\n\n```sh\npip install pDESy\n# pip install git+ssh://git@github.com/pDESy/pDESy.git # INSTALL FROM GITHUB\n# conda install -c conda-forge -c taiga4112 pDESy # INSTALL FROM ANACONDA\n```\n\n## License\n[MIT](https://github.com/pDESy/pDESy/blob/master/LICENSE)\n\n## Documentation\nAPI Documentation is [https://pDESy.github.io/pDESy/index.html](https://pDESy.github.io/pDESy/index.html).\n\n## Background\n**pDESy** is developed by a part of next generation DES tool of **[pDES](https://github.com/pDESy/pDES)**.\n\n## Contribution\n1. Fork it ( http://github.com/pDESy/pDESy/fork )\n2. Create your feature branch (git checkout -b my-new-feature)\n3. Commit your changes (git commit -am 'Add some feature')\n4. Push to the branch (git push origin my-new-feature)\n5. Create new Pull Request\n\nIf you want to join this project as a researcher, please contact [me](https://github.com/taiga4112).",
+    'long_description': "# pDESy: Discrete-Event Simulator in Python\n\n[![PyPI version](https://badge.fury.io/py/pDESy.svg)](https://badge.fury.io/py/pDESy)\n[![Anaconda-Server Badge](https://anaconda.org/taiga4112/pdesy/badges/version.svg)](https://anaconda.org/taiga4112/pdesy)\n![test](https://github.com/pDESy/pDESy/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/pDESy/pDESy/branch/master/graph/badge.svg)](https://codecov.io/gh/pDESy/pDESy)\n\n## What is it?\n\n**pDESy** is a Python package of Discrete-Event Simulator (DES). It aims to be the fundamental high-level building block for doing practical, real world engineering project management by using DES and other DES modeling tools. **pDESy** has only the function of discrete-event simulation, does not include the function of visual modeling.\n\n\n## Where to get it\nThe source code is currently hosted on GitHub at: [https://github.com/pDESy/pDESy](https://github.com/pDESy/pDESy)\n\nBinary installers for the latest released version will be available at the Python package index. Now, please install pDESy as following.\n\n```sh\npip install pDESy\n# pip install git+ssh://git@github.com/pDESy/pDESy.git # INSTALL FROM GITHUB\n# conda install -c conda-forge -c taiga4112 pDESy # INSTALL FROM ANACONDA\n```\n\n## License\n[MIT](https://github.com/pDESy/pDESy/blob/master/LICENSE)\n\n## Documentation\nAPI Documentation is [https://pDESy.github.io/pDESy/index.html](https://pDESy.github.io/pDESy/index.html).\n\n## Background\n**pDESy** is developed by a part of next generation DES tool of **[pDES](https://github.com/pDESy/pDES)**.\n\n## Contribution\n1. Fork it ( http://github.com/pDESy/pDESy/fork )\n2. Create your feature branch (git checkout -b my-new-feature)\n3. Commit your changes (git commit -am 'Add some feature')\n4. Push to the branch (git push origin my-new-feature)\n5. Create new Pull Request\n\nIf you want to join this project as a researcher, please contact [me](https://github.com/taiga4112).",
     'author': 'Taiga MITSUYUKI',
     'author_email': 'mitsuyuki-taiga-my@ynu.ac.jp',
     'maintainer': 'Taiga MITSUYUKI',
     'maintainer_email': 'mitsuyuki-taiga-my@ynu.ac.jp',
     'url': 'https://github.com/pDESy/pDESy',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pDESy-0.4.9/PKG-INFO` & `pDESy-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: pdesy
-Version: 0.4.9
+Version: 0.5.0
 Summary: pDESy: Discrete Event Simulation of Python
 Home-page: https://github.com/pDESy/pDESy
 License: MIT
 Author: Taiga MITSUYUKI
 Author-email: mitsuyuki-taiga-my@ynu.ac.jp
 Maintainer: Taiga MITSUYUKI
 Maintainer-email: mitsuyuki-taiga-my@ynu.ac.jp
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Pillow (>=9.1.0,<10.0.0)
-Requires-Dist: codecov (>=2.1.12,<3.0.0)
 Requires-Dist: coverage (>=6.3.2,<7.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: networkx (>=2.8,<3.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: plotly (>=5.8.2,<6.0.0)
 Requires-Dist: poetry (>=1.1.13,<2.0.0)
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/pDESy/pDESy
 Description-Content-Type: text/markdown
 
 # pDESy: Discrete-Event Simulator in Python
 
-[![PyPi version](https://pypip.in/v/pDESy/badge.png)](https://pypi.org/project/pDESy/)
+[![PyPI version](https://badge.fury.io/py/pDESy.svg)](https://badge.fury.io/py/pDESy)
 [![Anaconda-Server Badge](https://anaconda.org/taiga4112/pdesy/badges/version.svg)](https://anaconda.org/taiga4112/pdesy)
 ![test](https://github.com/pDESy/pDESy/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/pDESy/pDESy/branch/master/graph/badge.svg)](https://codecov.io/gh/pDESy/pDESy)
 
 ## What is it?
 
 **pDESy** is a Python package of Discrete-Event Simulator (DES). It aims to be the fundamental high-level building block for doing practical, real world engineering project management by using DES and other DES modeling tools. **pDESy** has only the function of discrete-event simulation, does not include the function of visual modeling.
```

