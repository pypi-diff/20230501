# Comparing `tmp/napatrackmater-3.4.6.tar.gz` & `tmp/napatrackmater-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-glozzy6i/napatrackmater-3.4.6.tar", last modified: Mon May  1 15:33:06 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-as82i6zu/napatrackmater-3.4.7.tar", last modified: Mon May  1 18:02:37 2023, max compression
```

## Comparing `napatrackmater-3.4.6.tar` & `napatrackmater-3.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 15:33:06.689738 napatrackmater-3.4.6/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.6/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 15:33:06.679647 napatrackmater-3.4.6/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.6/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 15:33:06.322342 napatrackmater-3.4.6/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.6/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.6/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110192 2023-05-01 15:31:25.000000 napatrackmater-3.4.6/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.6/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.6/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.6/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.6/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.6/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.6/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-01 15:31:56.000000 napatrackmater-3.4.6/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 15:33:06.619946 napatrackmater-3.4.6/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 15:33:05.000000 napatrackmater-3.4.6/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-01 15:33:05.000000 napatrackmater-3.4.6/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-01 15:33:05.000000 napatrackmater-3.4.6/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-01 15:33:05.000000 napatrackmater-3.4.6/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-01 15:33:05.000000 napatrackmater-3.4.6/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-01 15:33:05.000000 napatrackmater-3.4.6/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-01 15:33:06.692170 napatrackmater-3.4.6/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.6/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 18:02:37.550547 napatrackmater-3.4.7/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.7/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 18:02:37.543482 napatrackmater-3.4.7/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.7/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 18:02:37.269426 napatrackmater-3.4.7/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.7/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.7/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   108805 2023-05-01 17:59:29.000000 napatrackmater-3.4.7/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.7/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.7/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.7/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.7/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.7/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.7/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-01 18:01:28.000000 napatrackmater-3.4.7/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 18:02:37.501565 napatrackmater-3.4.7/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 18:02:36.000000 napatrackmater-3.4.7/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-01 18:02:36.000000 napatrackmater-3.4.7/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-01 18:02:36.000000 napatrackmater-3.4.7/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-01 18:02:36.000000 napatrackmater-3.4.7/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-01 18:02:36.000000 napatrackmater-3.4.7/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-01 18:02:36.000000 napatrackmater-3.4.7/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-01 18:02:37.553549 napatrackmater-3.4.7/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.7/setup.py
```

### Comparing `napatrackmater-3.4.6/LICENSE` & `napatrackmater-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/PKG-INFO` & `napatrackmater-3.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.4.6
+Version: 3.4.7
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.4.6/README.md` & `napatrackmater-3.4.7/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.4.7/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.4.7/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/Trackmate.py` & `napatrackmater-3.4.7/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3704,3184 +3704,3098 @@
 0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e780: 2020 2020 2020 2020 2020 6368 616e 6e65            channe
 0000e790: 6c5f 6669 6c74 6572 6564 5f74 7261 636b  l_filtered_track
 0000e7a0: 732e 6170 7065 6e64 2874 7261 636b 5f69  s.append(track_i
 0000e7b0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
 0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e7d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e7e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 200d 0a0d 0a0d 0a20 2020 2020 2020 2020   ......         
-0000e810: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-0000e820: 6172 656e 7420 696e 2073 656c 662e 786d  arent in self.xm
-0000e830: 6c5f 726f 6f74 2e66 696e 6461 6c6c 2827  l_root.findall('
-0000e840: 4d6f 6465 6c27 293a 0d0a 2020 2020 2020  Model'):..      
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 2020 666f 7220 6669 7273 7463 6869 6c64    for firstchild
-0000e870: 2069 6e20 7061 7265 6e74 2e66 696e 6461   in parent.finda
-0000e880: 6c6c 2827 416c 6c53 706f 7473 2729 3a0d  ll('AllSpots'):.
-0000e890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e8a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000e8b0: 2073 6563 6f6e 6463 6869 6c64 2069 6e20   secondchild in 
-0000e8c0: 6669 7273 7463 6869 6c64 2e66 696e 6461  firstchild.finda
-0000e8d0: 6c6c 2827 5370 6f74 7349 6e46 7261 6d65  ll('SpotsInFrame
-0000e8e0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e900: 2020 2020 2066 6f72 2053 706f 7463 6861       for Spotcha
-0000e910: 6e6e 656c 6f62 6a65 6374 2069 6e20 7365  nnelobject in se
-0000e920: 636f 6e64 6368 696c 642e 6669 6e64 616c  condchild.findal
-0000e930: 6c28 2753 706f 7427 293a 0d0a 2020 2020  l('Spot'):..    
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e960: 7370 6f74 5f69 6420 3d20 696e 7428 5370  spot_id = int(Sp
-0000e970: 6f74 6368 616e 6e65 6c6f 626a 6563 742e  otchannelobject.
-0000e980: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-0000e990: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 2020 2020 2020 2069 6620 7370             if sp
-0000e9c0: 6f74 5f69 6420 6e6f 7420 696e 2073 656c  ot_id not in sel
-0000e9d0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e9e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e9f0: 2e6b 6579 7328 293a 2020 2020 0d0a 2020  .keys():    ..  
-0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea20: 2020 2020 2020 7365 636f 6e64 6368 696c        secondchil
-0000ea30: 642e 7265 6d6f 7665 2853 706f 7463 6861  d.remove(Spotcha
-0000ea40: 6e6e 656c 6f62 6a65 6374 290d 0a20 2020  nnelobject)..   
-0000ea50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea60: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000ea90: 2020 2020 2020 2020 2066 6f72 2070 6172           for par
-0000eaa0: 656e 7420 696e 2073 656c 662e 786d 6c5f  ent in self.xml_
-0000eab0: 726f 6f74 2e66 696e 6461 6c6c 2827 4d6f  root.findall('Mo
-0000eac0: 6465 6c27 293a 0d0a 2020 2020 2020 2020  del'):..        
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 666f 7220 6669 7273 7463 6869 6c64 2069  for firstchild i
-0000eaf0: 6e20 7061 7265 6e74 2e66 696e 6461 6c6c  n parent.findall
-0000eb00: 2827 416c 6c54 7261 636b 7327 293a 0d0a  ('AllTracks'):..
-0000eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000eb30: 7365 636f 6e64 6368 696c 6420 696e 2066  secondchild in f
-0000eb40: 6972 7374 6368 696c 642e 6669 6e64 616c  irstchild.findal
-0000eb50: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000eb80: 2045 6467 656f 626a 6563 7420 696e 2073   Edgeobject in s
-0000eb90: 6563 6f6e 6463 6869 6c64 2e66 696e 6461  econdchild.finda
-0000eba0: 6c6c 2827 4564 6765 2729 3a0d 0a20 2020  ll('Edge'):..   
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebd0: 2020 2020 2073 706f 745f 736f 7572 6365       spot_source
-0000ebe0: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
-0000ebf0: 4564 6765 6f62 6a65 6374 2e67 6574 2873  Edgeobject.get(s
-0000ec00: 656c 662e 7370 6f74 5f73 6f75 7263 655f  elf.spot_source_
-0000ec10: 6964 5f6b 6579 2929 2920 200d 0a20 2020  id_key)))  ..   
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e7f0: 6c66 2e78 6d6c 5f74 7265 652e 7772 6974  lf.xml_tree.writ
+0000e800: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
+0000e810: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
+0000e820: 7061 7468 2c20 7365 6c66 2e63 6861 6e6e  path, self.chann
+0000e830: 656c 5f78 6d6c 5f6e 616d 6529 2920 0d0a  el_xml_name)) ..
+0000e840: 0d0a 2020 2020 6465 6620 5f67 6574 5f78  ..    def _get_x
+0000e850: 6d6c 5f64 6174 6128 7365 6c66 293a 0d0a  ml_data(self):..
+0000e860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e870: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000e880: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
+0000e890: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
+0000e8a0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8c0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000e8d0: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
+0000e8e0: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
+0000e8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e900: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
+0000e910: 7472 6565 203d 2065 742e 7061 7273 6528  tree = et.parse(
+0000e920: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
+0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e940: 2020 2020 2020 7365 6c66 2e78 6d6c 5f72        self.xml_r
+0000e950: 6f6f 7420 3d20 7365 6c66 2e78 6d6c 5f74  oot = self.xml_t
+0000e960: 7265 652e 6765 7472 6f6f 7428 290d 0a20  ree.getroot().. 
+0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e980: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+0000e990: 6c5f 786d 6c5f 6e61 6d65 203d 2027 7365  l_xml_name = 'se
+0000e9a0: 636f 6e64 5f63 6861 6e6e 656c 5f27 202b  cond_channel_' +
+0000e9b0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0000e9c0: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+0000e9d0: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
+0000e9e0: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
+0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea00: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
+0000ea10: 656c 5f78 6d6c 5f70 6174 6820 3d20 6f73  el_xml_path = os
+0000ea20: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
+0000ea30: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea50: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
+0000ea60: 5f63 6861 6e6e 656c 5f74 7265 6528 290d  _channel_tree().
+0000ea70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea80: 2069 6620 7365 6c66 2e63 6c75 7374 6572   if self.cluster
+0000ea90: 5f6d 6f64 656c 2069 7320 6e6f 7420 4e6f  _model is not No
+0000eaa0: 6e65 2061 6e64 2073 656c 662e 7365 675f  ne and self.seg_
+0000eab0: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+0000eac0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000ead0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eae0: 6d61 7374 6572 5f78 6d6c 5f63 6f6e 7465  master_xml_conte
+0000eaf0: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+0000eb00: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+0000eb10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000eb20: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
+0000eb30: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
+0000eb40: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb60: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000eb70: 5f78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  _xml_root = self
+0000eb80: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
+0000eb90: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
+0000eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebb0: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
+0000ebc0: 6d6c 5f6e 616d 6520 3d20 276d 6173 7465  ml_name = 'maste
+0000ebd0: 725f 2720 2b20 7365 6c66 2e6d 6173 7465  r_' + self.maste
+0000ebe0: 725f 6578 7472 615f 6e61 6d65 2020 2b20  r_extra_name  + 
+0000ebf0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+0000ec00: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
+0000ec10: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000ec20: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
 0000ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec40: 2020 2020 2073 706f 745f 7461 7267 6574       spot_target
-0000ec50: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
-0000ec60: 4564 6765 6f62 6a65 6374 2e67 6574 2873  Edgeobject.get(s
-0000ec70: 656c 662e 7370 6f74 5f74 6172 6765 745f  elf.spot_target_
-0000ec80: 6964 5f6b 6579 2929 2920 2020 2020 200d  id_key)))      .
-0000ec90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecb0: 2020 2020 2020 2020 2069 6620 7370 6f74           if spot
-0000ecc0: 5f73 6f75 7263 655f 6964 206e 6f74 2069  _source_id not i
-0000ecd0: 6e20 7365 6c66 2e63 6861 6e6e 656c 5f75  n self.channel_u
-0000ece0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-0000ecf0: 7274 6965 732e 6b65 7973 2829 206f 7220  rties.keys() or 
-0000ed00: 7370 6f74 5f74 6172 6765 745f 6964 206e  spot_target_id n
-0000ed10: 6f74 2069 6e20 7365 6c66 2e63 6861 6e6e  ot in self.chann
-0000ed20: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000ed30: 726f 7065 7274 6965 732e 6b65 7973 2829  roperties.keys()
-0000ed40: 3a20 2020 2020 0d0a 2020 2020 2020 2020  :     ..        
-0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec40: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000ec50: 725f 786d 6c5f 7061 7468 203d 206f 732e  r_xml_path = os.
+0000ec60: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
+0000ec70: 662e 786d 6c5f 7061 7468 2920 2020 2020  f.xml_path)     
+0000ec80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000ec90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000eca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ecb0: 2e75 6e69 7175 655f 6f62 6a65 6374 7320  .unique_objects 
+0000ecc0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0000ecd0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000ece0: 655f 7072 6f70 6572 7469 6573 203d 207b  e_properties = {
+0000ecf0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+0000ed00: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000ed10: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+0000ed20: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
+0000ed30: 6976 6964 696e 6754 7261 636b 4964 7320  ividingTrackIds 
+0000ed40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+0000ed50: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000ed60: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
 0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed80: 2020 2020 7365 636f 6e64 6368 696c 642e      secondchild.
-0000ed90: 7265 6d6f 7665 2845 6467 656f 626a 6563  remove(Edgeobjec
-0000eda0: 7429 2020 0d0a 0d0a 2020 2020 2020 2020  t)  ....        
-0000edb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000edc0: 7061 7265 6e74 2069 6e20 7365 6c66 2e78  parent in self.x
-0000edd0: 6d6c 5f72 6f6f 742e 6669 6e64 616c 6c28  ml_root.findall(
-0000ede0: 274d 6f64 656c 2729 3a0d 0a20 2020 2020  'Model'):..     
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee00: 2020 2066 6f72 2066 6972 7374 6368 696c     for firstchil
-0000ee10: 6420 696e 2070 6172 656e 742e 6669 6e64  d in parent.find
-0000ee20: 616c 6c28 2746 696c 7465 7265 6454 7261  all('FilteredTra
-0000ee30: 636b 7327 293a 0d0a 2020 2020 2020 2020  cks'):..        
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 2020 2020 666f 7220 7365 636f 6e64 6368      for secondch
-0000ee60: 696c 6420 696e 2066 6972 7374 6368 696c  ild in firstchil
-0000ee70: 642e 6669 6e64 616c 6c28 2754 7261 636b  d.findall('Track
-0000ee80: 4944 2729 3a20 0d0a 2020 2020 2020 2020  ID'): ..        
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eea0: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-0000eeb0: 6572 5f74 7261 636b 5f69 6420 3d20 696e  er_track_id = in
-0000eec0: 7428 7365 636f 6e64 6368 696c 642e 6765  t(secondchild.ge
-0000eed0: 7428 7365 6c66 2e74 7261 636b 6964 5f6b  t(self.trackid_k
-0000eee0: 6579 2929 2020 0d0a 2020 2020 2020 2020  ey))  ..        
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef00: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0000ef10: 696c 7465 725f 7472 6163 6b5f 6964 206e  ilter_track_id n
-0000ef20: 6f74 2069 6e20 6368 616e 6e65 6c5f 6669  ot in channel_fi
-0000ef30: 6c74 6572 6564 5f74 7261 636b 733a 0d0a  ltered_tracks:..
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef60: 2020 2020 2020 2020 2020 2020 6669 7273              firs
-0000ef70: 7463 6869 6c64 2e72 656d 6f76 6528 7365  tchild.remove(se
-0000ef80: 636f 6e64 6368 696c 6429 2020 2020 2020  condchild)      
-0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efa0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0000efb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000efc0: 662e 786d 6c5f 7472 6565 2e77 7269 7465  f.xml_tree.write
-0000efd0: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-0000efe0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
-0000eff0: 6174 682c 2073 656c 662e 6368 616e 6e65  ath, self.channe
-0000f000: 6c5f 786d 6c5f 6e61 6d65 2929 200d 0a0d  l_xml_name)) ...
-0000f010: 0a20 2020 2064 6566 205f 6765 745f 786d  .    def _get_xm
-0000f020: 6c5f 6461 7461 2873 656c 6629 3a0d 0a0d  l_data(self):...
-0000f030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f040: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000f050: 2020 2020 2069 6620 7365 6c66 2e63 6861       if self.cha
-0000f060: 6e6e 656c 5f73 6567 5f69 6d61 6765 2069  nnel_seg_image i
-0000f070: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f090: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-0000f0a0: 786d 6c5f 636f 6e74 656e 7420 3d20 7365  xml_content = se
-0000f0b0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a  lf.xml_content..
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f74        self.xml_t
-0000f0e0: 7265 6520 3d20 6574 2e70 6172 7365 2873  ree = et.parse(s
-0000f0f0: 656c 662e 786d 6c5f 7061 7468 290d 0a20  elf.xml_path).. 
-0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f110: 2020 2020 2073 656c 662e 786d 6c5f 726f       self.xml_ro
-0000f120: 6f74 203d 2073 656c 662e 786d 6c5f 7472  ot = self.xml_tr
-0000f130: 6565 2e67 6574 726f 6f74 2829 0d0a 2020  ee.getroot()..  
-0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-0000f160: 5f78 6d6c 5f6e 616d 6520 3d20 2773 6563  _xml_name = 'sec
-0000f170: 6f6e 645f 6368 616e 6e65 6c5f 2720 2b20  ond_channel_' + 
-0000f180: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
-0000f190: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
-0000f1a0: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000f1b0: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
-0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1d0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-0000f1e0: 6c5f 786d 6c5f 7061 7468 203d 206f 732e  l_xml_path = os.
-0000f1f0: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
-0000f200: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
-0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
-0000f230: 6368 616e 6e65 6c5f 7472 6565 2829 0d0a  channel_tree()..
-0000f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f250: 6966 2073 656c 662e 636c 7573 7465 725f  if self.cluster_
-0000f260: 6d6f 6465 6c20 6973 206e 6f74 204e 6f6e  model is not Non
-0000f270: 6520 616e 6420 7365 6c66 2e73 6567 5f69  e and self.seg_i
-0000f280: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000f290: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000f2a0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000f2b0: 6173 7465 725f 786d 6c5f 636f 6e74 656e  aster_xml_conten
-0000f2c0: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
-0000f2d0: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
-0000f2e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f2f0: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
-0000f300: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
-0000f310: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
-0000f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f330: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000f340: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
-0000f350: 6d61 7374 6572 5f78 6d6c 5f74 7265 652e  master_xml_tree.
-0000f360: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f380: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
-0000f390: 6c5f 6e61 6d65 203d 2027 6d61 7374 6572  l_name = 'master
-0000f3a0: 5f27 202b 2073 656c 662e 6d61 7374 6572  _' + self.master
-0000f3b0: 5f65 7874 7261 5f6e 616d 6520 202b 206f  _extra_name  + o
-0000f3c0: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
-0000f3d0: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-0000f3e0: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
-0000f3f0: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
-0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f410: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-0000f420: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
-0000f430: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
-0000f440: 2e78 6d6c 5f70 6174 6829 2020 2020 2020  .xml_path)      
-0000f450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f460: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000f470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f480: 756e 6971 7565 5f6f 626a 6563 7473 203d  unique_objects =
-0000f490: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-0000f4a0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000f4b0: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-0000f4c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f4d0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
-0000f4e0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0000f4f0: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000f500: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
-0000f510: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0000f520: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-0000f530: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
-0000f540: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f550: 656c 662e 616c 6c5f 7472 6163 6b5f 7072  elf.all_track_pr
-0000f560: 6f70 6572 7469 6573 203d 205b 5d0d 0a20  operties = [].. 
-0000f570: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f580: 656c 662e 7370 6c69 745f 706f 696e 7473  elf.split_points
-0000f590: 5f74 696d 6573 203d 205b 5d0d 0a0d 0a20  _times = [].... 
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f5c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000f5d0: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000f5e0: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
-0000f5f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f600: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
-0000f610: 7261 636b 4964 732e 6170 7065 6e64 284e  rackIds.append(N
-0000f620: 6f6e 6529 0d0a 2020 2020 2020 2020 2020  one)..          
-0000f630: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-0000f640: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000f650: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
-0000f660: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000f670: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000f680: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
-0000f690: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000f6a0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000f6b0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000f6c0: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
-0000f6d0: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
-0000f6e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f6f0: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
-0000f700: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
-0000f710: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
-0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f740: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f750: 2020 2020 7365 6c66 2e53 706f 746f 626a      self.Spotobj
-0000f760: 6563 7473 203d 2073 656c 662e 786d 6c5f  ects = self.xml_
-0000f770: 636f 6e74 656e 742e 6669 6e64 2827 4d6f  content.find('Mo
-0000f780: 6465 6c27 292e 6669 6e64 2827 416c 6c53  del').find('AllS
-0000f790: 706f 7473 2729 0d0a 2020 2020 2020 2020  pots')..        
-0000f7a0: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
-0000f7b0: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
-0000f7c0: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
-0000f7d0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000f7e0: 6b73 203d 2073 656c 662e 786d 6c5f 636f  ks = self.xml_co
-0000f7f0: 6e74 656e 742e 6669 6e64 2822 4d6f 6465  ntent.find("Mode
-0000f800: 6c22 292e 6669 6e64 2822 416c 6c54 7261  l").find("AllTra
-0000f810: 636b 7322 290d 0a20 2020 2020 2020 2020  cks")..         
-0000f820: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000f830: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-0000f840: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-0000f850: 7474 696e 6773 2229 2e66 696e 6428 2249  ttings").find("I
-0000f860: 6d61 6765 4461 7461 2229 0d0a 2020 2020  mageData")..    
-0000f870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f880: 2e78 6361 6c69 6272 6174 696f 6e20 3d20  .xcalibration = 
-0000f890: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000f8a0: 6e67 732e 6765 7428 2270 6978 656c 7769  ngs.get("pixelwi
-0000f8b0: 6474 6822 2929 0d0a 2020 2020 2020 2020  dth"))..        
-0000f8c0: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
-0000f8d0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
-0000f8e0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
-0000f8f0: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
-0000f900: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
-0000f910: 2020 2020 2073 656c 662e 7a63 616c 6962       self.zcalib
-0000f920: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000f930: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000f940: 2822 766f 7865 6c64 6570 7468 2229 290d  ("voxeldepth")).
-0000f950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f960: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
-0000f970: 6f6e 203d 2069 6e74 2866 6c6f 6174 2873  on = int(float(s
-0000f980: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000f990: 2822 7469 6d65 696e 7465 7276 616c 2229  ("timeinterval")
-0000f9a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000f9b0: 2020 2020 7365 6c66 2e64 6574 6563 746f      self.detecto
-0000f9c0: 7273 6574 7469 6e67 7320 3d20 7365 6c66  rsettings = self
-0000f9d0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000f9e0: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000f9f0: 6e64 2822 4465 7465 6374 6f72 5365 7474  nd("DetectorSett
-0000fa00: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
-0000fa10: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
-0000fa20: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
-0000fa30: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000fa40: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
-0000fa50: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
-0000fa60: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
-0000fa70: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
-0000fa80: 746f 7263 6861 6e6e 656c 203d 2069 6e74  torchannel = int
-0000fa90: 2866 6c6f 6174 2873 656c 662e 6465 7465  (float(self.dete
-0000faa0: 6374 6f72 7365 7474 696e 6773 2e67 6574  ctorsettings.get
-0000fab0: 2822 5441 5247 4554 5f43 4841 4e4e 454c  ("TARGET_CHANNEL
-0000fac0: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
-0000fad0: 2020 2020 2020 7365 6c66 2e74 7374 6172        self.tstar
-0000fae0: 7420 3d20 696e 7428 666c 6f61 7428 7365  t = int(float(se
-0000faf0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
-0000fb00: 2e67 6574 2822 7473 7461 7274 2229 2929  .get("tstart")))
-0000fb10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fb20: 2020 7365 6c66 2e74 656e 6420 3d20 696e    self.tend = in
-0000fb30: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
-0000fb40: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
-0000fb50: 7465 6e64 2229 2929 0d0a 2020 2020 2020  tend")))..      
-0000fb60: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000fb70: 6765 745f 626f 756e 6461 7279 5f70 6f69  get_boundary_poi
-0000fb80: 6e74 7328 290d 0a20 2020 2020 2020 2020  nts()..         
-0000fb90: 2020 2020 2020 2070 7269 6e74 2827 4974         print('It
-0000fba0: 6572 6174 696e 6720 6f76 6572 2073 706f  erating over spo
-0000fbb0: 7473 2069 6e20 6672 616d 6527 290d 0a20  ts in frame').. 
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fbd0: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000fbf0: 7574 7572 6573 203d 205b 5d0d 0a0d 0a20  utures = [].... 
-0000fc00: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000fc10: 6974 6820 636f 6e63 7572 7265 6e74 2e66  ith concurrent.f
-0000fc20: 7574 7572 6573 2e54 6872 6561 6450 6f6f  utures.ThreadPoo
-0000fc30: 6c45 7865 6375 746f 7228 6d61 785f 776f  lExecutor(max_wo
-0000fc40: 726b 6572 7320 3d20 6f73 2e63 7075 5f63  rkers = os.cpu_c
-0000fc50: 6f75 6e74 2829 2920 6173 2065 7865 6375  ount()) as execu
-0000fc60: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
-0000fc70: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc90: 666f 7220 6672 616d 6520 696e 2073 656c  for frame in sel
-0000fca0: 662e 5370 6f74 6f62 6a65 6374 732e 6669  f.Spotobjects.fi
-0000fcb0: 6e64 616c 6c28 2753 706f 7473 496e 4672  ndall('SpotsInFr
-0000fcc0: 616d 6527 293a 0d0a 2020 2020 2020 2020  ame'):..        
+0000ed80: 7365 6c66 2e61 6c6c 5f74 7261 636b 5f70  self.all_track_p
+0000ed90: 726f 7065 7274 6965 7320 3d20 5b5d 0d0a  roperties = []..
+0000eda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edb0: 7365 6c66 2e73 706c 6974 5f70 6f69 6e74  self.split_point
+0000edc0: 735f 7469 6d65 7320 3d20 5b5d 0d0a 0d0a  s_times = []....
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ede0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000edf0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ee00: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+0000ee10: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
+0000ee20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ee30: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
+0000ee40: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000ee50: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
+0000ee60: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+0000ee70: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
+0000ee80: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
+0000ee90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000eea0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eeb0: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+0000eec0: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000eed0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000eee0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+0000eef0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+0000ef00: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000ef10: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000ef20: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000ef30: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
+0000ef40: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
+0000ef50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000ef70: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ef80: 2020 2020 2073 656c 662e 5370 6f74 6f62       self.Spotob
+0000ef90: 6a65 6374 7320 3d20 7365 6c66 2e78 6d6c  jects = self.xml
+0000efa0: 5f63 6f6e 7465 6e74 2e66 696e 6428 274d  _content.find('M
+0000efb0: 6f64 656c 2729 2e66 696e 6428 2741 6c6c  odel').find('All
+0000efc0: 5370 6f74 7327 290d 0a20 2020 2020 2020  Spots')..       
+0000efd0: 2020 2020 2020 2020 2023 2045 7874 7261           # Extra
+0000efe0: 6374 2074 6865 2074 7261 636b 7320 6672  ct the tracks fr
+0000eff0: 6f6d 2078 6d6c 0d0a 2020 2020 2020 2020  om xml..        
+0000f000: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000f010: 636b 7320 3d20 7365 6c66 2e78 6d6c 5f63  cks = self.xml_c
+0000f020: 6f6e 7465 6e74 2e66 696e 6428 224d 6f64  ontent.find("Mod
+0000f030: 656c 2229 2e66 696e 6428 2241 6c6c 5472  el").find("AllTr
+0000f040: 6163 6b73 2229 0d0a 2020 2020 2020 2020  acks")..        
+0000f050: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000f060: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+0000f070: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+0000f080: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+0000f090: 496d 6167 6544 6174 6122 290d 0a20 2020  ImageData")..   
+0000f0a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f0b0: 662e 7863 616c 6962 7261 7469 6f6e 203d  f.xcalibration =
+0000f0c0: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
+0000f0d0: 696e 6773 2e67 6574 2822 7069 7865 6c77  ings.get("pixelw
+0000f0e0: 6964 7468 2229 290d 0a20 2020 2020 2020  idth"))..       
+0000f0f0: 2020 2020 2020 2020 2073 656c 662e 7963           self.yc
+0000f100: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
+0000f110: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000f120: 2e67 6574 2822 7069 7865 6c68 6569 6768  .get("pixelheigh
+0000f130: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
+0000f140: 2020 2020 2020 7365 6c66 2e7a 6361 6c69        self.zcali
+0000f150: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+0000f160: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000f170: 7428 2276 6f78 656c 6465 7074 6822 2929  t("voxeldepth"))
+0000f180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f190: 2020 7365 6c66 2e74 6361 6c69 6272 6174    self.tcalibrat
+0000f1a0: 696f 6e20 3d20 696e 7428 666c 6f61 7428  ion = int(float(
+0000f1b0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000f1c0: 7428 2274 696d 6569 6e74 6572 7661 6c22  t("timeinterval"
+0000f1d0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000f1e0: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
+0000f1f0: 6f72 7365 7474 696e 6773 203d 2073 656c  orsettings = sel
+0000f200: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000f210: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000f220: 696e 6428 2244 6574 6563 746f 7253 6574  ind("DetectorSet
+0000f230: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
+0000f240: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+0000f250: 7369 6373 6574 7469 6e67 7320 3d20 7365  sicsettings = se
+0000f260: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000f270: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000f280: 6669 6e64 2822 4261 7369 6353 6574 7469  find("BasicSetti
+0000f290: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
+0000f2a0: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
+0000f2b0: 6374 6f72 6368 616e 6e65 6c20 3d20 696e  ctorchannel = in
+0000f2c0: 7428 666c 6f61 7428 7365 6c66 2e64 6574  t(float(self.det
+0000f2d0: 6563 746f 7273 6574 7469 6e67 732e 6765  ectorsettings.ge
+0000f2e0: 7428 2254 4152 4745 545f 4348 414e 4e45  t("TARGET_CHANNE
+0000f2f0: 4c22 2929 290d 0a20 2020 2020 2020 2020  L")))..         
+0000f300: 2020 2020 2020 2073 656c 662e 7473 7461         self.tsta
+0000f310: 7274 203d 2069 6e74 2866 6c6f 6174 2873  rt = int(float(s
+0000f320: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
+0000f330: 732e 6765 7428 2274 7374 6172 7422 2929  s.get("tstart"))
+0000f340: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f350: 2020 2073 656c 662e 7465 6e64 203d 2069     self.tend = i
+0000f360: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+0000f370: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+0000f380: 2274 656e 6422 2929 290d 0a20 2020 2020  "tend")))..     
+0000f390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f3a0: 5f67 6574 5f62 6f75 6e64 6172 795f 706f  _get_boundary_po
+0000f3b0: 696e 7473 2829 0d0a 2020 2020 2020 2020  ints()..        
+0000f3c0: 2020 2020 2020 2020 7072 696e 7428 2749          print('I
+0000f3d0: 7465 7261 7469 6e67 206f 7665 7220 7370  terating over sp
+0000f3e0: 6f74 7320 696e 2066 7261 6d65 2729 0d0a  ots in frame')..
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f400: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f420: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
+0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f440: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
+0000f450: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
+0000f460: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
+0000f470: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
+0000f480: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
+0000f490: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
+0000f4a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4c0: 2066 6f72 2066 7261 6d65 2069 6e20 7365   for frame in se
+0000f4d0: 6c66 2e53 706f 746f 626a 6563 7473 2e66  lf.Spotobjects.f
+0000f4e0: 696e 6461 6c6c 2827 5370 6f74 7349 6e46  indall('SpotsInF
+0000f4f0: 7261 6d65 2729 3a0d 0a20 2020 2020 2020  rame'):..       
+0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f510: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
+0000f520: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
+0000f530: 626d 6974 2873 656c 662e 5f73 706f 745f  bmit(self._spot_
+0000f540: 636f 6d70 7574 6572 2c20 6672 616d 6529  computer, frame)
+0000f550: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f560: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000f570: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+0000f580: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5d0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000f5e0: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
+0000f5f0: 6563 7469 6e67 2053 706f 7473 220d 0a20  ecting Spots".. 
+0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000f630: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
+0000f640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f660: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 2020 2020 6c65 6e28 6675 7475 7265 7329      len(futures)
+0000f6a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f6f0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000f700: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
+0000f710: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000f720: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
+0000f730: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
+0000f740: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
+0000f750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f770: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+0000f780: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
+0000f790: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+0000f7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7b0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000f7c0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+0000f7d0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f800: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000f810: 722e 7661 6c75 6520 3d20 2073 656c 662e  r.value =  self.
+0000f820: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f840: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
+0000f850: 756c 7428 290d 0a0d 0a20 2020 2020 2020  ult()....       
+0000f860: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0000f870: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+0000f880: 7472 6163 6b73 207b 6c65 6e28 7365 6c66  tracks {len(self
+0000f890: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000f8a0: 6964 7329 7d27 2920 200d 0a20 2020 2020  ids)}')  ..     
+0000f8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f8c0: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
+0000f8d0: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000f8e0: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
+0000f8f0: 2020 2020 2020 2020 2077 6974 6820 636f           with co
+0000f900: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+0000f910: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
+0000f920: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
+0000f930: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
+0000f940: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
+0000f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f960: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000f970: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
+0000f980: 6163 6b20 696e 2073 656c 662e 7472 6163  ack in self.trac
+0000f990: 6b73 2e66 696e 6461 6c6c 2827 5472 6163  ks.findall('Trac
+0000f9a0: 6b27 293a 0d0a 2020 2020 2020 2020 2020  k'):..          
+0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
+0000f9f0: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
+0000fa00: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
+0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa20: 2020 2020 2020 2020 2069 6620 7472 6163           if trac
+0000fa30: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+0000fa40: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+0000fa50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa70: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
+0000fa80: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
+0000fa90: 6974 2873 656c 662e 5f74 7261 636b 5f63  it(self._track_c
+0000faa0: 6f6d 7075 7465 722c 2074 7261 636b 2c20  omputer, track, 
+0000fab0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fad0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+0000fae0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+0000faf0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000fb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000fb40: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
+0000fb50: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
+0000fb60: 5472 6163 6b73 220d 0a20 2020 2020 2020  Tracks"..       
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fb90: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
+0000fba0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
+0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbd0: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbf0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000fc00: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
+0000fc10: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc40: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0000fc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc60: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000fc70: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
+0000fc80: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+0000fc90: 2020 2020 2020 2020 2020 666f 7220 7220            for r 
+0000fca0: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
+0000fcb0: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
+0000fcc0: 6564 2866 7574 7572 6573 293a 0d0a 2020  ed(futures):..  
 0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fce0: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
-0000fcf0: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
-0000fd00: 6d69 7428 7365 6c66 2e5f 7370 6f74 5f63  mit(self._spot_c
-0000fd10: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
-0000fd20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fd30: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000fd40: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-0000fd50: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcf0: 2020 7365 6c66 2e63 6f75 6e74 203d 2073    self.count = s
+0000fd00: 656c 662e 636f 756e 7420 2b20 310d 0a20  elf.count + 1.. 
+0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+0000fd40: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+0000fd50: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
 0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd70: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000fdb0: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
-0000fdc0: 6374 696e 6720 5370 6f74 7322 0d0a 2020  cting Spots"..  
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdf0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000fe00: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000fd70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fd80: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+0000fd90: 616c 7565 203d 2073 656c 662e 636f 756e  alue = self.coun
+0000fda0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdc0: 2020 2020 2020 2072 2e72 6573 756c 7428         r.result(
+0000fdd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fde0: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
+0000fdf0: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
+0000fe00: 6e6f 7420 4e6f 6e65 3a20 200d 0a20 2020  not None:  ..   
 0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe30: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
-0000fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe60: 2020 206c 656e 2866 7574 7572 6573 292c     len(futures),
-0000fe70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe90: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000feb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fec0: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
-0000fed0: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
-0000fee0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000fef0: 2072 2069 6e20 636f 6e63 7572 7265 6e74   r in concurrent
-0000ff00: 2e66 7574 7572 6573 2e61 735f 636f 6d70  .futures.as_comp
-0000ff10: 6c65 7465 6428 6675 7475 7265 7329 3a0d  leted(futures):.
-0000ff20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000ff50: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
-0000ff60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff80: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0000ff90: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-0000ffa0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000fe20: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
+0000fe30: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
+0000fe40: 786d 6c28 290d 0a20 2020 2020 2020 2020  xml()..         
+0000fe50: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+0000fe60: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
+0000fe70: 6b2c 7629 2069 6e20 7365 6c66 2e67 7261  k,v) in self.gra
+0000fe80: 7068 5f73 706c 6974 2e69 7465 6d73 2829  ph_split.items()
+0000fe90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fec0: 2020 2020 2020 2020 2020 2020 6461 7567              daug
+0000fed0: 6874 6572 5f74 7261 636b 5f69 6420 3d20  hter_track_id = 
+0000fee0: 2069 6e74 2866 6c6f 6174 2873 7472 2873   int(float(str(s
+0000fef0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+0000ff00: 7072 6f70 6572 7469 6573 5b69 6e74 2866  properties[int(f
+0000ff10: 6c6f 6174 286b 2929 5d5b 7365 6c66 2e75  loat(k))][self.u
+0000ff20: 6e69 7175 6569 645f 6b65 795d 2929 290d  niqueid_key]))).
+0000ff30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff40: 2020 2020 2020 2020 2020 2020 2070 6172               par
+0000ff50: 656e 745f 7472 6163 6b5f 6964 203d 2069  ent_track_id = i
+0000ff60: 6e74 2866 6c6f 6174 2873 7472 2873 656c  nt(float(str(sel
+0000ff70: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+0000ff80: 6f70 6572 7469 6573 5b69 6e74 2866 6c6f  operties[int(flo
+0000ff90: 6174 2876 2929 5d5b 7365 6c66 2e75 6e69  at(v))][self.uni
+0000ffa0: 7175 6569 645f 6b65 795d 2929 290d 0a20  queid_key]))).. 
 0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ffd0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000ffe0: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
-0000fff0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-00010000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010010: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
-00010020: 6c74 2829 0d0a 0d0a 2020 2020 2020 2020  lt()....        
-00010030: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00010040: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
-00010050: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
-00010060: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-00010070: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
-00010080: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00010090: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-000100a0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-000100b0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-000100c0: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
-000100d0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-000100e0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
-000100f0: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
-00010100: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
-00010110: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
-00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010130: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010140: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
-00010150: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
-00010160: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
-00010170: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000ffc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ffd0: 6772 6170 685f 7472 6163 6b73 5b64 6175  graph_tracks[dau
+0000ffe0: 6768 7465 725f 7472 6163 6b5f 6964 5d20  ghter_track_id] 
+0000fff0: 3d20 7061 7265 6e74 5f74 7261 636b 5f69  = parent_track_i
+00010000: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
+00010010: 2020 2073 656c 662e 5f67 6574 5f61 7474     self._get_att
+00010020: 7269 6275 7465 7328 290d 0a20 2020 2020  ributes()..     
+00010030: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00010040: 6c66 2e63 6c75 7374 6572 5f6d 6f64 656c  lf.cluster_model
+00010050: 2061 6e64 2073 656c 662e 7365 675f 696d   and self.seg_im
+00010060: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+00010070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010080: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00010090: 7373 6967 6e5f 636c 7573 7465 725f 636c  ssign_cluster_cl
+000100a0: 6173 7328 290d 0a20 2020 2020 2020 2020  ass()..         
+000100b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000100c0: 6c66 2e5f 6372 6561 7465 5f6d 6173 7465  lf._create_maste
+000100d0: 725f 786d 6c28 290d 0a20 2020 2020 2020  r_xml()..       
+000100e0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+000100f0: 756e 7420 3d20 3020 0d0a 2020 2020 2020  unt = 0 ..      
+00010100: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
+00010110: 6163 6b5f 6964 2069 6e20 7365 6c66 2e66  ack_id in self.f
+00010120: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+00010130: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010150: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010160: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+00010170: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000101b0: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
-000101c0: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
-000101d0: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+000101b0: 5f62 6172 2e6c 6162 656c 203d 2022 4a75  _bar.label = "Ju
+000101c0: 7374 206f 6e65 206d 6f72 6520 7468 696e  st one more thin
+000101d0: 6722 0d0a 2020 2020 2020 2020 2020 2020  g"..            
 000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101f0: 2020 2020 2020 2020 6966 2074 7261 636b          if track
-00010200: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
-00010210: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
-00010220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010200: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+00010210: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
+00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010240: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
-00010250: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
-00010260: 7428 7365 6c66 2e5f 7472 6163 6b5f 636f  t(self._track_co
-00010270: 6d70 7574 6572 2c20 7472 6163 6b2c 2074  mputer, track, t
-00010280: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
-00010290: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000102a0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-000102b0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-000102c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010240: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010270: 2020 2020 2020 2020 2020 2020 206c 656e               len
+00010280: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
+00010290: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102c0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
 000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010310: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-00010320: 203d 2022 436f 6c6c 6563 7469 6e67 2054   = "Collecting T
-00010330: 7261 636b 7322 0d0a 2020 2020 2020 2020  racks"..        
-00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010360: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
-00010370: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
-00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+00010300: 5f62 6172 2e73 686f 7728 290d 0a20 2020  _bar.show()..   
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010330: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+00010340: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
+00010350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010370: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00010380: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
+00010390: 6520 3d20 7365 6c66 2e63 6f75 6e74 0d0a  e = self.count..
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103c0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-000103d0: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-000103e0: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
-000103f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010430: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00010440: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-00010450: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00010460: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
-00010470: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
-00010480: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
-00010490: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
-000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
-000104d0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
-000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010500: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-00010510: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-00010520: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010550: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-00010560: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
-00010570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
-000105a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000105b0: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
-000105c0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
-000105d0: 6f74 204e 6f6e 653a 2020 0d0a 2020 2020  ot None:  ..    
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
-00010600: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
-00010610: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
-00010620: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00010630: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-00010640: 2c76 2920 696e 2073 656c 662e 6772 6170  ,v) in self.grap
-00010650: 685f 7370 6c69 742e 6974 656d 7328 293a  h_split.items():
-00010660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010670: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000103c0: 2020 2020 7365 6c66 2e5f 6669 6e61 6c5f      self._final_
+000103d0: 7472 6163 6b73 2874 7261 636b 5f69 6429  tracks(track_id)
+000103e0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+000103f0: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
+00010400: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
+00010410: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00010420: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
+00010430: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
+00010440: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00010450: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
+00010460: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
+00010470: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00010480: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010490: 662e 5f74 656d 706f 7261 6c5f 706c 6f74  f._temporal_plot
+000104a0: 735f 7472 6163 6b6d 6174 6528 290d 0a20  s_trackmate().. 
+000104b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000104c0: 0a0d 0a20 2020 2064 6566 205f 6372 6561  ...    def _crea
+000104d0: 7465 5f6d 6173 7465 725f 786d 6c28 7365  te_master_xml(se
+000104e0: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
+000104f0: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+00010500: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
+00010510: 6f62 6a65 6374 2069 6e20 7365 6c66 2e6d  object in self.m
+00010520: 6173 7465 725f 786d 6c5f 726f 6f74 2e69  aster_xml_root.i
+00010530: 7465 7228 2753 706f 7427 293a 0d0a 2020  ter('Spot'):..  
+00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010550: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00010560: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
+00010570: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+00010580: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000105b0: 2063 656c 6c5f 6964 2069 6e20 7365 6c66   cell_id in self
+000105c0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000105d0: 7065 7274 6965 732e 6b65 7973 2829 3a0d  perties.keys():.
+000105e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010630: 2066 6f72 206b 2069 6e20 7365 6c66 2e75   for k in self.u
+00010640: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00010650: 7274 6965 735b 6365 6c6c 5f69 645d 2e6b  rties[cell_id].k
+00010660: 6579 7328 293a 0d0a 0d0a 2020 2020 2020  eys():....      
+00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010690: 2020 2020 2020 2020 2020 2064 6175 6768             daugh
-000106a0: 7465 725f 7472 6163 6b5f 6964 203d 2020  ter_track_id =  
-000106b0: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
-000106c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000106d0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
-000106e0: 6f61 7428 6b29 295d 5b73 656c 662e 756e  oat(k))][self.un
-000106f0: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
-00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2020 2020 2020 2020 2020 2020 7061 7265              pare
-00010720: 6e74 5f74 7261 636b 5f69 6420 3d20 696e  nt_track_id = in
-00010730: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
-00010740: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00010750: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
-00010760: 7428 7629 295d 5b73 656c 662e 756e 6971  t(v))][self.uniq
-00010770: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
+00010690: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+000106a0: 7365 7428 6b2c 2073 7472 2873 656c 662e  set(k, str(self.
+000106b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000106c0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+000106d0: 6b5d 2929 2020 200d 0a0d 0a20 2020 2020  k]))   ....     
+000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010700: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00010710: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+00010720: 7472 6565 2e77 7269 7465 286f 732e 7061  tree.write(os.pa
+00010730: 7468 2e6a 6f69 6e28 7365 6c66 2e6d 6173  th.join(self.mas
+00010740: 7465 725f 786d 6c5f 7061 7468 2c20 7365  ter_xml_path, se
+00010750: 6c66 2e6d 6173 7465 725f 786d 6c5f 6e61  lf.master_xml_na
+00010760: 6d65 2929 0d0a 2020 2020 2020 2020 2020  me))..          
+00010770: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-000107a0: 7261 7068 5f74 7261 636b 735b 6461 7567  raph_tracks[daug
-000107b0: 6874 6572 5f74 7261 636b 5f69 645d 203d  hter_track_id] =
-000107c0: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-000107d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000107e0: 2020 7365 6c66 2e5f 6765 745f 6174 7472    self._get_attr
-000107f0: 6962 7574 6573 2829 0d0a 2020 2020 2020  ibutes()..      
-00010800: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00010810: 662e 636c 7573 7465 725f 6d6f 6465 6c20  f.cluster_model 
-00010820: 616e 6420 7365 6c66 2e73 6567 5f69 6d61  and self.seg_ima
-00010830: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00010840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010850: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-00010860: 7369 676e 5f63 6c75 7374 6572 5f63 6c61  sign_cluster_cla
-00010870: 7373 2829 0d0a 2020 2020 2020 2020 2020  ss()..          
-00010880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010890: 662e 5f63 7265 6174 655f 6d61 7374 6572  f._create_master
-000108a0: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
-000108b0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-000108c0: 6e74 203d 2030 200d 0a20 2020 2020 2020  nt = 0 ..       
-000108d0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
-000108e0: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
-000108f0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-00010900: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010790: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107c0: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
+000107d0: 6173 7369 676e 5f63 6c75 7374 6572 5f63  assign_cluster_c
+000107e0: 6c61 7373 2873 656c 6629 3a0d 0a20 2020  lass(self):..   
+000107f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00010800: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010810: 6c66 2e61 7865 7320 3d20 7365 6c66 2e61  lf.axes = self.a
+00010820: 7865 732e 7265 706c 6163 6528 2254 222c  xes.replace("T",
+00010830: 2022 2229 0d0a 2020 2020 2020 2020 2020   "")..          
+00010840: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010860: 666f 7220 636f 756e 742c 2074 696d 655f  for count, time_
+00010870: 6b65 7920 696e 2065 6e75 6d65 7261 7465  key in enumerate
+00010880: 2873 656c 662e 5f74 696d 6564 5f63 656e  (self._timed_cen
+00010890: 7472 6f69 642e 6b65 7973 2829 293a 0d0a  troid.keys()):..
+000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108d0: 2020 2020 2020 2020 7472 6565 2c20 7370          tree, sp
+000108e0: 6f74 5f63 656e 7472 6f69 6473 203d 2073  ot_centroids = s
+000108f0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+00010900: 6f69 645b 7469 6d65 5f6b 6579 5d0d 0a20  oid[time_key].. 
 00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010920: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00010930: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-00010940: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00010920: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00010930: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+00010940: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
 00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010970: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010980: 6261 722e 6c61 6265 6c20 3d20 224a 7573  bar.label = "Jus
-00010990: 7420 6f6e 6520 6d6f 7265 2074 6869 6e67  t one more thing
-000109a0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00010960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010970: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+00010980: 6162 656c 203d 2022 436f 6d70 7574 696e  abel = "Computin
+00010990: 6720 636c 7573 7465 7269 6e67 2063 6c61  g clustering cla
+000109a0: 7373 6573 220d 0a20 2020 2020 2020 2020  sses"..         
 000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000109d0: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
-000109e0: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
+000109c0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+000109d0: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
+000109e0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
 000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a10: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
-00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
 00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a40: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-00010a50: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-00010a60: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
-00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 2020 2020 2020 2020 6c65 6e28 7365 6c66          len(self
+00010a70: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+00010a80: 2e6b 6579 7328 2929 202b 2031 2c0d 0a20  .keys()) + 1,.. 
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010ad0: 6261 722e 7368 6f77 2829 0d0a 2020 2020  bar.show()..    
-00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-00010b10: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
-00010b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b40: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010b50: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-00010b60: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b90: 2020 2073 656c 662e 5f66 696e 616c 5f74     self._final_t
-00010ba0: 7261 636b 7328 7472 6163 6b5f 6964 2920  racks(track_id) 
-00010bb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00010bc0: 2020 2020 6966 2073 656c 662e 666f 7572      if self.four
-00010bd0: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
-00010be0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00010bf0: 636f 6d70 7574 696e 6720 466f 7572 6965  computing Fourie
-00010c00: 7227 290d 0a20 2020 2020 2020 2020 2020  r')..           
-00010c10: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
-00010c20: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
-00010c30: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
-00010c40: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00010c50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010c60: 2e5f 7465 6d70 6f72 616c 5f70 6c6f 7473  ._temporal_plots
-00010c70: 5f74 7261 636b 6d61 7465 2829 0d0a 2020  _trackmate()..  
-00010c80: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00010c90: 0d0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
-00010ca0: 655f 6d61 7374 6572 5f78 6d6c 2873 656c  e_master_xml(sel
-00010cb0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-00010cc0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00010cd0: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
-00010ce0: 626a 6563 7420 696e 2073 656c 662e 6d61  bject in self.ma
-00010cf0: 7374 6572 5f78 6d6c 5f72 6f6f 742e 6974  ster_xml_root.it
-00010d00: 6572 2827 5370 6f74 2729 3a0d 0a20 2020  er('Spot'):..   
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00010d30: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
-00010d40: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
-00010d50: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
-00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010d80: 6365 6c6c 5f69 6420 696e 2073 656c 662e  cell_id in self.
-00010d90: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00010da0: 6572 7469 6573 2e6b 6579 7328 293a 0d0a  erties.keys():..
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ac0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010af0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010b00: 7661 6c75 6520 3d20 2063 6f75 6e74 200d  value =  count .
+00010b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00010b40: 6172 2e73 686f 7728 290d 0a0d 0a20 2020  ar.show()....   
+00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b60: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+00010b70: 6576 616c 203d 2043 6c75 7374 6572 696e  eval = Clusterin
+00010b80: 6728 7365 6c66 2e73 6567 5f69 6d61 6765  g(self.seg_image
+00010b90: 5b69 6e74 2874 696d 655f 6b65 7929 2c3a  [int(time_key),:
+00010ba0: 5d2c 2020 7365 6c66 2e61 7865 732c 2073  ],  self.axes, s
+00010bb0: 656c 662e 6e75 6d5f 706f 696e 7473 2c20  elf.num_points, 
+00010bc0: 7365 6c66 2e63 6c75 7374 6572 5f6d 6f64  self.cluster_mod
+00010bd0: 656c 2c20 6b65 7920 3d20 7469 6d65 5f6b  el, key = time_k
+00010be0: 6579 2c20 7072 6f67 7265 7373 5f62 6172  ey, progress_bar
+00010bf0: 3d73 656c 662e 7072 6f67 7265 7373 5f62  =self.progress_b
+00010c00: 6172 2c20 6261 7463 685f 7369 7a65 203d  ar, batch_size =
+00010c10: 2073 656c 662e 6261 7463 685f 7369 7a65   self.batch_size
+00010c20: 2920 2020 2020 2020 0d0a 2020 2020 2020  )       ..      
+00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c40: 2020 2020 2063 6c75 7374 6572 5f65 7661       cluster_eva
+00010c50: 6c2e 5f63 7265 6174 655f 636c 7573 7465  l._create_cluste
+00010c60: 725f 6c61 6265 6c73 2829 0d0a 2020 2020  r_labels()..    
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c80: 2020 2020 2020 2074 696d 6564 5f63 6c75         timed_clu
+00010c90: 7374 6572 5f6c 6162 656c 203d 2063 6c75  ster_label = clu
+00010ca0: 7374 6572 5f65 7661 6c2e 7469 6d65 645f  ster_eval.timed_
+00010cb0: 636c 7573 7465 725f 6c61 6265 6c20 0d0a  cluster_label ..
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00010ce0: 745f 6c61 6265 6c73 2c20 6f75 7470 7574  t_labels, output
+00010cf0: 5f63 6c75 7374 6572 5f73 636f 7265 2c20  _cluster_score, 
+00010d00: 6f75 7470 7574 5f63 6c75 7374 6572 5f63  output_cluster_c
+00010d10: 6c61 7373 2c20 6f75 7470 7574 5f63 6c75  lass, output_clu
+00010d20: 7374 6572 5f63 656e 7472 6f69 642c 206f  ster_centroid, o
+00010d30: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
+00010d40: 6e74 7269 6369 7479 2c20 6f75 7470 7574  ntricity, output
+00010d50: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
+00010d60: 6374 6f72 2c20 6f75 7470 7574 5f63 6c6f  ctor, output_clo
+00010d70: 7564 5f73 7572 6661 6365 5f61 7265 6120  ud_surface_area 
+00010d80: 3d20 7469 6d65 645f 636c 7573 7465 725f  = timed_cluster_
+00010d90: 6c61 6265 6c5b 7469 6d65 5f6b 6579 5d0d  label[time_key].
+00010da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010db0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 666f 7220 6b20 696e 2073 656c 662e 756e  for k in self.un
-00010e10: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00010e20: 7469 6573 5b63 656c 6c5f 6964 5d2e 6b65  ties[cell_id].ke
-00010e30: 7973 2829 3a0d 0a0d 0a20 2020 2020 2020  ys():....       
-00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-00010e70: 6574 286b 2c20 7374 7228 7365 6c66 2e75  et(k, str(self.u
-00010e80: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00010e90: 7274 6965 735b 6365 6c6c 5f69 645d 5b6b  rties[cell_id][k
-00010ea0: 5d29 2920 2020 0d0a 0d0a 2020 2020 2020  ]))   ....      
+00010dd0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00010de0: 6e20 7261 6e67 6528 6c65 6e28 6f75 7470  n range(len(outp
+00010df0: 7574 5f63 6c75 7374 6572 5f63 656e 7472  ut_cluster_centr
+00010e00: 6f69 6429 293a 0d0a 2020 2020 2020 2020  oid)):..        
+00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e20: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
+00010e30: 726f 6964 203d 206f 7574 7075 745f 636c  roid = output_cl
+00010e40: 7573 7465 725f 6365 6e74 726f 6964 5b69  uster_centroid[i
+00010e50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e70: 2020 2020 2020 2063 6c75 7374 6572 5f63         cluster_c
+00010e80: 6c61 7373 203d 206f 7574 7075 745f 636c  lass = output_cl
+00010e90: 7573 7465 725f 636c 6173 735b 695d 0d0a  uster_class[i]..
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ed0: 0d0a 0d0a 2020 2020 2020 2020 2020 2073  ....           s
-00010ee0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f74  elf.master_xml_t
-00010ef0: 7265 652e 7772 6974 6528 6f73 2e70 6174  ree.write(os.pat
-00010f00: 682e 6a6f 696e 2873 656c 662e 6d61 7374  h.join(self.mast
-00010f10: 6572 5f78 6d6c 5f70 6174 682c 2073 656c  er_xml_path, sel
-00010f20: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
-00010f30: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-00010f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010ec0: 2020 2020 636c 7573 7465 725f 7363 6f72      cluster_scor
+00010ed0: 6520 3d20 6f75 7470 7574 5f63 6c75 7374  e = output_clust
+00010ee0: 6572 5f73 636f 7265 5b69 5d0d 0a20 2020  er_score[i]..   
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f10: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00010f20: 6d70 5f66 6972 7374 797a 203d 206f 7574  mp_firstyz = out
+00010f30: 7075 745f 636c 6f75 645f 6563 6365 6e74  put_cloud_eccent
+00010f40: 7269 6369 7479 5b69 5d0d 0a20 2020 2020  ricity[i]..     
 00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 0d0a 0d0a 2020 2020 6465 6620 5f61    ....    def _a
-00010fa0: 7373 6967 6e5f 636c 7573 7465 725f 636c  ssign_cluster_cl
-00010fb0: 6173 7328 7365 6c66 293a 0d0a 2020 2020  ass(self):..    
-00010fc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010fe0: 662e 6178 6573 203d 2073 656c 662e 6178  f.axes = self.ax
-00010ff0: 6573 2e72 6570 6c61 6365 2822 5422 2c20  es.replace("T", 
-00011000: 2222 290d 0a20 2020 2020 2020 2020 2020  "")..           
-00011010: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00011020: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011030: 6f72 2063 6f75 6e74 2c20 7469 6d65 5f6b  or count, time_k
-00011040: 6579 2069 6e20 656e 756d 6572 6174 6528  ey in enumerate(
-00011050: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
-00011060: 726f 6964 2e6b 6579 7328 2929 3a0d 0a20  roid.keys()):.. 
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00010f70: 656c 6c5f 6178 6973 203d 206f 7574 7075  ell_axis = outpu
+00010f80: 745f 6c61 7267 6573 745f 6569 6765 6e76  t_largest_eigenv
+00010f90: 6563 746f 725b 695d 0d0a 2020 2020 2020  ector[i]..      
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00010fc0: 7266 6163 655f 6172 6561 203d 206f 7574  rface_area = out
+00010fd0: 7075 745f 636c 6f75 645f 7375 7266 6163  put_cloud_surfac
+00010fe0: 655f 6172 6561 5b69 5d0d 0a20 2020 2020  e_area[i]..     
+00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011000: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00011010: 6973 742c 2069 6e64 6578 203d 2074 7265  ist, index = tre
+00011020: 652e 7175 6572 7928 6365 6e74 726f 6964  e.query(centroid
+00011030: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
+00011060: 656e 7472 6f69 6420 3d20 7370 6f74 5f63  entroid = spot_c
+00011070: 656e 7472 6f69 6473 5b69 6e64 6578 5d0d  entroids[index].
+00011080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2074 7265 652c 2073 706f         tree, spo
-000110b0: 745f 6365 6e74 726f 6964 7320 3d20 7365  t_centroids = se
-000110c0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
-000110d0: 6964 5b74 696d 655f 6b65 795d 0d0a 2020  id[time_key]..  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00011100: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-00011110: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011140: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-00011150: 6265 6c20 3d20 2243 6f6d 7075 7469 6e67  bel = "Computing
-00011160: 2063 6c75 7374 6572 696e 6720 636c 6173   clustering clas
-00011170: 7365 7322 0d0a 2020 2020 2020 2020 2020  ses"..          
+000110a0: 2020 2020 2066 7261 6d65 5f73 706f 745f       frame_spot_
+000110b0: 6365 6e74 726f 6964 203d 2028 696e 7428  centroid = (int(
+000110c0: 7469 6d65 5f6b 6579 292c 636c 6f73 6573  time_key),closes
+000110d0: 745f 6365 6e74 726f 6964 5b30 5d2c 2063  t_centroid[0], c
+000110e0: 6c6f 7365 7374 5f63 656e 7472 6f69 645b  losest_centroid[
+000110f0: 315d 2c20 636c 6f73 6573 745f 6365 6e74  1], closest_cent
+00011100: 726f 6964 5b32 5d29 0d0a 2020 2020 2020  roid[2])..      
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00011130: 6f73 6573 745f 6365 6c6c 5f69 6420 3d20  osest_cell_id = 
+00011140: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00011150: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
+00011160: 7370 6f74 5f63 656e 7472 6f69 645d 0d0a  spot_centroid]..
+00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-000111a0: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-000111b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111f0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
-00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-00011240: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
-00011250: 6b65 7973 2829 2920 2b20 312c 0d0a 2020  keys()) + 1,..  
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011290: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00011190: 2020 2020 6d61 736b 5f76 6563 746f 7220      mask_vector 
+000111a0: 3d20 5b20 666c 6f61 7428 7365 6c66 2e75  = [ float(self.u
+000111b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000111c0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+000111d0: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
+000111e0: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
+000111f0: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
+00011200: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00011210: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00011220: 7365 7374 5f63 656c 6c5f 6964 295d 5b73  sest_cell_id)][s
+00011230: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00011240: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+00011250: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00011260: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00011270: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00011280: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+00011290: 6f69 645f 7a5f 6b65 795d 2920 5d0d 0a20  oid_z_key]) ].. 
 000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000112c0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
-000112d0: 616c 7565 203d 2020 636f 756e 7420 0d0a  alue =  count ..
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011300: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00011310: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 2020 2020 2020 2063 6c75 7374 6572 5f65         cluster_e
-00011340: 7661 6c20 3d20 436c 7573 7465 7269 6e67  val = Clustering
-00011350: 2873 656c 662e 7365 675f 696d 6167 655b  (self.seg_image[
-00011360: 696e 7428 7469 6d65 5f6b 6579 292c 3a5d  int(time_key),:]
-00011370: 2c20 2073 656c 662e 6178 6573 2c20 7365  ,  self.axes, se
-00011380: 6c66 2e6e 756d 5f70 6f69 6e74 732c 2073  lf.num_points, s
-00011390: 656c 662e 636c 7573 7465 725f 6d6f 6465  elf.cluster_mode
-000113a0: 6c2c 206b 6579 203d 2074 696d 655f 6b65  l, key = time_ke
-000113b0: 792c 2070 726f 6772 6573 735f 6261 723d  y, progress_bar=
-000113c0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-000113d0: 722c 2062 6174 6368 5f73 697a 6520 3d20  r, batch_size = 
-000113e0: 7365 6c66 2e62 6174 6368 5f73 697a 6529  self.batch_size)
-000113f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011410: 2020 2020 636c 7573 7465 725f 6576 616c      cluster_eval
-00011420: 2e5f 6372 6561 7465 5f63 6c75 7374 6572  ._create_cluster
-00011430: 5f6c 6162 656c 7328 290d 0a20 2020 2020  _labels()..     
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
+000112d0: 6b20 3d20 616e 6775 6c61 725f 6368 616e  k = angular_chan
+000112e0: 6765 2863 656c 6c5f 6178 6973 2c20 6d61  ge(cell_axis, ma
+000112f0: 736b 5f76 6563 746f 7229 0d0a 2020 2020  sk_vector)..    
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00011350: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011360: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00011370: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00011380: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
+00011390: 736b 5f6b 6579 203a 2063 656c 6c5f 6178  sk_key : cell_ax
+000113a0: 6973 5f6d 6173 6b7d 290d 0a20 2020 2020  is_mask})..     
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000113d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000113e0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000113f0: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00011400: 2e75 7064 6174 6528 7b73 656c 662e 636c  .update({self.cl
+00011410: 7573 7465 7263 6c61 7373 5f6b 6579 203a  usterclass_key :
+00011420: 2063 6c75 7374 6572 5f63 6c61 7373 7d29   cluster_class})
+00011430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2020 2020 7469 6d65 645f 636c 7573        timed_clus
-00011460: 7465 725f 6c61 6265 6c20 3d20 636c 7573  ter_label = clus
-00011470: 7465 725f 6576 616c 2e74 696d 6564 5f63  ter_eval.timed_c
-00011480: 6c75 7374 6572 5f6c 6162 656c 200d 0a20  luster_label .. 
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114a0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-000114b0: 5f6c 6162 656c 732c 206f 7574 7075 745f  _labels, output_
-000114c0: 636c 7573 7465 725f 7363 6f72 652c 206f  cluster_score, o
-000114d0: 7574 7075 745f 636c 7573 7465 725f 636c  utput_cluster_cl
-000114e0: 6173 732c 206f 7574 7075 745f 636c 7573  ass, output_clus
-000114f0: 7465 725f 6365 6e74 726f 6964 2c20 6f75  ter_centroid, ou
-00011500: 7470 7574 5f63 6c6f 7564 5f65 6363 656e  tput_cloud_eccen
-00011510: 7472 6963 6974 792c 206f 7574 7075 745f  tricity, output_
-00011520: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00011530: 746f 722c 206f 7574 7075 745f 636c 6f75  tor, output_clou
-00011540: 645f 7375 7266 6163 655f 6172 6561 203d  d_surface_area =
-00011550: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
-00011560: 6162 656c 5b74 696d 655f 6b65 795d 0d0a  abel[time_key]..
-00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011580: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000115b0: 2072 616e 6765 286c 656e 286f 7574 7075   range(len(outpu
-000115c0: 745f 636c 7573 7465 725f 6365 6e74 726f  t_cluster_centro
-000115d0: 6964 2929 3a0d 0a20 2020 2020 2020 2020  id)):..         
-000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 2020 2020 2020 2020 2020 2063 656e 7472             centr
-00011600: 6f69 6420 3d20 6f75 7470 7574 5f63 6c75  oid = output_clu
-00011610: 7374 6572 5f63 656e 7472 6f69 645b 695d  ster_centroid[i]
-00011620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011640: 2020 2020 2020 636c 7573 7465 725f 636c        cluster_cl
-00011650: 6173 7320 3d20 6f75 7470 7574 5f63 6c75  ass = output_clu
-00011660: 7374 6572 5f63 6c61 7373 5b69 5d0d 0a20  ster_class[i].. 
-00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011690: 2020 2063 6c75 7374 6572 5f73 636f 7265     cluster_score
-000116a0: 203d 206f 7574 7075 745f 636c 7573 7465   = output_cluste
-000116b0: 725f 7363 6f72 655b 695d 0d0a 2020 2020  r_score[i]..    
-000116c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116e0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-000116f0: 705f 6669 7273 7479 7a20 3d20 6f75 7470  p_firstyz = outp
-00011700: 7574 5f63 6c6f 7564 5f65 6363 656e 7472  ut_cloud_eccentr
-00011710: 6963 6974 795b 695d 0d0a 2020 2020 2020  icity[i]..      
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011730: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00011740: 6c6c 5f61 7869 7320 3d20 6f75 7470 7574  ll_axis = output
-00011750: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
-00011760: 6374 6f72 5b69 5d0d 0a20 2020 2020 2020  ctor[i]..       
-00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2020 2020 2073 7572               sur
-00011790: 6661 6365 5f61 7265 6120 3d20 6f75 7470  face_area = outp
-000117a0: 7574 5f63 6c6f 7564 5f73 7572 6661 6365  ut_cloud_surface
-000117b0: 5f61 7265 615b 695d 0d0a 2020 2020 2020  _area[i]..      
-000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-000117e0: 7374 2c20 696e 6465 7820 3d20 7472 6565  st, index = tree
-000117f0: 2e71 7565 7279 2863 656e 7472 6f69 6429  .query(centroid)
-00011800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 2020 2020 636c 6f73 6573 745f 6365        closest_ce
-00011830: 6e74 726f 6964 203d 2073 706f 745f 6365  ntroid = spot_ce
-00011840: 6e74 726f 6964 735b 696e 6465 785d 0d0a  ntroids[index]..
-00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011870: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
-00011880: 656e 7472 6f69 6420 3d20 2869 6e74 2874  entroid = (int(t
-00011890: 696d 655f 6b65 7929 2c63 6c6f 7365 7374  ime_key),closest
-000118a0: 5f63 656e 7472 6f69 645b 305d 2c20 636c  _centroid[0], cl
-000118b0: 6f73 6573 745f 6365 6e74 726f 6964 5b31  osest_centroid[1
-000118c0: 5d2c 2063 6c6f 7365 7374 5f63 656e 7472  ], closest_centr
-000118d0: 6f69 645b 325d 290d 0a20 2020 2020 2020  oid[2])..       
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118f0: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
-00011900: 7365 7374 5f63 656c 6c5f 6964 203d 2073  sest_cell_id = s
-00011910: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00011920: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
-00011930: 706f 745f 6365 6e74 726f 6964 5d0d 0a20  pot_centroid].. 
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011960: 2020 206d 6173 6b5f 7665 6374 6f72 203d     mask_vector =
-00011970: 205b 2066 6c6f 6174 2873 656c 662e 756e   [ float(self.un
-00011980: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011990: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-000119a0: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
-000119b0: 6d61 736b 6365 6e74 726f 6964 5f78 5f6b  maskcentroid_x_k
-000119c0: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
-000119d0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000119e0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-000119f0: 6573 745f 6365 6c6c 5f69 6429 5d5b 7365  est_cell_id)][se
-00011a00: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-00011a10: 795f 6b65 795d 292c 2066 6c6f 6174 2873  y_key]), float(s
-00011a20: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00011a30: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00011a40: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00011a50: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
-00011a60: 6964 5f7a 5f6b 6579 5d29 205d 0d0a 2020  id_z_key]) ]..  
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a90: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
-00011aa0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-00011ab0: 6528 6365 6c6c 5f61 7869 732c 206d 6173  e(cell_axis, mas
-00011ac0: 6b5f 7665 6374 6f72 290d 0a20 2020 2020  k_vector)..     
-00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ae0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00011af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b10: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00011b20: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011b30: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00011b40: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00011b50: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
-00011b60: 6b5f 6b65 7920 3a20 6365 6c6c 5f61 7869  k_key : cell_axi
-00011b70: 735f 6d61 736b 7d29 0d0a 2020 2020 2020  s_mask})..      
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011ba0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00011bb0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00011bc0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00011bd0: 7570 6461 7465 287b 7365 6c66 2e63 6c75  update({self.clu
-00011be0: 7374 6572 636c 6173 735f 6b65 7920 3a20  sterclass_key : 
-00011bf0: 636c 7573 7465 725f 636c 6173 737d 290d  cluster_class}).
-00011c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c20: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00011c30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011c40: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00011c50: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00011c60: 656c 662e 636c 7573 7465 7273 636f 7265  elf.clusterscore
-00011c70: 5f6b 6579 203a 2063 6c75 7374 6572 5f73  _key : cluster_s
-00011c80: 636f 7265 7d29 0d0a 2020 2020 2020 2020  core})..        
-00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011cb0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00011cc0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-00011cd0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-00011ce0: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
-00011cf0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00011d00: 7374 6b65 7920 3a20 6563 6365 6e74 7269  stkey : eccentri
-00011d10: 6369 7479 5f63 6f6d 705f 6669 7273 7479  city_comp_firsty
-00011d20: 7a5b 305d 7d29 0d0a 2020 2020 2020 2020  z[0]})..        
-00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011d50: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00011d60: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-00011d70: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-00011d80: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
-00011d90: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00011da0: 6f6e 646b 6579 203a 2065 6363 656e 7472  ondkey : eccentr
-00011db0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00011dc0: 797a 5b31 5d7d 290d 0a20 2020 2020 2020  yz[1]})..       
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011df0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00011e00: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00011e10: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00011e20: 7064 6174 6528 7b73 656c 662e 7375 7266  pdate({self.surf
-00011e30: 6163 655f 6172 6561 5f6b 6579 203a 2073  ace_area_key : s
-00011e40: 7572 6661 6365 5f61 7265 617d 290d 0a0d  urface_area})...
-00011e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e70: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-00011ea0: 656c 662e 726f 6f74 5f73 706f 7473 2e69  elf.root_spots.i
-00011eb0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ed0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011ee0: 726f 6f74 5f73 706f 7473 5b6b 5d20 3d20  root_spots[k] = 
-00011ef0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011f00: 5f70 726f 7065 7274 6965 735b 6b5d 2020  _properties[k]  
-00011f10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00011f20: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
-00011f30: 6566 205f 636f 6d70 7574 655f 7068 656e  ef _compute_phen
-00011f40: 6f74 7970 6573 2873 656c 6629 3a0d 0a0d  otypes(self):...
-00011f50: 0a20 2020 2020 2020 2020 2066 6f72 2028  .          for (
-00011f60: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-00011f70: 7175 655f 7472 6163 6b73 2e69 7465 6d73  que_tracks.items
-00011f80: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00011f90: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011fa0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-00011fb0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
-00011fc0: 2020 2020 2074 7261 636b 6c65 745f 7072       tracklet_pr
-00011fd0: 6f70 6572 7469 6573 203d 2073 656c 662e  operties = self.
-00011fe0: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
-00011ff0: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00012000: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00012010: 6b73 203d 2073 656c 662e 756e 6971 7565  ks = self.unique
-00012020: 5f74 7261 636b 735b 6b5d 0d0a 2020 2020  _tracks[k]..    
-00012030: 2020 2020 2020 2020 2020 2020 5a20 3d20              Z = 
-00012040: 7472 6163 6b73 5b3a 2c32 5d0d 0a20 2020  tracks[:,2]..   
-00012050: 2020 2020 2020 2020 2020 2020 2059 203d               Y =
-00012060: 2074 7261 636b 735b 3a2c 335d 0d0a 2020   tracks[:,3]..  
-00012070: 2020 2020 2020 2020 2020 2020 2020 5820                X 
-00012080: 3d20 7472 6163 6b73 5b3a 2c34 5d0d 0a20  = tracks[:,4].. 
-00012090: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000120a0: 696d 6520 3d20 7472 6163 6b6c 6574 5f70  ime = tracklet_p
-000120b0: 726f 7065 7274 6965 735b 3a2c 305d 0d0a  roperties[:,0]..
-000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120d0: 756e 6971 7565 5f69 6473 203d 2074 7261  unique_ids = tra
-000120e0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000120f0: 5b3a 2c31 5d0d 0a20 2020 2020 2020 2020  [:,1]..         
-00012100: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-00012110: 735f 7365 7420 3d20 7365 7428 756e 6971  s_set = set(uniq
-00012120: 7565 5f69 6473 290d 0a20 2020 2020 2020  ue_ids)..       
-00012130: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-00012140: 696f 6e5f 6964 7320 3d20 7472 6163 6b6c  ion_ids = trackl
-00012150: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00012160: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00012170: 2020 2020 7261 6469 7573 203d 2074 7261      radius = tra
-00012180: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00012190: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
-000121a0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
-000121b0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-000121c0: 6965 735b 3a2c 345d 0d0a 2020 2020 2020  ies[:,4]..      
-000121d0: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-000121e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000121f0: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
-00012200: 7065 7274 6965 735b 3a2c 355d 0d0a 2020  perties[:,5]..  
-00012210: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00012220: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00012230: 7365 636f 6e64 203d 2074 7261 636b 6c65  second = trackle
-00012240: 745f 7072 6f70 6572 7469 6573 5b3a 2c36  t_properties[:,6
-00012250: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012260: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
-00012270: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012280: 7274 6965 735b 3a2c 375d 0d0a 2020 2020  rties[:,7]..    
-00012290: 2020 2020 2020 2020 2020 2020 636c 7573              clus
-000122a0: 7465 725f 636c 6173 7320 3d20 7472 6163  ter_class = trac
-000122b0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-000122c0: 3a2c 385d 0d0a 2020 2020 2020 2020 2020  :,8]..          
-000122d0: 2020 2020 2020 636c 7573 7465 725f 636c        cluster_cl
-000122e0: 6173 735f 7363 6f72 6520 3d20 7472 6163  ass_score = trac
-000122f0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00012300: 3a2c 395d 0d0a 2020 2020 2020 2020 2020  :,9]..          
-00012310: 2020 2020 2020 696e 7465 6e73 6974 7920        intensity 
-00012320: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012330: 7274 6965 735b 3a2c 3130 5d0d 0a20 2020  rties[:,10]..   
-00012340: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-00012350: 6564 203d 2074 7261 636b 6c65 745f 7072  ed = tracklet_pr
-00012360: 6f70 6572 7469 6573 5b3a 2c31 315d 0d0a  operties[:,11]..
-00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012380: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 2074  motion_angle = t
-00012390: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000123a0: 6573 5b3a 2c31 325d 0d0a 2020 2020 2020  es[:,12]..      
-000123b0: 2020 2020 2020 2020 2020 6163 6365 6c65            accele
-000123c0: 7261 7469 6f6e 203d 2074 7261 636b 6c65  ration = trackle
-000123d0: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-000123e0: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
-000123f0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-00012400: 6c5f 6d61 736b 203d 2074 7261 636b 6c65  l_mask = trackle
-00012410: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-00012420: 345d 0d0a 2020 2020 2020 2020 2020 2020  4]..            
-00012430: 2020 2020 7261 6469 616c 5f61 6e67 6c65      radial_angle
-00012440: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00012450: 6572 7469 6573 5b3a 2c31 355d 0d0a 2020  erties[:,15]..  
-00012460: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00012470: 6c6c 5f61 7869 735f 6d61 736b 203d 2074  ll_axis_mask = t
-00012480: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00012490: 6573 5b3a 2c31 365d 0d0a 0d0a 0d0a 2020  es[:,16]......  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-000124d0: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
-000124e0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-000124f0: 2020 2020 2075 6e69 7175 655f 636c 7573       unique_clus
-00012500: 7465 725f 7072 6f70 6572 7469 6573 5f74  ter_properties_t
-00012510: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
-00012520: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012530: 6c66 2e75 6e69 7175 655f 6666 745f 7072  lf.unique_fft_pr
-00012540: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-00012550: 645d 203d 207b 7d0d 0a20 2020 2020 2020  d] = {}..       
-00012560: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00012570: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
-00012580: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00012590: 5d20 3d20 7b7d 0d0a 0d0a 2020 2020 2020  ] = {}....      
-000125a0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-000125b0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-000125c0: 735f 7472 6163 6b6c 6574 203d 207b 7d0d  s_tracklet = {}.
-000125d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125e0: 2075 6e69 7175 655f 6479 6e61 6d69 635f   unique_dynamic_
-000125f0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00012600: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
-00012610: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00012620: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00012630: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00012640: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00012650: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012660: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-00012670: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
-00012680: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00012690: 2020 2020 2020 6578 7061 6e64 6564 5f74        expanded_t
-000126a0: 696d 6520 3d20 6e70 2e7a 6572 6f73 2873  ime = np.zeros(s
-000126b0: 656c 662e 7465 6e64 202d 2073 656c 662e  elf.tend - self.
-000126c0: 7473 7461 7274 202b 2031 290d 0a20 2020  tstart + 1)..   
-000126d0: 2020 2020 2020 2020 2020 2020 2070 6f69               poi
-000126e0: 6e74 5f73 616d 706c 6520 3d20 6578 7061  nt_sample = expa
-000126f0: 6e64 6564 5f74 696d 652e 7368 6170 655b  nded_time.shape[
-00012700: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-00012710: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00012720: 6765 286c 656e 2865 7870 616e 6465 645f  ge(len(expanded_
-00012730: 7469 6d65 2929 3a0d 0a20 2020 2020 2020  time)):..       
-00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012750: 6578 7061 6e64 6564 5f74 696d 655b 695d  expanded_time[i]
-00012760: 203d 2069 200d 0a20 2020 2020 2020 2020   = i ..         
-00012770: 2020 2020 2020 2066 6f72 2063 7572 7265         for curre
-00012780: 6e74 5f75 6e69 7175 655f 6964 2069 6e20  nt_unique_id in 
-00012790: 756e 6971 7565 5f69 6473 5f73 6574 3a0d  unique_ids_set:.
-000127a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000127b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000127c0: 2020 2020 2020 2020 2065 7870 616e 6465           expande
-000127d0: 645f 696e 7465 6e73 6974 7920 3d20 6e70  d_intensity = np
-000127e0: 2e7a 6572 6f73 2873 656c 662e 7465 6e64  .zeros(self.tend
-000127f0: 202d 2073 656c 662e 7473 7461 7274 202b   - self.tstart +
-00012800: 2031 290d 0a20 2020 2020 2020 2020 2020   1)..           
-00012810: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012820: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
-00012850: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012860: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012870: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00012880: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012890: 6e74 5f79 203d 205b 5d0d 0a20 2020 2020  nt_y = []..     
-000128a0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000128b0: 7272 656e 745f 7820 3d20 5b5d 0d0a 2020  rrent_x = []..  
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128d0: 2063 7572 7265 6e74 5f69 6e74 656e 7369   current_intensi
-000128e0: 7479 203d 205b 5d0d 0a20 2020 2020 2020  ty = []..       
-000128f0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012900: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
-00012910: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00012920: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012930: 6e74 5f63 6c75 7374 6572 5f63 6c61 7373  nt_cluster_class
-00012940: 5f73 636f 7265 203d 205b 5d0d 0a20 2020  _score = []..   
-00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012960: 6375 7272 656e 745f 7261 6469 7573 203d  current_radius =
-00012970: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012980: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012990: 766f 6c75 6d65 203d 205b 5d0d 0a20 2020  volume = []..   
-000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129b0: 6375 7272 656e 745f 7370 6565 6420 3d20  current_speed = 
-000129c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000129d0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-000129e0: 6f74 696f 6e5f 616e 676c 6520 3d20 5b5d  otion_angle = []
-000129f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012a00: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
-00012a10: 656c 6572 6174 696f 6e20 3d20 5b5d 0d0a  eleration = []..
-00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a30: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-00012a40: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-00012a50: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00012a60: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-00012a70: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00012a80: 5f66 6972 7374 203d 205b 5d0d 0a20 2020  _first = []..   
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00012ab0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-00012ac0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012ad0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012ae0: 745f 7375 7266 6163 655f 6172 6561 203d  t_surface_area =
-00012af0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00012b00: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012b10: 745f 7261 6469 616c 5f61 6e67 6c65 203d  t_radial_angle =
-00012b20: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012b30: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012b40: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
-00012b50: 205b 5d20 0d0a 2020 2020 2020 2020 2020   [] ..          
-00012b60: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012b70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00012b80: 7220 6a20 696e 2072 616e 6765 2874 696d  r j in range(tim
-00012b90: 652e 7368 6170 655b 305d 293a 0d0a 2020  e.shape[0]):..  
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2020 2020 2020 6966 2063 7572 7265          if curre
-00012bc0: 6e74 5f75 6e69 7175 655f 6964 203d 3d20  nt_unique_id == 
-00012bd0: 756e 6971 7565 5f69 6473 5b6a 5d3a 0d0a  unique_ids[j]:..
-00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c00: 2063 7572 7265 6e74 5f74 696d 652e 6170   current_time.ap
-00012c10: 7065 6e64 2874 696d 655b 6a5d 290d 0a20  pend(time[j]).. 
-00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c40: 6375 7272 656e 745f 7a2e 6170 7065 6e64  current_z.append
-00012c50: 285a 5b6a 5d29 0d0a 2020 2020 2020 2020  (Z[j])..        
-00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012c80: 5f79 2e61 7070 656e 6428 595b 6a5d 290d  _y.append(Y[j]).
-00012c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cb0: 2020 6375 7272 656e 745f 782e 6170 7065    current_x.appe
-00012cc0: 6e64 2858 5b6a 5d29 0d0a 2020 2020 2020  nd(X[j])..      
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ce0: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-00012cf0: 6465 645f 696e 7465 6e73 6974 795b 696e  ded_intensity[in
-00012d00: 7428 7469 6d65 5b6a 5d29 5d20 3d20 696e  t(time[j])] = in
-00012d10: 7465 6e73 6974 795b 6a5d 0d0a 2020 2020  tensity[j]..    
-00012d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d30: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012d40: 7265 6e74 5f69 6e74 656e 7369 7479 2e61  rent_intensity.a
-00012d50: 7070 656e 6428 696e 7465 6e73 6974 795b  ppend(intensity[
-00012d60: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
-00012d90: 7573 7465 725f 636c 6173 732e 6170 7065  uster_class.appe
-00012da0: 6e64 2863 6c75 7374 6572 5f63 6c61 7373  nd(cluster_class
-00012db0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dd0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00012de0: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
-00012df0: 7265 2e61 7070 656e 6428 636c 7573 7465  re.append(cluste
-00012e00: 725f 636c 6173 735f 7363 6f72 655b 6a5d  r_class_score[j]
-00012e10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-00012e40: 7573 2e61 7070 656e 6428 7261 6469 7573  us.append(radius
-00012e50: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e70: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
-00012e80: 6f6c 756d 652e 6170 7065 6e64 2876 6f6c  olume.append(vol
-00012e90: 756d 655b 6a5d 290d 0a20 2020 2020 2020  ume[j])..       
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012eb0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012ec0: 745f 7370 6565 642e 6170 7065 6e64 2873  t_speed.append(s
-00012ed0: 7065 6564 5b6a 5d29 0d0a 2020 2020 2020  peed[j])..      
-00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ef0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012f00: 6e74 5f6d 6f74 696f 6e5f 616e 676c 652e  nt_motion_angle.
-00012f10: 6170 7065 6e64 286d 6f74 696f 6e5f 616e  append(motion_an
-00012f20: 676c 655b 6a5d 290d 0a20 2020 2020 2020  gle[j])..       
-00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012f50: 745f 6163 6365 6c65 7261 7469 6f6e 2e61  t_acceleration.a
-00012f60: 7070 656e 6428 6163 6365 6c65 7261 7469  ppend(accelerati
-00012f70: 6f6e 5b6a 5d29 0d0a 2020 2020 2020 2020  on[j])..        
-00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f90: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00012fa0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00012fb0: 6173 6b2e 6170 7065 6e64 2864 6973 7461  ask.append(dista
-00012fc0: 6e63 655f 6365 6c6c 5f6d 6173 6b5b 6a5d  nce_cell_mask[j]
-00012fd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ff0: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-00013000: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00013010: 7273 742e 6170 7065 6e64 2865 6363 656e  rst.append(eccen
-00013020: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00013030: 7374 5b6a 5d29 0d0a 2020 2020 2020 2020  st[j])..        
-00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013060: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00013070: 6d70 5f73 6563 6f6e 642e 6170 7065 6e64  mp_second.append
-00013080: 2865 6363 656e 7472 6963 6974 795f 636f  (eccentricity_co
-00013090: 6d70 5f73 6563 6f6e 645b 6a5d 290d 0a20  mp_second[j]).. 
-000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130c0: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
-000130d0: 6172 6561 2e61 7070 656e 6428 7375 7266  area.append(surf
-000130e0: 6163 655f 6172 6561 5b6a 5d29 0d0a 2020  ace_area[j])..  
-000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013110: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
-00013120: 676c 652e 6170 7065 6e64 2872 6164 6961  gle.append(radia
-00013130: 6c5f 616e 676c 655b 6a5d 290d 0a20 2020  l_angle[j])..   
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013160: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
-00013170: 6d61 736b 2e61 7070 656e 6428 6365 6c6c  mask.append(cell
-00013180: 5f61 7869 735f 6d61 736b 5b6a 5d29 0d0a  _axis_mask[j])..
-00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131a0: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-000131b0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-000131c0: 7265 6e74 5f74 696d 6529 0d0a 2020 2020  rent_time)..    
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000131e0: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
-000131f0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00013200: 7272 656e 745f 696e 7465 6e73 6974 7929  rrent_intensity)
-00013210: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
-00013220: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013230: 5f63 6c75 7374 6572 5f63 6c61 7373 203d  _cluster_class =
-00013240: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00013250: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
-00013260: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00013270: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00013280: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
-00013290: 7265 203d 206e 702e 6173 6172 7261 7928  re = np.asarray(
-000132a0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
-000132b0: 636c 6173 735f 7363 6f72 6529 2020 200d  class_score)   .
-000132c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000132d0: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
-000132e0: 6469 7573 203d 206e 702e 6173 6172 7261  dius = np.asarra
-000132f0: 7928 6375 7272 656e 745f 7261 6469 7573  y(current_radius
-00013300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013310: 2020 2020 2020 6375 7272 656e 745f 766f        current_vo
-00013320: 6c75 6d65 203d 206e 702e 6173 6172 7261  lume = np.asarra
-00013330: 7928 6375 7272 656e 745f 766f 6c75 6d65  y(current_volume
-00013340: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013350: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-00013360: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00013370: 6669 7273 7420 3d20 6e70 2e61 7361 7272  first = np.asarr
-00013380: 6179 2863 7572 7265 6e74 5f65 6363 656e  ay(current_eccen
-00013390: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-000133a0: 7374 290d 0a20 2020 2020 2020 2020 2020  st)..           
-000133b0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000133c0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-000133d0: 705f 7365 636f 6e64 203d 206e 702e 6173  p_second = np.as
-000133e0: 6172 7261 7928 6375 7272 656e 745f 6563  array(current_ec
-000133f0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00013400: 7365 636f 6e64 290d 0a20 2020 2020 2020  second)..       
-00013410: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013420: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
-00013430: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00013440: 7272 656e 745f 7375 7266 6163 655f 6172  rrent_surface_ar
-00013450: 6561 290d 0a0d 0a20 2020 2020 2020 2020  ea)....         
-00013460: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013470: 745f 7370 6565 6420 3d20 6e70 2e61 7361  t_speed = np.asa
-00013480: 7272 6179 2863 7572 7265 6e74 5f73 7065  rray(current_spe
-00013490: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
-000134a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000134b0: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 206e  motion_angle = n
-000134c0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-000134d0: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 290d  t_motion_angle).
-000134e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000134f0: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-00013500: 6c65 7261 7469 6f6e 203d 206e 702e 6173  leration = np.as
-00013510: 6172 7261 7928 6375 7272 656e 745f 6163  array(current_ac
-00013520: 6365 6c65 7261 7469 6f6e 290d 0a20 2020  celeration)..   
-00013530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013540: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-00013550: 5f63 656c 6c5f 6d61 736b 203d 206e 702e  _cell_mask = np.
-00013560: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00013570: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00013580: 736b 290d 0a20 2020 2020 2020 2020 2020  sk)..           
-00013590: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000135a0: 7261 6469 616c 5f61 6e67 6c65 203d 206e  radial_angle = n
-000135b0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-000135c0: 745f 7261 6469 616c 5f61 6e67 6c65 290d  t_radial_angle).
-000135d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000135e0: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
-000135f0: 5f61 7869 735f 6d61 736b 203d 206e 702e  _axis_mask = np.
-00013600: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00013610: 6365 6c6c 5f61 7869 735f 6d61 736b 290d  cell_axis_mask).
-00013620: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00013630: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00013640: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00013650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013660: 2020 6966 2070 6f69 6e74 5f73 616d 706c    if point_sampl
-00013670: 6520 3e20 303a 0d0a 2020 2020 2020 2020  e > 0:..        
-00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013690: 2020 2020 2020 2020 7866 5f73 616d 706c          xf_sampl
-000136a0: 6520 3d20 6666 7466 7265 7128 706f 696e  e = fftfreq(poin
-000136b0: 745f 7361 6d70 6c65 2c20 7365 6c66 2e74  t_sample, self.t
-000136c0: 6361 6c69 6272 6174 696f 6e29 0d0a 2020  calibration)..  
-000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136e0: 2020 2020 2020 2020 2020 2020 2020 6666                ff
-000136f0: 7473 7472 6970 5f73 616d 706c 6520 3d20  tstrip_sample = 
-00013700: 6666 7428 6578 7061 6e64 6564 5f69 6e74  fft(expanded_int
-00013710: 656e 7369 7479 290d 0a20 2020 2020 2020  ensity)..       
-00013720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013730: 2020 2020 2020 2020 2066 6674 746f 7461           ffttota
-00013740: 6c5f 7361 6d70 6c65 203d 206e 702e 6162  l_sample = np.ab
-00013750: 7328 6666 7473 7472 6970 5f73 616d 706c  s(fftstrip_sampl
-00013760: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013780: 2020 2020 7866 5f73 616d 706c 6520 3d20      xf_sample = 
-00013790: 7866 5f73 616d 706c 655b 3020 3a20 6c65  xf_sample[0 : le
-000137a0: 6e28 7866 5f73 616d 706c 6529 202f 2f20  n(xf_sample) // 
-000137b0: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-000137c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137d0: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
-000137e0: 706c 6520 3d20 6666 7474 6f74 616c 5f73  ple = ffttotal_s
-000137f0: 616d 706c 655b 3020 3a20 6c65 6e28 6666  ample[0 : len(ff
-00013800: 7474 6f74 616c 5f73 616d 706c 6529 202f  ttotal_sample) /
-00013810: 2f20 325d 0d0a 0d0a 2020 2020 2020 2020  / 2]....        
-00013820: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00013830: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-00013840: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00013850: 745f 756e 6971 7565 5f69 645d 203d 2065  t_unique_id] = e
-00013860: 7870 616e 6465 645f 7469 6d65 2c20 6578  xpanded_time, ex
-00013870: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
-00013880: 2c20 7866 5f73 616d 706c 652c 2066 6674  , xf_sample, fft
-00013890: 746f 7461 6c5f 7361 6d70 6c65 0d0a 2020  total_sample..  
-000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2075 6e69 7175 655f 636c 7573 7465 725f   unique_cluster_
-000138c0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-000138d0: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-000138e0: 7565 5f69 645d 203d 2020 6375 7272 656e  ue_id] =  curren
-000138f0: 745f 7469 6d65 2c20 6375 7272 656e 745f  t_time, current_
-00013900: 636c 7573 7465 725f 636c 6173 732c 2063  cluster_class, c
-00013910: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
-00013920: 6c61 7373 5f73 636f 7265 0d0a 2020 2020  lass_score..    
-00013930: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00013940: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00013950: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-00013960: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00013970: 645d 203d 2063 7572 7265 6e74 5f74 696d  d] = current_tim
-00013980: 652c 2063 7572 7265 6e74 5f7a 2c20 6375  e, current_z, cu
-00013990: 7272 656e 745f 792c 2063 7572 7265 6e74  rrent_y, current
-000139a0: 5f78 2c20 6375 7272 656e 745f 7261 6469  _x, current_radi
-000139b0: 7573 2c20 6375 7272 656e 745f 766f 6c75  us, current_volu
-000139c0: 6d65 2c20 6375 7272 656e 745f 6563 6365  me, current_ecce
-000139d0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-000139e0: 7273 742c 2063 7572 7265 6e74 5f65 6363  rst, current_ecc
-000139f0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00013a00: 6563 6f6e 642c 2063 7572 7265 6e74 5f73  econd, current_s
-00013a10: 7572 6661 6365 5f61 7265 612c 2063 7572  urface_area, cur
-00013a20: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
-00013a30: 7373 2c20 6375 7272 656e 745f 636c 7573  ss, current_clus
-00013a40: 7465 725f 636c 6173 735f 7363 6f72 650d  ter_class_score.
-00013a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a60: 2020 2020 756e 6971 7565 5f64 796e 616d      unique_dynam
-00013a70: 6963 5f70 726f 7065 7274 6965 735f 7472  ic_properties_tr
-00013a80: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
-00013a90: 6e69 7175 655f 6964 5d20 3d20 6375 7272  nique_id] = curr
-00013aa0: 656e 745f 7469 6d65 2c20 6375 7272 656e  ent_time, curren
-00013ab0: 745f 7370 6565 642c 2063 7572 7265 6e74  t_speed, current
-00013ac0: 5f6d 6f74 696f 6e5f 616e 676c 652c 2063  _motion_angle, c
-00013ad0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00013ae0: 696f 6e2c 2063 7572 7265 6e74 5f64 6973  ion, current_dis
-00013af0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
-00013b00: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
-00013b10: 616e 676c 652c 2063 7572 7265 6e74 5f63  angle, current_c
-00013b20: 656c 6c5f 6178 6973 5f6d 6173 6b0d 0a20  ell_axis_mask.. 
+00011450: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00011460: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011470: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00011480: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00011490: 7365 6c66 2e63 6c75 7374 6572 7363 6f72  self.clusterscor
+000114a0: 655f 6b65 7920 3a20 636c 7573 7465 725f  e_key : cluster_
+000114b0: 7363 6f72 657d 290d 0a20 2020 2020 2020  score})..       
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000114e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000114f0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00011500: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00011510: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+00011520: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00011530: 7273 746b 6579 203a 2065 6363 656e 7472  rstkey : eccentr
+00011540: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+00011550: 797a 5b30 5d7d 290d 0a20 2020 2020 2020  yz[0]})..       
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011580: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00011590: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+000115a0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+000115b0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+000115c0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+000115d0: 636f 6e64 6b65 7920 3a20 6563 6365 6e74  condkey : eccent
+000115e0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+000115f0: 7479 7a5b 315d 7d29 0d0a 2020 2020 2020  tyz[1]})..      
+00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011610: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011620: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00011630: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011640: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00011650: 7570 6461 7465 287b 7365 6c66 2e73 7572  update({self.sur
+00011660: 6661 6365 5f61 7265 615f 6b65 7920 3a20  face_area_key : 
+00011670: 7375 7266 6163 655f 6172 6561 7d29 0d0a  surface_area})..
+00011680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116c0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+000116d0: 7365 6c66 2e72 6f6f 745f 7370 6f74 732e  self.root_spots.
+000116e0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011710: 2e72 6f6f 745f 7370 6f74 735b 6b5d 203d  .root_spots[k] =
+00011720: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00011730: 745f 7072 6f70 6572 7469 6573 5b6b 5d20  t_properties[k] 
+00011740: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00011750: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00011760: 6465 6620 5f63 6f6d 7075 7465 5f70 6865  def _compute_phe
+00011770: 6e6f 7479 7065 7328 7365 6c66 293a 0d0a  notypes(self):..
+00011780: 0d0a 2020 2020 2020 2020 2020 666f 7220  ..          for 
+00011790: 286b 2c76 2920 696e 2073 656c 662e 756e  (k,v) in self.un
+000117a0: 6971 7565 5f74 7261 636b 732e 6974 656d  ique_tracks.item
+000117b0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+000117c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000117d0: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+000117e0: 203d 206b 0d0a 2020 2020 2020 2020 2020   = k..          
+000117f0: 2020 2020 2020 7472 6163 6b6c 6574 5f70        tracklet_p
+00011800: 726f 7065 7274 6965 7320 3d20 7365 6c66  roperties = self
+00011810: 2e75 6e69 7175 655f 7472 6163 6b5f 7072  .unique_track_pr
+00011820: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
+00011830: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00011840: 636b 7320 3d20 7365 6c66 2e75 6e69 7175  cks = self.uniqu
+00011850: 655f 7472 6163 6b73 5b6b 5d0d 0a20 2020  e_tracks[k]..   
+00011860: 2020 2020 2020 2020 2020 2020 205a 203d               Z =
+00011870: 2074 7261 636b 735b 3a2c 325d 0d0a 2020   tracks[:,2]..  
+00011880: 2020 2020 2020 2020 2020 2020 2020 5920                Y 
+00011890: 3d20 7472 6163 6b73 5b3a 2c33 5d0d 0a20  = tracks[:,3].. 
+000118a0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+000118b0: 203d 2074 7261 636b 735b 3a2c 345d 0d0a   = tracks[:,4]..
+000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118d0: 7469 6d65 203d 2074 7261 636b 6c65 745f  time = tracklet_
+000118e0: 7072 6f70 6572 7469 6573 5b3a 2c30 5d0d  properties[:,0].
+000118f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011900: 2075 6e69 7175 655f 6964 7320 3d20 7472   unique_ids = tr
+00011910: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00011920: 735b 3a2c 315d 0d0a 2020 2020 2020 2020  s[:,1]..        
+00011930: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
+00011940: 6473 5f73 6574 203d 2073 6574 2875 6e69  ds_set = set(uni
+00011950: 7175 655f 6964 7329 0d0a 2020 2020 2020  que_ids)..      
+00011960: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
+00011970: 7469 6f6e 5f69 6473 203d 2074 7261 636b  tion_ids = track
+00011980: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00011990: 2c32 5d0d 0a20 2020 2020 2020 2020 2020  ,2]..           
+000119a0: 2020 2020 2072 6164 6975 7320 3d20 7472       radius = tr
+000119b0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000119c0: 735b 3a2c 335d 0d0a 2020 2020 2020 2020  s[:,3]..        
+000119d0: 2020 2020 2020 2020 766f 6c75 6d65 203d          volume =
+000119e0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+000119f0: 7469 6573 5b3a 2c34 5d0d 0a20 2020 2020  ties[:,4]..     
+00011a00: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
+00011a10: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00011a20: 7374 203d 2074 7261 636b 6c65 745f 7072  st = tracklet_pr
+00011a30: 6f70 6572 7469 6573 5b3a 2c35 5d0d 0a20  operties[:,5].. 
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011a50: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00011a60: 5f73 6563 6f6e 6420 3d20 7472 6163 6b6c  _second = trackl
+00011a70: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00011a80: 365d 0d0a 2020 2020 2020 2020 2020 2020  6]..            
+00011a90: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
+00011aa0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00011ab0: 6572 7469 6573 5b3a 2c37 5d0d 0a20 2020  erties[:,7]..   
+00011ac0: 2020 2020 2020 2020 2020 2020 2063 6c75               clu
+00011ad0: 7374 6572 5f63 6c61 7373 203d 2074 7261  ster_class = tra
+00011ae0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00011af0: 5b3a 2c38 5d0d 0a20 2020 2020 2020 2020  [:,8]..         
+00011b00: 2020 2020 2020 2063 6c75 7374 6572 5f63         cluster_c
+00011b10: 6c61 7373 5f73 636f 7265 203d 2074 7261  lass_score = tra
+00011b20: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00011b30: 5b3a 2c39 5d0d 0a20 2020 2020 2020 2020  [:,9]..         
+00011b40: 2020 2020 2020 2069 6e74 656e 7369 7479         intensity
+00011b50: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00011b60: 6572 7469 6573 5b3a 2c31 305d 0d0a 2020  erties[:,10]..  
+00011b70: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00011b80: 6565 6420 3d20 7472 6163 6b6c 6574 5f70  eed = tracklet_p
+00011b90: 726f 7065 7274 6965 735b 3a2c 3131 5d0d  roperties[:,11].
+00011ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011bb0: 206d 6f74 696f 6e5f 616e 676c 6520 3d20   motion_angle = 
+00011bc0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00011bd0: 6965 735b 3a2c 3132 5d0d 0a20 2020 2020  ies[:,12]..     
+00011be0: 2020 2020 2020 2020 2020 2061 6363 656c             accel
+00011bf0: 6572 6174 696f 6e20 3d20 7472 6163 6b6c  eration = trackl
+00011c00: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00011c10: 3133 5d0d 0a20 2020 2020 2020 2020 2020  13]..           
+00011c20: 2020 2020 2064 6973 7461 6e63 655f 6365       distance_ce
+00011c30: 6c6c 5f6d 6173 6b20 3d20 7472 6163 6b6c  ll_mask = trackl
+00011c40: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00011c50: 3134 5d0d 0a20 2020 2020 2020 2020 2020  14]..           
+00011c60: 2020 2020 2072 6164 6961 6c5f 616e 676c       radial_angl
+00011c70: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
+00011c80: 7065 7274 6965 735b 3a2c 3135 5d0d 0a20  perties[:,15].. 
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011ca0: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
+00011cb0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00011cc0: 6965 735b 3a2c 3136 5d0d 0a0d 0a0d 0a20  ies[:,16]...... 
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00011ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011cf0: 2075 6e69 7175 655f 6666 745f 7072 6f70   unique_fft_prop
+00011d00: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
+00011d10: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00011d20: 2020 2020 2020 756e 6971 7565 5f63 6c75        unique_clu
+00011d30: 7374 6572 5f70 726f 7065 7274 6965 735f  ster_properties_
+00011d40: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
+00011d50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011d60: 656c 662e 756e 6971 7565 5f66 6674 5f70  elf.unique_fft_p
+00011d70: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+00011d80: 6964 5d20 3d20 7b7d 0d0a 2020 2020 2020  id] = {}..      
+00011d90: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00011da0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
+00011db0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+00011dc0: 645d 203d 207b 7d0d 0a0d 0a20 2020 2020  d] = {}....     
+00011dd0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00011de0: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
+00011df0: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
+00011e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011e10: 2020 756e 6971 7565 5f64 796e 616d 6963    unique_dynamic
+00011e20: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00011e30: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
+00011e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011e50: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+00011e60: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00011e70: 5d20 3d20 7b7d 0d0a 2020 2020 2020 2020  ] = {}..        
+00011e80: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00011e90: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
+00011ea0: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+00011eb0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00011ec0: 2020 2020 2020 2065 7870 616e 6465 645f         expanded_
+00011ed0: 7469 6d65 203d 206e 702e 7a65 726f 7328  time = np.zeros(
+00011ee0: 7365 6c66 2e74 656e 6420 2d20 7365 6c66  self.tend - self
+00011ef0: 2e74 7374 6172 7420 2b20 3129 0d0a 2020  .tstart + 1)..  
+00011f00: 2020 2020 2020 2020 2020 2020 2020 706f                po
+00011f10: 696e 745f 7361 6d70 6c65 203d 2065 7870  int_sample = exp
+00011f20: 616e 6465 645f 7469 6d65 2e73 6861 7065  anded_time.shape
+00011f30: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+00011f40: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00011f50: 6e67 6528 6c65 6e28 6578 7061 6e64 6564  nge(len(expanded
+00011f60: 5f74 696d 6529 293a 0d0a 2020 2020 2020  _time)):..      
+00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f80: 2065 7870 616e 6465 645f 7469 6d65 5b69   expanded_time[i
+00011f90: 5d20 3d20 6920 0d0a 2020 2020 2020 2020  ] = i ..        
+00011fa0: 2020 2020 2020 2020 666f 7220 6375 7272          for curr
+00011fb0: 656e 745f 756e 6971 7565 5f69 6420 696e  ent_unique_id in
+00011fc0: 2075 6e69 7175 655f 6964 735f 7365 743a   unique_ids_set:
+00011fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011fe0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00011ff0: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
+00012000: 6564 5f69 6e74 656e 7369 7479 203d 206e  ed_intensity = n
+00012010: 702e 7a65 726f 7328 7365 6c66 2e74 656e  p.zeros(self.ten
+00012020: 6420 2d20 7365 6c66 2e74 7374 6172 7420  d - self.tstart 
+00012030: 2b20 3129 0d0a 2020 2020 2020 2020 2020  + 1)..          
+00012040: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00012050: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012070: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
+00012080: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012090: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000120a0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+000120b0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+000120c0: 656e 745f 7920 3d20 5b5d 0d0a 2020 2020  ent_y = []..    
+000120d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000120e0: 7572 7265 6e74 5f78 203d 205b 5d0d 0a20  urrent_x = [].. 
+000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012100: 2020 6375 7272 656e 745f 696e 7465 6e73    current_intens
+00012110: 6974 7920 3d20 5b5d 0d0a 2020 2020 2020  ity = []..      
+00012120: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012130: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+00012140: 7373 203d 205b 5d0d 0a20 2020 2020 2020  ss = []..       
+00012150: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012160: 656e 745f 636c 7573 7465 725f 636c 6173  ent_cluster_clas
+00012170: 735f 7363 6f72 6520 3d20 5b5d 0d0a 2020  s_score = []..  
+00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2063 7572 7265 6e74 5f72 6164 6975 7320   current_radius 
+000121a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000121b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000121c0: 5f76 6f6c 756d 6520 3d20 5b5d 0d0a 2020  _volume = []..  
+000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121e0: 2063 7572 7265 6e74 5f73 7065 6564 203d   current_speed =
+000121f0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00012200: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012210: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 205b  motion_angle = [
+00012220: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012230: 2020 2020 2020 6375 7272 656e 745f 6163        current_ac
+00012240: 6365 6c65 7261 7469 6f6e 203d 205b 5d0d  celeration = [].
+00012250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012260: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
+00012270: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00012280: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00012290: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000122a0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000122b0: 705f 6669 7273 7420 3d20 5b5d 0d0a 2020  p_first = []..  
+000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122d0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+000122e0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+000122f0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+00012300: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012310: 6e74 5f73 7572 6661 6365 5f61 7265 6120  nt_surface_area 
+00012320: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00012330: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012340: 6e74 5f72 6164 6961 6c5f 616e 676c 6520  nt_radial_angle 
+00012350: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012360: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012370: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b20  _cell_axis_mask 
+00012380: 3d20 5b5d 200d 0a20 2020 2020 2020 2020  = [] ..         
+00012390: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000123b0: 6f72 206a 2069 6e20 7261 6e67 6528 7469  or j in range(ti
+000123c0: 6d65 2e73 6861 7065 5b30 5d29 3a0d 0a20  me.shape[0]):.. 
+000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123e0: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
+000123f0: 656e 745f 756e 6971 7565 5f69 6420 3d3d  ent_unique_id ==
+00012400: 2075 6e69 7175 655f 6964 735b 6a5d 3a0d   unique_ids[j]:.
+00012410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012430: 2020 6375 7272 656e 745f 7469 6d65 2e61    current_time.a
+00012440: 7070 656e 6428 7469 6d65 5b6a 5d29 0d0a  ppend(time[j])..
+00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012470: 2063 7572 7265 6e74 5f7a 2e61 7070 656e   current_z.appen
+00012480: 6428 5a5b 6a5d 290d 0a20 2020 2020 2020  d(Z[j])..       
+00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000124b0: 745f 792e 6170 7065 6e64 2859 5b6a 5d29  t_y.append(Y[j])
+000124c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124e0: 2020 2063 7572 7265 6e74 5f78 2e61 7070     current_x.app
+000124f0: 656e 6428 585b 6a5d 290d 0a20 2020 2020  end(X[j])..     
+00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012510: 2020 2020 2020 2020 2020 2020 6578 7061              expa
+00012520: 6e64 6564 5f69 6e74 656e 7369 7479 5b69  nded_intensity[i
+00012530: 6e74 2874 696d 655b 6a5d 295d 203d 2069  nt(time[j])] = i
+00012540: 6e74 656e 7369 7479 5b6a 5d0d 0a20 2020  ntensity[j]..   
+00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012560: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012570: 7272 656e 745f 696e 7465 6e73 6974 792e  rrent_intensity.
+00012580: 6170 7065 6e64 2869 6e74 656e 7369 7479  append(intensity
+00012590: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125b0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+000125c0: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
+000125d0: 656e 6428 636c 7573 7465 725f 636c 6173  end(cluster_clas
+000125e0: 735b 6a5d 290d 0a20 2020 2020 2020 2020  s[j])..         
+000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012600: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012610: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
+00012620: 6f72 652e 6170 7065 6e64 2863 6c75 7374  ore.append(clust
+00012630: 6572 5f63 6c61 7373 5f73 636f 7265 5b6a  er_class_score[j
+00012640: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012660: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
+00012670: 6975 732e 6170 7065 6e64 2872 6164 6975  ius.append(radiu
+00012680: 735b 6a5d 290d 0a20 2020 2020 2020 2020  s[j])..         
+00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000126b0: 766f 6c75 6d65 2e61 7070 656e 6428 766f  volume.append(vo
+000126c0: 6c75 6d65 5b6a 5d29 0d0a 2020 2020 2020  lume[j])..      
+000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+000126f0: 6e74 5f73 7065 6564 2e61 7070 656e 6428  nt_speed.append(
+00012700: 7370 6565 645b 6a5d 290d 0a20 2020 2020  speed[j])..     
+00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012720: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012730: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
+00012740: 2e61 7070 656e 6428 6d6f 7469 6f6e 5f61  .append(motion_a
+00012750: 6e67 6c65 5b6a 5d29 0d0a 2020 2020 2020  ngle[j])..      
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012780: 6e74 5f61 6363 656c 6572 6174 696f 6e2e  nt_acceleration.
+00012790: 6170 7065 6e64 2861 6363 656c 6572 6174  append(accelerat
+000127a0: 696f 6e5b 6a5d 290d 0a20 2020 2020 2020  ion[j])..       
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127c0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000127d0: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
+000127e0: 6d61 736b 2e61 7070 656e 6428 6469 7374  mask.append(dist
+000127f0: 616e 6365 5f63 656c 6c5f 6d61 736b 5b6a  ance_cell_mask[j
+00012800: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012820: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
+00012830: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00012840: 6972 7374 2e61 7070 656e 6428 6563 6365  irst.append(ecce
+00012850: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00012860: 7273 745b 6a5d 290d 0a20 2020 2020 2020  rst[j])..       
+00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012880: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012890: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+000128a0: 6f6d 705f 7365 636f 6e64 2e61 7070 656e  omp_second.appen
+000128b0: 6428 6563 6365 6e74 7269 6369 7479 5f63  d(eccentricity_c
+000128c0: 6f6d 705f 7365 636f 6e64 5b6a 5d29 0d0a  omp_second[j])..
+000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128f0: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
+00012900: 5f61 7265 612e 6170 7065 6e64 2873 7572  _area.append(sur
+00012910: 6661 6365 5f61 7265 615b 6a5d 290d 0a20  face_area[j]).. 
+00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012940: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
+00012950: 6e67 6c65 2e61 7070 656e 6428 7261 6469  ngle.append(radi
+00012960: 616c 5f61 6e67 6c65 5b6a 5d29 0d0a 2020  al_angle[j])..  
+00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012980: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012990: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
+000129a0: 5f6d 6173 6b2e 6170 7065 6e64 2863 656c  _mask.append(cel
+000129b0: 6c5f 6178 6973 5f6d 6173 6b5b 6a5d 290d  l_axis_mask[j]).
+000129c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000129d0: 2020 2020 6375 7272 656e 745f 7469 6d65      current_time
+000129e0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+000129f0: 7272 656e 745f 7469 6d65 290d 0a20 2020  rrent_time)..   
+00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a10: 6375 7272 656e 745f 696e 7465 6e73 6974  current_intensit
+00012a20: 7920 3d20 6e70 2e61 7361 7272 6179 2863  y = np.asarray(c
+00012a30: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
+00012a40: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+00012a50: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012a60: 745f 636c 7573 7465 725f 636c 6173 7320  t_cluster_class 
+00012a70: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00012a80: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+00012a90: 7373 290d 0a20 2020 2020 2020 2020 2020  ss)..           
+00012aa0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00012ab0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
+00012ac0: 6f72 6520 3d20 6e70 2e61 7361 7272 6179  ore = np.asarray
+00012ad0: 2863 7572 7265 6e74 5f63 6c75 7374 6572  (current_cluster
+00012ae0: 5f63 6c61 7373 5f73 636f 7265 2920 2020  _class_score)   
+00012af0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00012b00: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00012b10: 6164 6975 7320 3d20 6e70 2e61 7361 7272  adius = np.asarr
+00012b20: 6179 2863 7572 7265 6e74 5f72 6164 6975  ay(current_radiu
+00012b30: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+00012b40: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
+00012b50: 6f6c 756d 6520 3d20 6e70 2e61 7361 7272  olume = np.asarr
+00012b60: 6179 2863 7572 7265 6e74 5f76 6f6c 756d  ay(current_volum
+00012b70: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00012b80: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
+00012b90: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00012ba0: 5f66 6972 7374 203d 206e 702e 6173 6172  _first = np.asar
+00012bb0: 7261 7928 6375 7272 656e 745f 6563 6365  ray(current_ecce
+00012bc0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00012bd0: 7273 7429 0d0a 2020 2020 2020 2020 2020  rst)..          
+00012be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012bf0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00012c00: 6d70 5f73 6563 6f6e 6420 3d20 6e70 2e61  mp_second = np.a
+00012c10: 7361 7272 6179 2863 7572 7265 6e74 5f65  sarray(current_e
+00012c20: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00012c30: 5f73 6563 6f6e 6429 0d0a 2020 2020 2020  _second)..      
+00012c40: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00012c50: 7265 6e74 5f73 7572 6661 6365 5f61 7265  rent_surface_are
+00012c60: 6120 3d20 6e70 2e61 7361 7272 6179 2863  a = np.asarray(c
+00012c70: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
+00012c80: 7265 6129 0d0a 0d0a 2020 2020 2020 2020  rea)....        
+00012c90: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012ca0: 6e74 5f73 7065 6564 203d 206e 702e 6173  nt_speed = np.as
+00012cb0: 6172 7261 7928 6375 7272 656e 745f 7370  array(current_sp
+00012cc0: 6565 6429 0d0a 2020 2020 2020 2020 2020  eed)..          
+00012cd0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012ce0: 5f6d 6f74 696f 6e5f 616e 676c 6520 3d20  _motion_angle = 
+00012cf0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00012d00: 6e74 5f6d 6f74 696f 6e5f 616e 676c 6529  nt_motion_angle)
+00012d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012d20: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
+00012d30: 656c 6572 6174 696f 6e20 3d20 6e70 2e61  eleration = np.a
+00012d40: 7361 7272 6179 2863 7572 7265 6e74 5f61  sarray(current_a
+00012d50: 6363 656c 6572 6174 696f 6e29 0d0a 2020  cceleration)..  
+00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d70: 2063 7572 7265 6e74 5f64 6973 7461 6e63   current_distanc
+00012d80: 655f 6365 6c6c 5f6d 6173 6b20 3d20 6e70  e_cell_mask = np
+00012d90: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00012da0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00012db0: 6173 6b29 0d0a 2020 2020 2020 2020 2020  ask)..          
+00012dc0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012dd0: 5f72 6164 6961 6c5f 616e 676c 6520 3d20  _radial_angle = 
+00012de0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00012df0: 6e74 5f72 6164 6961 6c5f 616e 676c 6529  nt_radial_angle)
+00012e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012e10: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+00012e20: 6c5f 6178 6973 5f6d 6173 6b20 3d20 6e70  l_axis_mask = np
+00012e30: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00012e40: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b29  _cell_axis_mask)
+00012e50: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00012e60: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00012e70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 2020 2069 6620 706f 696e 745f 7361 6d70     if point_samp
+00012ea0: 6c65 203e 2030 3a0d 0a20 2020 2020 2020  le > 0:..       
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 2020 2078 665f 7361 6d70           xf_samp
+00012ed0: 6c65 203d 2066 6674 6672 6571 2870 6f69  le = fftfreq(poi
+00012ee0: 6e74 5f73 616d 706c 652c 2073 656c 662e  nt_sample, self.
+00012ef0: 7463 616c 6962 7261 7469 6f6e 290d 0a20  tcalibration).. 
+00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f10: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00012f20: 6674 7374 7269 705f 7361 6d70 6c65 203d  ftstrip_sample =
+00012f30: 2066 6674 2865 7870 616e 6465 645f 696e   fft(expanded_in
+00012f40: 7465 6e73 6974 7929 0d0a 2020 2020 2020  tensity)..      
+00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f60: 2020 2020 2020 2020 2020 6666 7474 6f74            ffttot
+00012f70: 616c 5f73 616d 706c 6520 3d20 6e70 2e61  al_sample = np.a
+00012f80: 6273 2866 6674 7374 7269 705f 7361 6d70  bs(fftstrip_samp
+00012f90: 6c65 290d 0a20 2020 2020 2020 2020 2020  le)..           
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2078 665f 7361 6d70 6c65 203d       xf_sample =
+00012fc0: 2078 665f 7361 6d70 6c65 5b30 203a 206c   xf_sample[0 : l
+00012fd0: 656e 2878 665f 7361 6d70 6c65 2920 2f2f  en(xf_sample) //
+00012fe0: 2032 5d0d 0a20 2020 2020 2020 2020 2020   2]..           
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013000: 2020 2020 2066 6674 746f 7461 6c5f 7361       ffttotal_sa
+00013010: 6d70 6c65 203d 2066 6674 746f 7461 6c5f  mple = ffttotal_
+00013020: 7361 6d70 6c65 5b30 203a 206c 656e 2866  sample[0 : len(f
+00013030: 6674 746f 7461 6c5f 7361 6d70 6c65 2920  fttotal_sample) 
+00013040: 2f2f 2032 5d0d 0a0d 0a20 2020 2020 2020  // 2]....       
+00013050: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00013060: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00013070: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+00013080: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
+00013090: 6578 7061 6e64 6564 5f74 696d 652c 2065  expanded_time, e
+000130a0: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
+000130b0: 792c 2078 665f 7361 6d70 6c65 2c20 6666  y, xf_sample, ff
+000130c0: 7474 6f74 616c 5f73 616d 706c 650d 0a20  ttotal_sample.. 
+000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130e0: 2020 756e 6971 7565 5f63 6c75 7374 6572    unique_cluster
+000130f0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013100: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00013110: 7175 655f 6964 5d20 3d20 2063 7572 7265  que_id] =  curre
+00013120: 6e74 5f74 696d 652c 2063 7572 7265 6e74  nt_time, current
+00013130: 5f63 6c75 7374 6572 5f63 6c61 7373 2c20  _cluster_class, 
+00013140: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
+00013150: 636c 6173 735f 7363 6f72 650d 0a20 2020  class_score..   
+00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013170: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+00013180: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00013190: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+000131a0: 6964 5d20 3d20 6375 7272 656e 745f 7469  id] = current_ti
+000131b0: 6d65 2c20 6375 7272 656e 745f 7a2c 2063  me, current_z, c
+000131c0: 7572 7265 6e74 5f79 2c20 6375 7272 656e  urrent_y, curren
+000131d0: 745f 782c 2063 7572 7265 6e74 5f72 6164  t_x, current_rad
+000131e0: 6975 732c 2063 7572 7265 6e74 5f76 6f6c  ius, current_vol
+000131f0: 756d 652c 2063 7572 7265 6e74 5f65 6363  ume, current_ecc
+00013200: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00013210: 6972 7374 2c20 6375 7272 656e 745f 6563  irst, current_ec
+00013220: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013230: 7365 636f 6e64 2c20 6375 7272 656e 745f  second, current_
+00013240: 7375 7266 6163 655f 6172 6561 2c20 6375  surface_area, cu
+00013250: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
+00013260: 6173 732c 2063 7572 7265 6e74 5f63 6c75  ass, current_clu
+00013270: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
+00013280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013290: 2020 2020 2075 6e69 7175 655f 6479 6e61       unique_dyna
+000132a0: 6d69 635f 7072 6f70 6572 7469 6573 5f74  mic_properties_t
+000132b0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
+000132c0: 756e 6971 7565 5f69 645d 203d 2063 7572  unique_id] = cur
+000132d0: 7265 6e74 5f74 696d 652c 2063 7572 7265  rent_time, curre
+000132e0: 6e74 5f73 7065 6564 2c20 6375 7272 656e  nt_speed, curren
+000132f0: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  t_motion_angle, 
+00013300: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
+00013310: 7469 6f6e 2c20 6375 7272 656e 745f 6469  tion, current_di
+00013320: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00013330: 2c20 6375 7272 656e 745f 7261 6469 616c  , current_radial
+00013340: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
+00013350: 6365 6c6c 5f61 7869 735f 6d61 736b 0d0a  cell_axis_mask..
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 2020 2073 656c 662e 756e 6971 7565 5f66     self.unique_f
+00013380: 6674 5f70 726f 7065 7274 6965 735b 7472  ft_properties[tr
+00013390: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
+000133a0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+000133b0: 643a 756e 6971 7565 5f66 6674 5f70 726f  d:unique_fft_pro
+000133c0: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+000133d0: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+000133e0: 6964 5d7d 290d 0a20 2020 2020 2020 2020  id]})..         
+000133f0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00013400: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
+00013410: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+00013420: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
+00013430: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
+00013440: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
+00013450: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00013460: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013470: 645d 7d29 0d0a 0d0a 2020 2020 2020 2020  d]})....        
+00013480: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013490: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+000134a0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+000134b0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
+000134c0: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
+000134d0: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
+000134e0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+000134f0: 7265 6e74 5f75 6e69 7175 655f 6964 5d7d  rent_unique_id]}
+00013500: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013510: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00013520: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
+00013530: 7469 6573 5b74 7261 636b 5f69 645d 2e75  ties[track_id].u
+00013540: 7064 6174 6528 7b63 7572 7265 6e74 5f75  pdate({current_u
+00013550: 6e69 7175 655f 6964 3a75 6e69 7175 655f  nique_id:unique_
+00013560: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
+00013570: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
+00013580: 656e 745f 756e 6971 7565 5f69 645d 7d29  ent_unique_id]})
+00013590: 0d0a 0d0a 2020 2020 6465 6620 5f73 6563  ....    def _sec
+000135a0: 6f6e 645f 6368 616e 6e65 6c5f 7370 6f74  ond_channel_spot
+000135b0: 7328 7365 6c66 2c20 6672 616d 652c 207a  s(self, frame, z
+000135c0: 2c20 792c 2078 2c20 6365 6c6c 5f69 642c  , y, x, cell_id,
+000135d0: 2074 7261 636b 5f69 6429 3a0d 0a20 2020   track_id):..   
+000135e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000135f0: 2020 2020 2020 7472 6565 2c20 6365 6e74        tree, cent
+00013600: 726f 6964 732c 206c 6162 656c 732c 2076  roids, labels, v
+00013610: 6f6c 756d 652c 2069 6e74 656e 7369 7479  olume, intensity
+00013620: 5f6d 6561 6e2c 2069 6e74 656e 7369 7479  _mean, intensity
+00013630: 5f74 6f74 616c 2c20 626f 756e 6469 6e67  _total, bounding
+00013640: 5f62 6f78 6573 203d 2073 656c 662e 5f74  _boxes = self._t
+00013650: 696d 6564 5f63 6861 6e6e 656c 5f73 6567  imed_channel_seg
+00013660: 5f69 6d61 6765 5b73 7472 2869 6e74 2866  _image[str(int(f
+00013670: 6c6f 6174 2866 7261 6d65 2929 295d 0d0a  loat(frame)))]..
+00013680: 2020 2020 2020 2020 2020 2020 7069 7865              pixe
+00013690: 6c74 6573 746c 6f63 6174 696f 6e20 3d20  ltestlocation = 
+000136a0: 287a 2c79 2c78 290d 0a20 2020 2020 2020  (z,y,x)..       
+000136b0: 2020 2020 2064 6973 742c 2069 6e64 6578       dist, index
+000136c0: 203d 2074 7265 652e 7175 6572 7928 7069   = tree.query(pi
+000136d0: 7865 6c74 6573 746c 6f63 6174 696f 6e29  xeltestlocation)
+000136e0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+000136f0: 2020 6262 6f78 203d 2062 6f75 6e64 696e    bbox = boundin
+00013700: 675f 626f 7865 735b 696e 6465 785d 0d0a  g_boxes[index]..
+00013710: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00013720: 7a20 3d20 6162 7328 6262 6f78 5b30 5d20  z = abs(bbox[0] 
+00013730: 2d20 6262 6f78 5b33 5d29 0d0a 2020 2020  - bbox[3])..    
+00013740: 2020 2020 2020 2020 7369 7a65 7920 3d20          sizey = 
+00013750: 6162 7328 6262 6f78 5b31 5d20 2d20 6262  abs(bbox[1] - bb
+00013760: 6f78 5b34 5d29 0d0a 2020 2020 2020 2020  ox[4])..        
+00013770: 2020 2020 7369 7a65 7820 3d20 6162 7328      sizex = abs(
+00013780: 6262 6f78 5b32 5d20 2d20 6262 6f78 5b35  bbox[2] - bbox[5
+00013790: 5d29 200d 0a20 2020 2020 2020 2020 2020  ]) ..           
+000137a0: 2076 6574 6f5f 766f 6c75 6d65 203d 2073   veto_volume = s
+000137b0: 697a 6578 202a 2073 697a 6579 202a 2073  izex * sizey * s
+000137c0: 697a 657a 0d0a 2020 2020 2020 2020 2020  izez..          
+000137d0: 2020 7665 746f 5f72 6164 6975 7320 3d20    veto_radius = 
+000137e0: 6d61 7468 2e70 6f77 2833 202a 2076 6574  math.pow(3 * vet
+000137f0: 6f5f 766f 6c75 6d65 202f 2028 3420 2a20  o_volume / (4 * 
+00013800: 6d61 7468 2e70 6929 2c20 312e 3020 2f20  math.pi), 1.0 / 
+00013810: 332e 3029 0d0a 0d0a 2020 2020 2020 2020  3.0)....        
+00013820: 2020 2020 6c6f 6361 7469 6f6e 203d 2028      location = (
+00013830: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00013840: 5b30 5d20 2a20 7365 6c66 2e7a 6361 6c69  [0] * self.zcali
+00013850: 6272 6174 696f 6e2c 2063 656e 7472 6f69  bration, centroi
+00013860: 6473 5b69 6e64 6578 5d5b 315d 2a73 656c  ds[index][1]*sel
+00013870: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
+00013880: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00013890: 5b32 5d2a 7365 6c66 2e78 6361 6c69 6272  [2]*self.xcalibr
+000138a0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+000138b0: 2020 2020 5155 414c 4954 5920 3d20 766f      QUALITY = vo
+000138c0: 6c75 6d65 5b69 6e64 6578 5d0d 0a20 2020  lume[index]..   
+000138d0: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
+000138e0: 3d20 6d61 7468 2e70 6f77 2851 5541 4c49  = math.pow(QUALI
+000138f0: 5459 2c20 312e 302f 332e 3029 202a 2073  TY, 1.0/3.0) * s
+00013900: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00013910: 202a 2073 656c 662e 7963 616c 6962 7261   * self.ycalibra
+00013920: 7469 6f6e 202a 2073 656c 662e 7a63 616c  tion * self.zcal
+00013930: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+00013940: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+00013950: 656c 6c5f 6d61 736b 2c20 6d61 736b 6365  ell_mask, maskce
+00013960: 6e74 726f 6964 203d 2073 656c 662e 5f67  ntroid = self._g
+00013970: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
+00013980: 2866 7261 6d65 2c20 6c6f 6361 7469 6f6e  (frame, location
+00013990: 2c20 5241 4449 5553 290d 0a20 2020 2020  , RADIUS)..     
+000139a0: 2020 2020 2020 2069 6620 6469 7374 203c         if dist <
+000139b0: 3d20 3220 2a20 7665 746f 5f72 6164 6975  = 2 * veto_radiu
+000139c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000139d0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+000139e0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+000139f0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00013a00: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00013a10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013a20: 6c66 2e63 656c 6c69 645f 6b65 793a 2069  lf.cellid_key: i
+00013a30: 6e74 2863 656c 6c5f 6964 292c 200d 0a20  nt(cell_id), .. 
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a50: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+00013a60: 6569 645f 6b65 7920 3a20 696e 7428 6672  eid_key : int(fr
+00013a70: 616d 6529 2c0d 0a20 2020 2020 2020 2020  ame),..         
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013a90: 656c 662e 7a70 6f73 6964 5f6b 6579 203a  elf.zposid_key :
+00013aa0: 2066 6c6f 6174 2863 656e 7472 6f69 6473   float(centroids
+00013ab0: 5b69 6e64 6578 5d5b 305d 2a20 7365 6c66  [index][0]* self
+00013ac0: 2e7a 6361 6c69 6272 6174 696f 6e29 2c0d  .zcalibration),.
+00013ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ae0: 2020 2020 2020 2020 2073 656c 662e 7970           self.yp
+00013af0: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
+00013b00: 2863 656e 7472 6f69 6473 5b69 6e64 6578  (centroids[index
+00013b10: 5d5b 315d 2a20 7365 6c66 2e79 6361 6c69  ][1]* self.ycali
+00013b20: 6272 6174 696f 6e29 2c0d 0a20 2020 2020  bration),..     
 00013b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b40: 2020 7365 6c66 2e75 6e69 7175 655f 6666    self.unique_ff
-00013b50: 745f 7072 6f70 6572 7469 6573 5b74 7261  t_properties[tra
-00013b60: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00013b70: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013b80: 3a75 6e69 7175 655f 6666 745f 7072 6f70  :unique_fft_prop
-00013b90: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-00013ba0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00013bb0: 645d 7d29 0d0a 2020 2020 2020 2020 2020  d]})..          
-00013bc0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00013bd0: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
-00013be0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00013bf0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
-00013c00: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
-00013c10: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00013c20: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00013c30: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00013c40: 5d7d 290d 0a0d 0a20 2020 2020 2020 2020  ]})....         
-00013c50: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00013c60: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00013c70: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00013c80: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
-00013c90: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
-00013ca0: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
-00013cb0: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-00013cc0: 656e 745f 756e 6971 7565 5f69 645d 7d29  ent_unique_id]})
-00013cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013ce0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00013cf0: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
-00013d00: 6965 735b 7472 6163 6b5f 6964 5d2e 7570  ies[track_id].up
-00013d10: 6461 7465 287b 6375 7272 656e 745f 756e  date({current_un
-00013d20: 6971 7565 5f69 643a 756e 6971 7565 5f64  ique_id:unique_d
-00013d30: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
-00013d40: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-00013d50: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
-00013d60: 0a0d 0a20 2020 2064 6566 205f 7365 636f  ...    def _seco
-00013d70: 6e64 5f63 6861 6e6e 656c 5f73 706f 7473  nd_channel_spots
-00013d80: 2873 656c 662c 2066 7261 6d65 2c20 7a2c  (self, frame, z,
-00013d90: 2079 2c20 782c 2063 656c 6c5f 6964 2c20   y, x, cell_id, 
-00013da0: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
-00013db0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00013dc0: 2020 2020 2074 7265 652c 2063 656e 7472       tree, centr
-00013dd0: 6f69 6473 2c20 6c61 6265 6c73 2c20 766f  oids, labels, vo
-00013de0: 6c75 6d65 2c20 696e 7465 6e73 6974 795f  lume, intensity_
-00013df0: 6d65 616e 2c20 696e 7465 6e73 6974 795f  mean, intensity_
-00013e00: 746f 7461 6c2c 2062 6f75 6e64 696e 675f  total, bounding_
-00013e10: 626f 7865 7320 3d20 7365 6c66 2e5f 7469  boxes = self._ti
-00013e20: 6d65 645f 6368 616e 6e65 6c5f 7365 675f  med_channel_seg_
-00013e30: 696d 6167 655b 7374 7228 696e 7428 666c  image[str(int(fl
-00013e40: 6f61 7428 6672 616d 6529 2929 5d0d 0a20  oat(frame)))].. 
-00013e50: 2020 2020 2020 2020 2020 2070 6978 656c             pixel
-00013e60: 7465 7374 6c6f 6361 7469 6f6e 203d 2028  testlocation = (
-00013e70: 7a2c 792c 7829 0d0a 2020 2020 2020 2020  z,y,x)..        
-00013e80: 2020 2020 6469 7374 2c20 696e 6465 7820      dist, index 
-00013e90: 3d20 7472 6565 2e71 7565 7279 2870 6978  = tree.query(pix
-00013ea0: 656c 7465 7374 6c6f 6361 7469 6f6e 290d  eltestlocation).
-00013eb0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00013ec0: 2062 626f 7820 3d20 626f 756e 6469 6e67   bbox = bounding
-00013ed0: 5f62 6f78 6573 5b69 6e64 6578 5d0d 0a20  _boxes[index].. 
-00013ee0: 2020 2020 2020 2020 2020 2073 697a 657a             sizez
-00013ef0: 203d 2061 6273 2862 626f 785b 305d 202d   = abs(bbox[0] -
-00013f00: 2062 626f 785b 335d 290d 0a20 2020 2020   bbox[3])..     
-00013f10: 2020 2020 2020 2073 697a 6579 203d 2061         sizey = a
-00013f20: 6273 2862 626f 785b 315d 202d 2062 626f  bs(bbox[1] - bbo
-00013f30: 785b 345d 290d 0a20 2020 2020 2020 2020  x[4])..         
-00013f40: 2020 2073 697a 6578 203d 2061 6273 2862     sizex = abs(b
-00013f50: 626f 785b 325d 202d 2062 626f 785b 355d  box[2] - bbox[5]
-00013f60: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00013f70: 7665 746f 5f76 6f6c 756d 6520 3d20 7369  veto_volume = si
-00013f80: 7a65 7820 2a20 7369 7a65 7920 2a20 7369  zex * sizey * si
-00013f90: 7a65 7a0d 0a20 2020 2020 2020 2020 2020  zez..           
-00013fa0: 2076 6574 6f5f 7261 6469 7573 203d 206d   veto_radius = m
-00013fb0: 6174 682e 706f 7728 3320 2a20 7665 746f  ath.pow(3 * veto
-00013fc0: 5f76 6f6c 756d 6520 2f20 2834 202a 206d  _volume / (4 * m
-00013fd0: 6174 682e 7069 292c 2031 2e30 202f 2033  ath.pi), 1.0 / 3
-00013fe0: 2e30 290d 0a0d 0a20 2020 2020 2020 2020  .0)....         
-00013ff0: 2020 206c 6f63 6174 696f 6e20 3d20 2863     location = (c
-00014000: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00014010: 305d 202a 2073 656c 662e 7a63 616c 6962  0] * self.zcalib
-00014020: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
-00014030: 735b 696e 6465 785d 5b31 5d2a 7365 6c66  s[index][1]*self
-00014040: 2e79 6361 6c69 6272 6174 696f 6e2c 2063  .ycalibration, c
-00014050: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00014060: 325d 2a73 656c 662e 7863 616c 6962 7261  2]*self.xcalibra
-00014070: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00014080: 2020 2051 5541 4c49 5459 203d 2076 6f6c     QUALITY = vol
-00014090: 756d 655b 696e 6465 785d 0d0a 2020 2020  ume[index]..    
-000140a0: 2020 2020 2020 2020 5241 4449 5553 203d          RADIUS =
-000140b0: 206d 6174 682e 706f 7728 5155 414c 4954   math.pow(QUALIT
-000140c0: 592c 2031 2e30 2f33 2e30 2920 2a20 7365  Y, 1.0/3.0) * se
-000140d0: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
-000140e0: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-000140f0: 696f 6e20 2a20 7365 6c66 2e7a 6361 6c69  ion * self.zcali
-00014100: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00014110: 2020 2020 2064 6973 7461 6e63 655f 6365       distance_ce
-00014120: 6c6c 5f6d 6173 6b2c 206d 6173 6b63 656e  ll_mask, maskcen
-00014130: 7472 6f69 6420 3d20 7365 6c66 2e5f 6765  troid = self._ge
-00014140: 745f 626f 756e 6461 7279 5f64 6973 7428  t_boundary_dist(
-00014150: 6672 616d 652c 206c 6f63 6174 696f 6e2c  frame, location,
-00014160: 2052 4144 4955 5329 0d0a 2020 2020 2020   RADIUS)..      
-00014170: 2020 2020 2020 6966 2064 6973 7420 3c3d        if dist <=
-00014180: 2032 202a 2076 6574 6f5f 7261 6469 7573   2 * veto_radius
-00014190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000141a0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-000141b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000141c0: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
-000141d0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-000141e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000141f0: 662e 6365 6c6c 6964 5f6b 6579 3a20 696e  f.cellid_key: in
-00014200: 7428 6365 6c6c 5f69 6429 2c20 0d0a 2020  t(cell_id), ..  
-00014210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014220: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
-00014230: 6964 5f6b 6579 203a 2069 6e74 2866 7261  id_key : int(fra
-00014240: 6d65 292c 0d0a 2020 2020 2020 2020 2020  me),..          
-00014250: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014260: 6c66 2e7a 706f 7369 645f 6b65 7920 3a20  lf.zposid_key : 
-00014270: 666c 6f61 7428 6365 6e74 726f 6964 735b  float(centroids[
-00014280: 696e 6465 785d 5b30 5d2a 2073 656c 662e  index][0]* self.
-00014290: 7a63 616c 6962 7261 7469 6f6e 292c 0d0a  zcalibration),..
-000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142b0: 2020 2020 2020 2020 7365 6c66 2e79 706f          self.ypo
-000142c0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-000142d0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-000142e0: 5b31 5d2a 2073 656c 662e 7963 616c 6962  [1]* self.ycalib
-000142f0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
-00014300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014310: 2020 7365 6c66 2e78 706f 7369 645f 6b65    self.xposid_ke
-00014320: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
-00014330: 6964 735b 696e 6465 785d 5b32 5d2a 2073  ids[index][2]* s
-00014340: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-00014350: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00014360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014370: 2e74 7261 636b 6964 5f6b 6579 3a20 696e  .trackid_key: in
-00014380: 7428 7472 6163 6b5f 6964 292c 0d0a 2020  t(track_id),..  
-00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143a0: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-000143b0: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
-000143c0: 2028 666c 6f61 7428 696e 7465 6e73 6974   (float(intensit
-000143d0: 795f 746f 7461 6c5b 696e 6465 785d 2929  y_total[index]))
-000143e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000143f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014400: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
-00014410: 6579 203a 2028 666c 6f61 7428 696e 7465  ey : (float(inte
-00014420: 6e73 6974 795f 6d65 616e 5b69 6e64 6578  nsity_mean[index
-00014430: 5d29 292c 0d0a 0d0a 2020 2020 2020 2020  ])),....        
-00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
-00014460: 3a20 2866 6c6f 6174 2852 4144 4955 5329  : (float(RADIUS)
-00014470: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00014480: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014490: 2e71 7561 6c69 7479 5f6b 6579 203a 2028  .quality_key : (
-000144a0: 666c 6f61 7428 5155 414c 4954 5929 292c  float(QUALITY)),
-000144b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000144c0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000144d0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000144e0: 6b5f 6b65 793a 2066 6c6f 6174 2864 6973  k_key: float(dis
-000144f0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
-00014500: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014520: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
-00014530: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
-00014540: 6e74 726f 6964 5b30 5d29 2c0d 0a20 2020  ntroid[0]),..   
-00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014560: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
-00014570: 6e74 726f 6964 5f79 5f6b 6579 3a20 666c  ntroid_y_key: fl
-00014580: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
-00014590: 5b31 5d29 2c0d 0a20 2020 2020 2020 2020  [1]),..         
-000145a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000145b0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-000145c0: 5f78 5f6b 6579 3a20 666c 6f61 7428 6d61  _x_key: float(ma
-000145d0: 736b 6365 6e74 726f 6964 5b32 5d29 200d  skcentroid[2]) .
-000145e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000145f0: 2020 207d 200d 0a20 2020 2020 2020 2020     } ..         
-00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014610: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00014620: 6620 5f64 6963 745f 7570 6461 7465 2873  f _dict_update(s
-00014630: 656c 662c 2075 6e69 7175 655f 7472 6163  elf, unique_trac
-00014640: 6b6c 6574 5f69 6473 3a20 4c69 7374 2c20  klet_ids: List, 
-00014650: 2063 656c 6c5f 6964 3a20 696e 742c 2074   cell_id: int, t
-00014660: 7261 636b 5f69 643a 2069 6e74 2c20 736f  rack_id: int, so
-00014670: 7572 6365 5f69 643a 2069 6e74 2c20 7461  urce_id: int, ta
-00014680: 7267 6574 5f69 643a 2069 6e74 293a 0d0a  rget_id: int):..
-00014690: 0d0a 200d 0a20 2020 2020 2020 2067 656e  .. ..        gen
-000146a0: 6572 6174 696f 6e5f 6964 203d 2073 656c  eration_id = sel
-000146b0: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
-000146c0: 745b 6365 6c6c 5f69 645d 0d0a 2020 2020  t[cell_id]..    
-000146d0: 2020 2020 7472 6163 6b6c 6574 5f69 6420      tracklet_id 
-000146e0: 3d20 7365 6c66 2e74 7261 636b 6c65 745f  = self.tracklet_
-000146f0: 6469 6374 5b63 656c 6c5f 6964 5d0d 0a0d  dict[cell_id]...
-00014700: 0a20 2020 2020 2020 2075 6e69 7175 655f  .        unique_
-00014710: 6964 203d 2073 7472 2874 7261 636b 5f69  id = str(track_i
-00014720: 6429 202b 2073 7472 2873 656c 662e 6d61  d) + str(self.ma
-00014730: 785f 7472 6163 6b5f 6964 2920 2b20 7374  x_track_id) + st
-00014740: 7228 6765 6e65 7261 7469 6f6e 5f69 6429  r(generation_id)
-00014750: 202b 2073 7472 2874 7261 636b 6c65 745f   + str(tracklet_
-00014760: 6964 290d 0a20 2020 2020 2020 200d 0a20  id)..        .. 
-00014770: 2020 2020 2020 2076 6563 5f6d 6173 6b20         vec_mask 
-00014780: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
-00014790: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000147a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000147b0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-000147c0: 726f 6964 5f78 5f6b 6579 5d29 2c20 666c  roid_x_key]), fl
-000147d0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000147e0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000147f0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00014800: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-00014810: 795f 6b65 795d 292c 2066 6c6f 6174 2873  y_key]), float(s
-00014820: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014830: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014840: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00014850: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
-00014860: 5d29 205d 0d0a 0d0a 2020 2020 2020 2020  ]) ]....        
-00014870: 7665 635f 6365 6c6c 203d 205b 666c 6f61  vec_cell = [floa
-00014880: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00014890: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000148a0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-000148b0: 2e78 706f 7369 645f 6b65 795d 2920 2c20  .xposid_key]) , 
-000148c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000148d0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-000148e0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000148f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014900: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00014910: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
-00014920: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00014930: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00014940: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00014950: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014960: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00014970: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00014980: 5d0d 0a0d 0a20 2020 2020 2020 2061 6e67  ]....        ang
-00014990: 6c65 203d 2061 6e67 756c 6172 5f63 6861  le = angular_cha
-000149a0: 6e67 6528 7665 635f 6d61 736b 2c20 7665  nge(vec_mask, ve
-000149b0: 635f 6365 6c6c 290d 0a0d 0a20 2020 2020  c_cell)....     
-000149c0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000149d0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000149e0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000149f0: 6174 6528 7b73 656c 662e 7261 6469 616c  ate({self.radial
-00014a00: 5f61 6e67 6c65 5f6b 6579 203a 2061 6e67  _angle_key : ang
-00014a10: 6c65 7d29 2020 2020 2020 2020 2020 2020  le})            
-00014a20: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00014a30: 2020 2020 756e 6971 7565 5f74 7261 636b      unique_track
-00014a40: 6c65 745f 6964 732e 6170 7065 6e64 2873  let_ids.append(s
-00014a50: 7472 2875 6e69 7175 655f 6964 2929 0d0a  tr(unique_id))..
-00014a60: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014a70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014a80: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014a90: 5d2e 7570 6461 7465 287b 7365 6c66 2e63  ].update({self.c
-00014aa0: 6c75 7374 6572 636c 6173 735f 6b65 7920  lusterclass_key 
-00014ab0: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
-00014ac0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014ad0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014ae0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014af0: 7465 287b 7365 6c66 2e63 6c75 7374 6572  te({self.cluster
-00014b00: 7363 6f72 655f 6b65 7920 3a20 307d 290d  score_key : 0}).
-00014b10: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014b20: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014b30: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014b40: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014b50: 756e 6971 7565 6964 5f6b 6579 203a 2073  uniqueid_key : s
-00014b60: 7472 2875 6e69 7175 655f 6964 297d 290d  tr(unique_id)}).
-00014b70: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014b80: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014b90: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014ba0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014bb0: 7472 6163 6b6c 6574 6964 5f6b 6579 203a  trackletid_key :
-00014bc0: 2073 7472 2874 7261 636b 6c65 745f 6964   str(tracklet_id
-00014bd0: 297d 2920 0d0a 2020 2020 2020 2020 7365  )}) ..        se
-00014be0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014bf0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014c00: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014c10: 7365 6c66 2e67 656e 6572 6174 696f 6e69  self.generationi
-00014c20: 645f 6b65 7920 3a20 7374 7228 6765 6e65  d_key : str(gene
-00014c30: 7261 7469 6f6e 5f69 6429 7d29 200d 0a20  ration_id)}) .. 
-00014c40: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00014c50: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014c60: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00014c70: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
-00014c80: 6163 6b69 645f 6b65 7920 3a20 7374 7228  ackid_key : str(
-00014c90: 7472 6163 6b5f 6964 297d 290d 0a20 2020  track_id)})..   
-00014ca0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014cb0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014cc0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00014cd0: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
-00014ce0: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 2030  on_angle_key : 0
-00014cf0: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
-00014d00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014d10: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014d20: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014d30: 7365 6c66 2e73 7065 6564 5f6b 6579 203a  self.speed_key :
-00014d40: 2030 2e30 7d29 0d0a 2020 2020 2020 2020   0.0})..        
-00014d50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014d60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014d70: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014d80: 287b 7365 6c66 2e61 6363 656c 6572 6174  ({self.accelerat
-00014d90: 696f 6e5f 6b65 7920 3a20 302e 307d 290d  ion_key : 0.0}).
-00014da0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014db0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014dc0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014dd0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014de0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00014df0: 705f 6669 7273 746b 6579 203a 204e 6f6e  p_firstkey : Non
-00014e00: 657d 290d 0a20 2020 2020 2020 2073 656c  e})..        sel
-00014e10: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014e20: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014e30: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014e40: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00014e50: 5f63 6f6d 705f 7365 636f 6e64 6b65 7920  _comp_secondkey 
-00014e60: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
-00014e70: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00014e80: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00014e90: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00014ea0: 7465 287b 7365 6c66 2e73 7572 6661 6365  te({self.surface
-00014eb0: 5f61 7265 615f 6b65 7920 3a20 4e6f 6e65  _area_key : None
-00014ec0: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
-00014ed0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00014ee0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00014ef0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00014f00: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
-00014f10: 5f6b 6579 203a 204e 6f6e 657d 290d 0a0d  _key : None})...
-00014f20: 0a20 2020 2020 2020 2069 6620 736f 7572  .        if sour
-00014f30: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
-00014f40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00014f50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00014f60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00014f70: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00014f80: 287b 7365 6c66 2e62 6566 6f72 6569 645f  ({self.beforeid_
-00014f90: 6b65 7920 3a20 696e 7428 736f 7572 6365  key : int(source
-00014fa0: 5f69 6429 7d29 0d0a 2020 2020 2020 2020  _id)})..        
-00014fb0: 2020 2020 7665 635f 3120 3d20 5b66 6c6f      vec_1 = [flo
-00014fc0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00014fd0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00014fe0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00014ff0: 662e 7870 6f73 6964 5f6b 6579 5d29 202d  f.xposid_key]) -
-00015000: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00015010: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015020: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
-00015030: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-00015040: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015060: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00015070: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015080: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015090: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-000150a0: 6b65 795d 2920 2d20 666c 6f61 7428 7365  key]) - float(se
-000150b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000150c0: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
-000150d0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e79  urce_id)][self.y
-000150e0: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00015110: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015120: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015130: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00015140: 7a70 6f73 6964 5f6b 6579 5d29 202d 2020  zposid_key]) -  
-00015150: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015160: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015170: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-00015180: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00015190: 795d 295d 0d0a 2020 2020 2020 2020 2020  y])]..          
-000151a0: 2020 7370 6565 6420 3d20 6e70 2e73 7172    speed = np.sqr
-000151b0: 7428 6e70 2e64 6f74 2876 6563 5f31 2c20  t(np.dot(vec_1, 
-000151c0: 7665 635f 3129 292f 7365 6c66 2e74 6361  vec_1))/self.tca
-000151d0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-000151e0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000151f0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015200: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015210: 2e75 7064 6174 6528 7b73 656c 662e 7370  .update({self.sp
-00015220: 6565 645f 6b65 7920 3a20 7370 6565 647d  eed_key : speed}
-00015230: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00015240: 206d 6f74 696f 6e5f 616e 676c 6520 3d20   motion_angle = 
-00015250: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
-00015260: 6563 5f6d 6173 6b2c 2076 6563 5f31 290d  ec_mask, vec_1).
-00015270: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
-00015280: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015290: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000152a0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-000152b0: 7b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  {self.motion_ang
-000152c0: 6c65 5f6b 6579 203a 206d 6f74 696f 6e5f  le_key : motion_
-000152d0: 616e 676c 657d 2920 0d0a 0d0a 2020 2020  angle}) ....    
-000152e0: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
-000152f0: 655f 6964 2069 6e20 7365 6c66 2e65 6467  e_id in self.edg
-00015300: 655f 736f 7572 6365 5f6c 6f6f 6b75 703a  e_source_lookup:
-00015310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015320: 2020 2020 2020 7072 655f 736f 7572 6365        pre_source
-00015330: 5f69 6420 3d20 7365 6c66 2e65 6467 655f  _id = self.edge_
-00015340: 736f 7572 6365 5f6c 6f6f 6b75 705b 736f  source_lookup[so
-00015350: 7572 6365 5f69 645d 0d0a 2020 2020 2020  urce_id]..      
-00015360: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015380: 2020 2020 7665 635f 3220 3d20 5b66 6c6f      vec_2 = [flo
-00015390: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-000153a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000153b0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-000153c0: 662e 7870 6f73 6964 5f6b 6579 5d29 202d  f.xposid_key]) -
-000153d0: 2032 202a 2066 6c6f 6174 2873 656c 662e   2 * float(self.
-000153e0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000153f0: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015400: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
-00015410: 6964 5f6b 6579 5d29 202b 2066 6c6f 6174  id_key]) + float
-00015420: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015430: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015440: 2870 7265 5f73 6f75 7263 655f 6964 295d  (pre_source_id)]
-00015450: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00015460: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
-00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015480: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
-00015490: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000154a0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000154b0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-000154c0: 795d 2920 2d20 3220 2a20 666c 6f61 7428  y]) - 2 * float(
-000154d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000154e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000154f0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00015500: 2e79 706f 7369 645f 6b65 795d 2920 2b20  .yposid_key]) + 
-00015510: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015520: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015530: 735b 696e 7428 7072 655f 736f 7572 6365  s[int(pre_source
-00015540: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-00015550: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-00015580: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015590: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000155a0: 6c5f 6964 295d 5b73 656c 662e 7a70 6f73  l_id)][self.zpos
-000155b0: 6964 5f6b 6579 5d29 202d 2020 3220 2a20  id_key]) -  2 * 
-000155c0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000155d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000155e0: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-000155f0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00015600: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
-00015610: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015620: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
-00015630: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00015640: 2e7a 706f 7369 645f 6b65 795d 295d 0d0a  .zposid_key])]..
-00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015660: 2020 2020 6163 6320 3d20 6e70 2e73 7172      acc = np.sqr
-00015670: 7428 6e70 2e64 6f74 2876 6563 5f32 2c20  t(np.dot(vec_2, 
-00015680: 7665 635f 3229 292f 7365 6c66 2e74 6361  vec_2))/self.tca
-00015690: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-000156a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000156b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156c0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000156d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000156e0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-000156f0: 7064 6174 6528 7b73 656c 662e 6163 6365  pdate({self.acce
-00015700: 6c65 7261 7469 6f6e 5f6b 6579 203a 2061  leration_key : a
-00015710: 6363 7d29 0d0a 2020 2020 2020 2020 656c  cc})..        el
-00015720: 6966 2073 6f75 7263 655f 6964 2069 7320  if source_id is 
-00015730: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00015740: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015750: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015760: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015770: 6174 6528 7b73 656c 662e 6265 666f 7265  ate({self.before
-00015780: 6964 5f6b 6579 203a 204e 6f6e 657d 2920  id_key : None}) 
-00015790: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-000157a0: 0d0a 2020 2020 2020 2020 6966 2074 6172  ..        if tar
-000157b0: 6765 745f 6964 2069 7320 6e6f 7420 4e6f  get_id is not No
-000157c0: 6e65 3a20 2020 2020 2020 0d0a 2020 2020  ne:       ..    
-000157d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000157e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000157f0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015800: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-00015810: 6674 6572 6964 5f6b 6579 203a 2069 6e74  fterid_key : int
-00015820: 2874 6172 6765 745f 6964 297d 2920 0d0a  (target_id)}) ..
-00015830: 2020 2020 2020 2020 656c 6966 2074 6172          elif tar
-00015840: 6765 745f 6964 2069 7320 4e6f 6e65 3a0d  get_id is None:.
-00015850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015860: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015870: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015880: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015890: 656c 662e 6166 7465 7269 645f 6b65 7920  elf.afterid_key 
-000158a0: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
-000158b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000158c0: 7365 6c66 2e5f 7365 636f 6e64 5f63 6861  self._second_cha
-000158d0: 6e6e 656c 5f75 7064 6174 6528 6365 6c6c  nnel_update(cell
-000158e0: 5f69 642c 2074 7261 636b 5f69 6429 2020  _id, track_id)  
-000158f0: 2020 0d0a 0d0a 0d0a 2020 2020 6465 6620    ......    def 
-00015900: 5f74 656d 706f 7261 6c5f 706c 6f74 735f  _temporal_plots_
-00015910: 7472 6163 6b6d 6174 6528 7365 6c66 293a  trackmate(self):
-00015920: 0d0a 2020 2020 0d0a 2020 2020 0d0a 2020  ..    ..    ..  
-00015930: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00015940: 2020 2020 7365 6c66 2e41 7474 7220 3d20      self.Attr = 
-00015950: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00015960: 2020 2020 7374 6172 7474 696d 6520 3d20      starttime = 
-00015970: 696e 7428 6d69 6e28 7365 6c66 2e41 6c6c  int(min(self.All
-00015980: 5661 6c75 6573 5b73 656c 662e 6672 616d  Values[self.fram
-00015990: 6569 645f 6b65 795d 2929 0d0a 2020 2020  eid_key]))..    
-000159a0: 2020 2020 2020 2020 2020 2020 656e 6474              endt
-000159b0: 696d 6520 3d20 696e 7428 6d61 7828 7365  ime = int(max(se
-000159c0: 6c66 2e41 6c6c 5661 6c75 6573 5b73 656c  lf.AllValues[sel
-000159d0: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
-000159e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000159f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00015a00: 2020 2020 2073 656c 662e 7469 6d65 203d       self.time =
-00015a10: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015a20: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00015a30: 635f 6d65 616e 5f64 6973 705f 7a20 3d20  c_mean_disp_z = 
-00015a40: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00015a50: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015a60: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
-00015a70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015a80: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015a90: 5f6d 6561 6e5f 6469 7370 5f79 203d 205b  _mean_disp_y = [
-00015aa0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015ab0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00015ac0: 7661 725f 6469 7370 5f79 203d 205b 5d0d  var_disp_y = [].
-00015ad0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015ae0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00015af0: 6d65 616e 5f64 6973 705f 7820 3d20 5b5d  mean_disp_x = []
-00015b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015b10: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00015b20: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
-00015b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015b40: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00015b50: 6561 6e5f 7261 6469 7573 203d 205b 5d0d  ean_radius = [].
-00015b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015b70: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00015b80: 725f 7261 6469 7573 203d 205b 5d0d 0a0d  r_radius = []...
-00015b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ba0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00015bb0: 616e 5f73 7065 6564 203d 205b 5d0d 0a20  an_speed = [].. 
-00015bc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015bd0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00015be0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
-00015bf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015c00: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015c10: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
-00015c20: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015c30: 6974 6f74 6963 5f76 6172 5f61 6363 203d  itotic_var_acc =
-00015c40: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015c50: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015c60: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
-00015c70: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00015c80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015c90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00015ca0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00015cb0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
-00015cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015cd0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00015ce0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00015cf0: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00015d00: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015d10: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-00015d20: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00015d30: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00015d40: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00015d50: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015d60: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00015d70: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00015d80: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00015d90: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
-00015da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015db0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00015dc0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
-00015dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015de0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00015df0: 7661 725f 6469 7370 5f79 203d 205b 5d0d  var_disp_y = [].
-00015e00: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00015e10: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015e20: 7469 635f 6d65 616e 5f64 6973 705f 7820  tic_mean_disp_x 
-00015e30: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015e40: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015e50: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00015e60: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
-00015e70: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00015e80: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00015e90: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00015ea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015eb0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00015ec0: 725f 7261 6469 7573 203d 205b 5d0d 0a0d  r_radius = []...
-00015ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ee0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00015ef0: 635f 6d65 616e 5f73 7065 6564 203d 205b  c_mean_speed = [
-00015f00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015f10: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00015f20: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
-00015f30: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00015f40: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015f50: 6974 6f74 6963 5f6d 6561 6e5f 6163 6320  itotic_mean_acc 
-00015f60: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015f70: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015f80: 6974 6f74 6963 5f76 6172 5f61 6363 203d  itotic_var_acc =
-00015f90: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015fa0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00015fb0: 6d69 746f 7469 635f 6d65 616e 5f64 6972  mitotic_mean_dir
-00015fc0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00015fd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00015fe0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00015ff0: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
-00016000: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016010: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016020: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00016030: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
-00016040: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00016050: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016060: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00016070: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-00016080: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016090: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000160a0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-000160b0: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
-000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160d0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
-000160e0: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
-000160f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016100: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f79  .all_mean_disp_y
-00016110: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016120: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00016130: 7661 725f 6469 7370 5f79 203d 205b 5d0d  var_disp_y = [].
-00016140: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016150: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00016160: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00016170: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016180: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-00016190: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
-000161a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000161b0: 6c6c 5f6d 6561 6e5f 7261 6469 7573 203d  ll_mean_radius =
-000161c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000161d0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-000161e0: 725f 7261 6469 7573 203d 205b 5d0d 0a0d  r_radius = []...
-000161f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016200: 2073 656c 662e 616c 6c5f 6d65 616e 5f73   self.all_mean_s
-00016210: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00016220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016230: 616c 6c5f 7661 725f 7370 6565 6420 3d20  all_var_speed = 
-00016240: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016250: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00016260: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
-00016270: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016280: 6c66 2e61 6c6c 5f76 6172 5f61 6363 203d  lf.all_var_acc =
-00016290: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000162a0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000162b0: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
-000162c0: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-000162d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000162e0: 6c66 2e61 6c6c 5f76 6172 5f64 6972 6563  lf.all_var_direc
-000162f0: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016300: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016310: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00016320: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00016330: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00016340: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016350: 662e 616c 6c5f 7661 725f 6469 7374 616e  f.all_var_distan
-00016360: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016370: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016380: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00016390: 635f 636c 7573 7465 725f 636c 6173 7320  c_cluster_class 
-000163a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000163b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000163c0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-000163d0: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
-000163e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000163f0: 616c 6c5f 636c 7573 7465 725f 636c 6173  all_cluster_clas
-00016400: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-00016410: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00016420: 6f74 735f 7472 6163 6b73 203d 207b 7d0d  ots_tracks = {}.
-00016430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016440: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00016450: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016460: 726f 7065 7274 6965 732e 6974 656d 7328  roperties.items(
-00016470: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016480: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164a0: 2020 616c 6c5f 7370 6f74 7320 3d20 7365    all_spots = se
-000164b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000164c0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-000164d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164e0: 2020 2020 6966 2073 656c 662e 7472 6163      if self.trac
-000164f0: 6b69 645f 6b65 7920 696e 2061 6c6c 5f73  kid_key in all_s
-00016500: 706f 7473 3a0d 0a20 2020 2020 2020 2020  pots:..         
-00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016520: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00016530: 735b 6b5d 203d 2061 6c6c 5f73 706f 7473  s[k] = all_spots
-00016540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016550: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00013b40: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+00013b50: 6579 203a 2066 6c6f 6174 2863 656e 7472  ey : float(centr
+00013b60: 6f69 6473 5b69 6e64 6578 5d5b 325d 2a20  oids[index][2]* 
+00013b70: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00013b80: 6e29 2c0d 0a20 2020 2020 2020 2020 2020  n),..           
+00013b90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013ba0: 662e 7472 6163 6b69 645f 6b65 793a 2069  f.trackid_key: i
+00013bb0: 6e74 2874 7261 636b 5f69 6429 2c0d 0a20  nt(track_id),.. 
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+00013be0: 6c5f 696e 7465 6e73 6974 795f 6b65 7920  l_intensity_key 
+00013bf0: 3a20 2866 6c6f 6174 2869 6e74 656e 7369  : (float(intensi
+00013c00: 7479 5f74 6f74 616c 5b69 6e64 6578 5d29  ty_total[index])
+00013c10: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00013c20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013c30: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+00013c40: 6b65 7920 3a20 2866 6c6f 6174 2869 6e74  key : (float(int
+00013c50: 656e 7369 7479 5f6d 6561 6e5b 696e 6465  ensity_mean[inde
+00013c60: 785d 2929 2c0d 0a0d 0a20 2020 2020 2020  x])),....       
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c80: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
+00013c90: 203a 2028 666c 6f61 7428 5241 4449 5553   : (float(RADIUS
+00013ca0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+00013cb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013cc0: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+00013cd0: 2866 6c6f 6174 2851 5541 4c49 5459 2929  (float(QUALITY))
+00013ce0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00013cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013d00: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00013d10: 736b 5f6b 6579 3a20 666c 6f61 7428 6469  sk_key: float(di
+00013d20: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00013d30: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00013d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013d50: 2e6d 6173 6b63 656e 7472 6f69 645f 7a5f  .maskcentroid_z_
+00013d60: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+00013d70: 656e 7472 6f69 645b 305d 292c 0d0a 2020  entroid[0]),..  
+00013d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d90: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
+00013da0: 656e 7472 6f69 645f 795f 6b65 793a 2066  entroid_y_key: f
+00013db0: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
+00013dc0: 645b 315d 292c 0d0a 2020 2020 2020 2020  d[1]),..        
+00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013de0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+00013df0: 645f 785f 6b65 793a 2066 6c6f 6174 286d  d_x_key: float(m
+00013e00: 6173 6b63 656e 7472 6f69 645b 325d 2920  askcentroid[2]) 
+00013e10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00013e20: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
+00013e30: 2020 2065 6c69 6620 7365 6c66 2e65 6467     elif self.edg
+00013e40: 655f 736f 7572 6365 5f6c 6f6f 6b75 705b  e_source_lookup[
+00013e50: 6365 6c6c 5f69 645d 2069 7320 6e6f 7420  cell_id] is not 
+00013e60: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00013e70: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00013e80: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00013e90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00013ea0: 735b 7365 6c66 2e65 6467 655f 736f 7572  s[self.edge_sour
+00013eb0: 6365 5f6c 6f6f 6b75 705b 6365 6c6c 5f69  ce_lookup[cell_i
+00013ec0: 645d 5d20 6973 206e 6f74 204e 6f6e 653a  d]] is not None:
+00013ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013ee0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00013ef0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00013f00: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00013f10: 6c5f 6964 5d20 3d20 7365 6c66 2e63 6861  l_id] = self.cha
+00013f20: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+00013f30: 5f70 726f 7065 7274 6965 735b 7365 6c66  _properties[self
+00013f40: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+00013f50: 6b75 705b 6365 6c6c 5f69 645d 5d0d 0a20  kup[cell_id]].. 
+00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f70: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f90: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+00013fa0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00013fb0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+00013fc0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00013fd0: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+00013fe0: 5f69 645d 2020 2020 200d 0a20 2020 2020  _id]     ..     
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014000: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00014010: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00014020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014030: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00014040: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014050: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
+00014060: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00014070: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+00014080: 6c6c 5f69 645d 0d0a 0d0a 0d0a 2020 2020  ll_id]......    
+00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140a0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000140b0: 2020 2064 6566 205f 6469 6374 5f75 7064     def _dict_upd
+000140c0: 6174 6528 7365 6c66 2c20 756e 6971 7565  ate(self, unique
+000140d0: 5f74 7261 636b 6c65 745f 6964 733a 204c  _tracklet_ids: L
+000140e0: 6973 742c 2020 6365 6c6c 5f69 643a 2069  ist,  cell_id: i
+000140f0: 6e74 2c20 7472 6163 6b5f 6964 3a20 696e  nt, track_id: in
+00014100: 742c 2073 6f75 7263 655f 6964 3a20 696e  t, source_id: in
+00014110: 742c 2074 6172 6765 745f 6964 3a20 696e  t, target_id: in
+00014120: 7429 3a0d 0a0d 0a20 0d0a 2020 2020 2020  t):.... ..      
+00014130: 2020 6765 6e65 7261 7469 6f6e 5f69 6420    generation_id 
+00014140: 3d20 7365 6c66 2e67 656e 6572 6174 696f  = self.generatio
+00014150: 6e5f 6469 6374 5b63 656c 6c5f 6964 5d0d  n_dict[cell_id].
+00014160: 0a20 2020 2020 2020 2074 7261 636b 6c65  .        trackle
+00014170: 745f 6964 203d 2073 656c 662e 7472 6163  t_id = self.trac
+00014180: 6b6c 6574 5f64 6963 745b 6365 6c6c 5f69  klet_dict[cell_i
+00014190: 645d 0d0a 0d0a 2020 2020 2020 2020 756e  d]....        un
+000141a0: 6971 7565 5f69 6420 3d20 7374 7228 7472  ique_id = str(tr
+000141b0: 6163 6b5f 6964 2920 2b20 7374 7228 7365  ack_id) + str(se
+000141c0: 6c66 2e6d 6178 5f74 7261 636b 5f69 6429  lf.max_track_id)
+000141d0: 202b 2073 7472 2867 656e 6572 6174 696f   + str(generatio
+000141e0: 6e5f 6964 2920 2b20 7374 7228 7472 6163  n_id) + str(trac
+000141f0: 6b6c 6574 5f69 6429 0d0a 2020 2020 2020  klet_id)..      
+00014200: 2020 0d0a 2020 2020 2020 2020 7665 635f    ..        vec_
+00014210: 6d61 736b 203d 205b 666c 6f61 7428 7365  mask = [float(se
+00014220: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014230: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014240: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
+00014250: 6b63 656e 7472 6f69 645f 785f 6b65 795d  kcentroid_x_key]
+00014260: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
+00014270: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014280: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00014290: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
+000142a0: 726f 6964 5f79 5f6b 6579 5d29 2c20 666c  roid_y_key]), fl
+000142b0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000142c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000142d0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+000142e0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+000142f0: 7a5f 6b65 795d 2920 5d0d 0a0d 0a20 2020  z_key]) ]....   
+00014300: 2020 2020 2076 6563 5f63 656c 6c20 3d20       vec_cell = 
+00014310: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
+00014320: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014330: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014340: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+00014350: 5d29 202c 200d 0a20 2020 2020 2020 2020  ]) , ..         
+00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014370: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+00014380: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00014390: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000143a0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+000143b0: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143d0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
+000143e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000143f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014400: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00014410: 6b65 795d 295d 0d0a 0d0a 2020 2020 2020  key])]....      
+00014420: 2020 616e 676c 6520 3d20 616e 6775 6c61    angle = angula
+00014430: 725f 6368 616e 6765 2876 6563 5f6d 6173  r_change(vec_mas
+00014440: 6b2c 2076 6563 5f63 656c 6c29 0d0a 0d0a  k, vec_cell)....
+00014450: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00014460: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014470: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014480: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
+00014490: 6164 6961 6c5f 616e 676c 655f 6b65 7920  adial_angle_key 
+000144a0: 3a20 616e 676c 657d 2920 2020 2020 2020  : angle})       
+000144b0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+000144c0: 0a20 2020 2020 2020 2075 6e69 7175 655f  .        unique_
+000144d0: 7472 6163 6b6c 6574 5f69 6473 2e61 7070  tracklet_ids.app
+000144e0: 656e 6428 7374 7228 756e 6971 7565 5f69  end(str(unique_i
+000144f0: 6429 290d 0a20 2020 2020 2020 2073 656c  d))..        sel
+00014500: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014510: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014520: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00014530: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
+00014540: 5f6b 6579 203a 204e 6f6e 657d 290d 0a20  _key : None}).. 
+00014550: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014560: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014570: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014580: 2e75 7064 6174 6528 7b73 656c 662e 636c  .update({self.cl
+00014590: 7573 7465 7273 636f 7265 5f6b 6579 203a  usterscore_key :
+000145a0: 2030 7d29 0d0a 2020 2020 2020 2020 7365   0})..        se
+000145b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000145c0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000145d0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000145e0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+000145f0: 7920 3a20 7374 7228 756e 6971 7565 5f69  y : str(unique_i
+00014600: 6429 7d29 0d0a 2020 2020 2020 2020 7365  d)})..        se
+00014610: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014620: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014630: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00014640: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
+00014650: 6b65 7920 3a20 7374 7228 7472 6163 6b6c  key : str(trackl
+00014660: 6574 5f69 6429 7d29 200d 0a20 2020 2020  et_id)}) ..     
+00014670: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00014680: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014690: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000146a0: 6174 6528 7b73 656c 662e 6765 6e65 7261  ate({self.genera
+000146b0: 7469 6f6e 6964 5f6b 6579 203a 2073 7472  tionid_key : str
+000146c0: 2867 656e 6572 6174 696f 6e5f 6964 297d  (generation_id)}
+000146d0: 2920 0d0a 2020 2020 2020 2020 7365 6c66  ) ..        self
+000146e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000146f0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00014700: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00014710: 6c66 2e74 7261 636b 6964 5f6b 6579 203a  lf.trackid_key :
+00014720: 2073 7472 2874 7261 636b 5f69 6429 7d29   str(track_id)})
+00014730: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00014740: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00014750: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00014760: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00014770: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
+00014780: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
+00014790: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+000147a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000147b0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000147c0: 6174 6528 7b73 656c 662e 7370 6565 645f  ate({self.speed_
+000147d0: 6b65 7920 3a20 302e 307d 290d 0a20 2020  key : 0.0})..   
+000147e0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000147f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014800: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00014810: 7064 6174 6528 7b73 656c 662e 6163 6365  pdate({self.acce
+00014820: 6c65 7261 7469 6f6e 5f6b 6579 203a 2030  leration_key : 0
+00014830: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
+00014840: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014850: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014860: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00014870: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+00014880: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
+00014890: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
+000148a0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+000148b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000148c0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+000148d0: 7465 287b 7365 6c66 2e65 6363 656e 7472  te({self.eccentr
+000148e0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+000148f0: 646b 6579 203a 204e 6f6e 657d 290d 0a20  dkey : None}).. 
+00014900: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014910: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014920: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014930: 2e75 7064 6174 6528 7b73 656c 662e 7375  .update({self.su
+00014940: 7266 6163 655f 6172 6561 5f6b 6579 203a  rface_area_key :
+00014950: 204e 6f6e 657d 290d 0a20 2020 2020 2020   None})..       
+00014960: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014970: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014980: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014990: 6528 7b73 656c 662e 6365 6c6c 6178 6973  e({self.cellaxis
+000149a0: 5f6d 6173 6b5f 6b65 7920 3a20 4e6f 6e65  _mask_key : None
+000149b0: 7d29 0d0a 0d0a 2020 2020 2020 2020 6966  })....        if
+000149c0: 2073 6f75 7263 655f 6964 2069 7320 6e6f   source_id is no
+000149d0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+000149e0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000149f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014a00: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00014a10: 7064 6174 6528 7b73 656c 662e 6265 666f  pdate({self.befo
+00014a20: 7265 6964 5f6b 6579 203a 2069 6e74 2873  reid_key : int(s
+00014a30: 6f75 7263 655f 6964 297d 290d 0a20 2020  ource_id)})..   
+00014a40: 2020 2020 2020 2020 2076 6563 5f31 203d           vec_1 =
+00014a50: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
+00014a60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014a70: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014a80: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00014a90: 795d 2920 2d20 666c 6f61 7428 7365 6c66  y]) - float(self
+00014aa0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014ab0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00014ac0: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
+00014ad0: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+00014ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014af0: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+00014b00: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014b10: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00014b20: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
+00014b30: 6f73 6964 5f6b 6579 5d29 202d 2066 6c6f  osid_key]) - flo
+00014b40: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00014b50: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00014b60: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+00014b70: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00014b80: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00014b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ba0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014bb0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014bc0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00014bd0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00014be0: 2920 2d20 2066 6c6f 6174 2873 656c 662e  ) -  float(self.
+00014bf0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014c00: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
+00014c10: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
+00014c20: 6964 5f6b 6579 5d29 5d0d 0a20 2020 2020  id_key])]..     
+00014c30: 2020 2020 2020 2073 7065 6564 203d 206e         speed = n
+00014c40: 702e 7371 7274 286e 702e 646f 7428 7665  p.sqrt(np.dot(ve
+00014c50: 635f 312c 2076 6563 5f31 2929 2f73 656c  c_1, vec_1))/sel
+00014c60: 662e 7463 616c 6962 7261 7469 6f6e 0d0a  f.tcalibration..
+00014c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014c80: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014c90: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00014ca0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00014cb0: 6c66 2e73 7065 6564 5f6b 6579 203a 2073  lf.speed_key : s
+00014cc0: 7065 6564 7d29 0d0a 0d0a 2020 2020 2020  peed})....      
+00014cd0: 2020 2020 2020 6d6f 7469 6f6e 5f61 6e67        motion_ang
+00014ce0: 6c65 203d 2061 6e67 756c 6172 5f63 6861  le = angular_cha
+00014cf0: 6e67 6528 7665 635f 6d61 736b 2c20 7665  nge(vec_mask, ve
+00014d00: 635f 3129 0d0a 0d0a 2020 2020 2020 2020  c_1)....        
+00014d10: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014d20: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00014d30: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00014d40: 6461 7465 287b 7365 6c66 2e6d 6f74 696f  date({self.motio
+00014d50: 6e5f 616e 676c 655f 6b65 7920 3a20 6d6f  n_angle_key : mo
+00014d60: 7469 6f6e 5f61 6e67 6c65 7d29 200d 0a0d  tion_angle}) ...
+00014d70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00014d80: 736f 7572 6365 5f69 6420 696e 2073 656c  source_id in sel
+00014d90: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
+00014da0: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
+00014db0: 2020 2020 2020 2020 2020 2070 7265 5f73             pre_s
+00014dc0: 6f75 7263 655f 6964 203d 2073 656c 662e  ource_id = self.
+00014dd0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
+00014de0: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
+00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00014e10: 2020 2020 2020 2020 2076 6563 5f32 203d           vec_2 =
+00014e20: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
+00014e30: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014e40: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014e50: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00014e60: 795d 2920 2d20 3220 2a20 666c 6f61 7428  y]) - 2 * float(
+00014e70: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014e80: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014e90: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
+00014ea0: 2e78 706f 7369 645f 6b65 795d 2920 2b20  .xposid_key]) + 
+00014eb0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00014ec0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00014ed0: 735b 696e 7428 7072 655f 736f 7572 6365  s[int(pre_source
+00014ee0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
+00014ef0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f10: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00014f20: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014f30: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014f40: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
+00014f50: 6964 5f6b 6579 5d29 202d 2032 202a 2066  id_key]) - 2 * f
+00014f60: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00014f70: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00014f80: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
+00014f90: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00014fa0: 5d29 202b 2066 6c6f 6174 2873 656c 662e  ]) + float(self.
+00014fb0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014fc0: 6572 7469 6573 5b69 6e74 2870 7265 5f73  erties[int(pre_s
+00014fd0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+00014fe0: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
+00014ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015000: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00015010: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015020: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015030: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00015040: 2e7a 706f 7369 645f 6b65 795d 2920 2d20  .zposid_key]) - 
+00015050: 2032 202a 2066 6c6f 6174 2873 656c 662e   2 * float(self.
+00015060: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015070: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
+00015080: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
+00015090: 6964 5f6b 6579 5d29 202b 2066 6c6f 6174  id_key]) + float
+000150a0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000150b0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000150c0: 2870 7265 5f73 6f75 7263 655f 6964 295d  (pre_source_id)]
+000150d0: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
+000150e0: 5d29 5d0d 0a20 2020 2020 2020 2020 2020  ])]..           
+000150f0: 2020 2020 2020 2020 2061 6363 203d 206e           acc = n
+00015100: 702e 7371 7274 286e 702e 646f 7428 7665  p.sqrt(np.dot(ve
+00015110: 635f 322c 2076 6563 5f32 2929 2f73 656c  c_2, vec_2))/sel
+00015120: 662e 7463 616c 6962 7261 7469 6f6e 0d0a  f.tcalibration..
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00015150: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00015160: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015170: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015180: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015190: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
+000151a0: 7920 3a20 6163 637d 290d 0a20 2020 2020  y : acc})..     
+000151b0: 2020 2065 6c69 6620 736f 7572 6365 5f69     elif source_i
+000151c0: 6420 6973 204e 6f6e 653a 0d0a 2020 2020  d is None:..    
+000151d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000151e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000151f0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015200: 5d2e 7570 6461 7465 287b 7365 6c66 2e62  ].update({self.b
+00015210: 6566 6f72 6569 645f 6b65 7920 3a20 4e6f  eforeid_key : No
+00015220: 6e65 7d29 200d 0a20 2020 2020 2020 2020  ne}) ..         
+00015230: 2020 200d 0a0d 0a20 2020 2020 2020 2069     ....        i
+00015240: 6620 7461 7267 6574 5f69 6420 6973 206e  f target_id is n
+00015250: 6f74 204e 6f6e 653a 2020 2020 2020 200d  ot None:       .
+00015260: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00015270: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015280: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015290: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+000152a0: 656c 662e 6166 7465 7269 645f 6b65 7920  elf.afterid_key 
+000152b0: 3a20 696e 7428 7461 7267 6574 5f69 6429  : int(target_id)
+000152c0: 7d29 200d 0a20 2020 2020 2020 2065 6c69  }) ..        eli
+000152d0: 6620 7461 7267 6574 5f69 6420 6973 204e  f target_id is N
+000152e0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000152f0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00015300: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00015310: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00015320: 7465 287b 7365 6c66 2e61 6674 6572 6964  te({self.afterid
+00015330: 5f6b 6579 203a 204e 6f6e 657d 290d 0a20  _key : None}).. 
+00015340: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00015350: 2020 2020 2073 656c 662e 5f73 6563 6f6e       self._secon
+00015360: 645f 6368 616e 6e65 6c5f 7570 6461 7465  d_channel_update
+00015370: 2863 656c 6c5f 6964 2c20 7472 6163 6b5f  (cell_id, track_
+00015380: 6964 2920 2020 200d 0a0d 0a0d 0a20 2020  id)    ......   
+00015390: 2064 6566 205f 7465 6d70 6f72 616c 5f70   def _temporal_p
+000153a0: 6c6f 7473 5f74 7261 636b 6d61 7465 2873  lots_trackmate(s
+000153b0: 656c 6629 3a0d 0a20 2020 200d 0a20 2020  elf):..    ..   
+000153c0: 200d 0a20 2020 200d 0a20 2020 2020 2020   ..    ..       
+000153d0: 2020 2020 2020 2020 2073 656c 662e 4174           self.At
+000153e0: 7472 203d 207b 7d0d 0a20 2020 2020 2020  tr = {}..       
+000153f0: 2020 2020 2020 2020 2073 7461 7274 7469           startti
+00015400: 6d65 203d 2069 6e74 286d 696e 2873 656c  me = int(min(sel
+00015410: 662e 416c 6c56 616c 7565 735b 7365 6c66  f.AllValues[self
+00015420: 2e66 7261 6d65 6964 5f6b 6579 5d29 290d  .frameid_key])).
+00015430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015440: 2065 6e64 7469 6d65 203d 2069 6e74 286d   endtime = int(m
+00015450: 6178 2873 656c 662e 416c 6c56 616c 7565  ax(self.AllValue
+00015460: 735b 7365 6c66 2e66 7261 6d65 6964 5f6b  s[self.frameid_k
+00015470: 6579 5d29 290d 0a20 2020 2020 2020 2020  ey]))..         
+00015480: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00015490: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000154a0: 696d 6520 3d20 5b5d 0d0a 2020 2020 2020  ime = []..      
+000154b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000154c0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+000154d0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+000154e0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+000154f0: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
+00015500: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00015510: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00015520: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00015530: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00015540: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015550: 6f74 6963 5f76 6172 5f64 6973 705f 7920  otic_var_disp_y 
+00015560: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015570: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015580: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
+00015590: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000155a0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+000155b0: 7469 635f 7661 725f 6469 7370 5f78 203d  tic_var_disp_x =
+000155c0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+000155d0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+000155e0: 7469 635f 6d65 616e 5f72 6164 6975 7320  tic_mean_radius 
+000155f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00015600: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015610: 6963 5f76 6172 5f72 6164 6975 7320 3d20  ic_var_radius = 
+00015620: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015630: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00015640: 6963 5f6d 6561 6e5f 7370 6565 6420 3d20  ic_mean_speed = 
+00015650: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015660: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00015670: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
+00015680: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00015690: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000156a0: 6d65 616e 5f61 6363 203d 205b 5d0d 0a20  mean_acc = [].. 
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000156c0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+000156d0: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
+000156e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000156f0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00015700: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00015710: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00015720: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015730: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
+00015740: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00015750: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00015760: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015770: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
+00015780: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00015790: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000157a0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+000157b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000157c0: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
+000157d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000157e0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000157f0: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
+00015800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015810: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00015820: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
+00015830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015840: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00015850: 635f 6d65 616e 5f64 6973 705f 7920 3d20  c_mean_disp_y = 
+00015860: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00015870: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00015880: 6f74 6963 5f76 6172 5f64 6973 705f 7920  otic_var_disp_y 
+00015890: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+000158a0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000158b0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+000158c0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+000158d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000158e0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+000158f0: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
+00015900: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015910: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00015920: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
+00015930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015940: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00015950: 6963 5f76 6172 5f72 6164 6975 7320 3d20  ic_var_radius = 
+00015960: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015970: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00015980: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+00015990: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+000159a0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000159b0: 5f6d 6974 6f74 6963 5f76 6172 5f73 7065  _mitotic_var_spe
+000159c0: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
+000159d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000159e0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000159f0: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
+00015a00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015a10: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00015a20: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
+00015a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015a40: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00015a50: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
+00015a60: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
+00015a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015a80: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00015a90: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00015aa0: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
+00015ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015ac0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00015ad0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00015ae0: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
+00015af0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00015b00: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00015b10: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00015b20: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
+00015b30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015b40: 6c6c 5f6d 6561 6e5f 6469 7370 5f7a 203d  ll_mean_disp_z =
+00015b50: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00015b60: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00015b70: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
+00015b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b90: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00015ba0: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
+00015bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015bc0: 2e61 6c6c 5f76 6172 5f64 6973 705f 7920  .all_var_disp_y 
+00015bd0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00015be0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00015bf0: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
+00015c00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015c10: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00015c20: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
+00015c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015c40: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
+00015c50: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
+00015c60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00015c70: 6c6c 5f76 6172 5f72 6164 6975 7320 3d20  ll_var_radius = 
+00015c80: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00015c90: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00015ca0: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
+00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cc0: 7365 6c66 2e61 6c6c 5f76 6172 5f73 7065  self.all_var_spe
+00015cd0: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
+00015ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015cf0: 616c 6c5f 6d65 616e 5f61 6363 203d 205b  all_mean_acc = [
+00015d00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015d10: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00015d20: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
+00015d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015d40: 2e61 6c6c 5f6d 6561 6e5f 6469 7265 6374  .all_mean_direct
+00015d50: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00015d60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015d70: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00015d80: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00015d90: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
+00015da0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015db0: 616c 6c5f 6d65 616e 5f64 6973 7461 6e63  all_mean_distanc
+00015dc0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
+00015dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015de0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
+00015df0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00015e00: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
+00015e10: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015e20: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00015e30: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
+00015e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015e50: 6e6f 6e5f 6d69 746f 7469 635f 636c 7573  non_mitotic_clus
+00015e60: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
+00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e80: 7365 6c66 2e61 6c6c 5f63 6c75 7374 6572  self.all_cluster
+00015e90: 5f63 6c61 7373 203d 205b 5d0d 0a0d 0a20  _class = [].... 
+00015ea0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00015eb0: 6c6c 5f73 706f 7473 5f74 7261 636b 7320  ll_spots_tracks 
+00015ec0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00015ed0: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+00015ee0: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
+00015ef0: 706f 745f 7072 6f70 6572 7469 6573 2e69  pot_properties.i
+00015f00: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+00015f10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00015f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015f30: 2020 2020 2020 2061 6c6c 5f73 706f 7473         all_spots
+00015f40: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+00015f50: 706f 745f 7072 6f70 6572 7469 6573 5b6b  pot_properties[k
+00015f60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015f70: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00015f80: 2e74 7261 636b 6964 5f6b 6579 2069 6e20  .trackid_key in 
+00015f90: 616c 6c5f 7370 6f74 733a 0d0a 2020 2020  all_spots:..    
+00015fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fb0: 2020 2020 2020 616c 6c5f 7370 6f74 735f        all_spots_
+00015fc0: 7472 6163 6b73 5b6b 5d20 3d20 616c 6c5f  tracks[k] = all_
+00015fd0: 7370 6f74 730d 0a20 2020 2020 2020 2020  spots..         
+00015fe0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00015ff0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016000: 2020 2020 2020 2020 2020 2020 2066 7574               fut
+00016010: 7572 6573 203d 205b 5d0d 0a20 2020 2020  ures = []..     
+00016020: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00016030: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+00016040: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
+00016050: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
+00016060: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
+00016070: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
+00016080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016090: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000160a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000160b0: 7220 6920 696e 2074 7164 6d28 7261 6e67  r i in tqdm(rang
+000160c0: 6528 7374 6172 7474 696d 652c 2065 6e64  e(starttime, end
+000160d0: 7469 6d65 292c 2074 6f74 616c 3d65 6e64  time), total=end
+000160e0: 7469 6d65 202d 2073 7461 7274 7469 6d65  time - starttime
+000160f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016100: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016120: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
+00016130: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
+00016140: 6974 2873 656c 662e 5f63 6f6d 7075 7465  it(self._compute
+00016150: 5f74 656d 706f 7261 6c2c 2069 2c20 616c  _temporal, i, al
+00016160: 6c5f 7370 6f74 735f 7472 6163 6b73 2929  l_spots_tracks))
+00016170: 0d0a 200d 0a20 2020 2020 2020 2020 2020  .. ..           
+00016180: 2020 2020 2020 2020 205b 722e 7265 7375           [r.resu
+00016190: 6c74 2829 2066 6f72 2072 2069 6e20 636f  lt() for r in co
+000161a0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+000161b0: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+000161c0: 7475 7265 7329 5d0d 0a0d 0a0d 0a20 2020  tures)]......   
+000161d0: 2064 6566 205f 636f 6d70 7574 655f 7465   def _compute_te
+000161e0: 6d70 6f72 616c 2873 656c 662c 2069 2c20  mporal(self, i, 
+000161f0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016200: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
+00016210: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00016220: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016230: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
+00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016250: 206d 6974 6f74 6963 5f64 6973 705f 7920   mitotic_disp_y 
+00016260: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016270: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016280: 635f 6469 7370 5f78 203d 205b 5d0d 0a20  c_disp_x = [].. 
+00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162a0: 2020 206d 6974 6f74 6963 5f72 6164 6975     mitotic_radiu
+000162b0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+000162c0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000162d0: 7469 635f 7370 6565 6420 3d20 5b5d 0d0a  tic_speed = []..
+000162e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162f0: 2020 2020 6d69 746f 7469 635f 6163 6320      mitotic_acc 
+00016300: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016310: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016320: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00016330: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
+00016340: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016350: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
+00016360: 6c61 7373 203d 205b 5d0d 0a20 2020 2020  lass = []..     
+00016370: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00016380: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00016390: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+000163a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000163b0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+000163c0: 635f 6469 7370 5f7a 203d 205b 5d0d 0a20  c_disp_z = [].. 
+000163d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163e0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+000163f0: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
+00016400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016410: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00016420: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00016430: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016440: 5f6d 6974 6f74 6963 5f72 6164 6975 7320  _mitotic_radius 
+00016450: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016460: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016470: 746f 7469 635f 7370 6565 6420 3d20 5b5d  totic_speed = []
+00016480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016490: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+000164a0: 635f 6163 6320 3d20 5b5d 0d0a 2020 2020  c_acc = []..    
+000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164c0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
+000164d0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+000164e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000164f0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00016500: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
+00016510: 7373 203d 205b 5d0d 0a20 2020 2020 2020  ss = []..       
+00016520: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016530: 5f6d 6974 6f74 6963 5f64 6973 7461 6e63  _mitotic_distanc
+00016540: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
+00016550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00016560: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00016570: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
-00016580: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016590: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-000165a0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-000165b0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-000165c0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-000165d0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-000165e0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-000165f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016600: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016610: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00016620: 6e20 7471 646d 2872 616e 6765 2873 7461  n tqdm(range(sta
-00016630: 7274 7469 6d65 2c20 656e 6474 696d 6529  rttime, endtime)
-00016640: 2c20 746f 7461 6c3d 656e 6474 696d 6520  , total=endtime 
-00016650: 2d20 7374 6172 7474 696d 6529 3a0d 0a20  - starttime):.. 
-00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016670: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00016680: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00016690: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-000166a0: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-000166b0: 6c66 2e5f 636f 6d70 7574 655f 7465 6d70  lf._compute_temp
-000166c0: 6f72 616c 2c20 692c 2061 6c6c 5f73 706f  oral, i, all_spo
-000166d0: 7473 5f74 7261 636b 7329 290d 0a20 0d0a  ts_tracks)).. ..
-000166e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166f0: 2020 2020 5b72 2e72 6573 756c 7428 2920      [r.result() 
-00016700: 666f 7220 7220 696e 2063 6f6e 6375 7272  for r in concurr
-00016710: 656e 742e 6675 7475 7265 732e 6173 5f63  ent.futures.as_c
-00016720: 6f6d 706c 6574 6564 2866 7574 7572 6573  ompleted(futures
-00016730: 295d 0d0a 0d0a 0d0a 2020 2020 6465 6620  )]......    def 
-00016740: 5f63 6f6d 7075 7465 5f74 656d 706f 7261  _compute_tempora
-00016750: 6c28 7365 6c66 2c20 692c 2061 6c6c 5f73  l(self, i, all_s
-00016760: 706f 7473 5f74 7261 636b 7329 3a20 2020  pots_tracks):   
-00016770: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00016780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016790: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-000167a0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-000167b0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000167c0: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-000167d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000167e0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-000167f0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00016800: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016810: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
-00016820: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016830: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
-00016840: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00016850: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00016860: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-00016870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016880: 2020 2020 206d 6974 6f74 6963 5f64 6972       mitotic_dir
-00016890: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000168a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000168b0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000168c0: 635f 636c 7573 7465 725f 636c 6173 7320  c_cluster_class 
-000168d0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000168e0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000168f0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00016900: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-00016910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016920: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00016930: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00016940: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016950: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00016960: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016970: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016980: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-00016990: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000169a0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000169b0: 7469 635f 7261 6469 7573 203d 205b 5d0d  tic_radius = [].
-000169c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169d0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000169e0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+00016570: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00016580: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
+00016590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165a0: 2061 6c6c 5f64 6973 705f 7920 3d20 5b5d   all_disp_y = []
+000165b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000165c0: 2020 2020 2020 616c 6c5f 6469 7370 5f78        all_disp_x
+000165d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000165e0: 2020 2020 2020 2020 2020 2061 6c6c 5f72             all_r
+000165f0: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
+00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016610: 616c 6c5f 7370 6565 6420 3d20 5b5d 0d0a  all_speed = []..
+00016620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016630: 2020 2020 616c 6c5f 6163 6320 3d20 5b5d      all_acc = []
+00016640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016650: 2020 2020 2020 616c 6c5f 6469 7265 6374        all_direct
+00016660: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00016670: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016680: 2020 2020 2020 2061 6c6c 5f63 6c75 7374         all_clust
+00016690: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
+000166a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166b0: 2020 2061 6c6c 5f64 6973 7461 6e63 655f     all_distance_
+000166c0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+000166d0: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
+000166e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000166f0: 286b 2c76 2920 696e 2061 6c6c 5f73 706f  (k,v) in all_spo
+00016700: 7473 5f74 7261 636b 732e 6974 656d 7328  ts_tracks.items(
+00016710: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016740: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00016750: 7272 656e 745f 7469 6d65 203d 2061 6c6c  rrent_time = all
+00016760: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016770: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
+00016780: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+00016790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167a0: 6d69 746f 7469 6320 3d20 616c 6c5f 7370  mitotic = all_sp
+000167b0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000167c0: 6c66 2e64 6976 6964 696e 675f 6b65 795d  lf.dividing_key]
+000167d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000167e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016800: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
+00016810: 3d3d 2069 6e74 2863 7572 7265 6e74 5f74  == int(current_t
+00016820: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
+00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016840: 2020 2020 2020 2020 2069 6620 6d69 746f           if mito
+00016850: 7469 633a 0d0a 2020 2020 2020 2020 2020  tic:..          
+00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016870: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016880: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
+00016890: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+000168a0: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
+000168b0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+000168c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168e0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+000168f0: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
+00016900: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00016910: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016940: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016950: 6469 7370 5f78 2e61 7070 656e 6428 616c  disp_x.append(al
+00016960: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00016970: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00016980: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00016990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169a0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+000169b0: 6f74 6963 5f72 6164 6975 732e 6170 7065  otic_radius.appe
+000169c0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+000169d0: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
+000169e0: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
 000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
-00016a10: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016a20: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016a30: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00016a40: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a10: 2020 6d69 746f 7469 635f 7370 6565 642e    mitotic_speed.
+00016a20: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016a30: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016a40: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
 00016a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a60: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00016a70: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-00016a80: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016a90: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00016aa0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-00016ab0: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a70: 2020 2020 206d 6974 6f74 6963 5f61 6363       mitotic_acc
+00016a80: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00016a90: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00016aa0: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
+00016ab0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ad0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016ae0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00016af0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-00016b00: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016b10: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
-00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b30: 2061 6c6c 5f64 6973 705f 7820 3d20 5b5d   all_disp_x = []
-00016b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016b50: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
-00016b60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016b70: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
-00016b80: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00016b90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016ba0: 6c6c 5f61 6363 203d 205b 5d0d 0a20 2020  ll_acc = []..   
+00016ad0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00016ae0: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
+00016af0: 5f63 6861 6e67 652e 6170 7065 6e64 2861  _change.append(a
+00016b00: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00016b10: 6b5d 5b73 656c 662e 6d6f 7469 6f6e 5f61  k][self.motion_a
+00016b20: 6e67 6c65 5f6b 6579 5d29 0d0a 2020 2020  ngle_key])..    
+00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b50: 2020 2020 6d69 746f 7469 635f 6469 7374      mitotic_dist
+00016b60: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00016b70: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00016b80: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
+00016b90: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00016ba0: 6b5f 6b65 795d 290d 0a20 2020 2020 2020  k_key])..       
 00016bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bc0: 2061 6c6c 5f64 6972 6563 7469 6f6e 616c   all_directional
-00016bd0: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
-00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bf0: 2020 616c 6c5f 636c 7573 7465 725f 636c    all_cluster_cl
-00016c00: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016c10: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00016c20: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-00016c30: 6d61 736b 203d 205b 5d0d 0a0d 0a0d 0a0d  mask = [].......
-00016c40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016c50: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-00016c60: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
-00016c70: 6163 6b73 2e69 7465 6d73 2829 3a0d 0a20  acks.items():.. 
-00016c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c90: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00016ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cb0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00016cc0: 5f74 696d 6520 3d20 616c 6c5f 7370 6f74  _time = all_spot
-00016cd0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00016ce0: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d00: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016d10: 6963 203d 2061 6c6c 5f73 706f 7473 5f74  ic = all_spots_t
-00016d20: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00016d30: 7669 6469 6e67 5f6b 6579 5d0d 0a20 2020  viding_key]..   
-00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d70: 2020 2020 2020 6966 2069 203d 3d20 696e        if i == in
-00016d80: 7428 6375 7272 656e 745f 7469 6d65 293a  t(current_time):
-00016d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bd0: 2069 6620 7365 6c66 2e63 6c75 7374 6572   if self.cluster
+00016be0: 636c 6173 735f 6b65 7920 696e 2061 6c6c  class_key in all
+00016bf0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016c00: 2e6b 6579 7328 2920 3a0d 0a20 2020 2020  .keys() :..     
+00016c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c30: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00016c40: 635f 636c 7573 7465 725f 636c 6173 732e  c_cluster_class.
+00016c50: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00016c60: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00016c70: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
+00016c80: 5d29 0d0a 0d0a 0d0a 2020 2020 2020 2020  ])......        
+00016c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ca0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00016cb0: 206d 6974 6f74 6963 3a0d 0a20 2020 2020   mitotic:..     
+00016cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ce0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00016cf0: 6973 705f 7a2e 6170 7065 6e64 2861 6c6c  isp_z.append(all
+00016d00: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00016d10: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
+00016d20: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d40: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00016d50: 6d69 746f 7469 635f 6469 7370 5f79 2e61  mitotic_disp_y.a
+00016d60: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00016d70: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
+00016d80: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00016d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016db0: 2020 2020 6966 206d 6974 6f74 6963 3a0d      if mitotic:.
-00016dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016de0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016df0: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
-00016e00: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00016e10: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
-00016e20: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00016e50: 746f 7469 635f 6469 7370 5f79 2e61 7070  totic_disp_y.app
-00016e60: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00016e70: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
-00016e80: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016eb0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00016ec0: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
-00016ed0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00016ee0: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f10: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00016f20: 7261 6469 7573 2e61 7070 656e 6428 616c  radius.append(al
-00016f30: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016f40: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
-00016f50: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f70: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016f80: 6f74 6963 5f73 7065 6564 2e61 7070 656e  otic_speed.appen
-00016f90: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00016fa0: 6b73 5b6b 5d5b 7365 6c66 2e73 7065 6564  ks[k][self.speed
-00016fb0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00016db0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016dc0: 5f64 6973 705f 782e 6170 7065 6e64 2861  _disp_x.append(a
+00016dd0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00016de0: 6b5d 5b73 656c 662e 7870 6f73 6964 5f6b  k][self.xposid_k
+00016df0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00016e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e10: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016e20: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+00016e30: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00016e40: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00016e50: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
+00016e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e80: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016e90: 6963 5f73 7065 6564 2e61 7070 656e 6428  ic_speed.append(
+00016ea0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016eb0: 5b6b 5d5b 7365 6c66 2e73 7065 6564 5f6b  [k][self.speed_k
+00016ec0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ee0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016ef0: 6e5f 6d69 746f 7469 635f 6163 632e 6170  n_mitotic_acc.ap
+00016f00: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00016f10: 7261 636b 735b 6b5d 5b73 656c 662e 6163  racks[k][self.ac
+00016f20: 6365 6c65 7261 7469 6f6e 5f6b 6579 5d29  celeration_key])
+00016f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f50: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016f60: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00016f70: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00016f80: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00016f90: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
+00016fa0: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
+00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fe0: 6d69 746f 7469 635f 6163 632e 6170 7065  mitotic_acc.appe
-00016ff0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017000: 636b 735b 6b5d 5b73 656c 662e 6163 6365  cks[k][self.acce
-00017010: 6c65 7261 7469 6f6e 5f6b 6579 5d29 0d0a  leration_key])..
-00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fd0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00016fe0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00016ff0: 6173 6b2e 6170 7065 6e64 2861 6c6c 5f73  ask.append(all_s
+00017000: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017010: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
+00017020: 6c5f 6d61 736b 5f6b 6579 5d29 0d0a 2020  l_mask_key])..  
 00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017050: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00017060: 6765 2e61 7070 656e 6428 616c 6c5f 7370  ge.append(all_sp
-00017070: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017080: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-00017090: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00017040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017050: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
+00017060: 7573 7465 7263 6c61 7373 5f6b 6579 2069  usterclass_key i
+00017070: 6e20 616c 6c5f 7370 6f74 735f 7472 6163  n all_spots_trac
+00017080: 6b73 5b6b 5d2e 6b65 7973 2829 203a 0d0a  ks[k].keys() :..
+00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000170c0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-000170d0: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-000170e0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000170f0: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00017100: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00017110: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000170b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000170c0: 6f6e 5f6d 6974 6f74 6963 5f63 6c75 7374  on_mitotic_clust
+000170d0: 6572 5f63 6c61 7373 2e61 7070 656e 6428  er_class.append(
+000170e0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000170f0: 5b6b 5d5b 7365 6c66 2e63 6c75 7374 6572  [k][self.cluster
+00017100: 636c 6173 735f 6b65 795d 290d 0a0d 0a20  class_key]).... 
+00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017130: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017140: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00017150: 5f6b 6579 2069 6e20 616c 6c5f 7370 6f74  _key in all_spot
-00017160: 735f 7472 6163 6b73 5b6b 5d2e 6b65 7973  s_tracks[k].keys
-00017170: 2829 203a 0d0a 2020 2020 2020 2020 2020  () :..          
-00017180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171a0: 2020 2020 206d 6974 6f74 6963 5f63 6c75       mitotic_clu
-000171b0: 7374 6572 5f63 6c61 7373 2e61 7070 656e  ster_class.appen
-000171c0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000171d0: 6b73 5b6b 5d5b 7365 6c66 2e63 6c75 7374  ks[k][self.clust
-000171e0: 6572 636c 6173 735f 6b65 795d 290d 0a0d  erclass_key])...
-000171f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017210: 2020 2020 2069 6620 6e6f 7420 6d69 746f       if not mito
-00017220: 7469 633a 0d0a 2020 2020 2020 2020 2020  tic:..          
+00017130: 2061 6c6c 5f64 6973 705f 7a2e 6170 7065   all_disp_z.appe
+00017140: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017150: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
+00017160: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017180: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017190: 6469 7370 5f79 2e61 7070 656e 6428 616c  disp_y.append(al
+000171a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000171b0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+000171c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171e0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+000171f0: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
+00017200: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017210: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+00017220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017240: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017250: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
-00017260: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017270: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017280: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
-00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172b0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000172c0: 6963 5f64 6973 705f 792e 6170 7065 6e64  ic_disp_y.append
-000172d0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000172e0: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
-000172f0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00017330: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
-00017340: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017350: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
-00017360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017390: 6f74 6963 5f72 6164 6975 732e 6170 7065  otic_radius.appe
-000173a0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000173b0: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
-000173c0: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
-000173d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 6e6f 6e5f 6d69 746f 7469 635f 7370    non_mitotic_sp
-00017400: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
-00017410: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017420: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
-00017430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017450: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00017460: 6f74 6963 5f61 6363 2e61 7070 656e 6428  otic_acc.append(
-00017470: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017480: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
-00017490: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
-000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000174d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000174e0: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
-000174f0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017500: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00017510: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00017240: 2020 616c 6c5f 7261 6469 7573 2e61 7070    all_radius.app
+00017250: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017260: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
+00017270: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017290: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000172a0: 5f73 7065 6564 2e61 7070 656e 6428 616c  _speed.append(al
+000172b0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000172c0: 5d5b 7365 6c66 2e73 7065 6564 5f6b 6579  ][self.speed_key
+000172d0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000172e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172f0: 2020 2020 2020 616c 6c5f 6163 632e 6170        all_acc.ap
+00017300: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00017310: 7261 636b 735b 6b5d 5b73 656c 662e 6163  racks[k][self.ac
+00017320: 6365 6c65 7261 7469 6f6e 5f6b 6579 5d29  celeration_key])
+00017330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017350: 2020 2020 616c 6c5f 6469 7265 6374 696f      all_directio
+00017360: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00017370: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017380: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
+00017390: 6e5f 616e 676c 655f 6b65 795d 2920 2020  n_angle_key])   
+000173a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 2020 2020 616c 6c5f 6469 7374 616e 6365      all_distance
+000173d0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+000173e0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+000173f0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+00017400: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00017410: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017430: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00017440: 6c75 7374 6572 636c 6173 735f 6b65 7920  lusterclass_key 
+00017450: 696e 2061 6c6c 5f73 706f 7473 5f74 7261  in all_spots_tra
+00017460: 636b 735b 6b5d 2e6b 6579 7328 2920 3a0d  cks[k].keys() :.
+00017470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174a0: 616c 6c5f 636c 7573 7465 725f 636c 6173  all_cluster_clas
+000174b0: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
+000174c0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+000174d0: 662e 636c 7573 7465 7263 6c61 7373 5f6b  f.clusterclass_k
+000174e0: 6579 5d29 2020 2020 0d0a 2020 2020 2020  ey])    ..      
+000174f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017510: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
 00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017540: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00017550: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00017560: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017570: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
-00017580: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00017590: 6b5f 6b65 795d 290d 0a20 2020 2020 2020  k_key])..       
-000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 2069 6620 7365 6c66 2e63 6c75 7374 6572   if self.cluster
-000175d0: 636c 6173 735f 6b65 7920 696e 2061 6c6c  class_key in all
-000175e0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-000175f0: 2e6b 6579 7328 2920 3a0d 0a20 2020 2020  .keys() :..     
-00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017620: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017630: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00017640: 6173 732e 6170 7065 6e64 2861 6c6c 5f73  ass.append(all_s
-00017650: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017660: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
-00017670: 5f6b 6579 5d29 0d0a 0d0a 2020 2020 2020  _key])....      
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000176a0: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
-000176b0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000176c0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-000176d0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017530: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
+00017540: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00017550: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
+00017560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017570: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00017580: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
+00017590: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
+000175a0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+000175b0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000175c0: 7469 635f 6469 7370 5f78 203d 206e 702e  tic_disp_x = np.
+000175d0: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
+000175e0: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
+000175f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017600: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017610: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
+00017620: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
+00017630: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
+00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00017660: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
+00017670: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
+00017680: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
+00017690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176a0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+000176b0: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
+000176c0: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
+000176d0: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
 000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00017700: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
-00017710: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017720: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
-00017730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017750: 2020 616c 6c5f 6469 7370 5f78 2e61 7070    all_disp_x.app
-00017760: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017770: 6163 6b73 5b6b 5d5b 7365 6c66 2e78 706f  acks[k][self.xpo
-00017780: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000177b0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
-000177c0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000177d0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
-000177e0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017800: 2020 2020 2020 2020 616c 6c5f 7370 6565          all_spee
-00017810: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-00017820: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017830: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017860: 2061 6c6c 5f61 6363 2e61 7070 656e 6428   all_acc.append(
-00017870: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017880: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
-00017890: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000178c0: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-000178d0: 6861 6e67 652e 6170 7065 6e64 2861 6c6c  hange.append(all
-000178e0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-000178f0: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
-00017900: 6c65 5f6b 6579 5d29 2020 200d 0a20 2020  le_key])   ..   
-00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017920: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017930: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-00017940: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
-00017950: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017960: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
-00017970: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
-00017980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179a0: 2020 6966 2073 656c 662e 636c 7573 7465    if self.cluste
-000179b0: 7263 6c61 7373 5f6b 6579 2069 6e20 616c  rclass_key in al
-000179c0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000179d0: 5d2e 6b65 7973 2829 203a 0d0a 2020 2020  ].keys() :..    
-000179e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a00: 2020 2020 2020 2020 2020 2061 6c6c 5f63             all_c
-00017a10: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
-00017a20: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017a30: 6163 6b73 5b6b 5d5b 7365 6c66 2e63 6c75  acks[k][self.clu
-00017a40: 7374 6572 636c 6173 735f 6b65 795d 2920  sterclass_key]) 
-00017a50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a80: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-00017a90: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00017aa0: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
-00017ab0: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
-00017ac0: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
-00017ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ae0: 206d 6974 6f74 6963 5f64 6973 705f 7920   mitotic_disp_y 
-00017af0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017b00: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
-00017b10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017b20: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00017b30: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
-00017b40: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
-00017b50: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
-00017b60: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017b70: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00017b80: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
-00017b90: 6666 286e 6f6e 5f6d 6974 6f74 6963 5f64  ff(non_mitotic_d
-00017ba0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00017bb0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017bc0: 5f6d 6974 6f74 6963 5f64 6973 705f 7920  _mitotic_disp_y 
-00017bd0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017be0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00017bf0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-00017c00: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017c10: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-00017c20: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
-00017c30: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00017c40: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
-00017c50: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00017c60: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
-00017c70: 702e 6469 6666 2861 6c6c 5f64 6973 705f  p.diff(all_disp_
-00017c80: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
-00017c90: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00017ca0: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
-00017cb0: 6469 6666 2861 6c6c 5f64 6973 705f 7929  diff(all_disp_y)
-00017cc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017cd0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00017ce0: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
-00017cf0: 6666 2861 6c6c 5f64 6973 705f 7829 290d  ff(all_disp_x)).
-00017d00: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d20: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d40: 2020 2073 656c 662e 7469 6d65 2e61 7070     self.time.app
-00017d50: 656e 6428 6920 2a20 7365 6c66 2e74 6361  end(i * self.tca
-00017d60: 6c69 6272 6174 696f 6e29 0d0a 0d0a 2020  libration)....  
-00017d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d80: 2020 7365 6c66 2e6d 6974 6f74 6963 5f63    self.mitotic_c
-00017d90: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
-00017da0: 656e 6428 6e70 2e61 7361 7272 6179 286d  end(np.asarray(m
-00017db0: 6974 6f74 6963 5f63 6c75 7374 6572 5f63  itotic_cluster_c
-00017dc0: 6c61 7373 2929 0d0a 2020 2020 2020 2020  lass))..        
-00017dd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017de0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f63 6c75  .non_mitotic_clu
-00017df0: 7374 6572 5f63 6c61 7373 2e61 7070 656e  ster_class.appen
-00017e00: 6428 6e70 2e61 7361 7272 6179 286e 6f6e  d(np.asarray(non
-00017e10: 5f6d 6974 6f74 6963 5f63 6c75 7374 6572  _mitotic_cluster
-00017e20: 5f63 6c61 7373 2929 0d0a 2020 2020 2020  _class))..      
-00017e30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017e40: 6c66 2e61 6c6c 5f63 6c75 7374 6572 5f63  lf.all_cluster_c
-00017e50: 6c61 7373 2e61 7070 656e 6428 6e70 2e61  lass.append(np.a
-00017e60: 7361 7272 6179 2861 6c6c 5f63 6c75 7374  sarray(all_clust
-00017e70: 6572 5f63 6c61 7373 2929 0d0a 0d0a 2020  er_class))....  
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00017ea0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
-00017eb0: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
-00017ec0: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
-00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ee0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00017ef0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-00017f00: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00017f10: 7370 5f7a 2929 0d0a 0d0a 2020 2020 2020  sp_z))....      
-00017f20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017f30: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00017f40: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-00017f50: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
-00017f60: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00017f70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017f80: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00017f90: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
-00017fa0: 6428 6d69 746f 7469 635f 6469 7370 5f79  d(mitotic_disp_y
-00017fb0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00017fc0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017fd0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00017fe0: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
-00017ff0: 6e28 6d69 746f 7469 635f 6469 7370 5f78  n(mitotic_disp_x
-00018000: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018010: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018020: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
-00018030: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00018040: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-00018050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018060: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018070: 6963 5f6d 6561 6e5f 7261 6469 7573 2e61  ic_mean_radius.a
-00018080: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018090: 746f 7469 635f 7261 6469 7573 2929 0d0a  totic_radius))..
+000176f0: 616c 6c5f 6469 7370 5f7a 203d 206e 702e  all_disp_z = np.
+00017700: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
+00017710: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+00017720: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017730: 6c5f 6469 7370 5f79 203d 206e 702e 6162  l_disp_y = np.ab
+00017740: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
+00017750: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+00017760: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017770: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
+00017780: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
+00017790: 5f78 2929 0d0a 0d0a 0d0a 2020 2020 2020  _x))......      
+000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000177d0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+000177e0: 652e 6170 7065 6e64 2869 202a 2073 656c  e.append(i * sel
+000177f0: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
+00017800: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017810: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017820: 7469 635f 636c 7573 7465 725f 636c 6173  tic_cluster_clas
+00017830: 732e 6170 7065 6e64 286e 702e 6173 6172  s.append(np.asar
+00017840: 7261 7928 6d69 746f 7469 635f 636c 7573  ray(mitotic_clus
+00017850: 7465 725f 636c 6173 7329 290d 0a20 2020  ter_class))..   
+00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017870: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00017880: 635f 636c 7573 7465 725f 636c 6173 732e  c_cluster_class.
+00017890: 6170 7065 6e64 286e 702e 6173 6172 7261  append(np.asarra
+000178a0: 7928 6e6f 6e5f 6d69 746f 7469 635f 636c  y(non_mitotic_cl
+000178b0: 7573 7465 725f 636c 6173 7329 290d 0a20  uster_class)).. 
+000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178d0: 2020 2073 656c 662e 616c 6c5f 636c 7573     self.all_clus
+000178e0: 7465 725f 636c 6173 732e 6170 7065 6e64  ter_class.append
+000178f0: 286e 702e 6173 6172 7261 7928 616c 6c5f  (np.asarray(all_
+00017900: 636c 7573 7465 725f 636c 6173 7329 290d  cluster_class)).
+00017910: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017920: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017930: 7469 635f 6d65 616e 5f64 6973 705f 7a2e  tic_mean_disp_z.
+00017940: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00017950: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
+00017960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017970: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017980: 635f 7661 725f 6469 7370 5f7a 2e61 7070  c_var_disp_z.app
+00017990: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+000179a0: 6963 5f64 6973 705f 7a29 290d 0a0d 0a20  ic_disp_z)).... 
+000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179c0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000179d0: 6d65 616e 5f64 6973 705f 792e 6170 7065  mean_disp_y.appe
+000179e0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+000179f0: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
+00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a10: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00017a20: 725f 6469 7370 5f79 2e61 7070 656e 6428  r_disp_y.append(
+00017a30: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00017a40: 6973 705f 7929 290d 0a0d 0a20 2020 2020  isp_y))....     
+00017a50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017a60: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00017a70: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00017a80: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
+00017a90: 6973 705f 7829 290d 0a20 2020 2020 2020  isp_x))..       
+00017aa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017ab0: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00017ac0: 7370 5f78 2e61 7070 656e 6428 6e70 2e73  sp_x.append(np.s
+00017ad0: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
+00017ae0: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00017af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017b00: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
+00017b10: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
+00017b20: 616e 286d 6974 6f74 6963 5f72 6164 6975  an(mitotic_radiu
+00017b30: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
+00017b40: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00017b50: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00017b60: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00017b70: 6974 6f74 6963 5f72 6164 6975 7329 290d  itotic_radius)).
+00017b80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017b90: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017ba0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
+00017bb0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00017bc0: 746f 7469 635f 7370 6565 6429 290d 0a20  totic_speed)).. 
+00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017be0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00017bf0: 7661 725f 7370 6565 642e 6170 7065 6e64  var_speed.append
+00017c00: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
+00017c10: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+00017c20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017c30: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00017c40: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
+00017c50: 6561 6e28 6d69 746f 7469 635f 6163 6329  ean(mitotic_acc)
+00017c60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017c70: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017c80: 7469 635f 7661 725f 6163 632e 6170 7065  tic_var_acc.appe
+00017c90: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00017ca0: 635f 6163 6329 290d 0a0d 0a20 2020 2020  c_acc))....     
+00017cb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017cc0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00017cd0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00017ce0: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+00017cf0: 616e 286d 6974 6f74 6963 5f64 6972 6563  an(mitotic_direc
+00017d00: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+00017d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017d20: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017d30: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
+00017d40: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00017d50: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00017d60: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00017d70: 6529 290d 0a0d 0a20 2020 2020 2020 2020  e))....         
+00017d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017d90: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00017da0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00017db0: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00017dc0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00017dd0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00017de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017df0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00017e00: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00017e10: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
+00017e20: 7464 286d 6974 6f74 6963 5f64 6973 7461  td(mitotic_dista
+00017e30: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+00017e40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017e50: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00017e60: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00017e70: 705f 7a2e 6170 7065 6e64 286e 702e 6d65  p_z.append(np.me
+00017e80: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+00017e90: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00017ea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017eb0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00017ec0: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
+00017ed0: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00017ee0: 6963 5f64 6973 705f 7a29 290d 0a0d 0a20  ic_disp_z)).... 
+00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f00: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00017f10: 7469 635f 6d65 616e 5f64 6973 705f 792e  tic_mean_disp_y.
+00017f20: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00017f30: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017f40: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00017f50: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00017f60: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00017f70: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
+00017f80: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00017f90: 6973 705f 7929 290d 0a0d 0a20 2020 2020  isp_y))....     
+00017fa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017fb0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00017fc0: 6d65 616e 5f64 6973 705f 782e 6170 7065  mean_disp_x.appe
+00017fd0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00017fe0: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00017ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018000: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018010: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
+00018020: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00018030: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00018040: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00018050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018060: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00018070: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+00018080: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018090: 6963 5f72 6164 6975 7329 290d 0a20 2020  ic_radius))..   
 000180a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180b0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000180c0: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-000180d0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-000180e0: 635f 7261 6469 7573 2929 0d0a 0d0a 2020  c_radius))....  
-000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018100: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00018110: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
-00018120: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00018130: 5f73 7065 6564 2929 0d0a 2020 2020 2020  _speed))..      
-00018140: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018150: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f73  lf.mitotic_var_s
-00018160: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
-00018170: 7464 286d 6974 6f74 6963 5f73 7065 6564  td(mitotic_speed
-00018180: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018190: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000181a0: 6974 6f74 6963 5f6d 6561 6e5f 6163 632e  itotic_mean_acc.
-000181b0: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-000181c0: 6974 6f74 6963 5f61 6363 2929 0d0a 2020  itotic_acc))..  
-000181d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181e0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-000181f0: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
-00018200: 2e73 7464 286d 6974 6f74 6963 5f61 6363  .std(mitotic_acc
-00018210: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018220: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018230: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
-00018240: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00018250: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018260: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-00018270: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-000182a0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000182b0: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
-000182c0: 6428 6d69 746f 7469 635f 6469 7265 6374  d(mitotic_direct
-000182d0: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-000182e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000182f0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018300: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
-00018310: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-00018320: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
-00018330: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00018340: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
-00018350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018360: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00018370: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00018380: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00018390: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-000183a0: 656c 6c5f 6d61 736b 2929 0d0a 0d0a 2020  ell_mask))....  
-000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183c0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000183d0: 6963 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ic_mean_disp_z.a
-000183e0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-000183f0: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
-00018400: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018410: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018420: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00018430: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
-00018440: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-00018450: 7370 5f7a 2929 0d0a 0d0a 2020 2020 2020  sp_z))....      
-00018460: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018470: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00018480: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
-00018490: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-000184a0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
-000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184c0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-000184d0: 6f74 6963 5f76 6172 5f64 6973 705f 792e  otic_var_disp_y.
-000184e0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-000184f0: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00018500: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018510: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018520: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000180b0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000180c0: 635f 7661 725f 7261 6469 7573 2e61 7070  c_var_radius.app
+000180d0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+000180e0: 6974 6f74 6963 5f72 6164 6975 7329 290d  itotic_radius)).
+000180f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018100: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018110: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
+00018120: 6564 2e61 7070 656e 6428 6e70 2e6d 6561  ed.append(np.mea
+00018130: 6e28 6e6f 6e5f 6d69 746f 7469 635f 7370  n(non_mitotic_sp
+00018140: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
+00018150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018160: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00018170: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+00018180: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+00018190: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000181b0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000181c0: 6d65 616e 5f61 6363 2e61 7070 656e 6428  mean_acc.append(
+000181d0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+000181e0: 7469 635f 6163 6329 290d 0a20 2020 2020  tic_acc))..     
+000181f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018200: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018210: 7661 725f 6163 632e 6170 7065 6e64 286e  var_acc.append(n
+00018220: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018230: 635f 6163 6329 290d 0a0d 0a20 2020 2020  c_acc))....     
+00018240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018250: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00018260: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00018270: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00018280: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+00018290: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+000182a0: 6861 6e67 6529 290d 0a20 2020 2020 2020  hange))..       
+000182b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000182c0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+000182d0: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+000182e0: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
+000182f0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00018300: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018310: 6529 2920 0d0a 0d0a 2020 2020 2020 2020  e)) ....        
+00018320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018330: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00018340: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+00018350: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
+00018360: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00018370: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018380: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
+00018390: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000183a0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+000183b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000183c0: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+000183d0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+000183e0: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
+000183f0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00018400: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018410: 6c6c 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ll_mean_disp_z.a
+00018420: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018430: 6c5f 6469 7370 5f7a 2929 0d0a 2020 2020  l_disp_z))..    
+00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018450: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00018460: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+00018470: 6428 616c 6c5f 6469 7370 5f7a 2929 0d0a  d(all_disp_z))..
+00018480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018490: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+000184a0: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
+000184b0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+000184c0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+000184d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000184e0: 2e61 6c6c 5f76 6172 5f64 6973 705f 792e  .all_var_disp_y.
+000184f0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018500: 6c5f 6469 7370 5f79 2929 0d0a 0d0a 2020  l_disp_y))....  
+00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018520: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
 00018530: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-00018540: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018550: 635f 6469 7370 5f78 2929 0d0a 2020 2020  c_disp_x))..    
-00018560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018570: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018580: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
-00018590: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-000185a0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-000185b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000185c0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000185d0: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-000185e0: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
-000185f0: 6e28 6e6f 6e5f 6d69 746f 7469 635f 7261  n(non_mitotic_ra
-00018600: 6469 7573 2929 0d0a 2020 2020 2020 2020  dius))..        
-00018610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018620: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018630: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
-00018640: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00018650: 635f 7261 6469 7573 2929 0d0a 0d0a 2020  c_radius))....  
-00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018670: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018680: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
-00018690: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-000186a0: 5f6d 6974 6f74 6963 5f73 7065 6564 2929  _mitotic_speed))
-000186b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000186c0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000186d0: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
-000186e0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-000186f0: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
-00018700: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018710: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018720: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018730: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
-00018740: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f61  an(non_mitotic_a
-00018750: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
-00018760: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018770: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
-00018780: 6363 2e61 7070 656e 6428 6e70 2e73 7464  cc.append(np.std
-00018790: 286e 6f6e 5f6d 6974 6f74 6963 5f61 6363  (non_mitotic_acc
-000187a0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000187b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000187c0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000187d0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-000187e0: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-000187f0: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018800: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018810: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018820: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018830: 5f6d 6974 6f74 6963 5f76 6172 5f64 6972  _mitotic_var_dir
-00018840: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00018850: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-00018860: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
-00018870: 696f 6e61 6c5f 6368 616e 6765 2929 200d  ional_change)) .
-00018880: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018890: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-000188a0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-000188b0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-000188c0: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
-000188d0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
-000188e0: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-000188f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018900: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018910: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-00018920: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00018930: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
-00018940: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-00018950: 6365 6c6c 5f6d 6173 6b29 290d 0a0d 0a0d  cell_mask)).....
-00018960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018970: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018980: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
-00018990: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
-000189a0: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-000189b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000189c0: 616c 6c5f 7661 725f 6469 7370 5f7a 2e61  all_var_disp_z.a
-000189d0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-000189e0: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
-000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a00: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00018a10: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-00018a20: 6d65 616e 2861 6c6c 5f64 6973 705f 7929  mean(all_disp_y)
-00018a30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018a40: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018a50: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
-00018a60: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-00018a70: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
-00018a80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018a90: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-00018aa0: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
-00018ab0: 2861 6c6c 5f64 6973 705f 7829 290d 0a20  (all_disp_x)).. 
-00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ad0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018ae0: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-00018af0: 2e73 7464 2861 6c6c 5f64 6973 705f 7829  .std(all_disp_x)
-00018b00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018b10: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018b20: 6c5f 6d65 616e 5f72 6164 6975 732e 6170  l_mean_radius.ap
-00018b30: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00018b40: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-00018b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018b60: 656c 662e 616c 6c5f 7661 725f 7261 6469  elf.all_var_radi
-00018b70: 7573 2e61 7070 656e 6428 6e70 2e73 7464  us.append(np.std
-00018b80: 2861 6c6c 5f72 6164 6975 7329 290d 0a0d  (all_radius))...
-00018b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ba0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00018bb0: 616e 5f73 7065 6564 2e61 7070 656e 6428  an_speed.append(
-00018bc0: 6e70 2e6d 6561 6e28 616c 6c5f 7370 6565  np.mean(all_spee
-00018bd0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00018be0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018bf0: 6c5f 7661 725f 7370 6565 642e 6170 7065  l_var_speed.appe
-00018c00: 6e64 286e 702e 7374 6428 616c 6c5f 7370  nd(np.std(all_sp
-00018c10: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00018c20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018c30: 662e 616c 6c5f 6d65 616e 5f61 6363 2e61  f.all_mean_acc.a
-00018c40: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-00018c50: 6c5f 6163 6329 290d 0a20 2020 2020 2020  l_acc))..       
-00018c60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018c70: 662e 616c 6c5f 7661 725f 6163 632e 6170  f.all_var_acc.ap
-00018c80: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00018c90: 6163 6329 290d 0a0d 0a0d 0a0d 0a20 2020  acc))........   
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cb0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00018cc0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018cd0: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
-00018ce0: 2861 6c6c 5f64 6972 6563 7469 6f6e 616c  (all_directional
-00018cf0: 5f63 6861 6e67 6529 290d 0a20 2020 2020  _change))..     
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018d10: 656c 662e 616c 6c5f 7661 725f 6469 7265  elf.all_var_dire
-00018d20: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00018d30: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00018d40: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018d50: 6e67 6529 290d 0a0d 0a20 2020 2020 2020  nge))....       
-00018d60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018d70: 662e 616c 6c5f 6d65 616e 5f64 6973 7461  f.all_mean_dista
-00018d80: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00018d90: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00018da0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018db0: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-00018dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018dd0: 616c 6c5f 7661 725f 6469 7374 616e 6365  all_var_distance
-00018de0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-00018df0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-00018e00: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
-00018e10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018e20: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00018e30: 0a20 2020 2020 2020 200d 0a64 6566 2062  .        ..def b
-00018e40: 6f75 6e64 6172 795f 706f 696e 7473 286d  oundary_points(m
-00018e50: 6173 6b2c 2078 6361 6c69 6272 6174 696f  ask, xcalibratio
-00018e60: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
-00018e70: 207a 6361 6c69 6272 6174 696f 6e29 3a0d   zcalibration):.
-00018e80: 0a0d 0a20 2020 206e 6469 6d20 3d20 6c65  ...    ndim = le
-00018e90: 6e28 6d61 736b 2e73 6861 7065 290d 0a20  n(mask.shape).. 
-00018ea0: 2020 2074 696d 6564 5f6d 6173 6b20 3d20     timed_mask = 
-00018eb0: 7b7d 0d0a 2020 2020 6d61 736b 203d 206d  {}..    mask = m
-00018ec0: 6173 6b20 3e20 300d 0a20 2020 206d 6173  ask > 0..    mas
-00018ed0: 6b20 3d20 6d61 736b 2e61 7374 7970 6528  k = mask.astype(
-00018ee0: 2775 696e 7438 2729 0d0a 2020 2020 2320  'uint8')..    # 
-00018ef0: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
-00018f00: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
-00018f10: 2032 3a0d 0a20 2020 2020 2020 200d 0a20   2:..        .. 
-00018f20: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
-00018f30: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
-00018f40: 7328 6d61 736b 290d 0a20 2020 2020 2020  s(mask)..       
-00018f50: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
-00018f60: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
-00018f70: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
-00018f80: 7279 2920 0d0a 2020 2020 2020 2020 696e  ry) ..        in
-00018f90: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
-00018fa0: 2862 6f75 6e64 6172 7920 3e20 3029 0d0a  (boundary > 0)..
-00018fb0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00018fc0: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-00018fd0: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-00018fe0: 6e64 6963 6573 2929 2e63 6f70 7928 290d  ndices)).copy().
-00018ff0: 0a0d 0a20 2020 2020 2020 2066 6f72 206a  ...        for j
-00019000: 2069 6e20 7261 6e67 6528 302c 206c 656e   in range(0, len
-00019010: 2872 6561 6c5f 696e 6469 6365 7329 293a  (real_indices)):
-00019020: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019030: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019040: 305d 203d 2072 6561 6c5f 696e 6469 6365  0] = real_indice
-00019050: 735b 6a5d 5b30 5d20 2a20 7963 616c 6962  s[j][0] * ycalib
-00019060: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00019070: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00019080: 5b6a 5d5b 315d 203d 2072 6561 6c5f 696e  [j][1] = real_in
-00019090: 6469 6365 735b 6a5d 5b31 5d20 2a20 7863  dices[j][1] * xc
-000190a0: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
-000190b0: 2020 2020 2020 7472 6565 203d 2073 7061        tree = spa
-000190c0: 7469 616c 2e63 4b44 5472 6565 2872 6561  tial.cKDTree(rea
-000190d0: 6c5f 696e 6469 6365 7329 0d0a 2020 2020  l_indices)..    
-000190e0: 2020 2020 2320 5468 6973 206f 626a 6563      # This objec
-000190f0: 7420 636f 6e74 6169 6e73 206c 6973 7420  t contains list 
-00019100: 6f66 2061 6c6c 2074 6865 2070 6f69 6e74  of all the point
-00019110: 7320 666f 7220 616c 6c20 7468 6520 6c61  s for all the la
-00019120: 6265 6c73 2069 6e20 7468 6520 4d61 736b  bels in the Mask
-00019130: 2069 6d61 6765 2077 6974 6820 7468 6520   image with the 
-00019140: 6c61 6265 6c20 6964 2061 6e64 2076 6f6c  label id and vol
-00019150: 756d 6520 6f66 2065 6163 6820 6c61 6265  ume of each labe
-00019160: 6c0d 0a20 2020 2020 2020 2074 696d 6564  l..        timed
-00019170: 5f6d 6173 6b5b 7374 7228 3029 5d20 3d20  _mask[str(0)] = 
-00019180: 5b74 7265 652c 2069 6e64 6963 6573 2c20  [tree, indices, 
-00019190: 7265 6769 6f6e 6365 6e74 726f 6964 5d0d  regioncentroid].
-000191a0: 0a0d 0a20 2020 2023 2054 5958 2073 6861  ...    # TYX sha
-000191b0: 7065 6420 6f62 6a65 6374 0d0a 2020 2020  ped object..    
-000191c0: 6966 206e 6469 6d20 3d3d 2033 3a0d 0a0d  if ndim == 3:...
-000191d0: 0a0d 0a20 2020 2020 2020 2066 6f72 2069  ...        for i
-000191e0: 2069 6e20 7471 646d 2872 616e 6765 2830   in tqdm(range(0
-000191f0: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
-00019200: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00019210: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00019220: 2020 2020 2020 626f 756e 6461 7279 203d        boundary =
-00019230: 2066 696e 645f 626f 756e 6461 7269 6573   find_boundaries
-00019240: 286d 6173 6b5b 692c 3a5d 290d 0a20 2020  (mask[i,:])..   
-00019250: 2020 2020 2020 2020 2020 2020 2072 6567               reg
-00019260: 696f 6e63 656e 7472 6f69 6420 3d20 2830  ioncentroid = (0
-00019270: 2c29 202b 2063 6f6d 7075 7465 5f63 656e  ,) + compute_cen
-00019280: 7472 6f69 6428 626f 756e 6461 7279 2920  troid(boundary) 
-00019290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000192a0: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-000192b0: 6865 7265 2862 6f75 6e64 6172 7920 3e20  here(boundary > 
-000192c0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-000192d0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-000192e0: 203d 206e 702e 7472 616e 7370 6f73 6528   = np.transpose(
-000192f0: 6e70 2e61 7361 7272 6179 2869 6e64 6963  np.asarray(indic
-00019300: 6573 2929 2e63 6f70 7928 290d 0a0d 0a20  es)).copy().... 
-00019310: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00019320: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-00019330: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
-00019340: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
-00019350: 2020 2020 2020 2020 2020 2020 7265 616c              real
-00019360: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
-00019370: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019380: 5b30 5d20 2a20 7963 616c 6962 7261 7469  [0] * ycalibrati
-00019390: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000193a0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-000193b0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
-000193c0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-000193d0: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
-000193e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000193f0: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
-00019400: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
-00019410: 6469 6365 7329 0d0a 0d0a 2020 2020 2020  dices)....      
-00019420: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
-00019430: 6d61 736b 5b73 7472 2869 295d 203d 205b  mask[str(i)] = [
-00019440: 7472 6565 2c20 696e 6469 6365 732c 2072  tree, indices, r
-00019450: 6567 696f 6e63 656e 7472 6f69 645d 0d0a  egioncentroid]..
-00019460: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00019470: 2020 2320 545a 5958 2073 6861 7065 6420    # TZYX shaped 
-00019480: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
-00019490: 6469 6d20 3d3d 2034 3a0d 0a20 2020 2020  dim == 4:..     
-000194a0: 2020 2070 7269 6e74 2827 4d61 736b 7320     print('Masks 
-000194b0: 6d61 6465 2069 6e74 6f20 6120 3444 2063  made into a 4D c
-000194c0: 796c 696e 6465 722c 2075 7027 290d 0a20  ylinder, up').. 
-000194d0: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
-000194e0: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
-000194f0: 2020 2020 2020 2020 205b 6d61 736b 2e73           [mask.s
-00019500: 6861 7065 5b30 5d2c 206d 6173 6b2e 7368  hape[0], mask.sh
-00019510: 6170 655b 315d 2c20 6d61 736b 2e73 6861  ape[1], mask.sha
-00019520: 7065 5b32 5d2c 206d 6173 6b2e 7368 6170  pe[2], mask.shap
-00019530: 655b 335d 5d0d 0a20 2020 2020 2020 2029  e[3]]..        )
-00019540: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-00019550: 696e 2072 616e 6765 2830 2c20 6d61 736b  in range(0, mask
-00019560: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
-00019570: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00019580: 2020 2020 2020 2062 6f75 6e64 6172 795b         boundary[
-00019590: 692c 3a5d 203d 2066 696e 645f 626f 756e  i,:] = find_boun
-000195a0: 6461 7269 6573 286d 6173 6b5b 692c 3a5d  daries(mask[i,:]
-000195b0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-000195c0: 6567 696f 6e63 656e 7472 6f69 6420 3d20  egioncentroid = 
-000195d0: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-000195e0: 2862 6f75 6e64 6172 795b 692c 3a5d 2920  (boundary[i,:]) 
-000195f0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00019600: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
-00019610: 2862 6f75 6e64 6172 795b 692c 3a5d 203e  (boundary[i,:] >
-00019620: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
-00019630: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
-00019640: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
-00019650: 6173 6172 7261 7928 696e 6469 6365 7329  asarray(indices)
-00019660: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
-00019670: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-00019680: 2072 616e 6765 2830 2c20 6c65 6e28 7265   range(0, len(re
-00019690: 616c 5f69 6e64 6963 6573 2929 3a0d 0a0d  al_indices)):...
-000196a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000196b0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-000196c0: 735b 6a5d 5b30 5d20 3d20 7265 616c 5f69  s[j][0] = real_i
-000196d0: 6e64 6963 6573 5b6a 5d5b 305d 202a 207a  ndices[j][0] * z
-000196e0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019700: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-00019710: 5b31 5d20 3d20 7265 616c 5f69 6e64 6963  [1] = real_indic
-00019720: 6573 5b6a 5d5b 315d 202a 2079 6361 6c69  es[j][1] * ycali
-00019730: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00019740: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00019750: 6c5f 696e 6469 6365 735b 6a5d 5b32 5d20  l_indices[j][2] 
-00019760: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-00019770: 5d5b 325d 202a 2078 6361 6c69 6272 6174  ][2] * xcalibrat
-00019780: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
-00019790: 2020 2074 7265 6520 3d20 7370 6174 6961     tree = spatia
-000197a0: 6c2e 634b 4454 7265 6528 7265 616c 5f69  l.cKDTree(real_i
-000197b0: 6e64 6963 6573 290d 0a20 2020 2020 2020  ndices)..       
-000197c0: 2020 2020 2074 696d 6564 5f6d 6173 6b5b       timed_mask[
-000197d0: 7374 7228 6929 5d20 3d20 5b74 7265 652c  str(i)] = [tree,
-000197e0: 2069 6e64 6963 6573 2c20 7265 6769 6f6e   indices, region
-000197f0: 6365 6e74 726f 6964 5d0d 0a20 2020 2070  centroid]..    p
-00019800: 7269 6e74 2827 436f 6d70 7574 6564 2074  rint('Computed t
-00019810: 6865 2062 6f75 6e64 6172 7920 706f 696e  he boundary poin
-00019820: 7473 2729 0d0a 0d0a 2020 2020 7265 7475  ts')....    retu
-00019830: 726e 2074 696d 6564 5f6d 6173 6b2c 2062  rn timed_mask, b
-00019840: 6f75 6e64 6172 7920 2020 2020 2020 200d  oundary        .
-00019850: 0a0d 0a64 6566 2063 6f6d 7075 7465 5f63  ...def compute_c
-00019860: 656e 7472 6f69 6428 6269 6e61 7279 5f69  entroid(binary_i
-00019870: 6d61 6765 293a 0d0a 2020 2020 2320 456e  mage):..    # En
-00019880: 7375 7265 2062 696e 6172 7920 696d 6167  sure binary imag
-00019890: 6520 6973 2061 204e 756d 5079 2061 7272  e is a NumPy arr
-000198a0: 6179 0d0a 2020 2020 6269 6e61 7279 5f69  ay..    binary_i
-000198b0: 6d61 6765 203d 206e 702e 6172 7261 7928  mage = np.array(
-000198c0: 6269 6e61 7279 5f69 6d61 6765 290d 0a0d  binary_image)...
-000198d0: 0a20 2020 2077 6869 7465 5f70 6978 656c  .    white_pixel
-000198e0: 7320 3d20 6e70 2e77 6865 7265 2862 696e  s = np.where(bin
-000198f0: 6172 795f 696d 6167 6520 3d3d 2031 290d  ary_image == 1).
-00019900: 0a20 2020 206e 756d 5f70 6978 656c 7320  .    num_pixels 
-00019910: 3d20 6c65 6e28 7768 6974 655f 7069 7865  = len(white_pixe
-00019920: 6c73 5b30 5d29 0d0a 0d0a 2020 2020 2320  ls[0])....    # 
-00019930: 436f 6d70 7574 6520 7468 6520 6365 6e74  Compute the cent
-00019940: 726f 6964 206f 6620 7468 6520 7768 6974  roid of the whit
-00019950: 6520 7069 7865 6c73 2069 6e20 7468 6520  e pixels in the 
-00019960: 626f 756e 6461 7279 2069 6d61 6765 0d0a  boundary image..
-00019970: 2020 2020 6365 6e74 726f 6964 203d 206e      centroid = n
-00019980: 702e 7a65 726f 7328 6269 6e61 7279 5f69  p.zeros(binary_i
-00019990: 6d61 6765 2e6e 6469 6d29 0d0a 2020 2020  mage.ndim)..    
-000199a0: 666f 7220 6469 6d20 696e 2072 616e 6765  for dim in range
-000199b0: 2862 696e 6172 795f 696d 6167 652e 6e64  (binary_image.nd
-000199c0: 696d 293a 0d0a 2020 2020 2020 2020 6365  im):..        ce
-000199d0: 6e74 726f 6964 5b64 696d 5d20 3d20 7768  ntroid[dim] = wh
-000199e0: 6974 655f 7069 7865 6c73 5b64 696d 5d2e  ite_pixels[dim].
-000199f0: 7375 6d28 2920 2f20 6e75 6d5f 7069 7865  sum() / num_pixe
-00019a00: 6c73 0d0a 0d0a 2020 2020 7265 7475 726e  ls....    return
-00019a10: 2063 656e 7472 6f69 640d 0a0d 0a0d 0a0d   centroid.......
-00019a20: 0a20 0d0a 0d0a 6465 6620 6765 745f 6373  . ....def get_cs
-00019a30: 765f 6461 7461 2863 7376 293a 0d0a 0d0a  v_data(csv):....
-00019a40: 2020 2020 2020 2020 6461 7461 7365 7420          dataset 
-00019a50: 3d20 7064 2e72 6561 645f 6373 7628 0d0a  = pd.read_csv(..
-00019a60: 2020 2020 2020 2020 2020 2020 6373 762c              csv,
-00019a70: 2064 656c 696d 6974 6572 3d22 2c22 2c20   delimiter=",", 
-00019a80: 656e 636f 6469 6e67 3d22 756e 6963 6f64  encoding="unicod
-00019a90: 655f 6573 6361 7065 222c 206c 6f77 5f6d  e_escape", low_m
-00019aa0: 656d 6f72 793d 4661 6c73 650d 0a20 2020  emory=False..   
-00019ab0: 2020 2020 2029 5b33 3a5d 0d0a 2020 2020       )[3:]..    
-00019ac0: 2020 2020 6461 7461 7365 745f 696e 6465      dataset_inde
-00019ad0: 7820 3d20 6461 7461 7365 742e 696e 6465  x = dataset.inde
-00019ae0: 780d 0a20 2020 2020 2020 2072 6574 7572  x..        retur
-00019af0: 6e20 6461 7461 7365 742c 2064 6174 6173  n dataset, datas
-00019b00: 6574 5f69 6e64 6578 0d0a 2020 2020 0d0a  et_index..    ..
-00019b10: 6465 6620 6765 745f 7370 6f74 5f64 6174  def get_spot_dat
-00019b20: 6173 6574 2873 706f 745f 6461 7461 7365  aset(spot_datase
-00019b30: 742c 2074 7261 636b 5f61 6e61 6c79 7369  t, track_analysi
-00019b40: 735f 7370 6f74 5f6b 6579 732c 2078 6361  s_spot_keys, xca
-00019b50: 6c69 6272 6174 696f 6e2c 2079 6361 6c69  libration, ycali
-00019b60: 6272 6174 696f 6e2c 207a 6361 6c69 6272  bration, zcalibr
-00019b70: 6174 696f 6e2c 2041 7474 7269 6275 7465  ation, Attribute
-00019b80: 426f 786e 616d 652c 2064 6574 6563 7469  Boxname, detecti
-00019b90: 6f6e 6368 616e 6e65 6c29 3a0d 0a20 2020  onchannel):..   
-00019ba0: 2020 2020 2041 6c6c 5661 6c75 6573 203d       AllValues =
-00019bb0: 207b 7d0d 0a20 2020 2020 2020 2070 6f73   {}..        pos
-00019bc0: 6978 203d 2074 7261 636b 5f61 6e61 6c79  ix = track_analy
-00019bd0: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
-00019be0: 6f73 6978 225d 0d0a 2020 2020 2020 2020  osix"]..        
-00019bf0: 706f 7369 7920 3d20 7472 6163 6b5f 616e  posiy = track_an
-00019c00: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019c10: 5b22 706f 7369 7922 5d0d 0a20 2020 2020  ["posiy"]..     
-00019c20: 2020 2070 6f73 697a 203d 2074 7261 636b     posiz = track
-00019c30: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019c40: 6579 735b 2270 6f73 697a 225d 0d0a 2020  eys["posiz"]..  
-00019c50: 2020 2020 2020 6672 616d 6520 3d20 7472        frame = tr
-00019c60: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019c70: 745f 6b65 7973 5b22 6672 616d 6522 5d0d  t_keys["frame"].
-00019c80: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00019c90: 2020 204c 6f63 6174 696f 6e58 203d 2028     LocationX = (
-00019ca0: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-00019cb0: 6f74 5f64 6174 6173 6574 5b70 6f73 6978  ot_dataset[posix
-00019cc0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-00019cd0: 2920 2f20 7863 616c 6962 7261 7469 6f6e  ) / xcalibration
-00019ce0: 0d0a 2020 2020 2020 2020 292e 6173 7479  ..        ).asty
-00019cf0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
-00019d00: 2020 204c 6f63 6174 696f 6e59 203d 2028     LocationY = (
-00019d10: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-00019d20: 6f74 5f64 6174 6173 6574 5b70 6f73 6979  ot_dataset[posiy
-00019d30: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-00019d40: 2920 2f20 7963 616c 6962 7261 7469 6f6e  ) / ycalibration
-00019d50: 0d0a 2020 2020 2020 2020 292e 6173 7479  ..        ).asty
-00019d60: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
-00019d70: 2020 204c 6f63 6174 696f 6e5a 203d 2028     LocationZ = (
-00019d80: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-00019d90: 6f74 5f64 6174 6173 6574 5b70 6f73 697a  ot_dataset[posiz
-00019da0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-00019db0: 2920 2f20 7a63 616c 6962 7261 7469 6f6e  ) / zcalibration
-00019dc0: 0d0a 2020 2020 2020 2020 292e 6173 7479  ..        ).asty
-00019dd0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
-00019de0: 2020 204c 6f63 6174 696f 6e54 203d 2028     LocationT = (
-00019df0: 7370 6f74 5f64 6174 6173 6574 5b66 7261  spot_dataset[fra
-00019e00: 6d65 5d2e 6173 7479 7065 2822 666c 6f61  me].astype("floa
-00019e10: 7422 2929 2e61 7374 7970 6528 2269 6e74  t")).astype("int
-00019e20: 2229 0d0a 2020 2020 2020 2020 0d0a 0d0a  ")..        ....
-00019e30: 2020 2020 2020 2020 6967 6e6f 7265 5f76          ignore_v
-00019e40: 616c 7565 7320 3d20 5b74 7261 636b 5f61  alues = [track_a
-00019e50: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019e60: 735b 226d 6561 6e5f 696e 7465 6e73 6974  s["mean_intensit
-00019e70: 7922 5d2c 7472 6163 6b5f 616e 616c 7973  y"],track_analys
-00019e80: 6973 5f73 706f 745f 6b65 7973 5b22 746f  is_spot_keys["to
-00019e90: 7461 6c5f 696e 7465 6e73 6974 7922 5d5d  tal_intensity"]]
-00019ea0: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
-00019eb0: 6b2c 7629 2069 6e20 7472 6163 6b5f 616e  k,v) in track_an
-00019ec0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-00019ed0: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
-00019ee0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00019ef0: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
-00019f00: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
-00019f10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00019f20: 6b20 3d3d 2022 6d65 616e 5f69 6e74 656e  k == "mean_inten
-00019f30: 7369 7479 5f63 6832 223a 0d0a 2020 2020  sity_ch2":..    
-00019f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f50: 2020 2020 2020 2076 616c 7565 203d 2074         value = t
-00019f60: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-00019f70: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
-00019f80: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
-00019f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fa0: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-00019fb0: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
-00019fc0: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-00019fd0: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-00019fe0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00019ff0: 6620 6b20 3d3d 2022 746f 7461 6c5f 696e  f k == "total_in
-0001a000: 7465 6e73 6974 795f 6368 3222 3a0d 0a20  tensity_ch2":.. 
-0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a020: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-0001a030: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001a040: 5f73 706f 745f 6b65 7973 5b22 746f 7461  _spot_keys["tota
-0001a050: 6c5f 696e 7465 6e73 6974 7922 5d0d 0a20  l_intensity"].. 
-0001a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a070: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-0001a080: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
-0001a090: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
-0001a0a0: 7970 6528 2266 6c6f 6174 2229 2020 2020  ype("float")    
-0001a0b0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-0001a0c0: 2020 2020 2020 2069 6620 7620 6e6f 7420         if v not 
-0001a0d0: 696e 2069 676e 6f72 655f 7661 6c75 6573  in ignore_values
-0001a0e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001a0f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a110: 2020 2041 6c6c 5661 6c75 6573 5b76 5d20     AllValues[v] 
-0001a120: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
-0001a130: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001a140: 290d 0a0d 0a20 2020 2020 2020 2041 6c6c  )....        All
-0001a150: 5661 6c75 6573 5b70 6f73 6978 5d20 3d20  Values[posix] = 
-0001a160: 726f 756e 6428 4c6f 6361 7469 6f6e 582c  round(LocationX,
-0001a170: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
-0001a180: 616c 7565 735b 706f 7369 795d 203d 2072  alues[posiy] = r
-0001a190: 6f75 6e64 284c 6f63 6174 696f 6e59 2c33  ound(LocationY,3
-0001a1a0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
-0001a1b0: 6c75 6573 5b70 6f73 697a 5d20 3d20 726f  lues[posiz] = ro
-0001a1c0: 756e 6428 4c6f 6361 7469 6f6e 5a2c 3329  und(LocationZ,3)
-0001a1d0: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
-0001a1e0: 7565 735b 6672 616d 655d 203d 2072 6f75  ues[frame] = rou
-0001a1f0: 6e64 284c 6f63 6174 696f 6e54 2c33 290d  nd(LocationT,3).
-0001a200: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
-0001a210: 7465 6964 7320 3d20 5b5d 0d0a 2020 2020  teids = []..    
-0001a220: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
-0001a230: 2e61 7070 656e 6428 4174 7472 6962 7574  .append(Attribut
-0001a240: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
-0001a250: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
-0001a260: 6e61 6d65 2069 6e20 416c 6c56 616c 7565  name in AllValue
-0001a270: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-0001a280: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
-0001a290: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
-0001a2a0: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
-0001a2b0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0001a2c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001a2d0: 2072 6574 7572 6e20 4174 7472 6962 7574   return Attribut
-0001a2e0: 6569 6473 2c20 416c 6c56 616c 7565 7320  eids, AllValues 
-0001a2f0: 2020 2020 0d0a 2020 2020 0d0a 6465 6620      ..    ..def 
-0001a300: 6765 745f 7472 6163 6b5f 6461 7461 7365  get_track_datase
-0001a310: 7428 7472 6163 6b5f 6461 7461 7365 742c  t(track_dataset,
-0001a320: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a330: 7370 6f74 5f6b 6579 732c 2074 7261 636b  spot_keys, track
-0001a340: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
-0001a350: 6b65 7973 2c20 5472 6163 6b41 7474 7269  keys, TrackAttri
-0001a360: 6275 7465 426f 786e 616d 6529 3a0d 0a0d  buteBoxname):...
-0001a370: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
-0001a380: 6b56 616c 7565 7320 3d20 7b7d 0d0a 2020  kValues = {}..  
-0001a390: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-0001a3a0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a3b0: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
-0001a3c0: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
-0001a3d0: 6964 203d 2074 7261 636b 5f64 6174 6173  id = track_datas
-0001a3e0: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
-0001a3f0: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001a400: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
-0001a410: 6c6c 5472 6163 6b56 616c 7565 735b 7472  llTrackValues[tr
-0001a420: 6163 6b5f 6964 5d20 3d20 5469 640d 0a20  ack_id] = Tid.. 
-0001a430: 2020 2020 200d 0a20 2020 2020 2020 2066       ..        f
-0001a440: 6f72 2028 6b2c 2076 2920 696e 2074 7261  or (k, v) in tra
-0001a450: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
-0001a460: 6b5f 6b65 7973 2e69 7465 6d73 2829 3a0d  k_keys.items():.
-0001a470: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a480: 2020 2078 203d 2074 7261 636b 5f64 6174     x = track_dat
-0001a490: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
-0001a4a0: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001a4b0: 2020 2020 2020 2020 206d 696e 7661 6c20           minval 
-0001a4c0: 3d20 6d69 6e28 7829 0d0a 2020 2020 2020  = min(x)..      
-0001a4d0: 2020 2020 2020 2020 2020 6d61 7876 616c            maxval
-0001a4e0: 203d 206d 6178 2878 290d 0a0d 0a20 2020   = max(x)....   
-0001a4f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a500: 6d69 6e76 616c 203e 2030 2061 6e64 206d  minval > 0 and m
-0001a510: 6178 7661 6c20 3c3d 2031 3a0d 0a0d 0a20  axval <= 1:.... 
-0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a530: 2020 2078 203d 2078 202b 2031 0d0a 0d0a     x = x + 1....
-0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a550: 416c 6c54 7261 636b 5661 6c75 6573 5b6b  AllTrackValues[k
-0001a560: 5d20 3d20 726f 756e 6428 782c 2033 290d  ] = round(x, 3).
-0001a570: 0a0d 0a20 2020 2020 2020 2054 7261 636b  ...        Track
-0001a580: 4174 7472 6962 7574 6569 6473 203d 205b  Attributeids = [
-0001a590: 5d0d 0a20 2020 2020 2020 2054 7261 636b  ]..        Track
-0001a5a0: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
-0001a5b0: 656e 6428 5472 6163 6b41 7474 7269 6275  end(TrackAttribu
-0001a5c0: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
-0001a5d0: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
-0001a5e0: 656e 616d 6520 696e 2074 7261 636b 5f61  ename in track_a
-0001a5f0: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
-0001a600: 7973 2e6b 6579 7328 293a 0d0a 2020 2020  ys.keys():..    
-0001a610: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
-0001a620: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
-0001a630: 2861 7474 7269 6275 7465 6e61 6d65 2920  (attributename) 
-0001a640: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
-0001a650: 2020 2072 6574 7572 6e20 5472 6163 6b41     return TrackA
-0001a660: 7474 7269 6275 7465 6964 732c 2041 6c6c  ttributeids, All
-0001a670: 5472 6163 6b56 616c 7565 730d 0a20 2020  TrackValues..   
-0001a680: 200d 0a64 6566 2067 6574 5f65 6467 6573   ..def get_edges
-0001a690: 5f64 6174 6173 6574 2865 6467 6573 5f64  _dataset(edges_d
-0001a6a0: 6174 6173 6574 2c20 6564 6765 735f 6461  ataset, edges_da
-0001a6b0: 7461 7365 745f 696e 6465 782c 2074 7261  taset_index, tra
-0001a6c0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a6d0: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
-0001a6e0: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
-0001a6f0: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
-0001a700: 6c45 6467 6573 5661 6c75 6573 203d 207b  lEdgesValues = {
-0001a710: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
-0001a720: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
-0001a730: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001a740: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
-0001a750: 2020 2020 5469 6420 3d20 6564 6765 735f      Tid = edges_
-0001a760: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
-0001a770: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001a780: 290d 0a20 2020 2020 2020 2069 6e64 6963  )..        indic
-0001a790: 6573 203d 206e 702e 7768 6572 6528 5469  es = np.where(Ti
-0001a7a0: 6420 3d3d 2030 290d 0a20 2020 2020 2020  d == 0)..       
-0001a7b0: 206d 6178 7472 6163 6b5f 6964 203d 206d   maxtrack_id = m
-0001a7c0: 6178 2854 6964 290d 0a20 2020 2020 2020  ax(Tid)..       
-0001a7d0: 2063 6f6e 6469 7469 6f6e 5f69 6e64 6963   condition_indic
-0001a7e0: 6573 203d 2065 6467 6573 5f64 6174 6173  es = edges_datas
-0001a7f0: 6574 5f69 6e64 6578 5b69 6e64 6963 6573  et_index[indices
-0001a800: 5d0d 0a20 2020 2020 2020 2054 6964 5b63  ]..        Tid[c
-0001a810: 6f6e 6469 7469 6f6e 5f69 6e64 6963 6573  ondition_indices
-0001a820: 5d20 3d20 6d61 7874 7261 636b 5f69 6420  ] = maxtrack_id 
-0001a830: 2b20 310d 0a20 2020 2020 2020 2041 6c6c  + 1..        All
-0001a840: 4564 6765 7356 616c 7565 735b 7472 6163  EdgesValues[trac
-0001a850: 6b5f 6964 5d20 3d20 5469 640d 0a0d 0a20  k_id] = Tid.... 
-0001a860: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-0001a870: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
-0001a880: 6467 6573 5f6b 6579 732e 7661 6c75 6573  dges_keys.values
-0001a890: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
-0001a8a0: 2020 2069 6620 6b20 213d 2074 7261 636b     if k != track
-0001a8b0: 5f69 643a 0d0a 2020 2020 2020 2020 2020  _id:..          
-0001a8c0: 2020 2020 2020 7820 3d20 6564 6765 735f        x = edges_
-0001a8d0: 6461 7461 7365 745b 6b5d 2e61 7374 7970  dataset[k].astyp
-0001a8e0: 6528 2266 6c6f 6174 2229 0d0a 0d0a 2020  e("float")....  
-0001a8f0: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001a900: 6c45 6467 6573 5661 6c75 6573 5b6b 5d20  lEdgesValues[k] 
-0001a910: 3d20 7820 2020 0d0a 2020 2020 2020 2020  = x   ..        
-0001a920: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
-0001a930: 6e20 416c 6c45 6467 6573 5661 6c75 6573  n AllEdgesValues
-0001a940: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
-0001a950: 2020 0d0a 2020 2020 0d0a 6465 6620 7363    ..    ..def sc
-0001a960: 616c 655f 7661 6c75 6528 782c 2073 6361  ale_value(x, sca
-0001a970: 6c65 203d 2032 3535 202a 2032 3535 293a  le = 255 * 255):
-0001a980: 0d0a 0d0a 0d0a 2020 2020 2072 6574 7572  ......     retur
-0001a990: 6e20 7820 2a20 7363 616c 6520 2020 0d0a  n x * scale   ..
-0001a9a0: 2020 2020 0d0a 0d0a 0d0a 6465 6620 7072      ......def pr
-0001a9b0: 6f62 5f73 6967 6d6f 6964 2878 293a 0d0a  ob_sigmoid(x):..
-0001a9c0: 2020 2020 7265 7475 726e 2031 202d 206d      return 1 - m
-0001a9d0: 6174 682e 6578 7028 2d78 290d 0a0d 0a0d  ath.exp(-x).....
-0001a9e0: 0a64 6566 2061 6e67 756c 6172 5f63 6861  .def angular_cha
-0001a9f0: 6e67 6528 7665 635f 302c 2076 6563 5f31  nge(vec_0, vec_1
-0001aa00: 293a 0d0a 2020 2020 2020 2020 0d0a 2020  ):..        ..  
-0001aa10: 2020 2020 2020 7665 635f 3020 3d20 7665        vec_0 = ve
-0001aa20: 635f 3020 2f20 6e70 2e6c 696e 616c 672e  c_0 / np.linalg.
-0001aa30: 6e6f 726d 2876 6563 5f30 290d 0a20 2020  norm(vec_0)..   
-0001aa40: 2020 2020 2076 6563 5f31 203d 2076 6563       vec_1 = vec
-0001aa50: 5f31 202f 206e 702e 6c69 6e61 6c67 2e6e  _1 / np.linalg.n
-0001aa60: 6f72 6d28 7665 635f 3129 0d0a 2020 2020  orm(vec_1)..    
-0001aa70: 2020 2020 616e 676c 6520 3d20 6e70 2e61      angle = np.a
-0001aa80: 7263 636f 7328 6e70 2e63 6c69 7028 6e70  rccos(np.clip(np
-0001aa90: 2e64 6f74 2876 6563 5f30 2c20 7665 635f  .dot(vec_0, vec_
-0001aaa0: 3129 2c20 2d31 2e30 2c20 312e 3029 290d  1), -1.0, 1.0)).
-0001aab0: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
-0001aac0: 2061 6e67 6c65 202a 2031 3830 202f 206e   angle * 180 / n
-0001aad0: 702e 7069 0d0a 2020 2020 2020 2020 7265  p.pi..        re
-0001aae0: 7475 726e 2061 6e67 6c65 0d0a 2020 2020  turn angle..    
-0001aaf0: 200d 0a0d 0a64 6566 2065 7661 6c5f 626f   ....def eval_bo
-0001ab00: 6f6c 2876 616c 7565 293a 0d0a 2020 2020  ol(value):..    
-0001ab10: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001ab20: 2020 2020 2020 2020 6966 2076 616c 7565          if value
-0001ab30: 2020 3d3d 2027 5472 7565 273a 200d 0a20    == 'True': .. 
-0001ab40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001ab50: 6976 5f6b 6579 203d 2054 7275 650d 0a20  iv_key = True.. 
-0001ab60: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0001ab70: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0001ab80: 765f 6b65 7920 3d20 4661 6c73 6520 0d0a  v_key = False ..
-0001ab90: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001aba0: 2064 6976 5f6b 6579 2020 2020 2020 2020   div_key        
-0001abb0: 2020 2020 2020 2020 0d0a 0d0a 6465 6620          ....def 
-0001abc0: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
-0001abd0: 5f6d 6173 6b28 6d61 736b 2c69 6d61 6765  _mask(mask,image
-0001abe0: 293a 0d0a 2020 2020 2020 200d 0a20 2020  ):..       ..   
-0001abf0: 2020 2020 2069 6620 6c65 6e28 6d61 736b       if len(mask
-0001ac00: 2e73 6861 7065 2920 3c20 6c65 6e28 696d  .shape) < len(im
-0001ac10: 6167 652e 7368 6170 6529 3a0d 0a20 2020  age.shape):..   
-0001ac20: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001ac30: 6d61 736b 203d 206e 702e 7a65 726f 7328  mask = np.zeros(
-0001ac40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ac50: 2020 2020 2020 2020 2020 2020 2020 5b0d                [.
-0001ac60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac80: 2069 6d61 6765 2e73 6861 7065 5b30 5d2c   image.shape[0],
-0001ac90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001acb0: 2020 696d 6167 652e 7368 6170 655b 315d    image.shape[1]
-0001acc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ace0: 2020 2069 6d61 6765 2e73 6861 7065 5b32     image.shape[2
-0001acf0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad10: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
-0001ad20: 335d 2c0d 0a20 2020 2020 2020 2020 2020  3],..           
-0001ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad40: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
-0001ad50: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0001ad60: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0001ad70: 2069 6e20 7261 6e67 6528 302c 2075 7064   in range(0, upd
-0001ad80: 6174 655f 6d61 736b 2e73 6861 7065 5b30  ate_mask.shape[0
-0001ad90: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-0001ada0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-0001adb0: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
-0001adc0: 736b 2e73 6861 7065 5b31 5d29 3a0d 0a0d  sk.shape[1]):...
-0001add0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ade0: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
-0001adf0: 5b69 2c20 6a2c 203a 2c20 3a5d 203d 206d  [i, j, :, :] = m
-0001ae00: 6173 6b5b 692c 203a 2c20 3a5d 0d0a 2020  ask[i, :, :]..  
-0001ae10: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-0001ae20: 2020 2020 2020 2020 2020 2020 2075 7064               upd
-0001ae30: 6174 655f 6d61 736b 203d 206d 6173 6b0d  ate_mask = mask.
-0001ae40: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0001ae50: 6e20 7570 6461 7465 5f6d 6173 6b20 2020  n update_mask   
-0001ae60: 2020 2020 200d 0a20 2020 2020 2020 0d0a       ..       ..
+00018540: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f78  .mean(all_disp_x
+00018550: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018560: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018570: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+00018580: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+00018590: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+000185a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000185b0: 6c66 2e61 6c6c 5f6d 6561 6e5f 7261 6469  lf.all_mean_radi
+000185c0: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
+000185d0: 6e28 616c 6c5f 7261 6469 7573 2929 0d0a  n(all_radius))..
+000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185f0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00018600: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+00018610: 702e 7374 6428 616c 6c5f 7261 6469 7573  p.std(all_radius
+00018620: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018630: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018640: 6c6c 5f6d 6561 6e5f 7370 6565 642e 6170  ll_mean_speed.ap
+00018650: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00018660: 5f73 7065 6564 2929 0d0a 2020 2020 2020  _speed))..      
+00018670: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018680: 6c66 2e61 6c6c 5f76 6172 5f73 7065 6564  lf.all_var_speed
+00018690: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+000186a0: 6c6c 5f73 7065 6564 2929 0d0a 0d0a 2020  ll_speed))....  
+000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186c0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+000186d0: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
+000186e0: 616e 2861 6c6c 5f61 6363 2929 0d0a 2020  an(all_acc))..  
+000186f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018700: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f61    self.all_var_a
+00018710: 6363 2e61 7070 656e 6428 6e70 2e73 7464  cc.append(np.std
+00018720: 2861 6c6c 5f61 6363 2929 0d0a 0d0a 0d0a  (all_acc))......
+00018730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018740: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018750: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+00018760: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+00018770: 2e6d 6561 6e28 616c 6c5f 6469 7265 6374  .mean(all_direct
+00018780: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187a0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000187b0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000187c0: 6e67 652e 6170 7065 6e64 286e 702e 7374  nge.append(np.st
+000187d0: 6428 616c 6c5f 6469 7265 6374 696f 6e61  d(all_directiona
+000187e0: 6c5f 6368 616e 6765 2929 0d0a 0d0a 2020  l_change))....  
+000187f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018800: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00018810: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018820: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
+00018830: 6e28 616c 6c5f 6469 7374 616e 6365 5f63  n(all_distance_c
+00018840: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
+00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018860: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00018870: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00018880: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018890: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
+000188a0: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188c0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+000188d0: 6465 6620 626f 756e 6461 7279 5f70 6f69  def boundary_poi
+000188e0: 6e74 7328 6d61 736b 2c20 7863 616c 6962  nts(mask, xcalib
+000188f0: 7261 7469 6f6e 2c20 7963 616c 6962 7261  ration, ycalibra
+00018900: 7469 6f6e 2c20 7a63 616c 6962 7261 7469  tion, zcalibrati
+00018910: 6f6e 293a 0d0a 0d0a 2020 2020 6e64 696d  on):....    ndim
+00018920: 203d 206c 656e 286d 6173 6b2e 7368 6170   = len(mask.shap
+00018930: 6529 0d0a 2020 2020 7469 6d65 645f 6d61  e)..    timed_ma
+00018940: 736b 203d 207b 7d0d 0a20 2020 206d 6173  sk = {}..    mas
+00018950: 6b20 3d20 6d61 736b 203e 2030 0d0a 2020  k = mask > 0..  
+00018960: 2020 6d61 736b 203d 206d 6173 6b2e 6173    mask = mask.as
+00018970: 7479 7065 2827 7569 6e74 3827 290d 0a20  type('uint8').. 
+00018980: 2020 2023 2059 5820 7368 6170 6564 206f     # YX shaped o
+00018990: 626a 6563 740d 0a20 2020 2069 6620 6e64  bject..    if nd
+000189a0: 696d 203d 3d20 323a 0d0a 2020 2020 2020  im == 2:..      
+000189b0: 2020 0d0a 2020 2020 2020 2020 626f 756e    ..        boun
+000189c0: 6461 7279 203d 2066 696e 645f 626f 756e  dary = find_boun
+000189d0: 6461 7269 6573 286d 6173 6b29 0d0a 2020  daries(mask)..  
+000189e0: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
+000189f0: 726f 6964 203d 2028 302c 2920 2b20 636f  roid = (0,) + co
+00018a00: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
+00018a10: 6f75 6e64 6172 7929 200d 0a20 2020 2020  oundary) ..     
+00018a20: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+00018a30: 7768 6572 6528 626f 756e 6461 7279 203e  where(boundary >
+00018a40: 2030 290d 0a20 2020 2020 2020 2072 6561   0)..        rea
+00018a50: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
+00018a60: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
+00018a70: 7261 7928 696e 6469 6365 7329 292e 636f  ray(indices)).co
+00018a80: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
+00018a90: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+00018aa0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
+00018ab0: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
+00018ac0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00018ad0: 735b 6a5d 5b30 5d20 3d20 7265 616c 5f69  s[j][0] = real_i
+00018ae0: 6e64 6963 6573 5b6a 5d5b 305d 202a 2079  ndices[j][0] * y
+00018af0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+00018b00: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00018b10: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
+00018b20: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+00018b30: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
+00018b40: 0a0d 0a20 2020 2020 2020 2074 7265 6520  ...        tree 
+00018b50: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
+00018b60: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
+00018b70: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+00018b80: 6f62 6a65 6374 2063 6f6e 7461 696e 7320  object contains 
+00018b90: 6c69 7374 206f 6620 616c 6c20 7468 6520  list of all the 
+00018ba0: 706f 696e 7473 2066 6f72 2061 6c6c 2074  points for all t
+00018bb0: 6865 206c 6162 656c 7320 696e 2074 6865  he labels in the
+00018bc0: 204d 6173 6b20 696d 6167 6520 7769 7468   Mask image with
+00018bd0: 2074 6865 206c 6162 656c 2069 6420 616e   the label id an
+00018be0: 6420 766f 6c75 6d65 206f 6620 6561 6368  d volume of each
+00018bf0: 206c 6162 656c 0d0a 2020 2020 2020 2020   label..        
+00018c00: 7469 6d65 645f 6d61 736b 5b73 7472 2830  timed_mask[str(0
+00018c10: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
+00018c20: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
+00018c30: 6f69 645d 0d0a 0d0a 2020 2020 2320 5459  oid]....    # TY
+00018c40: 5820 7368 6170 6564 206f 626a 6563 740d  X shaped object.
+00018c50: 0a20 2020 2069 6620 6e64 696d 203d 3d20  .    if ndim == 
+00018c60: 333a 0d0a 0d0a 0d0a 2020 2020 2020 2020  3:......        
+00018c70: 666f 7220 6920 696e 2074 7164 6d28 7261  for i in tqdm(ra
+00018c80: 6e67 6528 302c 206d 6173 6b2e 7368 6170  nge(0, mask.shap
+00018c90: 655b 305d 2929 3a0d 0a20 2020 2020 2020  e[0])):..       
+00018ca0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00018cb0: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
+00018cc0: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
+00018cd0: 6172 6965 7328 6d61 736b 5b69 2c3a 5d29  aries(mask[i,:])
+00018ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018cf0: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
+00018d00: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
+00018d10: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
+00018d20: 6172 7929 200d 0a20 2020 2020 2020 2020  ary) ..         
+00018d30: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+00018d40: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
+00018d50: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
+00018d60: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00018d70: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
+00018d80: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
+00018d90: 696e 6469 6365 7329 292e 636f 7079 2829  indices)).copy()
+00018da0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018db0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+00018dc0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+00018dd0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00018e00: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+00018e10: 6573 5b6a 5d5b 305d 202a 2079 6361 6c69  es[j][0] * ycali
+00018e20: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00018e30: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+00018e40: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00018e50: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00018e60: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
+00018e70: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
+00018e80: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
+00018e90: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
+00018ea0: 616c 5f69 6e64 6963 6573 290d 0a0d 0a20  al_indices).... 
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00018ec0: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
+00018ed0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
+00018ee0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
+00018ef0: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
+00018f00: 200d 0a20 2020 2023 2054 5a59 5820 7368   ..    # TZYX sh
+00018f10: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
+00018f20: 2069 6620 6e64 696d 203d 3d20 343a 0d0a   if ndim == 4:..
+00018f30: 2020 2020 2020 2020 7072 696e 7428 274d          print('M
+00018f40: 6173 6b73 206d 6164 6520 696e 746f 2061  asks made into a
+00018f50: 2034 4420 6379 6c69 6e64 6572 2c20 7570   4D cylinder, up
+00018f60: 2729 0d0a 2020 2020 2020 2020 626f 756e  ')..        boun
+00018f70: 6461 7279 203d 206e 702e 7a65 726f 7328  dary = np.zeros(
+00018f80: 0d0a 2020 2020 2020 2020 2020 2020 5b6d  ..            [m
+00018f90: 6173 6b2e 7368 6170 655b 305d 2c20 6d61  ask.shape[0], ma
+00018fa0: 736b 2e73 6861 7065 5b31 5d2c 206d 6173  sk.shape[1], mas
+00018fb0: 6b2e 7368 6170 655b 325d 2c20 6d61 736b  k.shape[2], mask
+00018fc0: 2e73 6861 7065 5b33 5d5d 0d0a 2020 2020  .shape[3]]..    
+00018fd0: 2020 2020 290d 0a20 2020 2020 2020 2066      )..        f
+00018fe0: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
+00018ff0: 206d 6173 6b2e 7368 6170 655b 305d 293a   mask.shape[0]):
+00019000: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00019010: 2020 2020 2020 2020 2020 2020 626f 756e              boun
+00019020: 6461 7279 5b69 2c3a 5d20 3d20 6669 6e64  dary[i,:] = find
+00019030: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
+00019040: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
+00019050: 2020 2020 7265 6769 6f6e 6365 6e74 726f      regioncentro
+00019060: 6964 203d 2063 6f6d 7075 7465 5f63 656e  id = compute_cen
+00019070: 7472 6f69 6428 626f 756e 6461 7279 5b69  troid(boundary[i
+00019080: 2c3a 5d29 200d 0a20 2020 2020 2020 2020  ,:]) ..         
+00019090: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+000190a0: 7768 6572 6528 626f 756e 6461 7279 5b69  where(boundary[i
+000190b0: 2c3a 5d20 3e20 3029 0d0a 2020 2020 2020  ,:] > 0)..      
+000190c0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+000190d0: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
+000190e0: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
+000190f0: 6963 6573 2929 2e63 6f70 7928 290d 0a0d  ices)).copy()...
+00019100: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00019110: 206a 2069 6e20 7261 6e67 6528 302c 206c   j in range(0, l
+00019120: 656e 2872 6561 6c5f 696e 6469 6365 7329  en(real_indices)
+00019130: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+00019140: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+00019150: 6e64 6963 6573 5b6a 5d5b 305d 203d 2072  ndices[j][0] = r
+00019160: 6561 6c5f 696e 6469 6365 735b 6a5d 5b30  eal_indices[j][0
+00019170: 5d20 2a20 7a63 616c 6962 7261 7469 6f6e  ] * zcalibration
+00019180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019190: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+000191a0: 6573 5b6a 5d5b 315d 203d 2072 6561 6c5f  es[j][1] = real_
+000191b0: 696e 6469 6365 735b 6a5d 5b31 5d20 2a20  indices[j][1] * 
+000191c0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+000191d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191e0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+000191f0: 5d5b 325d 203d 2072 6561 6c5f 696e 6469  ][2] = real_indi
+00019200: 6365 735b 6a5d 5b32 5d20 2a20 7863 616c  ces[j][2] * xcal
+00019210: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
+00019220: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+00019230: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
+00019240: 6561 6c5f 696e 6469 6365 7329 0d0a 2020  eal_indices)..  
+00019250: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
+00019260: 6d61 736b 5b73 7472 2869 295d 203d 205b  mask[str(i)] = [
+00019270: 7472 6565 2c20 696e 6469 6365 732c 2072  tree, indices, r
+00019280: 6567 696f 6e63 656e 7472 6f69 645d 0d0a  egioncentroid]..
+00019290: 2020 2020 7072 696e 7428 2743 6f6d 7075      print('Compu
+000192a0: 7465 6420 7468 6520 626f 756e 6461 7279  ted the boundary
+000192b0: 2070 6f69 6e74 7327 290d 0a0d 0a20 2020   points')....   
+000192c0: 2072 6574 7572 6e20 7469 6d65 645f 6d61   return timed_ma
+000192d0: 736b 2c20 626f 756e 6461 7279 2020 2020  sk, boundary    
+000192e0: 2020 2020 0d0a 0d0a 6465 6620 636f 6d70      ....def comp
+000192f0: 7574 655f 6365 6e74 726f 6964 2862 696e  ute_centroid(bin
+00019300: 6172 795f 696d 6167 6529 3a0d 0a20 2020  ary_image):..   
+00019310: 2023 2045 6e73 7572 6520 6269 6e61 7279   # Ensure binary
+00019320: 2069 6d61 6765 2069 7320 6120 4e75 6d50   image is a NumP
+00019330: 7920 6172 7261 790d 0a20 2020 2062 696e  y array..    bin
+00019340: 6172 795f 696d 6167 6520 3d20 6e70 2e61  ary_image = np.a
+00019350: 7272 6179 2862 696e 6172 795f 696d 6167  rray(binary_imag
+00019360: 6529 0d0a 0d0a 2020 2020 7768 6974 655f  e)....    white_
+00019370: 7069 7865 6c73 203d 206e 702e 7768 6572  pixels = np.wher
+00019380: 6528 6269 6e61 7279 5f69 6d61 6765 203d  e(binary_image =
+00019390: 3d20 3129 0d0a 2020 2020 6e75 6d5f 7069  = 1)..    num_pi
+000193a0: 7865 6c73 203d 206c 656e 2877 6869 7465  xels = len(white
+000193b0: 5f70 6978 656c 735b 305d 290d 0a0d 0a20  _pixels[0]).... 
+000193c0: 2020 2023 2043 6f6d 7075 7465 2074 6865     # Compute the
+000193d0: 2063 656e 7472 6f69 6420 6f66 2074 6865   centroid of the
+000193e0: 2077 6869 7465 2070 6978 656c 7320 696e   white pixels in
+000193f0: 2074 6865 2062 6f75 6e64 6172 7920 696d   the boundary im
+00019400: 6167 650d 0a20 2020 2063 656e 7472 6f69  age..    centroi
+00019410: 6420 3d20 6e70 2e7a 6572 6f73 2862 696e  d = np.zeros(bin
+00019420: 6172 795f 696d 6167 652e 6e64 696d 290d  ary_image.ndim).
+00019430: 0a20 2020 2066 6f72 2064 696d 2069 6e20  .    for dim in 
+00019440: 7261 6e67 6528 6269 6e61 7279 5f69 6d61  range(binary_ima
+00019450: 6765 2e6e 6469 6d29 3a0d 0a20 2020 2020  ge.ndim):..     
+00019460: 2020 2063 656e 7472 6f69 645b 6469 6d5d     centroid[dim]
+00019470: 203d 2077 6869 7465 5f70 6978 656c 735b   = white_pixels[
+00019480: 6469 6d5d 2e73 756d 2829 202f 206e 756d  dim].sum() / num
+00019490: 5f70 6978 656c 730d 0a0d 0a20 2020 2072  _pixels....    r
+000194a0: 6574 7572 6e20 6365 6e74 726f 6964 0d0a  eturn centroid..
+000194b0: 0d0a 0d0a 0d0a 200d 0a0d 0a64 6566 2067  ...... ....def g
+000194c0: 6574 5f63 7376 5f64 6174 6128 6373 7629  et_csv_data(csv)
+000194d0: 3a0d 0a0d 0a20 2020 2020 2020 2064 6174  :....        dat
+000194e0: 6173 6574 203d 2070 642e 7265 6164 5f63  aset = pd.read_c
+000194f0: 7376 280d 0a20 2020 2020 2020 2020 2020  sv(..           
+00019500: 2063 7376 2c20 6465 6c69 6d69 7465 723d   csv, delimiter=
+00019510: 222c 222c 2065 6e63 6f64 696e 673d 2275  ",", encoding="u
+00019520: 6e69 636f 6465 5f65 7363 6170 6522 2c20  nicode_escape", 
+00019530: 6c6f 775f 6d65 6d6f 7279 3d46 616c 7365  low_memory=False
+00019540: 0d0a 2020 2020 2020 2020 295b 333a 5d0d  ..        )[3:].
+00019550: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
+00019560: 5f69 6e64 6578 203d 2064 6174 6173 6574  _index = dataset
+00019570: 2e69 6e64 6578 0d0a 2020 2020 2020 2020  .index..        
+00019580: 7265 7475 726e 2064 6174 6173 6574 2c20  return dataset, 
+00019590: 6461 7461 7365 745f 696e 6465 780d 0a20  dataset_index.. 
+000195a0: 2020 200d 0a64 6566 2067 6574 5f73 706f     ..def get_spo
+000195b0: 745f 6461 7461 7365 7428 7370 6f74 5f64  t_dataset(spot_d
+000195c0: 6174 6173 6574 2c20 7472 6163 6b5f 616e  ataset, track_an
+000195d0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+000195e0: 2c20 7863 616c 6962 7261 7469 6f6e 2c20  , xcalibration, 
+000195f0: 7963 616c 6962 7261 7469 6f6e 2c20 7a63  ycalibration, zc
+00019600: 616c 6962 7261 7469 6f6e 2c20 4174 7472  alibration, Attr
+00019610: 6962 7574 6542 6f78 6e61 6d65 2c20 6465  ibuteBoxname, de
+00019620: 7465 6374 696f 6e63 6861 6e6e 656c 293a  tectionchannel):
+00019630: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
+00019640: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
+00019650: 2020 706f 7369 7820 3d20 7472 6163 6b5f    posix = track_
+00019660: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+00019670: 7973 5b22 706f 7369 7822 5d0d 0a20 2020  ys["posix"]..   
+00019680: 2020 2020 2070 6f73 6979 203d 2074 7261       posiy = tra
+00019690: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+000196a0: 5f6b 6579 735b 2270 6f73 6979 225d 0d0a  _keys["posiy"]..
+000196b0: 2020 2020 2020 2020 706f 7369 7a20 3d20          posiz = 
+000196c0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+000196d0: 706f 745f 6b65 7973 5b22 706f 7369 7a22  pot_keys["posiz"
+000196e0: 5d0d 0a20 2020 2020 2020 2066 7261 6d65  ]..        frame
+000196f0: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+00019700: 735f 7370 6f74 5f6b 6579 735b 2266 7261  s_spot_keys["fra
+00019710: 6d65 225d 0d0a 2020 2020 2020 2020 0d0a  me"]..        ..
+00019720: 2020 2020 2020 2020 4c6f 6361 7469 6f6e          Location
+00019730: 5820 3d20 280d 0a20 2020 2020 2020 2020  X = (..         
+00019740: 2020 2073 706f 745f 6461 7461 7365 745b     spot_dataset[
+00019750: 706f 7369 785d 2e61 7374 7970 6528 2266  posix].astype("f
+00019760: 6c6f 6174 2229 202f 2078 6361 6c69 6272  loat") / xcalibr
+00019770: 6174 696f 6e0d 0a20 2020 2020 2020 2029  ation..        )
+00019780: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+00019790: 2020 2020 2020 2020 4c6f 6361 7469 6f6e          Location
+000197a0: 5920 3d20 280d 0a20 2020 2020 2020 2020  Y = (..         
+000197b0: 2020 2073 706f 745f 6461 7461 7365 745b     spot_dataset[
+000197c0: 706f 7369 795d 2e61 7374 7970 6528 2266  posiy].astype("f
+000197d0: 6c6f 6174 2229 202f 2079 6361 6c69 6272  loat") / ycalibr
+000197e0: 6174 696f 6e0d 0a20 2020 2020 2020 2029  ation..        )
+000197f0: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+00019800: 2020 2020 2020 2020 4c6f 6361 7469 6f6e          Location
+00019810: 5a20 3d20 280d 0a20 2020 2020 2020 2020  Z = (..         
+00019820: 2020 2073 706f 745f 6461 7461 7365 745b     spot_dataset[
+00019830: 706f 7369 7a5d 2e61 7374 7970 6528 2266  posiz].astype("f
+00019840: 6c6f 6174 2229 202f 207a 6361 6c69 6272  loat") / zcalibr
+00019850: 6174 696f 6e0d 0a20 2020 2020 2020 2029  ation..        )
+00019860: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+00019870: 2020 2020 2020 2020 4c6f 6361 7469 6f6e          Location
+00019880: 5420 3d20 2873 706f 745f 6461 7461 7365  T = (spot_datase
+00019890: 745b 6672 616d 655d 2e61 7374 7970 6528  t[frame].astype(
+000198a0: 2266 6c6f 6174 2229 292e 6173 7479 7065  "float")).astype
+000198b0: 2822 696e 7422 290d 0a20 2020 2020 2020  ("int")..       
+000198c0: 200d 0a0d 0a20 2020 2020 2020 2069 676e   ....        ign
+000198d0: 6f72 655f 7661 6c75 6573 203d 205b 7472  ore_values = [tr
+000198e0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+000198f0: 745f 6b65 7973 5b22 6d65 616e 5f69 6e74  t_keys["mean_int
+00019900: 656e 7369 7479 225d 2c74 7261 636b 5f61  ensity"],track_a
+00019910: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+00019920: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
+00019930: 7479 225d 5d20 0d0a 2020 2020 2020 2020  ty"]] ..        
+00019940: 666f 7220 286b 2c76 2920 696e 2074 7261  for (k,v) in tra
+00019950: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+00019960: 5f6b 6579 732e 6974 656d 7328 293a 0d0a  _keys.items():..
+00019970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019980: 2020 6966 2064 6574 6563 7469 6f6e 6368    if detectionch
+00019990: 616e 6e65 6c20 3d3d 2031 3a0d 0a20 2020  annel == 1:..   
+000199a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199b0: 2020 6966 206b 203d 3d20 226d 6561 6e5f    if k == "mean_
+000199c0: 696e 7465 6e73 6974 795f 6368 3222 3a0d  intensity_ch2":.
+000199d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000199e0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+000199f0: 6520 3d20 7472 6163 6b5f 616e 616c 7973  e = track_analys
+00019a00: 6973 5f73 706f 745f 6b65 7973 5b22 6d65  is_spot_keys["me
+00019a10: 616e 5f69 6e74 656e 7369 7479 225d 0d0a  an_intensity"]..
+00019a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a30: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
+00019a40: 6c75 6573 5b76 616c 7565 5d20 3d20 7370  lues[value] = sp
+00019a50: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
+00019a60: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+00019a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a80: 2020 2020 6966 206b 203d 3d20 2274 6f74      if k == "tot
+00019a90: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
+00019aa0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00019ab0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00019ac0: 616c 7565 203d 2074 7261 636b 5f61 6e61  alue = track_ana
+00019ad0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00019ae0: 2274 6f74 616c 5f69 6e74 656e 7369 7479  "total_intensity
+00019af0: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+00019b00: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00019b10: 6c6c 5661 6c75 6573 5b76 616c 7565 5d20  llValues[value] 
+00019b20: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
+00019b30: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+00019b40: 2920 2020 2020 2020 0d0a 0d0a 2020 2020  )       ....    
+00019b50: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00019b60: 206e 6f74 2069 6e20 6967 6e6f 7265 5f76   not in ignore_v
+00019b70: 616c 7565 733a 0d0a 2020 2020 2020 2020  alues:..        
+00019b80: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00019b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ba0: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+00019bb0: 735b 765d 203d 2073 706f 745f 6461 7461  s[v] = spot_data
+00019bc0: 7365 745b 765d 2e61 7374 7970 6528 2266  set[v].astype("f
+00019bd0: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
+00019be0: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
+00019bf0: 785d 203d 2072 6f75 6e64 284c 6f63 6174  x] = round(Locat
+00019c00: 696f 6e58 2c33 290d 0a20 2020 2020 2020  ionX,3)..       
+00019c10: 2041 6c6c 5661 6c75 6573 5b70 6f73 6979   AllValues[posiy
+00019c20: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
+00019c30: 6f6e 592c 3329 0d0a 2020 2020 2020 2020  onY,3)..        
+00019c40: 416c 6c56 616c 7565 735b 706f 7369 7a5d  AllValues[posiz]
+00019c50: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
+00019c60: 6e5a 2c33 290d 0a20 2020 2020 2020 2041  nZ,3)..        A
+00019c70: 6c6c 5661 6c75 6573 5b66 7261 6d65 5d20  llValues[frame] 
+00019c80: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
+00019c90: 542c 3329 0d0a 2020 2020 2020 2020 4174  T,3)..        At
+00019ca0: 7472 6962 7574 6569 6473 203d 205b 5d0d  tributeids = [].
+00019cb0: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
+00019cc0: 7465 6964 732e 6170 7065 6e64 2841 7474  teids.append(Att
+00019cd0: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
+00019ce0: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
+00019cf0: 6962 7574 656e 616d 6520 696e 2041 6c6c  ibutename in All
+00019d00: 5661 6c75 6573 2e6b 6579 7328 293a 0d0a  Values.keys():..
+00019d10: 2020 2020 2020 2020 2020 2020 2020 4174                At
+00019d20: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
+00019d30: 6428 6174 7472 6962 7574 656e 616d 6529  d(attributename)
+00019d40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00019d50: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+00019d60: 2020 2020 2020 7265 7475 726e 2041 7474        return Att
+00019d70: 7269 6275 7465 6964 732c 2041 6c6c 5661  ributeids, AllVa
+00019d80: 6c75 6573 2020 2020 200d 0a20 2020 200d  lues     ..    .
+00019d90: 0a64 6566 2067 6574 5f74 7261 636b 5f64  .def get_track_d
+00019da0: 6174 6173 6574 2874 7261 636b 5f64 6174  ataset(track_dat
+00019db0: 6173 6574 2c20 7472 6163 6b5f 616e 616c  aset, track_anal
+00019dc0: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
+00019dd0: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
+00019de0: 7261 636b 5f6b 6579 732c 2054 7261 636b  rack_keys, Track
+00019df0: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+00019e00: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
+00019e10: 6c54 7261 636b 5661 6c75 6573 203d 207b  lTrackValues = {
+00019e20: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
+00019e30: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
+00019e40: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+00019e50: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
+00019e60: 2020 2020 5469 6420 3d20 7472 6163 6b5f      Tid = track_
+00019e70: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
+00019e80: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+00019e90: 290d 0a20 2020 2020 2020 0d0a 2020 2020  )..       ..    
+00019ea0: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
+00019eb0: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
+00019ec0: 6964 0d0a 2020 2020 2020 0d0a 2020 2020  id..      ..    
+00019ed0: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
+00019ee0: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+00019ef0: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
+00019f00: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+00019f10: 2020 2020 2020 2020 7820 3d20 7472 6163          x = trac
+00019f20: 6b5f 6461 7461 7365 745b 765d 2e61 7374  k_dataset[v].ast
+00019f30: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+00019f40: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00019f50: 6e76 616c 203d 206d 696e 2878 290d 0a20  nval = min(x).. 
+00019f60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00019f70: 6178 7661 6c20 3d20 6d61 7828 7829 0d0a  axval = max(x)..
+00019f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019f90: 2020 6966 206d 696e 7661 6c20 3e20 3020    if minval > 0 
+00019fa0: 616e 6420 6d61 7876 616c 203c 3d20 313a  and maxval <= 1:
+00019fb0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019fc0: 2020 2020 2020 2020 7820 3d20 7820 2b20          x = x + 
+00019fd0: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
+00019fe0: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+00019ff0: 7565 735b 6b5d 203d 2072 6f75 6e64 2878  ues[k] = round(x
+0001a000: 2c20 3329 0d0a 0d0a 2020 2020 2020 2020  , 3)....        
+0001a010: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001a020: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001a030: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001a040: 732e 6170 7065 6e64 2854 7261 636b 4174  s.append(TrackAt
+0001a050: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
+0001a060: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
+0001a070: 7269 6275 7465 6e61 6d65 2069 6e20 7472  ributename in tr
+0001a080: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+0001a090: 636b 5f6b 6579 732e 6b65 7973 2829 3a0d  ck_keys.keys():.
+0001a0a0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
+0001a0b0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
+0001a0c0: 7070 656e 6428 6174 7472 6962 7574 656e  ppend(attributen
+0001a0d0: 616d 6529 2020 2020 0d0a 2020 2020 0d0a  ame)    ..    ..
+0001a0e0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0001a0f0: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
+0001a100: 2c20 416c 6c54 7261 636b 5661 6c75 6573  , AllTrackValues
+0001a110: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001a120: 6564 6765 735f 6461 7461 7365 7428 6564  edges_dataset(ed
+0001a130: 6765 735f 6461 7461 7365 742c 2065 6467  ges_dataset, edg
+0001a140: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
+0001a150: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+0001a160: 5f73 706f 745f 6b65 7973 2c20 7472 6163  _spot_keys, trac
+0001a170: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001a180: 5f6b 6579 7329 3a0d 0a0d 0a20 2020 2020  _keys):....     
+0001a190: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001a1a0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0001a1b0: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
+0001a1c0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a1d0: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
+0001a1e0: 0a20 2020 2020 2020 2054 6964 203d 2065  .        Tid = e
+0001a1f0: 6467 6573 5f64 6174 6173 6574 5b74 7261  dges_dataset[tra
+0001a200: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
+0001a210: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
+0001a220: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+0001a230: 7265 2854 6964 203d 3d20 3029 0d0a 2020  re(Tid == 0)..  
+0001a240: 2020 2020 2020 6d61 7874 7261 636b 5f69        maxtrack_i
+0001a250: 6420 3d20 6d61 7828 5469 6429 0d0a 2020  d = max(Tid)..  
+0001a260: 2020 2020 2020 636f 6e64 6974 696f 6e5f        condition_
+0001a270: 696e 6469 6365 7320 3d20 6564 6765 735f  indices = edges_
+0001a280: 6461 7461 7365 745f 696e 6465 785b 696e  dataset_index[in
+0001a290: 6469 6365 735d 0d0a 2020 2020 2020 2020  dices]..        
+0001a2a0: 5469 645b 636f 6e64 6974 696f 6e5f 696e  Tid[condition_in
+0001a2b0: 6469 6365 735d 203d 206d 6178 7472 6163  dices] = maxtrac
+0001a2c0: 6b5f 6964 202b 2031 0d0a 2020 2020 2020  k_id + 1..      
+0001a2d0: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
+0001a2e0: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
+0001a2f0: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+0001a300: 6b20 696e 2074 7261 636b 5f61 6e61 6c79  k in track_analy
+0001a310: 7369 735f 6564 6765 735f 6b65 7973 2e76  sis_edges_keys.v
+0001a320: 616c 7565 7328 293a 0d0a 0d0a 2020 2020  alues():....    
+0001a330: 2020 2020 2020 2020 6966 206b 2021 3d20          if k != 
+0001a340: 7472 6163 6b5f 6964 3a0d 0a20 2020 2020  track_id:..     
+0001a350: 2020 2020 2020 2020 2020 2078 203d 2065             x = e
+0001a360: 6467 6573 5f64 6174 6173 6574 5b6b 5d2e  dges_dataset[k].
+0001a370: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001a380: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a390: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001a3a0: 735b 6b5d 203d 2078 2020 200d 0a20 2020  s[k] = x   ..   
+0001a3b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001a3c0: 7265 7475 726e 2041 6c6c 4564 6765 7356  return AllEdgesV
+0001a3d0: 616c 7565 7320 2020 0d0a 2020 2020 0d0a  alues   ..    ..
+0001a3e0: 2020 2020 2020 200d 0a20 2020 200d 0a64         ..    ..d
+0001a3f0: 6566 2073 6361 6c65 5f76 616c 7565 2878  ef scale_value(x
+0001a400: 2c20 7363 616c 6520 3d20 3235 3520 2a20  , scale = 255 * 
+0001a410: 3235 3529 3a0d 0a0d 0a0d 0a20 2020 2020  255):......     
+0001a420: 7265 7475 726e 2078 202a 2073 6361 6c65  return x * scale
+0001a430: 2020 200d 0a20 2020 200d 0a0d 0a0d 0a64     ..    ......d
+0001a440: 6566 2070 726f 625f 7369 676d 6f69 6428  ef prob_sigmoid(
+0001a450: 7829 3a0d 0a20 2020 2072 6574 7572 6e20  x):..    return 
+0001a460: 3120 2d20 6d61 7468 2e65 7870 282d 7829  1 - math.exp(-x)
+0001a470: 0d0a 0d0a 0d0a 6465 6620 616e 6775 6c61  ......def angula
+0001a480: 725f 6368 616e 6765 2876 6563 5f30 2c20  r_change(vec_0, 
+0001a490: 7665 635f 3129 3a0d 0a20 2020 2020 2020  vec_1):..       
+0001a4a0: 200d 0a20 2020 2020 2020 2076 6563 5f30   ..        vec_0
+0001a4b0: 203d 2076 6563 5f30 202f 206e 702e 6c69   = vec_0 / np.li
+0001a4c0: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3029  nalg.norm(vec_0)
+0001a4d0: 0d0a 2020 2020 2020 2020 7665 635f 3120  ..        vec_1 
+0001a4e0: 3d20 7665 635f 3120 2f20 6e70 2e6c 696e  = vec_1 / np.lin
+0001a4f0: 616c 672e 6e6f 726d 2876 6563 5f31 290d  alg.norm(vec_1).
+0001a500: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+0001a510: 206e 702e 6172 6363 6f73 286e 702e 636c   np.arccos(np.cl
+0001a520: 6970 286e 702e 646f 7428 7665 635f 302c  ip(np.dot(vec_0,
+0001a530: 2076 6563 5f31 292c 202d 312e 302c 2031   vec_1), -1.0, 1
+0001a540: 2e30 2929 0d0a 2020 2020 2020 2020 616e  .0))..        an
+0001a550: 676c 6520 3d20 616e 676c 6520 2a20 3138  gle = angle * 18
+0001a560: 3020 2f20 6e70 2e70 690d 0a20 2020 2020  0 / np.pi..     
+0001a570: 2020 2072 6574 7572 6e20 616e 676c 650d     return angle.
+0001a580: 0a20 2020 2020 0d0a 0d0a 6465 6620 6576  .     ....def ev
+0001a590: 616c 5f62 6f6f 6c28 7661 6c75 6529 3a0d  al_bool(value):.
+0001a5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a5b0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+0001a5c0: 7661 6c75 6520 203d 3d20 2754 7275 6527  value  == 'True'
+0001a5d0: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+0001a5e0: 2020 2020 6469 765f 6b65 7920 3d20 5472      div_key = Tr
+0001a5f0: 7565 0d0a 2020 2020 2020 2020 656c 7365  ue..        else
+0001a600: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a610: 2020 2064 6976 5f6b 6579 203d 2046 616c     div_key = Fal
+0001a620: 7365 200d 0a0d 0a20 2020 2020 2020 2072  se ....        r
+0001a630: 6574 7572 6e20 6469 765f 6b65 7920 2020  eturn div_key   
+0001a640: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0001a650: 0a64 6566 2063 6865 636b 5f61 6e64 5f75  .def check_and_u
+0001a660: 7064 6174 655f 6d61 736b 286d 6173 6b2c  pdate_mask(mask,
+0001a670: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
+0001a680: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0001a690: 286d 6173 6b2e 7368 6170 6529 203c 206c  (mask.shape) < l
+0001a6a0: 656e 2869 6d61 6765 2e73 6861 7065 293a  en(image.shape):
+0001a6b0: 0d0a 2020 2020 2020 2020 2020 2020 7570  ..            up
+0001a6c0: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
+0001a6d0: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6f0: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
+0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a710: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001a720: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
+0001a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a740: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
+0001a750: 7065 5b31 5d2c 0d0a 2020 2020 2020 2020  pe[1],..        
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a770: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
+0001a780: 6170 655b 325d 2c0d 0a20 2020 2020 2020  ape[2],..       
+0001a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7a0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
+0001a7b0: 6861 7065 5b33 5d2c 0d0a 2020 2020 2020  hape[3],..      
+0001a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7d0: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+0001a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7f0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0001a800: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+0001a810: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
+0001a820: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
+0001a830: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0001a840: 696e 2072 616e 6765 2830 2c20 7570 6461  in range(0, upda
+0001a850: 7465 5f6d 6173 6b2e 7368 6170 655b 315d  te_mask.shape[1]
+0001a860: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0001a870: 2020 2020 2020 2020 2020 7570 6461 7465            update
+0001a880: 5f6d 6173 6b5b 692c 206a 2c20 3a2c 203a  _mask[i, j, :, :
+0001a890: 5d20 3d20 6d61 736b 5b69 2c20 3a2c 203a  ] = mask[i, :, :
+0001a8a0: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
+0001a8b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a8c0: 2020 7570 6461 7465 5f6d 6173 6b20 3d20    update_mask = 
+0001a8d0: 6d61 736b 0d0a 0d0a 2020 2020 2020 2020  mask....        
+0001a8e0: 7265 7475 726e 2075 7064 6174 655f 6d61  return update_ma
+0001a8f0: 736b 2020 2020 2020 2020 0d0a 2020 2020  sk        ..    
+0001a900: 2020 200d 0a                                ..
```

### Comparing `napatrackmater-3.4.6/napatrackmater/Trackvector.py` & `napatrackmater-3.4.7/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/__init__.py` & `napatrackmater-3.4.7/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/clustering.py` & `napatrackmater-3.4.7/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.4.7/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/fate_mapping.py` & `napatrackmater-3.4.7/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater/pretrained.py` & `napatrackmater-3.4.7/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.4.7/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.4.6
+Version: 3.4.7
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.4.6/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.4.7/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.6/setup.py` & `napatrackmater-3.4.7/setup.py`

 * *Files identical despite different names*

