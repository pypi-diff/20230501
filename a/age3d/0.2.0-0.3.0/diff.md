# Comparing `tmp/age3d-0.2.0.tar.gz` & `tmp/age3d-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "age3d-0.2.0.tar", last modified: Sat Apr 29 06:18:45 2023, max compression
+gzip compressed data, was "age3d-0.3.0.tar", last modified: Mon May  1 04:38:56 2023, max compression
```

## Comparing `age3d-0.2.0.tar` & `age3d-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.991797 age3d-0.2.0/
--rw-rw-rw-   0        0        0      294 2023-04-29 06:09:41.000000 age3d-0.2.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0      493 2023-04-04 09:58:38.000000 age3d-0.2.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1114 2023-03-26 00:42:17.000000 age3d-0.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11357 2023-03-24 19:50:45.000000 age3d-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      644 2023-04-05 00:11:10.000000 age3d-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2570 2023-04-04 09:58:38.000000 age3d-0.2.0/Makefile
--rw-rw-rw-   0        0        0    17220 2023-04-29 06:18:45.990802 age3d-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3132 2023-04-04 09:58:38.000000 age3d-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.917794 age3d-0.2.0/age3d/
--rw-rw-rw-   0        0        0      339 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/__init__.py
--rw-rw-rw-   0        0        0     1215 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/__main__.py
--rw-rw-rw-   0        0        0       22 2023-04-29 06:09:41.000000 age3d-0.2.0/age3d/_version.py
--rw-rw-rw-   0        0        0    14077 2023-04-29 06:09:41.000000 age3d-0.2.0/age3d/age3d.py
--rw-rw-rw-   0        0        0    17586 2023-04-04 11:40:52.000000 age3d-0.2.0/age3d/examples.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.949794 age3d-0.2.0/age3d/models/
--rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.2.0/age3d/models/monkey.stl
--rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.2.0/age3d/models/monkey_cleaned.stl
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.954800 age3d-0.2.0/age3d/tests/
--rw-rw-rw-   0        0        0    11744 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/tests/monkey_triangles.npy
--rw-rw-rw-   0        0        0    68912 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/tests/monkey_vertices.npy
--rw-rw-rw-   0        0        0     7056 2023-03-25 23:20:12.000000 age3d-0.2.0/age3d/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.946796 age3d-0.2.0/age3d.egg-info/
--rw-rw-rw-   0        0        0    17220 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      912 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 06:18:45.000000 age3d-0.2.0/age3d.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.966795 age3d-0.2.0/docs/
--rw-rw-rw-   0        0        0      683 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0     1209 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       96 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/documentation.rst
--rw-rw-rw-   0        0        0    14680 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/examples.rst
--rw-rw-rw-   0        0        0     1340 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/getting_started.rst
-drwxrwxrwx   0        0        0        0 2023-04-29 06:18:45.986797 age3d-0.2.0/docs/img/
--rw-rw-rw-   0        0        0    63875 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey.png
--rw-rw-rw-   0        0        0    69385 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_below_above_between.png
--rw-rw-rw-   0        0        0   100655 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_bound_height.png
--rw-rw-rw-   0        0        0    81498 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_erode.png
--rw-rw-rw-   0        0        0   127495 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_erode_wireframe.png
--rw-rw-rw-   0        0        0    64955 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_min_max.png
--rw-rw-rw-   0        0        0    58693 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_neighbors.png
--rw-rw-rw-   0        0        0    67341 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_pc.png
--rw-rw-rw-   0        0        0   125751 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_subdivision.png
--rw-rw-rw-   0        0        0    73476 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/img/monkey_wireframe.png
--rw-rw-rw-   0        0        0      454 2023-04-04 11:40:52.000000 age3d-0.2.0/docs/index.rst
--rwxrwxrwx   0        0        0      765 2023-04-04 06:54:19.000000 age3d-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0     2214 2023-04-29 06:09:41.000000 age3d-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 06:18:45.991797 age3d-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-24 19:50:45.000000 age3d-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.463701 age3d-0.3.0/
+-rw-rw-rw-   0        0        0      294 2023-05-01 04:33:59.000000 age3d-0.3.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      493 2023-04-04 09:58:38.000000 age3d-0.3.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1114 2023-03-26 00:42:17.000000 age3d-0.3.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11357 2023-03-24 19:50:45.000000 age3d-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      644 2023-04-05 00:11:10.000000 age3d-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2570 2023-04-04 09:58:38.000000 age3d-0.3.0/Makefile
+-rw-rw-rw-   0        0        0    17220 2023-05-01 04:38:56.462695 age3d-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3132 2023-04-04 09:58:38.000000 age3d-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.328187 age3d-0.3.0/age3d/
+-rw-rw-rw-   0        0        0      339 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/__init__.py
+-rw-rw-rw-   0        0        0     1215 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-05-01 04:33:59.000000 age3d-0.3.0/age3d/_version.py
+-rw-rw-rw-   0        0        0    17283 2023-05-01 04:33:59.000000 age3d-0.3.0/age3d/age3d.py
+-rw-rw-rw-   0        0        0    17586 2023-04-04 11:40:52.000000 age3d-0.3.0/age3d/examples.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.362158 age3d-0.3.0/age3d/models/
+-rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.3.0/age3d/models/monkey.stl
+-rw-rw-rw-   0        0        0    48484 2023-03-24 19:50:45.000000 age3d-0.3.0/age3d/models/monkey_cleaned.stl
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.369156 age3d-0.3.0/age3d/tests/
+-rw-rw-rw-   0        0        0    11744 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/tests/monkey_triangles.npy
+-rw-rw-rw-   0        0        0    68912 2023-03-25 23:20:12.000000 age3d-0.3.0/age3d/tests/monkey_vertices.npy
+-rw-rw-rw-   0        0        0     7171 2023-05-01 04:33:59.000000 age3d-0.3.0/age3d/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.357153 age3d-0.3.0/age3d.egg-info/
+-rw-rw-rw-   0        0        0    17220 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      912 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 04:38:56.000000 age3d-0.3.0/age3d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.431706 age3d-0.3.0/docs/
+-rw-rw-rw-   0        0        0      683 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/Makefile
+-rw-rw-rw-   0        0        0     1209 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0       96 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/documentation.rst
+-rw-rw-rw-   0        0        0    14680 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/examples.rst
+-rw-rw-rw-   0        0        0     1340 2023-04-29 06:53:06.000000 age3d-0.3.0/docs/getting_started.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 04:38:56.459707 age3d-0.3.0/docs/img/
+-rw-rw-rw-   0        0        0    63875 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey.png
+-rw-rw-rw-   0        0        0    69385 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_below_above_between.png
+-rw-rw-rw-   0        0        0   100655 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_bound_height.png
+-rw-rw-rw-   0        0        0    81498 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_erode.png
+-rw-rw-rw-   0        0        0   127495 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_erode_wireframe.png
+-rw-rw-rw-   0        0        0    64955 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_min_max.png
+-rw-rw-rw-   0        0        0    58693 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_neighbors.png
+-rw-rw-rw-   0        0        0    67341 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_pc.png
+-rw-rw-rw-   0        0        0   125751 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_subdivision.png
+-rw-rw-rw-   0        0        0    73476 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/img/monkey_wireframe.png
+-rw-rw-rw-   0        0        0      454 2023-04-04 11:40:52.000000 age3d-0.3.0/docs/index.rst
+-rwxrwxrwx   0        0        0      765 2023-04-04 06:54:19.000000 age3d-0.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0     2214 2023-05-01 04:33:59.000000 age3d-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 04:38:56.463701 age3d-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-24 19:50:45.000000 age3d-0.3.0/setup.py
```

### Comparing `age3d-0.2.0/CONTRIBUTING.md` & `age3d-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/LICENSE` & `age3d-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/MANIFEST.in` & `age3d-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/Makefile` & `age3d-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/PKG-INFO` & `age3d-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age3d
-Version: 0.2.0
+Version: 0.3.0
 Summary: Aging 3D models
 Author-email: Abhishek Chaudhary <ac5003@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `age3d-0.2.0/README.md` & `age3d-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/__main__.py` & `age3d-0.3.0/age3d/__main__.py`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/age3d.py` & `age3d-0.3.0/age3d/age3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     Imports stl file as Mesh
 
     Args:
         file_path (str): file path of stl file
 
     Returns:
-
+        mesh (open3d.geometry.TriangleMesh): Mesh to be processed.
     """
     mesh = o3d.io.read_triangle_mesh(file_path)
     return mesh
 
 
 def export_mesh(file_path: str, mesh):
     """
@@ -310,28 +310,45 @@
     max_x_vertex = mesh_vertices_np[np.argmin(mesh_vertices_np[:, 0])]
     min_y_vertex = mesh_vertices_np[np.argmin(mesh_vertices_np[:, 1])]
     max_y_vertex = mesh_vertices_np[np.argmin(mesh_vertices_np[:, 1])]
 
     return min(min_x_vertex[2], max_x_vertex[2], min_y_vertex[2], max_y_vertex[2])
 
 
-def erode(mesh, iterations=2, erosion_lifetime=10):
+def erode(mesh: o3d.geometry.TriangleMesh, iterations: int = 2, erosion_lifetime: int = 10, verbose: list = []):
     """
     Erodes the mesh using the particle deposition and erosion method.
 
     Args:
         mesh (open3d.geometry.TriangleMesh): The mesh to be eroded.
         iterations (int, optional): The number of iterations for the erosion process. Defaults to 2.
         erosion_lifetime (int, optional): The maximum number of times a vertex can be eroded. Defaults to 10.
+        verbose (list[str], optional): A list of strings containing information to be printed.
+            Possible strings include 'all', 'vertex_progression', 'vector_direction',
+            'vector_angle', 'ray', 'ray_scene', 'mesh', and 'collision'.
+            Defaults to an empty list.
 
     Returns:
         Tuple[np.ndarray, open3d.geometry.TriangleMesh]: A tuple containing the updated vertex
         indices and the eroded mesh.
+
+    The `verbose` argument takes a list of strings that specify what information should be printed.
+        - 'all': Prints all below.
+        - 'vertex_progression': Prints information about vertex triples.
+        - 'vector_direction': Prints information about vector directions.
+        - 'vector_angle': Prints information about vector angles.
+        - 'ray': Prints information about the ray being casted.
+        - 'ray_scene': Prints information about the raycasting scene.
+        - 'mesh': Prints information about the mesh.
+        - 'collision': Prints information about the collision detection.
     """
     # total_vertex_count = np.asarray(mesh.vertices).shape[0]
+    verbose = set(verbose)
+    if len(verbose) > 0:
+        print('Printing with Settings:', verbose)
 
     vertices_idx, vertices = find_all_above(mesh, calculate_bounds_height(mesh), True)
 
     set_vertices_idx = set()
     for idx in vertices_idx:
         set_vertices_idx.add(idx)
     # print('set', set_vertices_idx)
@@ -359,54 +376,98 @@
         while lifetime < erosion_lifetime:
             neighbors_idx, _ = find_neighbors(new_mesh, v_idx_curr)
             v_idx_next = int(find_minimum(new_mesh, 1, neighbors_idx)[0])
 
             if v_idx_next not in vertices_idx:
                 break
 
-            # if #TODO Angle Calculations
             if v_idx_prev:
-                print(
-                    v_idx_prev,
-                    v_idx_curr,
-                    v_idx_next,
-                    type(new_vertices[v_idx_prev]),
-                    new_vertices[v_idx_prev],
-                    new_vertices[v_idx_curr],
-                    new_vertices[v_idx_next],
-                )
+                if 'vertex_progression' in verbose or 'all' in verbose:
+                    print(
+                        'Vertex Triples:',
+                        v_idx_prev,
+                        v_idx_curr,
+                        v_idx_next,
+                        type(new_vertices[v_idx_prev]),
+                        new_vertices[v_idx_prev],
+                        new_vertices[v_idx_curr],
+                        new_vertices[v_idx_next],
+                    )
                 vector_1 = new_vertices[v_idx_curr] - new_vertices[v_idx_prev]
                 vector_2 = new_vertices[v_idx_next] - new_vertices[v_idx_curr]
                 direction_1 = np.sign(vector_1)
                 direction_2 = np.sign(vector_2)
-                # print(vector_1, vector_2, direction_1, direction_2, np.dot(direction_1 , direction_2))
+                if 'vector_direction' in verbose or 'all' in verbose:
+                    print(vector_1, vector_2, direction_1, direction_2, np.dot(direction_1, direction_2))
 
                 if vector_2[2] > 0:
                     break
 
                 vector_1[2] = 0
                 vector_2[2] = 0
                 norm_vector_1 = np.linalg.norm(vector_1)
                 norm_vector_2 = np.linalg.norm(vector_2)
                 angle = np.arccos(np.clip(np.dot(vector_1, vector_2) / (norm_vector_1 * norm_vector_2), -1.0, 1.0))
-                print(vector_1, vector_2, direction_1, direction_2, np.dot(direction_1, direction_2), angle)
-                # if angle < 0:
-                #     print('negative angle', angle)
+                if 'vector_angle' in verbose or 'all' in verbose:
+                    print(vector_1, vector_2, direction_1, direction_2, np.dot(direction_1, direction_2), angle)
+                    # if angle < 0:
+                    #     print('Negative angle Calculated', angle)
                 if angle > np.pi / 2:
-                    # print('pi angle', angle)
+                    if 'vector_angle' in verbose or 'all' in verbose:
+                        print('Angle found > PI / 2', angle)
                     break
-                # if angle > np.pi / 2
 
-            new_vertices[v_idx_curr, 2] -= (
-                strength * abs(new_vertices[v_idx_next, 2] - new_vertices[v_idx_curr, 2]) / mesh_max_height
-            )
+            ray = o3d.core.Tensor([[*new_vertices[v_idx_curr], 0, 0, 1]], dtype=o3d.core.Dtype.Float32)
+            if 'ray' in verbose or 'all' in verbose:
+                print('ray:', ray, 'vertex:', new_vertices[v_idx_curr])
+
+            ray[0, 2] += 1e-6
+            if 'ray' in verbose or 'all' in verbose:
+                print('updated ray:', ray, 'vertex:', new_vertices[v_idx_curr])
+
+            raycasting_scene = o3d.t.geometry.RaycastingScene()
+            if 'ray_scene' in verbose or 'all' in verbose:
+                print('scene:', raycasting_scene)
+
+            if 'mesh' in verbose or 'all' in verbose:
+                print('new mesh', new_mesh, type(new_mesh))
+            new_mesh_legacy = o3d.t.geometry.TriangleMesh.from_legacy(new_mesh)
+            if 'mesh' in verbose or 'all' in verbose:
+                print('new mesh legacy', new_mesh_legacy, type(new_mesh_legacy))
+
+            mesh_id = raycasting_scene.add_triangles(new_mesh_legacy)
+            if 'mesh' in verbose or 'all' in verbose:
+                print('mesh_id:', mesh_id)
+
+            collision = raycasting_scene.cast_rays(ray)
+            if 'collision' in verbose or 'all' in verbose:
+                print(
+                    'collision t_hit:',
+                    collision['t_hit'],
+                    type(collision['t_hit']),
+                    collision['t_hit'].numpy(),
+                    type(collision['t_hit'].numpy()),
+                )
+
+            if collision['t_hit'].numpy()[0] == np.inf:
+                new_vertices[v_idx_curr, 2] -= (
+                    strength * abs(new_vertices[v_idx_next, 2] - new_vertices[v_idx_curr, 2]) / mesh_max_height
+                )
+            else:
+                new_vertices[v_idx_curr, 2] += (
+                    strength * abs(new_vertices[v_idx_next, 2] - new_vertices[v_idx_curr, 2]) / mesh_max_height
+                )
+
             new_mesh.vertices = o3d.utility.Vector3dVector(new_vertices)
             updated_vertices.append(v_idx_curr)
 
             lifetime += 1
             strength *= 0.69
             v_idx_prev = v_idx_curr
             v_idx_curr = v_idx_next
 
+    if len(verbose) > 0:
+        print('')
+
     new_mesh.vertices = o3d.utility.Vector3dVector(new_vertices)
     new_mesh.triangles = o3d.utility.Vector3iVector(new_triangles)
     return np.array(updated_vertices), new_mesh
```

### Comparing `age3d-0.2.0/age3d/examples.ipynb` & `age3d-0.3.0/age3d/examples.ipynb`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/models/monkey.stl` & `age3d-0.3.0/age3d/models/monkey.stl`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/models/monkey_cleaned.stl` & `age3d-0.3.0/age3d/models/monkey_cleaned.stl`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/tests/monkey_triangles.npy` & `age3d-0.3.0/age3d/tests/monkey_triangles.npy`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/tests/monkey_vertices.npy` & `age3d-0.3.0/age3d/tests/monkey_vertices.npy`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/age3d/tests/test_all.py` & `age3d-0.3.0/age3d/tests/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,16 @@
     mesh.vertices = o3d.utility.Vector3dVector(vertices)
     mesh.triangles = o3d.utility.Vector3iVector(triangles)
     v_idx, vertices = age3d.find_neighbors(mesh, 0)
 
     assert all(v_idx == [1, 2])
 
 
-@pytest.mark.parametrize(('file_path'), ["age3d/models/monkey.stl"])
-def test_full_run(file_path):
+@pytest.mark.parametrize(
+    ('file_path', 'verbose'), [("age3d/models/monkey.stl", ['all']), ("age3d/models/monkey.stl", [])]
+)
+def test_full_run(file_path, verbose):
     mesh = age3d.import_mesh(file_path)
-    mesh = age3d.mesh_subdivision(mesh, 3)
-    _, new_mesh = age3d.erode(mesh, 10, 10)
+    mesh = age3d.mesh_subdivision(mesh, 2)
+    _, new_mesh = age3d.erode(mesh, iterations=50, erosion_lifetime=10, verbose=verbose)
 
     assert all(np.asarray(mesh.triangles).flatten() == np.asarray(new_mesh.triangles).flatten())
```

### Comparing `age3d-0.2.0/age3d.egg-info/PKG-INFO` & `age3d-0.3.0/age3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: age3d
-Version: 0.2.0
+Version: 0.3.0
 Summary: Aging 3D models
 Author-email: Abhishek Chaudhary <ac5003@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `age3d-0.2.0/age3d.egg-info/SOURCES.txt` & `age3d-0.3.0/age3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/Makefile` & `age3d-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/conf.py` & `age3d-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/examples.rst` & `age3d-0.3.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/getting_started.rst` & `age3d-0.3.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey.png` & `age3d-0.3.0/docs/img/monkey.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_below_above_between.png` & `age3d-0.3.0/docs/img/monkey_below_above_between.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_bound_height.png` & `age3d-0.3.0/docs/img/monkey_bound_height.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_erode.png` & `age3d-0.3.0/docs/img/monkey_erode.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_erode_wireframe.png` & `age3d-0.3.0/docs/img/monkey_erode_wireframe.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_min_max.png` & `age3d-0.3.0/docs/img/monkey_min_max.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_neighbors.png` & `age3d-0.3.0/docs/img/monkey_neighbors.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_pc.png` & `age3d-0.3.0/docs/img/monkey_pc.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_subdivision.png` & `age3d-0.3.0/docs/img/monkey_subdivision.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/img/monkey_wireframe.png` & `age3d-0.3.0/docs/img/monkey_wireframe.png`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/docs/make.bat` & `age3d-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `age3d-0.2.0/pyproject.toml` & `age3d-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "age3d"
 authors = [{name = "Abhishek Chaudhary", email = "ac5003@columbia.edu"}]
 description="Aging 3D models"
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "open3d==0.16.0"
 ]
 
 classifiers = [
```

