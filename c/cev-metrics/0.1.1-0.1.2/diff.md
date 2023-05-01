# Comparing `tmp/cev_metrics-0.1.1.tar.gz` & `tmp/cev_metrics-0.1.2.tar.gz`

## Comparing `cev_metrics-0.1.1.tar` & `cev_metrics-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cev_metrics-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2845 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      123      152 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/.gitignore
--rw-r--r--   0     1001      123       63 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/README.md
--rw-r--r--   0     1001      123       10 2023-04-28 17:38:04.000000 cev_metrics-0.1.1/dist/cev_metrics-0.1.1.tar.gz
--rw-r--r--   0     1001      123      439 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123      362 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/python/cev_metrics/__init__.py
--rw-r--r--   0     1001      123     1647 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/python/cev_metrics/_rust.py
--rw-r--r--   0     1001      123    15314 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/python/cev_metrics/py.py
--rw-r--r--   0     1001      123    12891 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     3056 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/src/step_function.rs
--rwxr-xr-x   0     1001      123      492 2023-04-28 17:37:12.000000 cev_metrics-0.1.1/x.py
--rw-r--r--   0     1001      123    13105 2023-04-28 17:38:03.000000 cev_metrics-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 cev_metrics-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cev_metrics-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123     2845 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      152 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/.gitignore
+-rw-r--r--   0     1001      123       63 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/README.md
+-rw-r--r--   0     1001      123       10 2023-05-01 14:19:42.000000 cev_metrics-0.1.2/dist/cev_metrics-0.1.2.tar.gz
+-rw-r--r--   0     1001      123      439 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123      362 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/python/cev_metrics/__init__.py
+-rw-r--r--   0     1001      123     1647 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/python/cev_metrics/_rust.py
+-rw-r--r--   0     1001      123    15314 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/python/cev_metrics/py.py
+-rw-r--r--   0     1001      123    12819 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123     3056 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/src/step_function.rs
+-rwxr-xr-x   0     1001      123      492 2023-05-01 14:18:40.000000 cev_metrics-0.1.2/x.py
+-rw-r--r--   0     1001      123    13117 2023-05-01 14:19:41.000000 cev_metrics-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 cev_metrics-0.1.2/PKG-INFO
```

### Comparing `cev_metrics-0.1.1/.github/workflows/ci.yml` & `cev_metrics-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.1/python/cev_metrics/_rust.py` & `cev_metrics-0.1.2/python/cev_metrics/_rust.py`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.1/python/cev_metrics/py.py` & `cev_metrics-0.1.2/python/cev_metrics/py.py`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.1/src/lib.rs` & `cev_metrics-0.1.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     set: HashSet<NodeIndex>,
     boundaries: HashSet<EdgeIndex>,
     labels: &'a Labels<'a>,
 }
 
 impl<'a> ConfusionResult<'a> {
     fn contains(&self, node: &NodeIndex) -> bool {
-        self.set.contains(&node)
+        self.set.contains(node)
     }
 }
 
 trait ConfusionMatrix {
     fn counts(&self) -> Array2<u64>;
 }
 
@@ -68,18 +68,16 @@
         let mut data = vec![None; self.labels.n_categories];
         for (label, distance) in &self.distances {
             data[*label] = match data[*label] {
                 None => Some((1, *distance)),
                 Some(x) => Some((x.0 + 1, x.1 + *distance)),
             }
         }
-        for entry in data.iter_mut() {
-            if let Some((count, total)) = entry {
-                *total = *total / *count as f64;
-            }
+        for (count, total) in data.iter_mut().flatten() {
+            *total /= *count as f64;
         }
         data
     }
 }
 
 trait NeighborhoodSummary {
     fn scores(&self) -> Array2<f64>;
@@ -183,26 +181,26 @@
                     acc
                 },
             );
 
         // TODO, avoid second pass? Can we save edges found in bfs?
         let mut boundary_edges = HashSet::new();
 
-        for source in visited_with_threshold {
-            for edge in graph.graph.edges(source) {
+        for source in &visited_with_threshold {
+            for edge in graph.graph.edges(*source) {
                 if visited_without_threshold.contains(&edge.target()) {
                     boundary_edges.insert(edge.id());
                 }
             }
         }
 
         ConfusionResult {
-            set: visited_without_threshold,
+            set: visited_with_threshold,
             boundaries: boundary_edges,
-            labels: &self,
+            labels: self,
         }
     }
 
     fn confusion(&self, graph: &Graph) -> Vec<ConfusionResult> {
         (0..self.n_categories)
             .zip(self.confusion_threshold(graph))
             .map(|(label, threshold)| {
@@ -236,32 +234,32 @@
             })
             .collect();
 
         let connections = visited.iter().flat_map(|(edge, targets)| {
             let source_point = &graph.points[edge.source().index()];
             targets
                 .iter()
-                .filter(|target| !confusion_result.contains(&target))
+                .filter(|target| !confusion_result.contains(target))
                 .map(|target| {
                     let target_label = self.codes[target.index()] as usize;
                     let target_point = &graph.points[target.index()];
                     (target_label, euclidean_distance(source_point, target_point))
                 })
         });
 
         NeighborhoodResult {
             distances: boundary_distances.chain(connections).collect(),
-            labels: &self,
+            labels: self,
         }
     }
 
     fn neighborhood(
         &self,
         graph: &Graph,
-        counfusion_results: &Vec<ConfusionResult>,
+        counfusion_results: &[ConfusionResult],
         max_depth: usize,
     ) -> Vec<NeighborhoodResult> {
         counfusion_results
             .iter()
             .map(|c| self.neighborhood_for_label(graph, c, max_depth))
             .collect()
     }
@@ -275,15 +273,15 @@
 }
 
 impl From<&Vec<Point>> for Graph {
     fn from(points: &Vec<Point>) -> Self {
         let mut graph = UnGraph::<_, _>::from_elements(
             std::iter::repeat(Element::Node { weight: 0 }).take(points.len()),
         );
-        for triangle in triangulate(&points).triangles.chunks(3) {
+        for triangle in triangulate(points).triangles.chunks(3) {
             let (a, b, c) = (triangle[0], triangle[1], triangle[2]);
             // `update_edge` avoids adding duplicate edges
             graph.update_edge(
                 NodeIndex::new(a),
                 NodeIndex::new(b),
                 euclidean_distance(&points[a], &points[b]),
             );
@@ -376,41 +374,41 @@
 
     #[pyfn(m, name = "_confusion")]
     fn confusion_py<'py>(
         py: Python<'py>,
         graph: &Graph,
         codes: PyReadonlyArray1<'_, i16>,
     ) -> &'py PyArray2<u64> {
-        let labels = Labels::from_codes(&codes.as_slice().unwrap());
-        let confusion = labels.confusion(&graph);
+        let labels = Labels::from_codes(codes.as_slice().unwrap());
+        let confusion = labels.confusion(graph);
         confusion.counts().into_pyarray(py)
     }
 
     #[pyfn(m, name="_neighborhood", signature=(graph, codes, max_depth=1))]
     fn neighborhood_py<'py>(
         py: Python<'py>,
         graph: &Graph,
         codes: PyReadonlyArray1<'_, i16>,
         max_depth: usize,
     ) -> &'py PyArray2<f64> {
-        let labels = Labels::from_codes(&codes.as_slice().unwrap());
-        let confusion = labels.confusion(&graph);
+        let labels = Labels::from_codes(codes.as_slice().unwrap());
+        let confusion = labels.confusion(graph);
         let neighborhood = labels.neighborhood(graph, &confusion, max_depth);
         neighborhood.scores().into_pyarray(py)
     }
 
     #[pyfn(m, name="_confusion_and_neighborhood", signature=(graph, codes, neighborhood_max_depth=1))]
     fn confusion_and_neighborhood_py<'py>(
         py: Python<'py>,
         graph: &Graph,
         codes: PyReadonlyArray1<'_, i16>,
         neighborhood_max_depth: usize,
     ) -> (&'py PyArray2<u64>, &'py PyArray2<f64>) {
-        let labels = Labels::from_codes(&codes.as_slice().unwrap());
-        let confusion = labels.confusion(&graph);
+        let labels = Labels::from_codes(codes.as_slice().unwrap());
+        let confusion = labels.confusion(graph);
         let neighborhood = labels.neighborhood(graph, &confusion, neighborhood_max_depth);
         (
             confusion.counts().into_pyarray(py),
             neighborhood.scores().into_pyarray(py),
         )
     }
```

### Comparing `cev_metrics-0.1.1/src/step_function.rs` & `cev_metrics-0.1.2/src/step_function.rs`

 * *Files identical despite different names*

### Comparing `cev_metrics-0.1.1/Cargo.lock` & `cev_metrics-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "cev-metrics"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "delaunator",
  "numpy",
  "petgraph",
  "pyo3",
  "rayon",
 ]
@@ -140,18 +140,19 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.3"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb99c395ae250e1bf9133673f03ca9f97b7e71b705436bf8f089453445d1e9fe"
+checksum = "fcce854c9e76cfd191182c280eb5460cb8efd2cb4e58a1fd56bc41102d7e5802"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

