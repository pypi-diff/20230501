# Comparing `tmp/magicsoup-0.3.7.tar.gz` & `tmp/magicsoup-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.3.7.tar", last modified: Mon Apr 24 13:55:21 2023, max compression
+gzip compressed data, was "magicsoup-0.3.8.tar", last modified: Mon May  1 19:54:06 2023, max compression
```

## Comparing `magicsoup-0.3.7.tar` & `magicsoup-0.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.7/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-24 13:55:21.286378 magicsoup-0.3.7/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.7/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.7/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-24 13:55:21.286378 magicsoup-0.3.7/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-24 13:55:08.000000 magicsoup-0.3.7/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.7/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.7/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.7/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.7/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.7/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.7/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-14 19:52:19.000000 magicsoup-0.3.7/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    30687 2023-04-14 20:12:02.000000 magicsoup-0.3.7/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-12 14:59:48.000000 magicsoup-0.3.7/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.7/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    42780 2023-04-24 13:53:53.000000 magicsoup-0.3.7/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-24 13:55:21.000000 magicsoup-0.3.7/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-24 13:55:21.286378 magicsoup-0.3.7/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.7/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.7/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.7/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.7/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.7/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-01 19:54:06.189160 magicsoup-0.3.8/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.8/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-05-01 19:54:06.189160 magicsoup-0.3.8/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.8/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.8/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-05-01 19:54:06.189160 magicsoup-0.3.8/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-01 19:54:06.189160 magicsoup-0.3.8/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-01 19:54:06.189160 magicsoup-0.3.8/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-05-01 19:53:50.000000 magicsoup-0.3.8/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.3.8/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-27 20:14:11.000000 magicsoup-0.3.8/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-01 19:54:06.189160 magicsoup-0.3.8/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.8/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.8/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.8/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.8/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.3.8/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    30687 2023-04-27 20:15:08.000000 magicsoup-0.3.8/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-27 20:15:25.000000 magicsoup-0.3.8/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.8/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    42942 2023-05-01 19:50:00.000000 magicsoup-0.3.8/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-01 19:54:06.189160 magicsoup-0.3.8/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-05-01 19:54:06.000000 magicsoup-0.3.8/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-05-01 19:54:06.000000 magicsoup-0.3.8/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-05-01 19:54:06.000000 magicsoup-0.3.8/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-05-01 19:54:06.000000 magicsoup-0.3.8/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-01 19:54:06.189160 magicsoup-0.3.8/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.8/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.8/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    46871 2023-04-27 20:17:09.000000 magicsoup-0.3.8/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.8/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    19437 2023-05-01 19:52:39.000000 magicsoup-0.3.8/tests/test_world.py
```

### Comparing `magicsoup-0.3.7/LICENSE` & `magicsoup-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/PKG-INFO` & `magicsoup-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.7
+Version: 0.3.8
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.7/README.md` & `magicsoup-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/pyproject.toml` & `magicsoup-0.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/constants.py` & `magicsoup-0.3.8/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/containers.py` & `magicsoup-0.3.8/src/magicsoup/containers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import warnings
 import torch
+import warnings
 
 
 class Molecule:
     """
     Represents a molecule species which is part of the world, can diffuse, degrade,
     and be converted into other molecules.
```

### Comparing `magicsoup-0.3.7/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.3.8/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.3.8/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.3.8/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/genetics.py` & `magicsoup-0.3.8/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/kinetics.py` & `magicsoup-0.3.8/src/magicsoup/kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/mutations.py` & `magicsoup-0.3.8/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/util.py` & `magicsoup-0.3.8/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/src/magicsoup/world.py` & `magicsoup-0.3.8/src/magicsoup/world.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     CatalyticDomainFact,
     TransporterDomainFact,
     RegulatoryDomainFact,
 )
 from magicsoup.kinetics import Kinetics
 from magicsoup.genetics import Genetics
 
-import time
-
 
 def _torch_load(map_loc: str | None = None):
     # Closure rather than a lambda to preserve map_loc
     return lambda b: torch.load(BytesIO(b), map_location=map_loc)
 
 
 class _CPU_Unpickler(pickle.Unpickler):
@@ -509,18 +507,19 @@
             else:
                 kill_idxs.append(idx)
 
         proteomes = self.genetics.translate_genomes(genomes=transl_genomes)
 
         set_idxs = []
         set_proteomes = []
-        for proteome, idx in zip(proteomes, transl_idxs):
+        for proteome, idx, genome in zip(proteomes, transl_idxs, transl_genomes):
             if len(proteome) > 0:
                 set_proteomes.append(proteome)
                 set_idxs.append(idx)
+                self.genomes[idx] = genome
             else:
                 kill_idxs.append(idx)
 
         if len(set_proteomes) > 0:
             max_prots = max(len(d) for d in set_proteomes)
             self.kinetics.increase_max_proteins(max_n=max_prots)
             self.kinetics.set_cell_params(cell_idxs=set_idxs, proteomes=set_proteomes)
@@ -542,14 +541,16 @@
         E.g. if there are 10 cells and you kill the cell with index 8 (the 9th cell),
         the cell that used to have index 9 (10th cell) will now have index 9.
         """
         n_killed_cells = len(cell_idxs)
         if n_killed_cells == 0:
             return
 
+        # TODO: do list(set(cell_idxs))?
+        #       because further down .pop would fail if duplicates
         xs = self.cell_positions[cell_idxs, 0]
         ys = self.cell_positions[cell_idxs, 1]
         self.cell_map[xs, ys] = False
 
         spillout = self.cell_molecules[cell_idxs, :]
         self.molecule_map[:, xs, ys] += spillout.T
```

### Comparing `magicsoup-0.3.7/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.3.8/src/magicsoup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.7
+Version: 0.3.8
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.7/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.3.8/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/tests/test_containers.py` & `magicsoup-0.3.8/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/tests/test_genetics.py` & `magicsoup-0.3.8/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/tests/test_kinetics.py` & `magicsoup-0.3.8/tests/test_kinetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from magicsoup.containers import (
     Molecule,
     CatalyticDomain,
     RegulatoryDomain,
     TransporterDomain,
 )
 from magicsoup.kinetics import Kinetics
-from magicsoup.constants import GAS_CONSTANT
 
 TOLERANCE = 1e-4
 
 
 ma = Molecule("a", energy=15)
 mb = Molecule("b", energy=10)
 mc = Molecule("c", energy=10)
@@ -188,15 +187,14 @@
     assert p1.domains[1].substrates == [mb, mc]
     assert p1.domains[1].products == [md]
     assert p1.domains[1].vmax == pytest.approx(1.2, abs=TOLERANCE)
     assert p1.domains[1].km == pytest.approx(1.5, abs=TOLERANCE)
 
 
 def test_cell_params_with_transporter_domains():
-
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
         [
             (2, 5, 5, 1, 1)  # transporter, Vmax 1.5, Km 0.5, fwd, mol a
         ],
         [
@@ -349,15 +347,14 @@
     assert isinstance(p1.domains[1], TransporterDomain)
     assert p1.domains[1].molecule is ma
     assert p1.domains[1].vmax == pytest.approx(1.5, abs=TOLERANCE)
     assert p1.domains[1].km == pytest.approx(0.5, abs=TOLERANCE)
 
 
 def test_cell_params_with_regulatory_domains():
-
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
         [
             (1, 10, 5, 1, 1), # catal, Vmax 2.0, Km 0.5, fwd, a->b
             (3, 0, 10, 1, 3), # reg, Km 1.0, cyto, act, c
             (3, 0, 20, 2, 4), # reg, Km 2.0, cyto, inh, d
@@ -580,15 +577,14 @@
     assert p1.domains[2].effector is md
     assert not p1.domains[2].is_inhibiting
     assert not p1.domains[2].is_transmembrane
     assert p1.domains[2].km == pytest.approx(1.5, abs=TOLERANCE)
 
 
 def test_cell_params_with_catalytic_domains():
-
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
         [
             (1, 1, 5, 1, 1), # catal, Vmax 1.1, Km 0.5, fwd, a->b
             (1, 2, 15, 2, 3), # catal, Vmax 1.2, Km 1.5, bwd, bc->d
         ],
@@ -1388,15 +1384,14 @@
     # reaction energies (c, p)
     E = torch.full((2, 3), -99999.9)
     # E = -2000 ^= # ln(Ke) = 0.77
     E[0, 0] = -2000 # ln(Q) - ln(Ke) = 1.53 (switch N)
     E[0, 1] = -2000 # ln(Q) - ln(Ke) = -0.76 (reduce V)
     E[1, 0] = -2000 # ln(Q) - ln(Ke) = 0.02 (switch off)
     E[1, 1] = -2000 # ln(Q) - ln(Ke) = 0.28 (switch N, reduce V)
-    lKe = -E / 310.0 / GAS_CONSTANT
 
     # fmt: on
 
     def mm(x, k, v):
         return v * x / (k + x)
 
     # expected outcome
```

### Comparing `magicsoup-0.3.7/tests/test_util.py` & `magicsoup-0.3.8/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.7/tests/test_world.py` & `magicsoup-0.3.8/tests/test_world.py`

 * *Files 6% similar despite different names*

```diff
@@ -539,7 +539,35 @@
     assert (c2_1.int_molecules == c2_0.int_molecules).all()
     assert c0_1.genome == c0_0.genome
     assert c1_1.genome == c1_0.genome
     assert c2_1.genome == c2_0.genome
     assert c0_1.label == c0_0.label
     assert c1_1.label == c1_0.label
     assert c2_1.label == c2_0.label
+
+
+def test_change_genomes():
+    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
+    world = ms.World(chemistry=chemistry)
+
+    g0 = ms.random_genome(s=500)
+    world.add_cells(genomes=[g0] * 2)
+    assert world.genomes == [g0] * 2
+
+    g1 = ms.random_genome(s=1000)
+    world.add_cells(genomes=[g1])
+    assert world.genomes == [g0] * 2 + [g1]
+
+    g2 = ms.random_genome(s=600)
+    world.update_cells(genome_idx_pairs=[(g2, 1)])
+    assert world.genomes == [g0, g2, g1]
+
+    world.kill_cells(cell_idxs=[0])
+    assert world.genomes == [g2, g1]
+
+    g3 = ms.random_genome(s=700)
+    world.update_cells(genome_idx_pairs=[(g3, 1)])
+    assert world.genomes == [g2, g3]
+
+    g4 = ms.random_genome(s=500)
+    world.add_cells(genomes=[g4])
+    assert world.genomes == [g2, g3, g4]
```

