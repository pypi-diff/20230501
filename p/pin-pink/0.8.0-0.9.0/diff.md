# Comparing `tmp/pin-pink-0.8.0.tar.gz` & `tmp/pin-pink-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pin-pink-0.8.0.tar", last modified: Thu Feb  9 18:44:44 2023, max compression
+gzip compressed data, was "pin-pink-0.9.0.tar", last modified: Wed Mar 15 15:18:41 2023, max compression
```

## Comparing `pin-pink-0.8.0.tar` & `pin-pink-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,66 @@
--rw-r--r--   0        0        0     2651 2023-01-16 16:18:53.687730 pin-pink-0.8.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       77 2022-03-29 17:10:57.272648 pin-pink-0.8.0/.gitignore
--rw-r--r--   0        0        0     3752 2023-02-09 18:26:04.874017 pin-pink-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     2179 2023-01-16 13:21:07.602604 pin-pink-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2022-03-17 19:43:10.215116 pin-pink-0.8.0/LICENSE
--rw-r--r--   0        0        0     7358 2023-02-09 18:17:01.743702 pin-pink-0.8.0/README.md
--rw-r--r--   0        0        0     1174 2023-02-06 18:17:12.808634 pin-pink-0.8.0/doc/Makefile
--rw-r--r--   0        0        0     9828 2023-01-16 13:21:07.602604 pin-pink-0.8.0/doc/src/conf.py
--rw-r--r--   0        0        0      968 2022-03-04 11:43:18.830659 pin-pink-0.8.0/doc/src/css/custom.css
--rw-r--r--   0        0        0      459 2023-01-18 10:53:20.570424 pin-pink-0.8.0/doc/src/developer-notes.rst
--rw-r--r--   0        0        0    16030 2022-06-09 08:51:10.698591 pin-pink-0.8.0/doc/src/images/apple-touch-icon-180x180.png
--rw-r--r--   0        0        0     1013 2022-06-09 08:51:10.698591 pin-pink-0.8.0/doc/src/images/favicon-16x16.png
--rw-r--r--   0        0        0     1766 2022-06-09 08:51:10.698591 pin-pink-0.8.0/doc/src/images/favicon-32x32.png
--rw-r--r--   0        0        0    18638 2022-06-09 08:51:10.698591 pin-pink-0.8.0/doc/src/images/pink-round-corners-140x140.png
--rw-r--r--   0        0        0     1055 2023-01-16 16:18:53.687730 pin-pink-0.8.0/doc/src/index.rst
--rw-r--r--   0        0        0      685 2023-01-30 15:14:07.609694 pin-pink-0.8.0/doc/src/installation.rst
--rw-r--r--   0        0        0     1930 2023-01-16 16:18:53.687730 pin-pink-0.8.0/doc/src/introduction.rst
--rw-r--r--   0        0        0      899 2023-01-17 17:50:59.688578 pin-pink-0.8.0/doc/src/inverse-kinematics.rst
--rw-r--r--   0        0        0      189 2023-02-09 17:42:38.420493 pin-pink-0.8.0/doc/src/joint-limits.rst
--rw-r--r--   0        0        0      313 2023-01-16 16:18:53.687730 pin-pink-0.8.0/doc/src/tasks.rst
--rw-r--r--   0        0        0     3190 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/arm_kinova_gen2.py
--rw-r--r--   0        0        0     3232 2023-01-31 16:26:48.105196 pin-pink-0.8.0/examples/arm_ur3.py
--rw-r--r--   0        0        0     3082 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/double_pendulum.py
--rw-r--r--   0        0        0     4545 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/humanoid_jvrc.py
--rw-r--r--   0        0        0     4011 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/humanoid_sigmaban.py
--rw-r--r--   0        0        0     1303 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/load_custom_urdf.py
--rw-r--r--   0        0        0     3322 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/meshcat_shapes.py
--rw-r--r--   0        0        0     3070 2023-02-06 18:21:43.693511 pin-pink-0.8.0/examples/omnidirectional_wheeled_robot.py
--rw-r--r--   0        0        0     4719 2023-01-16 16:18:53.687730 pin-pink-0.8.0/examples/robots/double_pendulum.urdf
--rw-r--r--   0        0        0     2425 2023-02-06 18:21:43.693511 pin-pink-0.8.0/examples/robots/omnidirectional_wheeled_robot.urdf
--rw-r--r--   0        0        0     3961 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/visualize_in_meshcat.py
--rw-r--r--   0        0        0     3798 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/visualize_in_yourdfpy.py
--rw-r--r--   0        0        0     3904 2023-01-30 15:14:07.609694 pin-pink-0.8.0/examples/wheeled_biped_upkie.py
--rw-r--r--   0        0        0     1109 2023-02-09 18:17:34.331121 pin-pink-0.8.0/pink/__init__.py
--rw-r--r--   0        0        0     2644 2023-02-09 17:42:38.420493 pin-pink-0.8.0/pink/bounded_tangent.py
--rw-r--r--   0        0        0     7196 2023-02-09 17:42:38.420493 pin-pink-0.8.0/pink/configuration.py
--rw-r--r--   0        0        0     1971 2023-01-30 15:13:45.729252 pin-pink-0.8.0/pink/exceptions.py
--rw-r--r--   0        0        0     3251 2023-02-09 17:42:38.420493 pin-pink-0.8.0/pink/limits.py
--rw-r--r--   0        0        0     6145 2023-02-09 17:42:38.420493 pin-pink-0.8.0/pink/solve_ik.py
--rw-r--r--   0        0        0      865 2023-01-30 15:13:45.729252 pin-pink-0.8.0/pink/tasks/__init__.py
--rw-r--r--   0        0        0    10869 2023-02-01 14:28:01.871229 pin-pink-0.8.0/pink/tasks/body_task.py
--rw-r--r--   0        0        0      808 2023-01-30 15:13:45.733252 pin-pink-0.8.0/pink/tasks/exceptions.py
--rw-r--r--   0        0        0     5160 2023-01-30 15:13:45.733252 pin-pink-0.8.0/pink/tasks/posture_task.py
--rw-r--r--   0        0        0     3762 2023-01-30 15:13:45.733252 pin-pink-0.8.0/pink/tasks/task.py
--rw-r--r--   0        0        0     3575 2023-01-30 15:14:07.609694 pin-pink-0.8.0/pink/tasks/utils.py
--rw-r--r--   0        0        0     3001 2023-01-30 15:13:45.733252 pin-pink-0.8.0/pink/utils.py
--rw-r--r--   0        0        0     1128 2023-01-30 15:13:45.733252 pin-pink-0.8.0/pink/visualization.py
--rw-r--r--   0        0        0     1725 2023-01-30 15:14:07.609694 pin-pink-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      705 2022-03-17 19:45:00.229277 pin-pink-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     8571 2023-02-01 14:28:01.871229 pin-pink-0.8.0/tests/test_body_task.py
--rw-r--r--   0        0        0     2422 2023-02-09 17:42:38.424493 pin-pink-0.8.0/tests/test_bounded_tangent.py
--rw-r--r--   0        0        0    13580 2023-01-17 17:50:59.688578 pin-pink-0.8.0/tests/test_configuration.py
--rw-r--r--   0        0        0     2625 2023-02-01 14:28:01.871229 pin-pink-0.8.0/tests/test_jacobians.py
--rw-r--r--   0        0        0     4070 2023-02-09 17:42:38.424493 pin-pink-0.8.0/tests/test_limits.py
--rw-r--r--   0        0        0     4138 2023-01-17 17:50:59.688578 pin-pink-0.8.0/tests/test_posture_task.py
--rw-r--r--   0        0        0    11934 2023-01-17 17:50:59.688578 pin-pink-0.8.0/tests/test_solve_ik.py
--rw-r--r--   0        0        0     1073 2022-04-04 12:32:05.841277 pin-pink-0.8.0/tests/test_task.py
--rw-r--r--   0        0        0     1771 2023-01-30 15:14:07.609694 pin-pink-0.8.0/tests/test_utils.py
--rw-r--r--   0        0        0     1389 2023-02-09 17:42:38.424493 pin-pink-0.8.0/tox.ini
--rw-r--r--   0        0        0     8701 1970-01-01 00:00:00.000000 pin-pink-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2651 2023-01-16 16:18:53.687730 pin-pink-0.9.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       77 2022-03-29 17:10:57.272648 pin-pink-0.9.0/.gitignore
+-rw-r--r--   0        0        0     4202 2023-03-15 15:17:39.664479 pin-pink-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2179 2023-02-28 10:12:07.208660 pin-pink-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2022-03-17 19:43:10.215116 pin-pink-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7614 2023-02-20 10:04:19.588236 pin-pink-0.9.0/README.md
+-rw-r--r--   0        0        0     1174 2023-02-28 10:12:07.212659 pin-pink-0.9.0/doc/Makefile
+-rw-r--r--   0        0        0     9828 2023-02-28 10:53:36.903715 pin-pink-0.9.0/doc/src/conf.py
+-rw-r--r--   0        0        0      968 2022-03-04 11:43:18.830659 pin-pink-0.9.0/doc/src/css/custom.css
+-rw-r--r--   0        0        0      459 2023-01-18 10:53:20.570424 pin-pink-0.9.0/doc/src/developer-notes.rst
+-rw-r--r--   0        0        0    16030 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/apple-touch-icon-180x180.png
+-rw-r--r--   0        0        0     1013 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1766 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/favicon-32x32.png
+-rw-r--r--   0        0        0    18638 2022-06-09 08:51:10.698591 pin-pink-0.9.0/doc/src/images/pink-round-corners-140x140.png
+-rw-r--r--   0        0        0     1074 2023-02-28 10:12:07.212659 pin-pink-0.9.0/doc/src/index.rst
+-rw-r--r--   0        0        0      685 2023-01-30 15:14:07.609694 pin-pink-0.9.0/doc/src/installation.rst
+-rw-r--r--   0        0        0     1930 2023-01-16 16:18:53.687730 pin-pink-0.9.0/doc/src/introduction.rst
+-rw-r--r--   0        0        0      844 2023-02-13 15:06:54.714801 pin-pink-0.9.0/doc/src/inverse-kinematics.rst
+-rw-r--r--   0        0        0      189 2023-02-28 10:12:07.212659 pin-pink-0.9.0/doc/src/joint-limits.rst
+-rw-r--r--   0        0        0      631 2023-02-22 16:16:17.624447 pin-pink-0.9.0/doc/src/references.rst
+-rw-r--r--   0        0        0      546 2023-03-15 15:13:51.505077 pin-pink-0.9.0/doc/src/tasks.rst
+-rw-r--r--   0        0        0     3194 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/arm_kinova_gen2.py
+-rw-r--r--   0        0        0     3236 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/arm_ur3.py
+-rw-r--r--   0        0        0     3053 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/double_pendulum.py
+-rw-r--r--   0        0        0     5285 2023-03-15 15:13:51.505077 pin-pink-0.9.0/examples/humanoid_draco3.py
+-rw-r--r--   0        0        0     4516 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/humanoid_jvrc.py
+-rw-r--r--   0        0        0     3982 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/humanoid_sigmaban.py
+-rw-r--r--   0        0        0     1303 2023-01-30 15:14:07.609694 pin-pink-0.9.0/examples/load_custom_urdf.py
+-rw-r--r--   0        0        0     3322 2023-01-30 15:14:07.609694 pin-pink-0.9.0/examples/meshcat_shapes.py
+-rw-r--r--   0        0        0     3041 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/omnidirectional_wheeled_robot.py
+-rw-r--r--   0        0        0     4719 2023-01-16 16:18:53.687730 pin-pink-0.9.0/examples/robots/double_pendulum.urdf
+-rw-r--r--   0        0        0     2425 2023-02-13 15:05:40.152104 pin-pink-0.9.0/examples/robots/omnidirectional_wheeled_robot.urdf
+-rw-r--r--   0        0        0     3932 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/visualize_in_meshcat.py
+-rw-r--r--   0        0        0     3755 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/visualize_in_yourdfpy.py
+-rw-r--r--   0        0        0     3875 2023-02-13 15:06:54.714801 pin-pink-0.9.0/examples/wheeled_biped_upkie.py
+-rw-r--r--   0        0        0      994 2023-03-15 15:17:32.616621 pin-pink-0.9.0/pink/__init__.py
+-rw-r--r--   0        0        0     2644 2023-02-28 10:12:07.212659 pin-pink-0.9.0/pink/bounded_tangent.py
+-rw-r--r--   0        0        0     7422 2023-02-28 10:12:07.216659 pin-pink-0.9.0/pink/configuration.py
+-rw-r--r--   0        0        0     1971 2023-03-15 14:58:57.683088 pin-pink-0.9.0/pink/exceptions.py
+-rw-r--r--   0        0        0     3251 2023-02-28 10:12:07.216659 pin-pink-0.9.0/pink/limits.py
+-rw-r--r--   0        0        0     6145 2023-02-28 10:12:07.216659 pin-pink-0.9.0/pink/solve_ik.py
+-rw-r--r--   0        0        0     1069 2023-03-15 15:13:51.505077 pin-pink-0.9.0/pink/tasks/__init__.py
+-rw-r--r--   0        0        0    10897 2023-02-28 10:53:36.903715 pin-pink-0.9.0/pink/tasks/body_task.py
+-rw-r--r--   0        0        0      926 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/tasks/exceptions.py
+-rw-r--r--   0        0        0     1919 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/tasks/joint_coupling_task.py
+-rw-r--r--   0        0        0     5955 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/tasks/linear_holonomic_task.py
+-rw-r--r--   0        0        0     5318 2023-02-20 10:04:19.588236 pin-pink-0.9.0/pink/tasks/posture_task.py
+-rw-r--r--   0        0        0     4431 2023-02-20 10:04:19.588236 pin-pink-0.9.0/pink/tasks/task.py
+-rw-r--r--   0        0        0     3575 2023-01-30 15:14:07.609694 pin-pink-0.9.0/pink/tasks/utils.py
+-rw-r--r--   0        0        0     3629 2023-03-15 15:13:51.509077 pin-pink-0.9.0/pink/utils.py
+-rw-r--r--   0        0        0     1128 2023-01-30 15:13:45.733252 pin-pink-0.9.0/pink/visualization.py
+-rw-r--r--   0        0        0     1725 2023-01-30 15:14:07.609694 pin-pink-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      705 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     8713 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/test_body_task.py
+-rw-r--r--   0        0        0     2422 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/test_bounded_tangent.py
+-rw-r--r--   0        0        0    14718 2023-02-28 10:12:07.220660 pin-pink-0.9.0/tests/test_configuration.py
+-rw-r--r--   0        0        0     2660 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_jacobians.py
+-rw-r--r--   0        0        0     2997 2023-03-15 15:13:51.509077 pin-pink-0.9.0/tests/test_joint_coupling_task.py
+-rw-r--r--   0        0        0     4148 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_limits.py
+-rw-r--r--   0        0        0     4706 2023-03-15 15:13:51.509077 pin-pink-0.9.0/tests/test_linear_holonomic_task.py
+-rw-r--r--   0        0        0     4331 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_posture_task.py
+-rw-r--r--   0        0        0    11941 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_solve_ik.py
+-rw-r--r--   0        0        0     1073 2023-02-28 10:12:07.224660 pin-pink-0.9.0/tests/test_task.py
+-rw-r--r--   0        0        0     1771 2023-02-28 10:12:07.228659 pin-pink-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1389 2023-03-15 15:13:51.509077 pin-pink-0.9.0/tox.ini
+-rw-r--r--   0        0        0     8957 1970-01-01 00:00:00.000000 pin-pink-0.9.0/PKG-INFO
```

### Comparing `pin-pink-0.8.0/.github/workflows/main.yml` & `pin-pink-0.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/CHANGELOG.md` & `pin-pink-0.9.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.9.0] - 2023/03/15
+
+### Added
+
+- Example: Draco 3 humanoid by @shbang91
+- Joint-coupling task by @shbang91
+- Linear holonomic task by @shbang91
+- Unit tests for joint-coupling and linear holonomic tasks by @shbang91
+
+### Changed
+
+- Refactor ``apply_configuration`` into ``Configuration`` constructor
+- Refactor ``assume_configuration`` into ``Configuration`` constructor
+- Refactor task dynamics into ``compute_error`` and ``compute_jacobian``
+
 ## [0.8.0] - 2023/02/09
 
 ### Added
 
 - BodyNotFound exception
 - Document spatial and body minus between transforms
 - Example: SigmaBan humanoid
```

### Comparing `pin-pink-0.8.0/CONTRIBUTING.md` & `pin-pink-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/LICENSE` & `pin-pink-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/README.md` & `pin-pink-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 Body tasks can be initialized, for example, from the robot's neutral configuration:
 
 ```python
 import pink
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 robot = load_robot_description("upkie_description")
-configuration = pink.apply_configuration(robot, robot.q0)
+configuration = pink.Configuration(robot.model, robot.data, robot.q0)
 for body, task in tasks.items():
     if type(task) is BodyTask:
         task.set_target(configuration.get_transform_body_to_world(body))
 ```
 
 A task can be added to the inverse kinematics once both its cost and target (if applicable) are defined.
 
@@ -104,42 +104,46 @@
 
 Pink solves differential inverse kinematics, meaning it outputs a velocity that steers the robot towards achieving all tasks at best. If we keep integrating that velocity, and task targets don't change over time, we will converge to a stationary configuration:
 
 ```python
 dt = 6e-3  # [s]
 for t in np.arange(0.0, 42.0, dt):
     velocity = solve_ik(configuration, tasks.values(), dt, solver="quadprog")
-    q = configuration.integrate(velocity, dt)
-    configuration = pink.apply_configuration(robot, q)
+    configuration.integrate_inplace(velocity, dt)
     time.sleep(dt)
 ```
 
 If task targets are continuously updated, there will be no stationary solution to converge to, but the model will keep on tracking each target at best. Note that [`solve_ik`](https://scaron.info/doc/pink/inverse-kinematics.html#pink.solve_ik.solve_ik) will take care of both configuration and velocity limits read from the robot model.
 
 ## Examples
 
-Pink works with all kinds of robot morphologies:
-
-* Arm: [Kinova Gen2](https://github.com/tasts-robots/pink/blob/master/examples/arm_kinova_gen2.py)
-* Arm: [UR3](https://github.com/tasts-robots/pink/blob/master/examples/arm_ur3.py)
-* Humanoid: [JVRC-1](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_jvrc.py)
-* Humanoid: [SigmaBan](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_sigmaban.py)
-* Wheeled biped: [Upkie](https://github.com/tasts-robots/pink/blob/master/examples/wheeled_biped_upkie.py)
-* Wheeled: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/omnidirectional_wheeled_robot.py)
-
-Basic examples are the best to get started:
+Basic examples to get started:
 
 * [Double pendulum](https://github.com/tasts-robots/pink/blob/master/examples/double_pendulum.py)
 * [Loading a custom URDF](https://github.com/tasts-robots/pink/blob/master/examples/load_custom_urdf.py)
 * [Visualization in MeshCat](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_meshcat.py)
 * [Visualization in yourdfpy](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_yourdfpy.py)
 
+Pink works with all kinds of robot morphologies:
+
+* Arms: [Kinova Gen2](https://github.com/tasts-robots/pink/blob/master/examples/arm_kinova_gen2.py), [UR3](https://github.com/tasts-robots/pink/blob/master/examples/arm_ur3.py)
+* Humanoids: [JVRC-1](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_jvrc.py), [SigmaBan](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_sigmaban.py)
+* Wheeled biped: [Upkie](https://github.com/tasts-robots/pink/blob/master/examples/wheeled_biped_upkie.py)
+* Wheeled: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/omnidirectional_wheeled_robot.py)
+
 Check out the [examples](https://github.com/tasts-robots/pink/tree/master/examples) folder for more.
 
 ## How can I help?
 
 Install the library and use it! Report bugs in the [issue tracker](https://github.com/tasts-robots/pink/issues). If you are a developer with some robotics experience looking to hack on open source, check out the [contribution guidelines](CONTRIBUTING.md).
 
 ## See also
 
+Software:
+
 - [Jink.jl](https://github.com/adubredu/Jink.jl): Julia package for differential multi-task inverse kinematics.
 - [pymanoid](https://github.com/stephane-caron/pymanoid): precursor to Pink based on OpenRAVE.
+
+Technical notes:
+
+- [Inverse kinematics](https://scaron.info/robotics/inverse-kinematics.html): a general introduction to differential inverse kinematics.
+- [Jacobian of a kinematic task and derivatives on manifolds](https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html).
```

### Comparing `pin-pink-0.8.0/doc/Makefile` & `pin-pink-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/conf.py` & `pin-pink-0.9.0/doc/src/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             break
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #
 # today = ''
 #
 # Else, today_fmt is used as the format for a strftime call.
```

### Comparing `pin-pink-0.8.0/doc/src/css/custom.css` & `pin-pink-0.9.0/doc/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/images/apple-touch-icon-180x180.png` & `pin-pink-0.9.0/doc/src/images/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/images/favicon-16x16.png` & `pin-pink-0.9.0/doc/src/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/images/favicon-32x32.png` & `pin-pink-0.9.0/doc/src/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/images/pink-round-corners-140x140.png` & `pin-pink-0.9.0/doc/src/images/pink-round-corners-140x140.png`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/index.rst` & `pin-pink-0.9.0/doc/src/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 
     installation.rst
     introduction.rst
     tasks.rst
     joint-limits.rst
     inverse-kinematics.rst
     developer-notes.rst
+    references.rst
 
 You can also download this documentation as a `PDF document <pink.pdf>`_.
```

### Comparing `pin-pink-0.8.0/doc/src/installation.rst` & `pin-pink-0.9.0/doc/src/installation.rst`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/introduction.rst` & `pin-pink-0.9.0/doc/src/introduction.rst`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/doc/src/inverse-kinematics.rst` & `pin-pink-0.9.0/doc/src/inverse-kinematics.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 .. code:: python
 
     rate = RateLimiter(frequency=100.0)
     while True:
         # [...] <- update task targets here
         velocity = solve_ik(configuration, tasks, rate.dt, solver=solver)
-        q = configuration.integrate(velocity, rate.dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, rate.dt)
         rate.sleep()
 
 See the ``examples/`` folder in the repository for complete use cases.
 
 .. autofunction:: pink.solve_ik.solve_ik
 
 It is also possible to ask Pink to only build the underlying inverse kinematics
```

### Comparing `pin-pink-0.8.0/examples/arm_kinova_gen2.py` & `pin-pink-0.9.0/examples/arm_kinova_gen2.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,18 +49,21 @@
 
     posture_task = PostureTask(
         cost=1e-3,  # [cost] / [rad]
     )
 
     tasks = [end_effector_task, posture_task]
 
-    q = custom_configuration_vector(
-        robot, j2s6s200_joint_2=1.0, j2s6s200_joint_3=1.0, j2s6s200_joint_5=1.0
+    q_ref = custom_configuration_vector(
+        robot,
+        j2s6s200_joint_2=1.0,
+        j2s6s200_joint_3=1.0,
+        j2s6s200_joint_5=1.0,
     )
-    configuration = pink.apply_configuration(robot, q)
+    configuration = pink.Configuration(robot.model, robot.data, q_ref)
     for task in tasks:
         task.set_target_from_configuration(configuration)
     viz.display(configuration.q)
 
     viewer = viz.viewer
     meshcat_shapes.frame(viewer["end_effector_target"], opacity=0.5)
     meshcat_shapes.frame(viewer["end_effector"], opacity=1.0)
@@ -85,14 +88,13 @@
             configuration.get_transform_body_to_world(
                 end_effector_task.body
             ).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/arm_ur3.py` & `pin-pink-0.9.0/examples/arm_ur3.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,21 @@
 
     posture_task = PostureTask(
         cost=1e-3,  # [cost] / [rad]
     )
 
     tasks = [end_effector_task, posture_task]
 
-    q = custom_configuration_vector(
-        robot, shoulder_lift_joint=1.0, shoulder_pan_joint=1.0, elbow_joint=1.0
+    q_ref = custom_configuration_vector(
+        robot,
+        shoulder_lift_joint=1.0,
+        shoulder_pan_joint=1.0,
+        elbow_joint=1.0,
     )
-    configuration = pink.apply_configuration(robot, q)
+    configuration = pink.Configuration(robot.model, robot.data, q_ref)
     for task in tasks:
         task.set_target_from_configuration(configuration)
     viz.display(configuration.q)
 
     viewer = viz.viewer
     meshcat_shapes.frame(viewer["end_effector_target"], opacity=0.5)
     meshcat_shapes.frame(viewer["end_effector"], opacity=1.0)
@@ -86,14 +89,13 @@
             configuration.get_transform_body_to_world(
                 end_effector_task.body
             ).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/double_pendulum.py` & `pin-pink-0.9.0/examples/double_pendulum.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         ),
         "posture": PostureTask(
             cost=1e-2,  # [cost] / [rad]
         ),
     }
 
     # Initialize tasks from the initial configuration
-    configuration = pink.apply_configuration(robot, robot.q0)
+    configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     for task in tasks.values():
         task.set_target_from_configuration(configuration)
     viz.display(configuration.q)
 
     # Homework: what happens if we replace -= by += in the following line?
     tasks["tip"].transform_target_to_world.translation[2] -= 0.1
 
@@ -88,14 +88,13 @@
         viewer["target_frame"].set_transform(T.np)
         viewer["tip_frame"].set_transform(
             configuration.get_transform_body_to_world(tasks["tip"].body).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/humanoid_jvrc.py` & `pin-pink-0.9.0/examples/humanoid_jvrc.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     viz = pin.visualize.MeshcatVisualizer(
         robot.model, robot.collision_model, robot.visual_model
     )
     robot.setVisualizer(viz, init=False)
     viz.initViewer(open=True)
     viz.loadViewerModel()
 
-    configuration = pink.apply_configuration(robot, robot.q0)
+    configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     viz.display(configuration.q)
 
     left_foot_task = BodyTask(
         "l_ankle", position_cost=1.0, orientation_cost=3.0
     )
     pelvis_task = BodyTask("PELVIS_S", position_cost=1.0, orientation_cost=0.0)
     right_foot_task = BodyTask(
@@ -133,14 +133,13 @@
     while True:
         # Update task targets
         right_wrist_task.set_target(right_wrist_pose.at(t))
         wrist_frame.set_transform(right_wrist_pose.at(t).np)
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/humanoid_sigmaban.py` & `pin-pink-0.9.0/examples/humanoid_sigmaban.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     viz = pin.visualize.MeshcatVisualizer(
         robot.model, robot.collision_model, robot.visual_model
     )
     robot.setVisualizer(viz, init=False)
     viz.initViewer(open=True)
     viz.loadViewerModel()
 
-    configuration = pink.apply_configuration(robot, robot.q0)
+    configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     viz.display(configuration.q)
     viewer = viz.viewer
 
     left_foot_task = BodyTask(
         "left_foot_tip",
         position_cost=1.0,
         orientation_cost=1.0,
@@ -114,14 +114,13 @@
 
     rate = RateLimiter(frequency=200.0)
     dt = rate.period
     t = 0.0  # [s]
     while True:
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/load_custom_urdf.py` & `pin-pink-0.9.0/examples/load_custom_urdf.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/examples/meshcat_shapes.py` & `pin-pink-0.9.0/examples/meshcat_shapes.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/examples/omnidirectional_wheeled_robot.py` & `pin-pink-0.9.0/examples/omnidirectional_wheeled_robot.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 """Move an omnidirectional robot between two jumping targets.
 
 Illustrates the notion of screw path.
 """
 
 import os
 
+import meshcat_shapes
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from loop_rate_limiters import RateLimiter
 
-import meshcat_shapes
 import pink
 from pink import solve_ik
 from pink.tasks import BodyTask
 from pink.visualization import start_meshcat_visualizer
 
 if __name__ == "__main__":
 
@@ -59,15 +59,15 @@
         position_cost=1.0,  # [cost] / [m]
         orientation_cost=1e-5,  # [cost] / [rad]
     )
     base_task.gain = 0.22  # slow things down
     tasks = [base_task]
 
     # Initialize tasks from the initial configuration
-    configuration = pink.apply_configuration(robot, robot.q0)
+    configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     base_task.set_target_from_configuration(configuration)
     viz.display(configuration.q)
 
     # Select QP solver
     solver = qpsolvers.available_solvers[0]
     if "quadprog" in qpsolvers.available_solvers:
         solver = "quadprog"
@@ -87,14 +87,13 @@
         viewer["target_frame"].set_transform(T.np)
         viewer["tip_frame"].set_transform(
             configuration.get_transform_body_to_world(base_task.body).np
         )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks, dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/robots/double_pendulum.urdf` & `pin-pink-0.9.0/examples/robots/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/examples/robots/omnidirectional_wheeled_robot.urdf` & `pin-pink-0.9.0/examples/robots/omnidirectional_wheeled_robot.urdf`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/examples/visualize_in_meshcat.py` & `pin-pink-0.9.0/examples/visualize_in_meshcat.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         ),
     }
 
     tasks["posture"].set_target(
         custom_configuration_vector(robot, left_knee=0.2, right_knee=-0.2)
     )
 
-    configuration = pink.apply_configuration(robot, robot.q0)
+    configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     for body, task in tasks.items():
         if type(task) is BodyTask:
             task.set_target_from_configuration(configuration)
     viz.display(configuration.q)
 
     left_contact_target = tasks["left_contact"].transform_target_to_world
     right_contact_target = tasks["right_contact"].transform_target_to_world
@@ -103,14 +103,13 @@
         for body in ["left_contact", "right_contact"]:
             viewer[body].set_transform(
                 configuration.get_transform_body_to_world(body).np
             )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/examples/visualize_in_yourdfpy.py` & `pin-pink-0.9.0/examples/visualize_in_yourdfpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             orientation_cost=0.0,  # [cost] / [rad]
         ),
         "posture": PostureTask(
             cost=1e-3,  # [cost] / [rad]
         ),
     }
 
-    configuration = pink.apply_configuration(robot, robot.q0)
+    configuration = pink.Configuration(robot.model, robot.data, robot.q0)
     for body, task in tasks.items():
         if type(task) is BodyTask:
             task.set_target_from_configuration(configuration)
 
     tasks["posture"].set_target(
         custom_configuration_vector(robot, left_knee=0.2, right_knee=-0.2)
     )
@@ -99,16 +99,15 @@
         left_contact_target.translation[2] += 0.1 * np.sin(t) * dt
         right_contact_target.translation[2] += 0.1 * np.sin(t) * dt
         tasks["left_contact"].set_target(left_contact_target)
         tasks["right_contact"].set_target(right_contact_target)
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Display resulting configuration
         actuated_joints = configuration.q[7:]
         viz.update_cfg(actuated_joints)
 
         # Regulate visualizer FPS
         animation_time += dt
```

### Comparing `pin-pink-0.8.0/examples/wheeled_biped_upkie.py` & `pin-pink-0.9.0/examples/wheeled_biped_upkie.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             cost=1e-3,  # [cost] / [rad]
         ),
     }
 
     q_ref = custom_configuration_vector(
         robot, left_hip=-0.2, left_knee=0.4, right_hip=0.2, right_knee=-0.4
     )
-    configuration = pink.apply_configuration(robot, q_ref)
+    configuration = pink.Configuration(robot.model, robot.data, q_ref)
     for body, task in tasks.items():
         if type(task) is BodyTask:
             task.set_target_from_configuration(configuration)
     tasks["posture"].set_target(q_ref)
     viz.display(configuration.q)
 
     left_contact_target = tasks["left_contact"].transform_target_to_world
@@ -98,14 +98,13 @@
         for body in ["left_contact", "right_contact"]:
             viewer[body].set_transform(
                 configuration.get_transform_body_to_world(body).np
             )
 
         # Compute velocity and integrate it into next configuration
         velocity = solve_ik(configuration, tasks.values(), dt, solver=solver)
-        q = configuration.integrate(velocity, dt)
-        configuration = pink.apply_configuration(robot, q)
+        configuration.integrate_inplace(velocity, dt)
 
         # Visualize result at fixed FPS
-        viz.display(q)
+        viz.display(configuration.q)
         rate.sleep()
         t += dt
```

### Comparing `pin-pink-0.8.0/pink/__init__.py` & `pin-pink-0.9.0/pink/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,27 +13,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python inverse kinematics for your robot model based on Pinocchio."""
 
-from .configuration import (
-    Configuration,
-    apply_configuration,
-    assume_configuration,
-)
+from .configuration import Configuration
 from .solve_ik import build_ik, solve_ik
 from .tasks import Task
 from .utils import custom_configuration_vector
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 __all__ = [
     "Configuration",
-    "apply_configuration",
-    "assume_configuration",
     "build_ik",
     "custom_configuration_vector",
     "solve_ik",
     "Task",
 ]
```

### Comparing `pin-pink-0.8.0/pink/bounded_tangent.py` & `pin-pink-0.9.0/pink/bounded_tangent.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/pink/configuration.py` & `pin-pink-0.9.0/pink/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,45 +49,66 @@
 
     Notes:
         This class is meant to be used as a subclass of pin.RobotWrapper, not
         wrap it. However, right now pin.RobotWrapper does not have a shallow
         copy constructor. TODO(scaron): bring it up upstream.
 
     Attributes:
-        data: Data with kinematics matching the configuration vector
-            :data:`Configuration.q`.
+        data: Data corresponding to :data:`Configuration.model`.
         model: Kinodynamic model.
-        q: Configuration vector matching the kinematics in
-            :data:`Configuration.data`.
+        q: Configuration vector for the robot model.
     """
 
     data: pin.Data
     model: pin.Model
     q: np.ndarray
 
-    def __init__(self, model: pin.Model, data: pin.Data, q: np.ndarray):
+    def __init__(
+        self,
+        model: pin.Model,
+        data: pin.Data,
+        q: np.ndarray,
+        copy_data=True,
+        forward_kinematics=True,
+    ):
         """Initialize configuration.
 
         Args:
             model: Kinodynamic model.
-            data: Data with kinematics matching the configuration vector
-                :data:`Configuration.q`.
-            q: Configuration vector matching the kinematics in
-                :data:`Configuration.data`.
+            data: Data corresponding to the model.
+            q: Configuration vector.
+            copy_data: If true (default), work on an internal copy of the input
+                data. Otherwise, work on the input data directly.
+            forward_kinematics: If true (default), compute forward kinematics
+                from the q into the internal data.
+
+        Notes:
+            Configurations copy data and run forward kinematics by default so
+            that they are less error-prone for newcomers. You can avoid copies
+            or forward kinematics (e.g. if it is already computed by the
+            caller) using constructor parameters.
         """
         if not hasattr(model, "tangent"):
             model.tangent = VectorSpace(model.nv)
         if not hasattr(model, "bounded_tangent"):
             model.bounded_tangent = BoundedTangent(model)
         q_readonly = q.copy()
         q_readonly.setflags(write=False)
-        self.data = data
+        self.data = data.copy() if copy_data else data
         self.model = model
         self.q = q_readonly
         self.tangent = model.tangent
+        #
+        if forward_kinematics:
+            self.update()
+
+    def update(self) -> None:
+        """Run forward kinematics from the configuration."""
+        pin.computeJointJacobians(self.model, self.data, self.q)
+        pin.updateFramePlacements(self.model, self.data)
 
     def check_limits(self, tol: float = 1e-6) -> None:
         """Check that the current configuration is within limits.
 
         Args:
             tol: Tolerance in radians.
 
@@ -171,38 +192,16 @@
             dt: Integration duration in [s].
 
         Returns:
             New configuration vector after integration.
         """
         return pin.integrate(self.model, self.q, velocity * dt)
 
+    def integrate_inplace(self, velocity, dt) -> None:
+        """Integrate a velocity starting from the current configuration.
 
-def assume_configuration(
-    robot: pin.RobotWrapper, q: np.ndarray
-) -> Configuration:
-    """Assume that the provided robot wrapper has already been configured.
-
-    Args:
-        robot: Robot wrapper with its initial data.
-        q: Configuration matching the robot wrapper's data.
-
-    Returns:
-        Robot configuration.
-    """
-    return Configuration(robot.model, robot.data, q)
-
-
-def apply_configuration(
-    robot: pin.RobotWrapper, q: np.ndarray
-) -> Configuration:
-    """Apply configuration (forward kinematics) to a robot wrapper.
-
-    Args:
-        robot: Robot wrapper with its initial data.
-        q: Configuration vector to apply.
-
-    Returns:
-        Configured robot.
-    """
-    pin.computeJointJacobians(robot.model, robot.data, q)
-    pin.updateFramePlacements(robot.model, robot.data)
-    return Configuration(robot.model, robot.data, q)
+        Args:
+            velocity: Velocity in tangent space.
+            dt: Integration duration in [s].
+        """
+        self.q = pin.integrate(self.model, self.q, velocity * dt)
+        self.update()
```

### Comparing `pin-pink-0.8.0/pink/exceptions.py` & `pin-pink-0.9.0/pink/exceptions.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/pink/limits.py` & `pin-pink-0.9.0/pink/limits.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/pink/solve_ik.py` & `pin-pink-0.9.0/pink/solve_ik.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/pink/tasks/__init__.py` & `pin-pink-0.9.0/pink/tasks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Kinematic tasks."""
 
 from .body_task import BodyTask
-from .exceptions import TargetNotSet
+from .exceptions import TargetNotSet, TaskJacobianNotSet
+from .joint_coupling_task import JointCouplingTask
+from .linear_holonomic_task import LinearHolonomicTask
 from .posture_task import PostureTask
 from .task import Task
 
 __all__ = [
     "BodyTask",
-    "PostureTask",
     "TargetNotSet",
+    "TaskJacobianNotSet",
+    "JointCouplingTask",
+    "LinearHolonomicTask",
+    "PostureTask",
     "Task",
 ]
```

### Comparing `pin-pink-0.8.0/pink/tasks/body_task.py` & `pin-pink-0.9.0/pink/tasks/body_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,67 +145,69 @@
         """Set task target pose from a robot configuration.
 
         Args:
             configuration: Robot configuration.
         """
         self.set_target(configuration.get_transform_body_to_world(self.body))
 
-    def compute_error_in_body(
-        self, configuration: Configuration
-    ) -> np.ndarray:
-        r"""Compute the body twist error.
+    def compute_error(self, configuration: Configuration) -> np.ndarray:
+        r"""Compute body task error.
+
+        Mathematically this error is a twist :math:`e(q) \in se(3)` expressed
+        in the local frame (i.e., it is a bodytwist ). We map it to
+        :math:`\mathbb{R}^6` using Pinocchio's convention (linear coordinates
+        followed by angular coordinates).
 
-        The body twist error is the (box minus) difference between target and
-        current body configuration:
+        The error is the right-minus difference between target and current body
+        configuration:
 
         .. math::
 
             e(q) := {}_b \xi_{0b} = -(T_{t0} \boxminus T_{b0})
             = -\log(T_{t0} \cdot T_{0b}) = -\log(T_{tb}) = \log(T_{bt})
 
         where :math:`b` denotes the body frame, :math:`t` the target frame and
         :math:`0` the inertial frame.
 
+        See :func:`Task.compute_error` for more context, and [MLT]_ for details
+        on the right-minus operator.
+
         Args:
-            configuration: Robot configuration to read values from.
+            configuration: Robot configuration :math:`q`.
 
         Returns:
-            Coordinate vector of the body twist error.
+            Body task error :math:`e(q)`.
         """
         if self.transform_target_to_world is None:
             raise TargetNotSet(f"no target set for body {self.body}")
         transform_body_to_world = configuration.get_transform_body_to_world(
             self.body
         )
         error_in_body: np.ndarray = body_minus(
             self.transform_target_to_world,
             transform_body_to_world,
         )
         return error_in_body
 
-    def compute_task_dynamics(
-        self, configuration: Configuration
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        r"""Compute the task dynamics matrix and vector.
+    def compute_jacobian(self, configuration: Configuration) -> np.ndarray:
+        r"""Compute the body task Jacobian.
 
-        Those are the matrix :math:`J(q)` and vector :math:`\alpha e(q)` such
-        that the task dynamics are:
+        The task Jacobian :math:`J(q) \in \mathbb{R}^{6 \times n_v}` appears in
+        the task dynamics:
 
         .. math::
 
             J(q) \Delta q = \alpha e(q)
 
-        The Jacobian matrix is :math:`J(q) \in \mathbb{R}^{6 \times n}`,
-        with :math:`n` the dimension of the robot's tangent space, and the
-        error vector is :math:`e(q) \in \mathbb{R}^6`.
-
-        See :func:`Task.compute_task_dynamics` for more context.
+        The derivation of the formula for this Jacobian is detailed in
+        [BodyTaskJacobian]_. See also :func:`Task.compute_jacobian` for more
+        context on task Jacobians.
 
         Args:
-            configuration: Robot configuration to read values from.
+            configuration: Robot configuration :math:`q`.
 
         Returns:
             Pair :math:`(J, \alpha e)` of Jacobian matrix and error vector,
             both expressed in the body frame.
         """
         jacobian_in_body = configuration.get_body_jacobian(self.body)
 
@@ -215,17 +217,15 @@
         transform_body_to_world = configuration.get_transform_body_to_world(
             self.body
         )
         transform_body_to_target = (
             self.transform_target_to_world.inverse() * transform_body_to_world
         )
         J = pin.Jlog6(transform_body_to_target) @ jacobian_in_body
-
-        error_in_body = self.compute_error_in_body(configuration)
-        return J, self.gain * error_in_body
+        return J
 
     def compute_qp_objective(
         self, configuration: Configuration
     ) -> Tuple[np.ndarray, np.ndarray]:
         r"""Compute the matrix-vector pair :math:`(H, c)` of the QP objective.
 
         This pair is such that the contribution of the task to the QP objective
@@ -239,30 +239,29 @@
         The weight matrix :math:`W \in \mathbb{R}^{6 \times 6}` combines
         position and orientation costs. The unit of the overall contribution is
         :math:`[\mathrm{cost}]^2`. The configuration displacement
         :math:`\Delta q` is the output of inverse kinematics (we divide it by
         :math:`\Delta t` to get a commanded velocity).
 
         Args:
-            configuration: Robot configuration to read values from.
+            configuration: Robot configuration :math:`q`.
 
         Returns:
-            Pair :math:`(H, c)` of Hessian matrix and linear vector of the QP
-            objective.
+            Pair :math:`(H(q), c(q))` of Hessian matrix and linear vector of
+            the QP objective.
 
         See Also:
-            Levenberg-Marquardt damping is described in
-            "Solvability-Unconcerned Inverse Kinematics by the
-            Levenberg-Marquardt Method" (Sugihara, 2011). The dimensional
-            analysis in this class is our own.
+            Levenberg-Marquardt damping is described in [Sugihara2011]_. The
+            dimensional analysis in this class is our own.
         """
-        jacobian, error = self.compute_task_dynamics(configuration)
+        jacobian = self.compute_jacobian(configuration)
+        gain_error = self.gain * self.compute_error(configuration)
         weight = np.diag(self.cost)  # [cost] * [twist]^{-1}
         weighted_jacobian = weight @ jacobian  # [cost]
-        weighted_error = weight @ error  # [cost]
+        weighted_error = weight @ gain_error  # [cost]
         mu = self.lm_damping * weighted_error @ weighted_error  # [cost]^2
         eye_tg = configuration.tangent.eye
         # Our Levenberg-Marquardt damping `mu * eye_tg` is isotropic in the
         # robot's tangent space. If it helps we can add a tangent-space scaling
         # to damp the floating base differently from joint angular velocities.
         H = weighted_jacobian.T @ weighted_jacobian + mu * eye_tg
         c = -weighted_error.T @ weighted_jacobian
```

### Comparing `pin-pink-0.8.0/pink/tasks/exceptions.py` & `pin-pink-0.9.0/pink/tasks/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,7 +18,11 @@
 """Exceptions raised by tasks."""
 
 from ..exceptions import PinkError
 
 
 class TargetNotSet(PinkError):
     """Exception raised when attempting to compute with an unset target."""
+
+
+class TaskJacobianNotSet(PinkError):
+    """Exception raised when attempting to compute without a task Jacobian."""
```

### Comparing `pin-pink-0.8.0/pink/tasks/posture_task.py` & `pin-pink-0.9.0/pink/tasks/posture_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,48 +76,55 @@
         """Set target posture from a robot configuration.
 
         Args:
             configuration: Robot configuration.
         """
         self.set_target(configuration.q)
 
-    def compute_task_dynamics(
-        self, configuration: Configuration
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        r"""Compute the task dynamics matrix and vector.
+    def compute_error(self, configuration: Configuration) -> np.ndarray:
+        """Compute posture task error.
 
-        Those are the matrix :math:`J(q)` and vector :math:`\alpha e(q)` such
-        that the task dynamics are:
+        See :func:`Task.compute_error` for more context.
 
-        .. math::
+        Args:
+            configuration: Robot configuration :math:`q`.
 
-            J(q) \Delta q = \alpha e(q)
+        Returns:
+            Posture task error :math:`e(q)`.
+        """
+        if self.target_q is None:
+            raise TargetNotSet("no posture target")
+        _, nv = get_root_joint_dim(configuration.model)
+        return pin.difference(
+            configuration.model, configuration.q, self.target_q
+        )[nv:]
+
+    def compute_jacobian(self, configuration: Configuration) -> np.ndarray:
+        r"""Compute posture task Jacobian.
+
+        The task Jacobian is the identity :math:`I_{n_v} \in \mathbb{R}^{n_v
+        \times n_v}`, with :math:`n_v` the dimension of the robot's tangent
+        space, so that the task dynamics are:
 
-        The Jacobian matrix is :math:`J(q) \in \mathbb{R}^{n \times n}`,
-        with :math:`n` the dimension of the robot's tangent space, and the
-        error vector is :math:`e(q) \in \mathbb{R}^n`. Both depend on the
-        configuration :math:`q` of the robot.
+        .. math::
+
+            J(q) \Delta q = \Delta_q = \alpha (q^* - q)
 
-        See :func:`Task.compute_task_dynamics` for more context.
+        See :func:`Task.compute_jacobian` for more context.
 
         Args:
-            configuration: Robot configuration to read kinematics from.
+            configuration: Robot configuration :math:`q`.
 
         Returns:
-            Pair :math:`(J, \alpha e)` of Jacobian matrix and error vector,
-            both expressed in the body frame.
+            Posture task Jacobian :math:`J(q)`.
         """
         if self.target_q is None:
             raise TargetNotSet("no posture target")
         _, nv = get_root_joint_dim(configuration.model)
-        jacobian = configuration.tangent.eye[nv:, :]
-        error = pin.difference(
-            configuration.model, configuration.q, self.target_q
-        )[nv:]
-        return (jacobian, self.gain * error)
+        return configuration.tangent.eye[nv:, :]
 
     def compute_qp_objective(
         self, configuration: Configuration
     ) -> Tuple[np.ndarray, np.ndarray]:
         r"""Compute the matrix-vector pair :math:`(H, c)` of the QP objective.
 
         This pair is such that the contribution of the task to the QP objective
@@ -137,17 +144,18 @@
         Args:
             configuration: Robot configuration.
 
         Returns:
             Pair :math:`(H, c)` of Hessian matrix and linear vector of the QP
             objective.
         """
-        jacobian, error = self.compute_task_dynamics(configuration)
+        jacobian = self.compute_jacobian(configuration)
+        gain_error = self.gain * self.compute_error(configuration)
         weighted_jacobian = self.cost * jacobian  # [cost]
-        weighted_error = self.cost * error  # [cost]
+        weighted_error = self.cost * gain_error  # [cost]
         H = weighted_jacobian.T @ weighted_jacobian
         c = -weighted_error.T @ weighted_jacobian
         return (H, c)
 
     def __repr__(self):
         """Human-readable representation of the task."""
         return f"PostureTask(cost={self.cost}, gain={self.gain})"
```

### Comparing `pin-pink-0.8.0/pink/tasks/utils.py` & `pin-pink-0.9.0/pink/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/pink/utils.py` & `pin-pink-0.9.0/pink/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 """Utility classes and functions."""
 
 from typing import Tuple
 
 import numpy as np
 import pinocchio as pin
 
+from .exceptions import PinkError
+
 
 def custom_configuration_vector(robot: pin.Model, **kwargs) -> np.ndarray:
     """Generate a configuration vector where named joints have specific values.
 
     Args:
         robot: Robot model.
         kwargs: Custom values for joint coordinates.
@@ -55,14 +57,34 @@
     if model.existJointName("root_joint"):
         root_joint_id = model.getJointId("root_joint")
         root_joint = model.joints[root_joint_id]
         return root_joint.nq, root_joint.nv
     return 0, 0
 
 
+def get_joint_idx(model: pin.Model, joint_name: str) -> Tuple[int, int]:
+    """Get joint index in the configuration and tangent space.
+
+    Args:
+        model: Robot model.
+        joint_name: Joint name.
+
+    Returns:
+        idx_q: Joint idx in configuration space.
+        idx_v: Joint idx in tangent space.
+    """
+    if model.existJointName(joint_name):
+        joint_id = model.getJointId(joint_name)
+        joint = model.joints[joint_id]
+        return joint.idx_q, joint.idx_v
+    raise PinkError(
+        f"cannot find the joint index corresponding to joint {joint_name}"
+    )
+
+
 class VectorSpace:
     """Wrapper to refer to a vector space and its characteristic matrices."""
 
     __dim: int
     __eye: np.ndarray
     __ones: np.ndarray
     __zeros: np.ndarray
```

### Comparing `pin-pink-0.8.0/pink/visualization.py` & `pin-pink-0.9.0/pink/visualization.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/pyproject.toml` & `pin-pink-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/tests/__init__.py` & `pin-pink-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/tests/test_body_task.py` & `pin-pink-0.9.0/tests/test_body_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import unittest
 
 import numpy as np
 import pinocchio as pin
 from qpsolvers import solve_qp
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
-import pink
+from pink import Configuration
 from pink.tasks import BodyTask, TargetNotSet
 
 
 class TestBodyTask(unittest.TestCase):
 
     """
     Test consistency of the body task.
@@ -39,15 +39,15 @@
     """
 
     def setUp(self):
         """Prepare test fixture."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        self.configuration = pink.apply_configuration(robot, robot.q0)
+        self.configuration = Configuration(robot.model, robot.data, robot.q0)
 
     def test_set_target_from_configuration(self):
         task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
         task.set_target_from_configuration(self.configuration)
         transform_ankle_to_world = (
             self.configuration.get_transform_body_to_world("l_ankle")
         )
@@ -66,17 +66,17 @@
         self.assertTrue("cost=" in repr(earflap_task))
         self.assertTrue("target=" in repr(earflap_task))
 
     def test_target_not_set(self):
         """Raise an exception when the target is not set."""
         task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
         with self.assertRaises(TargetNotSet):
-            task.compute_error_in_body(self.configuration)
+            task.compute_error(self.configuration)
         with self.assertRaises(TargetNotSet):
-            task.compute_task_dynamics(self.configuration)
+            task.compute_jacobian(self.configuration)
 
     def test_target_set_properly(self):
         """Return target properly once it's set."""
         task = BodyTask("l_ankle", position_cost=1.0, orientation_cost=0.1)
         T = self.configuration.get_transform_body_to_world("l_ankle")
         task.set_target(T)
         self.assertIsNotNone(task.transform_target_to_world)
@@ -105,15 +105,16 @@
             )
 
     def test_zero_error_when_target_at_body(self):
         """Error is zero when the target and body are at the same location."""
         task = BodyTask("r_ankle", position_cost=1.0, orientation_cost=0.1)
         target = self.configuration.get_transform_body_to_world("r_ankle")
         task.set_target(target)  # error == 0
-        J, e = task.compute_task_dynamics(self.configuration)
+        J = task.compute_jacobian(self.configuration)
+        e = task.compute_error(self.configuration)
         self.assertTrue(
             np.allclose(J, self.configuration.get_body_jacobian("r_ankle"))
         )
         self.assertLess(np.linalg.norm(e), 1e-10)
 
     def test_unit_cost_qp_objective(self):
         """Unit cost means the QP objective is exactly (J^T J, -e^T J)."""
@@ -122,15 +123,16 @@
             np.eye(3), np.array([0.0, 0.01, 0.0])
         )
         target = (
             self.configuration.get_transform_body_to_world("r_wrist")
             * transform_target_to_body
         )
         task.set_target(target)
-        J, e = task.compute_task_dynamics(self.configuration)
+        J = task.compute_jacobian(self.configuration)
+        e = task.compute_error(self.configuration)
         task.set_position_cost(1.0)
         task.set_orientation_cost(1.0)
         task.lm_damping = 0.0
         H, c = task.compute_qp_objective(self.configuration)
         self.assertTrue(np.allclose(J.T @ J, H))
         self.assertTrue(np.allclose(-e.T @ J, c))
 
@@ -145,15 +147,16 @@
             np.eye(3), np.array([0.1, 0.02, 0.01])
         )
         target = (
             self.configuration.get_transform_body_to_world("l_wrist")
             * transform_target_to_body
         )
         task.set_target(target)
-        J, e = task.compute_task_dynamics(self.configuration)
+        J = task.compute_jacobian(self.configuration)
+        e = task.compute_error(self.configuration)
         qd = np.random.random(J.shape[1:])
         test_cases = {
             "position_only": (1.0, 0.0, slice(0, 3)),
             "orientation_only": (0.0, 1.0, slice(3, 6)),
             "position_0": ([1.0, 0.0, 0.0], 0.0, slice(0, 1)),
             "position_1": ([0.0, 1.0, 0.0], 0.0, slice(1, 2)),
             "position_2": ([0.0, 0.0, 1.0], 0.0, slice(2, 3)),
```

### Comparing `pin-pink-0.8.0/tests/test_bounded_tangent.py` & `pin-pink-0.9.0/tests/test_bounded_tangent.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/tests/test_configuration.py` & `pin-pink-0.9.0/tests/test_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,49 +11,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Test the Configuration type.
-"""
+"""Test the Configuration type."""
 
 import unittest
 
 import numpy as np
 import pinocchio as pin
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
-import pink
+from pink import Configuration
 from pink.exceptions import BodyNotFound, NotWithinConfigurationLimits
 
 
 class TestConfiguration(unittest.TestCase):
-    def test_assume_configuration(self):
-        """
-        Assuming a configuration does not change data.
-        """
+    def test_constructor(self):
+        """Constructing a configuration computes Jacobians."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         robot.data.J.fill(42.0)
-        configuration = pink.assume_configuration(robot, robot.q0)
-        self.assertTrue(np.allclose(configuration.data.J, 42.0))
-
-    def test_apply_configuration(self):
-        """
-        Applying a configuration computes Jacobians.
-        """
-        robot = load_robot_description(
-            "jvrc_description", root_joint=pin.JointModelFreeFlyer()
-        )
-        robot.data.J.fill(42.0)
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         J_check = np.array(
             [
                 [
                     1.0,
                     0.0,
                     0.0,
                     0.0,
@@ -364,109 +349,134 @@
                     0.0,
                     0.0,
                 ],
             ]
         )
         self.assertTrue(np.allclose(configuration.data.J, J_check))
 
+    def test_copy_no_forward_kinematics(self):
+        """Refer to the input data, compute forward kinematics."""
+        robot = load_robot_description(
+            "jvrc_description", root_joint=pin.JointModelFreeFlyer()
+        )
+        robot.data.J.fill(42.0)
+        configuration = Configuration(
+            robot.model,
+            robot.data,
+            robot.q0,
+            copy_data=False,
+            forward_kinematics=True,
+        )
+        self.assertFalse(np.allclose(configuration.data.J, 42.0))
+        configuration.data.J.fill(12.0)
+        self.assertTrue(np.allclose(robot.data.J, 12.0))
+
+    def test_no_copy_no_forward_kinematics(self):
+        """Not copying means working directly on the underlying data."""
+        robot = load_robot_description(
+            "jvrc_description", root_joint=pin.JointModelFreeFlyer()
+        )
+        robot.data.J.fill(42.0)
+        configuration = Configuration(
+            robot.model,
+            robot.data,
+            robot.q0,
+            copy_data=False,
+            forward_kinematics=False,
+        )
+        self.assertTrue(np.allclose(configuration.data.J, 42.0))
+        configuration.data.J.fill(12.0)
+        self.assertTrue(np.allclose(robot.data.J, 12.0))
+
     def test_transform_found(self):
-        """
-        Return the pose of an existing robot body.
-        """
+        """Return the pose of an existing robot body."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         transform_pelvis_to_world = configuration.get_transform_body_to_world(
             "PELVIS_S"
         )
         self.assertTrue(
             np.allclose(
                 transform_pelvis_to_world.np[3, :],
                 np.array([0.0, 0.0, 0.0, 1.0]),
             )
         )
 
     def test_transform_not_found(self):
-        """
-        Raise an error when the request robot body is not found.
-        """
+        """Raise an error when the request robot body is not found."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         with self.assertRaises(KeyError):
             configuration.get_transform_body_to_world("foo")
 
     def test_check_limits(self):
-        """
-        Raise an error if and only if a joint limit is exceened.
-        """
+        """Raise an error if and only if a joint limit is exceened."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         q = robot.q0
-        configuration = pink.apply_configuration(robot, q)
+        configuration = Configuration(robot.model, robot.data, q)
         configuration.check_limits()
         q[-10] += 1e4  # move configuration out of bounds
-        configuration = pink.apply_configuration(robot, q)
+        configuration = Configuration(robot.model, robot.data, q)
         with self.assertRaises(NotWithinConfigurationLimits):
             configuration.check_limits()
 
     def test_q_is_a_read_only_copy(self):
-        """
-        The `q` attribute of a configuration is a read-only copy.
-        """
+        """The `q` attribute of a configuration is a read-only copy."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
         original_q = robot.q0
-        configuration = pink.apply_configuration(robot, original_q)
+        configuration = Configuration(robot.model, robot.data, original_q)
         the_answer = 42.0
         self.assertNotEqual(configuration.q[2], the_answer)
         original_q[2] = the_answer
         self.assertNotEqual(configuration.q[2], the_answer)
         with self.assertRaises(ValueError):
             configuration.q[2] += 3.0  # read-only
 
     def test_tangent_eye(self):
-        """
-        Configuration's tangent eye is an identity matrix.
-        """
+        """Configuration's tangent eye is an identity matrix."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         v = np.array([i for i in range(robot.model.nv)])
         self.assertTrue(np.allclose(configuration.tangent.eye.dot(v), v))
 
     def test_tangent_ones(self):
-        """
-        Configuration's tangent ones is a vector of 1.0's.
-        """
+        """Configuration's tangent ones is a vector of 1.0's."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         self.assertEqual(np.sum(configuration.tangent.ones), robot.model.nv)
 
     def test_tangent_zeros(self):
-        """
-        Configuration's tangent ones is a vector of 0.0's.
-        """
+        """Configuration's tangent ones is a vector of 0.0's."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         self.assertAlmostEqual(np.sum(configuration.tangent.zeros), 0.0)
         self.assertEqual(len(configuration.tangent.zeros), robot.model.nv)
 
-    def test_get_body_jacobian(self):
-        """
-        Querying a body that does not exist raises a ValueError.
-        """
+    def test_body_jacobian_not_found(self):
+        """Querying a body that does not exist raises a ValueError."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = pink.apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         with self.assertRaises(BodyNotFound):
             configuration.get_body_jacobian("does_not_exist")
+
+    def test_get_integrate_inplace(self):
+        robot = load_robot_description("sigmaban_description", root_joint=None)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
+        velocity = robot.model.tangent.ones
+        configuration.integrate_inplace(velocity, dt=1e-3)
+        self.assertGreater(np.linalg.norm(configuration.q - robot.q0), 2e-3)
```

### Comparing `pin-pink-0.8.0/tests/test_jacobians.py` & `pin-pink-0.9.0/tests/test_jacobians.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import unittest
 
 import numpy as np
 import pinocchio as pin
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
-import pink
+from pink import Configuration
 from pink.tasks import BodyTask
 
 
 class TestJacobians(unittest.TestCase):
 
     """
     Test task Jacobian matrices against finite differences.
@@ -40,14 +40,16 @@
         random_dirs = random_dq / l2norms.reshape((nb_dirs, 1))
         random_q = (
             0.1 * np.pi * (2.0 * np.random.random((nb_configs, 6)) - 1.0)
         )
         robot = load_robot_description("ur3_description")
         self.assertEqual(robot.nq, 6)
         self.body = "ee_link"
+        self.data = robot.data
+        self.model = robot.model
         self.random_dirs = random_dirs
         self.random_q = random_q
         self.robot = robot
 
     def test_body_task(self, tol=1e-6):
         """
         Test BodyTask Jacobian matrix.
@@ -55,21 +57,20 @@
         Args:
             tol: Test tolerance.
         """
         task = BodyTask(self.body, position_cost=1.0, orientation_cost=1.0)
         task.set_target(pin.SE3.Random())
 
         def e(q):
-            configuration = pink.apply_configuration(self.robot, q)
-            return task.compute_error_in_body(configuration)
+            configuration = Configuration(self.model, self.data, q)
+            return task.compute_error(configuration)
 
         def J(q):
-            configuration = pink.apply_configuration(self.robot, q)
-            jacobian, _ = task.compute_task_dynamics(configuration)
-            return jacobian
+            configuration = Configuration(self.model, self.data, q)
+            return task.compute_jacobian(configuration)
 
         nq = self.robot.model.nq
         nv = self.robot.model.nv
         for q_0 in self.random_q:
             J_0 = J(q_0)
             e_0 = e(q_0)
```

### Comparing `pin-pink-0.8.0/tests/test_limits.py` & `pin-pink-0.9.0/tests/test_limits.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,40 +21,42 @@
 
 import unittest
 
 import numpy as np
 import pinocchio as pin
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
-from pink import apply_configuration
+from pink import Configuration
 from pink.limits import compute_velocity_limits
 
 
 class TestLimits(unittest.TestCase):
     def setUp(self):
-        self.robot = load_robot_description(
+        robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
+        self.data = robot.data
+        self.model = robot.model
+        self.robot = robot
 
     def test_limit_dimension(self):
         """Velocity limit dimension is the number of bounded joints."""
-        model = self.robot.model
-        configuration = apply_configuration(self.robot, self.robot.q0)
+        configuration = Configuration(self.model, self.data, self.robot.q0)
         v_max, v_min = compute_velocity_limits(configuration, dt=1e-3)
-        self.assertEqual(v_max.shape, (model.bounded_tangent.dim,))
-        self.assertEqual(v_min.shape, (model.bounded_tangent.dim,))
+        self.assertEqual(v_max.shape, (self.model.bounded_tangent.dim,))
+        self.assertEqual(v_min.shape, (self.model.bounded_tangent.dim,))
 
     def test_model_with_no_joint_limit(self):
         """Model with no joint limit has no velocity-limit vector."""
         model = pin.Model()
         model.addJoint(
             0, pin.JointModelSpherical(), pin.SE3.Identity(), "spherical"
         )
         robot = pin.RobotWrapper(model=model)
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         v_max, v_min = compute_velocity_limits(configuration, dt=1e-3)
         self.assertIsNone(v_max)
         self.assertIsNone(v_min)
 
     def test_model_with_limitless_joint(self):
         """Same as previous test, but the joint has a limit set to zero."""
         model = pin.Model()
@@ -65,41 +67,40 @@
             "revolute",
             max_effort=np.array([0.0]),
             max_velocity=np.array([0.0]),
             min_config=np.array([0.0]),
             max_config=np.array([0.0]),
         )
         robot = pin.RobotWrapper(model=model)
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         v_max, v_min = compute_velocity_limits(configuration, dt=1e-3)
         self.assertIsNone(v_max)
         self.assertIsNone(v_min)
 
     def test_forward_velocity_limit(self):
         """Velocity limits have no effect far from configuration limits.
 
         When we are far away from configuration limits, the velocity limit is
         simply the configuration-agnostic one from the robot.
         """
-        configuration = apply_configuration(self.robot, self.robot.q0)
+        configuration = Configuration(self.model, self.data, self.robot.q0)
         v_max, v_min = compute_velocity_limits(configuration, dt=1e-3)
         v_lim = configuration.model.bounded_tangent.velocity_limit
         tol = 1e-10
         self.assertLess(np.max(v_max - v_lim), tol)
         self.assertLess(np.max(-v_lim - v_min), tol)
 
     def test_configuration_limit_repulsion(self):
         """Velocities are scaled down when close to a configuration limit."""
         dt = 1e-3  # [s]
-        model = self.robot.model
-        configuration = apply_configuration(self.robot, self.robot.q0)
+        configuration = Configuration(self.model, self.data, self.robot.q0)
         slack_vel = 5.5e-4 * configuration.tangent.ones
-        bounded_slack_vel = slack_vel[model.bounded_tangent.indices]
-        model.upperPositionLimit = configuration.integrate(slack_vel, dt)
+        bounded_slack_vel = slack_vel[self.model.bounded_tangent.indices]
+        self.model.upperPositionLimit = configuration.integrate(slack_vel, dt)
         v_max, v_min = compute_velocity_limits(
             configuration, dt, config_limit_gain=0.5
         )
         tol = 1e-10
         self.assertLess(
-            np.max(v_max - model.bounded_tangent.velocity_limit), tol
+            np.max(v_max - self.model.bounded_tangent.velocity_limit), tol
         )
         self.assertLess(np.max(v_max - bounded_slack_vel), tol)
```

### Comparing `pin-pink-0.8.0/tests/test_posture_task.py` & `pin-pink-0.9.0/tests/test_posture_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import unittest
 
 import numpy as np
 import pinocchio as pin
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
-import pink
+from pink import Configuration
 from pink.tasks import PostureTask, TargetNotSet
 
 
 class TestPostureTask(unittest.TestCase):
     """Test consistency of the posture task.
 
     Note:
@@ -36,27 +36,29 @@
     """
 
     def setUp(self):
         """Prepare test fixture."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
-        self.configuration = pink.apply_configuration(robot, robot.q0)
+        self.configuration = Configuration(robot.model, robot.data, robot.q0)
 
     def test_task_repr(self):
         """String representation reports the task gain, costs and target."""
         task = PostureTask(cost=1.0)
         self.assertTrue("cost=" in repr(task))
         self.assertTrue("gain=" in repr(task))
 
     def test_target_not_set(self):
         """Raise an exception when the target is not set."""
         task = PostureTask(cost=1.0)
         with self.assertRaises(TargetNotSet):
-            task.compute_task_dynamics(self.configuration)
+            task.compute_error(self.configuration)
+        with self.assertRaises(TargetNotSet):
+            task.compute_jacobian(self.configuration)
 
     def test_set_target_from_configuration(self):
         task = PostureTask(cost=1.0)
         task.set_target_from_configuration(self.configuration)
         self.assertTrue(np.allclose(self.configuration.q, task.target_q))
 
     def test_target_set_properly(self):
@@ -76,34 +78,36 @@
         task.set_target(q)
         self.assertIsNotNone(task.target_q)
 
     def test_zero_error_when_target_at_body(self):
         """Error is zero when the target and body are at the same location."""
         task = PostureTask(cost=1.0)
         task.set_target(self.configuration.q)  # error == 0
-        _, e = task.compute_task_dynamics(self.configuration)
+        e = task.compute_error(self.configuration)
         self.assertLess(np.linalg.norm(e), 1e-10)
 
     def test_unit_cost_qp_objective(self):
         """A unit cost vector means the QP objective is (J^T J, -e^T J)."""
         task = PostureTask(cost=1.0)
         task.set_target(self.configuration.q)
         q_new = self.configuration.q.copy()
         q_new[1] += 1.0
         q_new[3] += 1.0
         q_new[5] += 1.0
         self.configuration.q = q_new
-        J, e = task.compute_task_dynamics(self.configuration)
+        e = task.compute_error(self.configuration)
+        J = task.compute_jacobian(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         self.assertTrue(np.allclose(J.T @ J, H))
         self.assertTrue(np.allclose(-e.T @ J, c))
 
     def test_zero_cost_same_as_disabling_task(self):
         """The task has no effect when its cost is zero."""
         task = PostureTask(cost=0.0)
         q = self.configuration.q
         task.set_target(q)
-        J, e = task.compute_task_dynamics(self.configuration)
+        J = task.compute_jacobian(self.configuration)
+        e = task.compute_error(self.configuration)
         H, c = task.compute_qp_objective(self.configuration)
         qd = np.random.random(J.shape[1:])
         cost = qd.T @ H @ qd + c @ qd
         self.assertAlmostEqual(cost, 0.0)
```

### Comparing `pin-pink-0.8.0/tests/test_solve_ik.py` & `pin-pink-0.9.0/tests/test_solve_ik.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
 import numpy as np
 import pinocchio as pin
 import qpsolvers
 from numpy.linalg import norm
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
-import pink
-from pink import apply_configuration, build_ik, solve_ik
+from pink import Configuration, build_ik, solve_ik
 from pink.exceptions import NotWithinConfigurationLimits
 from pink.tasks import BodyTask
 
 
 class TestSolveIK(unittest.TestCase):
 
     """Test fixture for the solve_ik function."""
@@ -38,61 +37,61 @@
     def test_checks_configuration_limits(self):
         """IK checks for configuration limits."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
         q = robot.q0
         q[7] = 20  # above limit for Upkie's first joint
-        configuration = pink.apply_configuration(robot, q)
+        configuration = Configuration(robot.model, robot.data, q)
         with self.assertRaises(NotWithinConfigurationLimits):
             solve_ik(configuration, [], dt=1.0, solver="quadprog")
 
     def test_model_with_no_joint_limit(self):
         """Model with no joint limit has no inequality constraints."""
         model = pin.Model()
         model.addJoint(
             0, pin.JointModelSpherical(), pin.SE3.Identity(), "spherical"
         )
         robot = pin.RobotWrapper(model=model)
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         problem = build_ik(configuration, [], dt=1.0)
         self.assertIsNone(problem.G)
         self.assertIsNone(problem.h)
 
     def test_no_task(self):
         """Raise an error when the robot body is not found."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         tasks = []
         v = solve_ik(configuration, tasks, dt=1e-3, solver="quadprog")
         self.assertTrue(np.allclose(v, np.zeros(robot.nv)))
 
     def test_single_task_fulfilled(self):
         """Velocity is zero when the only task is already fulfilled."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         task = BodyTask(
             "left_contact", position_cost=1.0, orientation_cost=1.0
         )
         task.set_target(
             configuration.get_transform_body_to_world("left_contact")
         )
         velocity = solve_ik(configuration, [task], dt=5e-3, solver="quadprog")
         self.assertTrue(np.allclose(velocity, 0.0))
 
     def test_single_task_convergence(self):
         """Integrating velocities makes a task converge to its target."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         task = BodyTask(
             "left_contact", position_cost=1.0, orientation_cost=1.0
         )
         transform_init_to_world = configuration.get_transform_body_to_world(
             "left_contact"
         )
         transform_target_to_init = pin.SE3(
@@ -103,54 +102,48 @@
         )
         task.set_target(transform_target_to_world)
         dt = 5e-3  # [s]
         velocity = solve_ik(configuration, [task], dt, solver="quadprog")
 
         # Initially we are nowhere near the target and moving
         self.assertFalse(np.allclose(velocity, 0.0))
-        self.assertAlmostEqual(
-            norm(task.compute_error_in_body(configuration)),
-            0.1,
-        )
+        self.assertAlmostEqual(norm(task.compute_error(configuration)), 0.1)
         self.assertFalse(
             configuration.get_transform_body_to_world("left_contact").isApprox(
                 transform_target_to_world, prec=1e-4
             )
         )
 
         last_error = 1e6
         for nb_steps in range(42):
-            error = norm(task.compute_error_in_body(configuration))
+            error = norm(task.compute_error(configuration))
             if error < 1e-6 and np.allclose(velocity, 0.0):
                 break
             self.assertLess(error, last_error)  # error stictly decreases
             last_error = error
             q = configuration.integrate(velocity, dt)
-            configuration = apply_configuration(robot, q)
+            configuration = Configuration(robot.model, robot.data, q)
             velocity = solve_ik(configuration, [task], dt, solver="quadprog")
 
         # After nb_steps we are at the target and not moving
         self.assertTrue(np.allclose(velocity, 0.0))
-        self.assertAlmostEqual(
-            norm(task.compute_error_in_body(configuration)),
-            0.0,
-        )
+        self.assertAlmostEqual(norm(task.compute_error(configuration)), 0.0)
         self.assertTrue(
             configuration.get_transform_body_to_world("left_contact").isApprox(
                 transform_target_to_world, prec=1e-8
             )
         )
         self.assertLess(nb_steps, 3)
 
     def test_single_task_translation(self):
         """Translating a target yields a pure linear velocity."""
         robot = load_robot_description(
             "upkie_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         contact_task = BodyTask(
             "right_contact", position_cost=1.0, orientation_cost=1.0
         )
         transform_target_to_world = configuration.get_transform_body_to_world(
             "right_contact"
         ).copy()
         self.assertTrue(
@@ -179,15 +172,15 @@
         self.assertAlmostEqual(linear_velocity_contact_in_contact[2], 0.0)
 
     def test_three_tasks_fulfilled(self):
         """No motion when all targets are reached."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         left_ankle_task = BodyTask(
             "l_ankle", position_cost=1.0, orientation_cost=3.0
         )
         right_ankle_task = BodyTask(
             "r_ankle", position_cost=1.0, orientation_cost=3.0
         )
         pelvis_task = BodyTask(
@@ -209,15 +202,15 @@
         self.assertTrue(np.allclose(velocity, 0.0))
 
     def test_three_tasks_convergence(self):
         """Three simultaneously feasible tasks on the JVRC model converge."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
 
         # Define tasks
         left_ankle_task = BodyTask(
             "l_ankle", position_cost=1.0, orientation_cost=3.0
         )
         right_ankle_task = BodyTask(
             "r_ankle", position_cost=1.0, orientation_cost=3.0
@@ -249,31 +242,31 @@
         # Run IK in closed loop
         dt = 4e-3  # [s]
         for nb_iter in range(42):
             velocity = solve_ik(configuration, tasks, dt, solver="quadprog")
             if norm(velocity) < 1e-10:
                 break
             q = configuration.integrate(velocity, dt)
-            configuration = apply_configuration(robot, q)
+            configuration = Configuration(robot.model, robot.data, q)
         self.assertLess(nb_iter, 42)
         self.assertLess(norm(velocity), 1e-10)
         self.assertLess(
             max(
-                norm(task.compute_error_in_body(configuration))
+                norm(task.compute_error(configuration))
                 for task in tasks
             ),
             0.5,
         )
 
     def get_jvrc_problem(self):
         """Get an IK problem with three tasks on a humanoid model."""
         robot = load_robot_description(
             "jvrc_description", root_joint=pin.JointModelFreeFlyer()
         )
-        configuration = apply_configuration(robot, robot.q0)
+        configuration = Configuration(robot.model, robot.data, robot.q0)
         left_ankle_task = BodyTask(
             "l_ankle", position_cost=1.0, orientation_cost=3.0
         )
         right_ankle_task = BodyTask(
             "r_ankle", position_cost=1.0, orientation_cost=3.0
         )
         pelvis_task = BodyTask(
```

### Comparing `pin-pink-0.8.0/tests/test_task.py` & `pin-pink-0.9.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/tests/test_utils.py` & `pin-pink-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pin-pink-0.8.0/tox.ini` & `pin-pink-0.9.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 
 [testenv]
 deps =
     numpy
     pin >=2.6.4
     qpsolvers >=2.7.2
     quadprog >=0.1.11
-    robot_descriptions >=0.5.0
+    robot_descriptions >=1.4.1
 commands =
     python -m unittest discover --failfast
 
 [testenv:coverage]
 deps =
     coverage
     numpy
     pin >=2.6.4
     qpsolvers >=2.7.2
     quadprog >=0.1.11
-    robot_descriptions >=0.5.0
+    robot_descriptions >=1.4.1
 commands =
     coverage erase
     coverage run -m unittest discover --failfast
     coverage report --include="pink/*"
 
 [testenv:lint]
 deps =
     black >=22.10.0
     ruff >=0.0.220
     mypy >=0.812
     pin >=2.6.4
     pylint >=2.8.2
     qpsolvers >=2.7.2
     quadprog >=0.1.11
-    robot_descriptions >=0.5.0
+    robot_descriptions >=1.4.1
 commands =
     black --check --diff pink
     ruff pink
     pylint pink --exit-zero --rcfile={toxinidir}/tox.ini
     mypy pink --ignore-missing-imports
 
 [pylint]
```

### Comparing `pin-pink-0.8.0/PKG-INFO` & `pin-pink-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pin-pink
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python inverse kinematics for your robot model based on Pinocchio.
 Keywords: inverse,kinematics,pinocchio
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -118,15 +118,15 @@
 Body tasks can be initialized, for example, from the robot's neutral configuration:
 
 ```python
 import pink
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
 robot = load_robot_description("upkie_description")
-configuration = pink.apply_configuration(robot, robot.q0)
+configuration = pink.Configuration(robot.model, robot.data, robot.q0)
 for body, task in tasks.items():
     if type(task) is BodyTask:
         task.set_target(configuration.get_transform_body_to_world(body))
 ```
 
 A task can be added to the inverse kinematics once both its cost and target (if applicable) are defined.
 
@@ -134,43 +134,47 @@
 
 Pink solves differential inverse kinematics, meaning it outputs a velocity that steers the robot towards achieving all tasks at best. If we keep integrating that velocity, and task targets don't change over time, we will converge to a stationary configuration:
 
 ```python
 dt = 6e-3  # [s]
 for t in np.arange(0.0, 42.0, dt):
     velocity = solve_ik(configuration, tasks.values(), dt, solver="quadprog")
-    q = configuration.integrate(velocity, dt)
-    configuration = pink.apply_configuration(robot, q)
+    configuration.integrate_inplace(velocity, dt)
     time.sleep(dt)
 ```
 
 If task targets are continuously updated, there will be no stationary solution to converge to, but the model will keep on tracking each target at best. Note that [`solve_ik`](https://scaron.info/doc/pink/inverse-kinematics.html#pink.solve_ik.solve_ik) will take care of both configuration and velocity limits read from the robot model.
 
 ## Examples
 
-Pink works with all kinds of robot morphologies:
-
-* Arm: [Kinova Gen2](https://github.com/tasts-robots/pink/blob/master/examples/arm_kinova_gen2.py)
-* Arm: [UR3](https://github.com/tasts-robots/pink/blob/master/examples/arm_ur3.py)
-* Humanoid: [JVRC-1](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_jvrc.py)
-* Humanoid: [SigmaBan](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_sigmaban.py)
-* Wheeled biped: [Upkie](https://github.com/tasts-robots/pink/blob/master/examples/wheeled_biped_upkie.py)
-* Wheeled: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/omnidirectional_wheeled_robot.py)
-
-Basic examples are the best to get started:
+Basic examples to get started:
 
 * [Double pendulum](https://github.com/tasts-robots/pink/blob/master/examples/double_pendulum.py)
 * [Loading a custom URDF](https://github.com/tasts-robots/pink/blob/master/examples/load_custom_urdf.py)
 * [Visualization in MeshCat](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_meshcat.py)
 * [Visualization in yourdfpy](https://github.com/tasts-robots/pink/blob/master/examples/visualize_in_yourdfpy.py)
 
+Pink works with all kinds of robot morphologies:
+
+* Arms: [Kinova Gen2](https://github.com/tasts-robots/pink/blob/master/examples/arm_kinova_gen2.py), [UR3](https://github.com/tasts-robots/pink/blob/master/examples/arm_ur3.py)
+* Humanoids: [JVRC-1](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_jvrc.py), [SigmaBan](https://github.com/tasts-robots/pink/blob/master/examples/humanoid_sigmaban.py)
+* Wheeled biped: [Upkie](https://github.com/tasts-robots/pink/blob/master/examples/wheeled_biped_upkie.py)
+* Wheeled: [Omnidirectional robot](https://github.com/tasts-robots/pink/blob/master/examples/omnidirectional_wheeled_robot.py)
+
 Check out the [examples](https://github.com/tasts-robots/pink/tree/master/examples) folder for more.
 
 ## How can I help?
 
 Install the library and use it! Report bugs in the [issue tracker](https://github.com/tasts-robots/pink/issues). If you are a developer with some robotics experience looking to hack on open source, check out the [contribution guidelines](CONTRIBUTING.md).
 
 ## See also
 
+Software:
+
 - [Jink.jl](https://github.com/adubredu/Jink.jl): Julia package for differential multi-task inverse kinematics.
 - [pymanoid](https://github.com/stephane-caron/pymanoid): precursor to Pink based on OpenRAVE.
 
+Technical notes:
+
+- [Inverse kinematics](https://scaron.info/robotics/inverse-kinematics.html): a general introduction to differential inverse kinematics.
+- [Jacobian of a kinematic task and derivatives on manifolds](https://scaron.info/robotics/jacobian-of-a-kinematic-task-and-derivatives-on-manifolds.html).
+
```

