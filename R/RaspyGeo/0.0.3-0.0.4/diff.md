# Comparing `tmp/RaspyGeo-0.0.3.tar.gz` & `tmp/RaspyGeo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RaspyGeo-0.0.3.tar", last modified: Wed Mar 29 21:37:55 2023, max compression
+gzip compressed data, was "RaspyGeo-0.0.4.tar", last modified: Mon May  1 20:02:43 2023, max compression
```

## Comparing `RaspyGeo-0.0.3.tar` & `RaspyGeo-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 21:37:55.676764 RaspyGeo-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-03-16 22:03:16.000000 RaspyGeo-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6270 2023-03-29 21:37:55.676764 RaspyGeo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5650 2023-03-29 20:49:32.000000 RaspyGeo-0.0.3/README.md
--rw-rw-rw-   0        0        0        0 2022-05-18 19:11:54.000000 RaspyGeo-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      802 2023-03-29 21:37:55.681750 RaspyGeo-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 21:37:55.604065 RaspyGeo-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 21:37:55.623015 RaspyGeo-0.0.3/src/RaspyGeo/
--rw-rw-rw-   0        0        0      156 2023-03-28 20:02:11.000000 RaspyGeo-0.0.3/src/RaspyGeo/__init__.py
--rw-rw-rw-   0        0        0     1463 2023-03-27 15:03:57.000000 RaspyGeo-0.0.3/src/RaspyGeo/display.py
--rw-rw-rw-   0        0        0    13195 2023-03-29 21:36:29.000000 RaspyGeo-0.0.3/src/RaspyGeo/geofun.py
--rw-rw-rw-   0        0        0     5645 2023-03-24 22:15:32.000000 RaspyGeo-0.0.3/src/RaspyGeo/hecgeo.py
--rw-rw-rw-   0        0        0     2784 2023-03-28 20:07:59.000000 RaspyGeo-0.0.3/src/RaspyGeo/iterate.py
--rw-rw-rw-   0        0        0     5175 2023-03-29 20:51:11.000000 RaspyGeo-0.0.3/src/RaspyGeo/parse_geo.py
--rw-rw-rw-   0        0        0     2518 2023-03-28 18:30:20.000000 RaspyGeo-0.0.3/src/RaspyGeo/testing.py
--rw-rw-rw-   0        0        0     7806 2023-03-29 20:52:49.000000 RaspyGeo-0.0.3/src/RaspyGeo/write_geo.py
-drwxrwxrwx   0        0        0        0 2023-03-29 21:37:55.675767 RaspyGeo-0.0.3/src/RaspyGeo.egg-info/
--rw-rw-rw-   0        0        0     6270 2023-03-29 21:37:55.000000 RaspyGeo-0.0.3/src/RaspyGeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-03-29 21:37:55.000000 RaspyGeo-0.0.3/src/RaspyGeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 21:37:55.000000 RaspyGeo-0.0.3/src/RaspyGeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-29 21:37:55.000000 RaspyGeo-0.0.3/src/RaspyGeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-29 21:37:55.000000 RaspyGeo-0.0.3/src/RaspyGeo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.843059 RaspyGeo-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-03-16 22:03:16.000000 RaspyGeo-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6542 2023-05-01 20:02:43.844056 RaspyGeo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5922 2023-05-01 20:02:15.000000 RaspyGeo-0.0.4/README.md
+-rw-rw-rw-   0        0        0        0 2022-05-18 19:11:54.000000 RaspyGeo-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      802 2023-05-01 20:02:43.845054 RaspyGeo-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.688850 RaspyGeo-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.778223 RaspyGeo-0.0.4/src/RaspyGeo/
+-rw-rw-rw-   0        0        0      156 2023-03-28 20:02:11.000000 RaspyGeo-0.0.4/src/RaspyGeo/__init__.py
+-rw-rw-rw-   0        0        0     1463 2023-03-27 15:03:57.000000 RaspyGeo-0.0.4/src/RaspyGeo/display.py
+-rw-rw-rw-   0        0        0    13548 2023-05-01 19:54:09.000000 RaspyGeo-0.0.4/src/RaspyGeo/geofun.py
+-rw-rw-rw-   0        0        0     5645 2023-03-24 22:15:32.000000 RaspyGeo-0.0.4/src/RaspyGeo/hecgeo.py
+-rw-rw-rw-   0        0        0     3628 2023-05-01 19:53:26.000000 RaspyGeo-0.0.4/src/RaspyGeo/iterate.py
+-rw-rw-rw-   0        0        0     5175 2023-03-29 20:51:11.000000 RaspyGeo-0.0.4/src/RaspyGeo/parse_geo.py
+-rw-rw-rw-   0        0        0     2518 2023-03-28 18:30:20.000000 RaspyGeo-0.0.4/src/RaspyGeo/testing.py
+-rw-rw-rw-   0        0        0     7806 2023-03-29 20:52:49.000000 RaspyGeo-0.0.4/src/RaspyGeo/write_geo.py
+drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.842063 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/
+-rw-rw-rw-   0        0        0     6542 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/top_level.txt
```

### Comparing `RaspyGeo-0.0.3/LICENSE` & `RaspyGeo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.3/PKG-INFO` & `RaspyGeo-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: RaspyGeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS
 Home-page: https://github.com/quantum-dan/RaspyGeo
 Author: Daniel Philippus
 Author-email: daniel@dphilippus.com
 Project-URL: Bug Tracker, https://github.com/quantum-dan/RaspyGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RaspyGeo
-Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS.  Depends on Raspy (`raspy-auto` on PyPI).  Works for steady-state simulations.
+
+Automated geometry scenario runner (loosely analogous to the Geometry Modification tool) for HEC-RAS.  Depends on Raspy (`raspy-auto` on PyPI).  Currently works for steady-state simulations. RaspyGeo is available on PyPI as [RaspyGeo](https://pypi.org/project/RaspyGeo/).
+
+# Updates and Added Features
+
+If additional capabilities would be useful to you, open an Issue and I will check
+into it.  Otherwise, I develop updates as I need them.
 
 # Usage
 
 Scenario running is fully automated through `run`.  The HEC-RAS project must
 already be set up with a reference (baseline) geometry **and** a new (scenario)
 geometry file, and the current plan must be set up to run the scenario geometry.
 Then, the user specifies:
```

### Comparing `RaspyGeo-0.0.3/README.md` & `RaspyGeo-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # RaspyGeo
-Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS.  Depends on Raspy (`raspy-auto` on PyPI).  Works for steady-state simulations.
+
+Automated geometry scenario runner (loosely analogous to the Geometry Modification tool) for HEC-RAS.  Depends on Raspy (`raspy-auto` on PyPI).  Currently works for steady-state simulations. RaspyGeo is available on PyPI as [RaspyGeo](https://pypi.org/project/RaspyGeo/).
+
+# Updates and Added Features
+
+If additional capabilities would be useful to you, open an Issue and I will check
+into it.  Otherwise, I develop updates as I need them.
 
 # Usage
 
 Scenario running is fully automated through `run`.  The HEC-RAS project must
 already be set up with a reference (baseline) geometry **and** a new (scenario)
 geometry file, and the current plan must be set up to run the scenario geometry.
 Then, the user specifies:
```

### Comparing `RaspyGeo-0.0.3/setup.cfg` & `RaspyGeo-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2052 6173 7079 4765 6f0d 0a76 6572   = RaspyGeo..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6175  sion = 0.0.3..au
+00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 6175  sion = 0.0.4..au
 00000030: 7468 6f72 203d 2044 616e 6965 6c20 5068  thor = Daniel Ph
 00000040: 696c 6970 7075 730d 0a61 7574 686f 725f  ilippus..author_
 00000050: 656d 6169 6c20 3d20 6461 6e69 656c 4064  email = daniel@d
 00000060: 7068 696c 6970 7075 732e 636f 6d0d 0a64  philippus.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 7574  escription = Aut
 00000080: 6f6d 6174 6564 2067 656f 6d65 7472 7920  omated geometry 
 00000090: 7363 656e 6172 696f 2072 756e 6e65 7220  scenario runner
```

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/display.py` & `RaspyGeo-0.0.4/src/RaspyGeo/display.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/geofun.py` & `RaspyGeo-0.0.4/src/RaspyGeo/geofun.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,24 +137,24 @@
         - LFC side slope roughness
         - LFC bottom roughness
     Bank stations are set at the top edges of the LFC.
     Units are assumed to be consistent with geometry and not accounted for.
     """
     def geofun(coordinates, roughness, banks):
         xs0 = [co[0] for co in coordinates]
-        ys0 = [co[1] for co in coordinates]
+        ys0 = [co[1] + lfc_h for co in coordinates]
         rox0 = [ro[0] for ro in roughness]
         ron0 = [ro[1] for ro in roughness]
         # First: identify center
         centx = 0.5*(min(xs0) + max(xs0))
         # Now,  build fixed geometry
         # LFC bottom
         lfc_bleft = centx - lfc_w / 2
         lfc_bright = centx + lfc_w / 2
-        lfc_by = min(ys0)
+        lfc_by = min(ys0) - lfc_h
         # LFC side slopes
         lfc_sw = lfc_z * lfc_h
         lfc_tleft = lfc_bleft - lfc_sw
         lfc_tright = lfc_bright + lfc_sw
         lfc_ty = lfc_by + lfc_h
         # This gives us the new bank stations, conveniently
         nbanks = (lfc_tleft, lfc_tright)
@@ -177,17 +177,21 @@
         # the existing channel (where do they daylight?)  Identifying
         # the daylight point gets its own function, for simplicity.
         # daylight(x, y, start, z, direction) returns the x-coordinate of
         # daylight.
         afp_tleft = daylight(xs0, ys0, afp_bleft,
                              lfc_ty, afp_z, -1) if avail > 0 else \
             afp_bleft - 0.1
+        afp_tleft = afp_tleft if afp_bleft - afp_tleft > 0.01 else \
+            afp_bleft - 0.1
         afp_tright = daylight(xs0, ys0, afp_bright,
                               lfc_ty, afp_z, 1) if avail > 0 else \
             afp_bright + 0.1
+        afp_tright = afp_tright if afp_tright - afp_bright > 0.01 else \
+            afp_bright + 0.1
         # Compute height based on side slope width and slope
         afp_tyleft = lfc_ty + (afp_bleft - afp_tleft) / afp_z if \
             avail > 0 else lfc_ty
         afp_tyright = lfc_ty + (afp_tright - afp_bright) / afp_z if \
             avail > 0 else lfc_ty
         # We now have all key points.  Next, we rebuild the coordinates
         # and specify roughness.
@@ -257,59 +261,59 @@
         side_n):
     """
     Simplified geometry function building just an LFC with horizontal
     daylighting.
     """
     def geofun(coordinates, roughness, banks):
         xs0 = [co[0] for co in coordinates]
-        ys0 = [co[1] for co in coordinates]
+        ys0 = [co[1] + lfc_h for co in coordinates]
         rox0 = [ro[0] for ro in roughness]
         ron0 = [ro[1] for ro in roughness]
         # First: identify center
         centx = 0.5*(min(xs0) + max(xs0))
         # Now,  build fixed geometry
         # LFC bottom
         lfc_bleft = centx - lfc_w / 2
         lfc_bright = centx + lfc_w / 2
-        lfc_by = min(ys0)
+        lfc_by = min(ys0) - lfc_h
         # LFC side slopes
         lfc_sw = lfc_z * lfc_h
         lfc_tleft = lfc_bleft - lfc_sw
         lfc_tright = lfc_bright + lfc_sw
         lfc_ty = lfc_by + lfc_h
         # This gives us the new bank stations, conveniently
         nbanks = (lfc_tleft, lfc_tright)
         keepl = [(x, ys0[ix]) for (ix, x) in enumerate(xs0)
                  if x < (lfc_tleft - 0.1)]
         keepr = [(x, ys0[ix]) for (ix, x) in enumerate(xs0)
                  if x > (lfc_tright + 0.1)]
         # Now, build the new geometry coordinates.
-        co_new = [
-            (keepl[-1][0] if len(keepl) > 0 else min(min(xs0), lfc_tleft),
-             lfc_ty),
-            (lfc_tleft, lfc_ty),
-            (lfc_bleft, lfc_by),
-            (lfc_bright, lfc_by),
-            (lfc_tright, lfc_ty),
-            (keepr[0][0] if len(keepr) > 0 else max(max(xs0), lfc_tright),
-             lfc_ty)
-            ]
+        co_new = ([(keepl[-1][0], lfc_ty)] if len(keepl) > 0 else []) +\
+            [(lfc_tleft, lfc_ty),
+             (lfc_bleft, lfc_by),
+             (lfc_bright, lfc_by),
+             (lfc_tright, lfc_ty)] +\
+            ([(keepr[0][0], lfc_ty)] if len(keepr) > 0 else [])
         # co_out = sorted(keepl + co_new + keepr,
         #                 key = lambda x: x[0])
         co_out = keepl[:-1] + co_new + keepr[1:]
         nkeepl = [(x, ron0[rox0.index(x)]) for x in rox0
                   if x < (lfc_tleft - 0.1)]
         nkeepr = [(x, ron0[rox0.index(x)]) for x in rox0
                   if x > (lfc_tright + 0.1)]
+        # Also need to find the roughness to continue with.
+        xnresume = max([x for x in rox0 if x < lfc_tright])
+        nresume = ron0[rox0.index(xnresume)]
         # Right-most coordinate that is left of the AFP edge.
         proprox = [rx for rx in rox0 if rx <= lfc_tright][-1]
         propn = ron0[rox0.index(proprox)]
         # Now we can build the new geometry.
         ro_new = [
             (lfc_tleft, side_n),
             (lfc_bleft, bot_n),
-            (lfc_bright, side_n)
+            (lfc_bright, side_n),
+            (lfc_tright, nresume)
             ]
         ro_out = sorted(nkeepl + ro_new + nkeepr,
                         key = lambda x: x[0])
         return (co_out, ro_out, nbanks)
     return geofun
```

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/hecgeo.py` & `RaspyGeo-0.0.4/src/RaspyGeo/hecgeo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/iterate.py` & `RaspyGeo-0.0.4/src/RaspyGeo/iterate.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,37 @@
 vel.lob,vel.mc,vel.rob,depth.lob,depth.mc,depth.rob\n"
 
 
 def row_join(row):
     return ",".join([str(r) for r in row])
 
 
+def twovalfix(vals, maxC=False, av=False):
+    # Sometimes HEC-RAS will return just two values.  This fixes it to
+    # distribute them across the overbanks and MC.
+    # If maxC (max center), the max value goes in the MC, and the missing
+    # value is set to 0.
+    # If av (average), then all three are set to the mean.
+    # If both are false, then it just returns three NAs.
+    if len(vals) == 3:
+        return vals
+    if len(vals) == 1:
+        return [0, vals[0], 0]
+    if maxC:
+        if vals[0] > vals[1]:  # larger is left
+            return [0] + vals
+        else:  # larger is right
+            return vals + [0]
+    if av:
+        mean = sum(vals)/len(vals)
+        return [mean, mean, mean]
+    else:
+        return ["NA", "NA", "NA"]
+
+
 def loc_data(ras, nprof, loc, scenario):
     # loc -> [identifier, river, reach, rs]
     # Returns [formatted row according to `cols`] for a single location
     # flow_data: {profile: SimData}, where SimData has
     # velocity, maxDepth, flow, shear as lists of [l, c, r]
     ident = loc[0]
     riv = loc[1].strip()
@@ -55,17 +78,17 @@
     flow_data = ras.data.allFlowDist(riv,
                                      rch,
                                      rs,
                                      nprof)
     return [row_join(
         [scenario, ident, riv, rch, rs,
          sum(fd.flow)] +
-        fd.shear +
-        fd.velocity +
-        fd.maxDepth
+        twovalfix(fd.shear, av=True) +
+        twovalfix(fd.velocity, maxC=True) +
+        twovalfix(fd.maxDepth, maxC=True)
         ) for fd in flow_data.values()]
 
 
 def scenario_data(ras, nprof, locations, scenario):
     # locations -> [[identifier, river, reach, rs]]
     # nprof -> number of flow profiles
     # Returns [formatted row according to `cols`]
```

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/parse_geo.py` & `RaspyGeo-0.0.4/src/RaspyGeo/parse_geo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/testing.py` & `RaspyGeo-0.0.4/src/RaspyGeo/testing.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo/write_geo.py` & `RaspyGeo-0.0.4/src/RaspyGeo/write_geo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.3/src/RaspyGeo.egg-info/PKG-INFO` & `RaspyGeo-0.0.4/src/RaspyGeo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: RaspyGeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS
 Home-page: https://github.com/quantum-dan/RaspyGeo
 Author: Daniel Philippus
 Author-email: daniel@dphilippus.com
 Project-URL: Bug Tracker, https://github.com/quantum-dan/RaspyGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RaspyGeo
-Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS.  Depends on Raspy (`raspy-auto` on PyPI).  Works for steady-state simulations.
+
+Automated geometry scenario runner (loosely analogous to the Geometry Modification tool) for HEC-RAS.  Depends on Raspy (`raspy-auto` on PyPI).  Currently works for steady-state simulations. RaspyGeo is available on PyPI as [RaspyGeo](https://pypi.org/project/RaspyGeo/).
+
+# Updates and Added Features
+
+If additional capabilities would be useful to you, open an Issue and I will check
+into it.  Otherwise, I develop updates as I need them.
 
 # Usage
 
 Scenario running is fully automated through `run`.  The HEC-RAS project must
 already be set up with a reference (baseline) geometry **and** a new (scenario)
 geometry file, and the current plan must be set up to run the scenario geometry.
 Then, the user specifies:
```

