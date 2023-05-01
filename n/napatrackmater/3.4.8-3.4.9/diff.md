# Comparing `tmp/napatrackmater-3.4.8.tar.gz` & `tmp/napatrackmater-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-rg_i21_c/napatrackmater-3.4.8.tar", last modified: Mon May  1 18:40:56 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-36fl4xtz/napatrackmater-3.4.9.tar", last modified: Mon May  1 19:09:13 2023, max compression
```

## Comparing `napatrackmater-3.4.8.tar` & `napatrackmater-3.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 18:40:56.895221 napatrackmater-3.4.8/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 18:40:56.890952 napatrackmater-3.4.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.8/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 18:40:56.638600 napatrackmater-3.4.8/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.8/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.8/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   108842 2023-05-01 18:40:17.000000 napatrackmater-3.4.8/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.8/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.8/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.8/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.8/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.8/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.8/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-01 18:38:28.000000 napatrackmater-3.4.8/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 18:40:56.854984 napatrackmater-3.4.8/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 18:40:55.000000 napatrackmater-3.4.8/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-01 18:40:56.000000 napatrackmater-3.4.8/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-01 18:40:55.000000 napatrackmater-3.4.8/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-01 18:40:55.000000 napatrackmater-3.4.8/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-01 18:40:55.000000 napatrackmater-3.4.8/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-01 18:40:55.000000 napatrackmater-3.4.8/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-01 18:40:56.897253 napatrackmater-3.4.8/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.8/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 19:09:13.626053 napatrackmater-3.4.9/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.9/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 19:09:13.620948 napatrackmater-3.4.9/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.9/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 19:09:13.409791 napatrackmater-3.4.9/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.9/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.9/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   108833 2023-05-01 19:08:21.000000 napatrackmater-3.4.9/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.9/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.9/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.9/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.9/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.9/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.9/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-01 19:08:30.000000 napatrackmater-3.4.9/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 19:09:13.589153 napatrackmater-3.4.9/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 19:09:12.000000 napatrackmater-3.4.9/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-01 19:09:13.000000 napatrackmater-3.4.9/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-01 19:09:12.000000 napatrackmater-3.4.9/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-01 19:09:12.000000 napatrackmater-3.4.9/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-01 19:09:12.000000 napatrackmater-3.4.9/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-01 19:09:12.000000 napatrackmater-3.4.9/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-01 19:09:13.627358 napatrackmater-3.4.9/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.9/setup.py
```

### Comparing `napatrackmater-3.4.8/LICENSE` & `napatrackmater-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/PKG-INFO` & `napatrackmater-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.4.8
+Version: 3.4.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.4.8/README.md` & `napatrackmater-3.4.9/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.4.9/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.4.9/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/Trackmate.py` & `napatrackmater-3.4.9/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -5087,1717 +5087,1717 @@
 00013de0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
 00013df0: 645f 785f 6b65 793a 2066 6c6f 6174 286d  d_x_key: float(m
 00013e00: 6173 6b63 656e 7472 6f69 645b 325d 2920  askcentroid[2]) 
 00013e10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00013e20: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
 00013e30: 2020 2065 6c69 6620 6365 6c6c 5f69 6420     elif cell_id 
 00013e40: 696e 2073 656c 662e 6564 6765 5f73 6f75  in self.edge_sou
-00013e50: 7263 655f 6c6f 6f6b 7570 5b63 656c 6c5f  rce_lookup[cell_
-00013e60: 6964 5d2e 6b65 7973 2829 3a0d 0a20 2020  id].keys():..   
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013e90: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00013ea0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-00013eb0: 705b 6365 6c6c 5f69 645d 2069 6e20 7365  p[cell_id] in se
-00013ec0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-00013ed0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00013ee0: 732e 6b65 7973 2829 2069 7320 6e6f 7420  s.keys() is not 
-00013ef0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00013f00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013f10: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-00013f20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00013f30: 735b 6365 6c6c 5f69 645d 203d 2073 656c  s[cell_id] = sel
-00013f40: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-00013f50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00013f60: 5b73 656c 662e 6564 6765 5f73 6f75 7263  [self.edge_sourc
-00013f70: 655f 6c6f 6f6b 7570 5b63 656c 6c5f 6964  e_lookup[cell_id
-00013f80: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
-00013f90: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fb0: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-00013fc0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-00013fd0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00013fe0: 645d 203d 2073 656c 662e 756e 6971 7565  d] = self.unique
-00013ff0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014000: 5b63 656c 6c5f 6964 5d20 2020 2020 0d0a  [cell_id]     ..
+00013e50: 7263 655f 6c6f 6f6b 7570 2e6b 6579 7328  rce_lookup.keys(
+00013e60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00013e70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00013e80: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013e90: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
+00013ea0: 655f 6c6f 6f6b 7570 5b63 656c 6c5f 6964  e_lookup[cell_id
+00013eb0: 5d20 696e 2073 656c 662e 6368 616e 6e65  ] in self.channe
+00013ec0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+00013ed0: 6f70 6572 7469 6573 2e6b 6579 7328 2920  operties.keys() 
+00013ee0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f00: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+00013f10: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+00013f20: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00013f30: 5d20 3d20 7365 6c66 2e63 6861 6e6e 656c  ] = self.channel
+00013f40: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00013f50: 7065 7274 6965 735b 7365 6c66 2e65 6467  perties[self.edg
+00013f60: 655f 736f 7572 6365 5f6c 6f6f 6b75 705b  e_source_lookup[
+00013f70: 6365 6c6c 5f69 645d 5d0d 0a20 2020 2020  cell_id]]..     
+00013f80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00013f90: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00013fa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013fb0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00013fc0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00013fd0: 5b63 656c 6c5f 6964 5d20 3d20 7365 6c66  [cell_id] = self
+00013fe0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00013ff0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00014000: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014020: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00014030: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00014040: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00014050: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00014060: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-00014070: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-00014080: 5f69 645d 203d 2073 656c 662e 756e 6971  _id] = self.uniq
-00014090: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000140a0: 6573 5b63 656c 6c5f 6964 5d0d 0a0d 0a0d  es[cell_id].....
-000140b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140d0: 2020 0d0a 2020 2020 6465 6620 5f64 6963    ..    def _dic
-000140e0: 745f 7570 6461 7465 2873 656c 662c 2075  t_update(self, u
-000140f0: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-00014100: 6473 3a20 4c69 7374 2c20 2063 656c 6c5f  ds: List,  cell_
-00014110: 6964 3a20 696e 742c 2074 7261 636b 5f69  id: int, track_i
-00014120: 643a 2069 6e74 2c20 736f 7572 6365 5f69  d: int, source_i
-00014130: 643a 2069 6e74 2c20 7461 7267 6574 5f69  d: int, target_i
-00014140: 643a 2069 6e74 293a 0d0a 0d0a 200d 0a20  d: int):.... .. 
-00014150: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
-00014160: 6e5f 6964 203d 2073 656c 662e 6765 6e65  n_id = self.gene
-00014170: 7261 7469 6f6e 5f64 6963 745b 6365 6c6c  ration_dict[cell
-00014180: 5f69 645d 0d0a 2020 2020 2020 2020 7472  _id]..        tr
-00014190: 6163 6b6c 6574 5f69 6420 3d20 7365 6c66  acklet_id = self
-000141a0: 2e74 7261 636b 6c65 745f 6469 6374 5b63  .tracklet_dict[c
-000141b0: 656c 6c5f 6964 5d0d 0a0d 0a20 2020 2020  ell_id]....     
-000141c0: 2020 2075 6e69 7175 655f 6964 203d 2073     unique_id = s
-000141d0: 7472 2874 7261 636b 5f69 6429 202b 2073  tr(track_id) + s
-000141e0: 7472 2873 656c 662e 6d61 785f 7472 6163  tr(self.max_trac
-000141f0: 6b5f 6964 2920 2b20 7374 7228 6765 6e65  k_id) + str(gene
-00014200: 7261 7469 6f6e 5f69 6429 202b 2073 7472  ration_id) + str
-00014210: 2874 7261 636b 6c65 745f 6964 290d 0a20  (tracklet_id).. 
-00014220: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00014230: 2076 6563 5f6d 6173 6b20 3d20 5b66 6c6f   vec_mask = [flo
-00014240: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014250: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014260: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014270: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
-00014280: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
-00014290: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000142a0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-000142b0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-000142c0: 6b63 656e 7472 6f69 645f 795f 6b65 795d  kcentroid_y_key]
-000142d0: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
-000142e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000142f0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014300: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-00014310: 726f 6964 5f7a 5f6b 6579 5d29 205d 0d0a  roid_z_key]) ]..
-00014320: 0d0a 2020 2020 2020 2020 7665 635f 6365  ..        vec_ce
-00014330: 6c6c 203d 205b 666c 6f61 7428 7365 6c66  ll = [float(self
-00014340: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014350: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014360: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-00014370: 645f 6b65 795d 2920 2c20 0d0a 2020 2020  d_key]) , ..    
-00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014390: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-000143a0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000143b0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-000143c0: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-000143d0: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+00014020: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00014030: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00014040: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014050: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+00014060: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014070: 6573 5b63 656c 6c5f 6964 5d20 3d20 7365  es[cell_id] = se
+00014080: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014090: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+000140a0: 645d 0d0a 0d0a 0d0a 2020 2020 2020 2020  d]......        
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+000140d0: 6566 205f 6469 6374 5f75 7064 6174 6528  ef _dict_update(
+000140e0: 7365 6c66 2c20 756e 6971 7565 5f74 7261  self, unique_tra
+000140f0: 636b 6c65 745f 6964 733a 204c 6973 742c  cklet_ids: List,
+00014100: 2020 6365 6c6c 5f69 643a 2069 6e74 2c20    cell_id: int, 
+00014110: 7472 6163 6b5f 6964 3a20 696e 742c 2073  track_id: int, s
+00014120: 6f75 7263 655f 6964 3a20 696e 742c 2074  ource_id: int, t
+00014130: 6172 6765 745f 6964 3a20 696e 7429 3a0d  arget_id: int):.
+00014140: 0a0d 0a20 0d0a 2020 2020 2020 2020 6765  ... ..        ge
+00014150: 6e65 7261 7469 6f6e 5f69 6420 3d20 7365  neration_id = se
+00014160: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00014170: 6374 5b63 656c 6c5f 6964 5d0d 0a20 2020  ct[cell_id]..   
+00014180: 2020 2020 2074 7261 636b 6c65 745f 6964       tracklet_id
+00014190: 203d 2073 656c 662e 7472 6163 6b6c 6574   = self.tracklet
+000141a0: 5f64 6963 745b 6365 6c6c 5f69 645d 0d0a  _dict[cell_id]..
+000141b0: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
+000141c0: 5f69 6420 3d20 7374 7228 7472 6163 6b5f  _id = str(track_
+000141d0: 6964 2920 2b20 7374 7228 7365 6c66 2e6d  id) + str(self.m
+000141e0: 6178 5f74 7261 636b 5f69 6429 202b 2073  ax_track_id) + s
+000141f0: 7472 2867 656e 6572 6174 696f 6e5f 6964  tr(generation_id
+00014200: 2920 2b20 7374 7228 7472 6163 6b6c 6574  ) + str(tracklet
+00014210: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
+00014220: 2020 2020 2020 2020 7665 635f 6d61 736b          vec_mask
+00014230: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+00014240: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014250: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014260: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00014270: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+00014280: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00014290: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000142a0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+000142b0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+000142c0: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+000142d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000142e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000142f0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00014300: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+00014310: 795d 2920 5d0d 0a0d 0a20 2020 2020 2020  y]) ]....       
+00014320: 2076 6563 5f63 656c 6c20 3d20 5b66 6c6f   vec_cell = [flo
+00014330: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014340: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014350: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00014360: 662e 7870 6f73 6964 5f6b 6579 5d29 202c  f.xposid_key]) ,
+00014370: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00014380: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014390: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000143a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000143b0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+000143c0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+000143d0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
 000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143f0: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00014400: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014410: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014420: 656c 6c5f 6964 295d 5b73 656c 662e 7a70  ell_id)][self.zp
-00014430: 6f73 6964 5f6b 6579 5d29 5d0d 0a0d 0a20  osid_key])].... 
-00014440: 2020 2020 2020 2061 6e67 6c65 203d 2061         angle = a
-00014450: 6e67 756c 6172 5f63 6861 6e67 6528 7665  ngular_change(ve
-00014460: 635f 6d61 736b 2c20 7665 635f 6365 6c6c  c_mask, vec_cell
-00014470: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
-00014480: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014490: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000144a0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000144b0: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
-000144c0: 5f6b 6579 203a 2061 6e67 6c65 7d29 2020  _key : angle})  
-000144d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144e0: 2020 0d0a 0d0a 2020 2020 2020 2020 756e    ....        un
-000144f0: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
-00014500: 732e 6170 7065 6e64 2873 7472 2875 6e69  s.append(str(uni
-00014510: 7175 655f 6964 2929 0d0a 2020 2020 2020  que_id))..      
-00014520: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014530: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014540: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014550: 7465 287b 7365 6c66 2e63 6c75 7374 6572  te({self.cluster
-00014560: 636c 6173 735f 6b65 7920 3a20 4e6f 6e65  class_key : None
-00014570: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00014580: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014590: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000145a0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-000145b0: 6c66 2e63 6c75 7374 6572 7363 6f72 655f  lf.clusterscore_
-000145c0: 6b65 7920 3a20 307d 290d 0a20 2020 2020  key : 0})..     
-000145d0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000145e0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000145f0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00014600: 6174 6528 7b73 656c 662e 756e 6971 7565  ate({self.unique
-00014610: 6964 5f6b 6579 203a 2073 7472 2875 6e69  id_key : str(uni
-00014620: 7175 655f 6964 297d 290d 0a20 2020 2020  que_id)})..     
-00014630: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00014640: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014650: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00014660: 6174 6528 7b73 656c 662e 7472 6163 6b6c  ate({self.trackl
-00014670: 6574 6964 5f6b 6579 203a 2073 7472 2874  etid_key : str(t
-00014680: 7261 636b 6c65 745f 6964 297d 2920 0d0a  racklet_id)}) ..
-00014690: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000146a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000146b0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000146c0: 5d2e 7570 6461 7465 287b 7365 6c66 2e67  ].update({self.g
-000146d0: 656e 6572 6174 696f 6e69 645f 6b65 7920  enerationid_key 
-000146e0: 3a20 7374 7228 6765 6e65 7261 7469 6f6e  : str(generation
-000146f0: 5f69 6429 7d29 200d 0a20 2020 2020 2020  _id)}) ..       
-00014700: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014710: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014720: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014730: 6528 7b73 656c 662e 7472 6163 6b69 645f  e({self.trackid_
-00014740: 6b65 7920 3a20 7374 7228 7472 6163 6b5f  key : str(track_
-00014750: 6964 297d 290d 0a20 2020 2020 2020 2073  id)})..        s
-00014760: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014770: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014780: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014790: 7b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  {self.motion_ang
-000147a0: 6c65 5f6b 6579 203a 2030 2e30 7d29 0d0a  le_key : 0.0})..
-000147b0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000147c0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000147d0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000147e0: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
-000147f0: 7065 6564 5f6b 6579 203a 2030 2e30 7d29  peed_key : 0.0})
-00014800: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00014810: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014820: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014830: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014840: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00014850: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
-00014860: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00014870: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014880: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00014890: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-000148a0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000148b0: 746b 6579 203a 204e 6f6e 657d 290d 0a20  tkey : None}).. 
-000148c0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000148d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000148e0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-000148f0: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
-00014900: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00014910: 7365 636f 6e64 6b65 7920 3a20 4e6f 6e65  secondkey : None
-00014920: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00014930: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014940: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014950: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014960: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-00014970: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
-00014980: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00014990: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000149a0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000149b0: 7570 6461 7465 287b 7365 6c66 2e63 656c  update({self.cel
-000149c0: 6c61 7869 735f 6d61 736b 5f6b 6579 203a  laxis_mask_key :
-000149d0: 204e 6f6e 657d 290d 0a0d 0a20 2020 2020   None})....     
-000149e0: 2020 2069 6620 736f 7572 6365 5f69 6420     if source_id 
-000149f0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00014a00: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00014a10: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014a20: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014a30: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00014a40: 2e62 6566 6f72 6569 645f 6b65 7920 3a20  .beforeid_key : 
-00014a50: 696e 7428 736f 7572 6365 5f69 6429 7d29  int(source_id)})
-00014a60: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
-00014a70: 635f 3120 3d20 5b66 6c6f 6174 2873 656c  c_1 = [float(sel
-00014a80: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014a90: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014aa0: 6c5f 6964 295d 5b73 656c 662e 7870 6f73  l_id)][self.xpos
-00014ab0: 6964 5f6b 6579 5d29 202d 2066 6c6f 6174  id_key]) - float
-00014ac0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00014ad0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014ae0: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-00014af0: 662e 7870 6f73 6964 5f6b 6579 5d29 2c20  f.xposid_key]), 
-00014b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014b10: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-00014b20: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00014b30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014b40: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00014b50: 6c66 2e79 706f 7369 645f 6b65 795d 2920  lf.yposid_key]) 
-00014b60: 2d20 666c 6f61 7428 7365 6c66 2e75 6e69  - float(self.uni
-00014b70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014b80: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-00014b90: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-00014ba0: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
-00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bc0: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
-00014bd0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014be0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014bf0: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00014c00: 5f6b 6579 5d29 202d 2020 666c 6f61 7428  _key]) -  float(
-00014c10: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014c20: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014c30: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00014c40: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
-00014c50: 2020 2020 2020 2020 2020 2020 7370 6565              spee
-00014c60: 6420 3d20 6e70 2e73 7172 7428 6e70 2e64  d = np.sqrt(np.d
-00014c70: 6f74 2876 6563 5f31 2c20 7665 635f 3129  ot(vec_1, vec_1)
-00014c80: 292f 7365 6c66 2e74 6361 6c69 6272 6174  )/self.tcalibrat
-00014c90: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00014ca0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00014cb0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00014cc0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00014cd0: 6528 7b73 656c 662e 7370 6565 645f 6b65  e({self.speed_ke
-00014ce0: 7920 3a20 7370 6565 647d 290d 0a0d 0a20  y : speed}).... 
-00014cf0: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
-00014d00: 6e5f 616e 676c 6520 3d20 616e 6775 6c61  n_angle = angula
-00014d10: 725f 6368 616e 6765 2876 6563 5f6d 6173  r_change(vec_mas
-00014d20: 6b2c 2076 6563 5f31 290d 0a0d 0a20 2020  k, vec_1)....   
-00014d30: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00014d40: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014d50: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014d60: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014d70: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-00014d80: 203a 206d 6f74 696f 6e5f 616e 676c 657d   : motion_angle}
-00014d90: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-00014da0: 2020 6966 2073 6f75 7263 655f 6964 2069    if source_id i
-00014db0: 6e20 7365 6c66 2e65 6467 655f 736f 7572  n self.edge_sour
-00014dc0: 6365 5f6c 6f6f 6b75 703a 0d0a 2020 2020  ce_lookup:..    
-00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014de0: 7072 655f 736f 7572 6365 5f69 6420 3d20  pre_source_id = 
-00014df0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
-00014e00: 5f6c 6f6f 6b75 705b 736f 7572 6365 5f69  _lookup[source_i
-00014e10: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00014e20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00014e30: 2020 2020 2020 2020 2020 2020 2020 7665                ve
-00014e40: 635f 3220 3d20 5b66 6c6f 6174 2873 656c  c_2 = [float(sel
-00014e50: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014e60: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014e70: 6c5f 6964 295d 5b73 656c 662e 7870 6f73  l_id)][self.xpos
-00014e80: 6964 5f6b 6579 5d29 202d 2032 202a 2066  id_key]) - 2 * f
-00014e90: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00014ea0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014eb0: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
-00014ec0: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00014ed0: 5d29 202b 2066 6c6f 6174 2873 656c 662e  ]) + float(self.
-00014ee0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014ef0: 6572 7469 6573 5b69 6e74 2870 7265 5f73  erties[int(pre_s
-00014f00: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-00014f10: 7870 6f73 6964 5f6b 6579 5d29 2c20 0d0a  xposid_key]), ..
+000143f0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014400: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014410: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014420: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00014430: 295d 0d0a 0d0a 2020 2020 2020 2020 616e  )]....        an
+00014440: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+00014450: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+00014460: 6563 5f63 656c 6c29 0d0a 0d0a 2020 2020  ec_cell)....    
+00014470: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014480: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014490: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000144a0: 6461 7465 287b 7365 6c66 2e72 6164 6961  date({self.radia
+000144b0: 6c5f 616e 676c 655f 6b65 7920 3a20 616e  l_angle_key : an
+000144c0: 676c 657d 2920 2020 2020 2020 2020 2020  gle})           
+000144d0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+000144e0: 2020 2020 2075 6e69 7175 655f 7472 6163       unique_trac
+000144f0: 6b6c 6574 5f69 6473 2e61 7070 656e 6428  klet_ids.append(
+00014500: 7374 7228 756e 6971 7565 5f69 6429 290d  str(unique_id)).
+00014510: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00014520: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014530: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014540: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00014550: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00014560: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+00014570: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014580: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014590: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000145a0: 6174 6528 7b73 656c 662e 636c 7573 7465  ate({self.cluste
+000145b0: 7273 636f 7265 5f6b 6579 203a 2030 7d29  rscore_key : 0})
+000145c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+000145d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000145e0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000145f0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014600: 2e75 6e69 7175 6569 645f 6b65 7920 3a20  .uniqueid_key : 
+00014610: 7374 7228 756e 6971 7565 5f69 6429 7d29  str(unique_id)})
+00014620: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014630: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014640: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014650: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014660: 2e74 7261 636b 6c65 7469 645f 6b65 7920  .trackletid_key 
+00014670: 3a20 7374 7228 7472 6163 6b6c 6574 5f69  : str(tracklet_i
+00014680: 6429 7d29 200d 0a20 2020 2020 2020 2073  d)}) ..        s
+00014690: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000146a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000146b0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000146c0: 7b73 656c 662e 6765 6e65 7261 7469 6f6e  {self.generation
+000146d0: 6964 5f6b 6579 203a 2073 7472 2867 656e  id_key : str(gen
+000146e0: 6572 6174 696f 6e5f 6964 297d 2920 0d0a  eration_id)}) ..
+000146f0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014700: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014710: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014720: 5d2e 7570 6461 7465 287b 7365 6c66 2e74  ].update({self.t
+00014730: 7261 636b 6964 5f6b 6579 203a 2073 7472  rackid_key : str
+00014740: 2874 7261 636b 5f69 6429 7d29 0d0a 2020  (track_id)})..  
+00014750: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014760: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014770: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00014780: 7570 6461 7465 287b 7365 6c66 2e6d 6f74  update({self.mot
+00014790: 696f 6e5f 616e 676c 655f 6b65 7920 3a20  ion_angle_key : 
+000147a0: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
+000147b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000147c0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000147d0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000147e0: 7b73 656c 662e 7370 6565 645f 6b65 7920  {self.speed_key 
+000147f0: 3a20 302e 307d 290d 0a20 2020 2020 2020  : 0.0})..       
+00014800: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014810: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014820: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014830: 6528 7b73 656c 662e 6163 6365 6c65 7261  e({self.accelera
+00014840: 7469 6f6e 5f6b 6579 203a 2030 2e30 7d29  tion_key : 0.0})
+00014850: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014860: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014870: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014880: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014890: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+000148a0: 6d70 5f66 6972 7374 6b65 7920 3a20 4e6f  mp_firstkey : No
+000148b0: 6e65 7d29 0d0a 2020 2020 2020 2020 7365  ne})..        se
+000148c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000148d0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000148e0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000148f0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+00014900: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
+00014910: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+00014920: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014930: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014940: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00014950: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
+00014960: 655f 6172 6561 5f6b 6579 203a 204e 6f6e  e_area_key : Non
+00014970: 657d 290d 0a20 2020 2020 2020 2073 656c  e})..        sel
+00014980: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014990: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+000149a0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+000149b0: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
+000149c0: 6b5f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  k_key : None})..
+000149d0: 0d0a 2020 2020 2020 2020 6966 2073 6f75  ..        if sou
+000149e0: 7263 655f 6964 2069 7320 6e6f 7420 4e6f  rce_id is not No
+000149f0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00014a00: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014a10: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014a20: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014a30: 6528 7b73 656c 662e 6265 666f 7265 6964  e({self.beforeid
+00014a40: 5f6b 6579 203a 2069 6e74 2873 6f75 7263  _key : int(sourc
+00014a50: 655f 6964 297d 290d 0a20 2020 2020 2020  e_id)})..       
+00014a60: 2020 2020 2076 6563 5f31 203d 205b 666c       vec_1 = [fl
+00014a70: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014a80: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014a90: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014aa0: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00014ab0: 2d20 666c 6f61 7428 7365 6c66 2e75 6e69  - float(self.uni
+00014ac0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014ad0: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+00014ae0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00014af0: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00014b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b10: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00014b20: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014b30: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014b40: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+00014b50: 5f6b 6579 5d29 202d 2066 6c6f 6174 2873  _key]) - float(s
+00014b60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014b70: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+00014b80: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+00014b90: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bb0: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00014bc0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014bd0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014be0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014bf0: 2e7a 706f 7369 645f 6b65 795d 2920 2d20  .zposid_key]) - 
+00014c00: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014c10: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014c20: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00014c30: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00014c40: 6579 5d29 5d0d 0a20 2020 2020 2020 2020  ey])]..         
+00014c50: 2020 2073 7065 6564 203d 206e 702e 7371     speed = np.sq
+00014c60: 7274 286e 702e 646f 7428 7665 635f 312c  rt(np.dot(vec_1,
+00014c70: 2076 6563 5f31 2929 2f73 656c 662e 7463   vec_1))/self.tc
+00014c80: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00014c90: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014ca0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014cb0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014cc0: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
+00014cd0: 7065 6564 5f6b 6579 203a 2073 7065 6564  peed_key : speed
+00014ce0: 7d29 0d0a 0d0a 2020 2020 2020 2020 2020  })....          
+00014cf0: 2020 6d6f 7469 6f6e 5f61 6e67 6c65 203d    motion_angle =
+00014d00: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+00014d10: 7665 635f 6d61 736b 2c20 7665 635f 3129  vec_mask, vec_1)
+00014d20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014d30: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014d40: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014d50: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014d60: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
+00014d70: 676c 655f 6b65 7920 3a20 6d6f 7469 6f6e  gle_key : motion
+00014d80: 5f61 6e67 6c65 7d29 200d 0a0d 0a20 2020  _angle}) ....   
+00014d90: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00014da0: 6365 5f69 6420 696e 2073 656c 662e 6564  ce_id in self.ed
+00014db0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
+00014dc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00014dd0: 2020 2020 2020 2070 7265 5f73 6f75 7263         pre_sourc
+00014de0: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
+00014df0: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
+00014e00: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00014e10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00014e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e30: 2020 2020 2076 6563 5f32 203d 205b 666c       vec_2 = [fl
+00014e40: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00014e50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014e60: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00014e70: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00014e80: 2d20 3220 2a20 666c 6f61 7428 7365 6c66  - 2 * float(self
+00014e90: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014ea0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00014eb0: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
+00014ec0: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
+00014ed0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014ee0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014ef0: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
+00014f00: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00014f10: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
 00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f30: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00014f40: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00014f50: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014f60: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00014f70: 2e79 706f 7369 645f 6b65 795d 2920 2d20  .yposid_key]) - 
-00014f80: 3220 2a20 666c 6f61 7428 7365 6c66 2e75  2 * float(self.u
-00014f90: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014fa0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-00014fb0: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-00014fc0: 645f 6b65 795d 2920 2b20 666c 6f61 7428  d_key]) + float(
-00014fd0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014fe0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014ff0: 7072 655f 736f 7572 6365 5f69 6429 5d5b  pre_source_id)][
-00015000: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00015010: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015030: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00015040: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015050: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015060: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-00015070: 5d29 202d 2020 3220 2a20 666c 6f61 7428  ]) -  2 * float(
-00015080: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015090: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000150a0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-000150b0: 2e7a 706f 7369 645f 6b65 795d 2920 2b20  .zposid_key]) + 
-000150c0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000150d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000150e0: 735b 696e 7428 7072 655f 736f 7572 6365  s[int(pre_source
-000150f0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-00015100: 645f 6b65 795d 295d 0d0a 2020 2020 2020  d_key])]..      
-00015110: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00015120: 6320 3d20 6e70 2e73 7172 7428 6e70 2e64  c = np.sqrt(np.d
-00015130: 6f74 2876 6563 5f32 2c20 7665 635f 3229  ot(vec_2, vec_2)
-00015140: 292f 7365 6c66 2e74 6361 6c69 6272 6174  )/self.tcalibrat
-00015150: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00015160: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00015170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015180: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015190: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000151a0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-000151b0: 7b73 656c 662e 6163 6365 6c65 7261 7469  {self.accelerati
-000151c0: 6f6e 5f6b 6579 203a 2061 6363 7d29 0d0a  on_key : acc})..
-000151d0: 2020 2020 2020 2020 656c 6966 2073 6f75          elif sou
-000151e0: 7263 655f 6964 2069 7320 4e6f 6e65 3a0d  rce_id is None:.
-000151f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015200: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015210: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015220: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015230: 656c 662e 6265 666f 7265 6964 5f6b 6579  elf.beforeid_key
-00015240: 203a 204e 6f6e 657d 2920 0d0a 2020 2020   : None}) ..    
-00015250: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00015260: 2020 2020 6966 2074 6172 6765 745f 6964      if target_id
-00015270: 2069 7320 6e6f 7420 4e6f 6e65 3a20 2020   is not None:   
-00015280: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00015290: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-000152a0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000152b0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-000152c0: 7465 287b 7365 6c66 2e61 6674 6572 6964  te({self.afterid
-000152d0: 5f6b 6579 203a 2069 6e74 2874 6172 6765  _key : int(targe
-000152e0: 745f 6964 297d 2920 0d0a 2020 2020 2020  t_id)}) ..      
-000152f0: 2020 656c 6966 2074 6172 6765 745f 6964    elif target_id
-00015300: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00015310: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00015320: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015330: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015340: 2e75 7064 6174 6528 7b73 656c 662e 6166  .update({self.af
-00015350: 7465 7269 645f 6b65 7920 3a20 4e6f 6e65  terid_key : None
-00015360: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00015370: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00015380: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
-00015390: 7064 6174 6528 6365 6c6c 5f69 642c 2074  pdate(cell_id, t
-000153a0: 7261 636b 5f69 6429 2020 2020 0d0a 0d0a  rack_id)    ....
-000153b0: 0d0a 2020 2020 6465 6620 5f74 656d 706f  ..    def _tempo
-000153c0: 7261 6c5f 706c 6f74 735f 7472 6163 6b6d  ral_plots_trackm
-000153d0: 6174 6528 7365 6c66 293a 0d0a 2020 2020  ate(self):..    
-000153e0: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
-000153f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015400: 6c66 2e41 7474 7220 3d20 7b7d 0d0a 2020  lf.Attr = {}..  
-00015410: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00015420: 6172 7474 696d 6520 3d20 696e 7428 6d69  arttime = int(mi
-00015430: 6e28 7365 6c66 2e41 6c6c 5661 6c75 6573  n(self.AllValues
-00015440: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
-00015450: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
-00015460: 2020 2020 2020 656e 6474 696d 6520 3d20        endtime = 
-00015470: 696e 7428 6d61 7828 7365 6c66 2e41 6c6c  int(max(self.All
-00015480: 5661 6c75 6573 5b73 656c 662e 6672 616d  Values[self.fram
-00015490: 6569 645f 6b65 795d 2929 0d0a 2020 2020  eid_key]))..    
-000154a0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000154c0: 656c 662e 7469 6d65 203d 205b 5d0d 0a20  elf.time = [].. 
-000154d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000154e0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-000154f0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00015500: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015510: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00015520: 6973 705f 7a20 3d20 5b5d 0d0a 0d0a 2020  isp_z = []....  
-00015530: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015540: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015550: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
-00015560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015570: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00015580: 7370 5f79 203d 205b 5d0d 0a0d 0a20 2020  sp_y = []....   
-00015590: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000155a0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-000155b0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-000155c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000155d0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-000155e0: 705f 7820 3d20 5b5d 0d0a 0d0a 2020 2020  p_x = []....    
-000155f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015600: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7261  .mitotic_mean_ra
-00015610: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-00015620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015630: 6d69 746f 7469 635f 7661 725f 7261 6469  mitotic_var_radi
-00015640: 7573 203d 205b 5d0d 0a0d 0a20 2020 2020  us = []....     
-00015650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015660: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
-00015670: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-00015680: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015690: 746f 7469 635f 7661 725f 7370 6565 6420  totic_var_speed 
-000156a0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-000156b0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000156c0: 6f74 6963 5f6d 6561 6e5f 6163 6320 3d20  otic_mean_acc = 
-000156d0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000156e0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000156f0: 5f76 6172 5f61 6363 203d 205b 5d0d 0a0d  _var_acc = []...
-00015700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015710: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00015720: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00015730: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
-00015740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015750: 2e6d 6974 6f74 6963 5f76 6172 5f64 6972  .mitotic_var_dir
-00015760: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00015770: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00015780: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015790: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
-000157a0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-000157b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000157c0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-000157d0: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
-000157e0: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a20  l_mask = [].... 
-000157f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015800: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00015810: 6d65 616e 5f64 6973 705f 7a20 3d20 5b5d  mean_disp_z = []
-00015820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015830: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00015840: 6963 5f76 6172 5f64 6973 705f 7a20 3d20  ic_var_disp_z = 
-00015850: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015860: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015870: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00015880: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00015890: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000158a0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-000158b0: 7370 5f79 203d 205b 5d0d 0a0d 0a20 2020  sp_y = []....   
-000158c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000158d0: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-000158e0: 616e 5f64 6973 705f 7820 3d20 5b5d 0d0a  an_disp_x = []..
-000158f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015900: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015910: 5f76 6172 5f64 6973 705f 7820 3d20 5b5d  _var_disp_x = []
-00015920: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015930: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00015940: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
-00015950: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015960: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015970: 6d69 746f 7469 635f 7661 725f 7261 6469  mitotic_var_radi
-00015980: 7573 203d 205b 5d0d 0a0d 0a20 2020 2020  us = []....     
-00015990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000159a0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-000159b0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-000159c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000159d0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-000159e0: 725f 7370 6565 6420 3d20 5b5d 0d0a 0d0a  r_speed = []....
-000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a00: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015a10: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
-00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a30: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015a40: 5f76 6172 5f61 6363 203d 205b 5d0d 0a0d  _var_acc = []...
-00015a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a60: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015a70: 635f 6d65 616e 5f64 6972 6563 7469 6f6e  c_mean_direction
-00015a80: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015aa0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015ab0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-00015ac0: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 0d0a  _change = []....
-00015ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ae0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015af0: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
-00015b00: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
-00015b10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015b20: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00015b30: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
-00015b40: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a20  l_mask = [].... 
-00015b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015b60: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
-00015b70: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00015b80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00015b90: 6c6c 5f76 6172 5f64 6973 705f 7a20 3d20  ll_var_disp_z = 
-00015ba0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015bb0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00015bc0: 6561 6e5f 6469 7370 5f79 203d 205b 5d0d  ean_disp_y = [].
-00015bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015be0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00015bf0: 7370 5f79 203d 205b 5d0d 0a0d 0a20 2020  sp_y = []....   
-00015c00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015c10: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-00015c20: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00015c30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015c40: 5f76 6172 5f64 6973 705f 7820 3d20 5b5d  _var_disp_x = []
-00015c50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015c60: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00015c70: 6e5f 7261 6469 7573 203d 205b 5d0d 0a20  n_radius = [].. 
-00015c80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015c90: 656c 662e 616c 6c5f 7661 725f 7261 6469  elf.all_var_radi
-00015ca0: 7573 203d 205b 5d0d 0a0d 0a20 2020 2020  us = []....     
-00015cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015cc0: 616c 6c5f 6d65 616e 5f73 7065 6564 203d  all_mean_speed =
-00015cd0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015ce0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00015cf0: 725f 7370 6565 6420 3d20 5b5d 0d0a 0d0a  r_speed = []....
-00015d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d10: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6163  self.all_mean_ac
-00015d20: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
-00015d30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015d40: 5f76 6172 5f61 6363 203d 205b 5d0d 0a0d  _var_acc = []...
-00015d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015d60: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00015d70: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00015d80: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00015d90: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00015da0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-00015db0: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 0d0a  _change = []....
-00015dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015dd0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00015de0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00015df0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015e00: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00015e10: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
-00015e20: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a20  l_mask = [].... 
-00015e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015e40: 656c 662e 6d69 746f 7469 635f 636c 7573  elf.mitotic_clus
-00015e50: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
-00015e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e70: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00015e80: 5f63 6c75 7374 6572 5f63 6c61 7373 203d  _cluster_class =
-00015e90: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015ea0: 2020 2020 2073 656c 662e 616c 6c5f 636c       self.all_cl
-00015eb0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
-00015ec0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015ed0: 2020 2020 616c 6c5f 7370 6f74 735f 7472      all_spots_tr
-00015ee0: 6163 6b73 203d 207b 7d0d 0a20 2020 2020  acks = {}..     
-00015ef0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-00015f00: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-00015f10: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015f20: 6965 732e 6974 656d 7328 293a 0d0a 2020  ies.items():..  
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00015f50: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00015f60: 7370 6f74 7320 3d20 7365 6c66 2e75 6e69  spots = self.uni
-00015f70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015f80: 6965 735b 6b5d 0d0a 2020 2020 2020 2020  ies[k]..        
-00015f90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00015fa0: 2073 656c 662e 7472 6163 6b69 645f 6b65   self.trackid_ke
-00015fb0: 7920 696e 2061 6c6c 5f73 706f 7473 3a0d  y in all_spots:.
-00015fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015fd0: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
-00015fe0: 706f 7473 5f74 7261 636b 735b 6b5d 203d  pots_tracks[k] =
-00015ff0: 2061 6c6c 5f73 706f 7473 0d0a 2020 2020   all_spots..    
-00016000: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00016010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016030: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
-00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016050: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-00016060: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-00016070: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-00016080: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-00016090: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-000160a0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-000160b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160d0: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
-000160e0: 2872 616e 6765 2873 7461 7274 7469 6d65  (range(starttime
-000160f0: 2c20 656e 6474 696d 6529 2c20 746f 7461  , endtime), tota
-00016100: 6c3d 656e 6474 696d 6520 2d20 7374 6172  l=endtime - star
-00016110: 7474 696d 6529 3a0d 0a20 2020 2020 2020  ttime):..       
-00016120: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00016130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016140: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-00016150: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
-00016160: 2e73 7562 6d69 7428 7365 6c66 2e5f 636f  .submit(self._co
-00016170: 6d70 7574 655f 7465 6d70 6f72 616c 2c20  mpute_temporal, 
-00016180: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
-00016190: 636b 7329 290d 0a20 0d0a 2020 2020 2020  cks)).. ..      
-000161a0: 2020 2020 2020 2020 2020 2020 2020 5b72                [r
-000161b0: 2e72 6573 756c 7428 2920 666f 7220 7220  .result() for r 
-000161c0: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
-000161d0: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-000161e0: 6564 2866 7574 7572 6573 295d 0d0a 0d0a  ed(futures)]....
-000161f0: 0d0a 2020 2020 6465 6620 5f63 6f6d 7075  ..    def _compu
-00016200: 7465 5f74 656d 706f 7261 6c28 7365 6c66  te_temporal(self
-00016210: 2c20 692c 2061 6c6c 5f73 706f 7473 5f74  , i, all_spots_t
-00016220: 7261 636b 7329 3a20 2020 2020 2020 2020  racks):         
-00016230: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016240: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016250: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
-00016260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016270: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00016280: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00016290: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000162a0: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-000162b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000162c0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-000162d0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-000162e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162f0: 206d 6974 6f74 6963 5f73 7065 6564 203d   mitotic_speed =
-00016300: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016310: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016320: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00016330: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016340: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00016350: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00016360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016370: 2020 2020 6d69 746f 7469 635f 636c 7573      mitotic_clus
-00016380: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
-00016390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163a0: 2020 2020 6d69 746f 7469 635f 6469 7374      mitotic_dist
-000163b0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-000163c0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000163d0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000163e0: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
-000163f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016400: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016410: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-00016420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016430: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00016440: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016460: 2020 6e6f 6e5f 6d69 746f 7469 635f 7261    non_mitotic_ra
-00016470: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-00016480: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016490: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
-000164a0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000164b0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000164c0: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-000164d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000164e0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000164f0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00016500: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00016510: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016520: 6e5f 6d69 746f 7469 635f 636c 7573 7465  n_mitotic_cluste
-00016530: 725f 636c 6173 7320 3d20 5b5d 0d0a 2020  r_class = []..  
-00016540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016550: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00016560: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00016570: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016580: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00016590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165a0: 2061 6c6c 5f64 6973 705f 7a20 3d20 5b5d   all_disp_z = []
-000165b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000165c0: 2020 2020 2020 616c 6c5f 6469 7370 5f79        all_disp_y
-000165d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000165e0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-000165f0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016610: 616c 6c5f 7261 6469 7573 203d 205b 5d0d  all_radius = [].
-00016620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016630: 2020 2020 2061 6c6c 5f73 7065 6564 203d       all_speed =
-00016640: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016650: 2020 2020 2020 2020 2061 6c6c 5f61 6363           all_acc
-00016660: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016670: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00016680: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00016690: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-000166a0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000166b0: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-000166c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000166d0: 2020 2020 2020 2020 616c 6c5f 6469 7374          all_dist
-000166e0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-000166f0: 205b 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020   []..........   
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 2066 6f72 2028 6b2c 7629 2069 6e20 616c   for (k,v) in al
-00016720: 6c5f 7370 6f74 735f 7472 6163 6b73 2e69  l_spots_tracks.i
-00016730: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00016740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016750: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016770: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-00016780: 3d20 616c 6c5f 7370 6f74 735f 7472 6163  = all_spots_trac
-00016790: 6b73 5b6b 5d5b 7365 6c66 2e66 7261 6d65  ks[k][self.frame
-000167a0: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
-000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167c0: 2020 2020 206d 6974 6f74 6963 203d 2061       mitotic = a
-000167d0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000167e0: 6b5d 5b73 656c 662e 6469 7669 6469 6e67  k][self.dividing
-000167f0: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016810: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016830: 6966 2069 203d 3d20 696e 7428 6375 7272  if i == int(curr
-00016840: 656e 745f 7469 6d65 293a 0d0a 2020 2020  ent_time):..    
+00014f30: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+00014f40: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014f50: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014f60: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+00014f70: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
+00014f80: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00014f90: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014fa0: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+00014fb0: 662e 7970 6f73 6964 5f6b 6579 5d29 202b  f.yposid_key]) +
+00014fc0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00014fd0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014fe0: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
+00014ff0: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
+00015000: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+00015010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015020: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00015030: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015040: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015050: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
+00015060: 7369 645f 6b65 795d 2920 2d20 2032 202a  sid_key]) -  2 *
+00015070: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00015080: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015090: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+000150a0: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+000150b0: 6579 5d29 202b 2066 6c6f 6174 2873 656c  ey]) + float(sel
+000150c0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000150d0: 6f70 6572 7469 6573 5b69 6e74 2870 7265  operties[int(pre
+000150e0: 5f73 6f75 7263 655f 6964 295d 5b73 656c  _source_id)][sel
+000150f0: 662e 7a70 6f73 6964 5f6b 6579 5d29 5d0d  f.zposid_key])].
+00015100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015110: 2020 2020 2061 6363 203d 206e 702e 7371       acc = np.sq
+00015120: 7274 286e 702e 646f 7428 7665 635f 322c  rt(np.dot(vec_2,
+00015130: 2076 6563 5f32 2929 2f73 656c 662e 7463   vec_2))/self.tc
+00015140: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015170: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015180: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015190: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000151a0: 7570 6461 7465 287b 7365 6c66 2e61 6363  update({self.acc
+000151b0: 656c 6572 6174 696f 6e5f 6b65 7920 3a20  eleration_key : 
+000151c0: 6163 637d 290d 0a20 2020 2020 2020 2065  acc})..        e
+000151d0: 6c69 6620 736f 7572 6365 5f69 6420 6973  lif source_id is
+000151e0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+000151f0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015200: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015210: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015220: 6461 7465 287b 7365 6c66 2e62 6566 6f72  date({self.befor
+00015230: 6569 645f 6b65 7920 3a20 4e6f 6e65 7d29  eid_key : None})
+00015240: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
+00015250: 0a0d 0a20 2020 2020 2020 2069 6620 7461  ...        if ta
+00015260: 7267 6574 5f69 6420 6973 206e 6f74 204e  rget_id is not N
+00015270: 6f6e 653a 2020 2020 2020 200d 0a20 2020  one:       ..   
+00015280: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00015290: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000152a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000152b0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+000152c0: 6166 7465 7269 645f 6b65 7920 3a20 696e  afterid_key : in
+000152d0: 7428 7461 7267 6574 5f69 6429 7d29 200d  t(target_id)}) .
+000152e0: 0a20 2020 2020 2020 2065 6c69 6620 7461  .        elif ta
+000152f0: 7267 6574 5f69 6420 6973 204e 6f6e 653a  rget_id is None:
+00015300: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015310: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015320: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015330: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015340: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
+00015350: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
+00015360: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015370: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00015380: 616e 6e65 6c5f 7570 6461 7465 2863 656c  annel_update(cel
+00015390: 6c5f 6964 2c20 7472 6163 6b5f 6964 2920  l_id, track_id) 
+000153a0: 2020 200d 0a0d 0a0d 0a20 2020 2064 6566     ......    def
+000153b0: 205f 7465 6d70 6f72 616c 5f70 6c6f 7473   _temporal_plots
+000153c0: 5f74 7261 636b 6d61 7465 2873 656c 6629  _trackmate(self)
+000153d0: 3a0d 0a20 2020 200d 0a20 2020 200d 0a20  :..    ..    .. 
+000153e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000153f0: 2020 2020 2073 656c 662e 4174 7472 203d       self.Attr =
+00015400: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00015410: 2020 2020 2073 7461 7274 7469 6d65 203d       starttime =
+00015420: 2069 6e74 286d 696e 2873 656c 662e 416c   int(min(self.Al
+00015430: 6c56 616c 7565 735b 7365 6c66 2e66 7261  lValues[self.fra
+00015440: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
+00015450: 2020 2020 2020 2020 2020 2020 2065 6e64               end
+00015460: 7469 6d65 203d 2069 6e74 286d 6178 2873  time = int(max(s
+00015470: 656c 662e 416c 6c56 616c 7565 735b 7365  elf.AllValues[se
+00015480: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d29  lf.frameid_key])
+00015490: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000154a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000154b0: 2020 2020 2020 7365 6c66 2e74 696d 6520        self.time 
+000154c0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000154d0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+000154e0: 6963 5f6d 6561 6e5f 6469 7370 5f7a 203d  ic_mean_disp_z =
+000154f0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015500: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015510: 635f 7661 725f 6469 7370 5f7a 203d 205b  c_var_disp_z = [
+00015520: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00015530: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00015540: 635f 6d65 616e 5f64 6973 705f 7920 3d20  c_mean_disp_y = 
+00015550: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015560: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015570: 5f76 6172 5f64 6973 705f 7920 3d20 5b5d  _var_disp_y = []
+00015580: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015590: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000155a0: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
+000155b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000155c0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000155d0: 7661 725f 6469 7370 5f78 203d 205b 5d0d  var_disp_x = [].
+000155e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000155f0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015600: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
+00015610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015620: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00015630: 6172 5f72 6164 6975 7320 3d20 5b5d 0d0a  ar_radius = []..
+00015640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015650: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00015660: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
+00015670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015680: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00015690: 5f73 7065 6564 203d 205b 5d0d 0a0d 0a20  _speed = [].... 
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000156b0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000156c0: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
+000156d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000156e0: 6d69 746f 7469 635f 7661 725f 6163 6320  mitotic_var_acc 
+000156f0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015700: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015710: 6f74 6963 5f6d 6561 6e5f 6469 7265 6374  otic_mean_direct
+00015720: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00015730: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015740: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015750: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
+00015760: 6368 616e 6765 203d 205b 5d0d 0a0d 0a20  change = [].... 
+00015770: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015780: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00015790: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000157a0: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
+000157b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000157c0: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+000157d0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+000157e0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+000157f0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015800: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00015810: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+00015820: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00015830: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00015840: 7370 5f7a 203d 205b 5d0d 0a0d 0a20 2020  sp_z = []....   
+00015850: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015860: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00015870: 616e 5f64 6973 705f 7920 3d20 5b5d 0d0a  an_disp_y = []..
+00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015890: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000158a0: 5f76 6172 5f64 6973 705f 7920 3d20 5b5d  _var_disp_y = []
+000158b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000158c0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+000158d0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
+000158e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000158f0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015900: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015910: 5f78 203d 205b 5d0d 0a0d 0a20 2020 2020  _x = []....     
+00015920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015930: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00015940: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00015950: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015960: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00015970: 6172 5f72 6164 6975 7320 3d20 5b5d 0d0a  ar_radius = []..
+00015980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015990: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+000159a0: 6963 5f6d 6561 6e5f 7370 6565 6420 3d20  ic_mean_speed = 
+000159b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000159c0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+000159d0: 6f74 6963 5f76 6172 5f73 7065 6564 203d  otic_var_speed =
+000159e0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+000159f0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015a00: 6d69 746f 7469 635f 6d65 616e 5f61 6363  mitotic_mean_acc
+00015a10: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015a20: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015a30: 6d69 746f 7469 635f 7661 725f 6163 6320  mitotic_var_acc 
+00015a40: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015a50: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00015a60: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00015a70: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00015a80: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015a90: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015aa0: 6d69 746f 7469 635f 7661 725f 6469 7265  mitotic_var_dire
+00015ab0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00015ac0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015ad0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015ae0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00015af0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00015b00: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015b10: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015b20: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+00015b30: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00015b40: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015b50: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00015b60: 6561 6e5f 6469 7370 5f7a 203d 205b 5d0d  ean_disp_z = [].
+00015b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b80: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00015b90: 7370 5f7a 203d 205b 5d0d 0a0d 0a20 2020  sp_z = []....   
+00015ba0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015bb0: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00015bc0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00015bd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015be0: 5f76 6172 5f64 6973 705f 7920 3d20 5b5d  _var_disp_y = []
+00015bf0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015c00: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00015c10: 6e5f 6469 7370 5f78 203d 205b 5d0d 0a20  n_disp_x = [].. 
+00015c20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015c30: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00015c40: 5f78 203d 205b 5d0d 0a0d 0a20 2020 2020  _x = []....     
+00015c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015c60: 616c 6c5f 6d65 616e 5f72 6164 6975 7320  all_mean_radius 
+00015c70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015c80: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00015c90: 6172 5f72 6164 6975 7320 3d20 5b5d 0d0a  ar_radius = []..
+00015ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015cb0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00015cc0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00015cd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015ce0: 2e61 6c6c 5f76 6172 5f73 7065 6564 203d  .all_var_speed =
+00015cf0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015d00: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00015d10: 6d65 616e 5f61 6363 203d 205b 5d0d 0a20  mean_acc = [].. 
+00015d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015d30: 656c 662e 616c 6c5f 7661 725f 6163 6320  elf.all_var_acc 
+00015d40: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015d50: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015d60: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
+00015d70: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+00015d80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015d90: 656c 662e 616c 6c5f 7661 725f 6469 7265  elf.all_var_dire
+00015da0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00015db0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015dc0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00015dd0: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
+00015de0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00015df0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015e00: 6c66 2e61 6c6c 5f76 6172 5f64 6973 7461  lf.all_var_dista
+00015e10: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00015e20: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015e30: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015e40: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00015e50: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015e60: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00015e70: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00015e80: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+00015e90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015ea0: 2e61 6c6c 5f63 6c75 7374 6572 5f63 6c61  .all_cluster_cla
+00015eb0: 7373 203d 205b 5d0d 0a0d 0a20 2020 2020  ss = []....     
+00015ec0: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+00015ed0: 706f 7473 5f74 7261 636b 7320 3d20 7b7d  pots_tracks = {}
+00015ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015ef0: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+00015f00: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015f10: 7072 6f70 6572 7469 6573 2e69 7465 6d73  properties.items
+00015f20: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00015f30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f50: 2020 2061 6c6c 5f73 706f 7473 203d 2073     all_spots = s
+00015f60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015f70: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
+00015f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f90: 2020 2020 2069 6620 7365 6c66 2e74 7261       if self.tra
+00015fa0: 636b 6964 5f6b 6579 2069 6e20 616c 6c5f  ckid_key in all_
+00015fb0: 7370 6f74 733a 0d0a 2020 2020 2020 2020  spots:..        
+00015fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fd0: 2020 616c 6c5f 7370 6f74 735f 7472 6163    all_spots_trac
+00015fe0: 6b73 5b6b 5d20 3d20 616c 6c5f 7370 6f74  ks[k] = all_spot
+00015ff0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00016000: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00016010: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00016020: 2020 2020 2020 2020 2066 7574 7572 6573           futures
+00016030: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016040: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
+00016050: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
+00016060: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+00016070: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
+00016080: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
+00016090: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
+000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000160c0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000160d0: 696e 2074 7164 6d28 7261 6e67 6528 7374  in tqdm(range(st
+000160e0: 6172 7474 696d 652c 2065 6e64 7469 6d65  arttime, endtime
+000160f0: 292c 2074 6f74 616c 3d65 6e64 7469 6d65  ), total=endtime
+00016100: 202d 2073 7461 7274 7469 6d65 293a 0d0a   - starttime):..
+00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016120: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016140: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+00016150: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+00016160: 656c 662e 5f63 6f6d 7075 7465 5f74 656d  elf._compute_tem
+00016170: 706f 7261 6c2c 2069 2c20 616c 6c5f 7370  poral, i, all_sp
+00016180: 6f74 735f 7472 6163 6b73 2929 0d0a 200d  ots_tracks)).. .
+00016190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000161a0: 2020 2020 205b 722e 7265 7375 6c74 2829       [r.result()
+000161b0: 2066 6f72 2072 2069 6e20 636f 6e63 7572   for r in concur
+000161c0: 7265 6e74 2e66 7574 7572 6573 2e61 735f  rent.futures.as_
+000161d0: 636f 6d70 6c65 7465 6428 6675 7475 7265  completed(future
+000161e0: 7329 5d0d 0a0d 0a0d 0a20 2020 2064 6566  s)]......    def
+000161f0: 205f 636f 6d70 7574 655f 7465 6d70 6f72   _compute_tempor
+00016200: 616c 2873 656c 662c 2069 2c20 616c 6c5f  al(self, i, all_
+00016210: 7370 6f74 735f 7472 6163 6b73 293a 2020  spots_tracks):  
+00016220: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016240: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016250: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+00016260: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016270: 6f74 6963 5f64 6973 705f 7920 3d20 5b5d  otic_disp_y = []
+00016280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016290: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+000162a0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+000162b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000162c0: 6974 6f74 6963 5f72 6164 6975 7320 3d20  itotic_radius = 
+000162d0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000162e0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000162f0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00016300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016310: 6d69 746f 7469 635f 6163 6320 3d20 5b5d  mitotic_acc = []
+00016320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016330: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00016340: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00016350: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016360: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00016370: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
+00016380: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016390: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+000163a0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+000163b0: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 2020  _mask = []....  
+000163c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163d0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+000163e0: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+000163f0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016400: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00016410: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00016420: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016430: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+00016440: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016450: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016460: 6f74 6963 5f72 6164 6975 7320 3d20 5b5d  otic_radius = []
+00016470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016480: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00016490: 635f 7370 6565 6420 3d20 5b5d 0d0a 2020  c_speed = []..  
+000164a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164b0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6163    non_mitotic_ac
+000164c0: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+000164d0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+000164e0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+000164f0: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00016500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016510: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016520: 5f63 6c75 7374 6572 5f63 6c61 7373 203d  _cluster_class =
+00016530: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016540: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016550: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+00016560: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016580: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00016590: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+000165a0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+000165b0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000165c0: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
+000165d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165e0: 2020 616c 6c5f 6469 7370 5f78 203d 205b    all_disp_x = [
+000165f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016600: 2020 2020 2020 2061 6c6c 5f72 6164 6975         all_radiu
+00016610: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00016620: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00016630: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00016640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016650: 616c 6c5f 6163 6320 3d20 5b5d 0d0a 2020  all_acc = []..  
+00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016670: 2020 616c 6c5f 6469 7265 6374 696f 6e61    all_directiona
+00016680: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+00016690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166a0: 2020 2061 6c6c 5f63 6c75 7374 6572 5f63     all_cluster_c
+000166b0: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
+000166c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000166d0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+000166e0: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 0d0a  _mask = []......
+000166f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016700: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+00016710: 2920 696e 2061 6c6c 5f73 706f 7473 5f74  ) in all_spots_t
+00016720: 7261 636b 732e 6974 656d 7328 293a 0d0a  racks.items():..
+00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016740: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016760: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00016770: 745f 7469 6d65 203d 2061 6c6c 5f73 706f  t_time = all_spo
+00016780: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00016790: 662e 6672 616d 6569 645f 6b65 795d 0d0a  f.frameid_key]..
+000167a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167b0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000167c0: 7469 6320 3d20 616c 6c5f 7370 6f74 735f  tic = all_spots_
+000167d0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
+000167e0: 6976 6964 696e 675f 6b65 795d 0d0a 2020  ividing_key]..  
+000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016800: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00016810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016820: 2020 2020 2020 2069 6620 6920 3d3d 2069         if i == i
+00016830: 6e74 2863 7572 7265 6e74 5f74 696d 6529  nt(current_time)
+00016840: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016860: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016870: 206d 6974 6f74 6963 3a0d 0a20 2020 2020   mitotic:..     
+00016860: 2020 2020 2069 6620 6d69 746f 7469 633a       if mitotic:
+00016870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00016880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168a0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-000168b0: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
-000168c0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-000168d0: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00016890: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000168a0: 635f 6469 7370 5f7a 2e61 7070 656e 6428  c_disp_z.append(
+000168b0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000168c0: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
+000168d0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
 000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016900: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016910: 6469 7370 5f79 2e61 7070 656e 6428 616c  disp_y.append(al
-00016920: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016930: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-00016940: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000168f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016900: 6974 6f74 6963 5f64 6973 705f 792e 6170  itotic_disp_y.ap
+00016910: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00016920: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+00016930: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00016940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016960: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016970: 6f74 6963 5f64 6973 705f 782e 6170 7065  otic_disp_x.appe
-00016980: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00016990: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
-000169a0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00016960: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00016970: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
+00016980: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00016990: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+000169a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169d0: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
-000169e0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000169f0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00016a00: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
+000169c0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+000169d0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
+000169e0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+000169f0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+00016a00: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a30: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
-00016a40: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
-00016a50: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016a60: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
-00016a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a20: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016a30: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
+00016a40: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00016a50: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
+00016a60: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a90: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-00016aa0: 635f 6163 632e 6170 7065 6e64 2861 6c6c  c_acc.append(all
-00016ab0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00016ac0: 5b73 656c 662e 6163 6365 6c65 7261 7469  [self.accelerati
-00016ad0: 6f6e 5f6b 6579 5d29 0d0a 2020 2020 2020  on_key])..      
+00016a90: 206d 6974 6f74 6963 5f61 6363 2e61 7070   mitotic_acc.app
+00016aa0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00016ab0: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
+00016ac0: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
+00016ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b00: 2020 6d69 746f 7469 635f 6469 7265 6374    mitotic_direct
-00016b10: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
-00016b20: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00016b30: 6163 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74  acks[k][self.mot
-00016b40: 696f 6e5f 616e 676c 655f 6b65 795d 290d  ion_angle_key]).
-00016b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016af0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00016b00: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016b10: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
+00016b20: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016b30: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
+00016b40: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b70: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016b80: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00016b90: 6173 6b2e 6170 7065 6e64 2861 6c6c 5f73  ask.append(all_s
-00016ba0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00016bb0: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
-00016bc0: 6c5f 6d61 736b 5f6b 6579 5d29 0d0a 2020  l_mask_key])..  
+00016b70: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00016b80: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+00016b90: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016ba0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+00016bb0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00016bc0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 00016bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
-00016c00: 7573 7465 7263 6c61 7373 5f6b 6579 2069  usterclass_key i
-00016c10: 6e20 616c 6c5f 7370 6f74 735f 7472 6163  n all_spots_trac
-00016c20: 6b73 5b6b 5d2e 6b65 7973 2829 203a 0d0a  ks[k].keys() :..
+00016be0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016bf0: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+00016c00: 735f 6b65 7920 696e 2061 6c6c 5f73 706f  s_key in all_spo
+00016c10: 7473 5f74 7261 636b 735b 6b5d 2e6b 6579  ts_tracks[k].key
+00016c20: 7328 2920 3a0d 0a20 2020 2020 2020 2020  s() :..         
 00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016c60: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-00016c70: 6c61 7373 2e61 7070 656e 6428 616c 6c5f  lass.append(all_
-00016c80: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00016c90: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
-00016ca0: 735f 6b65 795d 290d 0a0d 0a0d 0a20 2020  s_key])......   
+00016c50: 2020 2020 2020 6d69 746f 7469 635f 636c        mitotic_cl
+00016c60: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
+00016c70: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00016c80: 636b 735b 6b5d 5b73 656c 662e 636c 7573  cks[k][self.clus
+00016c90: 7465 7263 6c61 7373 5f6b 6579 5d29 0d0a  terclass_key])..
+00016ca0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00016cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016cd0: 6620 6e6f 7420 6d69 746f 7469 633a 0d0a  f not mitotic:..
+00016cc0: 2020 2020 2020 6966 206e 6f74 206d 6974        if not mit
+00016cd0: 6f74 6963 3a0d 0a20 2020 2020 2020 2020  otic:..         
 00016ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d00: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016d10: 7469 635f 6469 7370 5f7a 2e61 7070 656e  tic_disp_z.appen
-00016d20: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016d30: 6b73 5b6b 5d5b 7365 6c66 2e7a 706f 7369  ks[k][self.zposi
-00016d40: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00016cf0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016d00: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00016d10: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
+00016d20: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00016d30: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d70: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00016d80: 705f 792e 6170 7065 6e64 2861 6c6c 5f73  p_y.append(all_s
-00016d90: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00016da0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00016db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016d60: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00016d70: 7469 635f 6469 7370 5f79 2e61 7070 656e  tic_disp_y.appen
+00016d80: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00016d90: 6b73 5b6b 5d5b 7365 6c66 2e79 706f 7369  ks[k][self.yposi
+00016da0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dd0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00016de0: 746f 7469 635f 6469 7370 5f78 2e61 7070  totic_disp_x.app
-00016df0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00016e00: 6163 6b73 5b6b 5d5b 7365 6c66 2e78 706f  acks[k][self.xpo
-00016e10: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00016dd0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00016de0: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
+00016df0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00016e00: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00016e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00016e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f72     non_mitotic_r
-00016e50: 6164 6975 732e 6170 7065 6e64 2861 6c6c  adius.append(all
-00016e60: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00016e70: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
-00016e80: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00016e30: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016e40: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
+00016e50: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00016e60: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
+00016e70: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00016eb0: 6d69 746f 7469 635f 7370 6565 642e 6170  mitotic_speed.ap
-00016ec0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00016ed0: 7261 636b 735b 6b5d 5b73 656c 662e 7370  racks[k][self.sp
-00016ee0: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
+00016ea0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f73     non_mitotic_s
+00016eb0: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
+00016ec0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00016ed0: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+00016ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f10: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f61     non_mitotic_a
-00016f20: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-00016f30: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00016f40: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-00016f50: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00016f00: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016f10: 746f 7469 635f 6163 632e 6170 7065 6e64  totic_acc.append
+00016f20: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00016f30: 735b 6b5d 5b73 656c 662e 6163 6365 6c65  s[k][self.accele
+00016f40: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
+00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00016f80: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-00016f90: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00016fa0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00016fb0: 7261 636b 735b 6b5d 5b73 656c 662e 6d6f  racks[k][self.mo
-00016fc0: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
-00016fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016f70: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00016f80: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00016f90: 616e 6765 2e61 7070 656e 6428 616c 6c5f  ange.append(all_
+00016fa0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00016fb0: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+00016fc0: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ff0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017000: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-00017010: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
-00017020: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017030: 5b6b 5d5b 7365 6c66 2e64 6973 7461 6e63  [k][self.distanc
-00017040: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 795d  e_cell_mask_key]
-00017050: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00016ff0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00017000: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00017010: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017020: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017030: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00017040: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
+00017050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00017080: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-00017090: 6b65 7920 696e 2061 6c6c 5f73 706f 7473  key in all_spots
-000170a0: 5f74 7261 636b 735b 6b5d 2e6b 6579 7328  _tracks[k].keys(
-000170b0: 2920 3a0d 0a20 2020 2020 2020 2020 2020  ) :..           
+00017070: 2020 6966 2073 656c 662e 636c 7573 7465    if self.cluste
+00017080: 7263 6c61 7373 5f6b 6579 2069 6e20 616c  rclass_key in al
+00017090: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000170a0: 5d2e 6b65 7973 2829 203a 0d0a 2020 2020  ].keys() :..    
+000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170e0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-000170f0: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
-00017100: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017110: 7261 636b 735b 6b5d 5b73 656c 662e 636c  racks[k][self.cl
-00017120: 7573 7465 7263 6c61 7373 5f6b 6579 5d29  usterclass_key])
-00017130: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
-00017160: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017170: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017180: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
+000170d0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+000170e0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+000170f0: 6c61 7373 2e61 7070 656e 6428 616c 6c5f  lass.append(all_
+00017100: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017110: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
+00017120: 735f 6b65 795d 290d 0a0d 0a20 2020 2020  s_key])....     
+00017130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017140: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017150: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
+00017160: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017170: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
+00017180: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171b0: 2061 6c6c 5f64 6973 705f 792e 6170 7065   all_disp_y.appe
-000171c0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000171d0: 636b 735b 6b5d 5b73 656c 662e 7970 6f73  cks[k][self.ypos
-000171e0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+000171a0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+000171b0: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
+000171c0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000171d0: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
+000171e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017200: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017210: 6469 7370 5f78 2e61 7070 656e 6428 616c  disp_x.append(al
-00017220: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017230: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00017240: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017260: 2020 2020 2020 2061 6c6c 5f72 6164 6975         all_radiu
-00017270: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00017280: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017290: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
+00017200: 2020 2061 6c6c 5f64 6973 705f 782e 6170     all_disp_x.ap
+00017210: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017220: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+00017230: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017260: 6c5f 7261 6469 7573 2e61 7070 656e 6428  l_radius.append(
+00017270: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017280: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
+00017290: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
 000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172c0: 2020 616c 6c5f 7370 6565 642e 6170 7065    all_speed.appe
-000172d0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000172e0: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-000172f0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+000172b0: 2020 2020 2020 2020 2061 6c6c 5f73 7065           all_spe
+000172c0: 6564 2e61 7070 656e 6428 616c 6c5f 7370  ed.append(all_sp
+000172d0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000172e0: 6c66 2e73 7065 6564 5f6b 6579 5d29 0d0a  lf.speed_key])..
+000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
-00017320: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-00017330: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017340: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-00017350: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017310: 2020 616c 6c5f 6163 632e 6170 7065 6e64    all_acc.append
+00017320: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017330: 735b 6b5d 5b73 656c 662e 6163 6365 6c65  s[k][self.accele
+00017340: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
+00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017370: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
-00017380: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00017390: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-000173a0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000173b0: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-000173c0: 5d29 2020 200d 0a20 2020 2020 2020 2020  ])   ..         
+00017370: 616c 6c5f 6469 7265 6374 696f 6e61 6c5f  all_directional_
+00017380: 6368 616e 6765 2e61 7070 656e 6428 616c  change.append(al
+00017390: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000173a0: 5d5b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ][self.motion_an
+000173b0: 676c 655f 6b65 795d 2920 2020 0d0a 2020  gle_key])   ..  
+000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173e0: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-000173f0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00017400: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017410: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017420: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017430: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
+000173e0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
+000173f0: 6c5f 6d61 736b 2e61 7070 656e 6428 616c  l_mask.append(al
+00017400: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017410: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
+00017420: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
+00017430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017460: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00017470: 5f6b 6579 2069 6e20 616c 6c5f 7370 6f74  _key in all_spot
-00017480: 735f 7472 6163 6b73 5b6b 5d2e 6b65 7973  s_tracks[k].keys
-00017490: 2829 203a 0d0a 2020 2020 2020 2020 2020  () :..          
+00017450: 2020 2069 6620 7365 6c66 2e63 6c75 7374     if self.clust
+00017460: 6572 636c 6173 735f 6b65 7920 696e 2061  erclass_key in a
+00017470: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017480: 6b5d 2e6b 6579 7328 2920 3a0d 0a20 2020  k].keys() :..   
+00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2020 2061 6c6c 5f63 6c75 7374 6572       all_cluster
-000174d0: 5f63 6c61 7373 2e61 7070 656e 6428 616c  _class.append(al
-000174e0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000174f0: 5d5b 7365 6c66 2e63 6c75 7374 6572 636c  ][self.clustercl
-00017500: 6173 735f 6b65 795d 2920 2020 200d 0a20  ass_key])    .. 
+000174b0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+000174c0: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+000174d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000174e0: 7261 636b 735b 6b5d 5b73 656c 662e 636c  racks[k][self.cl
+000174f0: 7573 7465 7263 6c61 7373 5f6b 6579 5d29  usterclass_key])
+00017500: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00017540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017550: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00017560: 705f 7a20 3d20 6e70 2e61 6273 286e 702e  p_z = np.abs(np.
-00017570: 6469 6666 286d 6974 6f74 6963 5f64 6973  diff(mitotic_dis
-00017580: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-00017590: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-000175a0: 6963 5f64 6973 705f 7920 3d20 6e70 2e61  ic_disp_y = np.a
-000175b0: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
-000175c0: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
-000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175e0: 206d 6974 6f74 6963 5f64 6973 705f 7820   mitotic_disp_x 
-000175f0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017600: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
-00017610: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00017620: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017630: 6f74 6963 5f64 6973 705f 7a20 3d20 6e70  otic_disp_z = np
-00017640: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
-00017650: 5f6d 6974 6f74 6963 5f64 6973 705f 7a29  _mitotic_disp_z)
-00017660: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017670: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00017680: 6963 5f64 6973 705f 7920 3d20 6e70 2e61  ic_disp_y = np.a
-00017690: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
-000176a0: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
-000176b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000176c0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000176d0: 5f64 6973 705f 7820 3d20 6e70 2e61 6273  _disp_x = np.abs
-000176e0: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
-000176f0: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
-00017700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017710: 2020 2020 2061 6c6c 5f64 6973 705f 7a20       all_disp_z 
-00017720: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017730: 2861 6c6c 5f64 6973 705f 7a29 290d 0a20  (all_disp_z)).. 
-00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017750: 2020 2061 6c6c 5f64 6973 705f 7920 3d20     all_disp_y = 
-00017760: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
-00017770: 6c6c 5f64 6973 705f 7929 290d 0a20 2020  ll_disp_y))..   
-00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 2061 6c6c 5f64 6973 705f 7820 3d20 6e70   all_disp_x = np
-000177a0: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
-000177b0: 5f64 6973 705f 7829 290d 0a0d 0a0d 0a20  _disp_x))...... 
+00017530: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00017540: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00017550: 7469 635f 6469 7370 5f7a 203d 206e 702e  tic_disp_z = np.
+00017560: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
+00017570: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
+00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017590: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
+000175a0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+000175b0: 6628 6d69 746f 7469 635f 6469 7370 5f79  f(mitotic_disp_y
+000175c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000175d0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000175e0: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
+000175f0: 6e70 2e64 6966 6628 6d69 746f 7469 635f  np.diff(mitotic_
+00017600: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
+00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017620: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00017630: 5f7a 203d 206e 702e 6162 7328 6e70 2e64  _z = np.abs(np.d
+00017640: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
+00017650: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00017660: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00017670: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00017680: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+00017690: 6628 6e6f 6e5f 6d69 746f 7469 635f 6469  f(non_mitotic_di
+000176a0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+000176b0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+000176c0: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+000176d0: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+000176e0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+000176f0: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
+00017700: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017710: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
+00017720: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
+00017730: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+00017740: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00017750: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
+00017760: 2e64 6966 6628 616c 6c5f 6469 7370 5f79  .diff(all_disp_y
+00017770: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00017780: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00017790: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
+000177a0: 6966 6628 616c 6c5f 6469 7370 5f78 2929  iff(all_disp_x))
+000177b0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
 000177c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000177f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017800: 662e 7469 6d65 2e61 7070 656e 6428 6920  f.time.append(i 
-00017810: 2a20 7365 6c66 2e74 6361 6c69 6272 6174  * self.tcalibrat
-00017820: 696f 6e29 0d0a 0d0a 2020 2020 2020 2020  ion)....        
-00017830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017840: 2e6d 6974 6f74 6963 5f63 6c75 7374 6572  .mitotic_cluster
-00017850: 5f63 6c61 7373 2e61 7070 656e 6428 6e70  _class.append(np
-00017860: 2e61 7361 7272 6179 286d 6974 6f74 6963  .asarray(mitotic
-00017870: 5f63 6c75 7374 6572 5f63 6c61 7373 2929  _cluster_class))
-00017880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017890: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000178a0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-000178b0: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
-000178c0: 7361 7272 6179 286e 6f6e 5f6d 6974 6f74  sarray(non_mitot
-000178d0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
-000178e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000178f0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017900: 5f63 6c75 7374 6572 5f63 6c61 7373 2e61  _cluster_class.a
-00017910: 7070 656e 6428 6e70 2e61 7361 7272 6179  ppend(np.asarray
-00017920: 2861 6c6c 5f63 6c75 7374 6572 5f63 6c61  (all_cluster_cla
-00017930: 7373 2929 0d0a 0d0a 2020 2020 2020 2020  ss))....        
-00017940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017950: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00017960: 7370 5f7a 2e61 7070 656e 6428 6e70 2e6d  sp_z.append(np.m
-00017970: 6561 6e28 6d69 746f 7469 635f 6469 7370  ean(mitotic_disp
-00017980: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
-00017990: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000179a0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-000179b0: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
-000179c0: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-000179d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000179e0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000179f0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-00017a00: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00017a10: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
-00017a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017a30: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017a40: 6963 5f76 6172 5f64 6973 705f 792e 6170  ic_var_disp_y.ap
-00017a50: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-00017a60: 7469 635f 6469 7370 5f79 2929 0d0a 0d0a  tic_disp_y))....
-00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a80: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017a90: 5f6d 6561 6e5f 6469 7370 5f78 2e61 7070  _mean_disp_x.app
-00017aa0: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00017ab0: 7469 635f 6469 7370 5f78 2929 0d0a 2020  tic_disp_x))..  
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00017ae0: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
-00017af0: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00017b00: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
-00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b20: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00017b30: 6e5f 7261 6469 7573 2e61 7070 656e 6428  n_radius.append(
-00017b40: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-00017b50: 7261 6469 7573 2929 0d0a 2020 2020 2020  radius))..      
-00017b60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017b70: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f72  lf.mitotic_var_r
-00017b80: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00017b90: 7374 6428 6d69 746f 7469 635f 7261 6469  std(mitotic_radi
-00017ba0: 7573 2929 0d0a 0d0a 2020 2020 2020 2020  us))....        
-00017bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017bc0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7370  .mitotic_mean_sp
-00017bd0: 6565 642e 6170 7065 6e64 286e 702e 6d65  eed.append(np.me
-00017be0: 616e 286d 6974 6f74 6963 5f73 7065 6564  an(mitotic_speed
-00017bf0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00017c00: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00017c10: 6f74 6963 5f76 6172 5f73 7065 6564 2e61  otic_var_speed.a
-00017c20: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00017c30: 6f74 6963 5f73 7065 6564 2929 0d0a 0d0a  otic_speed))....
-00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c50: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017c60: 5f6d 6561 6e5f 6163 632e 6170 7065 6e64  _mean_acc.append
-00017c70: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00017c80: 5f61 6363 2929 0d0a 2020 2020 2020 2020  _acc))..        
-00017c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017ca0: 2e6d 6974 6f74 6963 5f76 6172 5f61 6363  .mitotic_var_acc
-00017cb0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-00017cc0: 6974 6f74 6963 5f61 6363 2929 0d0a 0d0a  itotic_acc))....
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ce0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017cf0: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-00017d00: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-00017d10: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-00017d20: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00017d30: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
-00017d40: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017d50: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
-00017d60: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-00017d70: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-00017d80: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-00017d90: 6368 616e 6765 2929 0d0a 0d0a 2020 2020  change))....    
-00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017db0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00017dc0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-00017dd0: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
-00017de0: 6561 6e28 6d69 746f 7469 635f 6469 7374  ean(mitotic_dist
-00017df0: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00017e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017e10: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017e20: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
-00017e30: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00017e40: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00017e50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017e60: 736b 2929 0d0a 0d0a 2020 2020 2020 2020  sk))....        
-00017e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017e80: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00017e90: 6e5f 6469 7370 5f7a 2e61 7070 656e 6428  n_disp_z.append(
-00017ea0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-00017eb0: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
-00017ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ed0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00017ee0: 6963 5f76 6172 5f64 6973 705f 7a2e 6170  ic_var_disp_z.ap
-00017ef0: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00017f00: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-00017f10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017f20: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00017f30: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00017f40: 7370 5f79 2e61 7070 656e 6428 6e70 2e6d  sp_y.append(np.m
-00017f50: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-00017f60: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
-00017f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017f80: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00017f90: 6172 5f64 6973 705f 792e 6170 7065 6e64  ar_disp_y.append
-00017fa0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
-00017fb0: 7469 635f 6469 7370 5f79 2929 0d0a 0d0a  tic_disp_y))....
-00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fd0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00017fe0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
-00017ff0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018000: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018010: 5f78 2929 0d0a 2020 2020 2020 2020 2020  _x))..          
-00018020: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018030: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00018040: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-00018050: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00018060: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
-00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018080: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018090: 5f6d 6561 6e5f 7261 6469 7573 2e61 7070  _mean_radius.app
-000180a0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
-000180b0: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
-000180c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000180d0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000180e0: 6974 6f74 6963 5f76 6172 5f72 6164 6975  itotic_var_radiu
-000180f0: 732e 6170 7065 6e64 286e 702e 7374 6428  s.append(np.std(
-00018100: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
-00018110: 7573 2929 0d0a 0d0a 2020 2020 2020 2020  us))....        
-00018120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018130: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00018140: 6e5f 7370 6565 642e 6170 7065 6e64 286e  n_speed.append(n
-00018150: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
-00018160: 6963 5f73 7065 6564 2929 0d0a 2020 2020  ic_speed))..    
-00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018180: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018190: 5f76 6172 5f73 7065 6564 2e61 7070 656e  _var_speed.appen
-000181a0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-000181b0: 6f74 6963 5f73 7065 6564 2929 0d0a 0d0a  otic_speed))....
-000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181d0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000181e0: 6f74 6963 5f6d 6561 6e5f 6163 632e 6170  otic_mean_acc.ap
-000181f0: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00018200: 5f6d 6974 6f74 6963 5f61 6363 2929 0d0a  _mitotic_acc))..
-00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018220: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00018230: 6f74 6963 5f76 6172 5f61 6363 2e61 7070  otic_var_acc.app
-00018240: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
-00018250: 6974 6f74 6963 5f61 6363 2929 0d0a 0d0a  itotic_acc))....
-00018260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018270: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00018280: 6f74 6963 5f6d 6561 6e5f 6469 7265 6374  otic_mean_direct
-00018290: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
-000182a0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
-000182b0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
-000182c0: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
-000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182e0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000182f0: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
-00018300: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00018310: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
-00018320: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-00018330: 6368 616e 6765 2929 200d 0a0d 0a20 2020  change)) ....   
-00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018350: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018360: 635f 6d65 616e 5f64 6973 7461 6e63 655f  c_mean_distance_
-00018370: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00018380: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018390: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-000183a0: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-000183b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000183c0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-000183d0: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
-000183e0: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
-000183f0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00018400: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018410: 6173 6b29 290d 0a0d 0a0d 0a20 2020 2020  ask))......     
-00018420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018430: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
-00018440: 705f 7a2e 6170 7065 6e64 286e 702e 6d65  p_z.append(np.me
-00018450: 616e 2861 6c6c 5f64 6973 705f 7a29 290d  an(all_disp_z)).
-00018460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018470: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00018480: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
-00018490: 6e70 2e73 7464 2861 6c6c 5f64 6973 705f  np.std(all_disp_
-000184a0: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
-000184b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000184c0: 616c 6c5f 6d65 616e 5f64 6973 705f 792e  all_mean_disp_y.
-000184d0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-000184e0: 6c6c 5f64 6973 705f 7929 290d 0a20 2020  ll_disp_y))..   
-000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00018510: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
-00018520: 7464 2861 6c6c 5f64 6973 705f 7929 290d  td(all_disp_y)).
-00018530: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018540: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018550: 6d65 616e 5f64 6973 705f 782e 6170 7065  mean_disp_x.appe
-00018560: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
-00018570: 6973 705f 7829 290d 0a20 2020 2020 2020  isp_x))..       
-00018580: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018590: 662e 616c 6c5f 7661 725f 6469 7370 5f78  f.all_var_disp_x
-000185a0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-000185b0: 6c6c 5f64 6973 705f 7829 290d 0a0d 0a20  ll_disp_x)).... 
-000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185d0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-000185e0: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
-000185f0: 702e 6d65 616e 2861 6c6c 5f72 6164 6975  p.mean(all_radiu
-00018600: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
-00018610: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018620: 6c5f 7661 725f 7261 6469 7573 2e61 7070  l_var_radius.app
-00018630: 656e 6428 6e70 2e73 7464 2861 6c6c 5f72  end(np.std(all_r
-00018640: 6164 6975 7329 290d 0a0d 0a20 2020 2020  adius))....     
-00018650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018660: 656c 662e 616c 6c5f 6d65 616e 5f73 7065  elf.all_mean_spe
-00018670: 6564 2e61 7070 656e 6428 6e70 2e6d 6561  ed.append(np.mea
-00018680: 6e28 616c 6c5f 7370 6565 6429 290d 0a20  n(all_speed)).. 
-00018690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186a0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-000186b0: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
-000186c0: 7374 6428 616c 6c5f 7370 6565 6429 290d  std(all_speed)).
-000186d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000186e0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000186f0: 6d65 616e 5f61 6363 2e61 7070 656e 6428  mean_acc.append(
-00018700: 6e70 2e6d 6561 6e28 616c 6c5f 6163 6329  np.mean(all_acc)
-00018710: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018720: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018730: 7661 725f 6163 632e 6170 7065 6e64 286e  var_acc.append(n
-00018740: 702e 7374 6428 616c 6c5f 6163 6329 290d  p.std(all_acc)).
-00018750: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
-00018760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018770: 616c 6c5f 6d65 616e 5f64 6972 6563 7469  all_mean_directi
-00018780: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00018790: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
-000187a0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-000187b0: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-000187c0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000187d0: 6c5f 7661 725f 6469 7265 6374 696f 6e61  l_var_directiona
-000187e0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-000187f0: 6e70 2e73 7464 2861 6c6c 5f64 6972 6563  np.std(all_direc
-00018800: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
-00018810: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018820: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018830: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
-00018840: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-00018850: 702e 6d65 616e 2861 6c6c 5f64 6973 7461  p.mean(all_dista
-00018860: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-00018870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018880: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00018890: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-000188a0: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
-000188b0: 7464 2861 6c6c 5f64 6973 7461 6e63 655f  td(all_distance_
-000188c0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+000177d0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177f0: 2020 2020 7365 6c66 2e74 696d 652e 6170      self.time.ap
+00017800: 7065 6e64 2869 202a 2073 656c 662e 7463  pend(i * self.tc
+00017810: 616c 6962 7261 7469 6f6e 290d 0a0d 0a20  alibration).... 
+00017820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017830: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017840: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+00017850: 7065 6e64 286e 702e 6173 6172 7261 7928  pend(np.asarray(
+00017860: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00017870: 636c 6173 7329 290d 0a20 2020 2020 2020  class))..       
+00017880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017890: 662e 6e6f 6e5f 6d69 746f 7469 635f 636c  f.non_mitotic_cl
+000178a0: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
+000178b0: 6e64 286e 702e 6173 6172 7261 7928 6e6f  nd(np.asarray(no
+000178c0: 6e5f 6d69 746f 7469 635f 636c 7573 7465  n_mitotic_cluste
+000178d0: 725f 636c 6173 7329 290d 0a20 2020 2020  r_class))..     
+000178e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000178f0: 656c 662e 616c 6c5f 636c 7573 7465 725f  elf.all_cluster_
+00017900: 636c 6173 732e 6170 7065 6e64 286e 702e  class.append(np.
+00017910: 6173 6172 7261 7928 616c 6c5f 636c 7573  asarray(all_clus
+00017920: 7465 725f 636c 6173 7329 290d 0a0d 0a20  ter_class)).... 
+00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017940: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017950: 6d65 616e 5f64 6973 705f 7a2e 6170 7065  mean_disp_z.appe
+00017960: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+00017970: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
+00017980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017990: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+000179a0: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
+000179b0: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+000179c0: 6973 705f 7a29 290d 0a0d 0a20 2020 2020  isp_z))....     
+000179d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000179e0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000179f0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+00017a00: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
+00017a10: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
+00017a20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017a30: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00017a40: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
+00017a50: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
+00017a60: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
+00017a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017a80: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00017a90: 705f 782e 6170 7065 6e64 286e 702e 6d65  p_x.append(np.me
+00017aa0: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
+00017ab0: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
+00017ac0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00017ad0: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
+00017ae0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00017af0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00017b00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017b10: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017b20: 7469 635f 6d65 616e 5f72 6164 6975 732e  tic_mean_radius.
+00017b30: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00017b40: 6974 6f74 6963 5f72 6164 6975 7329 290d  itotic_radius)).
+00017b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b60: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017b70: 635f 7661 725f 7261 6469 7573 2e61 7070  c_var_radius.app
+00017b80: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00017b90: 6963 5f72 6164 6975 7329 290d 0a0d 0a20  ic_radius)).... 
+00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bb0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017bc0: 6d65 616e 5f73 7065 6564 2e61 7070 656e  mean_speed.appen
+00017bd0: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00017be0: 635f 7370 6565 6429 290d 0a20 2020 2020  c_speed))..     
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017c00: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+00017c10: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+00017c20: 7374 6428 6d69 746f 7469 635f 7370 6565  std(mitotic_spee
+00017c30: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
+00017c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017c50: 6d69 746f 7469 635f 6d65 616e 5f61 6363  mitotic_mean_acc
+00017c60: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00017c70: 6d69 746f 7469 635f 6163 6329 290d 0a20  mitotic_acc)).. 
+00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c90: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017ca0: 7661 725f 6163 632e 6170 7065 6e64 286e  var_acc.append(n
+00017cb0: 702e 7374 6428 6d69 746f 7469 635f 6163  p.std(mitotic_ac
+00017cc0: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
+00017cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017ce0: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
+00017cf0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00017d00: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00017d10: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+00017d20: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
+00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d40: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00017d50: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00017d60: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
+00017d70: 7464 286d 6974 6f74 6963 5f64 6972 6563  td(mitotic_direc
+00017d80: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+00017d90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017da0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017db0: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
+00017dc0: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00017dd0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+00017de0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00017df0: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+00017e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017e10: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00017e20: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00017e30: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00017e40: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00017e50: 6365 6c6c 5f6d 6173 6b29 290d 0a0d 0a20  cell_mask)).... 
+00017e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e70: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00017e80: 7469 635f 6d65 616e 5f64 6973 705f 7a2e  tic_mean_disp_z.
+00017e90: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00017ea0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017eb0: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+00017ec0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00017ed0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00017ee0: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
+00017ef0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00017f00: 6973 705f 7a29 290d 0a0d 0a20 2020 2020  isp_z))....     
+00017f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017f20: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00017f30: 6d65 616e 5f64 6973 705f 792e 6170 7065  mean_disp_y.appe
+00017f40: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00017f50: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+00017f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017f70: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00017f80: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+00017f90: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00017fa0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017fb0: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
+00017fc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017fd0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00017fe0: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00017ff0: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018000: 6963 5f64 6973 705f 7829 290d 0a20 2020  ic_disp_x))..   
+00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018020: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018030: 635f 7661 725f 6469 7370 5f78 2e61 7070  c_var_disp_x.app
+00018040: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+00018050: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00018060: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018070: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018080: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
+00018090: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
+000180a0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f72  an(non_mitotic_r
+000180b0: 6164 6975 7329 290d 0a20 2020 2020 2020  adius))..       
+000180c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000180d0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+000180e0: 725f 7261 6469 7573 2e61 7070 656e 6428  r_radius.append(
+000180f0: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00018100: 6963 5f72 6164 6975 7329 290d 0a0d 0a20  ic_radius)).... 
+00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018120: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018130: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
+00018140: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018150: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
+00018160: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018170: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018180: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
+00018190: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
+000181a0: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
+000181b0: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
+000181c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000181d0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000181e0: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
+000181f0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00018200: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
+00018210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018220: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00018230: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
+00018240: 6428 6e6f 6e5f 6d69 746f 7469 635f 6163  d(non_mitotic_ac
+00018250: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
+00018260: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018270: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00018280: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018290: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+000182a0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+000182b0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000182c0: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+000182d0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000182e0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+000182f0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018300: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00018310: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
+00018320: 7469 6f6e 616c 5f63 6861 6e67 6529 2920  tional_change)) 
+00018330: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018340: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018350: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00018360: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018370: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018380: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+00018390: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
+000183a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000183b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000183c0: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+000183d0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+000183e0: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+000183f0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00018400: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
+00018410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018420: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018430: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
+00018440: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+00018450: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+00018460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018470: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a2e  .all_var_disp_z.
+00018480: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018490: 6c5f 6469 7370 5f7a 2929 0d0a 0d0a 2020  l_disp_z))....  
+000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184b0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+000184c0: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+000184d0: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f79  .mean(all_disp_y
+000184e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000184f0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018500: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
+00018510: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+00018520: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
+00018530: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018540: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+00018550: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
+00018560: 6e28 616c 6c5f 6469 7370 5f78 2929 0d0a  n(all_disp_x))..
+00018570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018580: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00018590: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+000185a0: 702e 7374 6428 616c 6c5f 6469 7370 5f78  p.std(all_disp_x
+000185b0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000185c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000185d0: 6c6c 5f6d 6561 6e5f 7261 6469 7573 2e61  ll_mean_radius.a
+000185e0: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+000185f0: 6c5f 7261 6469 7573 2929 0d0a 2020 2020  l_radius))..    
+00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018610: 7365 6c66 2e61 6c6c 5f76 6172 5f72 6164  self.all_var_rad
+00018620: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+00018630: 6428 616c 6c5f 7261 6469 7573 2929 0d0a  d(all_radius))..
+00018640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018650: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018660: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
+00018670: 286e 702e 6d65 616e 2861 6c6c 5f73 7065  (np.mean(all_spe
+00018680: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
+00018690: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000186a0: 6c6c 5f76 6172 5f73 7065 6564 2e61 7070  ll_var_speed.app
+000186b0: 656e 6428 6e70 2e73 7464 2861 6c6c 5f73  end(np.std(all_s
+000186c0: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
+000186d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000186e0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 632e  lf.all_mean_acc.
+000186f0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+00018700: 6c6c 5f61 6363 2929 0d0a 2020 2020 2020  ll_acc))..      
+00018710: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018720: 6c66 2e61 6c6c 5f76 6172 5f61 6363 2e61  lf.all_var_acc.a
+00018730: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+00018740: 5f61 6363 2929 0d0a 0d0a 0d0a 0d0a 2020  _acc))........  
+00018750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018760: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00018770: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018780: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
+00018790: 6e28 616c 6c5f 6469 7265 6374 696f 6e61  n(all_directiona
+000187a0: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
+000187b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187c0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6972  self.all_var_dir
+000187d0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+000187e0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+000187f0: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
+00018800: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
+00018810: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018820: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
+00018830: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018840: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018850: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
+00018860: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
+00018870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018880: 2e61 6c6c 5f76 6172 5f64 6973 7461 6e63  .all_var_distanc
+00018890: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+000188a0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+000188b0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000188c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000188f0: 2020 200d 0a64 6566 2062 6f75 6e64 6172     ..def boundar
-00018900: 795f 706f 696e 7473 286d 6173 6b2c 2078  y_points(mask, x
-00018910: 6361 6c69 6272 6174 696f 6e2c 2079 6361  calibration, yca
-00018920: 6c69 6272 6174 696f 6e2c 207a 6361 6c69  libration, zcali
-00018930: 6272 6174 696f 6e29 3a0d 0a0d 0a20 2020  bration):....   
-00018940: 206e 6469 6d20 3d20 6c65 6e28 6d61 736b   ndim = len(mask
-00018950: 2e73 6861 7065 290d 0a20 2020 2074 696d  .shape)..    tim
-00018960: 6564 5f6d 6173 6b20 3d20 7b7d 0d0a 2020  ed_mask = {}..  
-00018970: 2020 6d61 736b 203d 206d 6173 6b20 3e20    mask = mask > 
-00018980: 300d 0a20 2020 206d 6173 6b20 3d20 6d61  0..    mask = ma
-00018990: 736b 2e61 7374 7970 6528 2775 696e 7438  sk.astype('uint8
-000189a0: 2729 0d0a 2020 2020 2320 5958 2073 6861  ')..    # YX sha
-000189b0: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
-000189c0: 6966 206e 6469 6d20 3d3d 2032 3a0d 0a20  if ndim == 2:.. 
-000189d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000189e0: 2062 6f75 6e64 6172 7920 3d20 6669 6e64   boundary = find
-000189f0: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
-00018a00: 290d 0a20 2020 2020 2020 2072 6567 696f  )..        regio
-00018a10: 6e63 656e 7472 6f69 6420 3d20 2830 2c29  ncentroid = (0,)
-00018a20: 202b 2063 6f6d 7075 7465 5f63 656e 7472   + compute_centr
-00018a30: 6f69 6428 626f 756e 6461 7279 2920 0d0a  oid(boundary) ..
-00018a40: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-00018a50: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
-00018a60: 6172 7920 3e20 3029 0d0a 2020 2020 2020  ary > 0)..      
-00018a70: 2020 7265 616c 5f69 6e64 6963 6573 203d    real_indices =
-00018a80: 206e 702e 7472 616e 7370 6f73 6528 6e70   np.transpose(np
-00018a90: 2e61 7361 7272 6179 2869 6e64 6963 6573  .asarray(indices
-00018aa0: 2929 2e63 6f70 7928 290d 0a0d 0a20 2020  )).copy()....   
-00018ab0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-00018ac0: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
-00018ad0: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
-00018ae0: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-00018af0: 6e64 6963 6573 5b6a 5d5b 305d 203d 2072  ndices[j][0] = r
-00018b00: 6561 6c5f 696e 6469 6365 735b 6a5d 5b30  eal_indices[j][0
-00018b10: 5d20 2a20 7963 616c 6962 7261 7469 6f6e  ] * ycalibration
-00018b20: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00018b30: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-00018b40: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-00018b50: 6a5d 5b31 5d20 2a20 7863 616c 6962 7261  j][1] * xcalibra
-00018b60: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
-00018b70: 7472 6565 203d 2073 7061 7469 616c 2e63  tree = spatial.c
-00018b80: 4b44 5472 6565 2872 6561 6c5f 696e 6469  KDTree(real_indi
-00018b90: 6365 7329 0d0a 2020 2020 2020 2020 2320  ces)..        # 
-00018ba0: 5468 6973 206f 626a 6563 7420 636f 6e74  This object cont
-00018bb0: 6169 6e73 206c 6973 7420 6f66 2061 6c6c  ains list of all
-00018bc0: 2074 6865 2070 6f69 6e74 7320 666f 7220   the points for 
-00018bd0: 616c 6c20 7468 6520 6c61 6265 6c73 2069  all the labels i
-00018be0: 6e20 7468 6520 4d61 736b 2069 6d61 6765  n the Mask image
-00018bf0: 2077 6974 6820 7468 6520 6c61 6265 6c20   with the label 
-00018c00: 6964 2061 6e64 2076 6f6c 756d 6520 6f66  id and volume of
-00018c10: 2065 6163 6820 6c61 6265 6c0d 0a20 2020   each label..   
-00018c20: 2020 2020 2074 696d 6564 5f6d 6173 6b5b       timed_mask[
-00018c30: 7374 7228 3029 5d20 3d20 5b74 7265 652c  str(0)] = [tree,
-00018c40: 2069 6e64 6963 6573 2c20 7265 6769 6f6e   indices, region
-00018c50: 6365 6e74 726f 6964 5d0d 0a0d 0a20 2020  centroid]....   
-00018c60: 2023 2054 5958 2073 6861 7065 6420 6f62   # TYX shaped ob
-00018c70: 6a65 6374 0d0a 2020 2020 6966 206e 6469  ject..    if ndi
-00018c80: 6d20 3d3d 2033 3a0d 0a0d 0a0d 0a20 2020  m == 3:......   
-00018c90: 2020 2020 2066 6f72 2069 2069 6e20 7471       for i in tq
-00018ca0: 646d 2872 616e 6765 2830 2c20 6d61 736b  dm(range(0, mask
-00018cb0: 2e73 6861 7065 5b30 5d29 293a 0d0a 2020  .shape[0])):..  
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 626f 756e 6461 7279 203d 2066 696e 645f  boundary = find_
-00018cf0: 626f 756e 6461 7269 6573 286d 6173 6b5b  boundaries(mask[
-00018d00: 692c 3a5d 290d 0a20 2020 2020 2020 2020  i,:])..         
-00018d10: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
-00018d20: 7472 6f69 6420 3d20 2830 2c29 202b 2063  troid = (0,) + c
-00018d30: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
-00018d40: 626f 756e 6461 7279 2920 0d0a 2020 2020  boundary) ..    
-00018d50: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-00018d60: 6365 7320 3d20 6e70 2e77 6865 7265 2862  ces = np.where(b
-00018d70: 6f75 6e64 6172 7920 3e20 3029 0d0a 2020  oundary > 0)..  
-00018d80: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00018d90: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
-00018da0: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
-00018db0: 7272 6179 2869 6e64 6963 6573 2929 2e63  rray(indices)).c
-00018dc0: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
-00018dd0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00018de0: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
-00018df0: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
-00018e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018e10: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00018e20: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
-00018e30: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
-00018e40: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-00018e70: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
-00018e80: 6365 735b 6a5d 5b31 5d20 2a20 7863 616c  ces[j][1] * xcal
-00018e90: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
-00018ea0: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-00018eb0: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-00018ec0: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
-00018ed0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018ee0: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
-00018ef0: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
-00018f00: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
-00018f10: 656e 7472 6f69 645d 0d0a 2020 2020 2020  entroid]..      
-00018f20: 2020 2020 2020 0d0a 2020 2020 2320 545a        ..    # TZ
-00018f30: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
-00018f40: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
-00018f50: 2034 3a0d 0a20 2020 2020 2020 2070 7269   4:..        pri
-00018f60: 6e74 2827 4d61 736b 7320 6d61 6465 2069  nt('Masks made i
-00018f70: 6e74 6f20 6120 3444 2063 796c 696e 6465  nto a 4D cylinde
-00018f80: 722c 2075 7027 290d 0a20 2020 2020 2020  r, up')..       
-00018f90: 2062 6f75 6e64 6172 7920 3d20 6e70 2e7a   boundary = np.z
-00018fa0: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
-00018fb0: 2020 205b 6d61 736b 2e73 6861 7065 5b30     [mask.shape[0
-00018fc0: 5d2c 206d 6173 6b2e 7368 6170 655b 315d  ], mask.shape[1]
-00018fd0: 2c20 6d61 736b 2e73 6861 7065 5b32 5d2c  , mask.shape[2],
-00018fe0: 206d 6173 6b2e 7368 6170 655b 335d 5d0d   mask.shape[3]].
-00018ff0: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-00019000: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00019010: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
-00019020: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
-00019030: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00019040: 2062 6f75 6e64 6172 795b 692c 3a5d 203d   boundary[i,:] =
-00019050: 2066 696e 645f 626f 756e 6461 7269 6573   find_boundaries
-00019060: 286d 6173 6b5b 692c 3a5d 290d 0a20 2020  (mask[i,:])..   
-00019070: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
-00019080: 656e 7472 6f69 6420 3d20 636f 6d70 7574  entroid = comput
-00019090: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
-000190a0: 6172 795b 692c 3a5d 2920 0d0a 2020 2020  ary[i,:]) ..    
-000190b0: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-000190c0: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
-000190d0: 6172 795b 692c 3a5d 203e 2030 290d 0a20  ary[i,:] > 0).. 
-000190e0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-000190f0: 696e 6469 6365 7320 3d20 6e70 2e74 7261  indices = np.tra
-00019100: 6e73 706f 7365 286e 702e 6173 6172 7261  nspose(np.asarra
-00019110: 7928 696e 6469 6365 7329 292e 636f 7079  y(indices)).copy
-00019120: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00019130: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
-00019140: 2830 2c20 6c65 6e28 7265 616c 5f69 6e64  (0, len(real_ind
-00019150: 6963 6573 2929 3a0d 0a0d 0a20 2020 2020  ices)):....     
-00019160: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019170: 6561 6c5f 696e 6469 6365 735b 6a5d 5b30  eal_indices[j][0
-00019180: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
-00019190: 5b6a 5d5b 305d 202a 207a 6361 6c69 6272  [j][0] * zcalibr
-000191a0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-000191b0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-000191c0: 696e 6469 6365 735b 6a5d 5b31 5d20 3d20  indices[j][1] = 
-000191d0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-000191e0: 315d 202a 2079 6361 6c69 6272 6174 696f  1] * ycalibratio
-000191f0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00019200: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00019210: 6365 735b 6a5d 5b32 5d20 3d20 7265 616c  ces[j][2] = real
-00019220: 5f69 6e64 6963 6573 5b6a 5d5b 325d 202a  _indices[j][2] *
-00019230: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
-00019240: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-00019250: 6520 3d20 7370 6174 6961 6c2e 634b 4454  e = spatial.cKDT
-00019260: 7265 6528 7265 616c 5f69 6e64 6963 6573  ree(real_indices
-00019270: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00019280: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
-00019290: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-000192a0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-000192b0: 6964 5d0d 0a20 2020 2070 7269 6e74 2827  id]..    print('
-000192c0: 436f 6d70 7574 6564 2074 6865 2062 6f75  Computed the bou
-000192d0: 6e64 6172 7920 706f 696e 7473 2729 0d0a  ndary points')..
-000192e0: 0d0a 2020 2020 7265 7475 726e 2074 696d  ..    return tim
-000192f0: 6564 5f6d 6173 6b2c 2062 6f75 6e64 6172  ed_mask, boundar
-00019300: 7920 2020 2020 2020 200d 0a0d 0a64 6566  y        ....def
-00019310: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
-00019320: 6428 6269 6e61 7279 5f69 6d61 6765 293a  d(binary_image):
-00019330: 0d0a 2020 2020 2320 456e 7375 7265 2062  ..    # Ensure b
-00019340: 696e 6172 7920 696d 6167 6520 6973 2061  inary image is a
-00019350: 204e 756d 5079 2061 7272 6179 0d0a 2020   NumPy array..  
-00019360: 2020 6269 6e61 7279 5f69 6d61 6765 203d    binary_image =
-00019370: 206e 702e 6172 7261 7928 6269 6e61 7279   np.array(binary
-00019380: 5f69 6d61 6765 290d 0a0d 0a20 2020 2077  _image)....    w
-00019390: 6869 7465 5f70 6978 656c 7320 3d20 6e70  hite_pixels = np
-000193a0: 2e77 6865 7265 2862 696e 6172 795f 696d  .where(binary_im
-000193b0: 6167 6520 3d3d 2031 290d 0a20 2020 206e  age == 1)..    n
-000193c0: 756d 5f70 6978 656c 7320 3d20 6c65 6e28  um_pixels = len(
-000193d0: 7768 6974 655f 7069 7865 6c73 5b30 5d29  white_pixels[0])
-000193e0: 0d0a 0d0a 2020 2020 2320 436f 6d70 7574  ....    # Comput
-000193f0: 6520 7468 6520 6365 6e74 726f 6964 206f  e the centroid o
-00019400: 6620 7468 6520 7768 6974 6520 7069 7865  f the white pixe
-00019410: 6c73 2069 6e20 7468 6520 626f 756e 6461  ls in the bounda
-00019420: 7279 2069 6d61 6765 0d0a 2020 2020 6365  ry image..    ce
-00019430: 6e74 726f 6964 203d 206e 702e 7a65 726f  ntroid = np.zero
-00019440: 7328 6269 6e61 7279 5f69 6d61 6765 2e6e  s(binary_image.n
-00019450: 6469 6d29 0d0a 2020 2020 666f 7220 6469  dim)..    for di
-00019460: 6d20 696e 2072 616e 6765 2862 696e 6172  m in range(binar
-00019470: 795f 696d 6167 652e 6e64 696d 293a 0d0a  y_image.ndim):..
-00019480: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-00019490: 5b64 696d 5d20 3d20 7768 6974 655f 7069  [dim] = white_pi
-000194a0: 7865 6c73 5b64 696d 5d2e 7375 6d28 2920  xels[dim].sum() 
-000194b0: 2f20 6e75 6d5f 7069 7865 6c73 0d0a 0d0a  / num_pixels....
-000194c0: 2020 2020 7265 7475 726e 2063 656e 7472      return centr
-000194d0: 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a  oid........ ....
-000194e0: 6465 6620 6765 745f 6373 765f 6461 7461  def get_csv_data
-000194f0: 2863 7376 293a 0d0a 0d0a 2020 2020 2020  (csv):....      
-00019500: 2020 6461 7461 7365 7420 3d20 7064 2e72    dataset = pd.r
-00019510: 6561 645f 6373 7628 0d0a 2020 2020 2020  ead_csv(..      
-00019520: 2020 2020 2020 6373 762c 2064 656c 696d        csv, delim
-00019530: 6974 6572 3d22 2c22 2c20 656e 636f 6469  iter=",", encodi
-00019540: 6e67 3d22 756e 6963 6f64 655f 6573 6361  ng="unicode_esca
-00019550: 7065 222c 206c 6f77 5f6d 656d 6f72 793d  pe", low_memory=
-00019560: 4661 6c73 650d 0a20 2020 2020 2020 2029  False..        )
-00019570: 5b33 3a5d 0d0a 2020 2020 2020 2020 6461  [3:]..        da
-00019580: 7461 7365 745f 696e 6465 7820 3d20 6461  taset_index = da
-00019590: 7461 7365 742e 696e 6465 780d 0a20 2020  taset.index..   
-000195a0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-000195b0: 7365 742c 2064 6174 6173 6574 5f69 6e64  set, dataset_ind
-000195c0: 6578 0d0a 2020 2020 0d0a 6465 6620 6765  ex..    ..def ge
-000195d0: 745f 7370 6f74 5f64 6174 6173 6574 2873  t_spot_dataset(s
-000195e0: 706f 745f 6461 7461 7365 742c 2074 7261  pot_dataset, tra
-000195f0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-00019600: 5f6b 6579 732c 2078 6361 6c69 6272 6174  _keys, xcalibrat
-00019610: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
-00019620: 6e2c 207a 6361 6c69 6272 6174 696f 6e2c  n, zcalibration,
-00019630: 2041 7474 7269 6275 7465 426f 786e 616d   AttributeBoxnam
-00019640: 652c 2064 6574 6563 7469 6f6e 6368 616e  e, detectionchan
-00019650: 6e65 6c29 3a0d 0a20 2020 2020 2020 2041  nel):..        A
-00019660: 6c6c 5661 6c75 6573 203d 207b 7d0d 0a20  llValues = {}.. 
-00019670: 2020 2020 2020 2070 6f73 6978 203d 2074         posix = t
-00019680: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019690: 6f74 5f6b 6579 735b 2270 6f73 6978 225d  ot_keys["posix"]
-000196a0: 0d0a 2020 2020 2020 2020 706f 7369 7920  ..        posiy 
-000196b0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-000196c0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
-000196d0: 7922 5d0d 0a20 2020 2020 2020 2070 6f73  y"]..        pos
-000196e0: 697a 203d 2074 7261 636b 5f61 6e61 6c79  iz = track_analy
-000196f0: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
-00019700: 6f73 697a 225d 0d0a 2020 2020 2020 2020  osiz"]..        
-00019710: 6672 616d 6520 3d20 7472 6163 6b5f 616e  frame = track_an
-00019720: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019730: 5b22 6672 616d 6522 5d0d 0a20 2020 2020  ["frame"]..     
-00019740: 2020 200d 0a20 2020 2020 2020 204c 6f63     ..        Loc
-00019750: 6174 696f 6e58 203d 2028 0d0a 2020 2020  ationX = (..    
-00019760: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
-00019770: 6173 6574 5b70 6f73 6978 5d2e 6173 7479  aset[posix].asty
-00019780: 7065 2822 666c 6f61 7422 2920 2f20 7863  pe("float") / xc
-00019790: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-000197a0: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
-000197b0: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
-000197c0: 6174 696f 6e59 203d 2028 0d0a 2020 2020  ationY = (..    
-000197d0: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
-000197e0: 6173 6574 5b70 6f73 6979 5d2e 6173 7479  aset[posiy].asty
-000197f0: 7065 2822 666c 6f61 7422 2920 2f20 7963  pe("float") / yc
-00019800: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019810: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
-00019820: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
-00019830: 6174 696f 6e5a 203d 2028 0d0a 2020 2020  ationZ = (..    
-00019840: 2020 2020 2020 2020 7370 6f74 5f64 6174          spot_dat
-00019850: 6173 6574 5b70 6f73 697a 5d2e 6173 7479  aset[posiz].asty
-00019860: 7065 2822 666c 6f61 7422 2920 2f20 7a63  pe("float") / zc
-00019870: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019880: 2020 2020 292e 6173 7479 7065 2822 696e      ).astype("in
-00019890: 7422 290d 0a20 2020 2020 2020 204c 6f63  t")..        Loc
-000198a0: 6174 696f 6e54 203d 2028 7370 6f74 5f64  ationT = (spot_d
-000198b0: 6174 6173 6574 5b66 7261 6d65 5d2e 6173  ataset[frame].as
-000198c0: 7479 7065 2822 666c 6f61 7422 2929 2e61  type("float")).a
-000198d0: 7374 7970 6528 2269 6e74 2229 0d0a 2020  stype("int")..  
-000198e0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-000198f0: 2020 6967 6e6f 7265 5f76 616c 7565 7320    ignore_values 
-00019900: 3d20 5b74 7261 636b 5f61 6e61 6c79 7369  = [track_analysi
-00019910: 735f 7370 6f74 5f6b 6579 735b 226d 6561  s_spot_keys["mea
-00019920: 6e5f 696e 7465 6e73 6974 7922 5d2c 7472  n_intensity"],tr
-00019930: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019940: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
-00019950: 7465 6e73 6974 7922 5d5d 200d 0a20 2020  tensity"]] ..   
-00019960: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-00019970: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
-00019980: 5f73 706f 745f 6b65 7973 2e69 7465 6d73  _spot_keys.items
-00019990: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-000199a0: 2020 2020 2020 2069 6620 6465 7465 6374         if detect
-000199b0: 696f 6e63 6861 6e6e 656c 203d 3d20 313a  ionchannel == 1:
-000199c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000199d0: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
-000199e0: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
-000199f0: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
-00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a10: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
-00019a20: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019a30: 735b 226d 6561 6e5f 696e 7465 6e73 6974  s["mean_intensit
-00019a40: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
-00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a60: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
-00019a70: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
-00019a80: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-00019a90: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00019aa0: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
-00019ab0: 2022 746f 7461 6c5f 696e 7465 6e73 6974   "total_intensit
-00019ac0: 795f 6368 3222 3a0d 0a20 2020 2020 2020  y_ch2":..       
-00019ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ae0: 2020 2020 7661 6c75 6520 3d20 7472 6163      value = trac
-00019af0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-00019b00: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
-00019b10: 6e73 6974 7922 5d0d 0a20 2020 2020 2020  nsity"]..       
-00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b30: 2020 2020 416c 6c56 616c 7565 735b 7661      AllValues[va
-00019b40: 6c75 655d 203d 2073 706f 745f 6461 7461  lue] = spot_data
-00019b50: 7365 745b 765d 2e61 7374 7970 6528 2266  set[v].astype("f
-00019b60: 6c6f 6174 2229 2020 2020 2020 200d 0a0d  loat")       ...
-00019b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019b80: 2069 6620 7620 6e6f 7420 696e 2069 676e   if v not in ign
-00019b90: 6f72 655f 7661 6c75 6573 3a0d 0a20 2020  ore_values:..   
-00019ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bb0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00019bc0: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-00019bd0: 5661 6c75 6573 5b76 5d20 3d20 7370 6f74  Values[v] = spot
-00019be0: 5f64 6174 6173 6574 5b76 5d2e 6173 7479  _dataset[v].asty
-00019bf0: 7065 2822 666c 6f61 7422 290d 0a0d 0a20  pe("float").... 
-00019c00: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-00019c10: 5b70 6f73 6978 5d20 3d20 726f 756e 6428  [posix] = round(
-00019c20: 4c6f 6361 7469 6f6e 582c 3329 0d0a 2020  LocationX,3)..  
-00019c30: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-00019c40: 706f 7369 795d 203d 2072 6f75 6e64 284c  posiy] = round(L
-00019c50: 6f63 6174 696f 6e59 2c33 290d 0a20 2020  ocationY,3)..   
-00019c60: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
-00019c70: 6f73 697a 5d20 3d20 726f 756e 6428 4c6f  osiz] = round(Lo
-00019c80: 6361 7469 6f6e 5a2c 3329 0d0a 2020 2020  cationZ,3)..    
-00019c90: 2020 2020 416c 6c56 616c 7565 735b 6672      AllValues[fr
-00019ca0: 616d 655d 203d 2072 6f75 6e64 284c 6f63  ame] = round(Loc
-00019cb0: 6174 696f 6e54 2c33 290d 0a20 2020 2020  ationT,3)..     
-00019cc0: 2020 2041 7474 7269 6275 7465 6964 7320     Attributeids 
-00019cd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 4174  = []..        At
-00019ce0: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
-00019cf0: 6428 4174 7472 6962 7574 6542 6f78 6e61  d(AttributeBoxna
-00019d00: 6d65 290d 0a20 2020 2020 2020 2066 6f72  me)..        for
-00019d10: 2061 7474 7269 6275 7465 6e61 6d65 2069   attributename i
-00019d20: 6e20 416c 6c56 616c 7565 732e 6b65 7973  n AllValues.keys
-00019d30: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00019d40: 2020 2041 7474 7269 6275 7465 6964 732e     Attributeids.
-00019d50: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
-00019d60: 6e61 6d65 2920 2020 200d 0a20 2020 2020  name)    ..     
-00019d70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00019d80: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-00019d90: 6e20 4174 7472 6962 7574 6569 6473 2c20  n Attributeids, 
-00019da0: 416c 6c56 616c 7565 7320 2020 2020 0d0a  AllValues     ..
-00019db0: 2020 2020 0d0a 6465 6620 6765 745f 7472      ..def get_tr
-00019dc0: 6163 6b5f 6461 7461 7365 7428 7472 6163  ack_dataset(trac
-00019dd0: 6b5f 6461 7461 7365 742c 2074 7261 636b  k_dataset, track
-00019de0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019df0: 6579 732c 2074 7261 636b 5f61 6e61 6c79  eys, track_analy
-00019e00: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
-00019e10: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
-00019e20: 786e 616d 6529 3a0d 0a0d 0a20 2020 2020  xname):....     
-00019e30: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-00019e40: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-00019e50: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
-00019e60: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019e70: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
-00019e80: 0a20 2020 2020 2020 2054 6964 203d 2074  .        Tid = t
-00019e90: 7261 636b 5f64 6174 6173 6574 5b74 7261  rack_dataset[tra
-00019ea0: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
-00019eb0: 6c6f 6174 2229 0d0a 2020 2020 2020 200d  loat")..       .
-00019ec0: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
-00019ed0: 6b56 616c 7565 735b 7472 6163 6b5f 6964  kValues[track_id
-00019ee0: 5d20 3d20 5469 640d 0a20 2020 2020 200d  ] = Tid..      .
-00019ef0: 0a20 2020 2020 2020 2066 6f72 2028 6b2c  .        for (k,
-00019f00: 2076 2920 696e 2074 7261 636b 5f61 6e61   v) in track_ana
-00019f10: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
-00019f20: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
-00019f30: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-00019f40: 2074 7261 636b 5f64 6174 6173 6574 5b76   track_dataset[v
-00019f50: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-00019f60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019f70: 2020 206d 696e 7661 6c20 3d20 6d69 6e28     minval = min(
-00019f80: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-00019f90: 2020 2020 6d61 7876 616c 203d 206d 6178      maxval = max
-00019fa0: 2878 290d 0a0d 0a20 2020 2020 2020 2020  (x)....         
-00019fb0: 2020 2020 2020 2069 6620 6d69 6e76 616c         if minval
-00019fc0: 203e 2030 2061 6e64 206d 6178 7661 6c20   > 0 and maxval 
-00019fd0: 3c3d 2031 3a0d 0a0d 0a20 2020 2020 2020  <= 1:....       
-00019fe0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
-00019ff0: 2078 202b 2031 0d0a 0d0a 2020 2020 2020   x + 1....      
-0001a000: 2020 2020 2020 2020 2020 416c 6c54 7261            AllTra
-0001a010: 636b 5661 6c75 6573 5b6b 5d20 3d20 726f  ckValues[k] = ro
-0001a020: 756e 6428 782c 2033 290d 0a0d 0a20 2020  und(x, 3)....   
-0001a030: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001a040: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
-0001a050: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001a060: 7574 6569 6473 2e61 7070 656e 6428 5472  uteids.append(Tr
-0001a070: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
-0001a080: 616d 6529 0d0a 2020 2020 2020 2020 666f  ame)..        fo
-0001a090: 7220 6174 7472 6962 7574 656e 616d 6520  r attributename 
-0001a0a0: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001a0b0: 735f 7472 6163 6b5f 6b65 7973 2e6b 6579  s_track_keys.key
-0001a0c0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-0001a0d0: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
-0001a0e0: 6964 732e 6170 7065 6e64 2861 7474 7269  ids.append(attri
-0001a0f0: 6275 7465 6e61 6d65 2920 2020 200d 0a20  butename)    .. 
-0001a100: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001a110: 7572 6e20 5472 6163 6b41 7474 7269 6275  urn TrackAttribu
-0001a120: 7465 6964 732c 2041 6c6c 5472 6163 6b56  teids, AllTrackV
-0001a130: 616c 7565 730d 0a20 2020 200d 0a64 6566  alues..    ..def
-0001a140: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
-0001a150: 6574 2865 6467 6573 5f64 6174 6173 6574  et(edges_dataset
-0001a160: 2c20 6564 6765 735f 6461 7461 7365 745f  , edges_dataset_
-0001a170: 696e 6465 782c 2074 7261 636b 5f61 6e61  index, track_ana
-0001a180: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001a190: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a1a0: 6564 6765 735f 6b65 7973 293a 0d0a 0d0a  edges_keys):....
-0001a1b0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001a1c0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
-0001a1d0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-0001a1e0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a1f0: 706f 745f 6b65 7973 5b22 7472 6163 6b5f  pot_keys["track_
-0001a200: 6964 225d 0d0a 2020 2020 2020 2020 5469  id"]..        Ti
-0001a210: 6420 3d20 6564 6765 735f 6461 7461 7365  d = edges_datase
-0001a220: 745b 7472 6163 6b5f 6964 5d2e 6173 7479  t[track_id].asty
-0001a230: 7065 2822 666c 6f61 7422 290d 0a20 2020  pe("float")..   
-0001a240: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-0001a250: 702e 7768 6572 6528 5469 6420 3d3d 2030  p.where(Tid == 0
-0001a260: 290d 0a20 2020 2020 2020 206d 6178 7472  )..        maxtr
-0001a270: 6163 6b5f 6964 203d 206d 6178 2854 6964  ack_id = max(Tid
-0001a280: 290d 0a20 2020 2020 2020 2063 6f6e 6469  )..        condi
-0001a290: 7469 6f6e 5f69 6e64 6963 6573 203d 2065  tion_indices = e
-0001a2a0: 6467 6573 5f64 6174 6173 6574 5f69 6e64  dges_dataset_ind
-0001a2b0: 6578 5b69 6e64 6963 6573 5d0d 0a20 2020  ex[indices]..   
-0001a2c0: 2020 2020 2054 6964 5b63 6f6e 6469 7469       Tid[conditi
-0001a2d0: 6f6e 5f69 6e64 6963 6573 5d20 3d20 6d61  on_indices] = ma
-0001a2e0: 7874 7261 636b 5f69 6420 2b20 310d 0a20  xtrack_id + 1.. 
-0001a2f0: 2020 2020 2020 2041 6c6c 4564 6765 7356         AllEdgesV
-0001a300: 616c 7565 735b 7472 6163 6b5f 6964 5d20  alues[track_id] 
-0001a310: 3d20 5469 640d 0a0d 0a20 2020 2020 2020  = Tid....       
-0001a320: 2066 6f72 206b 2069 6e20 7472 6163 6b5f   for k in track_
-0001a330: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-0001a340: 6579 732e 7661 6c75 6573 2829 3a0d 0a0d  eys.values():...
-0001a350: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a360: 6b20 213d 2074 7261 636b 5f69 643a 0d0a  k != track_id:..
-0001a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a380: 7820 3d20 6564 6765 735f 6461 7461 7365  x = edges_datase
-0001a390: 745b 6b5d 2e61 7374 7970 6528 2266 6c6f  t[k].astype("flo
-0001a3a0: 6174 2229 0d0a 0d0a 2020 2020 2020 2020  at")....        
-0001a3b0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001a3c0: 5661 6c75 6573 5b6b 5d20 3d20 7820 2020  Values[k] = x   
-0001a3d0: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-0001a3e0: 2020 2020 2072 6574 7572 6e20 416c 6c45       return AllE
-0001a3f0: 6467 6573 5661 6c75 6573 2020 200d 0a20  dgesValues   .. 
-0001a400: 2020 200d 0a20 2020 2020 2020 0d0a 2020     ..       ..  
-0001a410: 2020 0d0a 6465 6620 7363 616c 655f 7661    ..def scale_va
-0001a420: 6c75 6528 782c 2073 6361 6c65 203d 2032  lue(x, scale = 2
-0001a430: 3535 202a 2032 3535 293a 0d0a 0d0a 0d0a  55 * 255):......
-0001a440: 2020 2020 2072 6574 7572 6e20 7820 2a20       return x * 
-0001a450: 7363 616c 6520 2020 0d0a 2020 2020 0d0a  scale   ..    ..
-0001a460: 0d0a 0d0a 6465 6620 7072 6f62 5f73 6967  ....def prob_sig
-0001a470: 6d6f 6964 2878 293a 0d0a 2020 2020 7265  moid(x):..    re
-0001a480: 7475 726e 2031 202d 206d 6174 682e 6578  turn 1 - math.ex
-0001a490: 7028 2d78 290d 0a0d 0a0d 0a64 6566 2061  p(-x)......def a
-0001a4a0: 6e67 756c 6172 5f63 6861 6e67 6528 7665  ngular_change(ve
-0001a4b0: 635f 302c 2076 6563 5f31 293a 0d0a 2020  c_0, vec_1):..  
-0001a4c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a4d0: 7665 635f 3020 3d20 7665 635f 3020 2f20  vec_0 = vec_0 / 
-0001a4e0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
-0001a4f0: 6563 5f30 290d 0a20 2020 2020 2020 2076  ec_0)..        v
-0001a500: 6563 5f31 203d 2076 6563 5f31 202f 206e  ec_1 = vec_1 / n
-0001a510: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7665  p.linalg.norm(ve
-0001a520: 635f 3129 0d0a 2020 2020 2020 2020 616e  c_1)..        an
-0001a530: 676c 6520 3d20 6e70 2e61 7263 636f 7328  gle = np.arccos(
-0001a540: 6e70 2e63 6c69 7028 6e70 2e64 6f74 2876  np.clip(np.dot(v
-0001a550: 6563 5f30 2c20 7665 635f 3129 2c20 2d31  ec_0, vec_1), -1
-0001a560: 2e30 2c20 312e 3029 290d 0a20 2020 2020  .0, 1.0))..     
-0001a570: 2020 2061 6e67 6c65 203d 2061 6e67 6c65     angle = angle
-0001a580: 202a 2031 3830 202f 206e 702e 7069 0d0a   * 180 / np.pi..
-0001a590: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0001a5a0: 6e67 6c65 0d0a 2020 2020 200d 0a0d 0a64  ngle..     ....d
-0001a5b0: 6566 2065 7661 6c5f 626f 6f6c 2876 616c  ef eval_bool(val
-0001a5c0: 7565 293a 0d0a 2020 2020 2020 2020 2020  ue):..          
-0001a5d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001a5e0: 2020 6966 2076 616c 7565 2020 3d3d 2027    if value  == '
-0001a5f0: 5472 7565 273a 200d 0a20 2020 2020 2020  True': ..       
-0001a600: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
-0001a610: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
-0001a620: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001a630: 2020 2020 2020 2020 6469 765f 6b65 7920          div_key 
-0001a640: 3d20 4661 6c73 6520 0d0a 0d0a 2020 2020  = False ....    
-0001a650: 2020 2020 7265 7475 726e 2064 6976 5f6b      return div_k
-0001a660: 6579 2020 2020 2020 2020 2020 2020 2020  ey              
-0001a670: 2020 0d0a 0d0a 6465 6620 6368 6563 6b5f    ....def check_
-0001a680: 616e 645f 7570 6461 7465 5f6d 6173 6b28  and_update_mask(
-0001a690: 6d61 736b 2c69 6d61 6765 293a 0d0a 2020  mask,image):..  
-0001a6a0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-0001a6b0: 6620 6c65 6e28 6d61 736b 2e73 6861 7065  f len(mask.shape
-0001a6c0: 2920 3c20 6c65 6e28 696d 6167 652e 7368  ) < len(image.sh
-0001a6d0: 6170 6529 3a0d 0a20 2020 2020 2020 2020  ape):..         
-0001a6e0: 2020 2075 7064 6174 655f 6d61 736b 203d     update_mask =
-0001a6f0: 206e 702e 7a65 726f 7328 0d0a 2020 2020   np.zeros(..    
-0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a710: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
+000188e0: 0d0a 2020 2020 2020 2020 0d0a 6465 6620  ..        ..def 
+000188f0: 626f 756e 6461 7279 5f70 6f69 6e74 7328  boundary_points(
+00018900: 6d61 736b 2c20 7863 616c 6962 7261 7469  mask, xcalibrati
+00018910: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
+00018920: 2c20 7a63 616c 6962 7261 7469 6f6e 293a  , zcalibration):
+00018930: 0d0a 0d0a 2020 2020 6e64 696d 203d 206c  ....    ndim = l
+00018940: 656e 286d 6173 6b2e 7368 6170 6529 0d0a  en(mask.shape)..
+00018950: 2020 2020 7469 6d65 645f 6d61 736b 203d      timed_mask =
+00018960: 207b 7d0d 0a20 2020 206d 6173 6b20 3d20   {}..    mask = 
+00018970: 6d61 736b 203e 2030 0d0a 2020 2020 6d61  mask > 0..    ma
+00018980: 736b 203d 206d 6173 6b2e 6173 7479 7065  sk = mask.astype
+00018990: 2827 7569 6e74 3827 290d 0a20 2020 2023  ('uint8')..    #
+000189a0: 2059 5820 7368 6170 6564 206f 626a 6563   YX shaped objec
+000189b0: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
+000189c0: 3d20 323a 0d0a 2020 2020 2020 2020 0d0a  = 2:..        ..
+000189d0: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
+000189e0: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
+000189f0: 6573 286d 6173 6b29 0d0a 2020 2020 2020  es(mask)..      
+00018a00: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
+00018a10: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
+00018a20: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
+00018a30: 6172 7929 200d 0a20 2020 2020 2020 2069  ary) ..        i
+00018a40: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
+00018a50: 6528 626f 756e 6461 7279 203e 2030 290d  e(boundary > 0).
+00018a60: 0a20 2020 2020 2020 2072 6561 6c5f 696e  .        real_in
+00018a70: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
+00018a80: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
+00018a90: 696e 6469 6365 7329 292e 636f 7079 2829  indices)).copy()
+00018aa0: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+00018ab0: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
+00018ac0: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
+00018ad0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00018ae0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00018af0: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+00018b00: 6573 5b6a 5d5b 305d 202a 2079 6361 6c69  es[j][0] * ycali
+00018b10: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00018b20: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00018b30: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
+00018b40: 6e64 6963 6573 5b6a 5d5b 315d 202a 2078  ndices[j][1] * x
+00018b50: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+00018b60: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
+00018b70: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
+00018b80: 616c 5f69 6e64 6963 6573 290d 0a20 2020  al_indices)..   
+00018b90: 2020 2020 2023 2054 6869 7320 6f62 6a65       # This obje
+00018ba0: 6374 2063 6f6e 7461 696e 7320 6c69 7374  ct contains list
+00018bb0: 206f 6620 616c 6c20 7468 6520 706f 696e   of all the poin
+00018bc0: 7473 2066 6f72 2061 6c6c 2074 6865 206c  ts for all the l
+00018bd0: 6162 656c 7320 696e 2074 6865 204d 6173  abels in the Mas
+00018be0: 6b20 696d 6167 6520 7769 7468 2074 6865  k image with the
+00018bf0: 206c 6162 656c 2069 6420 616e 6420 766f   label id and vo
+00018c00: 6c75 6d65 206f 6620 6561 6368 206c 6162  lume of each lab
+00018c10: 656c 0d0a 2020 2020 2020 2020 7469 6d65  el..        time
+00018c20: 645f 6d61 736b 5b73 7472 2830 295d 203d  d_mask[str(0)] =
+00018c30: 205b 7472 6565 2c20 696e 6469 6365 732c   [tree, indices,
+00018c40: 2072 6567 696f 6e63 656e 7472 6f69 645d   regioncentroid]
+00018c50: 0d0a 0d0a 2020 2020 2320 5459 5820 7368  ....    # TYX sh
+00018c60: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
+00018c70: 2069 6620 6e64 696d 203d 3d20 333a 0d0a   if ndim == 3:..
+00018c80: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+00018c90: 6920 696e 2074 7164 6d28 7261 6e67 6528  i in tqdm(range(
+00018ca0: 302c 206d 6173 6b2e 7368 6170 655b 305d  0, mask.shape[0]
+00018cb0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00018cc0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00018cd0: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
+00018ce0: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
+00018cf0: 7328 6d61 736b 5b69 2c3a 5d29 0d0a 2020  s(mask[i,:])..  
+00018d00: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00018d10: 6769 6f6e 6365 6e74 726f 6964 203d 2028  gioncentroid = (
+00018d20: 302c 2920 2b20 636f 6d70 7574 655f 6365  0,) + compute_ce
+00018d30: 6e74 726f 6964 2862 6f75 6e64 6172 7929  ntroid(boundary)
+00018d40: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00018d50: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+00018d60: 7768 6572 6528 626f 756e 6461 7279 203e  where(boundary >
+00018d70: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+00018d80: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00018d90: 7320 3d20 6e70 2e74 7261 6e73 706f 7365  s = np.transpose
+00018da0: 286e 702e 6173 6172 7261 7928 696e 6469  (np.asarray(indi
+00018db0: 6365 7329 292e 636f 7079 2829 0d0a 0d0a  ces)).copy()....
+00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018dd0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+00018de0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
+00018df0: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
+00018e00: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00018e10: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00018e20: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00018e30: 5d5b 305d 202a 2079 6361 6c69 6272 6174  ][0] * ycalibrat
+00018e40: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00018e50: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00018e60: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
+00018e70: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+00018e80: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
+00018e90: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018ea0: 2020 2074 7265 6520 3d20 7370 6174 6961     tree = spatia
+00018eb0: 6c2e 634b 4454 7265 6528 7265 616c 5f69  l.cKDTree(real_i
+00018ec0: 6e64 6963 6573 290d 0a0d 0a20 2020 2020  ndices)....     
+00018ed0: 2020 2020 2020 2020 2020 2074 696d 6564             timed
+00018ee0: 5f6d 6173 6b5b 7374 7228 6929 5d20 3d20  _mask[str(i)] = 
+00018ef0: 5b74 7265 652c 2069 6e64 6963 6573 2c20  [tree, indices, 
+00018f00: 7265 6769 6f6e 6365 6e74 726f 6964 5d0d  regioncentroid].
+00018f10: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00018f20: 2020 2023 2054 5a59 5820 7368 6170 6564     # TZYX shaped
+00018f30: 206f 626a 6563 740d 0a20 2020 2069 6620   object..    if 
+00018f40: 6e64 696d 203d 3d20 343a 0d0a 2020 2020  ndim == 4:..    
+00018f50: 2020 2020 7072 696e 7428 274d 6173 6b73      print('Masks
+00018f60: 206d 6164 6520 696e 746f 2061 2034 4420   made into a 4D 
+00018f70: 6379 6c69 6e64 6572 2c20 7570 2729 0d0a  cylinder, up')..
+00018f80: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
+00018f90: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
+00018fa0: 2020 2020 2020 2020 2020 5b6d 6173 6b2e            [mask.
+00018fb0: 7368 6170 655b 305d 2c20 6d61 736b 2e73  shape[0], mask.s
+00018fc0: 6861 7065 5b31 5d2c 206d 6173 6b2e 7368  hape[1], mask.sh
+00018fd0: 6170 655b 325d 2c20 6d61 736b 2e73 6861  ape[2], mask.sha
+00018fe0: 7065 5b33 5d5d 0d0a 2020 2020 2020 2020  pe[3]]..        
+00018ff0: 290d 0a20 2020 2020 2020 2066 6f72 2069  )..        for i
+00019000: 2069 6e20 7261 6e67 6528 302c 206d 6173   in range(0, mas
+00019010: 6b2e 7368 6170 655b 305d 293a 0d0a 2020  k.shape[0]):..  
+00019020: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00019030: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
+00019040: 5b69 2c3a 5d20 3d20 6669 6e64 5f62 6f75  [i,:] = find_bou
+00019050: 6e64 6172 6965 7328 6d61 736b 5b69 2c3a  ndaries(mask[i,:
+00019060: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00019070: 7265 6769 6f6e 6365 6e74 726f 6964 203d  regioncentroid =
+00019080: 2063 6f6d 7075 7465 5f63 656e 7472 6f69   compute_centroi
+00019090: 6428 626f 756e 6461 7279 5b69 2c3a 5d29  d(boundary[i,:])
+000190a0: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
+000190b0: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
+000190c0: 6528 626f 756e 6461 7279 5b69 2c3a 5d20  e(boundary[i,:] 
+000190d0: 3e20 3029 0d0a 2020 2020 2020 2020 2020  > 0)..          
+000190e0: 2020 7265 616c 5f69 6e64 6963 6573 203d    real_indices =
+000190f0: 206e 702e 7472 616e 7370 6f73 6528 6e70   np.transpose(np
+00019100: 2e61 7361 7272 6179 2869 6e64 6963 6573  .asarray(indices
+00019110: 2929 2e63 6f70 7928 290d 0a0d 0a20 2020  )).copy()....   
+00019120: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00019130: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+00019140: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
+00019150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019160: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+00019170: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
+00019180: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
+00019190: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191b0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+000191c0: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
+000191d0: 6365 735b 6a5d 5b31 5d20 2a20 7963 616c  ces[j][1] * ycal
+000191e0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+000191f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00019200: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
+00019210: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+00019220: 6a5d 5b32 5d20 2a20 7863 616c 6962 7261  j][2] * xcalibra
+00019230: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00019240: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
+00019250: 616c 2e63 4b44 5472 6565 2872 6561 6c5f  al.cKDTree(real_
+00019260: 696e 6469 6365 7329 0d0a 2020 2020 2020  indices)..      
+00019270: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
+00019280: 5b73 7472 2869 295d 203d 205b 7472 6565  [str(i)] = [tree
+00019290: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
+000192a0: 6e63 656e 7472 6f69 645d 0d0a 2020 2020  ncentroid]..    
+000192b0: 7072 696e 7428 2743 6f6d 7075 7465 6420  print('Computed 
+000192c0: 7468 6520 626f 756e 6461 7279 2070 6f69  the boundary poi
+000192d0: 6e74 7327 290d 0a0d 0a20 2020 2072 6574  nts')....    ret
+000192e0: 7572 6e20 7469 6d65 645f 6d61 736b 2c20  urn timed_mask, 
+000192f0: 626f 756e 6461 7279 2020 2020 2020 2020  boundary        
+00019300: 0d0a 0d0a 6465 6620 636f 6d70 7574 655f  ....def compute_
+00019310: 6365 6e74 726f 6964 2862 696e 6172 795f  centroid(binary_
+00019320: 696d 6167 6529 3a0d 0a20 2020 2023 2045  image):..    # E
+00019330: 6e73 7572 6520 6269 6e61 7279 2069 6d61  nsure binary ima
+00019340: 6765 2069 7320 6120 4e75 6d50 7920 6172  ge is a NumPy ar
+00019350: 7261 790d 0a20 2020 2062 696e 6172 795f  ray..    binary_
+00019360: 696d 6167 6520 3d20 6e70 2e61 7272 6179  image = np.array
+00019370: 2862 696e 6172 795f 696d 6167 6529 0d0a  (binary_image)..
+00019380: 0d0a 2020 2020 7768 6974 655f 7069 7865  ..    white_pixe
+00019390: 6c73 203d 206e 702e 7768 6572 6528 6269  ls = np.where(bi
+000193a0: 6e61 7279 5f69 6d61 6765 203d 3d20 3129  nary_image == 1)
+000193b0: 0d0a 2020 2020 6e75 6d5f 7069 7865 6c73  ..    num_pixels
+000193c0: 203d 206c 656e 2877 6869 7465 5f70 6978   = len(white_pix
+000193d0: 656c 735b 305d 290d 0a0d 0a20 2020 2023  els[0])....    #
+000193e0: 2043 6f6d 7075 7465 2074 6865 2063 656e   Compute the cen
+000193f0: 7472 6f69 6420 6f66 2074 6865 2077 6869  troid of the whi
+00019400: 7465 2070 6978 656c 7320 696e 2074 6865  te pixels in the
+00019410: 2062 6f75 6e64 6172 7920 696d 6167 650d   boundary image.
+00019420: 0a20 2020 2063 656e 7472 6f69 6420 3d20  .    centroid = 
+00019430: 6e70 2e7a 6572 6f73 2862 696e 6172 795f  np.zeros(binary_
+00019440: 696d 6167 652e 6e64 696d 290d 0a20 2020  image.ndim)..   
+00019450: 2066 6f72 2064 696d 2069 6e20 7261 6e67   for dim in rang
+00019460: 6528 6269 6e61 7279 5f69 6d61 6765 2e6e  e(binary_image.n
+00019470: 6469 6d29 3a0d 0a20 2020 2020 2020 2063  dim):..        c
+00019480: 656e 7472 6f69 645b 6469 6d5d 203d 2077  entroid[dim] = w
+00019490: 6869 7465 5f70 6978 656c 735b 6469 6d5d  hite_pixels[dim]
+000194a0: 2e73 756d 2829 202f 206e 756d 5f70 6978  .sum() / num_pix
+000194b0: 656c 730d 0a0d 0a20 2020 2072 6574 7572  els....    retur
+000194c0: 6e20 6365 6e74 726f 6964 0d0a 0d0a 0d0a  n centroid......
+000194d0: 0d0a 200d 0a0d 0a64 6566 2067 6574 5f63  .. ....def get_c
+000194e0: 7376 5f64 6174 6128 6373 7629 3a0d 0a0d  sv_data(csv):...
+000194f0: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
+00019500: 203d 2070 642e 7265 6164 5f63 7376 280d   = pd.read_csv(.
+00019510: 0a20 2020 2020 2020 2020 2020 2063 7376  .            csv
+00019520: 2c20 6465 6c69 6d69 7465 723d 222c 222c  , delimiter=",",
+00019530: 2065 6e63 6f64 696e 673d 2275 6e69 636f   encoding="unico
+00019540: 6465 5f65 7363 6170 6522 2c20 6c6f 775f  de_escape", low_
+00019550: 6d65 6d6f 7279 3d46 616c 7365 0d0a 2020  memory=False..  
+00019560: 2020 2020 2020 295b 333a 5d0d 0a20 2020        )[3:]..   
+00019570: 2020 2020 2064 6174 6173 6574 5f69 6e64       dataset_ind
+00019580: 6578 203d 2064 6174 6173 6574 2e69 6e64  ex = dataset.ind
+00019590: 6578 0d0a 2020 2020 2020 2020 7265 7475  ex..        retu
+000195a0: 726e 2064 6174 6173 6574 2c20 6461 7461  rn dataset, data
+000195b0: 7365 745f 696e 6465 780d 0a20 2020 200d  set_index..    .
+000195c0: 0a64 6566 2067 6574 5f73 706f 745f 6461  .def get_spot_da
+000195d0: 7461 7365 7428 7370 6f74 5f64 6174 6173  taset(spot_datas
+000195e0: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
+000195f0: 6973 5f73 706f 745f 6b65 7973 2c20 7863  is_spot_keys, xc
+00019600: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
+00019610: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
+00019620: 7261 7469 6f6e 2c20 4174 7472 6962 7574  ration, Attribut
+00019630: 6542 6f78 6e61 6d65 2c20 6465 7465 6374  eBoxname, detect
+00019640: 696f 6e63 6861 6e6e 656c 293a 0d0a 2020  ionchannel):..  
+00019650: 2020 2020 2020 416c 6c56 616c 7565 7320        AllValues 
+00019660: 3d20 7b7d 0d0a 2020 2020 2020 2020 706f  = {}..        po
+00019670: 7369 7820 3d20 7472 6163 6b5f 616e 616c  six = track_anal
+00019680: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00019690: 706f 7369 7822 5d0d 0a20 2020 2020 2020  posix"]..       
+000196a0: 2070 6f73 6979 203d 2074 7261 636b 5f61   posiy = track_a
+000196b0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+000196c0: 735b 2270 6f73 6979 225d 0d0a 2020 2020  s["posiy"]..    
+000196d0: 2020 2020 706f 7369 7a20 3d20 7472 6163      posiz = trac
+000196e0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+000196f0: 6b65 7973 5b22 706f 7369 7a22 5d0d 0a20  keys["posiz"].. 
+00019700: 2020 2020 2020 2066 7261 6d65 203d 2074         frame = t
+00019710: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+00019720: 6f74 5f6b 6579 735b 2266 7261 6d65 225d  ot_keys["frame"]
+00019730: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00019740: 2020 2020 4c6f 6361 7469 6f6e 5820 3d20      LocationX = 
+00019750: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+00019760: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
+00019770: 785d 2e61 7374 7970 6528 2266 6c6f 6174  x].astype("float
+00019780: 2229 202f 2078 6361 6c69 6272 6174 696f  ") / xcalibratio
+00019790: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
+000197a0: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+000197b0: 2020 2020 4c6f 6361 7469 6f6e 5920 3d20      LocationY = 
+000197c0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+000197d0: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
+000197e0: 795d 2e61 7374 7970 6528 2266 6c6f 6174  y].astype("float
+000197f0: 2229 202f 2079 6361 6c69 6272 6174 696f  ") / ycalibratio
+00019800: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
+00019810: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+00019820: 2020 2020 4c6f 6361 7469 6f6e 5a20 3d20      LocationZ = 
+00019830: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+00019840: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
+00019850: 7a5d 2e61 7374 7970 6528 2266 6c6f 6174  z].astype("float
+00019860: 2229 202f 207a 6361 6c69 6272 6174 696f  ") / zcalibratio
+00019870: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
+00019880: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+00019890: 2020 2020 4c6f 6361 7469 6f6e 5420 3d20      LocationT = 
+000198a0: 2873 706f 745f 6461 7461 7365 745b 6672  (spot_dataset[fr
+000198b0: 616d 655d 2e61 7374 7970 6528 2266 6c6f  ame].astype("flo
+000198c0: 6174 2229 292e 6173 7479 7065 2822 696e  at")).astype("in
+000198d0: 7422 290d 0a20 2020 2020 2020 200d 0a0d  t")..        ...
+000198e0: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
+000198f0: 7661 6c75 6573 203d 205b 7472 6163 6b5f  values = [track_
+00019900: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019910: 7973 5b22 6d65 616e 5f69 6e74 656e 7369  ys["mean_intensi
+00019920: 7479 225d 2c74 7261 636b 5f61 6e61 6c79  ty"],track_analy
+00019930: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
+00019940: 6f74 616c 5f69 6e74 656e 7369 7479 225d  otal_intensity"]
+00019950: 5d20 0d0a 2020 2020 2020 2020 666f 7220  ] ..        for 
+00019960: 286b 2c76 2920 696e 2074 7261 636b 5f61  (k,v) in track_a
+00019970: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+00019980: 732e 6974 656d 7328 293a 0d0a 0d0a 2020  s.items():....  
+00019990: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000199a0: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
+000199b0: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
+000199c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000199d0: 206b 203d 3d20 226d 6561 6e5f 696e 7465   k == "mean_inte
+000199e0: 6e73 6974 795f 6368 3222 3a0d 0a20 2020  nsity_ch2":..   
+000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a00: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00019a10: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00019a20: 706f 745f 6b65 7973 5b22 6d65 616e 5f69  pot_keys["mean_i
+00019a30: 6e74 656e 7369 7479 225d 0d0a 2020 2020  ntensity"]..    
+00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a50: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+00019a60: 5b76 616c 7565 5d20 3d20 7370 6f74 5f64  [value] = spot_d
+00019a70: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
+00019a80: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
+00019a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019aa0: 6966 206b 203d 3d20 2274 6f74 616c 5f69  if k == "total_i
+00019ab0: 6e74 656e 7369 7479 5f63 6832 223a 0d0a  ntensity_ch2":..
+00019ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ad0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00019ae0: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+00019af0: 735f 7370 6f74 5f6b 6579 735b 2274 6f74  s_spot_keys["tot
+00019b00: 616c 5f69 6e74 656e 7369 7479 225d 0d0a  al_intensity"]..
+00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b20: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
+00019b30: 6c75 6573 5b76 616c 7565 5d20 3d20 7370  lues[value] = sp
+00019b40: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
+00019b50: 7479 7065 2822 666c 6f61 7422 2920 2020  type("float")   
+00019b60: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00019b70: 2020 2020 2020 2020 6966 2076 206e 6f74          if v not
+00019b80: 2069 6e20 6967 6e6f 7265 5f76 616c 7565   in ignore_value
+00019b90: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00019ba0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bc0: 2020 2020 416c 6c56 616c 7565 735b 765d      AllValues[v]
+00019bd0: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
+00019be0: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
+00019bf0: 2229 0d0a 0d0a 2020 2020 2020 2020 416c  ")....        Al
+00019c00: 6c56 616c 7565 735b 706f 7369 785d 203d  lValues[posix] =
+00019c10: 2072 6f75 6e64 284c 6f63 6174 696f 6e58   round(LocationX
+00019c20: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
+00019c30: 5661 6c75 6573 5b70 6f73 6979 5d20 3d20  Values[posiy] = 
+00019c40: 726f 756e 6428 4c6f 6361 7469 6f6e 592c  round(LocationY,
+00019c50: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
+00019c60: 616c 7565 735b 706f 7369 7a5d 203d 2072  alues[posiz] = r
+00019c70: 6f75 6e64 284c 6f63 6174 696f 6e5a 2c33  ound(LocationZ,3
+00019c80: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
+00019c90: 6c75 6573 5b66 7261 6d65 5d20 3d20 726f  lues[frame] = ro
+00019ca0: 756e 6428 4c6f 6361 7469 6f6e 542c 3329  und(LocationT,3)
+00019cb0: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+00019cc0: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
+00019cd0: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+00019ce0: 732e 6170 7065 6e64 2841 7474 7269 6275  s.append(Attribu
+00019cf0: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
+00019d00: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
+00019d10: 656e 616d 6520 696e 2041 6c6c 5661 6c75  ename in AllValu
+00019d20: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
+00019d30: 2020 2020 2020 2020 2020 4174 7472 6962            Attrib
+00019d40: 7574 6569 6473 2e61 7070 656e 6428 6174  uteids.append(at
+00019d50: 7472 6962 7574 656e 616d 6529 2020 2020  tributename)    
+00019d60: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00019d70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00019d80: 2020 7265 7475 726e 2041 7474 7269 6275    return Attribu
+00019d90: 7465 6964 732c 2041 6c6c 5661 6c75 6573  teids, AllValues
+00019da0: 2020 2020 200d 0a20 2020 200d 0a64 6566       ..    ..def
+00019db0: 2067 6574 5f74 7261 636b 5f64 6174 6173   get_track_datas
+00019dc0: 6574 2874 7261 636b 5f64 6174 6173 6574  et(track_dataset
+00019dd0: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+00019de0: 5f73 706f 745f 6b65 7973 2c20 7472 6163  _spot_keys, trac
+00019df0: 6b5f 616e 616c 7973 6973 5f74 7261 636b  k_analysis_track
+00019e00: 5f6b 6579 732c 2054 7261 636b 4174 7472  _keys, TrackAttr
+00019e10: 6962 7574 6542 6f78 6e61 6d65 293a 0d0a  ibuteBoxname):..
+00019e20: 0d0a 2020 2020 2020 2020 416c 6c54 7261  ..        AllTra
+00019e30: 636b 5661 6c75 6573 203d 207b 7d0d 0a20  ckValues = {}.. 
+00019e40: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+00019e50: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+00019e60: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
+00019e70: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
+00019e80: 5469 6420 3d20 7472 6163 6b5f 6461 7461  Tid = track_data
+00019e90: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
+00019ea0: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+00019eb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019ec0: 416c 6c54 7261 636b 5661 6c75 6573 5b74  AllTrackValues[t
+00019ed0: 7261 636b 5f69 645d 203d 2054 6964 0d0a  rack_id] = Tid..
+00019ee0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019ef0: 666f 7220 286b 2c20 7629 2069 6e20 7472  for (k, v) in tr
+00019f00: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+00019f10: 636b 5f6b 6579 732e 6974 656d 7328 293a  ck_keys.items():
+00019f20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019f30: 2020 2020 7820 3d20 7472 6163 6b5f 6461      x = track_da
+00019f40: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+00019f50: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+00019f60: 2020 2020 2020 2020 2020 6d69 6e76 616c            minval
+00019f70: 203d 206d 696e 2878 290d 0a20 2020 2020   = min(x)..     
+00019f80: 2020 2020 2020 2020 2020 206d 6178 7661             maxva
+00019f90: 6c20 3d20 6d61 7828 7829 0d0a 0d0a 2020  l = max(x)....  
+00019fa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00019fb0: 206d 696e 7661 6c20 3e20 3020 616e 6420   minval > 0 and 
+00019fc0: 6d61 7876 616c 203c 3d20 313a 0d0a 0d0a  maxval <= 1:....
+00019fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fe0: 2020 2020 7820 3d20 7820 2b20 310d 0a0d      x = x + 1...
+00019ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a000: 2041 6c6c 5472 6163 6b56 616c 7565 735b   AllTrackValues[
+0001a010: 6b5d 203d 2072 6f75 6e64 2878 2c20 3329  k] = round(x, 3)
+0001a020: 0d0a 0d0a 2020 2020 2020 2020 5472 6163  ....        Trac
+0001a030: 6b41 7474 7269 6275 7465 6964 7320 3d20  kAttributeids = 
+0001a040: 5b5d 0d0a 2020 2020 2020 2020 5472 6163  []..        Trac
+0001a050: 6b41 7474 7269 6275 7465 6964 732e 6170  kAttributeids.ap
+0001a060: 7065 6e64 2854 7261 636b 4174 7472 6962  pend(TrackAttrib
+0001a070: 7574 6542 6f78 6e61 6d65 290d 0a20 2020  uteBoxname)..   
+0001a080: 2020 2020 2066 6f72 2061 7474 7269 6275       for attribu
+0001a090: 7465 6e61 6d65 2069 6e20 7472 6163 6b5f  tename in track_
+0001a0a0: 616e 616c 7973 6973 5f74 7261 636b 5f6b  analysis_track_k
+0001a0b0: 6579 732e 6b65 7973 2829 3a0d 0a20 2020  eys.keys():..   
+0001a0c0: 2020 2020 2020 2020 2054 7261 636b 4174           TrackAt
+0001a0d0: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
+0001a0e0: 6428 6174 7472 6962 7574 656e 616d 6529  d(attributename)
+0001a0f0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+0001a100: 2020 2020 7265 7475 726e 2054 7261 636b      return Track
+0001a110: 4174 7472 6962 7574 6569 6473 2c20 416c  Attributeids, Al
+0001a120: 6c54 7261 636b 5661 6c75 6573 0d0a 2020  lTrackValues..  
+0001a130: 2020 0d0a 6465 6620 6765 745f 6564 6765    ..def get_edge
+0001a140: 735f 6461 7461 7365 7428 6564 6765 735f  s_dataset(edges_
+0001a150: 6461 7461 7365 742c 2065 6467 6573 5f64  dataset, edges_d
+0001a160: 6174 6173 6574 5f69 6e64 6578 2c20 7472  ataset_index, tr
+0001a170: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001a180: 745f 6b65 7973 2c20 7472 6163 6b5f 616e  t_keys, track_an
+0001a190: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+0001a1a0: 7329 3a0d 0a0d 0a20 2020 2020 2020 2041  s):....        A
+0001a1b0: 6c6c 4564 6765 7356 616c 7565 7320 3d20  llEdgesValues = 
+0001a1c0: 7b7d 0d0a 2020 2020 2020 2020 7472 6163  {}..        trac
+0001a1d0: 6b5f 6964 203d 2074 7261 636b 5f61 6e61  k_id = track_ana
+0001a1e0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001a1f0: 2274 7261 636b 5f69 6422 5d0d 0a20 2020  "track_id"]..   
+0001a200: 2020 2020 2054 6964 203d 2065 6467 6573       Tid = edges
+0001a210: 5f64 6174 6173 6574 5b74 7261 636b 5f69  _dataset[track_i
+0001a220: 645d 2e61 7374 7970 6528 2266 6c6f 6174  d].astype("float
+0001a230: 2229 0d0a 2020 2020 2020 2020 696e 6469  ")..        indi
+0001a240: 6365 7320 3d20 6e70 2e77 6865 7265 2854  ces = np.where(T
+0001a250: 6964 203d 3d20 3029 0d0a 2020 2020 2020  id == 0)..      
+0001a260: 2020 6d61 7874 7261 636b 5f69 6420 3d20    maxtrack_id = 
+0001a270: 6d61 7828 5469 6429 0d0a 2020 2020 2020  max(Tid)..      
+0001a280: 2020 636f 6e64 6974 696f 6e5f 696e 6469    condition_indi
+0001a290: 6365 7320 3d20 6564 6765 735f 6461 7461  ces = edges_data
+0001a2a0: 7365 745f 696e 6465 785b 696e 6469 6365  set_index[indice
+0001a2b0: 735d 0d0a 2020 2020 2020 2020 5469 645b  s]..        Tid[
+0001a2c0: 636f 6e64 6974 696f 6e5f 696e 6469 6365  condition_indice
+0001a2d0: 735d 203d 206d 6178 7472 6163 6b5f 6964  s] = maxtrack_id
+0001a2e0: 202b 2031 0d0a 2020 2020 2020 2020 416c   + 1..        Al
+0001a2f0: 6c45 6467 6573 5661 6c75 6573 5b74 7261  lEdgesValues[tra
+0001a300: 636b 5f69 645d 203d 2054 6964 0d0a 0d0a  ck_id] = Tid....
+0001a310: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+0001a320: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a330: 6564 6765 735f 6b65 7973 2e76 616c 7565  edges_keys.value
+0001a340: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001a350: 2020 2020 6966 206b 2021 3d20 7472 6163      if k != trac
+0001a360: 6b5f 6964 3a0d 0a20 2020 2020 2020 2020  k_id:..         
+0001a370: 2020 2020 2020 2078 203d 2065 6467 6573         x = edges
+0001a380: 5f64 6174 6173 6574 5b6b 5d2e 6173 7479  _dataset[k].asty
+0001a390: 7065 2822 666c 6f61 7422 290d 0a0d 0a20  pe("float").... 
+0001a3a0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001a3b0: 6c6c 4564 6765 7356 616c 7565 735b 6b5d  llEdgesValues[k]
+0001a3c0: 203d 2078 2020 200d 0a20 2020 2020 2020   = x   ..       
+0001a3d0: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+0001a3e0: 726e 2041 6c6c 4564 6765 7356 616c 7565  rn AllEdgesValue
+0001a3f0: 7320 2020 0d0a 2020 2020 0d0a 2020 2020  s   ..    ..    
+0001a400: 2020 200d 0a20 2020 200d 0a64 6566 2073     ..    ..def s
+0001a410: 6361 6c65 5f76 616c 7565 2878 2c20 7363  cale_value(x, sc
+0001a420: 616c 6520 3d20 3235 3520 2a20 3235 3529  ale = 255 * 255)
+0001a430: 3a0d 0a0d 0a0d 0a20 2020 2020 7265 7475  :......     retu
+0001a440: 726e 2078 202a 2073 6361 6c65 2020 200d  rn x * scale   .
+0001a450: 0a20 2020 200d 0a0d 0a0d 0a64 6566 2070  .    ......def p
+0001a460: 726f 625f 7369 676d 6f69 6428 7829 3a0d  rob_sigmoid(x):.
+0001a470: 0a20 2020 2072 6574 7572 6e20 3120 2d20  .    return 1 - 
+0001a480: 6d61 7468 2e65 7870 282d 7829 0d0a 0d0a  math.exp(-x)....
+0001a490: 0d0a 6465 6620 616e 6775 6c61 725f 6368  ..def angular_ch
+0001a4a0: 616e 6765 2876 6563 5f30 2c20 7665 635f  ange(vec_0, vec_
+0001a4b0: 3129 3a0d 0a20 2020 2020 2020 200d 0a20  1):..        .. 
+0001a4c0: 2020 2020 2020 2076 6563 5f30 203d 2076         vec_0 = v
+0001a4d0: 6563 5f30 202f 206e 702e 6c69 6e61 6c67  ec_0 / np.linalg
+0001a4e0: 2e6e 6f72 6d28 7665 635f 3029 0d0a 2020  .norm(vec_0)..  
+0001a4f0: 2020 2020 2020 7665 635f 3120 3d20 7665        vec_1 = ve
+0001a500: 635f 3120 2f20 6e70 2e6c 696e 616c 672e  c_1 / np.linalg.
+0001a510: 6e6f 726d 2876 6563 5f31 290d 0a20 2020  norm(vec_1)..   
+0001a520: 2020 2020 2061 6e67 6c65 203d 206e 702e       angle = np.
+0001a530: 6172 6363 6f73 286e 702e 636c 6970 286e  arccos(np.clip(n
+0001a540: 702e 646f 7428 7665 635f 302c 2076 6563  p.dot(vec_0, vec
+0001a550: 5f31 292c 202d 312e 302c 2031 2e30 2929  _1), -1.0, 1.0))
+0001a560: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+0001a570: 3d20 616e 676c 6520 2a20 3138 3020 2f20  = angle * 180 / 
+0001a580: 6e70 2e70 690d 0a20 2020 2020 2020 2072  np.pi..        r
+0001a590: 6574 7572 6e20 616e 676c 650d 0a20 2020  eturn angle..   
+0001a5a0: 2020 0d0a 0d0a 6465 6620 6576 616c 5f62    ....def eval_b
+0001a5b0: 6f6f 6c28 7661 6c75 6529 3a0d 0a20 2020  ool(value):..   
+0001a5c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0001a5d0: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
+0001a5e0: 6520 203d 3d20 2754 7275 6527 3a20 0d0a  e  == 'True': ..
+0001a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a600: 6469 765f 6b65 7920 3d20 5472 7565 0d0a  div_key = True..
+0001a610: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001a620: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001a630: 6976 5f6b 6579 203d 2046 616c 7365 200d  iv_key = False .
+0001a640: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001a650: 6e20 6469 765f 6b65 7920 2020 2020 2020  n div_key       
+0001a660: 2020 2020 2020 2020 200d 0a0d 0a64 6566           ....def
+0001a670: 2063 6865 636b 5f61 6e64 5f75 7064 6174   check_and_updat
+0001a680: 655f 6d61 736b 286d 6173 6b2c 696d 6167  e_mask(mask,imag
+0001a690: 6529 3a0d 0a20 2020 2020 2020 0d0a 2020  e):..       ..  
+0001a6a0: 2020 2020 2020 6966 206c 656e 286d 6173        if len(mas
+0001a6b0: 6b2e 7368 6170 6529 203c 206c 656e 2869  k.shape) < len(i
+0001a6c0: 6d61 6765 2e73 6861 7065 293a 0d0a 2020  mage.shape):..  
+0001a6d0: 2020 2020 2020 2020 2020 7570 6461 7465            update
+0001a6e0: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
+0001a6f0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001a700: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0001a710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0001a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a730: 2020 2020 2020 2020 2020 2069 6d61 6765             image
-0001a740: 2e73 6861 7065 5b30 5d2c 0d0a 2020 2020  .shape[0],..    
+0001a730: 2020 696d 6167 652e 7368 6170 655b 305d    image.shape[0]
+0001a740: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a760: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001a770: 652e 7368 6170 655b 315d 2c0d 0a20 2020  e.shape[1],..   
+0001a760: 2020 2069 6d61 6765 2e73 6861 7065 5b31     image.shape[1
+0001a770: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
 0001a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a790: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001a7a0: 6765 2e73 6861 7065 5b32 5d2c 0d0a 2020  ge.shape[2],..  
+0001a790: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001a7a0: 325d 2c0d 0a20 2020 2020 2020 2020 2020  2],..           
 0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7c0: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001a7d0: 6167 652e 7368 6170 655b 335d 2c0d 0a20  age.shape[3],.. 
+0001a7c0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001a7d0: 5b33 5d2c 0d0a 2020 2020 2020 2020 2020  [3],..          
 0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7f0: 2020 2020 2020 2020 2020 205d 0d0a 2020             ]..  
-0001a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a810: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001a820: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0001a830: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
-0001a840: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
-0001a850: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001a860: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-0001a870: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001a880: 7065 5b31 5d29 3a0d 0a0d 0a20 2020 2020  pe[1]):....     
-0001a890: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0001a8a0: 7064 6174 655f 6d61 736b 5b69 2c20 6a2c  pdate_mask[i, j,
-0001a8b0: 203a 2c20 3a5d 203d 206d 6173 6b5b 692c   :, :] = mask[i,
-0001a8c0: 203a 2c20 3a5d 0d0a 2020 2020 2020 2020   :, :]..        
-0001a8d0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0001a8e0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
-0001a8f0: 736b 203d 206d 6173 6b0d 0a0d 0a20 2020  sk = mask....   
-0001a900: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
-0001a910: 7465 5f6d 6173 6b20 2020 2020 2020 200d  te_mask        .
-0001a920: 0a20 2020 2020 2020 0d0a                 .       ..
+0001a7f0: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
+0001a800: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001a810: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001a820: 6920 696e 2072 616e 6765 2830 2c20 7570  i in range(0, up
+0001a830: 6461 7465 5f6d 6173 6b2e 7368 6170 655b  date_mask.shape[
+0001a840: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+0001a850: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+0001a860: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
+0001a870: 6173 6b2e 7368 6170 655b 315d 293a 0d0a  ask.shape[1]):..
+0001a880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a890: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
+0001a8a0: 6b5b 692c 206a 2c20 3a2c 203a 5d20 3d20  k[i, j, :, :] = 
+0001a8b0: 6d61 736b 5b69 2c20 3a2c 203a 5d0d 0a20  mask[i, :, :].. 
+0001a8c0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001a8d0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0001a8e0: 6461 7465 5f6d 6173 6b20 3d20 6d61 736b  date_mask = mask
+0001a8f0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+0001a900: 726e 2075 7064 6174 655f 6d61 736b 2020  rn update_mask  
+0001a910: 2020 2020 2020 0d0a 2020 2020 2020 200d        ..       .
+0001a920: 0a                                       .
```

### Comparing `napatrackmater-3.4.8/napatrackmater/Trackvector.py` & `napatrackmater-3.4.9/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/__init__.py` & `napatrackmater-3.4.9/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/clustering.py` & `napatrackmater-3.4.9/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.4.9/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/fate_mapping.py` & `napatrackmater-3.4.9/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater/pretrained.py` & `napatrackmater-3.4.9/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.4.9/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.4.8
+Version: 3.4.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.4.8/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.4.9/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.8/setup.py` & `napatrackmater-3.4.9/setup.py`

 * *Files identical despite different names*

